# Comparing `tmp/dreifus-0.0.6.tar.gz` & `tmp/dreifus-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-9t5ppmgm/dreifus-0.0.6.tar", last modified: Wed Apr 19 23:40:52 2023, max compression
+gzip compressed data, was "/mnt/d/Projects/dreifus/dist/.tmp-qc7pkx08/dreifus-0.0.7.tar", last modified: Fri Jun  2 08:59:47 2023, max compression
```

## Comparing `dreifus-0.0.6.tar` & `dreifus-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-19 23:40:52.000000 dreifus-0.0.6/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.6/README.md
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-04-19 23:39:41.000000 dreifus-0.0.6/pyproject.toml
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-04-19 23:40:52.000000 dreifus-0.0.6/setup.cfg
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.6/setup.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.6/src/dreifus/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.6/src/dreifus/camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.6/src/dreifus/camera_bundle.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.6/src/dreifus/graphics.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/matrix/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.6/src/dreifus/matrix/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.6/src/dreifus/matrix/intrinsics_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.6/src/dreifus/matrix/intrinsics_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.6/src/dreifus/matrix/pose_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17557 2023-04-19 21:54:10.000000 dreifus-0.0.6/src/dreifus/matrix/pose_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.6/src/dreifus/matrix/pose_torch.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.6/src/dreifus/matrix/transform_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.6/src/dreifus/pyvista.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3367 2023-02-24 12:49:30.000000 dreifus-0.0.6/src/dreifus/trajectory.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus/util/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.6/src/dreifus/util/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.6/src/dreifus/util/typing.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/src/dreifus/vector/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.6/src/dreifus/vector/__init__.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.6/src/dreifus/vector/vector_base.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5371 2023-04-11 15:56:31.000000 dreifus-0.0.6/src/dreifus/vector/vector_numpy.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.6/src/dreifus/vector/vector_torch.py
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:51.000000 dreifus-0.0.6/src/dreifus.egg-info/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/PKG-INFO
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/SOURCES.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/dependency_links.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/requires.txt
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-04-19 23:40:50.000000 dreifus-0.0.6/src/dreifus.egg-info/top_level.txt
-drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-04-19 23:40:52.000000 dreifus-0.0.6/test/
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.6/test/test_camera.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.6/test/test_intrinsics.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.6/test/test_pose.py
--rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.6/test/test_vector.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.645101 dreifus-0.0.7/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-02 08:59:47.637962 dreifus-0.0.7/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       10 2023-02-13 11:32:40.000000 dreifus-0.0.7/README.md
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1087 2023-06-02 08:58:21.000000 dreifus-0.0.7/pyproject.toml
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       38 2023-06-02 08:59:47.646656 dreifus-0.0.7/setup.cfg
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      151 2023-02-13 09:12:52.000000 dreifus-0.0.7/setup.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.481742 dreifus-0.0.7/src/
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.788377 dreifus-0.0.7/src/dreifus/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 08:09:12.000000 dreifus-0.0.7/src/dreifus/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5520 2023-04-11 17:10:32.000000 dreifus-0.0.7/src/dreifus/camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5078 2023-04-11 17:41:05.000000 dreifus-0.0.7/src/dreifus/camera_bundle.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1483 2023-02-24 11:10:52.000000 dreifus-0.0.7/src/dreifus/graphics.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.258176 dreifus-0.0.7/src/dreifus/matrix/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      251 2023-04-11 16:52:12.000000 dreifus-0.0.7/src/dreifus/matrix/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5852 2023-02-23 11:03:29.000000 dreifus-0.0.7/src/dreifus/matrix/intrinsics_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3655 2023-02-13 10:22:40.000000 dreifus-0.0.7/src/dreifus/matrix/intrinsics_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1315 2023-02-13 11:10:42.000000 dreifus-0.0.7/src/dreifus/matrix/pose_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    17557 2023-04-19 21:54:10.000000 dreifus-0.0.7/src/dreifus/matrix/pose_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)    13757 2023-02-13 11:30:59.000000 dreifus-0.0.7/src/dreifus/matrix/pose_torch.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1329 2023-03-08 15:24:39.000000 dreifus-0.0.7/src/dreifus/matrix/transform_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     9414 2023-04-19 22:07:01.000000 dreifus-0.0.7/src/dreifus/pyvista.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3441 2023-05-22 13:04:13.000000 dreifus-0.0.7/src/dreifus/trajectory.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.322200 dreifus-0.0.7/src/dreifus/util/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-02-13 10:08:11.000000 dreifus-0.0.7/src/dreifus/util/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      274 2023-02-13 10:10:21.000000 dreifus-0.0.7/src/dreifus/util/typing.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.493856 dreifus-0.0.7/src/dreifus/vector/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      219 2023-02-13 13:27:37.000000 dreifus-0.0.7/src/dreifus/vector/__init__.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2078 2023-02-13 13:27:37.000000 dreifus-0.0.7/src/dreifus/vector/vector_base.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     5740 2023-05-22 13:07:11.000000 dreifus-0.0.7/src/dreifus/vector/vector_numpy.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     2340 2023-02-13 09:58:17.000000 dreifus-0.0.7/src/dreifus/vector/vector_torch.py
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:46.965796 dreifus-0.0.7/src/dreifus.egg-info/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      464 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/PKG-INFO
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)      873 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        1 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)       63 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/requires.txt
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)        8 2023-06-02 08:59:46.000000 dreifus-0.0.7/src/dreifus.egg-info/top_level.txt
+drwxrwxrwx   0 tobias    (1000) tobias    (1000)        0 2023-06-02 08:59:47.608820 dreifus-0.0.7/test/
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1165 2023-02-13 14:36:25.000000 dreifus-0.0.7/test/test_camera.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     1439 2023-02-13 10:23:32.000000 dreifus-0.0.7/test/test_intrinsics.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3487 2023-02-13 15:28:18.000000 dreifus-0.0.7/test/test_pose.py
+-rwxrwxrwx   0 tobias    (1000) tobias    (1000)     3677 2023-02-13 11:26:58.000000 dreifus-0.0.7/test/test_vector.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dreifus-0.0.6/pyproject.toml` & `dreifus-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dreifus"
-version = "0.0.6"
+version = "0.0.7"
 description = "dreifus lifts your 3D camera experience and facilitates computer vision applications"
 authors = [
     { name = "Tobias Kirschstein", email = "tobias.kirschstein@gmail.com" },
 ]
 readme = "README.md"
 license = { text = "Apache 2.0" }
 requires-python = ">=3.8.0"
```

### Comparing `dreifus-0.0.6/src/dreifus/camera.py` & `dreifus-0.0.7/src/dreifus/camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/camera_bundle.py` & `dreifus-0.0.7/src/dreifus/camera_bundle.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/graphics.py` & `dreifus-0.0.7/src/dreifus/graphics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/intrinsics_numpy.py` & `dreifus-0.0.7/src/dreifus/matrix/intrinsics_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/intrinsics_torch.py` & `dreifus-0.0.7/src/dreifus/matrix/intrinsics_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/pose_base.py` & `dreifus-0.0.7/src/dreifus/matrix/pose_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/pose_numpy.py` & `dreifus-0.0.7/src/dreifus/matrix/pose_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/pose_torch.py` & `dreifus-0.0.7/src/dreifus/matrix/pose_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/matrix/transform_numpy.py` & `dreifus-0.0.7/src/dreifus/matrix/transform_numpy.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/pyvista.py` & `dreifus-0.0.7/src/dreifus/pyvista.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/trajectory.py` & `dreifus-0.0.7/src/dreifus/trajectory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from math import cos, sin
 from typing import Optional, List
 
 import numpy as np
 
+from dreifus.camera import PoseType
 from dreifus.matrix import Pose
 from dreifus.vector import Vec3
 
 
 def point_around_axis(theta: float,
                       axis: Vec3 = Vec3(0, 0, 1)) -> Vec3:
     """
@@ -36,15 +37,15 @@
                        axis=Vec3(0, 0, 1),
                        up: Vec3 = Vec3(0, 0, 1),
                        move=Vec3(),
                        distance: float = 1.0,
                        distance_end: Optional[float] = None,
                        theta_from: float = 0,
                        theta_to: float = 2 * np.pi,
-                       look_at: Vec3 = Vec3()) -> List[Pose]:
+                       look_at: Vec3 = Vec3(0, 0, 0)) -> List[Pose]:
     """
     Computes `n_poses` many camera poses (cam2world) that circle with distance `distance` around the specified `axis`
     that is moved by `move`.
     Per default, one full circle is computed. With `theta_from` and `theta_to` one can specify parts of the circle
     or even multiple circulations around the axis.
 
     Parameters
@@ -80,15 +81,15 @@
     poses = []
     for i_pose in range(n_poses):
         alpha = i_pose / n_poses
         theta = theta_from + alpha * (theta_from - theta_to)
         distance = distance_start + alpha * (distance_end - distance_start)
         location = distance * point_around_axis(theta, axis=axis)
 
-        pose = Pose()
+        pose = Pose(pose_type=PoseType.CAM_2_WORLD)
         location += move
         pose.set_translation(location)
         pose.look_at(look_at, up=up)
 
         poses.append(pose)
 
     return poses
```

### Comparing `dreifus-0.0.6/src/dreifus/vector/vector_base.py` & `dreifus-0.0.7/src/dreifus/vector/vector_base.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus/vector/vector_numpy.py` & `dreifus-0.0.7/src/dreifus/vector/vector_numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,23 @@
 
     def cross(self, other: 'Vec3') -> 'Vec3':
         return Vec3(np.cross(self, other))
 
     def homogenize(self) -> 'Vec4':
         return Vec4(self, 1)
 
+    def sum(self) -> float:
+        # Ensure that .sum() does not return a Vec3 object with just one value
+        return super(Vec3, self).sum().item()
+
+    def __eq__(self, other) -> bool:
+        assert isinstance(other, Vec3), "Can only compare against other Vec3 instances"
+
+        return (self.x == other.x and self.y == other.y and self.z == other.z)
+
 
 class Vec4(np.ndarray):
     def __new__(cls,
                 x: Union[float, Tuple[float, float, float, float], np.ndarray, 'Vec4', 'Vec3'],
                 y: Optional[float] = None,
                 z: Optional[float] = None,
                 w: Optional[float] = None) -> 'Vec4':
```

### Comparing `dreifus-0.0.6/src/dreifus/vector/vector_torch.py` & `dreifus-0.0.7/src/dreifus/vector/vector_torch.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/src/dreifus.egg-info/SOURCES.txt` & `dreifus-0.0.7/src/dreifus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/test/test_camera.py` & `dreifus-0.0.7/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/test/test_intrinsics.py` & `dreifus-0.0.7/test/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/test/test_pose.py` & `dreifus-0.0.7/test/test_pose.py`

 * *Files identical despite different names*

### Comparing `dreifus-0.0.6/test/test_vector.py` & `dreifus-0.0.7/test/test_vector.py`

 * *Files identical despite different names*

