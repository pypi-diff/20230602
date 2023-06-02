# Comparing `tmp/objwrap-0.0.1-py3-none-any.whl.zip` & `tmp/objwrap-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 4429 bytes, number of entries: 11
+Zip file size: 5010 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      174 b- defN 23-Jun-01 12:13 objwrap/__init__.py
--rw-rw-rw-  2.0 fat     1444 b- defN 23-Jun-01 20:05 objwrap/closure.py
+-rw-rw-rw-  2.0 fat     2397 b- defN 23-Jun-02 07:11 objwrap/closure.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 23-Jun-01 11:50 objwrap/core.py
 -rw-rw-rw-  2.0 fat      259 b- defN 23-Jun-01 13:15 objwrap/wrapper.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-01 11:18 tests/__init__.py
 -rw-rw-rw-  2.0 fat      232 b- defN 23-Jun-01 11:52 tests/test_closed_wrapper.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jun-01 11:33 tests/test_wrapper.py
--rw-rw-rw-  2.0 fat     1643 b- defN 23-Jun-01 20:10 objwrap-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 20:10 objwrap-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-01 20:10 objwrap-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      826 b- defN 23-Jun-01 20:10 objwrap-0.0.1.dist-info/RECORD
-11 files, 10040 bytes uncompressed, 3043 bytes compressed:  69.7%
+-rw-rw-rw-  2.0 fat     2849 b- defN 23-Jun-02 07:40 objwrap-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-02 07:40 objwrap-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-02 07:40 objwrap-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      826 b- defN 23-Jun-02 07:40 objwrap-0.0.2.dist-info/RECORD
+11 files, 12199 bytes uncompressed, 3624 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: tests/test_closed_wrapper.py
 Comment: 
 
 Filename: tests/test_wrapper.py
 Comment: 
 
-Filename: objwrap-0.0.1.dist-info/METADATA
+Filename: objwrap-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: objwrap-0.0.1.dist-info/WHEEL
+Filename: objwrap-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: objwrap-0.0.1.dist-info/top_level.txt
+Filename: objwrap-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: objwrap-0.0.1.dist-info/RECORD
+Filename: objwrap-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## objwrap/closure.py

```diff
@@ -1,37 +1,73 @@
 from objwrap.wrapper import Wrapper
 from typing import Iterable
 from collections.abc import Mapping
 
-class _Future(tuple):
-    pass
+
+class Pending:
+    def __init__(self, method, args, kwargs):
+        self.method = method
+        self.args = args
+        self.kwargs = kwargs
+
+    def __len__(self):
+        return 3
+
+    def __iter__(self):
+        yield self.method
+        yield self.args
+        yield self.kwargs
 
 
 class ClosedWrapper(Wrapper):
     def __before__(self, method, args, kwargs):
-        args = [arg.__value__() if arg.__class__ == self.__class__ else arg for arg in args]
-        kwargs = {k: arg.__value__() if arg.__class__ == self.__class__ else arg for k, arg in kwargs.items()}
-        return method, args, kwargs
+        args = [
+            arg.__value__() if arg.__class__ == self.__class__ else arg for arg in args
+        ]
+        kwargs = {
+            k: arg.__value__() if arg.__class__ == self.__class__ else arg
+            for k, arg in kwargs.items()
+        }
+        return Pending(method, args, kwargs)
+
+    def __unknown__(self, obj, name, args, kwargs):
+        raise NotImplemented("Implement the __unknown__ fallback of __before__")
 
     def __after__(self, obj):
         return self.__class__(obj)
 
     def _wrapmethodcall(self, data):
-        if isinstance(data, _Future):
-            method, args, kwargs = data
+        if isinstance(data, Pending):
+            method, args, kwargs = data.method, data.args, data.kwargs
             return method(*args, **kwargs)
         if isinstance(data, Mapping):
-            return {k: self.__wrapmethodcall__(v) for k, v in data.items()}
+            return {k: self._wrapmethodcall(v) for k, v in data.items()}
         if isinstance(data, Iterable):
-            return (self.__wrapmethodcall__(v) for v in data)
-        raise Exception(f"Invalid _wrapmethodcall unpacking for type {type(data)}. Fix the outputs of __before__")
+            return (self._wrapmethodcall(v) for v in data)
+        raise Exception(
+            f"Invalid _wrapmethodcall unpacking for type {type(data)}. Fix the outputs of __before__ or __unknown__"
+        )
 
     def __wrapattr__(self, obj, name):
-        ret = super().__wrapattr__(obj, name)
-        if not callable(ret):
-            return ret
+        try:
+            ret = super().__wrapattr__(obj, name)
+            if not callable(ret):
+                return ret
+        except AttributeError:
+            ret = None
 
         def method(*args, **kwargs):
-            called_method, args, kwargs = self.__before__(ret, args, kwargs)
-            result = self._wrapmethodcall(_Future((called_method, args, kwargs)))
+            pending = (
+                self.__unknown__(self.__value__(), name, args, kwargs)
+                if ret is None
+                else self.__before__(ret, args, kwargs)
+            )
+            if (
+                not isinstance(pending, Pending)
+                and not isinstance(pending, Mapping)
+                and not isinstance(pending, Iterable)
+            ):
+                pending = Pending(*pending)
+            result = self._wrapmethodcall(pending)
             return self.__after__(result)
+
         return method
```

