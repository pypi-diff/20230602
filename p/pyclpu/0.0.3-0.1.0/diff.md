# Comparing `tmp/pyclpu-0.0.3.tar.gz` & `tmp/pyclpu-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyclpu-0.0.3.tar", last modified: Fri Jun  2 08:53:10 2023, max compression
+gzip compressed data, was "dist\pyclpu-0.1.0.tar", last modified: Fri Jun  2 09:57:51 2023, max compression
```

## Comparing `pyclpu-0.0.3.tar` & `pyclpu-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/
--rw-rw-rw-   0        0        0      382 2023-06-02 08:53:10.000000 pyclpu-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu/
--rw-rw-rw-   0        0        0     1878 2023-06-01 14:29:35.000000 pyclpu-0.0.3/pyclpu/constants.py
--rw-rw-rw-   0        0        0      942 2022-04-16 17:02:37.000000 pyclpu-0.0.3/pyclpu/formats.py
--rw-rw-rw-   0        0        0    17931 2023-06-02 08:49:07.000000 pyclpu-0.0.3/pyclpu/image.py
--rw-rw-rw-   0        0        0    30733 2023-05-31 09:32:25.000000 pyclpu-0.0.3/pyclpu/main.py
--rw-rw-rw-   0        0        0     7425 2022-04-16 17:02:37.000000 pyclpu-0.0.3/pyclpu/s33293804.py
--rw-rw-rw-   0        0        0      629 2023-06-02 08:52:40.000000 pyclpu-0.0.3/pyclpu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/
--rw-rw-rw-   0        0        0        1 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      382 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       23 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/requires.txt
--rw-rw-rw-   0        0        0      285 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 08:53:10.000000 pyclpu-0.0.3/pyclpu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1049 2023-06-01 16:05:31.000000 pyclpu-0.0.3/README.md
--rw-rw-rw-   0        0        0       92 2023-06-02 08:53:10.000000 pyclpu-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1803 2023-06-02 08:36:58.000000 pyclpu-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/
+-rw-rw-rw-   0        0        0      382 2023-06-02 09:57:51.000000 pyclpu-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu/
+-rw-rw-rw-   0        0        0     1878 2023-06-01 14:29:35.000000 pyclpu-0.1.0/pyclpu/constants.py
+-rw-rw-rw-   0        0        0      942 2022-04-16 17:02:37.000000 pyclpu-0.1.0/pyclpu/formats.py
+-rw-rw-rw-   0        0        0    19125 2023-06-02 09:47:41.000000 pyclpu-0.1.0/pyclpu/image.py
+-rw-rw-rw-   0        0        0    30733 2023-05-31 09:32:25.000000 pyclpu-0.1.0/pyclpu/main.py
+-rw-rw-rw-   0        0        0     7425 2022-04-16 17:02:37.000000 pyclpu-0.1.0/pyclpu/s33293804.py
+-rw-rw-rw-   0        0        0      629 2023-06-02 08:58:53.000000 pyclpu-0.1.0/pyclpu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      382 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      285 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 09:57:51.000000 pyclpu-0.1.0/pyclpu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2558 2023-06-02 09:30:25.000000 pyclpu-0.1.0/README.md
+-rw-rw-rw-   0        0        0       92 2023-06-02 09:57:51.000000 pyclpu-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1827 2023-06-02 09:41:36.000000 pyclpu-0.1.0/setup.py
```

### Comparing `pyclpu-0.0.3/pyclpu/constants.py` & `pyclpu-0.1.0/pyclpu/constants.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.3/pyclpu/formats.py` & `pyclpu-0.1.0/pyclpu/formats.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.3/pyclpu/image.py` & `pyclpu-0.1.0/pyclpu/image.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,14 @@
 # =============================================================================
 # EXTERNAL
 import os
 import sys
 from inspect import getsourcefile
 from importlib import reload
 
-import warnings
-
 import math
 import numpy as np
 
 import cv2
 import PIL
 
 # INTERNAL
@@ -275,26 +273,31 @@
         #1) Create from this class as cls a new instance of an object Main
         return Main(*args, **kwargs)
         
 class PointPicker():
     """
     The class allows interactive picking of a veriable number of points in a picture.
     
-    Call as a = image.PointPicker("n" = 4, image = image.imread("C:\\Users\\mehret\\GIT\\pyclpu\\pyclpu\\test.jpg"))
+    Call as a = image.PointPicker("n" = 4, image = image.imread("path/to/test.jpg"))
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
         # INTEGRITY
         if not hasattr(self, 'image'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `image` as `image=IMG`.")
         if not hasattr(self, 'n'):
             warning(self.__class__.__name__,"No number of points defined, expect key `n` as `n=INT`.")
+        # IN PLACE
+        if hasattr(self, 'image') and hasattr(self, 'n'):
+            self.__run__()
+        return None
+    def __run__(self):    
         # VARIABLES
         self.point_list = np.zeros((self.n, 2), dtype = "int")
         self.point_list_pointer = 0
         # METHODS
         def click_and_get(event, x, y, flags, param):
             '''
             HELPER FUNCTION: CLICK EVENT FUNCTION
@@ -316,15 +319,15 @@
                 self.point_list[self.point_list_pointer,1] = 0
             # draw points in the open named canvas outside the function
             self.drawing = self.enhanced.copy()
             for point in self.point_list:
                 if point[0] != 0 and point[1] != 0:
                     cv2.circle(self.drawing, (point[0],point[1]), 10, (255, 10, 10), -1)
             cv2.imshow(self.__class__.__name__, self.drawing)
-        # IN PLACE
+        # MAIN
         # prepare display
         self.enhanced = enhanced_visibility(self.image)
         self.drawing = self.enhanced.copy()
         # print instructions
         message(self.__class__.__name__,"PRESS LEFT MOUSE BUTTON TO ADD NEW POINT\nPRESS RIGHT MOUSE BUTTON TO REMOVE LAST POINT\nPRESS C TO CONFIRM SELECTION\nPRESS R KEY TO RESET\nPRESS Q KEY TO QUIT",headline="SELECT POINT")
         # create canvas and start dialogue
         cv2.namedWindow(self.__class__.__name__)
@@ -348,35 +351,70 @@
         else:
             self.status = True
         # housekeeping
         cv2.destroyAllWindows()
         del self.image
         del self.enhanced
         del self.drawing
+        return None
 
 # IMAGE MANIPULATION
 class Manipulate:
     def __new__(cls, *args, **kwargs):
         #1) Create from this class as cls a new instance of an object Main
         return Main(*args, **kwargs)
         
 class PerspectiveTransform():
     """
-    The class transforms a linearly distorted input image into a trapez-corrected view on it. Coordinates are interpreted as (x,y).
+    The class allows to transform a linearly distorted input image into a trapez-corrected view on it. Coordinates are interpreted as (x,y).
     
-    Call as b = image.PerspectiveTransform(source = image.imread("C:\\Users\\mehret\\GIT\\pyclpu\\pyclpu\\test.jpg"))
+    The class can be used in a functional way
+
+    ```
+    from pyclpu import image
+
+    warp = image.PerspectiveTransform(source = image.imread("path/to/test.jpg")) 
+    ```
+
+    with the warped image in `warp.warped` and the coordinates of cornes from the source image stored in `sourcecorners`. Note that the source image is not part of the object in its final form. A more object oriented use case can deal with loops where all warps have the same source corner coordinates
+
+    ```
+    from pyclpu import image
+
+    warp_it = image.PerspectiveTransform()
+
+    image_stack = image.imread(path/to/directory/with/many/images/)
+
+    warp = []
+
+    for image in image_stack:
+        warp_it.source = image
+        warp.append[{"warped" : warp.warped, "sourcecorners" : warp.sourcecorners}]
+    ```
+
+    with results beeing stored in a list `warp`.
     """
     # INI
     def __new__(cls, *args, **kwargs):
         return super().__new__(cls)
     def __init__(self, *args, **kwargs):
         self.__dict__.update(kwargs)
         # INTEGRITY
         if not hasattr(self, 'source'):
             warning(self.__class__.__name__,"No source image `IMG` defined, expect key `source` as `source=IMG`.")
+        # IN PLACE
+        if hasattr(self, 'source'):
+            self.__run__()
+        return None
+    def __setattr__(self, name, value):
+        super().__setattr__(name, value)
+        if name == "source":
+            self.__run__()
+        return None
+    def __run__(self):
         # METHODS
         def order_points(pts):
             """
             Orders automatically a list of coordinates of (rectangular) image corners as follows: top-left, top-right, bottom-right, bottom-left.
             """
             rect = np.zeros((4, 2), dtype = "float32")
             s = pts.sum(axis = 1)
@@ -407,24 +445,25 @@
                 [maxWidth - 1, maxHeight - 1],
                 [0, maxHeight - 1]], dtype = "float32")
             # compute perspective transform matrix and apply it
             M = cv2.getPerspectiveTransform(rect, dst)
             warped = cv2.warpPerspective(image, M, (maxWidth, maxHeight))
             # return the warped image
             return warped    
-        # IN PLACE
+        # MAIN
         self.sourcecorners = PointPicker(image=self.source,n=4)
         self.warped = four_point_transform(self.source, self.sourcecorners.point_list)
         message(self.__class__.__name__,"PRESS ANY KEY TO CLOSE IMAGE AND PROCEED",headline="DISPLAY WARP")
         cv2.namedWindow(self.__class__.__name__)
         cv2.imshow(self.__class__.__name__, self.warped)
         cv2.waitKey(0)
         # housekeeping
         cv2.destroyAllWindows()
         del self.source
+        return None
         
     
 # =============================================================================
 # PYTHON MAIN
 # =============================================================================
 # SELF AND TEST
 if globals()["__name__"] == '__main__':
```

### Comparing `pyclpu-0.0.3/pyclpu/main.py` & `pyclpu-0.1.0/pyclpu/main.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.3/pyclpu/s33293804.py` & `pyclpu-0.1.0/pyclpu/s33293804.py`

 * *Files identical despite different names*

### Comparing `pyclpu-0.0.3/pyclpu/__init__.py` & `pyclpu-0.1.0/pyclpu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 pyclpu.
 
 CLPU Utilities.
 """
 # main attributes
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 __author__ = 'Michael Ehret'
 __credits__ = 'Centro de Laseres Pulsados, Villamayor, Spain'
 
 """
 DEVELOPMENT ZONE
 
 Until the following is not resolved, attributes below __init__.py require manual import as from pyclpu import ATTRIBUTE
```

### Comparing `pyclpu-0.0.3/setup.py` & `pyclpu-0.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,17 @@
     author='Michael Ehret',\
     author_email='mehret@clpu.es',\
     url='https://git.clpu.es/mehret/pyclpu',\
     license='MIT',\
     packages=['pyclpu'],
     scripts=glob.glob("pyclpu/*.py"),
     install_requires=[\
-        'numpy','scipy',\
+        'numpy','scipy','opencv-python','cython','pillow',\
         'matplotlib',\
     ],\
-    # and build in modules cython, importlib.reload, inspect.getsourcefile, glob, math, opencv, pillow, os, sys, time, warnings
+    # and build in modules cython, importlib.reload, inspect.getsourcefile, glob, math, opencv, pillow, os, sys, time
     classifiers=[\
         'Development Status :: 1 - Planning',\
         'Intended Audience :: Science/Research',\
         'Programming Language :: Python :: 3.5',\
     ],\
 )
```

