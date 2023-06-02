# Comparing `tmp/PyOptionPane-0.621.tar.gz` & `tmp/PyOptionPane-0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyOptionPane-0.621.tar", last modified: Sat Oct  1 00:50:26 2022, max compression
+gzip compressed data, was "PyOptionPane-0.67.tar", last modified: Sat Oct  1 00:48:16 2022, max compression
```

## Comparing `PyOptionPane-0.621.tar` & `PyOptionPane-0.67.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:50:26.466790 PyOptionPane-0.621/
--rw-r--r--   0 yavda      (501) staff       (20)      409 2022-10-01 00:50:26.466666 PyOptionPane-0.621/PKG-INFO
-drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:50:26.466129 PyOptionPane-0.621/PyOptionPane/
--rw-r--r--   0 yavda      (501) staff       (20)     4091 2022-09-29 01:15:26.000000 PyOptionPane-0.621/PyOptionPane/PyOptionPane.py
--rw-r--r--   0 yavda      (501) staff       (20)      203 2022-10-01 00:49:30.000000 PyOptionPane-0.621/PyOptionPane/__init__.py
-drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:50:26.466523 PyOptionPane-0.621/PyOptionPane.egg-info/
--rw-r--r--   0 yavda      (501) staff       (20)      409 2022-10-01 00:50:26.000000 PyOptionPane-0.621/PyOptionPane.egg-info/PKG-INFO
--rw-r--r--   0 yavda      (501) staff       (20)      216 2022-10-01 00:50:26.000000 PyOptionPane-0.621/PyOptionPane.egg-info/SOURCES.txt
--rw-r--r--   0 yavda      (501) staff       (20)        1 2022-10-01 00:50:26.000000 PyOptionPane-0.621/PyOptionPane.egg-info/dependency_links.txt
--rw-r--r--   0 yavda      (501) staff       (20)       13 2022-10-01 00:50:26.000000 PyOptionPane-0.621/PyOptionPane.egg-info/top_level.txt
--rw-r--r--   0 yavda      (501) staff       (20)     2159 2022-09-30 00:10:52.000000 PyOptionPane-0.621/README.md
--rw-r--r--   0 yavda      (501) staff       (20)       38 2022-10-01 00:50:26.466824 PyOptionPane-0.621/setup.cfg
--rw-r--r--   0 yavda      (501) staff       (20)      824 2022-10-01 00:50:09.000000 PyOptionPane-0.621/setup.py
+drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:48:16.989003 PyOptionPane-0.67/
+-rw-r--r--   0 yavda      (501) staff       (20)      408 2022-10-01 00:48:16.988880 PyOptionPane-0.67/PKG-INFO
+drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:48:16.988296 PyOptionPane-0.67/PyOptionPane/
+-rw-r--r--   0 yavda      (501) staff       (20)     4091 2022-09-29 01:15:26.000000 PyOptionPane-0.67/PyOptionPane/PyOptionPane.py
+-rw-r--r--   0 yavda      (501) staff       (20)      155 2022-10-01 00:45:40.000000 PyOptionPane-0.67/PyOptionPane/__init__.py
+drwxr-xr-x   0 yavda      (501) staff       (20)        0 2022-10-01 00:48:16.988698 PyOptionPane-0.67/PyOptionPane.egg-info/
+-rw-r--r--   0 yavda      (501) staff       (20)      408 2022-10-01 00:48:16.000000 PyOptionPane-0.67/PyOptionPane.egg-info/PKG-INFO
+-rw-r--r--   0 yavda      (501) staff       (20)      216 2022-10-01 00:48:16.000000 PyOptionPane-0.67/PyOptionPane.egg-info/SOURCES.txt
+-rw-r--r--   0 yavda      (501) staff       (20)        1 2022-10-01 00:48:16.000000 PyOptionPane-0.67/PyOptionPane.egg-info/dependency_links.txt
+-rw-r--r--   0 yavda      (501) staff       (20)       13 2022-10-01 00:48:16.000000 PyOptionPane-0.67/PyOptionPane.egg-info/top_level.txt
+-rw-r--r--   0 yavda      (501) staff       (20)     2159 2022-09-30 00:10:52.000000 PyOptionPane-0.67/README.md
+-rw-r--r--   0 yavda      (501) staff       (20)       38 2022-10-01 00:48:16.989035 PyOptionPane-0.67/setup.cfg
+-rw-r--r--   0 yavda      (501) staff       (20)      823 2022-10-01 00:48:13.000000 PyOptionPane-0.67/setup.py
```

### Comparing `PyOptionPane-0.621/PyOptionPane/PyOptionPane.py` & `PyOptionPane-0.67/PyOptionPane/PyOptionPane.py`

 * *Files identical despite different names*

### Comparing `PyOptionPane-0.621/README.md` & `PyOptionPane-0.67/README.md`

 * *Files identical despite different names*

### Comparing `PyOptionPane-0.621/setup.py` & `PyOptionPane-0.67/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.89'
+VERSION = '0.1.45'
 DESCRIPTION = 'Python GUIS made easy'
 LONG_DESCRIPTION = 'Python GUIS made easy.'
 
 setup(
     name="PyOptionPane",
-    version="0.621",
+    version="0.67",
     author="yavda1",
     description="Python GUIs made easy",
     packages=find_packages(),
     keywords=['python', 'tkinter', 'gui'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
```

