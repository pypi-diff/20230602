# Comparing `tmp/wombo-1.0.1.tar.gz` & `tmp/wombo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wombo-1.0.1.tar", last modified: Fri Jun  2 06:50:03 2023, max compression
+gzip compressed data, was "wombo-1.0.2.tar", last modified: Fri Jun  2 06:52:37 2023, max compression
```

## Comparing `wombo-1.0.1.tar` & `wombo-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:50:03.483602 wombo-1.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-06-01 16:24:00.000000 wombo-1.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2023-06-02 06:50:03.483602 wombo-1.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-01 16:24:00.000000 wombo-1.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-02 06:50:03.483602 wombo-1.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      739 2023-06-02 06:47:33.000000 wombo-1.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:50:03.479602 wombo-1.0.1/wombo/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-06-02 06:49:29.000000 wombo-1.0.1/wombo/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4100 2023-06-01 22:02:57.000000 wombo-1.0.1/wombo/async_dream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2845 2023-06-01 22:02:57.000000 wombo-1.0.1/wombo/dream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3274 2023-06-01 22:02:57.000000 wombo-1.0.1/wombo/urls.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:50:03.483602 wombo-1.0.1/wombo.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2023-06-02 06:50:03.000000 wombo-1.0.1/wombo.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      248 2023-06-02 06:50:03.000000 wombo-1.0.1/wombo.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 06:50:03.000000 wombo-1.0.1/wombo.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-06-02 06:50:03.000000 wombo-1.0.1/wombo.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-06-02 06:50:03.000000 wombo-1.0.1/wombo.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:52:37.287602 wombo-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2023-06-01 16:24:00.000000 wombo-1.0.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2023-06-02 06:52:37.287602 wombo-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-06-01 16:24:00.000000 wombo-1.0.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-02 06:52:37.287602 wombo-1.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      739 2023-06-02 06:52:08.000000 wombo-1.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:52:37.287602 wombo-1.0.2/wombo/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-06-02 06:52:19.000000 wombo-1.0.2/wombo/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4100 2023-06-01 22:02:57.000000 wombo-1.0.2/wombo/async_dream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2845 2023-06-01 22:02:57.000000 wombo-1.0.2/wombo/dream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3274 2023-06-01 22:02:57.000000 wombo-1.0.2/wombo/urls.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 06:52:37.287602 wombo-1.0.2/wombo.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      539 2023-06-02 06:52:37.000000 wombo-1.0.2/wombo.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      248 2023-06-02 06:52:37.000000 wombo-1.0.2/wombo.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 06:52:37.000000 wombo-1.0.2/wombo.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-06-02 06:52:37.000000 wombo-1.0.2/wombo.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-06-02 06:52:37.000000 wombo-1.0.2/wombo.egg-info/top_level.txt
```

### Comparing `wombo-1.0.1/LICENSE` & `wombo-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wombo-1.0.1/PKG-INFO` & `wombo-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dream AI api library
 Home-page: https://github.com/pokedim13/WOMBO
 Author: H3try
 Author-email: skinxedovich@mail.ru
 Project-URL: Documentation, https://github.com/pokedim13/WOMBO
 Keywords: example python
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wombo-1.0.1/setup.py` & `wombo-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 setup(
   name='wombo',
-  version='1.0.1',
+  version='1.0.2',
   author='H3try',
   author_email='skinxedovich@mail.ru',
   description='Dream AI api library',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/pokedim13/WOMBO',
   packages=find_packages(),
```

### Comparing `wombo-1.0.1/wombo/async_dream.py` & `wombo-1.0.2/wombo/async_dream.py`

 * *Files identical despite different names*

### Comparing `wombo-1.0.1/wombo/dream.py` & `wombo-1.0.2/wombo/dream.py`

 * *Files identical despite different names*

### Comparing `wombo-1.0.1/wombo/urls.py` & `wombo-1.0.2/wombo/urls.py`

 * *Files identical despite different names*

### Comparing `wombo-1.0.1/wombo.egg-info/PKG-INFO` & `wombo-1.0.2/wombo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wombo
-Version: 1.0.1
+Version: 1.0.2
 Summary: Dream AI api library
 Home-page: https://github.com/pokedim13/WOMBO
 Author: H3try
 Author-email: skinxedovich@mail.ru
 Project-URL: Documentation, https://github.com/pokedim13/WOMBO
 Keywords: example python
 Classifier: Programming Language :: Python :: 3.11
```

