# Comparing `tmp/cerc-geometry-2.1.2.tar.gz` & `tmp/cerc-geometry-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-je2gv9gy/cerc-geometry-2.1.2.tar", last modified: Fri May 26 01:53:36 2023, max compression
+gzip compressed data, was "/Users/peteryefi/Desktop/dompark/geometry/dist/.tmp-gb3gx4ft/cerc-geometry-2.1.3.tar", last modified: Thu Jun  1 23:13:19 2023, max compression
```

## Comparing `cerc-geometry-2.1.2.tar` & `cerc-geometry-2.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.775304 cerc-geometry-2.1.2/
--rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.1.2/LICENSE.md
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-26 01:53:36.774974 cerc-geometry-2.1.2/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.1.2/README.md
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.730580 cerc-geometry-2.1.2/cerc_geometry.egg-info/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-05-26 01:53:36.000000 cerc-geometry-2.1.2/cerc_geometry.egg-info/PKG-INFO
--rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-05-26 01:53:36.000000 cerc-geometry-2.1.2/cerc_geometry.egg-info/SOURCES.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-05-26 01:53:36.000000 cerc-geometry-2.1.2/cerc_geometry.egg-info/dependency_links.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       56 2023-05-26 01:53:36.000000 cerc-geometry-2.1.2/cerc_geometry.egg-info/requires.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-05-26 01:53:36.000000 cerc-geometry-2.1.2/cerc_geometry.egg-info/top_level.txt
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.739199 cerc-geometry-2.1.2/geometry/
--rw-r--r--   0 peteryefi   (501) staff       (20)      200 2023-05-19 00:02:34.000000 cerc-geometry-2.1.2/geometry/__init__.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.726076 cerc-geometry-2.1.2/geometry/data/
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.739870 cerc-geometry-2.1.2/geometry/data/geolocation/
--rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.1.2/geometry/data/geolocation/cities15000.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)     5687 2023-05-26 01:30:59.000000 cerc-geometry-2.1.2/geometry/helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    11128 2023-05-24 23:38:41.000000 cerc-geometry-2.1.2/geometry/library.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      574 2023-05-18 23:39:06.000000 cerc-geometry-2.1.2/geometry/location.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      707 2023-05-18 23:38:20.000000 cerc-geometry-2.1.2/geometry/map_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     2168 2023-05-15 23:21:05.000000 cerc-geometry-2.1.2/geometry/plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1002 2023-05-15 23:21:05.000000 cerc-geometry-2.1.2/geometry/point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)    14604 2023-05-16 00:05:51.000000 cerc-geometry-2.1.2/geometry/polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     6590 2023-05-15 23:21:05.000000 cerc-geometry-2.1.2/geometry/polyhedron.py
--rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.1.2/pyproject.toml
--rw-r--r--   0 peteryefi   (501) staff       (20)       45 2023-05-26 01:51:38.000000 cerc-geometry-2.1.2/requirements.txt
--rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-05-26 01:53:36.775422 cerc-geometry-2.1.2/setup.cfg
--rw-r--r--   0 peteryefi   (501) staff       (20)     1446 2023-05-26 01:53:08.000000 cerc-geometry-2.1.2/setup.py
-drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-05-26 01:53:36.774334 cerc-geometry-2.1.2/tests/
--rw-r--r--   0 peteryefi   (501) staff       (20)     1961 2023-05-16 00:05:50.000000 cerc-geometry-2.1.2/tests/test_helper.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      736 2023-05-16 00:05:50.000000 cerc-geometry-2.1.2/tests/test_plane.py
--rw-r--r--   0 peteryefi   (501) staff       (20)      842 2023-05-16 00:05:50.000000 cerc-geometry-2.1.2/tests/test_point.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1513 2023-05-16 00:05:50.000000 cerc-geometry-2.1.2/tests/test_polygon.py
--rw-r--r--   0 peteryefi   (501) staff       (20)     1076 2023-05-16 00:05:50.000000 cerc-geometry-2.1.2/tests/test_polyhedron.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.732941 cerc-geometry-2.1.3/
+-rw-rw-rw-   0 peteryefi   (501) staff       (20)     7431 2023-05-11 00:53:33.000000 cerc-geometry-2.1.3/LICENSE.md
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-06-01 23:13:19.732569 cerc-geometry-2.1.3/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      522 2023-05-12 17:30:08.000000 cerc-geometry-2.1.3/README.md
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.688977 cerc-geometry-2.1.3/cerc_geometry.egg-info/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1269 2023-06-01 23:13:19.000000 cerc-geometry-2.1.3/cerc_geometry.egg-info/PKG-INFO
+-rw-r--r--   0 peteryefi   (501) staff       (20)      577 2023-06-01 23:13:19.000000 cerc-geometry-2.1.3/cerc_geometry.egg-info/SOURCES.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        1 2023-06-01 23:13:19.000000 cerc-geometry-2.1.3/cerc_geometry.egg-info/dependency_links.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       56 2023-06-01 23:13:19.000000 cerc-geometry-2.1.3/cerc_geometry.egg-info/requires.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)        9 2023-06-01 23:13:19.000000 cerc-geometry-2.1.3/cerc_geometry.egg-info/top_level.txt
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.695704 cerc-geometry-2.1.3/geometry/
+-rw-r--r--   0 peteryefi   (501) staff       (20)      237 2023-06-01 00:26:41.000000 cerc-geometry-2.1.3/geometry/__init__.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.684686 cerc-geometry-2.1.3/geometry/data/
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.696340 cerc-geometry-2.1.3/geometry/data/geolocation/
+-rw-r--r--   0 peteryefi   (501) staff       (20)  6284352 2023-05-12 21:46:09.000000 cerc-geometry-2.1.3/geometry/data/geolocation/cities15000.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)     5690 2023-06-01 23:07:58.000000 cerc-geometry-2.1.3/geometry/helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    14161 2023-06-01 01:57:34.000000 cerc-geometry-2.1.3/geometry/library.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      631 2023-06-01 01:59:17.000000 cerc-geometry-2.1.3/geometry/location.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)      778 2023-06-01 01:59:32.000000 cerc-geometry-2.1.3/geometry/map_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2550 2023-06-01 21:14:32.000000 cerc-geometry-2.1.3/geometry/plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1148 2023-06-01 02:09:56.000000 cerc-geometry-2.1.3/geometry/point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)    17151 2023-06-01 21:22:52.000000 cerc-geometry-2.1.3/geometry/polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     8059 2023-06-01 21:36:30.000000 cerc-geometry-2.1.3/geometry/polyhedron.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)       99 2023-05-15 23:40:38.000000 cerc-geometry-2.1.3/pyproject.toml
+-rw-r--r--   0 peteryefi   (501) staff       (20)       45 2023-05-26 01:51:38.000000 cerc-geometry-2.1.3/requirements.txt
+-rw-r--r--   0 peteryefi   (501) staff       (20)       38 2023-06-01 23:13:19.733064 cerc-geometry-2.1.3/setup.cfg
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1446 2023-06-01 23:12:33.000000 cerc-geometry-2.1.3/setup.py
+drwxr-xr-x   0 peteryefi   (501) staff       (20)        0 2023-06-01 23:13:19.731869 cerc-geometry-2.1.3/tests/
+-rw-r--r--   0 peteryefi   (501) staff       (20)     2788 2023-06-01 22:40:02.000000 cerc-geometry-2.1.3/tests/test_helper.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1136 2023-06-01 22:33:11.000000 cerc-geometry-2.1.3/tests/test_plane.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1317 2023-06-01 22:29:44.000000 cerc-geometry-2.1.3/tests/test_point.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1841 2023-06-01 22:24:28.000000 cerc-geometry-2.1.3/tests/test_polygon.py
+-rw-r--r--   0 peteryefi   (501) staff       (20)     1387 2023-06-01 22:23:02.000000 cerc-geometry-2.1.3/tests/test_polyhedron.py
```

### Comparing `cerc-geometry-2.1.2/LICENSE.md` & `cerc-geometry-2.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.1.2/PKG-INFO` & `cerc-geometry-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.1.2
+Version: 2.1.3
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.1.2/README.md` & `cerc-geometry-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.1.2/cerc_geometry.egg-info/PKG-INFO` & `cerc-geometry-2.1.3/cerc_geometry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerc-geometry
-Version: 2.1.2
+Version: 2.1.3
 Summary: CERC Geometry Library with different modules to manipulate geometric objects
 Home-page: https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Author: CERC
 Author-email:  cerc@concordia.ca
 Project-URL: Repository, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry
 Project-URL: Bug Tracker, https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cerc-geometry-2.1.2/cerc_geometry.egg-info/SOURCES.txt` & `cerc-geometry-2.1.3/cerc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.1.2/geometry/data/geolocation/cities15000.txt` & `cerc-geometry-2.1.3/geometry/data/geolocation/cities15000.txt`

 * *Files identical despite different names*

### Comparing `cerc-geometry-2.1.2/geometry/helper.py` & `cerc-geometry-2.1.3/geometry/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import numpy as np
 from typing import List
 import sys
 import math
 
 
 class Helper(object):
-
     _instance = None
 
     def __init__(self):
         raise RuntimeError('Call instance() instead')
 
     @classmethod
     def instance(cls):
@@ -43,15 +42,15 @@
     def points_from_string(cls, coordinates: str) -> np.ndarray:
         """
         Converts a string of coordinates go a point matrix
         :param coordinates: "x y z..."
         :return: [[x,y,z],[x,y,z]...]
         """
         try:
-            points = np.fromstring(coordinates, dtype=float, sep=' ')
+            points = np.array([float(string_coordinate) for string_coordinate in coordinates.split()])
             points = cls.to_points_matrix(points)
             return points
         except TypeError:
             sys.stderr.write('Expect coordinates to be a string of floats separated by spaces')
         except Exception as error:
             sys.stderr.write(f'An error occurred: {error}')
 
@@ -61,15 +60,15 @@
         Transform citygml surface names into hub names
         """
         if surface == 'WallSurface':
             return 'Wall'
         if surface == 'GroundSurface':
             return 'Ground'
         return 'Roof'
-        
+
     @classmethod
     def remove_last_point_from_string(cls, points: str) -> str:
         """
         Ignore last point in a string of points
         :param points:
         :return:
         """
@@ -94,15 +93,15 @@
             for point in points:
                 res.insert(0, point)
             return res
         except TypeError:
             sys.stderr.write('Expects point to be a list')
         except Exception as error:
             sys.stderr.write(f'An error occurred: {error}')
-        
+
     @classmethod
     def ground_area(cls, points: List) -> float:
         """
         Get ground surface area in square meters
         :return: float
         """
         # New method to calculate area
@@ -132,15 +131,15 @@
             return _area
         except TypeError as error:
             sys.stderr.write(f'A type error occurred: {error}')
         except IndexError as error:
             sys.stderr.write(f'A list index error occurred: {error}')
         except Exception as error:
             sys.stderr.write(f'An error occurred: {error}')
-            
+
     @classmethod
     def angle_between_vectors(cls, vec_1: List, vec_2: List):
         """
         angle between vectors in radians
         :param vec_1: vector
         :param vec_2: vector
         :return: float
@@ -156,8 +155,7 @@
                 cosine = -1
             alpha = math.acos(cosine)
             return alpha
         except TypeError as error:
             sys.stderr.write(f'A type error occurred: {error}')
         except Exception as error:
             sys.stderr.write(f'An error occurred: {error}')
-
```

### Comparing `cerc-geometry-2.1.2/geometry/location.py` & `cerc-geometry-2.1.3/geometry/location.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,28 @@
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 Code contributors: Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
 
 class Location:
-  """
-  Location
-  """
-  def __init__(self, country, city):
-    self._country = country
-    self._city = city
-
-  @property
-  def city(self):
     """
-    City name
+    Location
     """
-    return self._city
 
-  @property
-  def country(self):
-    """
-    Country code
-    """
-    return self._country
+    def __init__(self, country, city):
+        self._country = country
+        self._city = city
+
+    @property
+    def city(self):
+        """
+        City name
+        """
+        return self._city
+
+    @property
+    def country(self):
+        """
+        Country code
+        """
+        return self._country
```

### Comparing `cerc-geometry-2.1.2/geometry/map_point.py` & `cerc-geometry-2.1.3/geometry/map_point.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 Copyright © 2022 Concordia CERC group
 Project Coder Guille Gutierrez guillermo.gutierrezmorote@concordia.ca
 Code contributors: Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
 
 class MapPoint:
-  def __init__(self, x, y):
-    self._x = int(x)
-    self._y = int(y)
-
-  @property
-  def x(self):
-    return self._x
-
-  @property
-  def y(self):
-    return self._y
-
-  def __str__(self):
-    return f'({self.x}, {self.y})'
-
-  def __len__(self):
-    return 1
-
-  def __getitem__(self, index):
-    if index == 0:
-      return self._x
-    elif index == 1:
-      return self._y
-    else:
-      raise IndexError('Index error')
+    def __init__(self, x, y):
+        self._x = int(x)
+        self._y = int(y)
+
+    @property
+    def x(self):
+        return self._x
+
+    @property
+    def y(self):
+        return self._y
+
+    def __str__(self):
+        return f'({self.x}, {self.y})'
+
+    def __len__(self):
+        return 1
+
+    def __getitem__(self, index):
+        if index == 0:
+            return self._x
+        elif index == 1:
+            return self._y
+        else:
+            raise IndexError('Index error')
```

### Comparing `cerc-geometry-2.1.2/geometry/plane.py` & `cerc-geometry-2.1.3/geometry/plane.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,84 +2,85 @@
 Plane module
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
 from typing import TypeVar
-import numpy as np
 import sys
-Point = TypeVar('Point')
-
-
-class Plane:
-  """
-  Plane class
-  """
-
-  def __init__(self, origin, normal):
-    self._origin = origin
-    self._normal = normal
-    self._equation = None
-    self._opposite_normal = None
+import numpy as np
 
-  @property
-  def origin(self) -> Point:
-    """
-    Get plane origin point
-    :return: Point
-    """
-    return self._origin
 
-  @property
-  def normal(self):
-    """
-    Get plane normal [x, y, z]
-    :return: np.ndarray
-    """
-    return self._normal
-
-  @property
-  def equation(self) -> (float, float, float, float):
-    """
-    Get the plane equation components Ax + By + Cz + D = 0
-    :return: (A, B, C, D)
-    """
-    try:
-      if self._equation is None:
+Point = TypeVar('Point')
 
-        a = self.normal[0]
-        b = self.normal[1]
-        c = self.normal[2]
-        d = ((-1 * self.origin.coordinates[0]) * self.normal[0])
-        d += ((-1 * self.origin.coordinates[1]) * self.normal[1])
-        d += ((-1 * self.origin.coordinates[2]) * self.normal[2])
-        self._equation = (a, b, c, d)
-      return self._equation
-    except IndexError as error:
-      sys.stderr.write(f'You provided incorrect coordinates: {error}')
-    except Exception as error:
-      sys.stderr.write(f'An error occured: {error}')
 
-  def distance_to_point(self, point):
+class Plane:
     """
-    Distance between the given point and the plane
-    :return: float
+    Plane class
     """
-    p = point
-    e = self.equation
-    denominator = np.abs((p[0] * e[0]) + (p[1] * e[1]) + (p[2] * e[2]) + e[3])
-    numerator = np.sqrt((e[0]**2) + (e[1]**2) + (e[2]**2))
-    return float(denominator / numerator)
 
-  @property
-  def opposite_normal(self):
-    """
-    get plane normal in the opposite direction [x, y, z]
-    :return: np.ndarray
-    """
-    if self._opposite_normal is None:
-      coordinates = []
-      for coordinate in self.normal:
-        coordinates.append(-coordinate)
-      self._opposite_normal = np.array(coordinates)
-    return self._opposite_normal
+    def __init__(self, origin, normal):
+        self._origin = origin
+        self._normal = normal
+        self._equation = None
+        self._opposite_normal = None
+
+    @property
+    def origin(self) -> Point:
+        """
+        Get plane origin point
+        :return: Point
+        """
+        return self._origin
+
+    @property
+    def normal(self):
+        """
+        Get plane normal [x, y, z]
+        :return: np.ndarray
+        """
+        return self._normal
+
+    @property
+    def equation(self) -> (float, float, float, float):
+        """
+        Get the plane equation components Ax + By + Cz + D = 0
+        :return: (A, B, C, D)
+        """
+        try:
+            if self._equation is None:
+                a_value = self.normal[0]
+                b_value = self.normal[1]
+                c_value = self.normal[2]
+                d_value = -1 * self.origin.coordinates[0] * self.normal[0]
+                d_value += -1 * self.origin.coordinates[1] * self.normal[1]
+                d_value += -1 * self.origin.coordinates[2] * self.normal[2]
+                self._equation = (a_value, b_value, c_value, d_value)
+            return self._equation
+        except IndexError as error:
+            sys.stderr.write(f'You provided incorrect coordinates: {error}')
+            return None
+
+    def distance_to_point(self, point):
+        """
+        Distance between the given point and the plane
+        :return: float
+        """
+        point_copy = point
+        equation = self.equation
+        denominator = np.abs((point_copy[0] * equation[0]) +
+                             (point_copy[1] * equation[1]) + (point_copy[2] * equation[2]) + equation[3])
+        numerator = np.sqrt((equation[0] ** 2) + (equation[1] ** 2) + (equation[2] ** 2))
+        return float(denominator / numerator)
+
+    @property
+    def opposite_normal(self):
+        """
+        get plane normal in the opposite direction [x, y, z]
+        :return: np.ndarray
+        """
+        if self._opposite_normal is None:
+            coordinates = []
+            for coordinate in self.normal:
+                coordinates.append(-coordinate)
+            self._opposite_normal = np.array(coordinates)
+        return self._opposite_normal
```

### Comparing `cerc-geometry-2.1.2/geometry/point.py` & `cerc-geometry-2.1.3/geometry/point.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 Point module
 SPDX - License - Identifier: LGPL - 3.0 - or -later
 Copyright © 2022 Concordia CERC group
 Project Coder Pilar Monsalvete Alvarez de Uribarri pilar.monsalvete@concordia.ca
 """
 
 import math
-import numpy as np
 import sys
+import numpy as np
 
 
 class Point:
-  """
-  Point class
-  """
-
-  def __init__(self, coordinates: np.ndarray):
-    self._coordinates = coordinates
-
-  @property
-  def coordinates(self):
     """
-    Get point coordinates
-    :return: [ndarray]
+    Point class
     """
-    return self._coordinates
 
-  def distance_to_point(self, other_point):
-    """
-    Calculates distance between points in an n-D Euclidean space
-    :param other_point: point or vertex
-    :return: float
-    """
-    try:
-      power = 0
-      for dimension in range(0, len(self.coordinates)):
-        power += math.pow(other_point.coordinates[dimension]-self.coordinates[dimension], 2)
-      distance = math.sqrt(power)
-      return distance
-    except Exception as error:
-      sys.stderr.write(f'An error occurred: {error}')
-    
-   
+    def __init__(self, coordinates: np.ndarray):
+        self._coordinates = coordinates
+
+    @property
+    def coordinates(self):
+        """
+        Get point coordinates
+        :return: [ndarray]
+        """
+        return self._coordinates
+
+    def distance_to_point(self, other_point):
+        """
+        Calculates distance between points in an n-D Euclidean space
+        :param other_point: point or vertex
+        :return: float
+        """
+        try:
+            power = 0
+            for dimension, coordinate in enumerate(self.coordinates):
+                power += math.pow(other_point.coordinates[dimension]
+                                  - coordinate, 2)
+            distance = math.sqrt(power)
+            return distance
+        except Exception as error:
+            sys.stderr.write(f'An error occurred: {error}')
+            return None
```

### Comparing `cerc-geometry-2.1.2/geometry/polygon.py` & `cerc-geometry-2.1.3/geometry/polygon.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,443 +18,450 @@
 from geometry.point import Point
 from geometry.plane import Plane
 
 EPSILON = 0.0000001
 
 
 class Polygon:
-  """
-  Polygon class
-  """
-  def __init__(self, coordinates):
-    self._area = None
-    self._points = None
-    self._points_list = None
-    self._normal = None
-    self._inverse = None
-    self._edges = None
-    self._coordinates = coordinates
-    self._triangles = None
-    self._vertices = None
-    self._faces = None
-    self._plane = None
-
-  @property
-  def points(self) -> List[Point]:
-    """
-    Get the points belonging to the polygon [[x, y, z],...]
-    :return: [Point]
-    """
-    if self._points is None:
-      self._points = []
-      for coordinate in self.coordinates:
-        self._points.append(Point(coordinate))
-    return self._points
-
-  @property
-  def plane(self) -> Plane:
-    """
-    Get the polygon plane
-    :return: Plane
-    """
-    if self._plane is None:
-      self._plane = Plane(normal=self.normal, origin=self.points[0])
-    return self._plane
-
-  @property
-  def coordinates(self) -> List[np.ndarray]:
-    """
-    Get the points in the shape of its coordinates belonging to the polygon [[x, y, z],...]
-    :return: [np.ndarray]
-    """
-    return self._coordinates
-
-  def contains_point(self, point):
-    """
-    Determines if the given point is contained by the current polygon
-    :return: boolean
-    """
-    # fixme: This method doesn't seems to work.
-    n = len(self.vertices)
-    angle_sum = 0
-    for i in range(0, n):
-      vector_0 = self.vertices[i]
-      vector_1 = self.vertices[(i+1) % n]
-      # set to origin
-      vector_0[0] = vector_0[0] - point.coordinates[0]
-      vector_0[1] = vector_0[1] - point.coordinates[1]
-      vector_0[2] = vector_0[2] - point.coordinates[2]
-      vector_1[0] = vector_1[0] - point.coordinates[0]
-      vector_1[1] = vector_1[1] - point.coordinates[1]
-      vector_1[2] = vector_1[2] - point.coordinates[2]
-      module = np.linalg.norm(vector_0) * np.linalg.norm(vector_1)
-
-      scalar_product = np.dot(vector_0, vector_1)
-      angle = np.pi/2
-      if module != 0:
-        angle = abs(np.arcsin(scalar_product / module))
-      angle_sum += angle
-    return abs(angle_sum - math.pi*2) < EPSILON
-
-  def contains_polygon(self, polygon):
     """
-    Determines if the given polygon is contained by the current polygon
-    :return: boolean
+    Polygon class
     """
 
-    for point in polygon.points:
-      if not self.contains_point(point):
-        return False
-    return True
-
-  @property
-  def points_list(self) -> np.ndarray:
-    """
-    Get the solid surface point coordinates list [x, y, z, x, y, z,...]
-    :return: np.ndarray
-    """
-    try:
-      if self._points_list is None:
-        s = self.coordinates
-        self._points_list = np.reshape(s, len(s) * 3)
-      return self._points_list
-    except ValueError as error:
-      sys.stderr.write(f'Wrong coordinates: {error}')
-    except Exception as error:
-      sys.stderr.write(f'An error occurred: {error}')
-
-  @property
-  def edges(self) -> List[List[Point]]:
-    """
-    Get polygon edges list
-    :return: [[Point]]
-    """
-    if self._edges is None:
-      self._edges = []
-      for i in range(0, len(self.points) - 1):
-        point_1 = self.points[i]
-        point_2 = self.points[i + 1]
-        self._edges.append([point_1, point_2])
-      self._edges.append([self.points[len(self.points) - 1], self.points[0]])
-    return self._edges
-
-  @property
-  def area(self):
-    """
-    Get surface area in square meters
-    :return: float
-    """
-    if self._area is None:
-      self._area = 0
-      for triangle in self.triangles:
-        ab = np.zeros(3)
-        ac = np.zeros(3)
-        for i in range(0, 3):
-          ab[i] = triangle.coordinates[1][i] - triangle.coordinates[0][i]
-          ac[i] = triangle.coordinates[2][i] - triangle.coordinates[0][i]
-        self._area += np.linalg.norm(np.cross(ab, ac)) / 2
-    return self._area
-
-  @area.setter
-  def area(self, value):
-    self._area = value
-
-  @property
-  def normal(self) -> np.ndarray:
-    """
-    Get surface normal vector
-    :return: np.ndarray
-    """
-    if self._normal is None:
-      points = self.coordinates
-      # todo: IF THE FIRST ONE IS 0, START WITH THE NEXT
-      point_origin = points[len(points) - 2]
-      vector_1 = points[len(points) - 1] - point_origin
-      vector_2 = points[0] - point_origin
-      vector_3 = points[1] - point_origin
-      cross_product = np.cross(vector_1, vector_2)
-      if np.linalg.norm(cross_product) != 0:
-        cross_product = cross_product / np.linalg.norm(cross_product)
-        alpha = self._angle_between_vectors(vector_1, vector_2)
-      else:
-        cross_product = [0, 0, 0]
-        alpha = 0
-      if len(points) == 3:
-        return cross_product
-      if np.linalg.norm(cross_product) == 0:
-        return cross_product
-      alpha += self._angle(vector_2, vector_3, cross_product)
-      for i in range(0, len(points) - 4):
-        vector_1 = points[i + 1] - point_origin
-        vector_2 = points[i + 2] - point_origin
-        alpha += self._angle(vector_1, vector_2, cross_product)
-      vector_1 = points[len(points) - 1] - point_origin
-      vector_2 = points[0] - point_origin
-      if alpha < 0:
-        cross_product = np.cross(vector_2, vector_1)
-      else:
-        cross_product = np.cross(vector_1, vector_2)
-      self._normal = cross_product / np.linalg.norm(cross_product)
-    return self._normal
-
-  @staticmethod
-  def _angle(vector_1, vector_2, cross_product):
-    """
-    alpha angle in radians
-    :param vector_1: [float]
-    :param vector_2: [float]
-    :param cross_product: [float]
-    :return: float
-    """
-    accepted_normal_difference = 0.01
-    cross_product_next = np.cross(vector_1, vector_2)
-    if np.linalg.norm(cross_product_next) != 0:
-      cross_product_next = cross_product_next / np.linalg.norm(cross_product_next)
-      alpha = Polygon._angle_between_vectors(vector_1, vector_2)
-    else:
-      cross_product_next = [0, 0, 0]
-      alpha = 0
-    delta_normals = 0
-    for j in range(0, 3):
-      delta_normals += cross_product[j] - cross_product_next[j]
-    if np.abs(delta_normals) < accepted_normal_difference:
-      return alpha
-    return -alpha
-
-  @staticmethod
-  def triangle_mesh(vertices, normal):
-    min_x = 1e16
-    min_y = 1e16
-    min_z = 1e16
-    for vertex in vertices:
-      if vertex[0] < min_x:
-        min_x = vertex[0]
-      if vertex[1] < min_y:
-        min_y = vertex[1]
-      if vertex[2] < min_z:
-        min_z = vertex[2]
-
-    new_vertices = []
-    for vertex in vertices:
-      vertex = [vertex[0]-min_x, vertex[1]-min_y, vertex[2]-min_z]
-      new_vertices.append(vertex)
-
-    transformation_matrix = trimesh.geometry.plane_transform(origin=new_vertices[0], normal=normal)
-
-    coordinates = []
-    for vertex in vertices:
-      transformed_vertex = [vertex[0]-min_x, vertex[1]-min_y, vertex[2]-min_z, 1]
-      transformed_vertex = np.dot(transformation_matrix, transformed_vertex)
-      coordinate = [transformed_vertex[0], transformed_vertex[1]]
-      coordinates.append(coordinate)
-
-    polygon = shapley_polygon(coordinates)
-
-    try:
-      vertices_2d, faces = trimesh.creation.triangulate_polygon(polygon, engine='triangle')
-      mesh = Trimesh(vertices=vertices, faces=faces)
-
-      # check orientation
-      normal_sum = 0
-      for i in range(0, 3):
-        normal_sum += normal[i] + mesh.face_normals[0][i]
-
-      if abs(normal_sum) <= 1E-10:
-        new_faces = []
-        for face in faces:
-          new_face = []
-          for i in range(0, len(face)):
-            new_face.append(face[len(face)-i-1])
-          new_faces.append(new_face)
-        mesh = Trimesh(vertices=vertices, faces=new_faces)
-
-      return mesh
-
-    except ValueError:
-      sys.stderr.write(f'Not able to triangulate polygon\n')
-      _vertices = [[0, 0, 0], [0, 0, 1], [0, 1, 0]]
-      _faces = [[0, 1, 2]]
-      return Trimesh(vertices=_vertices, faces=_faces)
-
-  @property
-  def triangles(self) -> List[Polygon]:
-    try:
-      if self._triangles is None:
-        self._triangles = []
-        _mesh = self.triangle_mesh(self.coordinates, self.normal)
-        for face in _mesh.faces:
-          points = []
-          for vertex in face:
-            points.append(self.coordinates[vertex])
-          polygon = Polygon(points)
-          self._triangles.append(polygon)
-      return self._triangles
-    except ModuleNotFoundError as error:
-      print(f'Issues with trimesh module imports: {error}')
-    except Exception as error:
-      print(f'An error occurred: {error}')
-
-  @staticmethod
-  def _angle_between_vectors(vec_1, vec_2):
-    """
-    angle between vectors in radians
-    :param vec_1: vector
-    :param vec_2: vector
-    :return: float
-    """
-    if np.linalg.norm(vec_1) == 0 or np.linalg.norm(vec_2) == 0:
-      sys.stderr.write("Warning: impossible to calculate angle between planes' normal. Return 0\n")
-      return 0
-    cosine = np.dot(vec_1, vec_2) / np.linalg.norm(vec_1) / np.linalg.norm(vec_2)
-    if cosine > 1 and cosine - 1 < 1e-5:
-      cosine = 1
-    elif cosine < -1 and cosine + 1 > -1e-5:
-      cosine = -1
-    alpha = math.acos(cosine)
-    return alpha
-
-  @property
-  def inverse(self):
-    """
-    Get the polygon coordinates in reversed order
-    :return: [np.ndarray]
-    """
-    if self._inverse is None:
-      self._inverse = self.coordinates[::-1]
-    return self._inverse
-
-  def divide(self, plane):
-    """
-    Divides the polygon in two by a plane
-    :param plane: plane that intersects with self to divide it in two parts (Plane)
-    :return: Polygon, Polygon, [Point]
-    """
-    tri_polygons = Trimesh(vertices=self.vertices, faces=self.faces)
-    intersection = trimesh.intersections.mesh_plane(tri_polygons, plane.normal, plane.origin.coordinates)
-    polys_1 = trimesh.intersections.slice_mesh_plane(tri_polygons, plane.opposite_normal, plane.origin.coordinates)
-    polys_2 = trimesh.intersections.slice_mesh_plane(tri_polygons, plane.normal, plane.origin.coordinates)
-    triangles_1 = []
-    for triangle in polys_1.triangles:
-      triangles_1.append(Polygon(triangle))
-    polygon_1 = self._reshape(triangles_1)
-    triangles_2 = []
-    for triangle in polys_2.triangles:
-      triangles_2.append(Polygon(triangle))
-    polygon_2 = self._reshape(triangles_2)
-    return polygon_1, polygon_2, intersection
-
-  def _reshape(self, triangles) -> Polygon:
-    edges_list = []
-    for i in range(0, len(triangles)):
-      for edge in triangles[i].edges:
-        if not self._edge_in_edges_list(edge, edges_list):
-          edges_list.append(edge)
-        else:
-          edges_list = self._remove_from_list(edge, edges_list)
-    points = self._order_points(edges_list)
-    return Polygon(points)
-
-  @staticmethod
-  def _edge_in_edges_list(edge, edges_list):
-    for edge_element in edges_list:
-      if (edge_element[0].distance_to_point(edge[0]) == 0 and edge_element[1].distance_to_point(edge[1]) == 0) or \
-          (edge_element[1].distance_to_point(edge[0]) == 0 and edge_element[0].distance_to_point(
-            edge[1]) == 0):
+    def __init__(self, coordinates):
+        self._area = None
+        self._points = None
+        self._points_list = None
+        self._normal = None
+        self._inverse = None
+        self._edges = None
+        self._coordinates = coordinates
+        self._triangles = None
+        self._vertices = None
+        self._faces = None
+        self._plane = None
+
+    @property
+    def points(self) -> List[Point]:
+        """
+        Get the points belonging to the polygon [[x, y, z],...]
+        :return: [Point]
+        """
+        if self._points is None:
+            self._points = []
+            for coordinate in self.coordinates:
+                self._points.append(Point(coordinate))
+        return self._points
+
+    @property
+    def plane(self) -> Plane:
+        """
+        Get the polygon plane
+        :return: Plane
+        """
+        if self._plane is None:
+            self._plane = Plane(normal=self.normal, origin=self.points[0])
+        return self._plane
+
+    @property
+    def coordinates(self) -> List[np.ndarray]:
+        """
+        Get the points in the shape of its coordinates belonging to the polygon [[x, y, z],...]
+        :return: [np.ndarray]
+        """
+        return self._coordinates
+
+    def contains_point(self, point):
+        """
+        Determines if the given point is contained by the current polygon
+        :return: boolean
+        """
+        # fixme: This method doesn't seems to work.
+        vertices_length = len(self.vertices)
+        angle_sum = 0
+        for i in range(0, vertices_length):
+            vector_0 = self.vertices[i]
+            vector_1 = self.vertices[(i + 1) % vertices_length]
+            # set to origin
+            vector_0[0] = vector_0[0] - point.coordinates[0]
+            vector_0[1] = vector_0[1] - point.coordinates[1]
+            vector_0[2] = vector_0[2] - point.coordinates[2]
+            vector_1[0] = vector_1[0] - point.coordinates[0]
+            vector_1[1] = vector_1[1] - point.coordinates[1]
+            vector_1[2] = vector_1[2] - point.coordinates[2]
+            module = np.linalg.norm(vector_0) * np.linalg.norm(vector_1)
+            scalar_product = np.dot(vector_0, vector_1)
+            angle = np.pi / 2
+            if module != 0:
+                angle = abs(np.arcsin(scalar_product / module))
+            angle_sum += angle
+        return abs(angle_sum - math.pi * 2) < EPSILON
+
+    def contains_polygon(self, polygon):
+        """
+        Determines if the given polygon is contained by the current polygon
+        :return: boolean
+        """
+
+        for point in polygon.points:
+            if not self.contains_point(point):
+                return False
         return True
-    return False
-
-  @staticmethod
-  def _order_points(edges_list):
-    # todo: not sure that this method works for any case -> RECHECK
-    points = edges_list[0]
-    for _ in range(0, len(points)):
-      for i in range(1, len(edges_list)):
-        point_1 = edges_list[i][0]
-        point_2 = points[len(points) - 1]
-        if point_1.distance_to_point(point_2) == 0:
-          points.append(edges_list[i][1])
-    points.remove(points[len(points) - 1])
-    array_points = []
-    for point in points:
-      array_points.append(point.coordinates)
-    return np.array(array_points)
-
-  @staticmethod
-  def _remove_from_list(edge, edges_list):
-    new_list = []
-    for edge_element in edges_list:
-      if not ((edge_element[0].distance_to_point(edge[0]) == 0 and edge_element[1].distance_to_point(
-          edge[1]) == 0) or
-              (edge_element[1].distance_to_point(edge[0]) == 0 and edge_element[0].distance_to_point(
-                edge[1]) == 0)):
-        new_list.append(edge_element)
-    return new_list
-
-  @property
-  def vertices(self) -> np.ndarray:
-    """
-    Get polygon vertices
-    :return: np.ndarray(int)
-    """
-    if self._vertices is None:
-      vertices, self._vertices = [], []
-      _ = [vertices.extend(s.coordinates) for s in self.triangles]
-      for vertex_1 in vertices:
-        found = False
-        for vertex_2 in self._vertices:
-          found = False
-          power = 0
-          for dimension in range(0, 3):
-            power += math.pow(vertex_2[dimension] - vertex_1[dimension], 2)
-          distance = math.sqrt(power)
-          if distance == 0:
-            found = True
-            break
-        if not found:
-          self._vertices.append(vertex_1)
-      self._vertices = np.asarray(self._vertices)
-    return self._vertices
 
-  @property
-  def faces(self) -> List[List[int]]:
-    """
-    Get polygon triangular faces
-    :return: [face]
-    """
-    if self._faces is None:
-      self._faces = []
-
-      for polygon in self.triangles:
-        face = []
-        points = polygon.coordinates
-        if len(points) != 3:
-          sub_polygons = polygon.triangles
-          # todo: I modified this! To be checked @Guille
-          if len(sub_polygons) >= 1:
-            for sub_polygon in sub_polygons:
-              face = []
-              points = sub_polygon.coordinates
-              for point in points:
-                face.append(self._position_of(point, face))
-              self._faces.append(face)
+    @property
+    def points_list(self) -> np.ndarray:
+        """
+        Get the solid surface point coordinates list [x, y, z, x, y, z,...]
+        :return: np.ndarray
+        """
+        try:
+            if self._points_list is None:
+                coordinates = self.coordinates
+                self._points_list = np.reshape(coordinates, len(coordinates) * 3)
+            return self._points_list
+        except ValueError as error:
+            sys.stderr.write(f'Wrong coordinates: {error}')
+            return None
+
+    @property
+    def edges(self) -> List[List[Point]]:
+        """
+        Get polygon edges list
+        :return: [[Point]]
+        """
+        if self._edges is None:
+            self._edges = []
+            for i in range(0, len(self.points) - 1):
+                point_1 = self.points[i]
+                point_2 = self.points[i + 1]
+                self._edges.append([point_1, point_2])
+            self._edges.append([self.points[len(self.points) - 1], self.points[0]])
+        return self._edges
+
+    @property
+    def area(self):
+        """
+        Get surface area in square meters
+        :return: float
+        """
+        if self._area is None:
+            self._area = 0
+            for triangle in self.triangles:
+                ab_value = np.zeros(3)
+                ac_value = np.zeros(3)
+                for i in range(0, 3):
+                    ab_value[i] = triangle.coordinates[1][i] - triangle.coordinates[0][i]
+                    ac_value[i] = triangle.coordinates[2][i] - triangle.coordinates[0][i]
+                self._area += np.linalg.norm(np.cross(ab_value, ac_value)) / 2
+        return self._area
+
+    @area.setter
+    def area(self, value):
+        self._area = value
+
+    @property
+    def normal(self) -> np.ndarray:
+        """
+        Get surface normal vector
+        :return: np.ndarray
+        """
+        if self._normal is None:
+            points = self.coordinates
+            # todo: IF THE FIRST ONE IS 0, START WITH THE NEXT
+            point_origin = points[len(points) - 2]
+            vector_1 = points[len(points) - 1] - point_origin
+            vector_2 = points[0] - point_origin
+            vector_3 = points[1] - point_origin
+            cross_product = np.cross(vector_1, vector_2)
+            if np.linalg.norm(cross_product) != 0:
+                cross_product = cross_product / np.linalg.norm(cross_product)
+                alpha = self._angle_between_vectors(vector_1, vector_2)
+            else:
+                cross_product = [0, 0, 0]
+                alpha = 0
+            if len(points) == 3:
+                return cross_product
+            if np.linalg.norm(cross_product) == 0:
+                return cross_product
+            alpha += self._angle(vector_2, vector_3, cross_product)
+            for i in range(0, len(points) - 4):
+                vector_1 = points[i + 1] - point_origin
+                vector_2 = points[i + 2] - point_origin
+                alpha += self._angle(vector_1, vector_2, cross_product)
+            vector_1 = points[len(points) - 1] - point_origin
+            vector_2 = points[0] - point_origin
+            if alpha < 0:
+                cross_product = np.cross(vector_2, vector_1)
+            else:
+                cross_product = np.cross(vector_1, vector_2)
+            self._normal = cross_product / np.linalg.norm(cross_product)
+        return self._normal
+
+    @staticmethod
+    def _angle(vector_1, vector_2, cross_product):
+        """
+        alpha angle in radians
+        :param vector_1: [float]
+        :param vector_2: [float]
+        :param cross_product: [float]
+        :return: float
+        """
+        accepted_normal_difference = 0.01
+        cross_product_next = np.cross(vector_1, vector_2)
+        if np.linalg.norm(cross_product_next) != 0:
+            cross_product_next = cross_product_next / np.linalg.norm(cross_product_next)
+            alpha = Polygon._angle_between_vectors(vector_1, vector_2)
         else:
-          for point in points:
-            face.append(self._position_of(point, face))
-          self._faces.append(face)
-    return self._faces
+            cross_product_next = [0, 0, 0]
+            alpha = 0
+        delta_normals = 0
+        for j in range(0, 3):
+            delta_normals += cross_product[j] - cross_product_next[j]
+        if np.abs(delta_normals) < accepted_normal_difference:
+            return alpha
+        return -alpha
+
+    @staticmethod
+    def triangle_mesh(vertices, normal):
+        """
+        builds triangle mesh
+        :param vertices: the vertices of the triangle
+        :param normal: normal to the plane
+        :return: trimesh
+        """
+        min_x = 1e16
+        min_y = 1e16
+        min_z = 1e16
+        for vertex in vertices:
+            if vertex[0] < min_x:
+                min_x = vertex[0]
+            if vertex[1] < min_y:
+                min_y = vertex[1]
+            if vertex[2] < min_z:
+                min_z = vertex[2]
+        new_vertices = []
+        for vertex in vertices:
+            vertex = [vertex[0] - min_x, vertex[1] - min_y, vertex[2] - min_z]
+            new_vertices.append(vertex)
+
+        transformation_matrix = trimesh.geometry.plane_transform(origin=new_vertices[0], normal=normal)
+        coordinates = []
+        for vertex in vertices:
+            transformed_vertex = [vertex[0] - min_x, vertex[1] - min_y, vertex[2] - min_z, 1]
+            transformed_vertex = np.dot(transformation_matrix, transformed_vertex)
+            coordinate = [transformed_vertex[0], transformed_vertex[1]]
+            coordinates.append(coordinate)
+
+        polygon = shapley_polygon(coordinates)
+
+        try:
+            _, faces = trimesh.creation.triangulate_polygon(polygon, engine='triangle')
+            mesh = Trimesh(vertices=vertices, faces=faces)
+
+            # check orientation
+            normal_sum = 0
+            for i in range(0, 3):
+                normal_sum += normal[i] + mesh.face_normals[0][i]
+
+            if abs(normal_sum) <= 1E-10:
+                new_faces = []
+                for face in faces:
+                    new_face = []
+                    for i in range(0, len(face)):
+                        new_face.append(face[len(face) - i - 1])
+                    new_faces.append(new_face)
+                mesh = Trimesh(vertices=vertices, faces=new_faces)
+
+            return mesh
+
+        except ValueError:
+            sys.stderr.write('Not able to triangulate polygon')
+            _vertices = [[0, 0, 0], [0, 0, 1], [0, 1, 0]]
+            _faces = [[0, 1, 2]]
+            return Trimesh(vertices=_vertices, faces=_faces)
+
+    @property
+    def triangles(self) -> List[Polygon]:
+        """
+        triangles property
+        """
+        try:
+            if self._triangles is None:
+                self._triangles = []
+                _mesh = self.triangle_mesh(self.coordinates, self.normal)
+                for face in _mesh.faces:
+                    points = []
+                    for vertex in face:
+                        points.append(self.coordinates[vertex])
+                    polygon = Polygon(points)
+                    self._triangles.append(polygon)
+            return self._triangles
+        except ModuleNotFoundError as error:
+            print(f'Issues with trimesh module imports: {error}')
+            return None
+
+    @staticmethod
+    def _angle_between_vectors(vec_1, vec_2):
+        """
+        angle between vectors in radians
+        :param vec_1: vector
+        :param vec_2: vector
+        :return: float
+        """
+        if np.linalg.norm(vec_1) == 0 or np.linalg.norm(vec_2) == 0:
+            sys.stderr.write("Warning: impossible to calculate angle between planes' normal. Return 0\n")
+            return 0
+        cosine = np.dot(vec_1, vec_2) / np.linalg.norm(vec_1) / np.linalg.norm(vec_2)
+        if cosine > 1 and cosine - 1 < 1e-5:
+            cosine = 1
+        elif cosine < -1 and cosine + 1 > -1e-5:
+            cosine = -1
+        alpha = math.acos(cosine)
+        return alpha
+
+    @property
+    def inverse(self):
+        """
+        Get the polygon coordinates in reversed order
+        :return: [np.ndarray]
+        """
+        if self._inverse is None:
+            self._inverse = self.coordinates[::-1]
+        return self._inverse
+
+    def divide(self, plane):
+        """
+        Divides the polygon in two by a plane
+        :param plane: plane that intersects with self to divide it in two parts (Plane)
+        :return: Polygon, Polygon, [Point]
+        """
+        tri_polygons = Trimesh(vertices=self.vertices, faces=self.faces)
+        intersection = trimesh.intersections.mesh_plane(tri_polygons,
+                                                        plane.normal, plane.origin.coordinates)
+        polys_1 = trimesh.intersections.slice_mesh_plane(tri_polygons,
+                                                         plane.opposite_normal, plane.origin.coordinates)
+        polys_2 = trimesh.intersections.slice_mesh_plane(tri_polygons,
+                                                         plane.normal, plane.origin.coordinates)
+        triangles_1 = []
+        for triangle in polys_1.triangles:
+            triangles_1.append(Polygon(triangle))
+        polygon_1 = self._reshape(triangles_1)
+        triangles_2 = []
+        for triangle in polys_2.triangles:
+            triangles_2.append(Polygon(triangle))
+        polygon_2 = self._reshape(triangles_2)
+        return polygon_1, polygon_2, intersection
+
+    def _reshape(self, triangles) -> Polygon:
+        edges_list = []
+        for _, triangle in enumerate(triangles):
+            for edge in triangle.edges:
+                if not self._edge_in_edges_list(edge, edges_list):
+                    edges_list.append(edge)
+                else:
+                    edges_list = self._remove_from_list(edge, edges_list)
+        points = self._order_points(edges_list)
+        return Polygon(points)
+
+    @staticmethod
+    def _edge_in_edges_list(edge, edges_list):
+        for edge_element in edges_list:
+            if (edge_element[0].distance_to_point(edge[0]) == 0 and
+                edge_element[1].distance_to_point(edge[1]) == 0) or \
+                (edge_element[1].distance_to_point(edge[0]) == 0 and
+                 edge_element[0].distance_to_point(edge[1]) == 0):
+                return True
+        return False
 
-  def _position_of(self, point, face):
-    """
-    position of a specific point in the list of points that define a face
-    :return: int
-    """
-    vertices = self.vertices
-    for i in range(len(vertices)):
-      # ensure not duplicated vertex
-      power = 0
-      vertex2 = vertices[i]
-      for dimension in range(0, 3):
-        power += math.pow(vertex2[dimension] - point[dimension], 2)
-      distance = math.sqrt(power)
-      if i not in face and distance == 0:
-        return i
-    return -1
+    @staticmethod
+    def _order_points(edges_list):
+        # todo: not sure that this method works for any case -> RECHECK
+        points = edges_list[0]
+        for _ in range(0, len(points)):
+            for i in range(1, len(edges_list)):
+                point_1 = edges_list[i][0]
+                point_2 = points[len(points) - 1]
+                if point_1.distance_to_point(point_2) == 0:
+                    points.append(edges_list[i][1])
+        points.remove(points[len(points) - 1])
+        array_points = []
+        for point in points:
+            array_points.append(point.coordinates)
+        return np.array(array_points)
+
+    @staticmethod
+    def _remove_from_list(edge, edges_list):
+        new_list = []
+        for edge_element in edges_list:
+            if not ((edge_element[0].distance_to_point(edge[0]) == 0 and edge_element[1]
+                .distance_to_point(edge[1]) == 0) or
+                    (edge_element[1].distance_to_point(edge[0]) == 0 and edge_element[0]
+                        .distance_to_point(edge[1]) == 0)):
+                new_list.append(edge_element)
+        return new_list
+
+    @property
+    def vertices(self) -> np.ndarray:
+        """
+        Get polygon vertices
+        :return: np.ndarray(int)
+        """
+        if self._vertices is None:
+            vertices, self._vertices = [], []
+            _ = [vertices.extend(s.coordinates) for s in self.triangles]
+            for vertex_1 in vertices:
+                found = False
+                for vertex_2 in self._vertices:
+                    found = False
+                    power = 0
+                    for dimension in range(0, 3):
+                        power += math.pow(vertex_2[dimension] - vertex_1[dimension], 2)
+                    distance = math.sqrt(power)
+                    if distance == 0:
+                        found = True
+                        break
+                if not found:
+                    self._vertices.append(vertex_1)
+            self._vertices = np.asarray(self._vertices)
+        return self._vertices
+
+    @property
+    def faces(self) -> List[List[int]]:
+        """
+        Get polygon triangular faces
+        :return: [face]
+        """
+        if self._faces is None:
+            self._faces = []
+            for polygon in self.triangles:
+                face = []
+                points = polygon.coordinates
+                if len(points) != 3:
+                    sub_polygons = polygon.triangles
+                    # TODO: I modified this! To be checked @Guille
+                    if len(sub_polygons) >= 1:
+                        for sub_polygon in sub_polygons:
+                            face = []
+                            points = sub_polygon.coordinates
+                            for point in points:
+                                face.append(self._position_of(point, face))
+                            self._faces.append(face)
+                else:
+                    for point in points:
+                        face.append(self._position_of(point, face))
+                    self._faces.append(face)
+        return self._faces
+
+    def _position_of(self, point, face):
+        """
+        position of a specific point in the list of points that define a face
+        :return: int
+        """
+        vertices = self.vertices
+        for count, vertex2 in enumerate(vertices):
+            # ensure not duplicated vertex
+            power = 0
+            for dimension in range(0, 3):
+                power += math.pow(vertex2[dimension] - point[dimension], 2)
+            distance = math.sqrt(power)
+            if count not in face and distance == 0:
+                return count
+        return -1
```

### Comparing `cerc-geometry-2.1.2/geometry/polyhedron.py` & `cerc-geometry-2.1.3/geometry/polyhedron.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,244 +13,249 @@
 from trimesh import Trimesh
 
 MIN_COORDINATE = -1.7976931348623157e+308
 MAX_COORDINATE = 1.7976931348623157e+308
 
 
 class Polyhedron:
-  """
-  Polyhedron class
-  """
-
-  def __init__(self, polygons):
-    self._polygons = polygons
-    self._polyhedron = None
-    self._triangulated_polyhedron = None
-    self._volume = None
-    self._faces = None
-    self._vertices = None
-    self._trimesh = None
-    self._centroid = None
-    self._max_z = None
-    self._max_y = None
-    self._max_x = None
-    self._min_z = None
-    self._min_y = None
-    self._min_x = None
-
-  def _position_of(self, point, face):
-    """
-    position of a specific point in the list of points that define a face
-    :return: int
-    """
-    vertices = self.vertices
-    for i in range(len(vertices)):
-      # ensure not duplicated vertex
-      power = 0
-      vertex2 = vertices[i]
-      for dimension in range(0, 3):
-        power += math.pow(vertex2[dimension] - point[dimension], 2)
-      distance = math.sqrt(power)
-      if i not in face and distance == 0:
-        return i
-    return -1
-
-  @property
-  def vertices(self) -> np.ndarray:
-    """
-    Get polyhedron vertices
-    :return: np.ndarray(int)
-    """
-    if self._vertices is None:
-      vertices, self._vertices = [], []
-      _ = [vertices.extend(s.coordinates) for s in self._polygons]
-      for vertex_1 in vertices:
-        found = False
-        for vertex_2 in self._vertices:
-          found = False
-          power = 0
-          for dimension in range(0, 3):
-            power += math.pow(vertex_2[dimension] - vertex_1[dimension], 2)
-          distance = math.sqrt(power)
-          if distance == 0:
-            found = True
-            break
-        if not found:
-          self._vertices.append(vertex_1)
-      self._vertices = np.asarray(self._vertices)
-    return self._vertices
-
-  @property
-  def faces(self) -> List[List[int]]:
-    """
-    Get polyhedron triangular faces
-    :return: [face]
-    """
-    if self._faces is None:
-      self._faces = []
-
-      for polygon in self._polygons:
-
-        face = []
-        points = polygon.coordinates
-        if len(points) != 3:
-          sub_polygons = polygon.triangles
-          # todo: I modified this! To be checked @Guille
-          if len(sub_polygons) >= 1:
-            for sub_polygon in sub_polygons:
-              face = []
-              points = sub_polygon.coordinates
-              for point in points:
-                face.append(self._position_of(point, face))
-              self._faces.append(face)
-        else:
-          for point in points:
-            face.append(self._position_of(point, face))
-          self._faces.append(face)
-    return self._faces
-
-  @property
-  def trimesh(self) -> Union[Trimesh, None]:
-    """
-    Get polyhedron trimesh
-    :return: Trimesh
-    """
-    if self._trimesh is None:
-      for face in self.faces:
-        if len(face) != 3:
-          sys.stderr.write('Not able to generate trimesh\n')
-          return None
-      self._trimesh = Trimesh(vertices=self.vertices, faces=self.faces)
-    return self._trimesh
-
-  @property
-  def volume(self):
-    """
-    Get polyhedron volume in cubic meters
-    :return: float
-    """
-    if self._volume is None:
-      if self.trimesh is None:
-        self._volume = np.inf
-      elif not self.trimesh.is_volume:
-        self._volume = np.inf
-      else:
-        self._volume = self.trimesh.volume
-    return self._volume
-
-  @property
-  def max_z(self):
-    """
-    Get polyhedron maximal z value in meters
-    :return: float
-    """
-    if self._max_z is None:
-      self._max_z = MIN_COORDINATE
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          self._max_z = max(self._max_z, point[2])
-    return self._max_z
-
-  @property
-  def max_y(self):
-    """
-    Get polyhedron maximal y value in meters
-    :return: float
     """
-    if self._max_y is None:
-      self._max_y = MIN_COORDINATE
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          if self._max_y < point[1]:
-            self._max_y = point[1]
-    return self._max_y
-
-  @property
-  def max_x(self):
-    """
-    Get polyhedron maximal x value in meters
-    :return: float
-    """
-    if self._max_x is None:
-      self._max_x = MIN_COORDINATE
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          self._max_x = max(self._max_x, point[0])
-    return self._max_x
-
-  @property
-  def min_z(self):
-    """
-    Get polyhedron minimal z value in meters
-    :return: float
-    """
-    if self._min_z is None:
-      self._min_z = self.max_z
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          if self._min_z > point[2]:
-            self._min_z = point[2]
-    return self._min_z
-
-  @property
-  def min_y(self):
-    """
-    Get polyhedron minimal y value in meters
-    :return: float
-    """
-    if self._min_y is None:
-      self._min_y = self.max_y
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          if self._min_y > point[1]:
-            self._min_y = point[1]
-    return self._min_y
-
-  @property
-  def min_x(self):
-    """
-    Get polyhedron minimal x value in meters
-    :return: float
+    Polyhedron class
     """
-    if self._min_x is None:
-      self._min_x = self.max_x
-      for polygon in self._polygons:
-        for point in polygon.coordinates:
-          if self._min_x > point[0]:
-            self._min_x = point[0]
-    return self._min_x
 
-  @property
-  def centroid(self) -> Union[None, List[float]]:
-    """
-    Get polyhedron centroid
-    :return: [x,y,z]
-    """
-    if self._centroid is None:
-      trimesh = self.trimesh
-      if trimesh is None:
-        return None
-      self._centroid = self.trimesh.centroid
-    return self._centroid
-
-  def stl_export(self, full_path):
-    """
-    Export the polyhedron to stl given file
-    :param full_path: str
-    :return: None
-    """
-    self.trimesh.export(full_path, 'stl_ascii')
-
-  def obj_export(self, full_path):
-    """
-    Export the polyhedron to obj given file
-    :param full_path: str
-    :return: None
-    """
-    self.trimesh.export(full_path, 'obj')
-
-  def show(self):
-    """
-    Auxiliary function to render the polyhedron
-    :return: None
-    """
-    self.trimesh.show()
+    def __init__(self, polygons):
+        self._polygons = polygons
+        self._polyhedron = None
+        self._triangulated_polyhedron = None
+        self._volume = None
+        self._faces = None
+        self._vertices = None
+        self._trimesh = None
+        self._centroid = None
+        self._max_z = None
+        self._max_y = None
+        self._max_x = None
+        self._min_z = None
+        self._min_y = None
+        self._min_x = None
+
+    def _position_of(self, point, face):
+        """
+        position of a specific point in the list of points that define a face
+        :return: int
+        """
+        vertices = self.vertices
+        for i in range(len(vertices)):
+            # ensure not duplicated vertex
+            power = 0
+            vertex2 = vertices[i]
+            for dimension in range(0, 3):
+                power += math.pow(vertex2[dimension] - point[dimension], 2)
+            distance = math.sqrt(power)
+            if i not in face and distance == 0:
+                return i
+        return -1
+
+    @property
+    def vertices(self) -> np.ndarray:
+        """
+        Get polyhedron vertices
+        :return: np.ndarray(int)
+        """
+        if self._vertices is None:
+            vertices, self._vertices = [], []
+            _ = [vertices.extend(s.coordinates) for s in self._polygons]
+            for vertex_1 in vertices:
+                found = False
+                for vertex_2 in self._vertices:
+                    found = False
+                    power = 0
+                    for dimension in range(0, 3):
+                        power += math.pow(vertex_2[dimension] - vertex_1[dimension], 2)
+                    distance = math.sqrt(power)
+                    if distance == 0:
+                        found = True
+                        break
+                if not found:
+                    self._vertices.append(vertex_1)
+            self._vertices = np.asarray(self._vertices)
+        return self._vertices
+
+    @property
+    def faces(self) -> List[List[int]]:
+        """
+        Get polyhedron triangular faces
+        :return: [face]
+        """
+        try:
+            if self._faces is None:
+                self._faces = []
+
+                for polygon in self._polygons:
+
+                    face = []
+                    points = polygon.coordinates
+                    if len(points) != 3:
+                        sub_polygons = polygon.triangles
+                        # todo: I modified this! To be checked @Guille
+                        if len(sub_polygons) >= 1:
+                            for sub_polygon in sub_polygons:
+                                face = []
+                                points = sub_polygon.coordinates
+                                for point in points:
+                                    face.append(self._position_of(point, face))
+                                self._faces.append(face)
+                    else:
+                        for point in points:
+                            face.append(self._position_of(point, face))
+                        self._faces.append(face)
+            return self._faces
+        except TypeError as error:
+            print(f'Error accessing sub polygons: {error}')
+            return None
+
+    @property
+    def trimesh(self) -> Union[Trimesh, None]:
+        """
+        Get polyhedron trimesh
+        :return: Trimesh
+        """
+        if self._trimesh is None:
+            if self.faces is not None:
+                for face in self.faces:
+                    if len(face) != 3:
+                        sys.stderr.write('Not able to generate trimesh\n')
+                        return None
+                self._trimesh = Trimesh(vertices=self.vertices, faces=self.faces)
+        return self._trimesh
+
+    @property
+    def volume(self):
+        """
+        Get polyhedron volume in cubic meters
+        :return: float
+        """
+        if self._volume is None:
+            if self.trimesh is None:
+                self._volume = np.inf
+            elif not self.trimesh.is_volume:
+                self._volume = np.inf
+            else:
+                self._volume = self.trimesh.volume
+        return self._volume
+
+    @property
+    def max_z(self):
+        """
+        Get polyhedron maximal z value in meters
+        :return: float
+        """
+        if self._max_z is None:
+            self._max_z = MIN_COORDINATE
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    self._max_z = max(self._max_z, point[2])
+        return self._max_z
+
+    @property
+    def max_y(self):
+        """
+        Get polyhedron maximal y value in meters
+        :return: float
+        """
+        if self._max_y is None:
+            self._max_y = MIN_COORDINATE
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    if self._max_y < point[1]:
+                        self._max_y = point[1]
+        return self._max_y
+
+    @property
+    def max_x(self):
+        """
+        Get polyhedron maximal x value in meters
+        :return: float
+        """
+        if self._max_x is None:
+            self._max_x = MIN_COORDINATE
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    self._max_x = max(self._max_x, point[0])
+        return self._max_x
+
+    @property
+    def min_z(self):
+        """
+        Get polyhedron minimal z value in meters
+        :return: float
+        """
+        if self._min_z is None:
+            self._min_z = self.max_z
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    if self._min_z > point[2]:
+                        self._min_z = point[2]
+        return self._min_z
+
+    @property
+    def min_y(self):
+        """
+        Get polyhedron minimal y value in meters
+        :return: float
+        """
+        if self._min_y is None:
+            self._min_y = self.max_y
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    if self._min_y > point[1]:
+                        self._min_y = point[1]
+        return self._min_y
+
+    @property
+    def min_x(self):
+        """
+        Get polyhedron minimal x value in meters
+        :return: float
+        """
+        if self._min_x is None:
+            self._min_x = self.max_x
+            for polygon in self._polygons:
+                for point in polygon.coordinates:
+                    if self._min_x > point[0]:
+                        self._min_x = point[0]
+        return self._min_x
+
+    @property
+    def centroid(self) -> Union[None, List[float]]:
+        """
+        Get polyhedron centroid
+        :return: [x,y,z]
+        """
+        if self._centroid is None:
+            trimesh = self.trimesh
+            if trimesh is None:
+                return None
+            self._centroid = self.trimesh.centroid
+        return self._centroid
+
+    def stl_export(self, full_path):
+        """
+        Export the polyhedron to stl given file
+        :param full_path: str
+        :return: None
+        """
+        self.trimesh.export(full_path, 'stl_ascii')
+
+    def obj_export(self, full_path):
+        """
+        Export the polyhedron to obj given file
+        :param full_path: str
+        :return: None
+        """
+        self.trimesh.export(full_path, 'obj')
+
+    def show(self):
+        """
+        Auxiliary function to render the polyhedron
+        :return: None
+        """
+        self.trimesh.show()
```

### Comparing `cerc-geometry-2.1.2/setup.py` & `cerc-geometry-2.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     for requirement
     in pkg_resources.parse_requirements(r)
   ]
 install_requires.append('setuptools')
 
 setuptools.setup(
   name="cerc-geometry",
-  version="2.1.2",
+  version="2.1.3",
   author="CERC",
   author_email=" cerc@concordia.ca",
   description="CERC Geometry Library with different modules to manipulate geometric objects",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://nextgenerations-cities.encs.concordia.ca/gitea/p_yefi/geometry",
   project_urls={
```

### Comparing `cerc-geometry-2.1.2/tests/test_plane.py` & `cerc-geometry-2.1.3/tests/test_plane.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,45 @@
-from geometry import Plane
-from geometry import Point
+"""
+Unit tests for plane
+"""
 from unittest import TestCase
 import numpy as np
+from geometry import Plane
+from geometry import Point
 
 
 class TestPlane(TestCase):
-  
-  def setUp(self) -> None:
-    self.plane = Plane(Point(np.array([10, 5, 6])), [2, 3, 5])
-    
-  def test_opposite_normal(self):
-    self.assertEqual(self.plane.opposite_normal[0], -2)
-    self.assertEqual(self.plane.opposite_normal[2], -5)
-    self.assertEqual(self.plane.origin.coordinates[1], 5)
-    self.assertNotEqual(self.plane.opposite_normal[1], 3)
-  
-  def test_equation(self):
-    self.assertTupleEqual(self.plane.equation, tuple([2, 3, 5, -65]))
-  
-  def test_equation_with_wrong_coordinates(self):
-    plane = Plane(Point(np.array([5, 6])), [2, 3, 5])
-    self.assertIsNone(plane.equation)
+    """
+    Plane test class
+    """
+
+    def setUp(self) -> None:
+        """
+        Set up for tests
+        :return: None
+        """
+        self.plane = Plane(Point(np.array([10, 5, 6])), [2, 3, 5])
+
+    def test_opposite_normal(self):
+        """
+        test for plan normal
+        :return:
+        """
+        self.assertEqual(self.plane.opposite_normal[0], -2)
+        self.assertEqual(self.plane.opposite_normal[2], -5)
+        self.assertEqual(self.plane.origin.coordinates[1], 5)
+        self.assertNotEqual(self.plane.opposite_normal[1], 3)
+
+    def test_equation(self):
+        """
+        Test plane equations
+        :return:
+        """
+        self.assertTupleEqual(self.plane.equation, tuple([2, 3, 5, -65]))
+
+    def test_equation_with_wrong_coordinates(self):
+        """
+        test equation with wrong coordinate values
+        :return:
+        """
+        plane = Plane(Point(np.array([5, 6])), [2, 3, 5])
+        self.assertIsNone(plane.equation)
```

### Comparing `cerc-geometry-2.1.2/tests/test_polygon.py` & `cerc-geometry-2.1.3/tests/test_polygon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,52 @@
+"""
+Unit tests for polygon
+"""
 from unittest import TestCase
+import numpy as np
 from geometry import Point
 from geometry import Polygon
-import numpy as np
 
 
 class TestPolygon(TestCase):
-  
-  def setUp(self) -> None:
-    self._coordinates = [[-1.3125511246773556, 7.224814483190954], [-1.3131144073658163, 7.225133803311778],
-                         [-1.3137179245338189, 7.225313420780125], [-1.3144622623732403, 7.2245550354264765],
-                         [-1.314663434762565, 7.222938472924113], [-1.3138989796833869, 7.221202158613096],
-                         [-1.3116860834049078, 7.219745246059503], [-1.3085477941360182, 7.220523597186585],
-                         [-1.3072401736067434, 7.223716818554365], [-1.3125511246773556, 7.224814483190954]]
-    self._vertices = [[0, 0, 1000], [1000, 0, 1000], [1000, 1000, 1000], [0, 1000, 1000], [0, 0, 0], [1000, 0, 0],
-                      [1000, 1000, 0], [0, 1000, 0]]
-    self.polygon = Polygon(np.array(self._coordinates))
-    self.polygon_2 = Polygon(np.array(self._vertices))
-  
-  def test_polygon_properties(self):
-    self.assertIsInstance(self.polygon.points[0], Point)
-    self.assertIsNone(self.polygon.points_list)
-    self.assertEqual(self.polygon.normal, [0, 0, 0])
-    self.assertEqual(self.polygon.points[0].coordinates[0], -1.3125511246773556)
-    self.assertEqual(self.polygon.inverse[0][0], -1.3125511246773556)
-    self.assertIsNone(self.polygon_2.triangles)  # issue with trimesh module import
-    self.assertEqual(self.polygon_2.vertices.size, 0)  # issue with trimesh module import
+    """
+    Polygon test class
+    """
+
+    def setUp(self) -> None:
+        """
+        Set up for tests
+        :return: None
+        """
+        self._coordinates = [
+            [-1.3125511246773556, 7.224814483190954],
+            [-1.3131144073658163, 7.225133803311778],
+            [-1.3137179245338189, 7.225313420780125],
+            [-1.3144622623732403, 7.2245550354264765],
+            [-1.314663434762565, 7.222938472924113],
+            [-1.3138989796833869, 7.221202158613096],
+            [-1.3116860834049078, 7.219745246059503],
+            [-1.3085477941360182, 7.220523597186585],
+            [-1.3072401736067434, 7.223716818554365],
+            [-1.3125511246773556, 7.224814483190954]
+        ]
+        self._vertices = [
+            [0, 0, 1000], [1000, 0, 1000],
+            [1000, 1000, 1000], [0, 1000, 1000],
+            [0, 0, 0], [1000, 0, 0],
+            [1000, 1000, 0], [0, 1000, 0]
+        ]
+        self.polygon = Polygon(np.array(self._coordinates))
+        self.polygon_2 = Polygon(np.array(self._vertices))
+
+    def test_polygon_properties(self):
+        """
+        Test for polygon properties
+        :return:
+        """
+        self.assertIsInstance(self.polygon.points[0], Point)
+        self.assertIsNone(self.polygon.points_list)
+        self.assertEqual(self.polygon.normal, [0, 0, 0])
+        self.assertEqual(self.polygon.points[0].coordinates[0], -1.3125511246773556)
+        self.assertEqual(self.polygon.inverse[0][0], -1.3125511246773556)
+        self.assertIsNone(self.polygon_2.triangles)  # issue with trimesh module import
+        self.assertEqual(self.polygon_2.vertices.size, 0)  # issue with trimesh module import
```

