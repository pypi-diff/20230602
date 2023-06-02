# Comparing `tmp/mazemastery-0.0.1.tar.gz` & `tmp/mazemastery-0.0.3.tar.gz`

## Comparing `mazemastery-0.0.1.tar` & `mazemastery-0.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/__init__.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/api.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/debug_menu.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/maze.py
--rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/renderer.py
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/state.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/styles.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_e.png
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_n.png
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne.png
--rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner.png
--rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw.png
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner.png
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_s.png
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_s_seam.png
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_se.png
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner.png
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner_e.png
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner_s.png
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_spec.png
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw.png
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner.png
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
--rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_spec.png
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/cloud_w.png
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/minotaur.png
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/warrior_down.png
--rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/warrior_left.png
--rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/warrior_right.png
--rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.0.1/src/mazemastery/sprites/warrior_up.png
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.1/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 mazemastery-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mazemastery-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/__init__.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/api.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/debug_menu.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/maze.py
+-rw-r--r--   0        0        0    35221 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/renderer.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/state.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/styles.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_e.png
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_n.png
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne.png
+-rw-r--r--   0        0        0     5459 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner.png
+-rw-r--r--   0        0        0     5120 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_e.png
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_n.png
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw.png
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner.png
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_e.png
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_n.png
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_w.png
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_s.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_s_seam.png
+-rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se.png
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner.png
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_e.png
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_s.png
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_spec.png
+-rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw.png
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner.png
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_s.png
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_w.png
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_spec.png
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/cloud_w.png
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/minotaur.png
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_down.png
+-rw-r--r--   0        0        0    11600 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_left.png
+-rw-r--r--   0        0        0    11852 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_right.png
+-rw-r--r--   0        0        0    10990 2020-02-02 00:00:00.000000 mazemastery-0.0.3/src/mazemastery/sprites/warrior_up.png
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 mazemastery-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 mazemastery-0.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mazemastery-0.0.3/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 mazemastery-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 mazemastery-0.0.3/PKG-INFO
```

### Comparing `mazemastery-0.0.1/src/mazemastery/api.py` & `mazemastery-0.0.3/src/mazemastery/api.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/debug_menu.py` & `mazemastery-0.0.3/src/mazemastery/debug_menu.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/maze.py` & `mazemastery-0.0.3/src/mazemastery/maze.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/renderer.py` & `mazemastery-0.0.3/src/mazemastery/renderer.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/state.py` & `mazemastery-0.0.3/src/mazemastery/state.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/styles.py` & `mazemastery-0.0.3/src/mazemastery/styles.py`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_e.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_n.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner_e.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_ne_inner_corner_n.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_ne_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_e.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_n.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_n.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_nw_inner_corner_w.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_nw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_s.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_s_seam.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_s_seam.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_se.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner_e.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_e.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_inner_corner_s.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_se_spec.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_se_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner_s.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_s.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_inner_corner_w.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_inner_corner_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_sw_spec.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_sw_spec.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/cloud_w.png` & `mazemastery-0.0.3/src/mazemastery/sprites/cloud_w.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/minotaur.png` & `mazemastery-0.0.3/src/mazemastery/sprites/minotaur.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/warrior_down.png` & `mazemastery-0.0.3/src/mazemastery/sprites/warrior_down.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/warrior_left.png` & `mazemastery-0.0.3/src/mazemastery/sprites/warrior_left.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/warrior_right.png` & `mazemastery-0.0.3/src/mazemastery/sprites/warrior_right.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/src/mazemastery/sprites/warrior_up.png` & `mazemastery-0.0.3/src/mazemastery/sprites/warrior_up.png`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/LICENSE` & `mazemastery-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mazemastery-0.0.1/pyproject.toml` & `mazemastery-0.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires= ["hatchling", "Pillow"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mazemastery"
-version = "0.0.1"
+version = "0.0.3"
 description = "MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators."
 authors = [
     {name="Raphaël Baur", email="rabaur@ethz.ch"},
     {name="Jens Hartmann", email="s4jehart@uni-trier.de"},
     {name="Jaqueline Staub", email="staub@uni-trier.de"},
     {name="Martin Löhnertz", email="loehnert@uni-trier.de"},
 ]
```

### Comparing `mazemastery-0.0.1/PKG-INFO` & `mazemastery-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mazemastery
-Version: 0.0.1
+Version: 0.0.3
 Summary: MazeMastery is a Python framework for teaching maze traversal to high school students. It helps students develop abstraction skills by providing a didactic tool. They can test their algorithms against randomized test cases of increasing complexity. The framework facilitates learning analysis and conceptual challenges. MazeMastery is an open-source project for scientists and educators.
 Project-URL: Homepage, https://github.com/rabaur/MazeMastery
 Author-email: Raphaël Baur <rabaur@ethz.ch>, Jens Hartmann <s4jehart@uni-trier.de>, Jaqueline Staub <staub@uni-trier.de>, Martin Löhnertz <loehnert@uni-trier.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

