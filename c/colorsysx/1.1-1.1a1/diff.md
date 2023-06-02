# Comparing `tmp/colorsysx-1.1.tar.gz` & `tmp/colorsysx-1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorsysx-1.1.tar", last modified: Fri Jun  2 00:00:14 2023, max compression
+gzip compressed data, was "colorsysx-1.1a1.tar", last modified: Mon May 22 17:10:44 2023, max compression
```

## Comparing `colorsysx-1.1.tar` & `colorsysx-1.1a1.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0      506 2023-05-22 16:10:46.352674 colorsysx-1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0       53 2023-06-01 23:54:42.899378 colorsysx-1.1/.gitignore
--rw-r--r--   0        0        0     1082 2023-05-22 16:10:46.352674 colorsysx-1.1/LICENSE
--rw-r--r--   0        0        0     3186 2023-05-22 18:34:59.877058 colorsysx-1.1/README.md
--rw-r--r--   0        0        0     1471 2023-06-01 23:59:16.698557 colorsysx-1.1/colorsysx/__init__.py
--rw-r--r--   0        0        0     6421 2023-05-22 16:59:01.212529 colorsysx-1.1/colorsysx/_glhs.py
--rw-r--r--   0        0        0     4717 2023-05-22 16:35:31.724434 colorsysx-1.1/colorsysx/_hcy.py
--rw-r--r--   0        0        0      379 2023-05-22 16:12:08.181596 colorsysx-1.1/colorsysx/_helpers.py
--rw-r--r--   0        0        0     1246 2023-05-22 16:12:08.185596 colorsysx-1.1/colorsysx/_swizzle.py
--rw-r--r--   0        0        0     2051 2023-06-01 23:32:15.083070 colorsysx-1.1/colorsysx/_yiq.py
--rw-r--r--   0        0        0     3506 2023-06-01 23:30:38.474272 colorsysx-1.1/colorsysx/_yuv.py
--rw-r--r--   0        0        0     2929 2023-06-01 23:44:47.349273 colorsysx-1.1/colorsysx/weights.py
--rw-r--r--   0        0        0      819 2023-05-22 16:10:46.352674 colorsysx-1.1/pyproject.toml
--rw-r--r--   0        0        0     1261 2023-05-22 16:10:46.416675 colorsysx-1.1/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-22 16:12:08.185596 colorsysx-1.1/tests/__init__.py
--rw-r--r--   0        0        0      319 2023-05-22 16:12:08.189596 colorsysx-1.1/tests/context.py
--rw-r--r--   0        0        0     1438 2023-05-22 16:57:48.499880 colorsysx-1.1/tests/test_deprecations.py
--rw-r--r--   0        0        0     5806 2023-05-22 16:36:45.793029 colorsysx-1.1/tests/test_glhs.py
--rw-r--r--   0        0        0     2734 2023-05-22 16:24:40.122637 colorsysx-1.1/tests/test_hcy.py
--rw-r--r--   0        0        0      584 2023-05-22 16:31:57.978708 colorsysx-1.1/tests/test_swizzle.py
--rw-r--r--   0        0        0      815 2023-05-22 16:12:08.185596 colorsysx-1.1/tests/test_weights.py
--rw-r--r--   0        0        0     1930 2023-06-01 23:47:04.918407 colorsysx-1.1/tests/test_yiq.py
--rw-r--r--   0        0        0     2578 2023-06-01 23:15:51.122918 colorsysx-1.1/tests/test_yuv.py
--rw-r--r--   0        0        0     1030 2023-05-22 16:10:46.372674 colorsysx-1.1/tox.ini
--rw-r--r--   0        0        0     3973 1970-01-01 00:00:00.000000 colorsysx-1.1/PKG-INFO
+-rw-r--r--   0        0        0      506 2023-05-22 16:10:46.352674 colorsysx-1.1a1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0       53 2023-05-22 16:10:46.352674 colorsysx-1.1a1/.gitignore
+-rw-r--r--   0        0        0     1082 2023-05-22 16:10:46.352674 colorsysx-1.1a1/LICENSE
+-rw-r--r--   0        0        0     3186 2023-05-22 16:10:46.416675 colorsysx-1.1a1/README.md
+-rw-r--r--   0        0        0     1448 2023-05-22 16:40:25.210787 colorsysx-1.1a1/colorsysx/__init__.py
+-rw-r--r--   0        0        0     6421 2023-05-22 16:59:01.212529 colorsysx-1.1a1/colorsysx/_glhs.py
+-rw-r--r--   0        0        0     4717 2023-05-22 16:35:31.724434 colorsysx-1.1a1/colorsysx/_hcy.py
+-rw-r--r--   0        0        0      379 2023-05-22 16:12:08.181596 colorsysx-1.1a1/colorsysx/_helpers.py
+-rw-r--r--   0        0        0     1246 2023-05-22 16:12:08.185596 colorsysx-1.1a1/colorsysx/_swizzle.py
+-rw-r--r--   0        0        0     3248 2023-05-22 16:59:34.920828 colorsysx-1.1a1/colorsysx/_yuv.py
+-rw-r--r--   0        0        0     2929 2023-05-22 16:46:12.301566 colorsysx-1.1a1/colorsysx/weights.py
+-rw-r--r--   0        0        0      819 2023-05-22 16:10:46.352674 colorsysx-1.1a1/pyproject.toml
+-rw-r--r--   0        0        0     1261 2023-05-22 16:10:46.416675 colorsysx-1.1a1/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-22 16:12:08.185596 colorsysx-1.1a1/tests/__init__.py
+-rw-r--r--   0        0        0      319 2023-05-22 16:12:08.189596 colorsysx-1.1a1/tests/context.py
+-rw-r--r--   0        0        0     1438 2023-05-22 16:57:48.499880 colorsysx-1.1a1/tests/test_deprecations.py
+-rw-r--r--   0        0        0     5806 2023-05-22 16:36:45.793029 colorsysx-1.1a1/tests/test_glhs.py
+-rw-r--r--   0        0        0     2734 2023-05-22 16:24:40.122637 colorsysx-1.1a1/tests/test_hcy.py
+-rw-r--r--   0        0        0      584 2023-05-22 16:31:57.978708 colorsysx-1.1a1/tests/test_swizzle.py
+-rw-r--r--   0        0        0      815 2023-05-22 16:12:08.185596 colorsysx-1.1a1/tests/test_weights.py
+-rw-r--r--   0        0        0     1724 2023-05-22 16:28:20.952886 colorsysx-1.1a1/tests/test_yuv.py
+-rw-r--r--   0        0        0     1030 2023-05-22 16:10:46.372674 colorsysx-1.1a1/tox.ini
+-rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 colorsysx-1.1a1/PKG-INFO
```

### Comparing `colorsysx-1.1/LICENSE` & `colorsysx-1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/README.md` & `colorsysx-1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/colorsysx/__init__.py` & `colorsysx-1.1a1/colorsysx/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 See the corresponding module help texts for further details about each
 model. All of the colour spaces added by this package can be
 parameterized to tune them for different tasks. See the
 colorsysx.weights module for details.
 
 """
 
-__version__ = "1.1"
+__version__ = "1.1a1"
 
 # Imports::
 
 # Import just the functions,
 # people wanting weights can import .weights submodule.
 from ._yuv import rgb_to_yuv, yuv_to_rgb  # noqa: F401
 from ._hcy import rgb_to_hcy, hcy_to_rgb  # noqa: F401
 from ._glhs import rgb_to_glhs, glhs_to_rgb  # noqa: F401
-from ._yiq import rgb_to_yiq, yiq_to_rgb  # noqa: F401
 
 # Also make the stock colorsys funcs available.
 from colorsys import \
     rgb_to_hls, hls_to_rgb, \
-    rgb_to_hsv, hsv_to_rgb  # noqa: F401
+    rgb_to_hsv, hsv_to_rgb, \
+    rgb_to_yiq, yiq_to_rgb  # noqa: F401
 
 # Exports::
 
 __all__ = [
     "rgb_to_yuv", "yuv_to_rgb",
     "rgb_to_hcy", "hcy_to_rgb",
     "rgb_to_glhs", "glhs_to_rgb",
```

### Comparing `colorsysx-1.1/colorsysx/_glhs.py` & `colorsysx-1.1a1/colorsysx/_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/colorsysx/_hcy.py` & `colorsysx-1.1a1/colorsysx/_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/colorsysx/_swizzle.py` & `colorsysx-1.1a1/colorsysx/_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/colorsysx/_yuv.py` & `colorsysx-1.1a1/colorsysx/_yuv.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 * https://en.wikipedia.org/wiki/YCbCr#R'G'B'_to_Y'PbPr
 
 """
 
 # Imports::
 
 from . import weights
-from . import _helpers as helpers
+from ._helpers import matmul
+from ._helpers import clamp
 
 
 # Default values::
 
 DEFAULT_WEIGHTS = weights.RGBWeights.REC709
 
 
@@ -61,42 +62,35 @@
         weights_rgb = DEFAULT_WEIGHTS
     kr, kg, kb = weights_rgb
     color_matrix = [
         [kr,               kg,                kb],
         [-0.5 * kr/(1-kb), -0.5 * kg/(1-kb),  0.5],
         [0.5,              -0.5 * kg/(1-kr), -0.5 * kb/(1-kr)],
     ]
-    [[y], [u], [v]] = helpers.matmul(color_matrix, [[r], [g], [b]])
+    [[y], [u], [v]] = matmul(color_matrix, [[r], [g], [b]])
     return (y, u, v)
 
 
-def yuv_to_rgb(y, u, v, weights_rgb=DEFAULT_WEIGHTS, w_rgb=None, clamp=True):
+def yuv_to_rgb(y, u, v, weights_rgb=DEFAULT_WEIGHTS, w_rgb=None):
     """Convert from YUV to RGB.
 
-    The "y" parameter is a float in the interval [0, 1].
-    The range for "u" is approximately [-0.115, 0.115].
-    The range for "v" is approximately [-0.5, 0.5].
-    "weights" has the same meaning and default value as it
+    The "y", "u", and "v" parameters are floats between 0 and 1
+    inclusive.  "weights" has the same meaning and default value as it
     does in rgb_to_yuv().
 
     "w_rgb" is a deprecated override for "weights_rgb". It will be
     removed in colorsysx 2.0.
 
-    By default, the returned (R, G, B) components are constrained to lie
-    within the interval [0, 1]. Set "clamp" to False if you want to
-    perform your own checking.
+    Returns a tuple (r, g, b), clamped to between 0 and 1 inclusive.
 
     """
     weights_rgb = w_rgb or weights_rgb  # FIXME: remove in 2.0
     if weights_rgb is None:
         weights_rgb = DEFAULT_WEIGHTS
     kr, kg, kb = weights_rgb
     inverse_color_matrix = [
         [1., 0.,                 2 - 2*kr],
         [1., -(kb/kg)*(2-2*kb), -(kr/kg)*(2-2*kr)],
         [1., 2-2*kb,             0.],
     ]
-    [[r], [g], [b]] = helpers.matmul(inverse_color_matrix, [[y], [u], [v]])
-    if clamp:
-        return tuple(helpers.clamp(c, 0, 1) for c in (r, g, b))
-    else:
-        return (r, g, b)
+    [[r], [g], [b]] = matmul(inverse_color_matrix, [[y], [u], [v]])
+    return tuple(clamp(c, 0, 1) for c in (r, g, b))
```

### Comparing `colorsysx-1.1/colorsysx/weights.py` & `colorsysx-1.1a1/colorsysx/weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/pyproject.toml` & `colorsysx-1.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/requirements.txt` & `colorsysx-1.1a1/requirements.txt`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tests/test_deprecations.py` & `colorsysx-1.1a1/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tests/test_glhs.py` & `colorsysx-1.1a1/tests/test_glhs.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tests/test_hcy.py` & `colorsysx-1.1a1/tests/test_hcy.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tests/test_swizzle.py` & `colorsysx-1.1a1/tests/test_swizzle.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tests/test_weights.py` & `colorsysx-1.1a1/tests/test_weights.py`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/tox.ini` & `colorsysx-1.1a1/tox.ini`

 * *Files identical despite different names*

### Comparing `colorsysx-1.1/PKG-INFO` & `colorsysx-1.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorsysx
-Version: 1.1
+Version: 1.1a1
 Summary: Extra, human-relevant, colour spaces derived from RGB.
 Author-email: Andrew Chadwick <a.t.chadwick@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Graphics :: Presentation
```

