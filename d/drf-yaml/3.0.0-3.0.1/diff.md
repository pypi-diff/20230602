# Comparing `tmp/drf_yaml-3.0.0.tar.gz` & `tmp/drf_yaml-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_yaml-3.0.0.tar", max compression
+gzip compressed data, was "drf_yaml-3.0.1.tar", max compression
```

## Comparing `drf_yaml-3.0.0.tar` & `drf_yaml-3.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1520 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/LICENSE
--rw-r--r--   0        0        0     2051 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/README.md
--rw-r--r--   0        0        0       69 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/__init__.py
--rw-r--r--   0        0        0     4185 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/encoders.py
--rw-r--r--   0        0        0     1918 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/fields.py
--rw-r--r--   0        0        0     1197 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/parsers.py
--rw-r--r--   0        0        0        0 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/py.typed
--rw-r--r--   0        0        0     1044 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/renderers.py
--rw-r--r--   0        0        0      646 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/drf_yaml/styles.py
--rw-r--r--   0        0        0     2446 2023-06-02 03:30:17.346335 drf_yaml-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 drf_yaml-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1979 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/README.md
+-rw-r--r--   0        0        0       69 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/__init__.py
+-rw-r--r--   0        0        0     4185 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/encoders.py
+-rw-r--r--   0        0        0     1908 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/fields.py
+-rw-r--r--   0        0        0     1197 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/parsers.py
+-rw-r--r--   0        0        0        0 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/py.typed
+-rw-r--r--   0        0        0     1044 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/renderers.py
+-rw-r--r--   0        0        0      646 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/drf_yaml/styles.py
+-rw-r--r--   0        0        0     2428 2023-06-02 06:36:50.101691 drf_yaml-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3197 1970-01-01 00:00:00.000000 drf_yaml-3.0.1/PKG-INFO
```

### Comparing `drf_yaml-3.0.0/LICENSE` & `drf_yaml-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_yaml-3.0.0/README.md` & `drf_yaml-3.0.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # REST Framework YAML
 
 ![build-status-image]
 [![pypi-version]][pypi]
 
 **YAML support for Django REST Framework**
 
-Full documentation for the project is available at [http://qu4tro.github.io/django-rest-framework-yaml][docs].
+Full documentation for the project is available at [http://qu4tro.github.io/drf-yaml][docs].
 
 ## Overview
 
 YAML support for the Django REST Framework, forked from [https://github.com/jpadilla/django-rest-framework-yaml][original].
 
 ## Requirements
 
@@ -68,15 +68,15 @@
   is_staff: true
   url: "http://127.0.0.1:8000/users/1/"
   username: jpadilla
 ```
 
 ## Documentation & Support
 
-Full documentation for the project is available at [http://qu4tro.github.io/django-rest-framework-yaml][docs].
+Full documentation for the project is available at [http://qu4tro.github.io/drf-yaml][docs].
 
 
-[build-status-image]: https://img.shields.io/github/checks-status/Qu4tro/django-rest-framework-yaml/main
+[build-status-image]: https://img.shields.io/github/checks-status/Qu4tro/drf-yaml/main
 [pypi-version]: https://img.shields.io/pypi/v/drf-yaml.svg
 [pypi]: https://pypi.python.org/pypi/drf-yaml
-[docs]: http://qu4tro.github.io/django-rest-framework-yaml
+[docs]: http://qu4tro.github.io/drf-yaml
 [original]: https://github.com/jpadilla/django-rest-framework-yaml
```

### Comparing `drf_yaml-3.0.0/drf_yaml/encoders.py` & `drf_yaml-3.0.1/drf_yaml/encoders.py`

 * *Files identical despite different names*

### Comparing `drf_yaml-3.0.0/drf_yaml/fields.py` & `drf_yaml-3.0.1/drf_yaml/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,48 +11,48 @@
 
 
 class FlowStyleDictField(fields.DictField):
     """A DRF field which renders as a YAML flow style mapping."""
 
     def to_representation(self, value: Any) -> dict[Any, Any]:
         """Render a flow style mapping."""
-        return styles.flow_style_mapping(super().to_representation(value))
+        return styles.FlowStyleMapping(super().to_representation(value))
 
 
 class FlowStyleListField(fields.ListField):
     """A DRF field which renders as a YAML flow style sequence."""
 
     def to_representation(self, value: Any) -> list[Any]:
         """Render a flow style sequence."""
-        return styles.flow_style_sequence(super().to_representation(value))
+        return styles.FlowStyleSequence(super().to_representation(value))
 
 
 class SingleQuotedCharField(fields.CharField):
     """A DRF field which renders as a YAML single quoted string."""
 
     def to_representation(self, value: Any) -> str:
         """Render a single quoted string."""
-        return styles.single_quoted_str(super().to_representation(value))
+        return styles.SingleQuotedStr(super().to_representation(value))
 
 
 class DoubleQuotedCharField(fields.CharField):
     """A DRF field which renders as a YAML double quoted string."""
 
     def to_representation(self, value: Any) -> str:
         """Render a double quoted string."""
-        return styles.double_quoted_str(super().to_representation(value))
+        return styles.DoubleQuotedStr(super().to_representation(value))
 
 
 class FoldedCharField(fields.CharField):
     """A DRF field which renders as a YAML folded string."""
 
     def to_representation(self, value: Any) -> str:
         """Render a folded string."""
-        return styles.folded_str(super().to_representation(value))
+        return styles.FoldedStr(super().to_representation(value))
 
 
 class LiteralCharField(fields.CharField):
     """A DRF field which renders as a YAML literal string."""
 
     def to_representation(self, value: Any) -> str:
         """Render a literal string."""
-        return styles.literal_str(super().to_representation(value))
+        return styles.LiteralStr(super().to_representation(value))
```

### Comparing `drf_yaml-3.0.0/drf_yaml/parsers.py` & `drf_yaml-3.0.1/drf_yaml/parsers.py`

 * *Files identical despite different names*

### Comparing `drf_yaml-3.0.0/drf_yaml/renderers.py` & `drf_yaml-3.0.1/drf_yaml/renderers.py`

 * *Files identical despite different names*

### Comparing `drf_yaml-3.0.0/drf_yaml/styles.py` & `drf_yaml-3.0.1/drf_yaml/styles.py`

 * *Files identical despite different names*

### Comparing `drf_yaml-3.0.0/pyproject.toml` & `drf_yaml-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "drf-yaml"
-version = "3.0.0"
+version = "3.0.1"
 description = "YAML support for Django REST Framework"
 authors = [
     "José Padilla <hello@jpadilla.com>",
     "Xavier Francisco <xavier.n.francisco@gmail.com>",
 ]
 license = "BSD"
 readme = "README.md"
-homepage = "https://github.com/Qu4tro/django-rest-framework-yaml"
+homepage = "https://github.com/Qu4tro/drf-yaml"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
```

### Comparing `drf_yaml-3.0.0/PKG-INFO` & `drf_yaml-3.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: drf-yaml
-Version: 3.0.0
+Version: 3.0.1
 Summary: YAML support for Django REST Framework
-Home-page: https://github.com/Qu4tro/django-rest-framework-yaml
+Home-page: https://github.com/Qu4tro/drf-yaml
 License: BSD
 Author: José Padilla
 Author-email: hello@jpadilla.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,15 +32,15 @@
 # REST Framework YAML
 
 ![build-status-image]
 [![pypi-version]][pypi]
 
 **YAML support for Django REST Framework**
 
-Full documentation for the project is available at [http://qu4tro.github.io/django-rest-framework-yaml][docs].
+Full documentation for the project is available at [http://qu4tro.github.io/drf-yaml][docs].
 
 ## Overview
 
 YAML support for the Django REST Framework, forked from [https://github.com/jpadilla/django-rest-framework-yaml][original].
 
 ## Requirements
 
@@ -99,16 +99,16 @@
   is_staff: true
   url: "http://127.0.0.1:8000/users/1/"
   username: jpadilla
 ```
 
 ## Documentation & Support
 
-Full documentation for the project is available at [http://qu4tro.github.io/django-rest-framework-yaml][docs].
+Full documentation for the project is available at [http://qu4tro.github.io/drf-yaml][docs].
 
 
-[build-status-image]: https://img.shields.io/github/checks-status/Qu4tro/django-rest-framework-yaml/main
+[build-status-image]: https://img.shields.io/github/checks-status/Qu4tro/drf-yaml/main
 [pypi-version]: https://img.shields.io/pypi/v/drf-yaml.svg
 [pypi]: https://pypi.python.org/pypi/drf-yaml
-[docs]: http://qu4tro.github.io/django-rest-framework-yaml
+[docs]: http://qu4tro.github.io/drf-yaml
 [original]: https://github.com/jpadilla/django-rest-framework-yaml
```

