# Comparing `tmp/bike-0.3.1.tar.gz` & `tmp/bike-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.3.1.tar", max compression
+gzip compressed data, was "bike-0.3.2.tar", max compression
```

## Comparing `bike-0.3.1.tar` & `bike-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.1/LICENSE
--rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.1/README.md
--rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.1/bike/__init__.py
--rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.1/bike/controllers.py
--rw-r--r--   0        0        0     2780 2023-05-20 11:23:00.413966 bike-0.3.1/bike/fields.py
--rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.1/bike/models.py
--rw-r--r--   0        0        0      495 2023-05-26 09:59:14.492885 bike-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.2/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.2/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.2/bike/controllers.py
+-rw-r--r--   0        0        0     2995 2023-06-02 10:56:24.512070 bike-0.3.2/bike/fields.py
+-rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.2/bike/models.py
+-rw-r--r--   0        0        0      495 2023-06-02 11:01:56.163636 bike-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.2/PKG-INFO
```

### Comparing `bike-0.3.1/LICENSE` & `bike-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.3.1/README.md` & `bike-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `bike-0.3.1/bike/controllers.py` & `bike-0.3.2/bike/controllers.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.1/bike/fields.py` & `bike-0.3.2/bike/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,27 +59,31 @@
         if self.list:
             value = [
                 self.list_type(**item) if isinstance(item, dict) else self.list_type(item) for item in value
             ]
         elif self.object:
             value = self.list_type(**value) if isinstance(value, dict) else value
         else:
-            match self.type:
-                case int():
+            try:
+                if self.type == int:
                     value = int(value) if value else None
-                case datetime.datetime():
+                elif self.type == datetime.datetime:
                     value = datetime.datetime.strptime(value, '')
-                case datetime.date():
+                elif self.type == datetime.date:
                     value = datetime.datetime.strptime(value, '%Y-%m-%d').date()
-                case float():
+                elif self.type == float:
                     value = float(value)
-                case bool():
+                elif self.type == bool:
                     value = True if value == 'true' else False
-                case str():
+                elif self.type == str:
                     value = str(value)
+                else:
+                    value = self.type(value)
+            except Exception as e:
+                raise Exception(f'Field[{self.name}] - {e}')
         for validator in self.validators_pos:
             value = validator(instance, value)
         return value
 
     def set_validators(self, func: callable, pre: bool):
         if pre:
             self.validators_pre.append(func)
```

### Comparing `bike-0.3.1/bike/models.py` & `bike-0.3.2/bike/models.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.1/PKG-INFO` & `bike-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bike
-Version: 0.3.1
+Version: 0.3.2
 Summary: A lightweight model validator for modern projects.
 Home-page: https://github.com/manasseslima/bike
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

