# Comparing `tmp/git_ling-0.3.1.tar.gz` & `tmp/git_ling-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_ling-0.3.1.tar", last modified: Fri Jun  2 20:43:55 2023, max compression
+gzip compressed data, was "git_ling-0.3.2.tar", last modified: Fri Jun  2 20:46:44 2023, max compression
```

## Comparing `git_ling-0.3.1.tar` & `git_ling-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:43:55.082102 git_ling-0.3.1/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:43:55.082102 git_ling-0.3.1/PKG-INFO
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      867 2023-06-02 19:44:15.000000 git_ling-0.3.1/README.md
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:43:55.082102 git_ling-0.3.1/git_ling/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       47 2023-06-02 19:38:02.000000 git_ling-0.3.1/git_ling/__init__.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1219 2023-06-02 19:38:11.000000 git_ling-0.3.1/git_ling/cli.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     4440 2023-06-02 20:41:06.000000 git_ling-0.3.1/git_ling/git_ling.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1356 2023-06-02 19:37:08.000000 git_ling-0.3.1/git_ling/language_fetcher.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     2687 2023-06-02 19:37:08.000000 git_ling-0.3.1/git_ling/schemas.py
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:43:55.082102 git_ling-0.3.1/git_ling.egg-info/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/PKG-INFO
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      409 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/SOURCES.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)        1 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/dependency_links.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       48 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/entry_points.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       25 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/requires.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       15 2023-06-02 20:43:55.000000 git_ling-0.3.1/git_ling.egg-info/top_level.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       38 2023-06-02 20:43:55.082102 git_ling-0.3.1/setup.cfg
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      849 2023-06-02 20:43:19.000000 git_ling-0.3.1/setup.py
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:43:55.082102 git_ling-0.3.1/tests/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 16:34:23.000000 git_ling-0.3.1/tests/__init__.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1961 2023-06-02 19:43:25.000000 git_ling-0.3.1/tests/test_cli.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     3206 2023-06-02 20:42:04.000000 git_ling-0.3.1/tests/test_git_ling.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1712 2023-06-02 19:37:08.000000 git_ling-0.3.1/tests/test_language_fetcher.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:46:44.612101 git_ling-0.3.2/PKG-INFO
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      867 2023-06-02 19:44:15.000000 git_ling-0.3.2/README.md
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/git_ling/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       47 2023-06-02 19:38:02.000000 git_ling-0.3.2/git_ling/__init__.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1219 2023-06-02 19:38:11.000000 git_ling-0.3.2/git_ling/cli.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     4440 2023-06-02 20:41:06.000000 git_ling-0.3.2/git_ling/git_ling.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1356 2023-06-02 20:45:39.000000 git_ling-0.3.2/git_ling/language_fetcher.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     2687 2023-06-02 19:37:08.000000 git_ling-0.3.2/git_ling/schemas.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/git_ling.egg-info/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/PKG-INFO
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      409 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/SOURCES.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)        1 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/dependency_links.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       48 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/entry_points.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       25 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/requires.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       15 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/top_level.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       38 2023-06-02 20:46:44.612101 git_ling-0.3.2/setup.cfg
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      849 2023-06-02 20:46:40.000000 git_ling-0.3.2/setup.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/tests/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 16:34:23.000000 git_ling-0.3.2/tests/__init__.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1961 2023-06-02 19:43:25.000000 git_ling-0.3.2/tests/test_cli.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     3206 2023-06-02 20:42:04.000000 git_ling-0.3.2/tests/test_git_ling.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1712 2023-06-02 19:37:08.000000 git_ling-0.3.2/tests/test_language_fetcher.py
```

### Comparing `git_ling-0.3.1/PKG-INFO` & `git_ling-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_ling
-Version: 0.3.1
+Version: 0.3.2
 Summary: git_ling is a small library to detect programming languages from file names and extensions
 Home-page: UNKNOWN
 Author: Daniel Piro
 License: UNKNOWN
 Description: # git_ling
         
         git_ling is a small library to detect programming languages from file names and extensions.
```

### Comparing `git_ling-0.3.1/README.md` & `git_ling-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/git_ling/cli.py` & `git_ling-0.3.2/git_ling/cli.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/git_ling/git_ling.py` & `git_ling-0.3.2/git_ling/git_ling.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/git_ling/language_fetcher.py` & `git_ling-0.3.2/git_ling/language_fetcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             logger.debug("Successfully parsed YAML file")
             return content
         except yaml.YAMLError as e:
             logger.error("Error while parsing YAML file: %s", e)
             return {}
 
 def update_cache():
-    url = 'https://raw.githubusercontent.com/github-git_ling/git_ling/master/lib/git_ling/languages.yml'
+    url = 'https://raw.githubusercontent.com/github-linguist/linguist/master/lib/linguist/languages.yml'
     result=urllib.request.urlretrieve(url, CACHE_FILE)
     # Check if file was downloaded successfully
     if result[0] == CACHE_FILE:
         logger.info("Successfully updated cache")
 if __name__ == "__main__":
     # Pretty print the result
     import json
```

### Comparing `git_ling-0.3.1/git_ling/schemas.py` & `git_ling-0.3.2/git_ling/schemas.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/git_ling.egg-info/PKG-INFO` & `git_ling-0.3.2/git_ling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-ling
-Version: 0.3.1
+Version: 0.3.2
 Summary: git_ling is a small library to detect programming languages from file names and extensions
 Home-page: UNKNOWN
 Author: Daniel Piro
 License: UNKNOWN
 Description: # git_ling
         
         git_ling is a small library to detect programming languages from file names and extensions.
```

### Comparing `git_ling-0.3.1/setup.py` & `git_ling-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="git_ling",
-    version="0.3.1",
+    version="0.3.2",
     packages=find_packages(),
     author="Daniel Piro",
     description="git_ling is a small library to detect programming languages from file names and extensions",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `git_ling-0.3.1/tests/test_cli.py` & `git_ling-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/tests/test_git_ling.py` & `git_ling-0.3.2/tests/test_git_ling.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.1/tests/test_language_fetcher.py` & `git_ling-0.3.2/tests/test_language_fetcher.py`

 * *Files identical despite different names*

