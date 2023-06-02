# Comparing `tmp/usa-net-0.0.4.tar.gz` & `tmp/usa-net-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usa-net-0.0.4.tar", last modified: Tue May  2 21:46:42 2023, max compression
+gzip compressed data, was "usa-net-0.0.5.tar", last modified: Fri Jun  2 20:52:55 2023, max compression
```

## Comparing `usa-net-0.0.4.tar` & `usa-net-0.0.5.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 21:46:28.000000 usa-net-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 21:46:42.480197 usa-net-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-02 21:46:28.000000 usa-net-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-02 21:46:28.000000 usa-net-0.0.4/notebooks/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-02 21:46:28.000000 usa-net-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements-ipynb.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 21:46:28.000000 usa-net-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-02 21:46:42.480197 usa-net-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-02 21:46:28.000000 usa-net-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-02 21:46:28.000000 usa-net-0.0.4/tests/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/usa/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.472197 usa-net-0.0.4/usa/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/path_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/semantics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/trajectories.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/evaluation/visualize_semantics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37202 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/point2emb.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/models/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/planners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/clip_sdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/planners/occupancy_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/scripts/adhoc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/distribution_estimates.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/adhoc/show_point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.476197 usa-net-0.0.4/usa/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12748 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/clip_sdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/usa/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/home_robot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/posed_rgbd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/pybullet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/r3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/replica_cad.py
--rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13644 2023-05-02 21:46:28.000000 usa-net-0.0.4/usa/tasks/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:46:42.480197 usa-net-0.0.4/usa_net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 21:46:42.000000 usa-net-0.0.4/usa_net.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.252947 usa-net-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-02 20:52:42.000000 usa-net-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-02 20:52:55.256947 usa-net-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 20:52:42.000000 usa-net-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.244947 usa-net-0.0.5/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-02 20:52:42.000000 usa-net-0.0.5/notebooks/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-02 20:52:42.000000 usa-net-0.0.5/notebooks/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-02 20:52:42.000000 usa-net-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 20:52:42.000000 usa-net-0.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 20:52:42.000000 usa-net-0.0.5/requirements-ipynb.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-02 20:52:42.000000 usa-net-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 20:52:55.256947 usa-net-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-02 20:52:42.000000 usa-net-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.244947 usa-net-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 20:52:42.000000 usa-net-0.0.5/tests/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.244947 usa-net-0.0.5/usa/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.244947 usa-net-0.0.5/usa/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/path_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/semantics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/evaluation/visualize_semantics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.248947 usa-net-0.0.5/usa/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37200 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/models/point2emb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/models/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.248947 usa-net-0.0.5/usa/planners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/planners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/planners/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/planners/clip_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/planners/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/planners/occupancy_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.248947 usa-net-0.0.5/usa/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.248947 usa-net-0.0.5/usa/scripts/adhoc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/adhoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/adhoc/distribution_estimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/adhoc/get_pybullet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/adhoc/show_point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.252947 usa-net-0.0.5/usa/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/clip_sdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.252947 usa-net-0.0.5/usa/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/home_robot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/posed_rgbd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/pybullet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/r3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/replica_cad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-06-02 20:52:42.000000 usa-net-0.0.5/usa/tasks/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:52:55.252947 usa-net-0.0.5/usa_net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 20:52:55.000000 usa-net-0.0.5/usa_net.egg-info/top_level.txt
```

### Comparing `usa-net-0.0.4/PKG-INFO` & `usa-net-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usa-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: USA net project
 Home-page: https://github.com/codekansas/usa-net
 Author: Benjamin Bolte
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ipynb
@@ -56,7 +56,16 @@
 ### Development
 
 Add pre-commit hooks to clean Jupyter notebooks:
 
 ```bash
 pre-commit install
 ```
+
+### Notes
+
+- If you are having trouble installing Open3D on Mac, install Pybind through Conda instead:
+
+```bash
+pip uninstall open3d
+conda install open3d
+```
```

### Comparing `usa-net-0.0.4/README.md` & `usa-net-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -45,7 +45,16 @@
 ### Development
 
 Add pre-commit hooks to clean Jupyter notebooks:
 
 ```bash
 pre-commit install
 ```
+
+### Notes
+
+- If you are having trouble installing Open3D on Mac, install Pybind through Conda instead:
+
+```bash
+pip uninstall open3d
+conda install open3d
+```
```

### Comparing `usa-net-0.0.4/notebooks/test_planner.py` & `usa-net-0.0.5/notebooks/test_planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 model, task = ml.load_model_and_task(cfg_path)
 assert isinstance(model, Point2EmbModel)
 assert isinstance(task, ClipSdfTask)
 
 
 grid_planner = AStarPlanner(
-    dataset=task._dataset,
+    dataset=task._dataset(),
     model=model.double(),
     task=task.double(),
     device=task._device,
     # The heuristic to use for AStar
     heuristic="euclidean",
     # The grid resolution
     resolution=0.1,
     # Where to store cache artifacts
     cache_dir=None,
 ).double()
 
 gradient_planner = GradientPlanner(
-    dataset=task._dataset,
+    dataset=task._dataset(),
     model=model.double(),
     task=task.double(),
     device=task._device,
     # The learning rate for the optimizer for the waypoints
     lr=1e-2,
     # The weight for the total path distance loss term
     dist_loss_weight=1.0,
```

### Comparing `usa-net-0.0.4/pyproject.toml` & `usa-net-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -34,28 +34,23 @@
 
 # For TorchScript stuff.
 disable_error_code = ["attr-defined"]
 
 [[tool.mypy.overrides]]
 
 module = [
-    "_pytest.*",
     "cv2.*",
-    "faiss.*",
     "ffmpeg.*",
     "liblzfse.*",
     "matplotlib.*",
     "open3d.*",
-    "pandas.*",
-    "PIL.*",
-    "pytest.*",
+    "pybullet.*",
     "quaternion.*",
     "seaborn.*",
     "torchvision.*",
-    "tqdm.*",
 ]
 
 ignore_missing_imports = true
 
 [tool.isort]
 
 profile = "black"
```

### Comparing `usa-net-0.0.4/setup.py` & `usa-net-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/evaluation/path_length.py` & `usa-net-0.0.5/usa/evaluation/path_length.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/evaluation/semantics.py` & `usa-net-0.0.5/usa/evaluation/semantics.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/evaluation/trajectories.py` & `usa-net-0.0.5/usa/evaluation/trajectories.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     task: ClipSdfTask,
     planner_key: PlannerType,
     floor_ceil_heights: tuple[float, float],
     device: Type[ml.BaseDevice],
     dataset: Dataset[PosedRGBDItem] | None = None,
 ) -> Planner:
     if dataset is None:
-        dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
+        dataset = task.get_dataset("train")
     floor_height, ceil_height = floor_ceil_heights
 
     if planner_key == "a_star":
         return AStarClipSDFPlanner(
             dataset,
             model,
             task,
@@ -242,15 +242,15 @@
 
     # Loads the model from the model root.
     ckpt_path, config_path = Path(args.ckpt_path), Path(args.config_path)
     model, task = load_clip_sdf_model_from_ckpt_and_config(ckpt_path, config_path, device)
 
     # Gets the dataset and planner from the given model.
     floor_ceil_heights = float(args.floor_height), float(args.ceil_height)
-    dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
+    dataset = task.get_dataset("train")
     planner = get_planner(model, task, cast(PlannerType, args.planner), floor_ceil_heights, device, dataset)
 
     # Gets the starting XY coordinates, the goal locations and the artifacts directory from arguments.
     start_xy = float(args.xy[0]), float(args.xy[1])
     goals = cast(list[str], args.goals.split(";"))
     artifacts_dir = Path(args.artifacts_dir) if args.artifacts_dir else None
```

### Comparing `usa-net-0.0.4/usa/evaluation/utils.py` & `usa-net-0.0.5/usa/evaluation/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Type, cast
+from typing import Type
 
 import matplotlib.pyplot as plt
 import ml.api as ml
 import numpy as np
 import torch
 from omegaconf import OmegaConf
 from torch.utils.data.dataset import Dataset
@@ -139,15 +139,15 @@
         raise EnvironmentError(f"Checkpoint directory not found: {clip_sdf_exp_path}")
 
     # Gets the device (GPU, CPU, Metal...)
     os.environ["USE_FP64"] = "1"
     device = ml.AutoDevice.detect_device()
 
     model, task = load_clip_sdf_model(clip_sdf_exp_path, device)
-    dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
+    dataset = task.get_dataset("train")
 
     # Cache to the experiment directory.
     base_cache_dir = clip_sdf_exp_path / "eval_cache" / "semantics" / name
 
     planners: dict[str, Planner] = {
         "a_star_10_cm_clip_sdf": AStarClipSDFPlanner(
             dataset,
```

### Comparing `usa-net-0.0.4/usa/evaluation/visualize_semantics.py` & `usa-net-0.0.5/usa/evaluation/visualize_semantics.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     # Loads the model from the model root.
     ckpt_path, config_path = Path(args.ckpt_path), Path(args.config_path)
     model, task = load_clip_sdf_model_from_ckpt_and_config(ckpt_path, config_path, device)
 
     # Gets the dataset.
     floor_ceil_heights = float(args.floor_height), float(args.ceil_height)
-    dataset = cast(Dataset[PosedRGBDItem], task.get_dataset("train"))
+    dataset = task.get_dataset("train")
 
     # Gets the resolution, goal locations and artifacts directory from arguments.
     resolution = float(args.resolution)
     goals = cast(list[str], args.goals.split(";"))
     artifacts_dir = Path(args.artifacts_dir)
 
     visualize_semantics(model, task, device, floor_ceil_heights, dataset, goals, artifacts_dir, resolution)
```

### Comparing `usa-net-0.0.4/usa/models/clip.py` & `usa-net-0.0.5/usa/models/clip.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any, Literal, cast, get_args, overload
 
 import ftfy
 import ml.api as ml
 import numpy as np
+import PIL.Image
 import torch
 import torch.nn.functional as F
 import torchvision
-from PIL import Image as PILImage
 from pkg_resources import packaging
 from torch import Tensor, nn
 from torchvision.datasets.utils import download_url
 
 URL_PREFIX = "https://openaipublic.azureedge.net/clip/models"
 
 PretrainedModel = Literal[
@@ -57,15 +57,15 @@
     "ViT_L_14": f"{URL_PREFIX}/b8cca3fd41ae0c99ba7e8951adf17d267cdb84cd88be6f7c2e0eca1737a03836/ViT-L-14.pt",
     "ViT_L_14_336px": f"{URL_PREFIX}/3035c92b350959924f9f00213499208652fc7ea050643e8b385c2dac08641f02/ViT-L-14-336px.pt",  # noqa, pylint: disable=line-too-long
 }
 
 CLIP_VOCABULARY = "https://github.com/openai/CLIP/raw/main/clip/bpe_simple_vocab_16e6.txt.gz"
 
 
-def _convert_image_to_rgb(image: PILImage) -> PILImage:
+def _convert_image_to_rgb(image: PIL.Image.Image) -> PIL.Image.Image:
     return image.convert("RGB")
 
 
 def preprocess(n_px: int) -> torchvision.transforms.Compose:
     mean, std = (0.48145466, 0.4578275, 0.40821073), (0.26862954, 0.26130258, 0.27577711)
     return torchvision.transforms.Compose(
         [
@@ -979,15 +979,15 @@
 
     # Gets an image of a peach from Wikipedia.
     peach_url = "https://upload.wikimedia.org/wikipedia/commons/9/9e/Autumn_Red_peaches.jpg"
     url_path = Path("/tmp/peach.jpg")
     if not url_path.exists():
         download_url(peach_url, "/tmp", filename="peach.jpg")
 
-    peach_img = PILImage.open(url_path)
+    peach_img = PIL.Image.open(url_path)
     pos_desc = "A picture of an Autumn Red peach"
     neg_desc = "An Instagram photo of a cute puppy"
 
     # Loads the JIT'd model and the regular model.
     auto_device = ml.AutoDevice.detect_device()
     device, dtype = auto_device.get_device(), torch.half
     jit_model = cast(CLIP, torch.jit.load(get_pretrained_path(model_key), map_location="cpu"))
```

### Comparing `usa-net-0.0.4/usa/models/point2emb.py` & `usa-net-0.0.5/usa/models/point2emb.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/planners/base.py` & `usa-net-0.0.5/usa/planners/base.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/planners/clip_sdf.py` & `usa-net-0.0.5/usa/planners/clip_sdf.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/planners/common.py` & `usa-net-0.0.5/usa/planners/common.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/planners/occupancy_map.py` & `usa-net-0.0.5/usa/planners/occupancy_map.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/scripts/adhoc/distribution_estimates.py` & `usa-net-0.0.5/usa/scripts/adhoc/distribution_estimates.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/clip_sdf.py` & `usa-net-0.0.5/usa/tasks/clip_sdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import itertools
 import logging
 from dataclasses import dataclass
-from typing import Any, Callable
+from typing import Any, Callable, Sized, cast
 
 import ml.api as ml
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 import tqdm
 from omegaconf import MISSING
@@ -141,20 +141,16 @@
         return super()._apply(fn)
 
     def apply(self, fn: Callable[["torch.nn.Module"], None]) -> Any:
         self.clip.visual.apply(fn)
         self.clip.linguistic.apply(fn)
         return super().apply(fn)
 
-    def _get_posed_rgb_dataset(self) -> Dataset[PosedRGBDItem]:
-        return get_posed_rgbd_dataset(self.config.dataset, path=self.config.dataset_path)
-
-    @functools.cached_property
     def _dataset(self) -> Dataset[PosedRGBDItem]:
-        return self._get_posed_rgb_dataset()
+        return get_posed_rgbd_dataset(self.config.dataset, path=self.config.dataset_path)
 
     @functools.lru_cache
     def text_clip_embs(self, device: torch.device) -> Tensor:
         with torch.no_grad():
             tokens = self.clip.tokenizer.tokenize(self.config.queries).to(device)
             embs = self.clip.linguistic(tokens)
             return embs
@@ -294,16 +290,16 @@
             clip_min, clip_max = aminmax(clip_preds)
             clip_preds = (clip_preds - clip_min) / (clip_max - clip_min + 1e-3)
 
             # CLIP image has shape (num_embs, width, height)
             # SDF image has shape (width, height)
             return clip_preds.permute(2, 0, 1), sdf_preds
 
-    def get_dataset(self, phase: ml.Phase) -> Dataset:
-        return self._dataset
+    def get_dataset(self, phase: ml.Phase) -> Dataset[PosedRGBDItem]:
+        return self._dataset()
 
 
 def test_sdf_dataset(max_samples: int = 3) -> None:
     """Provides a helper script for testing the SDF dataset.
 
     Usage:
         python -m ml.tasks.sdf
@@ -314,14 +310,14 @@
 
     ml.configure_logging(use_tqdm=True)
 
     config = ClipSdfTaskConfig(dataset="replica_apt_2_mnp")
     task = ClipSdfTask(config)
     ds = task.get_dataset("train")
 
-    for i, item in enumerate(itertools.islice(tqdm.tqdm(ds, total=max_samples, desc="Samples"), max_samples)):
+    for i in itertools.islice(tqdm.trange(len(cast(Sized, ds)), total=max_samples, desc="Samples"), max_samples):
         logger.info("Checking sample %d", i)
-        item.check()
+        ds[i].check()
 
 
 if __name__ == "__main__":
     test_sdf_dataset()
```

### Comparing `usa-net-0.0.4/usa/tasks/datasets/home_robot.py` & `usa-net-0.0.5/usa/tasks/datasets/home_robot.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/posed_rgbd.py` & `usa-net-0.0.5/usa/tasks/datasets/posed_rgbd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Sized, cast
 
 import ml.api as ml
 import more_itertools
 import numpy as np
 import torch
 import tqdm
 from torch import Tensor
@@ -197,16 +197,16 @@
     # pylint: disable=unsupported-assignment-operation,unsubscriptable-object
     cache_loc = None if cache_dir is None else cache_dir / "poses.npy"
 
     if cache_loc is not None and cache_loc.is_file():
         return np.load(cache_loc)
 
     all_poses: list[np.ndarray] = []
-    for item in tqdm.tqdm(ds, desc="Poses"):
-        all_poses.append(item.pose.cpu().numpy())
+    for i in tqdm.trange(len(cast(Sized, ds)), desc="Poses"):
+        all_poses.append(ds[i].pose.cpu().numpy())
 
     poses = np.stack(all_poses)
     if cache_loc is not None:
         cache_loc.parent.mkdir(exist_ok=True, parents=True)
         np.save(cache_loc, poses)
 
     return poses
@@ -217,16 +217,16 @@
     cache_loc = None if cache_dir is None else cache_dir / "pose_bounds.npy"
 
     bounds: np.ndarray | None = None
 
     if cache_loc is not None and cache_loc.is_file():
         bounds = np.load(cache_loc)
     else:
-        for item in tqdm.tqdm(ds, desc="Pose bounds"):
-            xyz = item.pose[..., :3, 3].cpu().numpy()
+        for i in tqdm.trange(len(cast(Sized, ds)), desc="Pose bounds"):
+            xyz = ds[i].pose[..., :3, 3].cpu().numpy()
             if bounds is None:
                 bounds = np.stack((xyz, xyz), axis=1)
             else:
                 bounds[:, 0] = np.minimum(bounds[:, 0], xyz)
                 bounds[:, 1] = np.maximum(bounds[:, 1], xyz)
         assert bounds is not None, "No samples found"
         if cache_loc is not None:
```

### Comparing `usa-net-0.0.4/usa/tasks/datasets/pybullet.py` & `usa-net-0.0.5/usa/tasks/datasets/pybullet.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/r3d.py` & `usa-net-0.0.5/usa/tasks/datasets/r3d.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/replica_cad.py` & `usa-net-0.0.5/usa/tasks/datasets/replica_cad.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/stretch.py` & `usa-net-0.0.5/usa/tasks/datasets/stretch.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/types.py` & `usa-net-0.0.5/usa/tasks/datasets/types.py`

 * *Files identical despite different names*

### Comparing `usa-net-0.0.4/usa/tasks/datasets/utils.py` & `usa-net-0.0.5/usa/tasks/datasets/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import logging
 import os
 import time
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Sized, cast
 
 import ml.api as ml
 import numpy as np
 import open3d as o3d
 import torch
 import tqdm
 from torch import Tensor
@@ -200,15 +200,16 @@
         max_samples: The maximum number of samples to use, or None to use all
         rotate: Whether to rotate the camera 90 degrees
         concat_horizontal: Whether to concatenate the images horizontally
     """
 
     def iter_frames() -> Iterator[np.ndarray]:
         i = 0
-        for item in tqdm.tqdm(ds, desc="Processing video"):
+        for j in tqdm.trange(len(cast(Sized, ds)), desc="Processing video"):
+            item = ds[j]
             depth = (item.depth - item.depth.min()) / (item.depth.max() - item.depth.min())
             reg_depth = (255 * depth).to(torch.uint8)
             # inv_depth = (255 / (32 * depth + 1)).to(torch.uint8)
             image = (item.image * 255).to(torch.uint8)
             # mask = item.mask.to(torch.uint8) * 255
 
             if rotate:
@@ -269,24 +270,27 @@
         dataset=ds,
         batch_size=batch_size,
         shuffle=False,
         num_workers=num_workers,
         collate_fn=ml.collate,
     )
 
-    pf = device.get_prefetcher(dl)
+    with ml.Timer("getting prefetcher"):
+        pf = device.get_prefetcher(dl)
+        pf_iter = iter(pf)
+
     total = (len(ds) + batch_size - 1) // batch_size  # type: ignore
 
     # Saves the complete point cloud.
     final_pcd = o3d.geometry.PointCloud()
 
     i, j = 0, 0
 
     with torch.inference_mode():
-        for item in tqdm.tqdm(pf, desc="Processing point cloud", total=total):
+        for item in tqdm.tqdm(pf_iter, desc="Processing point cloud", total=total):
             j += 1
             if j < stride:
                 continue
             j = 0
 
             image, depth, mask, intrinsics, pose = item
```

### Comparing `usa-net-0.0.4/usa_net.egg-info/PKG-INFO` & `usa-net-0.0.5/usa_net.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usa-net
-Version: 0.0.4
+Version: 0.0.5
 Summary: USA net project
 Home-page: https://github.com/codekansas/usa-net
 Author: Benjamin Bolte
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ipynb
@@ -56,7 +56,16 @@
 ### Development
 
 Add pre-commit hooks to clean Jupyter notebooks:
 
 ```bash
 pre-commit install
 ```
+
+### Notes
+
+- If you are having trouble installing Open3D on Mac, install Pybind through Conda instead:
+
+```bash
+pip uninstall open3d
+conda install open3d
+```
```

### Comparing `usa-net-0.0.4/usa_net.egg-info/SOURCES.txt` & `usa-net-0.0.5/usa_net.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 usa/planners/clip_sdf.py
 usa/planners/common.py
 usa/planners/occupancy_map.py
 usa/scripts/__init__.py
 usa/scripts/cli.py
 usa/scripts/adhoc/__init__.py
 usa/scripts/adhoc/distribution_estimates.py
+usa/scripts/adhoc/get_pybullet_dataset.py
 usa/scripts/adhoc/show_point_cloud.py
 usa/tasks/__init__.py
 usa/tasks/clip_sdf.py
 usa/tasks/datasets/__init__.py
 usa/tasks/datasets/home_robot.py
 usa/tasks/datasets/posed_rgbd.py
 usa/tasks/datasets/pybullet.py
```

