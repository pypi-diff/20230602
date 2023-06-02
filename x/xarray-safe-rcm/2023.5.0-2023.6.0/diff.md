# Comparing `tmp/xarray-safe-rcm-2023.5.0.tar.gz` & `tmp/xarray-safe-rcm-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-rcm-2023.5.0.tar", last modified: Fri May  5 12:59:12 2023, max compression
+gzip compressed data, was "xarray-safe-rcm-2023.6.0.tar", last modified: Fri Jun  2 09:28:18 2023, max compression
```

## Comparing `xarray-safe-rcm-2023.5.0.tar` & `xarray-safe-rcm-2023.6.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.678566 xarray-safe-rcm-2023.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.678566 xarray-safe-rcm-2023.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.674566 xarray-safe-rcm-2023.5.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.682566 xarray-safe-rcm-2023.5.0/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.682566 xarray-safe-rcm-2023.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.682566 xarray-safe-rcm-2023.5.0/safe_rcm/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/calibrations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/safe_rcm/product/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/product/dicttoolz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/product/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/product/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/product/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/product/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/safe_rcm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/tests/test_product_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-05 12:58:52.000000 xarray-safe-rcm-2023.5.0/safe_rcm/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:59:12.686566 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 12:59:12.000000 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-05 12:59:12.000000 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:59:12.000000 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 12:59:12.000000 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 12:59:12.000000 xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.992341 xarray-safe-rcm-2023.6.0/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:17.996341 xarray-safe-rcm-2023.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/calibrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/product/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/dicttoolz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/product/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.000341 xarray-safe-rcm-2023.6.0/safe_rcm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/tests/test_product_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-02 09:28:03.000000 xarray-safe-rcm-2023.6.0/safe_rcm/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:28:18.004341 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 09:28:17.000000 xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/top_level.txt
```

### Comparing `xarray-safe-rcm-2023.5.0/.github/workflows/pypi.yaml` & `xarray-safe-rcm-2023.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/.pre-commit-config.yaml` & `xarray-safe-rcm-2023.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/LICENSE` & `xarray-safe-rcm-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/docs/conf.py` & `xarray-safe-rcm-2023.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/pyproject.toml` & `xarray-safe-rcm-2023.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "toolz",
     "numpy",
     "xarray",
     "xarray-datatree",
     "lxml",
     "xmlschema",
     "rioxarray",
+    "exceptiongroup; python_version < '3.11'",
 ]
 dynamic = ["version"]
 
 [build-system]
 requires = ["setuptools>=64.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/calibrations.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/calibrations.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/product/dicttoolz.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/product/dicttoolz.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/product/predicates.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/product/predicates.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/product/reader.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/product/reader.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/product/transformers.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/product/transformers.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/product/utils.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/product/utils.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/tests/test_product_utils.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/tests/test_product_utils.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-rcm-2023.5.0/safe_rcm/xml.py` & `xarray-safe-rcm-2023.6.0/safe_rcm/xml.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,53 @@
 import io
 import posixpath
 import re
+from collections import deque
 
 import xmlschema
 from lxml import etree
 from tlz.dicttoolz import keymap
 
 include_re = re.compile(r'\s*<xsd:include schemaLocation="(?P<location>[^"/]+)"\s?/>')
 
 
-def remove_includes(f):
-    text = f.read().decode()
+def remove_includes(text):
     return io.StringIO(include_re.sub("", text))
 
 
-def open_schema(mapper, root, name, *, glob="*.xsd"):
+def extract_includes(text):
+    return include_re.findall(text)
+
+
+def normalize(root, path):
+    if posixpath.isabs(path) or posixpath.dirname(path):
+        return path
+
+    return posixpath.join(root, path)
+
+
+def schema_paths(mapper, root_schema):
+    unvisited = deque([root_schema])
+    visited = []
+    while unvisited:
+        path = unvisited.popleft()
+        visited.append(path)
+
+        text = mapper[path].decode()
+        includes = extract_includes(text)
+
+        current_root = posixpath.dirname(path)
+        normalized = [normalize(current_root, p) for p in includes]
+
+        unvisited.extend([p for p in normalized if p not in visited])
+
+    return visited
+
+
+def open_schema(mapper, schema):
     """fsspec-compatible way to open remote schema files
 
     Parameters
     ----------
     fs : fsspec.filesystem
         pre-instantiated fsspec filesystem instance
     root : str
@@ -29,35 +58,29 @@
         The glob used to find other schema files
 
     Returns
     -------
     xmlschema.XMLSchema
         The opened schema object
     """
-    schema_root = mapper._key_to_str(root)
-    fs = mapper.fs
+    paths = schema_paths(mapper, schema)
+    preprocessed = [remove_includes(mapper[p].decode()) for p in paths]
 
-    urls = sorted(
-        fs.glob(f"{schema_root}/{glob}"), key=lambda u: u.endswith(name), reverse=True
-    )
-    preprocessed = [remove_includes(fs.open(u)) for u in urls]
     return xmlschema.XMLSchema(preprocessed)
 
 
 def read_xml(mapper, path):
     raw_data = mapper[path]
     tree = etree.fromstring(raw_data)
 
     namespaces = keymap(lambda x: x if x is not None else "rcm", tree.nsmap)
     schema_location = tree.xpath("./@xsi:schemaLocation", namespaces=namespaces)[0]
     _, schema_path_ = schema_location.split(" ")
 
     schema_path = posixpath.normpath(
         posixpath.join(posixpath.dirname(path), schema_path_)
     )
-    schema_root, schema_name = posixpath.split(schema_path)
-
-    schema = open_schema(mapper, schema_root, schema_name)
+    schema = open_schema(mapper, schema_path)
 
     decoded = schema.decode(tree)
 
     return decoded
```

### Comparing `xarray-safe-rcm-2023.5.0/xarray_safe_rcm.egg-info/SOURCES.txt` & `xarray-safe-rcm-2023.6.0/xarray_safe_rcm.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ci/requirements/environment.yaml
 docs/conf.py
 docs/index.md
 docs/requirements.txt
 safe_rcm/__init__.py
 safe_rcm/api.py
 safe_rcm/calibrations.py
+safe_rcm/manifest.py
 safe_rcm/xml.py
 safe_rcm/product/dicttoolz.py
 safe_rcm/product/predicates.py
 safe_rcm/product/reader.py
 safe_rcm/product/transformers.py
 safe_rcm/product/utils.py
 safe_rcm/tests/test_product_utils.py
```

