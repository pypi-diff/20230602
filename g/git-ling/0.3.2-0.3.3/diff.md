# Comparing `tmp/git_ling-0.3.2.tar.gz` & `tmp/git_ling-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_ling-0.3.2.tar", last modified: Fri Jun  2 20:46:44 2023, max compression
+gzip compressed data, was "git_ling-0.3.3.tar", last modified: Fri Jun  2 20:52:16 2023, max compression
```

## Comparing `git_ling-0.3.2.tar` & `git_ling-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:46:44.612101 git_ling-0.3.2/PKG-INFO
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      867 2023-06-02 19:44:15.000000 git_ling-0.3.2/README.md
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/git_ling/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       47 2023-06-02 19:38:02.000000 git_ling-0.3.2/git_ling/__init__.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1219 2023-06-02 19:38:11.000000 git_ling-0.3.2/git_ling/cli.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     4440 2023-06-02 20:41:06.000000 git_ling-0.3.2/git_ling/git_ling.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1356 2023-06-02 20:45:39.000000 git_ling-0.3.2/git_ling/language_fetcher.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     2687 2023-06-02 19:37:08.000000 git_ling-0.3.2/git_ling/schemas.py
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/git_ling.egg-info/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/PKG-INFO
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      409 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/SOURCES.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)        1 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/dependency_links.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       48 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/entry_points.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       25 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/requires.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       15 2023-06-02 20:46:44.000000 git_ling-0.3.2/git_ling.egg-info/top_level.txt
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)       38 2023-06-02 20:46:44.612101 git_ling-0.3.2/setup.cfg
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)      849 2023-06-02 20:46:40.000000 git_ling-0.3.2/setup.py
-drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:46:44.612101 git_ling-0.3.2/tests/
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 16:34:23.000000 git_ling-0.3.2/tests/__init__.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1961 2023-06-02 19:43:25.000000 git_ling-0.3.2/tests/test_cli.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     3206 2023-06-02 20:42:04.000000 git_ling-0.3.2/tests/test_git_ling.py
--rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1712 2023-06-02 19:37:08.000000 git_ling-0.3.2/tests/test_language_fetcher.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:52:16.892098 git_ling-0.3.3/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:52:16.892098 git_ling-0.3.3/PKG-INFO
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      867 2023-06-02 19:44:15.000000 git_ling-0.3.3/README.md
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:52:16.892098 git_ling-0.3.3/git_ling/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       47 2023-06-02 19:38:02.000000 git_ling-0.3.3/git_ling/__init__.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1219 2023-06-02 19:38:11.000000 git_ling-0.3.3/git_ling/cli.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     4335 2023-06-02 20:51:41.000000 git_ling-0.3.3/git_ling/git_ling.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1356 2023-06-02 20:45:39.000000 git_ling-0.3.3/git_ling/language_fetcher.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     2687 2023-06-02 19:37:08.000000 git_ling-0.3.3/git_ling/schemas.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:52:16.892098 git_ling-0.3.3/git_ling.egg-info/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1721 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/PKG-INFO
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      409 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/SOURCES.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)        1 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/dependency_links.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       48 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/entry_points.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       25 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/requires.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       15 2023-06-02 20:52:16.000000 git_ling-0.3.3/git_ling.egg-info/top_level.txt
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)       38 2023-06-02 20:52:16.892098 git_ling-0.3.3/setup.cfg
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)      849 2023-06-02 20:52:09.000000 git_ling-0.3.3/setup.py
+drwxr-xr-x   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 20:52:16.892098 git_ling-0.3.3/tests/
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)        0 2023-06-02 16:34:23.000000 git_ling-0.3.3/tests/__init__.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1961 2023-06-02 19:43:25.000000 git_ling-0.3.3/tests/test_cli.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     3206 2023-06-02 20:42:04.000000 git_ling-0.3.3/tests/test_git_ling.py
+-rw-r--r--   0 dpiro     (1000) dpiro     (1000)     1712 2023-06-02 19:37:08.000000 git_ling-0.3.3/tests/test_language_fetcher.py
```

### Comparing `git_ling-0.3.2/PKG-INFO` & `git_ling-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_ling
-Version: 0.3.2
+Version: 0.3.3
 Summary: git_ling is a small library to detect programming languages from file names and extensions
 Home-page: UNKNOWN
 Author: Daniel Piro
 License: UNKNOWN
 Description: # git_ling
         
         git_ling is a small library to detect programming languages from file names and extensions.
```

### Comparing `git_ling-0.3.2/README.md` & `git_ling-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/git_ling/cli.py` & `git_ling-0.3.3/git_ling/cli.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/git_ling/git_ling.py` & `git_ling-0.3.3/git_ling/git_ling.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,19 +55,18 @@
             return None
     
 
     def file_belongs_to_language(self, filename, language: Language, extra_filenames:List[str]=[])->bool:
         """
         Checks if a file belongs to a language
         """
-        # Check if file exist and is a file
-        if not os.path.isfile(filename):
-            raise FileNotFoundError(f"File {filename} does not exist")
         # Get the base name of the file (file name with extension)
         base_name = os.path.basename(filename)
+        if not base_name:
+            return False
         # To get the file name and extension separately, you can use os.path.splitext
         file_name, file_extension = os.path.splitext(base_name)
         self.logger.debug(f"Checking  if File name: {base_name} belongs to language {language.name}")
         # Check if file belongs to language
         if language.extensions:
             if file_extension in language.extensions: # Check if extension is in list of extensions
                 self.logger.debug(f"File extension {file_extension} is in list of extensions for language {language.name}")
```

### Comparing `git_ling-0.3.2/git_ling/language_fetcher.py` & `git_ling-0.3.3/git_ling/language_fetcher.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/git_ling/schemas.py` & `git_ling-0.3.3/git_ling/schemas.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/git_ling.egg-info/PKG-INFO` & `git_ling-0.3.3/git_ling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-ling
-Version: 0.3.2
+Version: 0.3.3
 Summary: git_ling is a small library to detect programming languages from file names and extensions
 Home-page: UNKNOWN
 Author: Daniel Piro
 License: UNKNOWN
 Description: # git_ling
         
         git_ling is a small library to detect programming languages from file names and extensions.
```

### Comparing `git_ling-0.3.2/setup.py` & `git_ling-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="git_ling",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(),
     author="Daniel Piro",
     description="git_ling is a small library to detect programming languages from file names and extensions",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
```

### Comparing `git_ling-0.3.2/tests/test_cli.py` & `git_ling-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/tests/test_git_ling.py` & `git_ling-0.3.3/tests/test_git_ling.py`

 * *Files identical despite different names*

### Comparing `git_ling-0.3.2/tests/test_language_fetcher.py` & `git_ling-0.3.3/tests/test_language_fetcher.py`

 * *Files identical despite different names*

