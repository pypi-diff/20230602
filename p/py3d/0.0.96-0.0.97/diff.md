# Comparing `tmp/py3d-0.0.96.tar.gz` & `tmp/py3d-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.96.tar", last modified: Mon May 29 15:54:55 2023, max compression
+gzip compressed data, was "py3d-0.0.97.tar", last modified: Fri Jun  2 15:23:10 2023, max compression
```

## Comparing `py3d-0.0.96.tar` & `py3d-0.0.97.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:54:55.569288 py3d-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-05-29 15:54:29.000000 py3d-0.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27956 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 15:54:55.569288 py3d-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-29 15:53:50.000000 py3d-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-02 15:23:10.783317 py3d-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-02 15:22:45.000000 py3d-0.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28253 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-06-02 15:21:54.000000 py3d-0.0.97/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:23:10.783317 py3d-0.0.97/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-02 15:23:10.000000 py3d-0.0.97/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 15:23:10.783317 py3d-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-02 15:21:54.000000 py3d-0.0.97/setup.py
```

### Comparing `py3d-0.0.96/PKG-INFO` & `py3d-0.0.97/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.96
+Version: 0.0.97
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -44,15 +44,14 @@
 
 ```
 
 ![example](docs/index.gif)
 
 ### API reference
 
-[Data](https://tumiz.github.io/scenario/Data.html)
 [Vector](https://tumiz.github.io/scenario/Vector.html)
 [Vector3](https://tumiz.github.io/scenario/Vector3.html)
 [Vector4](https://tumiz.github.io/scenario/Vector4.html)
 [Transform](https://tumiz.github.io/scenario/Transform.html)
 [Rotation](https://tumiz.github.io/scenario/Rotation.html)
 [Color](https://tumiz.github.io/scenario/Color.html)
```

### Comparing `py3d-0.0.96/README.md` & `py3d-0.0.97/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 ```
 
 ![example](docs/index.gif)
 
 ### API reference
 
-[Data](https://tumiz.github.io/scenario/Data.html)
 [Vector](https://tumiz.github.io/scenario/Vector.html)
 [Vector3](https://tumiz.github.io/scenario/Vector3.html)
 [Vector4](https://tumiz.github.io/scenario/Vector4.html)
 [Transform](https://tumiz.github.io/scenario/Transform.html)
 [Rotation](https://tumiz.github.io/scenario/Rotation.html)
 [Color](https://tumiz.github.io/scenario/Color.html)
```

### Comparing `py3d-0.0.96/py3d/core.py` & `py3d-0.0.97/py3d/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,21 +134,37 @@
             ret.append(tmp)
     ret = Vector(ret)
     for i, c in enumerate(cols):
         setattr(ret, c, ret[:, i])
     return ret
 
 
-class Data(numpy.ndarray):
+def read_csv(path):
+    return numpy.loadtxt(path, delimiter=',').view(Vector)
+
+
+class Vector(numpy.ndarray):
+    '''
+    Base class of Vector2, Vector3, Vector4 and Transform
+    '''
     BASE_SHAPE = ()
 
-    def __new__(cls, data: list | numpy.ndarray = [], n=()):
-        return numpy.tile(data, n + (1,)).view(cls)
+    def __new__(cls, data: list | numpy.ndarray = []):
+        nd = numpy.array(data)
+        if cls.BASE_SHAPE:
+            bn = len(cls.BASE_SHAPE)
+            ret = numpy.zeros(nd.shape[:-bn]+cls.BASE_SHAPE)
+            c = numpy.minimum(cls.BASE_SHAPE, nd.shape[-bn:])
+            mask = ..., *[slice(s) for s in c]
+            ret[mask] = nd[mask]
+            return ret.view(cls)
+        else:
+            return nd.view(cls)
 
-    def __imatmul__(self, value) -> Data:
+    def __imatmul__(self, value) -> Vector:
         return self @ value
 
     def tile(self, *n):
         return numpy.tile(self, n + self.ndim * (1,))
 
     def flatten(self):
         return self.reshape(-1, *self.BASE_SHAPE)
@@ -158,31 +174,21 @@
         base_dims = len(self.BASE_SHAPE)
         if base_dims:
             return self.shape[:-base_dims]
         else:
             return self.shape
 
     @classmethod
-    def Rand(cls, *n) -> Data:
+    def rand(cls, *n) -> Vector:
         n += cls.BASE_SHAPE
         return numpy.random.rand(*n).view(cls)
 
-    @classmethod
-    def load_csv(cls, path):
-        return numpy.loadtxt(path, delimiter=',').view(cls)
-
-    def save_csv(self, path):
+    def to_csv(self, path):
         numpy.savetxt(path, self, delimiter=',')
 
-
-class Vector(Data):
-    # Base class of Vector2, Vector3, Vector4
-    def __new__(cls, data: list | numpy.ndarray = [], n=()):
-        return super().__new__(cls, data, n)
-
     @property
     def x(self):
         return self[..., 0].view(numpy.ndarray)
 
     @x.setter
     def x(self, v):
         self[..., 0] = v
@@ -284,39 +290,39 @@
             f.write(" ".join([str(a) for a in p]) + "\n")
         f.close()
 
 
 class Vector2(Vector):
     BASE_SHAPE = 2,
 
-    def __new__(cls, data: list | numpy.ndarray = [], n=()):
-        return super().__new__(cls, data, n)
+    def __new__(cls, data: list | numpy.ndarray = []):
+        return super().__new__(cls, data)
 
 
 class Vector3(Vector):
     BASE_SHAPE = 3,
 
-    def __new__(cls, data: list | numpy.ndarray = [], x=0, y=0, z=0, n=()):
+    def __new__(cls, data: list | numpy.ndarray = [], x=0, y=0, z=0):
         '''
             Represent points, positions and translations
         '''
         if numpy.any(data):
-            return super().__new__(cls, data, n)
+            return super().__new__(cls, data)
         else:
-            n += max(numpy.shape(x), numpy.shape(y), numpy.shape(z))
-            ret = super().__new__(cls, [0., 0., 0.], n)
+            n = max(numpy.shape(x), numpy.shape(y), numpy.shape(z))
+            ret = numpy.empty(n + cls.BASE_SHAPE).view(cls)
             ret.x = x
             ret.y = y
             ret.z = z
             return ret
 
     @classmethod
     def grid(cls, x=0, y=0, z=0) -> Vector3:
         n = numpy.shape(x) + numpy.shape(y) + numpy.shape(z)
-        ret = super().__new__(cls, [0., 0., 0.], n)
+        ret = numpy.empty(n+(3, )).view(Vector3)
         i = numpy.arange(len(n))
         ret.x = numpy.expand_dims(x, axis=i[i != 0].tolist())
         ret.y = numpy.expand_dims(y, axis=i[i != 1].tolist())
         ret.z = numpy.expand_dims(z, axis=i[i != 2].tolist())
         return ret
 
     @classmethod
@@ -382,15 +388,15 @@
         return p0 + (self - p0).vector_projection(p1 - p0)
 
     def projection_on_plane(self, plane) -> numpy.ndarray:
         return self + (plane.position[:, numpy.newaxis] - self).vector_projection(
             plane.normal[:, numpy.newaxis]
         )
 
-    def interpolate(self, x, xp) -> Vector3:
+    def lerp(self, x, xp) -> Vector3:
         '''
         linear interpolation
         x: 1-D array, the data to be interpolated.
         xp: 1-D array, the data to interpolate into. For example, time series.
         '''
         x = numpy.array(x)
         xp = numpy.array(xp)
@@ -400,26 +406,19 @@
         x1 = xp[i]
         d = ((x-x0)/(x1-x0)).reshape(-1, 1)
         f0 = self[i-1]
         f1 = self[i]
         return (1-d)*f0+d*f1
 
     def as_scaling(self) -> Transform:
-        ret = Transform(n=self.n)
+        ret = Transform
         ret[..., 0, 0] = self[..., 0]
         ret[..., 1, 1] = self[..., 1]
         ret[..., 2, 2] = self[..., 2]
-        return ret
-
-    def as_translation(self) -> Transform:
-        ret = Transform(n=self.n)
-        ret[..., 3, 0] = self[..., 0]
-        ret[..., 3, 1] = self[..., 1]
-        ret[..., 3, 2] = self[..., 2]
-        return ret
+        return ret.view(Transform)
 
     def as_point(self) -> Point:
         entity = Point(*self.n)
         entity.xyz = self
         return entity
 
     def as_line(self) -> LineSegment:
@@ -461,21 +460,21 @@
         entity.end.xyz = numpy.expand_dims(self, axis=self.ndim - 1)
         return entity
 
 
 class Vector4(Vector):
     BASE_SHAPE = 4,
 
-    def __new__(cls, xyzw_list: list | numpy.ndarray = [], x=0, y=0, z=0, w=1, n=()):
+    def __new__(cls, xyzw_list: list | numpy.ndarray = [], x=0, y=0, z=0, w=1):
         if numpy.any(xyzw_list):
-            return super().__new__(cls, xyzw_list, n)
+            return super().__new__(cls, xyzw_list)
         else:
-            n += max(numpy.shape(x), numpy.shape(y),
-                     numpy.shape(z), numpy.shape(w))
-            ret = super().__new__(cls, [0., 0., 0., 1.], n)
+            n = max(numpy.shape(x), numpy.shape(y),
+                    numpy.shape(z), numpy.shape(w))
+            ret = numpy.empty(n + cls.BASE_SHAPE).view(cls)
             ret.x = x
             ret.y = y
             ret.z = z
             ret.w = w
             return ret
 
     @property
@@ -484,147 +483,157 @@
 
     @w.setter
     def w(self, v):
         self[..., 3] = v
 
     @property
     def wxyz(self) -> Vector:
-        ret = Vector([0., 0., 0., 0.], n=self.n)
+        ret = numpy.empty(self.n + self.BASE_SHAPE).view(Vector)
         ret[..., 0] = self.w
         ret[..., 1:4] = self.xyz
         return ret
 
     def from_axis_angle_to_quaternion(self) -> Vector4:
-        q = Vector4(n=self.n)
+        q = numpy.empty(self.n + self.BASE_SHAPE).view(Vector4)
         q.xyz = numpy.sin(self.w / 2)[..., numpy.newaxis] * self.xyz.U
         q.w = numpy.cos(self.w / 2)
         return q
 
     def from_quaternion_to_axis_angle(self) -> Vector4:
-        q = Vector4(n=self.n)
+        q = numpy.empty(self.n + self.BASE_SHAPE).view(Vector4)
         q.w = numpy.arccos(self.w) * 2
         sin_ha = numpy.sin(q.w / 2)[..., numpy.newaxis]
         q.xyz = numpy.divide(self.xyz, sin_ha,
                              where=sin_ha != 0)
         return q
 
 
-class Transform(Data):
+class Transform(Vector):
     BASE_SHAPE = 4, 4
 
-    def __new__(cls, data: list | numpy.ndarray = numpy.eye(4), n=()):
-        return super().__new__(cls, data, n + (1,))
+    def __new__(cls, data: list | numpy.ndarray = numpy.eye(4)):
+        return super().__new__(cls, data)
 
     @classmethod
-    def from_translation(cls, xyz_list: list | numpy.ndarray = [], x=0, y=0, z=0, n=()) -> Transform:
+    def from_translation(cls, xyz_list: list | numpy.ndarray = [], x=0, y=0, z=0) -> Transform:
         '''
         translation matrix
         '''
-        return Vector3(xyz_list, x, y, z, n).as_translation()
+        vec = Vector3(xyz_list, x, y, z)
+        ret = Transform().tile(*vec.n)
+        ret[..., 3, 0] = vec[..., 0]
+        ret[..., 3, 1] = vec[..., 1]
+        ret[..., 3, 2] = vec[..., 2]
+        return ret
 
     @classmethod
-    def from_scaling(cls, xyz_list: list | numpy.ndarray = [], x=1, y=1, z=1, n=()) -> Transform:
+    def from_scaling(cls, xyz_list: list | numpy.ndarray = [], x=1, y=1, z=1) -> Transform:
         '''
         scaling matrix
         '''
-        return Vector3(xyz_list, x, y, z, n).as_scaling()
+        vec = Vector3(xyz_list, x, y, z)
+        ret = Transform().tile(*vec.n)
+        ret[..., 0, 0] = vec[..., 0]
+        ret[..., 1, 1] = vec[..., 1]
+        ret[..., 2, 2] = vec[..., 2]
+        return ret
 
     @classmethod
-    def Rx(cls, a, n=()) -> Transform:
+    def Rx(cls, a) -> Transform:
         a = numpy.array(a)
-        ret = numpy.full(n + a.shape + (4, 4), numpy.eye(4))
+        ret = numpy.full(a.shape + (4, 4), numpy.eye(4))
         cos = numpy.cos(a)
         sin = numpy.sin(a)
         ret[..., 1, 1] = cos
         ret[..., 1, 2] = sin
         ret[..., 2, 1] = -sin
         ret[..., 2, 2] = cos
         return ret.view(cls)
 
-    def rx(self, a, n=()) -> Transform:
-        return self @ self.Rx(a, n)
+    def rx(self, a) -> Transform:
+        return self @ self.Rx(a)
 
     @classmethod
-    def Ry(cls, a, n=()) -> Transform:
+    def Ry(cls, a) -> Transform:
         a = numpy.array(a)
-        ret = numpy.full(n + a.shape + (4, 4), numpy.eye(4))
+        ret = numpy.full(a.shape + (4, 4), numpy.eye(4))
         cos = numpy.cos(a)
         sin = numpy.sin(a)
         ret[..., 0, 0] = cos
         ret[..., 0, 2] = -sin
         ret[..., 2, 0] = sin
         ret[..., 2, 2] = cos
         return ret.view(cls)
 
-    def ry(self, a, n=()) -> Transform:
-        return self @ self.Ry(a, n)
+    def ry(self, a) -> Transform:
+        return self @ self.Ry(a)
 
     @classmethod
-    def Rz(cls, a, n=()) -> Transform:
+    def Rz(cls, a) -> Transform:
         a = numpy.array(a)
-        ret = numpy.full(n + a.shape + (4, 4), numpy.eye(4))
+        ret = numpy.full(a.shape + (4, 4), numpy.eye(4))
         cos = numpy.cos(a)
         sin = numpy.sin(a)
         ret[..., 0, 0] = cos
         ret[..., 0, 1] = sin
         ret[..., 1, 0] = -sin
         ret[..., 1, 1] = cos
         return ret.view(cls)
 
-    def rz(self, a, n=()) -> Transform:
-        return self @ self.Rz(a, n)
+    def rz(self, a) -> Transform:
+        return self @ self.Rz(a)
 
     @classmethod
-    def from_axis_angle(cls, xyz_angle_list: list | Vector4 = [], axis=[0, 0, 1], angle=0, n=()) -> Transform:
+    def from_axis_angle(cls, xyz_angle_list: list | Vector4 = [], axis=[0, 0, 1], angle=0) -> Transform:
         axis = Vector3(axis)
         q = Vector4(xyz_angle_list, axis.x, axis.y, axis.z,
-                    angle, n).from_axis_angle_to_quaternion()
+                    angle).from_axis_angle_to_quaternion()
         return cls.from_quaternion(q)
 
     def as_axis_angle(self):
         return self.as_quaternion().from_quaternion_to_axis_angle()
 
     @classmethod
-    def from_rotation_vector(cls, xyz_list: list | Vector3 = [], x=0, y=0, z=0, n=()) -> Transform:
-        rv = Vector3(xyz_list, x, y, z, n)
-        axis_angle_list = Vector4(n=rv.n)
+    def from_rotation_vector(cls, xyz_list: list | Vector3 = [], x=0, y=0, z=0) -> Transform:
+        rv = Vector3(xyz_list, x, y, z)
+        axis_angle_list = Vector4().tile(*rv.n)
         axis_angle_list.w = rv.L
         axis_angle_list.xyz = rv.U
         return cls.from_axis_angle(axis_angle_list)
 
     def as_rotation_vector(self):
         q = self.as_axis_angle()
         return q.xyz.U * q.w
 
     @classmethod
     def from_two_vectors(cls, a: list | Vector3, b: list | Vector3) -> Transform:
         a = Vector3(a)
         b = Vector3(b)
-        q = Vector4(n=max(a.n, b.n))
+        q = Vector4().tile(*max(a.n, b.n))
         q.w = a.angle_to_vector(b).squeeze()
         q.xyz = a.cross(b)
         return cls.from_axis_angle(q)
 
     @classmethod
     def from_quaternion(cls, xyzw_list: list | numpy.ndarray) -> Transform:
         q = Vector4(xyzw_list)
-        ret = cls(n=q.shape[:-1])
+        ret = Transform().tile(*q.shape[:-1])
         ret[..., 0, 0] = 1 - 2 * q.y ** 2 - 2 * q.z ** 2
         ret[..., 0, 1] = 2 * q.w * q.z + 2 * q.x * q.y
         ret[..., 0, 2] = -2 * q.w * q.y + 2 * q.x * q.z
         ret[..., 1, 0] = -2 * q.w * q.z + 2 * q.x * q.y
         ret[..., 1, 1] = 1 - 2 * q.x ** 2 - 2 * q.z ** 2
         ret[..., 1, 2] = 2 * q.w * q.x + 2 * q.y * q.z
         ret[..., 2, 0] = 2 * q.w * q.y + 2 * q.x * q.z
         ret[..., 2, 1] = -2 * q.w * q.x + 2 * q.y * q.z
         ret[..., 2, 2] = 1 - 2 * q.x ** 2 - 2 * q.y ** 2
         return ret
 
     def as_quaternion(self) -> Vector4:
-        q = Vector4(n=self.n)
+        q = Vector4().tile(*self.n)
         q.w = numpy.sqrt(1+self[..., 0, 0]+self[..., 1, 1] + self[..., 2, 2])/2
         m0 = self[q.w == 0]
         m1, w1 = self[q.w != 0], q.w[q.w != 0]
         q.x[q.w != 0] = numpy.divide(m1[..., 1, 2]-m1[..., 2, 1], 4*w1)
         q.y[q.w != 0] = numpy.divide(m1[..., 2, 0]-m1[..., 0, 2], 4*w1)
         q.z[q.w != 0] = numpy.divide(m1[..., 0, 1]-m1[..., 1, 0], 4*w1)
         q.x[q.w == 0] = sign(m0[..., 1, 2]-m0[..., 2, 1]) * numpy.sqrt(
@@ -644,15 +653,15 @@
             return m[lo[0]](v[..., 0]) @ m[lo[1]](v[..., 1]) @ m[lo[2]](v[..., 2])
         else:
             return m[lo[2]](v[..., 2]) @ m[lo[1]](v[..., 1]) @ m[lo[0]](v[..., 0])
 
     def as_euler(self, sequence: str):
         extrinsic = sequence.islower()
         lo = sequence.lower()
-        ret = Vector3(n=self.n)
+        ret = Vector3().tile(*self.n)
         i = [0, 1, 2] if extrinsic else [2, 1, 0]
         m = [0 if o == 'x' else 1 if o == 'y' else 2 for o in lo]
         if not extrinsic:
             m.reverse()
 
         def f(x, y): return -1 if x-y == 2 or x - y == -1 else 1
         a = [f(m[1], m[0]), f(m[2], m[0]), f(m[2], m[1])]
@@ -735,15 +744,15 @@
             [0, 0, -2 * near * far * range_inv, 0]
         ])
 
     @classmethod
     def from_orthographic(cls, l, r, t, b, n, f):
         pass
 
-    def interpolate(self, x, xp) -> Transform:
+    def lerp(self, x, xp) -> Transform:
         '''
         Linear interpolation
         x: 1-D array, the data to be interpolated.
         xp: 1-D array, the data to interpolate into. For example, time series.
         Only translation, rotation and scaling can be interpolated
         '''
         xp = numpy.array(xp)
@@ -756,51 +765,54 @@
         r1: Transform = self.rotation[i]
         t0: Vector3 = self.translation_vector[i-1]
         t1: Vector3 = self.translation_vector[i]
         s0: Vector3 = self.scaling_vector[i-1]
         s1: Vector3 = self.scaling_vector[i]
         angle, axis = (r0.I@r1).as_angle_axis()
         rotation = Transform.from_angle_axis(d*angle, axis)
-        translation = (d[..., numpy.newaxis] * (t1 - t0)).as_translation()
-        scaling = (d[..., numpy.newaxis] * s1 / s0).as_scaling()
+        translation = Transform.from_translation(
+            d[..., numpy.newaxis] * (t1 - t0))
+        scaling = Transform.from_scaling(
+            d[..., numpy.newaxis] * s1 / s0).as_scaling()
         return self[i-1]@scaling@rotation@translation
 
 
 class Color(Vector):
     BASE_SHAPE = 4,
 
-    def __new__(cls, data: numpy.ndarray | list = [], r=0, g=0, b=0, a=1, n=()):
+    def __new__(cls, data: numpy.ndarray | list = [], r=0, g=0, b=0, a=1):
         if numpy.any(data):
-            return super().__new__(cls, data, n)
+            return super().__new__(cls, data)
         else:
-            n += max(numpy.shape(r), numpy.shape(g),
-                     numpy.shape(b), numpy.shape(a))
-            ret = super().__new__(cls, [0., 0., 0., 1.], n)
+            n = max(numpy.shape(r), numpy.shape(g),
+                    numpy.shape(b), numpy.shape(a))
+            ret = numpy.empty(n + cls.BASE_SHAPE)
             ret[..., 0] = r
             ret[..., 1] = g
             ret[..., 2] = b
             ret[..., 3] = a
-        return ret
+            return ret.view(cls)
 
     @classmethod
     def map(cls, value, start, end):
         center = (start + end)/2
         width = (end - start)/2
         r = numpy.maximum(value - center, 0)/width
         g = 1-numpy.abs(value - center)/width
         b = numpy.maximum(center - value, 0)/width
         return cls(r=r, g=g, b=b)
 
     @classmethod
-    def standard(cls, *n):
+    def standard(cls, n):
         size = numpy.prod(n)
         c = int(numpy.power(size, 1/3)) + 1
         s = numpy.linspace(.3, 1, c)
-        rgb = Vector3.grid(x=s, y=s, z=s).flatten()[:size]
-        return cls(rgb.H).reshape(n + (4,))
+        rgb: Vector3 = Vector3.grid(x=s, y=s, z=s).flatten()[
+            :size].reshape(n+(3,))
+        return rgb.H.view(cls)
 
     @property
     def r(self):
         return self[..., 0].view(numpy.ndarray)
 
     @r.setter
     def r(self, v):
@@ -837,15 +849,15 @@
 
 class Point(Vector):
     BASE_SHAPE = 7,
     TYPE = "POINTS"
 
     def __new__(cls, *n):
         ret = numpy.empty(n + cls.BASE_SHAPE).view(cls)
-        ret.color = Color.standard(*(n[:-1] + (1,)))
+        ret.color = Color.standard(n[:-1] + (1,))
         ret.color.a = 1
         return ret
 
     @property
     def color(self) -> Color:
         return self[..., 3:7].view(Color)
 
@@ -920,16 +932,16 @@
     size_x = wheelbase+front_overhang+rear_overhang
     size_y = track_width
     size_z = height-wheel_radius
     body = cube(size_x, size_y, size_z).xyz
     body @= Transform.from_translation(x=size_x /
                                        2-rear_overhang, z=size_z/2+wheel_radius)
     wheel = Vector3.circle(wheel_radius).as_lineloop().xyz
-    wheel @= Transform.from_rpy([pi/2, 0, 0]) @ Vector3.grid(x=[wheelbase, 0], y=[-size_y/2, size_y/2], z=wheel_radius
-                                                             ).as_translation()
+    wheel @= Transform.from_rpy([pi/2, 0, 0]) @ Transform.from_translation(
+        Vector3.grid(x=[wheelbase, 0], y=[-size_y/2, size_y/2], z=wheel_radius))
     return numpy.vstack((body.flatten(), wheel.flatten())).view(Vector3).as_linesegment()
 
 
 def axis(size=5) -> LineSegment:
     a = Vector3([[size, 0, 0], [0, size, 0], [0, 0, size]]).as_vector()
     a[0].color = Color(r=1)
     a[1].color = Color(g=1)
```

### Comparing `py3d-0.0.96/py3d/viewer.html` & `py3d-0.0.97/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.0.96/py3d.egg-info/PKG-INFO` & `py3d-0.0.97/py3d.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.96
+Version: 0.0.97
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
@@ -44,15 +44,14 @@
 
 ```
 
 ![example](docs/index.gif)
 
 ### API reference
 
-[Data](https://tumiz.github.io/scenario/Data.html)
 [Vector](https://tumiz.github.io/scenario/Vector.html)
 [Vector3](https://tumiz.github.io/scenario/Vector3.html)
 [Vector4](https://tumiz.github.io/scenario/Vector4.html)
 [Transform](https://tumiz.github.io/scenario/Transform.html)
 [Rotation](https://tumiz.github.io/scenario/Rotation.html)
 [Color](https://tumiz.github.io/scenario/Color.html)
```

### Comparing `py3d-0.0.96/setup.py` & `py3d-0.0.97/setup.py`

 * *Files identical despite different names*

