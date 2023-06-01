# Comparing `tmp/pydantic_view-0.2.2.tar.gz` & `tmp/pydantic_view-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.2.2.tar", max compression
+gzip compressed data, was "pydantic_view-0.2.3.tar", max compression
```

## Comparing `pydantic_view-0.2.2.tar` & `pydantic_view-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.2.2/LICENSE
--rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.000000 pydantic_view-0.2.2/README.md
--rw-r--r--   0        0        0      183 2023-05-10 12:31:33.000000 pydantic_view-0.2.2/pydantic_view/__init__.py
--rw-r--r--   0        0        0     8395 2023-05-18 11:21:26.000000 pydantic_view-0.2.2/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      876 2023-05-18 11:31:57.000000 pydantic_view-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.949673 pydantic_view-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5704 2023-05-07 10:28:55.636831 pydantic_view-0.2.3/README.md
+-rw-r--r--   0        0        0      183 2023-05-10 12:31:33.233976 pydantic_view-0.2.3/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     8425 2023-06-01 22:01:42.960775 pydantic_view-0.2.3/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      876 2023-06-01 22:17:43.001200 pydantic_view-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 pydantic_view-0.2.3/PKG-INFO
```

### Comparing `pydantic_view-0.2.2/LICENSE` & `pydantic_view-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.2/README.md` & `pydantic_view-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.2.2/pydantic_view/pydantic_view.py` & `pydantic_view-0.2.3/pydantic_view/pydantic_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 return name
 
         setattr(view_cls, "__view_name__", ViewNameClsDesc())
         setattr(view_cls, "__view_root_cls__", ViewRootClsDesc())
 
         if config:
             config_cls = type("Config", (__base__.Config,), config)
-            view_cls = type(view_cls_name, (view_cls,), {"Config": config_cls})
+            view_cls = type(view_cls_name, (view_cls,), {"__module__": cls.__module__, "Config": config_cls})
 
         view_cls.__fields__ = {k: v for k, v in view_cls.__fields__.items() if k in include and k not in exclude}
 
         for field_name in optional | optional_not_none:
             if field := view_cls.__fields__.get(field_name):
                 field.required = False
```

### Comparing `pydantic_view-0.2.2/pyproject.toml` & `pydantic_view-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.2.2"
+version = "0.2.3"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.2.2/PKG-INFO` & `pydantic_view-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.2.2
+Version: 0.2.3
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

