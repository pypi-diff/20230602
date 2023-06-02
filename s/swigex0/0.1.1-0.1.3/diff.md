# Comparing `tmp/swigex0-0.1.1-cp39-cp39-win_amd64.whl.zip` & `tmp/swigex0-0.1.3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 53877 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     8260 b- defN 23-May-23 22:49 swigex0-0.1.1.data/purelib/swigex0/__init__.py
--rw-rw-rw-  2.0 fat   138240 b- defN 23-May-23 22:49 swigex0-0.1.1.data/purelib/swigex0/_swigex0.pyd
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-23 22:49 swigex0-0.1.1.data/purelib/swigex0/version.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-May-23 22:50 swigex0-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-23 22:50 swigex0-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-23 22:49 swigex0-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      607 b- defN 23-May-23 22:50 swigex0-0.1.1.dist-info/RECORD
-7 files, 148335 bytes uncompressed, 52791 bytes compressed:  64.4%
+Zip file size: 54503 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     8344 b- defN 23-Jun-02 11:39 swigex0-0.1.3.data/purelib/swigex0/__init__.py
+-rw-rw-rw-  2.0 fat   139264 b- defN 23-Jun-02 11:39 swigex0-0.1.3.data/purelib/swigex0/_swigex0.pyd
+-rw-rw-rw-  2.0 fat       50 b- defN 23-Jun-02 11:39 swigex0-0.1.3.data/purelib/swigex0/version.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-02 11:39 swigex0-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-02 11:39 swigex0-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-02 11:39 swigex0-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      607 b- defN 23-Jun-02 11:39 swigex0-0.1.3.dist-info/RECORD
+7 files, 149443 bytes uncompressed, 53417 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: swigex0-0.1.1.data/purelib/swigex0/__init__.py
+Filename: swigex0-0.1.3.data/purelib/swigex0/__init__.py
 Comment: 
 
-Filename: swigex0-0.1.1.data/purelib/swigex0/_swigex0.pyd
+Filename: swigex0-0.1.3.data/purelib/swigex0/_swigex0.pyd
 Comment: 
 
-Filename: swigex0-0.1.1.data/purelib/swigex0/version.py
+Filename: swigex0-0.1.3.data/purelib/swigex0/version.py
 Comment: 
 
-Filename: swigex0-0.1.1.dist-info/METADATA
+Filename: swigex0-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: swigex0-0.1.1.dist-info/WHEEL
+Filename: swigex0-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: swigex0-0.1.1.dist-info/top_level.txt
+Filename: swigex0-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: swigex0-0.1.1.dist-info/RECORD
+Filename: swigex0-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `swigex0-0.1.1.data/purelib/swigex0/__init__.py` & `swigex0-0.1.3.data/purelib/swigex0/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,16 +244,19 @@
 
     def resetFromFiboRef(self, fib):
         return _swigex0.Fibo_resetFromFiboRef(self, fib)
 
     def display(self, showTitle=True):
         return _swigex0.Fibo_display(self, showTitle)
 
-    def get(self):
-        return _swigex0.Fibo_get(self)
+    def getVector(self):
+        return _swigex0.Fibo_getVector(self)
+
+    def getTitle(self):
+        return _swigex0.Fibo_getTitle(self)
 
 # Register Fibo in _swigex0:
 _swigex0.Fibo_swigregister(Fibo)
 class StdoutRedirect(object):
     thisown = property(lambda x: x.this.own(), lambda x, v: x.this.own(v), doc="The membership flag")
     __repr__ = _swig_repr
```

## Comparing `swigex0-0.1.1.dist-info/METADATA` & `swigex0-0.1.3.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swigex0
-Version: 0.1.1
+Version: 0.1.3
 Summary: C++ library and SWIG wrappers (R & Python)
 Home-page: https://github.com/fabien-ors/swigex
 Author: Fabien Ors
 Author-email: fabien.ors@minesparis.psl.eu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/fabien-ors/swigex/issues
 Platform: UNKNOWN
```

