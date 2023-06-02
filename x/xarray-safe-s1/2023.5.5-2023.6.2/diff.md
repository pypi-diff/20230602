# Comparing `tmp/xarray-safe-s1-2023.5.5.tar.gz` & `tmp/xarray-safe-s1-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-safe-s1-2023.5.5.tar", last modified: Fri May  5 07:19:07 2023, max compression
+gzip compressed data, was "xarray-safe-s1-2023.6.2.tar", last modified: Fri Jun  2 08:50:18 2023, max compression
```

## Comparing `xarray-safe-s1-2023.5.5.tar` & `xarray-safe-s1-2023.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.604241 xarray-safe-s1-2023.5.5/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/_static/css/xsar.css
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/examples/simple_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/safe_s1/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/sentinel1_xml_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/safe_s1/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-05 07:18:44.000000 xarray-safe-s1-2023.5.5/test/test_s1reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:19:07.608241 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:19:07.000000 xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.352232 xarray-safe-s1-2023.6.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/_static/css/xsar.css
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/examples/simple_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/safe_s1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    27910 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42062 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/sentinel1_xml_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/safe_s1/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-02 08:49:47.000000 xarray-safe-s1-2023.6.2/test/test_s1reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:50:18.356232 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 08:50:18.000000 xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/top_level.txt
```

### Comparing `xarray-safe-s1-2023.5.5/.github/workflows/publish.yml` & `xarray-safe-s1-2023.6.2/.github/workflows/publish.yml`

 * *Files 18% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         run: |
           python -m build --sdist --wheel .
       - name: Check the built archives
         run: |
           twine check dist/*
           pip install dist/*.whl
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@0bf742be3ebe032c25dd15117957dc15d0cfc38d
+        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
         with:
           password: ${{ secrets.pypi_token }}
           repository_url: https://upload.pypi.org/legacy/
           verify_metadata: true
```

### Comparing `xarray-safe-s1-2023.5.5/.pre-commit-config.yaml` & `xarray-safe-s1-2023.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/LICENSE` & `xarray-safe-s1-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/PKG-INFO` & `xarray-safe-s1-2023.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-Metadata-Version: 2.1
-Name: xarray-safe-s1
-Version: 2023.5.5
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
-![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
+[![Documentation Status](https://readthedocs.org/projects/xarray-safe-s1/badge/?version=latest)](https://xarray-safe-s1.readthedocs.io/en/latest/?badge=latest)
+
 # xarray-safe-s1
 
 Xarray Sentinel1 python SAFE files reader
 
  
 
 # Install
```

### Comparing `xarray-safe-s1-2023.5.5/README.md` & `xarray-safe-s1-2023.6.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
+Metadata-Version: 2.1
+Name: xarray-safe-s1
+Version: 2023.6.2
+License: MIT
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+[![Documentation Status](https://readthedocs.org/projects/xarray-safe-s1/badge/?version=latest)](https://xarray-safe-s1.readthedocs.io/en/latest/?badge=latest)
+
 # xarray-safe-s1
 
 Xarray Sentinel1 python SAFE files reader
 
  
 
 # Install
```

### Comparing `xarray-safe-s1-2023.5.5/ci/requirements/environment.yaml` & `xarray-safe-s1-2023.6.2/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/Makefile` & `xarray-safe-s1-2023.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/conf.py` & `xarray-safe-s1-2023.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/examples/simple_tutorial.ipynb` & `xarray-safe-s1-2023.6.2/docs/examples/simple_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/index.rst` & `xarray-safe-s1-2023.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/installing.rst` & `xarray-safe-s1-2023.6.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/docs/make.bat` & `xarray-safe-s1-2023.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/pyproject.toml` & `xarray-safe-s1-2023.6.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xarray-safe-s1"
-requires-python = ">= 3.10"
+requires-python = ">= 3.9"
 license = {text = "MIT"}
 dependencies = [
     "geopandas",
     "numpy",
     "xarray",
     "xarray-datatree",
     "lxml",
```

### Comparing `xarray-safe-s1-2023.5.5/safe_s1/metadata.py` & `xarray-safe-s1-2023.6.2/safe_s1/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,20 @@
             xpath_mappings=sentinel1_xml_mappings.xpath_mappings,
             compounds_vars=sentinel1_xml_mappings.compounds_vars,
             namespaces=sentinel1_xml_mappings.namespaces,
             mapper=mapper
         )
 
         self.manifest = 'manifest.safe'
-        self.manifest_attrs = self.xml_parser.get_compound_var(self.manifest, 'safe_attributes')
+        if 'SLC' in self.path or 'GRD' in self.path:
+            self.manifest_attrs = self.xml_parser.get_compound_var(self.manifest, 'safe_attributes_slcgrd')
+        elif 'SL2' in self.path:
+            self.manifest_attrs = self.xml_parser.get_compound_var(self.manifest, 'safe_attributes_sl2')
+        else:
+            raise Exception('case not handled')
 
         self._safe_files = None
         self._multidataset = False
         """True if multi dataset"""
         self._datasets_names = list(self.safe_files['dsid'].sort_index().unique())
         self.xsd_definitions = self.get_annotation_definitions()
         if self.name.endswith(':') and len(self._datasets_names) == 1:
@@ -570,15 +575,15 @@
         """
         tmp = []
         pols = []
         history = []
         for pol_code, xml_file in self.files['noise'].items():
             pol = os.path.basename(xml_file).split('-')[4].upper()
             pols.append(pol)
-            if self.product == 'SLC':
+            if self.product == 'SLC' or self.product=='SL2':
                 noise_lut_azi_raw_ds = self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_slc')
                 history.append(self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_slc', describe=True))
             else:
                 noise_lut_azi_raw_ds = self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_grd')
                 #noise_lut_azi_raw_ds.attrs[f'raw_azi_lut_{pol}'] = \
                 #    self.xml_parser.get_var(xml_file, 'noise.azi.noiseLut')
                 history.append(self.xml_parser.get_compound_var(xml_file, 'noise_lut_azi_raw_grd', describe=True))
```

### Comparing `xarray-safe-s1-2023.5.5/safe_s1/sentinel1_xml_mappings.py` & `xarray-safe-s1-2023.6.2/safe_s1/sentinel1_xml_mappings.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
         'product_type': (scalar, '//s1sarl1:standAloneProductInformation/s1sarl1:productType'),
         'mission': (scalar, '//safe:platform/safe:familyName'),
         'satellite': (scalar, '//safe:platform/safe:number'),
         'start_date': (date_converter, '//safe:acquisitionPeriod/safe:startTime'),
         'stop_date': (date_converter, '//safe:acquisitionPeriod/safe:stopTime'),
         'aux_cal': (scalar,
                     '//metadataSection/metadataObject/metadataWrap/xmlData/safe:processing/safe:resource/safe:processing/safe:resource[@role="AUX_CAL"]/@name'),
+        'aux_cal_sl2': (scalar,'//metadataSection/metadataObject/metadataWrap/xmlData/safe:processing/safe:resource[@role="AUX_CAL"]/@name'),
         'annotation_files': (
             normpath, '/xfdu:XFDU/dataObjectSection/*[@repID="s1Level1ProductSchema"]/byteStream/fileLocation/@href'),
         'measurement_files': (
             normpath,
             '/xfdu:XFDU/dataObjectSection/*[@repID="s1Level1MeasurementSchema"]/byteStream/fileLocation/@href'),
         'noise_files': (
             normpath, '/xfdu:XFDU/dataObjectSection/*[@repID="s1Level1NoiseSchema"]/byteStream/fileLocation/@href'),
@@ -706,26 +707,38 @@
 
 
 # dict of compounds variables.
 # compounds variables are variables composed of several variables.
 # the key is the variable name, and the value is a python structure,
 # where leaves are jmespath in xpath_mappings
 compounds_vars = {
-    'safe_attributes': {
+    'safe_attributes_slcgrd': {
         'ipf_version': 'manifest.ipf_version',
         'swath_type': 'manifest.swath_type',
         'polarizations': 'manifest.polarizations',
         'product_type': 'manifest.product_type',
         'mission': 'manifest.mission',
         'satellite': 'manifest.satellite',
         'start_date': 'manifest.start_date',
         'stop_date': 'manifest.stop_date',
         'footprints': 'manifest.footprints',
         'aux_cal': 'manifest.aux_cal'
     },
+    'safe_attributes_sl2': {
+        'ipf_version': 'manifest.ipf_version',
+        'swath_type': 'manifest.swath_type',
+        'polarizations': 'manifest.polarizations',
+        'product_type': 'manifest.product_type',
+        'mission': 'manifest.mission',
+        'satellite': 'manifest.satellite',
+        'start_date': 'manifest.start_date',
+        'stop_date': 'manifest.stop_date',
+        'footprints': 'manifest.footprints',
+        'aux_cal_sl2': 'manifest.aux_cal_sl2'
+    },
     'files': {
         'func': df_files,
         'args': (
             'manifest.annotation_files', 'manifest.measurement_files', 'manifest.noise_files',
             'manifest.calibration_files')
     },
     'xsd_files': {
```

### Comparing `xarray-safe-s1-2023.5.5/safe_s1/xml_parser.py` & `xarray-safe-s1-2023.6.2/safe_s1/xml_parser.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/test/test_s1reader.py` & `xarray-safe-s1-2023.6.2/test/test_s1reader.py`

 * *Files identical despite different names*

### Comparing `xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/PKG-INFO` & `xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: xarray-safe-s1
-Version: 2023.5.5
+Version: 2023.6.2
 License: MIT
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-![Install test](https://github.com/umr-lops/xsar/actions/workflows/install-test.yml/badge.svg)
+
+[![Documentation Status](https://readthedocs.org/projects/xarray-safe-s1/badge/?version=latest)](https://xarray-safe-s1.readthedocs.io/en/latest/?badge=latest)
+
 # xarray-safe-s1
 
 Xarray Sentinel1 python SAFE files reader
 
  
 
 # Install
```

### Comparing `xarray-safe-s1-2023.5.5/xarray_safe_s1.egg-info/SOURCES.txt` & `xarray-safe-s1-2023.6.2/xarray_safe_s1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

