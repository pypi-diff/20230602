# Comparing `tmp/lazydev-0.0.4.tar.gz` & `tmp/lazydev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.4.tar", last modified: Fri Jun  2 20:24:22 2023, max compression
+gzip compressed data, was "lazydev-0.0.5.tar", last modified: Fri Jun  2 20:45:06 2023, max compression
```

## Comparing `lazydev-0.0.4.tar` & `lazydev-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.544330 lazydev-0.0.4/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.4/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:24:22.544171 lazydev-0.0.4/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.4/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.542524 lazydev-0.0.4/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.4/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.4/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.543964 lazydev-0.0.4/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.4/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     5596 2023-06-02 20:23:45.000000 lazydev-0.0.4/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     4428 2023-06-02 16:54:25.000000 lazydev-0.0.4/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.4/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.543462 lazydev-0.0.4/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 20:24:22.544370 lazydev-0.0.4/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 20:24:17.000000 lazydev-0.0.4/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.456223 lazydev-0.0.5/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.5/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:45:06.456061 lazydev-0.0.5/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.5/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.453655 lazydev-0.0.5/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.5/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.5/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.455689 lazydev-0.0.5/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.5/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     5694 2023-06-02 20:35:48.000000 lazydev-0.0.5/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4520 2023-06-02 20:38:10.000000 lazydev-0.0.5/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.5/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:45:06.454790 lazydev-0.0.5/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 20:45:06.000000 lazydev-0.0.5/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 20:45:06.456260 lazydev-0.0.5/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 20:44:57.000000 lazydev-0.0.5/setup.py
```

### Comparing `lazydev-0.0.4/LICENSE` & `lazydev-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.4/PKG-INFO` & `lazydev-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.4/README.md` & `lazydev-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.4/lazydev/develop.py` & `lazydev-0.0.5/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.4/lazydev/modules/developer.py` & `lazydev-0.0.5/lazydev/modules/developer.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,16 @@
         # creating files and folders for the project
         print("Creating files...")
         self.generate_folder_structure()
         self.prioratize_files()
         self.files_written=[]
         for file_path in self.file_paths:
             file_name=file_path.split("/")[-1]
+            if(file_name.split(".")[-1] in ["png","jpg","jpeg","bimp"]):
+                continue
             print(f"\nWriting Code for :{file_name}")
             self.write_file_content(file_path)
```

### Comparing `lazydev-0.0.4/lazydev/modules/prompts.py` & `lazydev-0.0.5/lazydev/modules/prompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,12 +123,12 @@
 
 now you are about to write content the following file:
 {file_path_to_write}
 
 As your response will go to an automated parser, things to keep in mind all the time:
 * follow the exact format provided above without fail
 * only write the file content, no expiation, no pretext.
-* always add comments at the begening, which expains what you are about to do
+* if the language support, add comments at steps, which expains what you are about to do, dont add comment if comment is not supported by the file type example json file
 * keep in mind there wont be any additional files other then the full files list given above, only use files that are mentioned in that list
 Begin!
 """
```

### Comparing `lazydev-0.0.4/lazydev/modules/utils.py` & `lazydev-0.0.5/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.4/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.5/lazydev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.4
+Version: 0.0.5
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.4/setup.py` & `lazydev-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

