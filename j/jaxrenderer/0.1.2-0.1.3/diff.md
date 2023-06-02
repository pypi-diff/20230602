# Comparing `tmp/jaxrenderer-0.1.2.tar.gz` & `tmp/jaxrenderer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.1.2.tar", max compression
+gzip compressed data, was "jaxrenderer-0.1.3.tar", max compression
```

## Comparing `jaxrenderer-0.1.2.tar` & `jaxrenderer-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11367 2023-06-01 15:40:54.196204 jaxrenderer-0.1.2/LICENSE
--rw-r--r--   0        0        0     1700 2023-06-01 15:40:54.196204 jaxrenderer-0.1.2/README.md
--rw-r--r--   0        0        0     3758 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/changelog.md
--rw-r--r--   0        0        0     1540 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/README.md
--rw-r--r--   0        0        0      459 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/__init__.py
--rw-r--r--   0        0        0    33682 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/geometry.py
--rw-r--r--   0        0        0    14815 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/model.py
--rw-r--r--   0        0        0    11913 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/pipeline.py
--rw-r--r--   0        0        0    13485 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/renderer.py
--rw-r--r--   0        0        0     9726 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/types.py
--rw-r--r--   0        0        0     3074 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-01 15:40:54.200204 jaxrenderer-0.1.2/renderer/value_checker.py
--rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 jaxrenderer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1866 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/README.md
+-rw-r--r--   0        0        0     4148 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/changelog.md
+-rw-r--r--   0        0        0     1540 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/README.md
+-rw-r--r--   0        0        0      459 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/__init__.py
+-rw-r--r--   0        0        0    33725 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/geometry.py
+-rw-r--r--   0        0        0    14815 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/model.py
+-rw-r--r--   0        0        0    11913 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/pipeline.py
+-rw-r--r--   0        0        0    13883 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/renderer.py
+-rw-r--r--   0        0        0     9726 2023-06-02 15:14:13.067642 jaxrenderer-0.1.3/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/types.py
+-rw-r--r--   0        0        0     3074 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-02 15:14:13.071642 jaxrenderer-0.1.3/renderer/value_checker.py
+-rw-r--r--   0        0        0     3320 1970-01-01 00:00:00.000000 jaxrenderer-0.1.3/PKG-INFO
```

### Comparing `jaxrenderer-0.1.2/LICENSE` & `jaxrenderer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/README.md` & `jaxrenderer-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 ## Key Difference from [erwincoumans/tinyrenderer](https://github.com/erwincoumans/tinyrenderer)
 
 - Native JAX implementation, supports `jit`, `vmap`, etc.
 - Lighting is computed in main camera's eye space; while in PyTinyrenderer it is computed in world space.
 - Texture specification is different: in PyTinyrenderer, the texture is specified in a flattened array, while in JAX Renderer, the texture is specified in a shape of (width, height, colour channels). A simple way to transform old specification to new specification is to use the convenient method `build_texture_from_PyTinyrenderer`.
 - Rendering pipeline is different. PyTinyrenderer renders one object at a time, and share zbuffer and framebuffer across one pass. This renderer first merges all objects into one big mesh in world space, then process all vertices together, then interpolates and rasterise and render. For fragment shading, this is done by sweeping each row in a for loop, and batch compute all pixels together. For computing a pixel, all fragments for that pixels are batch compute together, then mixed. This is more memory efficient and allows `vmap` batching as far as possible.
 - Shadowing within the same object / mesh is allowed. This is not possible in PyTinyrenderer, as it deliberately checks if the shadow comes from the same object; if so, it will not consider to draw a shadow there.
+- Quaternion (for specifying rotation/orientation) is in the form of `(w, x, y, z)` instead of `(x, y, z, w)` in PyTinyrenderer. This is for consistency with `BRAX`.
 - Fix bugs
   - Specular lighting was wrong, where it forgets to reverse the light direction vector.
 
 ## Roadmap
 
 - [ ] Correctly implement a proper clipping algorithm
 - [ ] Support double-sided objects
```

### Comparing `jaxrenderer-0.1.2/changelog.md` & `jaxrenderer-0.1.3/changelog.md`

 * *Files 11% similar despite different names*

```diff
@@ -29,7 +29,13 @@
 ## 0.1.2
 
 1. Change the ordering of quaternions (in `geometry.py`) to `(w, x, y, z)` instead of `(x, y, z, w)` to be consistent with the convention used in `pytinyrenderer` and `BRAX`. Reference: [brax/math.py](https://github.com/google/brax/blob/aebd8b8cb34430f6eaf6f914293f901e3c8d9a22/brax/math.py).
 2. Fix: remove unnecessary `@staticmethod` decorator in `merge_objects`.
 3. Changed the way that `Camera` is created in `Renderer.create_camera_from_parameters` to force convert parameters into `float` weak type.
 4. Force convert `LightParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
 5. Downgrade minimum Python version to `3.9`, `numpy` version to `1.22.0`, `jax` and `jaxlib` version to `0.4.4`.
+
+## 0.1.3
+
+1. Correctly force convert `LightParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
+2. Fix `geometry.py::transform_matrix_from_rotation`. Also, change the order of quaternion to `(w, x, y, z)` instead of `(x, y, z, w)` for consistency.
+3. Force convert `ShadowParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
```

### Comparing `jaxrenderer-0.1.2/pyproject.toml` & `jaxrenderer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.1.2"
+version = "0.1.3"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
```

### Comparing `jaxrenderer-0.1.2/renderer/README.md` & `jaxrenderer-0.1.3/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/geometry.py` & `jaxrenderer-0.1.3/renderer/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -908,28 +908,26 @@
 
 
 @jaxtyped
 @jax.jit
 def transform_matrix_from_rotation(rotation: Vec4f) -> Float[Array, "3 3"]:
     """Generate a transform matrix from a quaternion rotation.
 
-    Supports non-unit rotation.
+    Quaternion is specified in (w, x, y, z) order. Supports non-unit rotation.
 
     References:
           - [Quaternions and spatial rotation#Quaternion-derived rotation matrix](https://en.wikipedia.org/wiki/Quaternions_and_spatial_rotation#Quaternion-derived_rotation_matrix)
           - [TinySceneRenderer::set_object_orientation](https://github.com/erwincoumans/tinyrenderer/blob/89e8adafb35ecf5134e7b17b71b0f825939dc6d9/tinyrenderer.cpp#LL997C20-L997C20)
     """
     d = rotation @ rotation
     s = 2.0 / d  # here s is $2\times s$ in Wikipedia.
 
-    rs: Vec3f = rotation[:3] * s
-    ((wx, wy, wz), (xx, xy, xz), (yy, yz, zz)) = jnp.outer(
-        rotation[jnp.array((3, 0, 1))],
-        rs,
-    )
+    rs: Vec3f = rotation[1:] * s  # x y z
+    ((wx, wy, wz), (xx, xy, xz), (_, yy, yz)) = jnp.outer(rotation[:3], rs)
+    zz = rotation[3] * rs[2]
 
     mat: Float[Array, "3 3"] = jnp.array((
         (1. - (yy + zz), xy - wz, xz + wy),
         (xy + wz, 1. - (xx + zz), yz - wx),
         (xz - wy, yz + wx, 1. - (xx + yy)),
     ))
     assert isinstance(mat, Float[Array, "3 3"])
```

### Comparing `jaxrenderer-0.1.2/renderer/model.py` & `jaxrenderer-0.1.3/renderer/model.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/pipeline.py` & `jaxrenderer-0.1.3/renderer/pipeline.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/renderer.py` & `jaxrenderer-0.1.3/renderer/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,27 +326,40 @@
         if isinstance(camera, CameraParameters):
             _camera = cls.create_camera_from_parameters(camera)
         else:
             _camera = camera
 
         assert isinstance(_camera, Camera), f"{_camera}"
 
-        light = tree_map(jnp.asarray, light)
+        light = tree_map(
+            jnp.asarray,
+            light,
+            # only flatten one layer
+            is_leaf=lambda x: not isinstance(x, LightParameters),
+        )
         assert isinstance(light, LightParameters), f"{light}"
 
         buffers: Buffers = cls.create_buffers(
             width=width,
             height=height,
             colour_default=colour_default,
             zbuffer_default=zbuffer_default,
         )
 
         model: MergedModel = merge_objects(objects)
         assert isinstance(model, MergedModel), f"{model}"
 
+        if shadow_param is not None:
+            shadow_param = tree_map(
+                jnp.asarray,
+                shadow_param,
+                # only flatten one layer
+                is_leaf=lambda x: not isinstance(x, ShadowParameters),
+            )
+
         canvas: Canvas
         _, (canvas, ) = cls.render(
             model=model,
             light=light,
             camera=_camera,
             buffers=buffers,
             shadow_param=shadow_param,
```

### Comparing `jaxrenderer-0.1.2/renderer/scene.py` & `jaxrenderer-0.1.3/renderer/scene.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shader.py` & `jaxrenderer-0.1.3/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/README.md` & `jaxrenderer-0.1.3/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/depth.py` & `jaxrenderer-0.1.3/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/gouraud.py` & `jaxrenderer-0.1.3/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.1.3/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/phong.py` & `jaxrenderer-0.1.3/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.1.3/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.1.3/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.1.3/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shadow.py` & `jaxrenderer-0.1.3/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shapes/capsule.py` & `jaxrenderer-0.1.3/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/shapes/cube.py` & `jaxrenderer-0.1.3/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/types.py` & `jaxrenderer-0.1.3/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/utils.py` & `jaxrenderer-0.1.3/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/renderer/value_checker.py` & `jaxrenderer-0.1.3/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.1.2/PKG-INFO` & `jaxrenderer-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -37,14 +37,15 @@
 ## Key Difference from [erwincoumans/tinyrenderer](https://github.com/erwincoumans/tinyrenderer)
 
 - Native JAX implementation, supports `jit`, `vmap`, etc.
 - Lighting is computed in main camera's eye space; while in PyTinyrenderer it is computed in world space.
 - Texture specification is different: in PyTinyrenderer, the texture is specified in a flattened array, while in JAX Renderer, the texture is specified in a shape of (width, height, colour channels). A simple way to transform old specification to new specification is to use the convenient method `build_texture_from_PyTinyrenderer`.
 - Rendering pipeline is different. PyTinyrenderer renders one object at a time, and share zbuffer and framebuffer across one pass. This renderer first merges all objects into one big mesh in world space, then process all vertices together, then interpolates and rasterise and render. For fragment shading, this is done by sweeping each row in a for loop, and batch compute all pixels together. For computing a pixel, all fragments for that pixels are batch compute together, then mixed. This is more memory efficient and allows `vmap` batching as far as possible.
 - Shadowing within the same object / mesh is allowed. This is not possible in PyTinyrenderer, as it deliberately checks if the shadow comes from the same object; if so, it will not consider to draw a shadow there.
+- Quaternion (for specifying rotation/orientation) is in the form of `(w, x, y, z)` instead of `(x, y, z, w)` in PyTinyrenderer. This is for consistency with `BRAX`.
 - Fix bugs
   - Specular lighting was wrong, where it forgets to reverse the light direction vector.
 
 ## Roadmap
 
 - [ ] Correctly implement a proper clipping algorithm
 - [ ] Support double-sided objects
```

