# Comparing `tmp/deepface-custom-0.0.81.tar.gz` & `tmp/deepface-custom-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepface-custom-0.0.81.tar", last modified: Fri Jun  2 10:37:06 2023, max compression
+gzip compressed data, was "deepface-custom-0.0.82.tar", last modified: Fri Jun  2 10:49:12 2023, max compression
```

## Comparing `deepface-custom-0.0.81.tar` & `deepface-custom-0.0.82.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/
--rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/LICENSE
--rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/PKG-INFO
--rw-rw-r--   0 real      (1000) real      (1000)    24826 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/README.md
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.111196 deepface-custom-0.0.81/deepface/
--rw-rw-r--   0 real      (1000) real      (1000)    30797 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/DeepFace.py
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/__init__.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/basemodels/
--rw-rw-r--   0 real      (1000) real      (1000)     4428 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/ArcFace.py
--rw-rw-r--   0 real      (1000) real      (1000)     2134 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DeepID.py
--rw-rw-r--   0 real      (1000) real      (1000)     2254 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DlibResNet.py
--rw-rw-r--   0 real      (1000) real      (1000)       97 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/DlibWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)    59157 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/Facenet.py
--rw-rw-r--   0 real      (1000) real      (1000)      771 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/Facenet512.py
--rw-rw-r--   0 real      (1000) real      (1000)     2553 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/FbDeepFace.py
--rw-rw-r--   0 real      (1000) real      (1000)    16727 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/OpenFace.py
--rw-rw-r--   0 real      (1000) real      (1000)     1237 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/SFace.py
--rw-rw-r--   0 real      (1000) real      (1000)     3382 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/VGGFace.py
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/basemodels/__init__.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/commons/
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/__init__.py
--rw-rw-r--   0 real      (1000) real      (1000)     1923 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/distance.py
--rw-rw-r--   0 real      (1000) real      (1000)    11640 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/functions.py
--rw-rw-r--   0 real      (1000) real      (1000)    33864 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/commons/realtime.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/detectors/
--rw-rw-r--   0 real      (1000) real      (1000)     2299 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/DlibWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)     3656 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/FaceDetector.py
--rw-rw-r--   0 real      (1000) real      (1000)     2033 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/MediapipeWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/MtcnnWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)     3857 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/OpenCvWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)     1842 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/RetinaFaceWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)     3640 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/SsdWrapper.py
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/detectors/__init__.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/extendedmodels/
--rw-rw-r--   0 real      (1000) real      (1000)     1835 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Age.py
--rw-rw-r--   0 real      (1000) real      (1000)     2377 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Emotion.py
--rw-rw-r--   0 real      (1000) real      (1000)     1781 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Gender.py
--rw-rw-r--   0 real      (1000) real      (1000)     1823 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/Race.py
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/extendedmodels/__init__.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface/models/
--rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.81/deepface/models/__init__.py
-drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/deepface_custom.egg-info/
--rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/PKG-INFO
--rw-rw-r--   0 real      (1000) real      (1000)     1253 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/SOURCES.txt
--rw-rw-r--   0 real      (1000) real      (1000)        1 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/dependency_links.txt
--rw-rw-r--   0 real      (1000) real      (1000)       51 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/entry_points.txt
--rw-rw-r--   0 real      (1000) real      (1000)      218 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/requires.txt
--rw-rw-r--   0 real      (1000) real      (1000)        9 2023-06-02 10:37:06.000000 deepface-custom-0.0.81/deepface_custom.egg-info/top_level.txt
--rw-rw-r--   0 real      (1000) real      (1000)       38 2023-06-02 10:37:06.115196 deepface-custom-0.0.81/setup.cfg
--rw-rw-r--   0 real      (1000) real      (1000)     1006 2023-06-02 10:36:56.000000 deepface-custom-0.0.81/setup.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/
+-rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/LICENSE
+-rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/PKG-INFO
+-rw-rw-r--   0 real      (1000) real      (1000)    24826 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/README.md
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/
+-rw-rw-r--   0 real      (1000) real      (1000)    30797 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/DeepFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/basemodels/
+-rw-rw-r--   0 real      (1000) real      (1000)     4428 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/ArcFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2134 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/DeepID.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2254 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/DlibResNet.py
+-rw-rw-r--   0 real      (1000) real      (1000)       97 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/DlibWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)    59157 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/Facenet.py
+-rw-rw-r--   0 real      (1000) real      (1000)      771 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/Facenet512.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2553 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/FbDeepFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)    16727 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/OpenFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1237 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/SFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3382 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/VGGFace.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/basemodels/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/commons/
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/commons/__init__.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1923 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/commons/distance.py
+-rw-rw-r--   0 real      (1000) real      (1000)    11640 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/commons/functions.py
+-rw-rw-r--   0 real      (1000) real      (1000)    33864 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/commons/realtime.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/detectors/
+-rw-rw-r--   0 real      (1000) real      (1000)     2299 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/DlibWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3656 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/FaceDetector.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2033 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/MediapipeWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1076 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/MtcnnWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3857 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/OpenCvWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1842 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/RetinaFaceWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)     3640 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/SsdWrapper.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/detectors/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/extendedmodels/
+-rw-rw-r--   0 real      (1000) real      (1000)     1835 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/extendedmodels/Age.py
+-rw-rw-r--   0 real      (1000) real      (1000)     2377 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/extendedmodels/Emotion.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1781 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/extendedmodels/Gender.py
+-rw-rw-r--   0 real      (1000) real      (1000)     1823 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/extendedmodels/Race.py
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/extendedmodels/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface/models/
+-rw-rw-r--   0 real      (1000) real      (1000)        0 2023-06-02 10:18:47.000000 deepface-custom-0.0.82/deepface/models/__init__.py
+drwxrwxr-x   0 real      (1000) real      (1000)        0 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/deepface_custom.egg-info/
+-rw-rw-r--   0 real      (1000) real      (1000)    25372 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/PKG-INFO
+-rw-rw-r--   0 real      (1000) real      (1000)     1253 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/SOURCES.txt
+-rw-rw-r--   0 real      (1000) real      (1000)        1 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/dependency_links.txt
+-rw-rw-r--   0 real      (1000) real      (1000)       51 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/entry_points.txt
+-rw-rw-r--   0 real      (1000) real      (1000)      218 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/requires.txt
+-rw-rw-r--   0 real      (1000) real      (1000)        9 2023-06-02 10:49:12.000000 deepface-custom-0.0.82/deepface_custom.egg-info/top_level.txt
+-rw-rw-r--   0 real      (1000) real      (1000)       38 2023-06-02 10:49:12.695160 deepface-custom-0.0.82/setup.cfg
+-rw-rw-r--   0 real      (1000) real      (1000)     1198 2023-06-02 10:49:11.000000 deepface-custom-0.0.82/setup.py
```

### Comparing `deepface-custom-0.0.81/LICENSE` & `deepface-custom-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/PKG-INFO` & `deepface-custom-0.0.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.81
+Version: 0.0.82
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.81/README.md` & `deepface-custom-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/DeepFace.py` & `deepface-custom-0.0.82/deepface/DeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/ArcFace.py` & `deepface-custom-0.0.82/deepface/basemodels/ArcFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/DeepID.py` & `deepface-custom-0.0.82/deepface/basemodels/DeepID.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/DlibResNet.py` & `deepface-custom-0.0.82/deepface/basemodels/DlibResNet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/Facenet.py` & `deepface-custom-0.0.82/deepface/basemodels/Facenet.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/Facenet512.py` & `deepface-custom-0.0.82/deepface/basemodels/Facenet512.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/FbDeepFace.py` & `deepface-custom-0.0.82/deepface/basemodels/FbDeepFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/OpenFace.py` & `deepface-custom-0.0.82/deepface/basemodels/OpenFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/SFace.py` & `deepface-custom-0.0.82/deepface/basemodels/SFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/basemodels/VGGFace.py` & `deepface-custom-0.0.82/deepface/basemodels/VGGFace.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/commons/distance.py` & `deepface-custom-0.0.82/deepface/commons/distance.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/commons/functions.py` & `deepface-custom-0.0.82/deepface/commons/functions.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/commons/realtime.py` & `deepface-custom-0.0.82/deepface/commons/realtime.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/DlibWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/DlibWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/FaceDetector.py` & `deepface-custom-0.0.82/deepface/detectors/FaceDetector.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/MediapipeWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/MediapipeWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/MtcnnWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/MtcnnWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/OpenCvWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/OpenCvWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/RetinaFaceWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/RetinaFaceWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/detectors/SsdWrapper.py` & `deepface-custom-0.0.82/deepface/detectors/SsdWrapper.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/extendedmodels/Age.py` & `deepface-custom-0.0.82/deepface/extendedmodels/Age.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/extendedmodels/Emotion.py` & `deepface-custom-0.0.82/deepface/extendedmodels/Emotion.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/extendedmodels/Gender.py` & `deepface-custom-0.0.82/deepface/extendedmodels/Gender.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface/extendedmodels/Race.py` & `deepface-custom-0.0.82/deepface/extendedmodels/Race.py`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/deepface_custom.egg-info/PKG-INFO` & `deepface-custom-0.0.82/deepface_custom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepface-custom
-Version: 0.0.81
+Version: 0.0.82
 Summary: A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python
 Home-page: https://github.com/kamoliddins/deepface
 Author: Sefik Ilkin Serengil, Kamoliddin Soliev
 Author-email: kamolsf8@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `deepface-custom-0.0.81/deepface_custom.egg-info/SOURCES.txt` & `deepface-custom-0.0.82/deepface_custom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepface-custom-0.0.81/setup.py` & `deepface-custom-0.0.82/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", "r", encoding="utf-8") as f:
-    requirements = f.read().split("\n")
-
 setuptools.setup(
     name="deepface-custom",
-    version="0.0.81",
+    version="0.0.82",
     author="Sefik Ilkin Serengil, Kamoliddin Soliev",
     author_email="kamolsf8@gmail.com",
     description="A Lightweight Face Recognition and Facial Attribute Analysis Framework (Age, Gender, Emotion, Race) for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kamoliddins/deepface",
     packages=setuptools.find_packages(),
@@ -21,9 +18,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         "console_scripts": ["deepface = deepface.DeepFace:cli"],
     },
     python_requires=">=3.5.5",
-    install_requires=requirements,
+    install_requires=['numpy>=1.14.0', 'pandas>=0.23.4', 'gdown>=3.10.1', 'tqdm>=4.30.0', 'Pillow>=5.2.0',
+                      'opencv-python>=4.5.5.64', 'tensorflow>=1.9.0', 'keras>=2.2.0', 'Flask>=1.1.2', 'mtcnn>=0.1.0',
+                      'retina-face>=0.0.1', 'fire>=0.4.0', 'gunicorn>=20.1.0', 'Deprecated>=1.2.13'],
 )
```

