# Comparing `tmp/pyclpu-0.0.2.tar.gz` & `tmp/pyclpu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyclpu-0.0.2.tar", last modified: Fri Jun  2 08:37:51 2023, max compression
+gzip compressed data, was "dist\pyclpu-0.0.3.tar", last modified: Fri Jun  2 08:53:10 2023, max compression
```

## Comparing `pyclpu-0.0.2.tar` & `pyclpu-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:37:51.000000 pyclpu-0.0.2/
--rw-rw-rw-   0        0        0      382 2023-06-02 08:37:51.000000 pyclpu-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 08:37:51.000000 pyclpu-0.0.2/pyclpu/
--rw-rw-rw-   0        0        0     1878 2023-06-01 14:29:35.000000 pyclpu-0.0.2/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2022-04-16 17:02:37.000000 pyclpu-0.0.2/pyclpu/formats.py
--rw-rw-rw-   0        0        0    17935 2023-06-01 15:49:51.000000 pyclpu-0.0.2/pyclpu/image.py
--rw-rw-rw-   0        0        0    30733 2023-05-31 09:32:25.000000 pyclpu-0.0.2/pyclpu/main.py
--rw-rw-rw-   0        0        0      629 2023-05-31 09:16:16.000000 pyclpu-0.0.2/pyclpu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:37:51.000000 pyclpu-0.0.2/pyclpu.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-02 08:37:50.000000 pyclpu-0.0.2/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      382 2023-06-02 08:37:50.000000 pyclpu-0.0.2/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-06-02 08:37:50.000000 pyclpu-0.0.2/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0      265 2023-06-02 08:37:50.000000 pyclpu-0.0.2/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 08:37:50.000000 pyclpu-0.0.2/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1049 2023-06-01 16:05:31.000000 pyclpu-0.0.2/README.md
--rw-rw-rw-   0        0        0       92 2023-06-02 08:37:51.000000 pyclpu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1803 2023-06-02 08:36:58.000000 pyclpu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/
+-rw-rw-rw-   0        0        0      382 2023-06-02 08:53:10.000000 pyclpu-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu/
+-rw-rw-rw-   0        0        0     1878 2023-06-01 14:29:35.000000 pyclpu-0.0.3/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2022-04-16 17:02:37.000000 pyclpu-0.0.3/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    17931 2023-06-02 08:49:07.000000 pyclpu-0.0.3/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30733 2023-05-31 09:32:25.000000 pyclpu-0.0.3/pyclpu/main.py
+-rw-rw-rw-   0        0        0     7425 2022-04-16 17:02:37.000000 pyclpu-0.0.3/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0      629 2023-06-02 08:52:40.000000 pyclpu-0.0.3/pyclpu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      382 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      285 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1049 2023-06-01 16:05:31.000000 pyclpu-0.0.3/README.md
+-rw-rw-rw-   0        0        0       92 2023-06-02 08:53:10.000000 pyclpu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1803 2023-06-02 08:36:58.000000 pyclpu-0.0.3/setup.py
```

### Comparing `pyclpu-0.0.2/pyclpu/constants.py` & `pyclpu-0.0.3/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.2/pyclpu/formats.py` & `pyclpu-0.0.3/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.2/pyclpu/image.py` & `pyclpu-0.0.3/pyclpu/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 root = os.path.dirname(os.path.abspath(getsourcefile(lambda:0))) # get environment
 sys.path.append(os.path.abspath(root))                           # add environment
 sys.path.append(os.path.abspath(root)+os.path.sep+"LIB")         # add library
 
 if "constants" not in globals() or globals()['constants'] == False:
     import constants            # import all global constants from                   constants.py
     import formats              # import all global formats from                     formats.py
-    from s33293804 import *     # import zoom PanZoomWindow for display images from  LIB/s33293804.py
+    from s33293804 import *     # import zoom PanZoomWindow for display images from  s33293804.py
     reload(constants)
     reload(formats)
 
 # STYLE
 
 # =============================================================================
 # CONSTANTS
```

### Comparing `pyclpu-0.0.2/pyclpu/main.py` & `pyclpu-0.0.3/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.2/pyclpu/__init__.py` & `pyclpu-0.0.3/pyclpu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-0.0.2/README.md` & `pyclpu-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.2/setup.py` & `pyclpu-0.0.3/setup.py`

 * *Files identical despite different names*

