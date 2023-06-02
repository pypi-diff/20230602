# Comparing `tmp/sdss-access-2.0.5.tar.gz` & `tmp/sdss-access-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sdss-access-2.0.5.tar", last modified: Wed Nov 30 23:28:41 2022, max compression
+gzip compressed data, was "dist/sdss-access-2.0.6.tar", last modified: Fri Jun  2 14:11:18 2023, max compression
```

## Comparing `sdss-access-2.0.5.tar` & `sdss-access-2.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1504 2022-11-30 23:28:28.000000 sdss-access-2.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)       44 2022-11-30 23:28:28.000000 sdss-access-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2022-11-30 23:28:41.000000 sdss-access-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2022-11-30 23:28:28.000000 sdss-access-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access/
--rw-r--r--   0 runner    (1001) docker     (122)      814 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access/etc/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/etc/sdss_access.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access/misc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7376 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/misc/docupaths.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access/path/
--rw-r--r--   0 runner    (1001) docker     (122)       46 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2578 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/path/changelog.py
--rw-r--r--   0 runner    (1001) docker     (122)    48388 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/path/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access/sync/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      598 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/access.py
--rw-r--r--   0 runner    (1001) docker     (122)     4772 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7722 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/baseaccess.py
--rw-r--r--   0 runner    (1001) docker     (122)     8069 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     9674 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/curl.py
--rw-r--r--   0 runner    (1001) docker     (122)     4851 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     3065 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/rsync.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/stream.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3378 2022-11-30 23:28:28.000000 sdss-access-2.0.5/python/sdss_access/sync/system_call.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2493 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      890 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      608 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2022-11-30 23:28:41.000000 sdss-access-2.0.5/python/sdss_access.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2347 2022-11-30 23:28:41.000000 sdss-access-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       72 2022-11-30 23:28:28.000000 sdss-access-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-02 14:11:05.000000 sdss-access-2.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 14:11:05.000000 sdss-access-2.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-02 14:11:18.000000 sdss-access-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-02 14:11:05.000000 sdss-access-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/etc/sdss_access.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/misc/docupaths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/path/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49019 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/path/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/baseaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/rsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3378 2023-06-02 14:11:05.000000 sdss-access-2.0.6/python/sdss_access/sync/system_call.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:11:18.000000 sdss-access-2.0.6/python/sdss_access.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 14:11:18.000000 sdss-access-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-02 14:11:05.000000 sdss-access-2.0.6/setup.py
```

### Comparing `sdss-access-2.0.5/LICENSE.md` & `sdss-access-2.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/PKG-INFO` & `sdss-access-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-access
-Version: 2.0.5
+Version: 2.0.6
 Summary: Package to dynamically build filepaths and access all SDSS SAS products
 Home-page: https://github.com/sdss/sdss_access
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdss_access
 Project-URL: Documentation, https://sdss-access.readthedocs.org
```

### Comparing `sdss-access-2.0.5/README.md` & `sdss-access-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/__init__.py` & `sdss-access-2.0.6/python/sdss_access/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/misc/docupaths.py` & `sdss-access-2.0.6/python/sdss_access/misc/docupaths.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/path/changelog.py` & `sdss-access-2.0.6/python/sdss_access/path/changelog.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/path/path.py` & `sdss-access-2.0.6/python/sdss_access/path/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1358,14 +1358,36 @@
         '''
 
         configid = kwargs.get('configid', None)
         if not configid:
             return '0000XX'
         return '{:0>4d}XX'.format(int(configid) // 100)
 
+    def configsubmodule(self, filetype, **kwargs):
+        ''' Returns configuration summary submodule group subdirectory
+
+        Parameters
+        ----------
+        filetype : str
+            File type parameter.
+        configid : int or str
+            Configuration ID number.  Will be converted to int internally.
+
+        Returns
+        -------
+        configsubmodule : str
+            Configuration submodule directory in the format ``NNNXXX``.
+
+        '''
+
+        configid = kwargs.get('configid', None)
+        if not configid:
+            return '000XXX'
+        return '{:0>3d}XXX'.format(int(configid) // 1000)
+
     def isplate(self, filetype, **kwargs):
         ''' Returns the plate flag for BOSS idlspec2d run2d versions that utilize it
 
         Parameters
         ---------
         filetype : str
             File type paramter
```

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/access.py` & `sdss-access-2.0.6/python/sdss_access/sync/access.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/auth.py` & `sdss-access-2.0.6/python/sdss_access/sync/auth.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/baseaccess.py` & `sdss-access-2.0.6/python/sdss_access/sync/baseaccess.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/cli.py` & `sdss-access-2.0.6/python/sdss_access/sync/cli.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/curl.py` & `sdss-access-2.0.6/python/sdss_access/sync/curl.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/http.py` & `sdss-access-2.0.6/python/sdss_access/sync/http.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/rsync.py` & `sdss-access-2.0.6/python/sdss_access/sync/rsync.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/stream.py` & `sdss-access-2.0.6/python/sdss_access/sync/stream.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access/sync/system_call.py` & `sdss-access-2.0.6/python/sdss_access/sync/system_call.py`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access.egg-info/PKG-INFO` & `sdss-access-2.0.6/python/sdss_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-access
-Version: 2.0.5
+Version: 2.0.6
 Summary: Package to dynamically build filepaths and access all SDSS SAS products
 Home-page: https://github.com/sdss/sdss_access
 Author: Brian Cherinka
 Author-email: bcherinka@stsci.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/sdss_access
 Project-URL: Documentation, https://sdss-access.readthedocs.org
```

### Comparing `sdss-access-2.0.5/python/sdss_access.egg-info/SOURCES.txt` & `sdss-access-2.0.6/python/sdss_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-access-2.0.5/python/sdss_access.egg-info/requires.txt` & `sdss-access-2.0.6/python/sdss_access.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 six>=1.11
 requests>=2.10.0
-sdss-tree>=3.1.2
+sdss-tree<4.0.0,>=3.1.2
 sdsstools>=0.4.5
 tqdm>=4.46.0
 
 [dev]
 Sphinx>=2.1.0
 sphinx_bootstrap_theme>=0.4.12
 recommonmark>=0.6
```

### Comparing `sdss-access-2.0.5/setup.cfg` & `sdss-access-2.0.6/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-access
-version = 2.0.5
+version = 2.0.6
 author = Brian Cherinka
 author_email = bcherinka@stsci.edu
 description = Package to dynamically build filepaths and access all SDSS SAS products
 url = https://github.com/sdss/sdss_access
 project_urls = 
 	Repository = https://github.com/sdss/sdss_access
 	Documentation = https://sdss-access.readthedocs.org
@@ -30,15 +30,15 @@
 python_requires = >=3.6
 packages = find:
 package_dir = 
 	= python
 install_requires = 
 	six>=1.11
 	requests>=2.10.0
-	sdss-tree>=3.1.2
+	sdss-tree>=3.1.2,<4.0.0
 	sdsstools>=0.4.5
 	tqdm>=4.46.0
 scripts = 
 
 [options.packages.find]
 where = 
 	python
```

