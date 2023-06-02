# Comparing `tmp/format-oc-1.6.1.tar.gz` & `tmp/format-oc-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "format-oc-1.6.1.tar", last modified: Mon Feb 13 16:39:32 2023, max compression
+gzip compressed data, was "format-oc-1.6.2.tar", last modified: Fri Jun  2 10:51:47 2023, max compression
```

## Comparing `format-oc-1.6.1.tar` & `format-oc-1.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-02-13 16:39:32.518592 format-oc-1.6.1/
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-02-13 16:39:32.514592 format-oc-1.6.1/FormatOC/
--rw-rw-r--   0 bast      (1002) bast      (1002)     2463 2022-05-20 13:42:04.000000 format-oc-1.6.1/FormatOC/JSON.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    60859 2023-02-13 16:12:41.000000 format-oc-1.6.1/FormatOC/__init__.py
--rw-r--r--   0 bast      (1002) bast      (1002)    11357 2021-06-08 11:57:56.000000 format-oc-1.6.1/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)     1022 2023-02-13 16:39:32.518592 format-oc-1.6.1/PKG-INFO
--rw-r--r--   0 bast      (1002) bast      (1002)      259 2021-06-08 11:57:56.000000 format-oc-1.6.1/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-02-13 16:39:32.514592 format-oc-1.6.1/format_oc.egg-info/
--rwxr-xr-x   0 bast      (1002) bast      (1002)     1022 2023-02-13 16:39:32.000000 format-oc-1.6.1/format_oc.egg-info/PKG-INFO
--rwxr-xr-x   0 bast      (1002) bast      (1002)      266 2023-02-13 16:39:32.000000 format-oc-1.6.1/format_oc.egg-info/SOURCES.txt
--rwxr-xr-x   0 bast      (1002) bast      (1002)        1 2023-02-13 16:39:32.000000 format-oc-1.6.1/format_oc.egg-info/dependency_links.txt
--rwxr-xr-x   0 bast      (1002) bast      (1002)        7 2023-02-13 16:39:32.000000 format-oc-1.6.1/format_oc.egg-info/requires.txt
--rwxr-xr-x   0 bast      (1002) bast      (1002)        9 2023-02-13 16:39:32.000000 format-oc-1.6.1/format_oc.egg-info/top_level.txt
--rwxr-xr-x   0 bast      (1002) bast      (1002)        1 2021-06-08 11:57:56.000000 format-oc-1.6.1/format_oc.egg-info/zip-safe
--rw-r--r--   0 bast      (1002) bast      (1002)       79 2023-02-13 16:39:32.518592 format-oc-1.6.1/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)      976 2023-02-13 16:03:48.000000 format-oc-1.6.1/setup.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:51:47.547439 format-oc-1.6.2/
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:51:47.547439 format-oc-1.6.2/FormatOC/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     2463 2022-05-20 13:42:04.000000 format-oc-1.6.2/FormatOC/JSON.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)    60882 2023-06-02 10:51:32.000000 format-oc-1.6.2/FormatOC/__init__.py
+-rw-r--r--   0 bast      (1002) bast      (1002)    11357 2021-06-08 11:57:56.000000 format-oc-1.6.2/LICENSE
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1022 2023-06-02 10:51:47.547439 format-oc-1.6.2/PKG-INFO
+-rw-r--r--   0 bast      (1002) bast      (1002)      259 2021-06-08 11:57:56.000000 format-oc-1.6.2/README.md
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:51:47.547439 format-oc-1.6.2/format_oc.egg-info/
+-rwxr-xr-x   0 bast      (1002) bast      (1002)     1022 2023-06-02 10:51:47.000000 format-oc-1.6.2/format_oc.egg-info/PKG-INFO
+-rwxr-xr-x   0 bast      (1002) bast      (1002)      266 2023-06-02 10:51:47.000000 format-oc-1.6.2/format_oc.egg-info/SOURCES.txt
+-rwxr-xr-x   0 bast      (1002) bast      (1002)        1 2023-06-02 10:51:47.000000 format-oc-1.6.2/format_oc.egg-info/dependency_links.txt
+-rwxr-xr-x   0 bast      (1002) bast      (1002)        7 2023-06-02 10:51:47.000000 format-oc-1.6.2/format_oc.egg-info/requires.txt
+-rwxr-xr-x   0 bast      (1002) bast      (1002)        9 2023-06-02 10:51:47.000000 format-oc-1.6.2/format_oc.egg-info/top_level.txt
+-rwxr-xr-x   0 bast      (1002) bast      (1002)        1 2021-06-08 11:57:56.000000 format-oc-1.6.2/format_oc.egg-info/zip-safe
+-rw-r--r--   0 bast      (1002) bast      (1002)       79 2023-06-02 10:51:47.547439 format-oc-1.6.2/setup.cfg
+-rw-rw-r--   0 bast      (1002) bast      (1002)      976 2023-06-02 10:51:32.000000 format-oc-1.6.2/setup.py
```

### Comparing `format-oc-1.6.1/FormatOC/JSON.py` & `format-oc-1.6.2/FormatOC/JSON.py`

 * *Files identical despite different names*

### Comparing `format-oc-1.6.1/FormatOC/__init__.py` & `format-oc-1.6.2/FormatOC/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,15 +585,15 @@
 			try:
 				lValues.append(self._node.clean(value[i], lLevel))
 			except ValueError as e:
 				lErrors.extend(e.args[0])
 
 		# If there's any errors
 		if lErrors:
-			raise lErrors
+			raise ValueError(lErrors)
 
 		# Return the cleaned list
 		return lValues
 
 	def minmax(self, minimum=None, maximum=None):
 		"""Min/Max
 
@@ -875,15 +875,15 @@
 		"""Child
 
 		Returns the child node associated with the hash
 
 		Returns:
 			_NodeInterface
 		"""
-		return self._node;
+		return self._node
 
 	def clean(self, value, level=[]):
 		"""Clean
 
 		Makes sure both the key and value are properly stored in their correct
 		representation
 
@@ -918,15 +918,15 @@
 			try:
 				dValues[str(self._key.clean(k))] = self._node.clean(v, lLevel)
 			except ValueError as e:
 				lErrors.extend(e.args[0])
 
 		# If there's errors
 		if lErrors:
-			raise lErrors
+			raise ValueError(lErrors)
 
 		# Return the cleaned value
 		return dValues
 
 	def toDict(self):
 		"""To Dict
```

### Comparing `format-oc-1.6.1/LICENSE` & `format-oc-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `format-oc-1.6.1/PKG-INFO` & `format-oc-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: format-oc
-Version: 1.6.1
+Version: 1.6.2
 Summary: Format-OC is a system designed in several languages that uses JSON files to define documents and their allowed parameters to such a fine degree that almost no knowledge of databases is required to get a fully functional back-end, with admin functions, up and running.
 Home-page: https://ouroboroscoding.com/format-oc
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/format-oc-python
 Project-URL: Tracker, https://github.com/ouroboroscoding/format-oc-python/issues
```

### Comparing `format-oc-1.6.1/format_oc.egg-info/PKG-INFO` & `format-oc-1.6.2/format_oc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: format-oc
-Version: 1.6.1
+Version: 1.6.2
 Summary: Format-OC is a system designed in several languages that uses JSON files to define documents and their allowed parameters to such a fine degree that almost no knowledge of databases is required to get a fully functional back-end, with admin functions, up and running.
 Home-page: https://ouroboroscoding.com/format-oc
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/ouroboroscoding/format-oc-python
 Project-URL: Tracker, https://github.com/ouroboroscoding/format-oc-python/issues
```

### Comparing `format-oc-1.6.1/setup.py` & `format-oc-1.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='format-oc',
-	version='1.6.1',
+	version='1.6.2',
 	description='Format-OC is a system designed in several languages that uses JSON files to define documents and their allowed parameters to such a fine degree that almost no knowledge of databases is required to get a fully functional back-end, with admin functions, up and running.',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/format-oc',
 	project_urls={
 		'Source': 'https://github.com/ouroboroscoding/format-oc-python',
 		'Tracker': 'https://github.com/ouroboroscoding/format-oc-python/issues'
```

