# Comparing `tmp/phyloroot-0.0.1.tar.gz` & `tmp/phyloroot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phyloroot-0.0.1.tar", last modified: Fri Jun  2 14:10:53 2023, max compression
+gzip compressed data, was "phyloroot-0.0.2.tar", last modified: Fri Jun  2 14:22:14 2023, max compression
```

## Comparing `phyloroot-0.0.1.tar` & `phyloroot-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:10:53.003476 phyloroot-0.0.1/
--rw-rw-r--   0 remie     (1000) remie     (1000)     1072 2023-06-02 13:57:14.000000 phyloroot-0.0.1/LICENCE
--rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:10:53.003476 phyloroot-0.0.1/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      152 2023-06-02 13:56:35.000000 phyloroot-0.0.1/README.md
--rw-rw-r--   0 remie     (1000) remie     (1000)      684 2023-06-02 14:02:29.000000 phyloroot-0.0.1/pyproject.toml
--rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-02 14:10:53.003476 phyloroot-0.0.1/setup.cfg
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:10:53.003476 phyloroot-0.0.1/src/
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:10:53.003476 phyloroot-0.0.1/src/phyloroot/
--rw-rw-r--   0 remie     (1000) remie     (1000)       22 2023-06-02 14:08:54.000000 phyloroot-0.0.1/src/phyloroot/__init__.py
--rw-rw-r--   0 remie     (1000) remie     (1000)     5398 2023-06-02 14:09:13.000000 phyloroot-0.0.1/src/phyloroot/network_rootability.py
--rw-rw-r--   0 remie     (1000) remie     (1000)    22349 2023-06-02 14:00:41.000000 phyloroot-0.0.1/src/phyloroot/rooting.py
-drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:10:53.003476 phyloroot-0.0.1/src/phyloroot.egg-info/
--rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:10:52.000000 phyloroot-0.0.1/src/phyloroot.egg-info/PKG-INFO
--rw-rw-r--   0 remie     (1000) remie     (1000)      268 2023-06-02 14:10:53.000000 phyloroot-0.0.1/src/phyloroot.egg-info/SOURCES.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-02 14:10:52.000000 phyloroot-0.0.1/src/phyloroot.egg-info/dependency_links.txt
--rw-rw-r--   0 remie     (1000) remie     (1000)       10 2023-06-02 14:10:52.000000 phyloroot-0.0.1/src/phyloroot.egg-info/top_level.txt
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.995552 phyloroot-0.0.2/
+-rw-rw-r--   0 remie     (1000) remie     (1000)     1072 2023-06-02 13:57:14.000000 phyloroot-0.0.2/LICENCE
+-rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:22:14.995552 phyloroot-0.0.2/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)      152 2023-06-02 13:56:35.000000 phyloroot-0.0.2/README.md
+-rw-rw-r--   0 remie     (1000) remie     (1000)      684 2023-06-02 14:21:09.000000 phyloroot-0.0.2/pyproject.toml
+-rw-rw-r--   0 remie     (1000) remie     (1000)       38 2023-06-02 14:22:14.995552 phyloroot-0.0.2/setup.cfg
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.991552 phyloroot-0.0.2/src/
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.991552 phyloroot-0.0.2/src/phyloroot/
+-rw-rw-r--   0 remie     (1000) remie     (1000)       23 2023-06-02 14:18:51.000000 phyloroot-0.0.2/src/phyloroot/__init__.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)     5398 2023-06-02 14:09:13.000000 phyloroot-0.0.2/src/phyloroot/network_rootability.py
+-rw-rw-r--   0 remie     (1000) remie     (1000)    22349 2023-06-02 14:00:41.000000 phyloroot-0.0.2/src/phyloroot/rooting.py
+drwxrwxr-x   0 remie     (1000) remie     (1000)        0 2023-06-02 14:22:14.995552 phyloroot-0.0.2/src/phyloroot.egg-info/
+-rw-rw-r--   0 remie     (1000) remie     (1000)      730 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/PKG-INFO
+-rw-rw-r--   0 remie     (1000) remie     (1000)      268 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/SOURCES.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)        1 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/dependency_links.txt
+-rw-rw-r--   0 remie     (1000) remie     (1000)       10 2023-06-02 14:22:14.000000 phyloroot-0.0.2/src/phyloroot.egg-info/top_level.txt
```

### Comparing `phyloroot-0.0.1/LICENCE` & `phyloroot-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `phyloroot-0.0.1/PKG-INFO` & `phyloroot-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyloroot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for orienting phylogenetic networks in several well-known classes.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/RootingNetworks
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/RootingNetworks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `phyloroot-0.0.1/pyproject.toml` & `phyloroot-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "networkx>=3.1",    
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phyloroot"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Remie Janssen", email="remiejanssen92@gmail.com" },
 ]
 description = "A package for orienting phylogenetic networks in several well-known classes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `phyloroot-0.0.1/src/phyloroot/network_rootability.py` & `phyloroot-0.0.2/src/phyloroot/network_rootability.py`

 * *Files identical despite different names*

### Comparing `phyloroot-0.0.1/src/phyloroot/rooting.py` & `phyloroot-0.0.2/src/phyloroot/rooting.py`

 * *Files identical despite different names*

### Comparing `phyloroot-0.0.1/src/phyloroot.egg-info/PKG-INFO` & `phyloroot-0.0.2/src/phyloroot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phyloroot
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for orienting phylogenetic networks in several well-known classes.
 Author-email: Remie Janssen <remiejanssen92@gmail.com>
 Project-URL: Homepage, https://github.com/RemieJanssen/RootingNetworks
 Project-URL: Bug Tracker, https://github.com/RemieJanssen/RootingNetworks/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

