# Comparing `tmp/gameauto-1.0.3.tar.gz` & `tmp/gameauto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameauto-1.0.3.tar", last modified: Fri Jun  2 05:10:07 2023, max compression
+gzip compressed data, was "gameauto-1.0.4.tar", last modified: Fri Jun  2 05:09:03 2023, max compression
```

## Comparing `gameauto-1.0.3.tar` & `gameauto-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:10:07.079817 gameauto-1.0.3/
--rw-rw-rw-   0        0        0     3355 2023-06-02 05:10:07.078820 gameauto-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-06-02 05:08:07.000000 gameauto-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 05:10:07.064484 gameauto-1.0.3/gameauto/
--rw-rw-rw-   0        0        0       62 2023-06-02 04:50:23.000000 gameauto-1.0.3/gameauto/__init__.py
--rw-rw-rw-   0        0        0     6005 2023-06-02 04:56:16.000000 gameauto-1.0.3/gameauto/core.py
--rw-rw-rw-   0        0        0     9475 2023-06-02 04:51:29.000000 gameauto-1.0.3/gameauto/images.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:10:07.077821 gameauto-1.0.3/gameauto.egg-info/
--rw-rw-rw-   0        0        0     3355 2023-06-02 05:10:06.000000 gameauto-1.0.3/gameauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-02 05:10:07.000000 gameauto-1.0.3/gameauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:10:06.000000 gameauto-1.0.3/gameauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-02 05:10:06.000000 gameauto-1.0.3/gameauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 05:10:06.000000 gameauto-1.0.3/gameauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 05:10:07.079817 gameauto-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      688 2023-06-02 05:09:53.000000 gameauto-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.984724 gameauto-1.0.4/
+-rw-rw-rw-   0        0        0     3355 2023-06-02 05:09:03.983540 gameauto-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3048 2023-06-02 05:08:07.000000 gameauto-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.955578 gameauto-1.0.4/gameauto/
+-rw-rw-rw-   0        0        0       62 2023-06-02 04:50:23.000000 gameauto-1.0.4/gameauto/__init__.py
+-rw-rw-rw-   0        0        0     6005 2023-06-02 04:56:16.000000 gameauto-1.0.4/gameauto/core.py
+-rw-rw-rw-   0        0        0     9475 2023-06-02 04:51:29.000000 gameauto-1.0.4/gameauto/images.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.982542 gameauto-1.0.4/gameauto.egg-info/
+-rw-rw-rw-   0        0        0     3355 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 05:09:03.985760 gameauto-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      688 2023-06-02 05:00:54.000000 gameauto-1.0.4/setup.py
```

### Comparing `gameauto-1.0.3/PKG-INFO` & `gameauto-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameauto
-Version: 1.0.3
+Version: 1.0.4
 Summary: Android Game Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `gameauto-1.0.3/README.md` & `gameauto-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gameauto-1.0.3/gameauto/core.py` & `gameauto-1.0.4/gameauto/core.py`

 * *Files identical despite different names*

### Comparing `gameauto-1.0.3/gameauto/images.py` & `gameauto-1.0.4/gameauto/images.py`

 * *Files identical despite different names*

### Comparing `gameauto-1.0.3/gameauto.egg-info/PKG-INFO` & `gameauto-1.0.4/gameauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameauto
-Version: 1.0.3
+Version: 1.0.4
 Summary: Android Game Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `gameauto-1.0.3/setup.py` & `gameauto-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='gameauto',
-      version='1.0.3',
+      version='1.0.4',
       description='Android Game Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
```

