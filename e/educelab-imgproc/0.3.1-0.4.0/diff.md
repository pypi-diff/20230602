# Comparing `tmp/educelab-imgproc-0.3.1.tar.gz` & `tmp/educelab-imgproc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educelab-imgproc-0.3.1.tar", last modified: Wed May 10 17:55:42 2023, max compression
+gzip compressed data, was "educelab-imgproc-0.4.0.tar", last modified: Fri Jun  2 14:28:29 2023, max compression
```

## Comparing `educelab-imgproc-0.3.1.tar` & `educelab-imgproc-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 17:55:42.062675 educelab-imgproc-0.3.1/
--rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab-imgproc-0.3.1/LICENSE
--rw-r--r--   0 seth       (501) staff       (20)     1357 2023-05-10 17:55:42.062730 educelab-imgproc-0.3.1/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab-imgproc-0.3.1/README.md
--rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab-imgproc-0.3.1/pyproject.toml
--rw-r--r--   0 seth       (501) staff       (20)       45 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.1/requirements.txt
--rw-r--r--   0 seth       (501) staff       (20)      918 2023-05-10 17:55:42.062977 educelab-imgproc-0.3.1/setup.cfg
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 17:55:42.060037 educelab-imgproc-0.3.1/src/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 17:55:42.059965 educelab-imgproc-0.3.1/src/educelab/
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 17:55:42.062020 educelab-imgproc-0.3.1/src/educelab/imgproc/
--rw-r--r--   0 seth       (501) staff       (20)      281 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/__init__.py
--rw-r--r--   0 seth       (501) staff       (20)      833 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/adjust.py
--rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/conversion.py
--rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/correction.py
--rw-r--r--   0 seth       (501) staff       (20)     3910 2023-05-10 17:49:06.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/enhance.py
--rw-r--r--   0 seth       (501) staff       (20)     1643 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/exiftool.py
--rw-r--r--   0 seth       (501) staff       (20)      241 2023-05-10 16:08:03.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/filters.py
--rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/pca.py
--rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab-imgproc-0.3.1/src/educelab/imgproc/roi.py
-drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-05-10 17:55:42.062581 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/
--rw-r--r--   0 seth       (501) staff       (20)     1357 2023-05-10 17:55:42.000000 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/PKG-INFO
--rw-r--r--   0 seth       (501) staff       (20)      565 2023-05-10 17:55:42.000000 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/SOURCES.txt
--rw-r--r--   0 seth       (501) staff       (20)        1 2023-05-10 17:55:42.000000 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/dependency_links.txt
--rw-r--r--   0 seth       (501) staff       (20)       78 2023-05-10 17:55:42.000000 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/requires.txt
--rw-r--r--   0 seth       (501) staff       (20)        9 2023-05-10 17:55:42.000000 educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/top_level.txt
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-02 14:28:29.608778 educelab-imgproc-0.4.0/
+-rw-r--r--   0 seth       (501) staff       (20)    34458 2023-03-30 17:42:22.000000 educelab-imgproc-0.4.0/LICENSE
+-rw-r--r--   0 seth       (501) staff       (20)     1357 2023-06-02 14:28:29.608826 educelab-imgproc-0.4.0/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      653 2023-04-06 00:38:08.000000 educelab-imgproc-0.4.0/README.md
+-rw-r--r--   0 seth       (501) staff       (20)      103 2023-03-30 17:42:22.000000 educelab-imgproc-0.4.0/pyproject.toml
+-rw-r--r--   0 seth       (501) staff       (20)       68 2023-06-02 14:26:57.000000 educelab-imgproc-0.4.0/requirements.txt
+-rw-r--r--   0 seth       (501) staff       (20)      918 2023-06-02 14:28:29.609062 educelab-imgproc-0.4.0/setup.cfg
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-02 14:28:29.605833 educelab-imgproc-0.4.0/src/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-02 14:28:29.605769 educelab-imgproc-0.4.0/src/educelab/
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-02 14:28:29.608133 educelab-imgproc-0.4.0/src/educelab/imgproc/
+-rw-r--r--   0 seth       (501) staff       (20)      364 2023-06-02 14:26:57.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/__init__.py
+-rw-r--r--   0 seth       (501) staff       (20)     2071 2023-06-02 14:26:57.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/adjust.py
+-rw-r--r--   0 seth       (501) staff       (20)      715 2023-04-06 00:33:44.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/conversion.py
+-rw-r--r--   0 seth       (501) staff       (20)      835 2023-04-06 00:33:44.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/correction.py
+-rw-r--r--   0 seth       (501) staff       (20)     3910 2023-05-10 17:49:06.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/enhance.py
+-rw-r--r--   0 seth       (501) staff       (20)     1643 2023-04-06 00:33:44.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/exiftool.py
+-rw-r--r--   0 seth       (501) staff       (20)      241 2023-05-10 16:08:03.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/filters.py
+-rw-r--r--   0 seth       (501) staff       (20)     2048 2023-04-06 00:33:44.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/pca.py
+-rw-r--r--   0 seth       (501) staff       (20)     5316 2023-06-02 14:26:57.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/pipeline.py
+-rw-r--r--   0 seth       (501) staff       (20)      718 2023-06-02 14:26:57.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/properties.py
+-rw-r--r--   0 seth       (501) staff       (20)     1027 2023-04-06 00:33:44.000000 educelab-imgproc-0.4.0/src/educelab/imgproc/roi.py
+drwxr-xr-x   0 seth       (501) staff       (20)        0 2023-06-02 14:28:29.608672 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/
+-rw-r--r--   0 seth       (501) staff       (20)     1357 2023-06-02 14:28:29.000000 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/PKG-INFO
+-rw-r--r--   0 seth       (501) staff       (20)      633 2023-06-02 14:28:29.000000 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/SOURCES.txt
+-rw-r--r--   0 seth       (501) staff       (20)        1 2023-06-02 14:28:29.000000 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/dependency_links.txt
+-rw-r--r--   0 seth       (501) staff       (20)      101 2023-06-02 14:28:29.000000 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/requires.txt
+-rw-r--r--   0 seth       (501) staff       (20)        9 2023-06-02 14:28:29.000000 educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/top_level.txt
```

### Comparing `educelab-imgproc-0.3.1/LICENSE` & `educelab-imgproc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/PKG-INFO` & `educelab-imgproc-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.3.1
+Version: 0.4.0
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.3.1/README.md` & `educelab-imgproc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/setup.cfg` & `educelab-imgproc-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = educelab-imgproc
-version = 0.3.1
+version = 0.4.0
 author = Seth Parker
 author_email = c.seth.parker@uky.edu
 description = EduceLab image processing module
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://educelab.gitlab.io/educelab-imgproc/
 download_url = https://gitlab.com/educelab/educelab-imgproc
```

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/conversion.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/conversion.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/correction.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/correction.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/enhance.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/enhance.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/exiftool.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/exiftool.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/pca.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/pca.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab/imgproc/roi.py` & `educelab-imgproc-0.4.0/src/educelab/imgproc/roi.py`

 * *Files identical despite different names*

### Comparing `educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/PKG-INFO` & `educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educelab-imgproc
-Version: 0.3.1
+Version: 0.4.0
 Summary: EduceLab image processing module
 Home-page: https://educelab.gitlab.io/educelab-imgproc/
 Download-URL: https://gitlab.com/educelab/educelab-imgproc
 Author: Seth Parker
 Author-email: c.seth.parker@uky.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `educelab-imgproc-0.3.1/src/educelab_imgproc.egg-info/SOURCES.txt` & `educelab-imgproc-0.4.0/src/educelab_imgproc.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,13 +7,15 @@
 src/educelab/imgproc/adjust.py
 src/educelab/imgproc/conversion.py
 src/educelab/imgproc/correction.py
 src/educelab/imgproc/enhance.py
 src/educelab/imgproc/exiftool.py
 src/educelab/imgproc/filters.py
 src/educelab/imgproc/pca.py
+src/educelab/imgproc/pipeline.py
+src/educelab/imgproc/properties.py
 src/educelab/imgproc/roi.py
 src/educelab_imgproc.egg-info/PKG-INFO
 src/educelab_imgproc.egg-info/SOURCES.txt
 src/educelab_imgproc.egg-info/dependency_links.txt
 src/educelab_imgproc.egg-info/requires.txt
 src/educelab_imgproc.egg-info/top_level.txt
```

