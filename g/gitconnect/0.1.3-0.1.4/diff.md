# Comparing `tmp/gitconnect-0.1.3.tar.gz` & `tmp/gitconnect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitconnect-0.1.3.tar", last modified: Wed May  3 08:51:22 2023, max compression
+gzip compressed data, was "gitconnect-0.1.4.tar", last modified: Fri Jun  2 08:09:21 2023, max compression
```

## Comparing `gitconnect-0.1.3.tar` & `gitconnect-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-03 08:51:22.012363 gitconnect-0.1.3/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      594 2023-05-03 08:51:22.012363 gitconnect-0.1.3/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)     1783 2023-05-02 08:09:31.000000 gitconnect-0.1.3/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-03 08:51:22.008362 gitconnect-0.1.3/gitconnect/
--rw-r--r--   0 agaba     (1000) agaba     (1000)     5293 2023-05-03 07:36:10.000000 gitconnect-0.1.3/gitconnect/GitWrapper.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)       34 2023-05-02 08:09:25.000000 gitconnect-0.1.3/gitconnect/__init__.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-05-03 08:51:22.012363 gitconnect-0.1.3/gitconnect.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      594 2023-05-03 08:51:21.000000 gitconnect-0.1.3/gitconnect.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      235 2023-05-03 08:51:21.000000 gitconnect-0.1.3/gitconnect.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-05-03 08:51:21.000000 gitconnect-0.1.3/gitconnect.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-05-03 08:51:21.000000 gitconnect-0.1.3/gitconnect.egg-info/requires.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       11 2023-05-03 08:51:21.000000 gitconnect-0.1.3/gitconnect.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-05-03 08:51:22.012363 gitconnect-0.1.3/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      662 2023-05-03 08:48:07.000000 gitconnect-0.1.3/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.266321 gitconnect-0.1.4/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 08:09:21.262321 gitconnect-0.1.4/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     1783 2023-05-02 08:09:31.000000 gitconnect-0.1.4/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.254321 gitconnect-0.1.4/gitconnect/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     6219 2023-06-02 07:48:59.000000 gitconnect-0.1.4/gitconnect/GitWrapper.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       34 2023-05-02 08:09:25.000000 gitconnect-0.1.4/gitconnect/__init__.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.262321 gitconnect-0.1.4/gitconnect.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      235 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/requires.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       11 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 08:09:21.266321 gitconnect-0.1.4/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      761 2023-06-02 08:06:35.000000 gitconnect-0.1.4/setup.py
```

### Comparing `gitconnect-0.1.3/PKG-INFO` & `gitconnect-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 
 UNKNOWN
```

### Comparing `gitconnect-0.1.3/README.md` & `gitconnect-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gitconnect-0.1.3/gitconnect/GitWrapper.py` & `gitconnect-0.1.4/gitconnect/GitWrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -130,7 +130,30 @@
         """
         endpoint = f'/repos/{owner}/{repo_name}/contents/{path}'
         params = {'ref': sha}
         response = self._get(endpoint, params)
         return response['content']
     
 
+    def get_source_files(self, owner: str, repo_name: str, file_extensions: list) -> list:
+        """
+        Get a list of source files with the specified file extensions for a given repository.
+
+        :param owner: The username or organization that owns the repository.
+        :type owner: str
+        :param repo_name: The name of the repository.
+        :type repo_name: str
+        :param file_extensions: The list of file extensions to filter for.
+        :type file_extensions: list
+        :return: A list of dictionaries containing information about the source files.
+        """
+        endpoint = f'/repos/{owner}/{repo_name}/contents'
+        response = self._get(endpoint)
+        source_files = []
+
+        for file in response:
+            if file['type'] == 'file' and any(file['name'].endswith(ext) for ext in file_extensions):
+                source_files.append(file)
+
+        return source_files
+    
+
```

### Comparing `gitconnect-0.1.3/gitconnect.egg-info/PKG-INFO` & `gitconnect-0.1.4/gitconnect.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 
 UNKNOWN
```

### Comparing `gitconnect-0.1.3/setup.py` & `gitconnect-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from setuptools import setup
 
 setup(
     name='gitconnect',
-    version='0.1.3',
+    version='0.1.4',
     description='A Python wrapper for the GitHub API',
     author='Ed',
     author_email='ed.a9a6a@gmail.com',
     packages=['gitconnect'],
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11'
     ],
 )
```

