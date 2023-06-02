# Comparing `tmp/gitconnect-0.1.4.tar.gz` & `tmp/gitconnect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitconnect-0.1.4.tar", last modified: Fri Jun  2 08:09:21 2023, max compression
+gzip compressed data, was "gitconnect-0.1.5.tar", last modified: Fri Jun  2 12:10:46 2023, max compression
```

## Comparing `gitconnect-0.1.4.tar` & `gitconnect-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.266321 gitconnect-0.1.4/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 08:09:21.262321 gitconnect-0.1.4/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)     1783 2023-05-02 08:09:31.000000 gitconnect-0.1.4/README.md
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.254321 gitconnect-0.1.4/gitconnect/
--rw-r--r--   0 agaba     (1000) agaba     (1000)     6219 2023-06-02 07:48:59.000000 gitconnect-0.1.4/gitconnect/GitWrapper.py
--rw-r--r--   0 agaba     (1000) agaba     (1000)       34 2023-05-02 08:09:25.000000 gitconnect-0.1.4/gitconnect/__init__.py
-drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 08:09:21.262321 gitconnect-0.1.4/gitconnect.egg-info/
--rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/PKG-INFO
--rw-r--r--   0 agaba     (1000) agaba     (1000)      235 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/SOURCES.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/dependency_links.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/requires.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       11 2023-06-02 08:09:20.000000 gitconnect-0.1.4/gitconnect.egg-info/top_level.txt
--rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 08:09:21.266321 gitconnect-0.1.4/setup.cfg
--rw-r--r--   0 agaba     (1000) agaba     (1000)      761 2023-06-02 08:06:35.000000 gitconnect-0.1.4/setup.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 12:10:46.307997 gitconnect-0.1.5/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 12:10:46.307997 gitconnect-0.1.5/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     1783 2023-05-02 08:09:31.000000 gitconnect-0.1.5/README.md
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 12:10:46.303997 gitconnect-0.1.5/gitconnect/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)     6014 2023-06-02 11:56:02.000000 gitconnect-0.1.5/gitconnect/GitWrapper.py
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       34 2023-05-02 08:09:25.000000 gitconnect-0.1.5/gitconnect/__init__.py
+drwxr-xr-x   0 agaba     (1000) agaba     (1000)        0 2023-06-02 12:10:46.303997 gitconnect-0.1.5/gitconnect.egg-info/
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      696 2023-06-02 12:10:46.000000 gitconnect-0.1.5/gitconnect.egg-info/PKG-INFO
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      235 2023-06-02 12:10:46.000000 gitconnect-0.1.5/gitconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        1 2023-06-02 12:10:46.000000 gitconnect-0.1.5/gitconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)        9 2023-06-02 12:10:46.000000 gitconnect-0.1.5/gitconnect.egg-info/requires.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       11 2023-06-02 12:10:46.000000 gitconnect-0.1.5/gitconnect.egg-info/top_level.txt
+-rw-r--r--   0 agaba     (1000) agaba     (1000)       38 2023-06-02 12:10:46.307997 gitconnect-0.1.5/setup.cfg
+-rw-r--r--   0 agaba     (1000) agaba     (1000)      761 2023-06-02 12:08:55.000000 gitconnect-0.1.5/setup.py
```

### Comparing `gitconnect-0.1.4/PKG-INFO` & `gitconnect-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitconnect-0.1.4/README.md` & `gitconnect-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gitconnect-0.1.4/gitconnect/GitWrapper.py` & `gitconnect-0.1.5/gitconnect/GitWrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,31 +77,27 @@
         :param order: The order to sort the results in. Defaults to 'desc'.
         :return: A list of dictionaries containing information about the matching repositories.
         """
         endpoint = f'/search/repositories?q=user:{username}+{query}&sort={sort}&order={order}'
         response = self._get(endpoint)
         return response['items']
     
-
-    def get_commits(self, owner: str, repo_name: str, branch: str = 'master') -> list:
+    def get_commits(self, owner: str, repo_name: str) -> list:
         """
-        Get a list of commits for a given repository and branch.
+        Get a list of commits for a GitHub repository.
 
         :param owner: The username or organization that owns the repository.
-        :str
+        :type owner: str
         :param repo_name: The name of the repository.
         :type repo_name: str
-        :param branch: The name of the branch to get commits for. Defaults to 'master'.
-        :type branch: str
         :return: A list of dictionaries containing information about the commits.
         """
         endpoint = f'/repos/{owner}/{repo_name}/commits'
-        params = {'sha': branch}
-        response = self._get(endpoint, params)
-        return response
+        return self._get(endpoint)
+
 
     def get_commit_files(self, owner: str, repo_name: str, sha: str) -> list:
         """
         Get a list of files changed in a given commit.
         :param owner: The username or organization that owns the repository.
         :type owner: str
         :param repo_name: The name of the repository.
```

### Comparing `gitconnect-0.1.4/gitconnect.egg-info/PKG-INFO` & `gitconnect-0.1.5/gitconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitconnect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python wrapper for the GitHub API
 Home-page: UNKNOWN
 Author: Ed
 Author-email: ed.a9a6a@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitconnect-0.1.4/setup.py` & `gitconnect-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='gitconnect',
-    version='0.1.4',
+    version='0.1.5',
     description='A Python wrapper for the GitHub API',
     author='Ed',
     author_email='ed.a9a6a@gmail.com',
     packages=['gitconnect'],
     install_requires=['requests'],
     classifiers=[
         'Development Status :: 3 - Alpha',
```

