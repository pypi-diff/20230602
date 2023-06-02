# Comparing `tmp/lazydev-0.0.3.tar.gz` & `tmp/lazydev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydev-0.0.3.tar", last modified: Fri Jun  2 18:31:22 2023, max compression
+gzip compressed data, was "lazydev-0.0.4.tar", last modified: Fri Jun  2 20:24:22 2023, max compression
```

## Comparing `lazydev-0.0.3.tar` & `lazydev-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.002395 lazydev-0.0.3/
--rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.3/LICENSE
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 18:31:22.002204 lazydev-0.0.3/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.3/README.md
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:21.999833 lazydev-0.0.3/lazydev/
--rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.3/lazydev/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.3/lazydev/develop.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.001863 lazydev-0.0.3/lazydev/modules/
--rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.3/lazydev/modules/__init__.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     5556 2023-06-02 12:54:47.000000 lazydev-0.0.3/lazydev/modules/developer.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     4428 2023-06-02 16:54:25.000000 lazydev-0.0.3/lazydev/modules/prompts.py
--rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.3/lazydev/modules/utils.py
-drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 18:31:22.000930 lazydev-0.0.3/lazydev.egg-info/
--rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/PKG-INFO
--rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/SOURCES.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/dependency_links.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/entry_points.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/requires.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 18:31:21.000000 lazydev-0.0.3/lazydev.egg-info/top_level.txt
--rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 18:31:22.002444 lazydev-0.0.3/setup.cfg
--rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 18:30:32.000000 lazydev-0.0.3/setup.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.544330 lazydev-0.0.4/
+-rw-r--r--   0 anirbankar   (501) staff       (20)    11357 2023-06-02 18:23:56.000000 lazydev-0.0.4/LICENSE
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:24:22.544171 lazydev-0.0.4/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)     3464 2023-06-02 18:29:53.000000 lazydev-0.0.4/README.md
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.542524 lazydev-0.0.4/lazydev/
+-rw-r--r--   0 anirbankar   (501) staff       (20)      482 2023-06-02 17:59:43.000000 lazydev-0.0.4/lazydev/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1247 2023-06-02 17:38:13.000000 lazydev-0.0.4/lazydev/develop.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.543964 lazydev-0.0.4/lazydev/modules/
+-rw-r--r--   0 anirbankar   (501) staff       (20)        0 2023-06-02 17:00:42.000000 lazydev-0.0.4/lazydev/modules/__init__.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     5596 2023-06-02 20:23:45.000000 lazydev-0.0.4/lazydev/modules/developer.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4428 2023-06-02 16:54:25.000000 lazydev-0.0.4/lazydev/modules/prompts.py
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1679 2023-06-02 11:49:48.000000 lazydev-0.0.4/lazydev/modules/utils.py
+drwxr-xr-x   0 anirbankar   (501) staff       (20)        0 2023-06-02 20:24:22.543462 lazydev-0.0.4/lazydev.egg-info/
+-rw-r--r--   0 anirbankar   (501) staff       (20)     4134 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/PKG-INFO
+-rw-r--r--   0 anirbankar   (501) staff       (20)      362 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/SOURCES.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        1 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/dependency_links.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       40 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/entry_points.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       34 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/requires.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)        8 2023-06-02 20:24:22.000000 lazydev-0.0.4/lazydev.egg-info/top_level.txt
+-rw-r--r--   0 anirbankar   (501) staff       (20)       38 2023-06-02 20:24:22.544370 lazydev-0.0.4/setup.cfg
+-rw-r--r--   0 anirbankar   (501) staff       (20)     1478 2023-06-02 20:24:17.000000 lazydev-0.0.4/setup.py
```

### Comparing `lazydev-0.0.3/LICENSE` & `lazydev-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.3/PKG-INFO` & `lazydev-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.3/README.md` & `lazydev-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.3/lazydev/develop.py` & `lazydev-0.0.4/lazydev/develop.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.3/lazydev/modules/developer.py` & `lazydev-0.0.4/lazydev/modules/developer.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,16 @@
     
     def write_file_content(self,file_path):
         prompt=PromptBook.write_file(
             question=self.requirement,
             clarifications=self.clarifications,
             plan=self.plannings,
             files_written=self.files_written,
-            file_path_to_write=file_path
+            file_path_to_write=file_path,
+            file_paths=self.file_paths
             )
         code=self.brain_storm(prompt,f'code-{file_path.split("/")[-1]}') 
         Utilities.write_to_file(code,file_path=file_path)
         self.files_written.append((
             file_path,
             code
         ))
```

### Comparing `lazydev-0.0.3/lazydev/modules/prompts.py` & `lazydev-0.0.4/lazydev/modules/prompts.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.3/lazydev/modules/utils.py` & `lazydev-0.0.4/lazydev/modules/utils.py`

 * *Files identical despite different names*

### Comparing `lazydev-0.0.3/lazydev.egg-info/PKG-INFO` & `lazydev-0.0.4/lazydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydev
-Version: 0.0.3
+Version: 0.0.4
 Summary: AI developer for lazy programmer
 Home-page: https://github.com/thecodacus/lazy-dev
 Author: Anirban Kat
 Author-email: thecodacus@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `lazydev-0.0.3/setup.py` & `lazydev-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name="lazydev",
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         "langchain>=0.0.188",
         "openai>=0.27.7"
     ],
     entry_points={
         'console_scripts': [
```

