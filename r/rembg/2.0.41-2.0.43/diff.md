# Comparing `tmp/rembg-2.0.41.tar.gz` & `tmp/rembg-2.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.41.tar", last modified: Thu Jun  1 06:30:29 2023, max compression
+gzip compressed data, was "rembg-2.0.43.tar", last modified: Fri Jun  2 12:28:41 2023, max compression
```

## Comparing `rembg-2.0.41.tar` & `rembg-2.0.43.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:30:29.133605 rembg-2.0.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 06:30:13.000000 rembg-2.0.41/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 06:30:13.000000 rembg-2.0.41/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-01 06:30:29.133605 rembg-2.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-01 06:30:13.000000 rembg-2.0.41/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-01 06:30:13.000000 rembg-2.0.41/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:30:29.133605 rembg-2.0.41/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 06:30:29.133605 rembg-2.0.41/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:30:29.133605 rembg-2.0.41/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:30:29.133605 rembg-2.0.41/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-01 06:30:13.000000 rembg-2.0.41/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 06:30:29.133605 rembg-2.0.41/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 06:30:29.000000 rembg-2.0.41/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-01 06:30:13.000000 rembg-2.0.41/requirements-gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 06:30:13.000000 rembg-2.0.41/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 06:30:29.133605 rembg-2.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-01 06:30:13.000000 rembg-2.0.41/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-01 06:30:13.000000 rembg-2.0.41/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 12:28:28.000000 rembg-2.0.43/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 12:28:28.000000 rembg-2.0.43/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-02 12:28:41.536268 rembg-2.0.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12388 2023-06-02 12:28:28.000000 rembg-2.0.43/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-02 12:28:28.000000 rembg-2.0.43/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.536268 rembg-2.0.43/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-02 12:28:28.000000 rembg-2.0.43/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:28:41.532268 rembg-2.0.43/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 12:28:41.000000 rembg-2.0.43/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 12:28:28.000000 rembg-2.0.43/requirements-gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-02 12:28:28.000000 rembg-2.0.43/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 12:28:41.536268 rembg-2.0.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 12:28:28.000000 rembg-2.0.43/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-02 12:28:28.000000 rembg-2.0.43/versioneer.py
```

### Comparing `rembg-2.0.41/LICENSE.txt` & `rembg-2.0.43/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/PKG-INFO` & `rembg-2.0.43/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.41
+Version: 2.0.43
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.41/README.md` & `rembg-2.0.43/README.md`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/bg.py` & `rembg-2.0.43/rembg/bg.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from PIL.Image import Image as PILImage
 from pymatting.alpha.estimate_alpha_cf import estimate_alpha_cf
 from pymatting.foreground.estimate_foreground_ml import estimate_foreground_ml
 from pymatting.util.util import stack_images
 from scipy.ndimage import binary_erosion
 
 from .session_factory import new_session
+from .sessions import sessions_class
 from .sessions.base import BaseSession
 
 kernel = getStructuringElement(MORPH_ELLIPSE, (3, 3))
 
 
 class ReturnType(Enum):
     BYTES = 0
@@ -113,14 +114,19 @@
     return colored_image
 
 
 def fix_image_orientation(img: PILImage) -> PILImage:
     return ImageOps.exif_transpose(img)
 
 
+def download_models() -> None:
+    for session in sessions_class:
+        session.download_models()
+
+
 def remove(
     data: Union[bytes, PILImage, np.ndarray],
     alpha_matting: bool = False,
     alpha_matting_foreground_threshold: int = 240,
     alpha_matting_background_threshold: int = 10,
     alpha_matting_erode_size: int = 10,
     session: Optional[BaseSession] = None,
```

### Comparing `rembg-2.0.41/rembg/commands/b_command.py` & `rembg-2.0.43/rembg/commands/b_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/commands/i_command.py` & `rembg-2.0.43/rembg/commands/i_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/commands/p_command.py` & `rembg-2.0.43/rembg/commands/p_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/commands/s_command.py` & `rembg-2.0.43/rembg/commands/s_command.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/session_factory.py` & `rembg-2.0.43/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/__init__.py` & `rembg-2.0.43/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/base.py` & `rembg-2.0.43/rembg/sessions/base.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/dis_anime.py` & `rembg-2.0.43/rembg/sessions/dis_anime.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/dis_general_use.py` & `rembg-2.0.43/rembg/sessions/dis_general_use.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/sam.py` & `rembg-2.0.43/rembg/sessions/sam.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/silueta.py` & `rembg-2.0.43/rembg/sessions/silueta.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/u2net.py` & `rembg-2.0.43/rembg/sessions/u2net.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.43/rembg/sessions/u2net_cloth_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.43/rembg/sessions/u2net_human_seg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg/sessions/u2netp.py` & `rembg-2.0.43/rembg/sessions/u2netp.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/rembg.egg-info/PKG-INFO` & `rembg-2.0.43/rembg.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.41
+Version: 2.0.43
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `rembg-2.0.41/rembg.egg-info/SOURCES.txt` & `rembg-2.0.43/rembg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/setup.py` & `rembg-2.0.43/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.41/versioneer.py` & `rembg-2.0.43/versioneer.py`

 * *Files identical despite different names*

