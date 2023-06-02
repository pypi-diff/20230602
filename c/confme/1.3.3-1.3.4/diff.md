# Comparing `tmp/confme-1.3.3.tar.gz` & `tmp/confme-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confme-1.3.3.tar", max compression
+gzip compressed data, was "confme-1.3.4.tar", max compression
```

## Comparing `confme-1.3.3.tar` & `confme-1.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1085 2023-06-02 10:05:49.127710 confme-1.3.3/LICENSE
--rw-r--r--   0        0        0     8192 2023-06-02 10:05:49.127710 confme-1.3.3/README.md
--rw-r--r--   0        0        0      238 2023-06-02 10:05:49.127710 confme-1.3.3/confme/__init__.py
--rw-r--r--   0        0        0      550 2023-06-02 10:05:49.127710 confme-1.3.3/confme/annotation.py
--rw-r--r--   0        0        0        0 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/__init__.py
--rw-r--r--   0        0        0     1076 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/argument_overwrite.py
--rw-r--r--   0        0        0     6785 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/base_config.py
--rw-r--r--   0        0        0      728 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/env_overwrite.py
--rw-r--r--   0        0        0     2262 2023-06-02 10:05:49.127710 confme-1.3.3/confme/core/global_config.py
--rw-r--r--   0        0        0    18170 2023-06-02 10:05:49.127710 confme-1.3.3/confme/pylintrc
--rw-r--r--   0        0        0      841 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/__init__.py
--rw-r--r--   0        0        0      728 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/backend_base.py
--rw-r--r--   0        0        0      847 2023-06-02 10:05:49.127710 confme-1.3.3/confme/source_backend/backend_yaml.py
--rw-r--r--   0        0        0        0 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/base_exception.py
--rw-r--r--   0        0        0      974 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/deprecated.py
--rw-r--r--   0        0        0     1099 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/dict_util.py
--rw-r--r--   0        0        0      832 2023-06-02 10:05:49.127710 confme-1.3.3/confme/utils/typing.py
--rw-r--r--   0        0        0     1353 2023-06-02 10:05:49.127710 confme-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     9443 1970-01-01 00:00:00.000000 confme-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-02 10:57:07.714049 confme-1.3.4/LICENSE
+-rw-r--r--   0        0        0     8192 2023-06-02 10:57:07.714049 confme-1.3.4/README.md
+-rw-r--r--   0        0        0      238 2023-06-02 10:57:07.714049 confme-1.3.4/confme/__init__.py
+-rw-r--r--   0        0        0      550 2023-06-02 10:57:07.714049 confme-1.3.4/confme/annotation.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/__init__.py
+-rw-r--r--   0        0        0     1076 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/argument_overwrite.py
+-rw-r--r--   0        0        0     6810 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/base_config.py
+-rw-r--r--   0        0        0      728 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/env_overwrite.py
+-rw-r--r--   0        0        0     2262 2023-06-02 10:57:07.714049 confme-1.3.4/confme/core/global_config.py
+-rw-r--r--   0        0        0    18170 2023-06-02 10:57:07.714049 confme-1.3.4/confme/pylintrc
+-rw-r--r--   0        0        0      841 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/backend_base.py
+-rw-r--r--   0        0        0      847 2023-06-02 10:57:07.714049 confme-1.3.4/confme/source_backend/backend_yaml.py
+-rw-r--r--   0        0        0        0 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/base_exception.py
+-rw-r--r--   0        0        0      974 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/deprecated.py
+-rw-r--r--   0        0        0     1099 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/dict_util.py
+-rw-r--r--   0        0        0      832 2023-06-02 10:57:07.714049 confme-1.3.4/confme/utils/typing.py
+-rw-r--r--   0        0        0     1353 2023-06-02 10:57:07.714049 confme-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9443 1970-01-01 00:00:00.000000 confme-1.3.4/PKG-INFO
```

### Comparing `confme-1.3.3/LICENSE` & `confme-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/README.md` & `confme-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/annotation.py` & `confme-1.3.4/confme/annotation.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/core/argument_overwrite.py` & `confme-1.3.4/confme/core/argument_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/core/base_config.py` & `confme-1.3.4/confme/core/base_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         return cls._cache[env]
 
     @classmethod
     def _load_file(cls, environment: str) -> T:
         files = Path(cls._config_path).glob(pattern='*')
         if cls._strict:
-            selected_files = [f for f in files if f.name == environment]
+            selected_files = [f for f in files if f.name == environment or f.stem == environment]
         else:
             selected_files = [f for f in files if environment in f.name]
 
         if len(selected_files) <= 0:
             raise ConfmeException(f'No configuration found for environment {environment} in '
                                   f'files {files}')
         elif len(selected_files) > 1:
```

### Comparing `confme-1.3.3/confme/core/env_overwrite.py` & `confme-1.3.4/confme/core/env_overwrite.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/core/global_config.py` & `confme-1.3.4/confme/core/global_config.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/pylintrc` & `confme-1.3.4/confme/pylintrc`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/source_backend/__init__.py` & `confme-1.3.4/confme/source_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/source_backend/backend_base.py` & `confme-1.3.4/confme/source_backend/backend_base.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/source_backend/backend_yaml.py` & `confme-1.3.4/confme/source_backend/backend_yaml.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/utils/deprecated.py` & `confme-1.3.4/confme/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/utils/dict_util.py` & `confme-1.3.4/confme/utils/dict_util.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/confme/utils/typing.py` & `confme-1.3.4/confme/utils/typing.py`

 * *Files identical despite different names*

### Comparing `confme-1.3.3/pyproject.toml` & `confme-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confme"
-version = "1.3.3"
+version = "1.3.4"
 description = "Easy configuration management in python"
 authors = ["Iwan Silvan Bolzern <iwan.bolzern@roche.com>"]
 license = "LICENSE"
 readme = "README.md"
 homepage = "https://github.com/iwanbolzern/confme"
 repository = "https://github.com/iwanbolzern/confme"
 classifiers = [
```

### Comparing `confme-1.3.3/PKG-INFO` & `confme-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confme
-Version: 1.3.3
+Version: 1.3.4
 Summary: Easy configuration management in python
 Home-page: https://github.com/iwanbolzern/confme
 License: LICENSE
 Author: Iwan Silvan Bolzern
 Author-email: iwan.bolzern@roche.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

