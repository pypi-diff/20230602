# Comparing `tmp/deepface-custom-0.0.79.tar.gz` & `tmp/deepface-custom-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepface-custom-0.0.79.tar", last modified: Fri Jun  2 08:26:59 2023, max compression
+gzip compressed data, was "deepface-custom-0.0.80.tar", last modified: Fri Jun  2 08:42:13 2023, max compression
```

## Comparing `deepface-custom-0.0.79.tar` & `deepface-custom-0.0.80.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.622134 deepface-custom-0.0.79/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/LICENSE
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:26:59.621972 deepface-custom-0.0.79/PKG-INFO
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    24826 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/README.md
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.616196 deepface-custom-0.0.79/deepface/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    30797 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/DeepFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.618011 deepface-custom-0.0.79/deepface/basemodels/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     4428 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/ArcFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2134 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/DeepID.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2254 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/DlibResNet.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       97 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/DlibWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    59157 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/Facenet.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      771 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/Facenet512.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2553 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/FbDeepFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    16727 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/OpenFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1237 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/SFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3382 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/VGGFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/basemodels/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.618520 deepface-custom-0.0.79/deepface/commons/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/commons/__init__.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1923 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/commons/distance.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    11640 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/commons/functions.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    33864 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/commons/realtime.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.620044 deepface-custom-0.0.79/deepface/detectors/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2299 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/DlibWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3656 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/FaceDetector.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2033 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/MediapipeWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/MtcnnWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3857 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/OpenCvWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1594 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/RetinaFaceWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3640 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/SsdWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/detectors/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.620802 deepface-custom-0.0.79/deepface/extendedmodels/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1835 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/extendedmodels/Age.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2377 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/extendedmodels/Emotion.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1781 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/extendedmodels/Gender.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1823 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/extendedmodels/Race.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/extendedmodels/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.620910 deepface-custom-0.0.79/deepface/models/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.79/deepface/models/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:26:59.621742 deepface-custom-0.0.79/deepface_custom.egg-info/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/PKG-INFO
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1253 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/SOURCES.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        1 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/dependency_links.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       51 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/entry_points.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      218 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/requires.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        9 2023-06-02 08:26:59.000000 deepface-custom-0.0.79/deepface_custom.egg-info/top_level.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       38 2023-06-02 08:26:59.622191 deepface-custom-0.0.79/setup.cfg
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1006 2023-06-02 08:26:45.000000 deepface-custom-0.0.79/setup.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.832631 deepface-custom-0.0.80/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/LICENSE
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:42:13.832462 deepface-custom-0.0.80/PKG-INFO
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    24826 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/README.md
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.826975 deepface-custom-0.0.80/deepface/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    30797 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/DeepFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/__init__.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.828796 deepface-custom-0.0.80/deepface/basemodels/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     4428 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/ArcFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2134 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DeepID.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2254 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DlibResNet.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       97 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DlibWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    59157 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/Facenet.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      771 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/Facenet512.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2553 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/FbDeepFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    16727 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/OpenFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1237 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/SFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3382 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/VGGFace.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/__init__.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.829299 deepface-custom-0.0.80/deepface/commons/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/__init__.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1923 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/distance.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    11640 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/functions.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    33864 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/realtime.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.830608 deepface-custom-0.0.80/deepface/detectors/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2299 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/DlibWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3656 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/FaceDetector.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2033 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/MediapipeWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/MtcnnWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3857 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/OpenCvWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1842 2023-06-02 08:37:35.000000 deepface-custom-0.0.80/deepface/detectors/RetinaFaceWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3640 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/SsdWrapper.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/__init__.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.831287 deepface-custom-0.0.80/deepface/extendedmodels/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1835 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Age.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2377 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Emotion.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1781 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Gender.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1823 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Race.py
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/__init__.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.831385 deepface-custom-0.0.80/deepface/models/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/models/__init__.py
+drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.832229 deepface-custom-0.0.80/deepface_custom.egg-info/
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/PKG-INFO
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1253 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/SOURCES.txt
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        1 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/dependency_links.txt
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       51 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/entry_points.txt
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      218 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/requires.txt
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        9 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/top_level.txt
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       38 2023-06-02 08:42:13.832683 deepface-custom-0.0.80/setup.cfg
+-rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1006 2023-06-02 08:39:15.000000 deepface-custom-0.0.80/setup.py
```

### Comparing `deepface-custom-0.0.79/LICENSE` & `deepface-custom-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/PKG-INFO` & `deepface-custom-0.0.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.79
+Version: 0.0.80
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.79/README.md` & `deepface-custom-0.0.80/README.md`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/DeepFace.py` & `deepface-custom-0.0.80/deepface/DeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/ArcFace.py` & `deepface-custom-0.0.80/deepface/basemodels/ArcFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/DeepID.py` & `deepface-custom-0.0.80/deepface/basemodels/DeepID.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/DlibResNet.py` & `deepface-custom-0.0.80/deepface/basemodels/DlibResNet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/Facenet.py` & `deepface-custom-0.0.80/deepface/basemodels/Facenet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/Facenet512.py` & `deepface-custom-0.0.80/deepface/basemodels/Facenet512.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/FbDeepFace.py` & `deepface-custom-0.0.80/deepface/basemodels/FbDeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/OpenFace.py` & `deepface-custom-0.0.80/deepface/basemodels/OpenFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/SFace.py` & `deepface-custom-0.0.80/deepface/basemodels/SFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/basemodels/VGGFace.py` & `deepface-custom-0.0.80/deepface/basemodels/VGGFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/commons/distance.py` & `deepface-custom-0.0.80/deepface/commons/distance.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/commons/functions.py` & `deepface-custom-0.0.80/deepface/commons/functions.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/commons/realtime.py` & `deepface-custom-0.0.80/deepface/commons/realtime.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/DlibWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/DlibWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/FaceDetector.py` & `deepface-custom-0.0.80/deepface/detectors/FaceDetector.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/MediapipeWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/MediapipeWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/MtcnnWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/MtcnnWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/OpenCvWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/OpenCvWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/detectors/RetinaFaceWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/RetinaFaceWrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,27 @@
     resp = []
 
     # --------------------------
 
     obj = RetinaFace.detect_faces(img, model=face_detector, threshold=0.9)
 
     if isinstance(obj, dict):
+        max_area = 0
         for face_idx in obj.keys():
             identity = obj[face_idx]
             facial_area = identity["facial_area"]
 
             y = facial_area[1]
             h = facial_area[3] - y
             x = facial_area[0]
             w = facial_area[2] - x
+            if w * h > max_area:
+                max_area = w * h
+            else:
+                continue
             img_region = [x, y, w, h]
             confidence = identity["score"]
 
             # detected_face = img[int(y):int(y+h), int(x):int(x+w)] #opencv
             detected_face = img[facial_area[1] : facial_area[3], facial_area[0] : facial_area[2]]
 
             if align:
@@ -41,10 +46,12 @@
                 # mouth_right = landmarks["mouth_right"]
                 # mouth_left = landmarks["mouth_left"]
 
                 detected_face = postprocess.alignment_procedure(
                     detected_face, right_eye, left_eye, nose
                 )
 
-            resp.append((detected_face, img_region, confidence))
-
+            if len(resp) == 0:
+                resp.append((detected_face, img_region, confidence))
+            else:
+                resp[0] = (detected_face, img_region, confidence)
     return resp
```

### Comparing `deepface-custom-0.0.79/deepface/detectors/SsdWrapper.py` & `deepface-custom-0.0.80/deepface/detectors/SsdWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/extendedmodels/Age.py` & `deepface-custom-0.0.80/deepface/extendedmodels/Age.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/extendedmodels/Emotion.py` & `deepface-custom-0.0.80/deepface/extendedmodels/Emotion.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/extendedmodels/Gender.py` & `deepface-custom-0.0.80/deepface/extendedmodels/Gender.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface/extendedmodels/Race.py` & `deepface-custom-0.0.80/deepface/extendedmodels/Race.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/deepface_custom.egg-info/PKG-INFO` & `deepface-custom-0.0.80/deepface_custom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.79
+Version: 0.0.80
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.79/deepface_custom.egg-info/SOURCES.txt` & `deepface-custom-0.0.80/deepface_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.79/setup.py` & `deepface-custom-0.0.80/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="deepface-custom",
-    version="0.0.79",
+    version="0.0.80",
     author="Sefik Ilkin Serengil, Kamoliddin Soliev",
     author_email="kamolsf8@gmail.com",
     description="A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kamoliddins/deepface",
     packages=setuptools.find_packages(),
```

