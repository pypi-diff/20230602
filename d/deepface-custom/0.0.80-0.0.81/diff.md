# Comparing `tmp/deepface-custom-0.0.80.tar.gz` & `tmp/deepface-custom-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepface-custom-0.0.80.tar", last modified: Fri Jun  2 08:42:13 2023, max compression
+gzip compressed data, was "deepface-custom-0.0.81.tar", last modified: Fri Jun  2 10:37:06 2023, max compression
```

## Comparing `deepface-custom-0.0.80.tar` & `deepface-custom-0.0.81.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.832631 deepface-custom-0.0.80/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/LICENSE
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:42:13.832462 deepface-custom-0.0.80/PKG-INFO
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    24826 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/README.md
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.826975 deepface-custom-0.0.80/deepface/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    30797 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/DeepFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.828796 deepface-custom-0.0.80/deepface/basemodels/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     4428 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/ArcFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2134 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DeepID.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2254 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DlibResNet.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       97 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/DlibWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    59157 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/Facenet.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      771 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/Facenet512.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2553 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/FbDeepFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    16727 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/OpenFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1237 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/SFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3382 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/VGGFace.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/basemodels/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.829299 deepface-custom-0.0.80/deepface/commons/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/__init__.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1923 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/distance.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    11640 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/functions.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    33864 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/commons/realtime.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.830608 deepface-custom-0.0.80/deepface/detectors/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2299 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/DlibWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3656 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/FaceDetector.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2033 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/MediapipeWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1076 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/MtcnnWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3857 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/OpenCvWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1842 2023-06-02 08:37:35.000000 deepface-custom-0.0.80/deepface/detectors/RetinaFaceWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     3640 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/SsdWrapper.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/detectors/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.831287 deepface-custom-0.0.80/deepface/extendedmodels/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1835 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Age.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     2377 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Emotion.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1781 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Gender.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1823 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/Race.py
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/extendedmodels/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.831385 deepface-custom-0.0.80/deepface/models/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 06:44:01.000000 deepface-custom-0.0.80/deepface/models/__init__.py
-drwxr-xr-x   0 kamoliddinsoliev   (501) staff       (20)        0 2023-06-02 08:42:13.832229 deepface-custom-0.0.80/deepface_custom.egg-info/
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)    25372 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/PKG-INFO
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1253 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/SOURCES.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        1 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/dependency_links.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       51 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/entry_points.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)      218 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/requires.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)        9 2023-06-02 08:42:13.000000 deepface-custom-0.0.80/deepface_custom.egg-info/top_level.txt
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)       38 2023-06-02 08:42:13.832683 deepface-custom-0.0.80/setup.cfg
--rw-r--r--   0 kamoliddinsoliev   (501) staff       (20)     1006 2023-06-02 08:39:15.000000 deepface-custom-0.0.80/setup.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/
+-rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/LICENSE
+-rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/PKG-INFO
+-rw-rw-r--   0 real      (1000) real      (1000)    24826 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/README.md
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.111196 deepface-custom-0.0.81/deepface/
+-rw-rw-r--   0 real      (1000) real      (1000)    30797 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/DeepFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/basemodels/
+-rw-rw-r--   0 real      (1000) real      (1000)     4428 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/ArcFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2134 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DeepID.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2254 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DlibResNet.py
+-rw-rw-r--   0 real      (1000) real      (1000)       97 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DlibWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)    59157 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/Facenet.py
+-rw-rw-r--   0 real      (1000) real      (1000)      771 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/Facenet512.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2553 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/FbDeepFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)    16727 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/OpenFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1237 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/SFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3382 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/VGGFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/commons/
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/__init__.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1923 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/distance.py
+-rw-rw-r--   0 real      (1000) real      (1000)    11640 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/functions.py
+-rw-rw-r--   0 real      (1000) real      (1000)    33864 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/realtime.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/detectors/
+-rw-rw-r--   0 real      (1000) real      (1000)     2299 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/DlibWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3656 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/FaceDetector.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2033 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/MediapipeWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/MtcnnWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3857 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/OpenCvWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1842 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/RetinaFaceWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3640 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/SsdWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/extendedmodels/
+-rw-rw-r--   0 real      (1000) real      (1000)     1835 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Age.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2377 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Emotion.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1781 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Gender.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1823 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Race.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/models/
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/models/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface_custom.egg-info/
+-rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/PKG-INFO
+-rw-rw-r--   0 real      (1000) real      (1000)     1253 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/SOURCES.txt
+-rw-rw-r--   0 real      (1000) real      (1000)        1 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/dependency_links.txt
+-rw-rw-r--   0 real      (1000) real      (1000)       51 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/entry_points.txt
+-rw-rw-r--   0 real      (1000) real      (1000)      218 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/requires.txt
+-rw-rw-r--   0 real      (1000) real      (1000)        9 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/top_level.txt
+-rw-rw-r--   0 real      (1000) real      (1000)       38 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/setup.cfg
+-rw-rw-r--   0 real      (1000) real      (1000)     1006 2023-06-02 10:36:56.000000 deepface-custom-0.0.81/setup.py
```

### Comparing `deepface-custom-0.0.80/LICENSE` & `deepface-custom-0.0.81/LICENSE`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/PKG-INFO` & `deepface-custom-0.0.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.80
+Version: 0.0.81
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.80/README.md` & `deepface-custom-0.0.81/README.md`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/DeepFace.py` & `deepface-custom-0.0.81/deepface/DeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/ArcFace.py` & `deepface-custom-0.0.81/deepface/basemodels/ArcFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/DeepID.py` & `deepface-custom-0.0.81/deepface/basemodels/DeepID.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/DlibResNet.py` & `deepface-custom-0.0.81/deepface/basemodels/DlibResNet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/Facenet.py` & `deepface-custom-0.0.81/deepface/basemodels/Facenet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/Facenet512.py` & `deepface-custom-0.0.81/deepface/basemodels/Facenet512.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/FbDeepFace.py` & `deepface-custom-0.0.81/deepface/basemodels/FbDeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/OpenFace.py` & `deepface-custom-0.0.81/deepface/basemodels/OpenFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/SFace.py` & `deepface-custom-0.0.81/deepface/basemodels/SFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/basemodels/VGGFace.py` & `deepface-custom-0.0.81/deepface/basemodels/VGGFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/commons/distance.py` & `deepface-custom-0.0.81/deepface/commons/distance.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/commons/functions.py` & `deepface-custom-0.0.81/deepface/commons/functions.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/commons/realtime.py` & `deepface-custom-0.0.81/deepface/commons/realtime.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/DlibWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/DlibWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/FaceDetector.py` & `deepface-custom-0.0.81/deepface/detectors/FaceDetector.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/MediapipeWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/MediapipeWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/MtcnnWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/MtcnnWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/OpenCvWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/OpenCvWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/RetinaFaceWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/RetinaFaceWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/detectors/SsdWrapper.py` & `deepface-custom-0.0.81/deepface/detectors/SsdWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/extendedmodels/Age.py` & `deepface-custom-0.0.81/deepface/extendedmodels/Age.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/extendedmodels/Emotion.py` & `deepface-custom-0.0.81/deepface/extendedmodels/Emotion.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/extendedmodels/Gender.py` & `deepface-custom-0.0.81/deepface/extendedmodels/Gender.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface/extendedmodels/Race.py` & `deepface-custom-0.0.81/deepface/extendedmodels/Race.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/deepface_custom.egg-info/PKG-INFO` & `deepface-custom-0.0.81/deepface_custom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.80
+Version: 0.0.81
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.80/deepface_custom.egg-info/SOURCES.txt` & `deepface-custom-0.0.81/deepface_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.80/setup.py` & `deepface-custom-0.0.81/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="deepface-custom",
-    version="0.0.80",
+    version="0.0.81",
     author="Sefik Ilkin Serengil, Kamoliddin Soliev",
     author_email="kamolsf8@gmail.com",
     description="A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kamoliddins/deepface",
     packages=setuptools.find_packages(),
```

