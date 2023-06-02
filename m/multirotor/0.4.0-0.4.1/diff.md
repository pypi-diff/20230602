# Comparing `tmp/multirotor-0.4.0.tar.gz` & `tmp/multirotor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multirotor-0.4.0.tar", last modified: Thu May 25 19:18:48 2023, max compression
+gzip compressed data, was "multirotor-0.4.1.tar", last modified: Fri Jun  2 16:13:33 2023, max compression
```

## Comparing `multirotor-0.4.0.tar` & `multirotor-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-05-25 19:18:48.300461 multirotor-0.4.0/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      823 2022-09-06 21:25:06.000000 multirotor-0.4.0/README.md
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/multirotor/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.4.0/multirotor/__init__.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2484 2022-12-12 19:19:30.000000 multirotor-0.4.0/multirotor/coords.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     8813 2023-05-25 18:30:50.000000 multirotor-0.4.0/multirotor/env.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    16660 2023-05-25 17:45:38.000000 multirotor-0.4.0/multirotor/helpers.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    15815 2023-05-25 18:01:00.000000 multirotor-0.4.0/multirotor/optimize.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6604 2023-04-21 20:33:09.000000 multirotor-0.4.0/multirotor/physics.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    22940 2023-05-04 21:54:19.000000 multirotor-0.4.0/multirotor/simulation.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     9821 2023-05-03 15:46:07.000000 multirotor-0.4.0/multirotor/trajectories.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5418 2023-04-11 13:45:56.000000 multirotor-0.4.0/multirotor/vehicle.py
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    14409 2023-05-04 15:21:26.000000 multirotor-0.4.0/multirotor/visualize.py
-drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-05-25 19:18:48.300461 multirotor-0.4.0/multirotor.egg-info/
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1079 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/PKG-INFO
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      430 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/SOURCES.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/dependency_links.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      109 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/requires.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2023-05-25 19:18:48.000000 multirotor-0.4.0/multirotor.egg-info/top_level.txt
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.4.0/pyproject.toml
--rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      494 2023-05-25 19:18:48.304461 multirotor-0.4.0/setup.cfg
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-06-02 16:13:33.071831 multirotor-0.4.1/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1514 2023-06-02 16:13:33.071831 multirotor-0.4.1/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1258 2023-05-26 17:44:05.000000 multirotor-0.4.1/README.md
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-06-02 16:13:33.071831 multirotor-0.4.1/multirotor/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        0 2022-09-06 21:25:06.000000 multirotor-0.4.1/multirotor/__init__.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     2484 2022-12-12 19:19:30.000000 multirotor-0.4.1/multirotor/coords.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     8813 2023-05-25 18:30:50.000000 multirotor-0.4.1/multirotor/env.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    16660 2023-05-25 17:45:38.000000 multirotor-0.4.1/multirotor/helpers.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    15815 2023-05-25 18:01:00.000000 multirotor-0.4.1/multirotor/optimize.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     6604 2023-04-21 20:33:09.000000 multirotor-0.4.1/multirotor/physics.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    22940 2023-05-04 21:54:19.000000 multirotor-0.4.1/multirotor/simulation.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     9821 2023-05-03 15:46:07.000000 multirotor-0.4.1/multirotor/trajectories.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     5437 2023-06-02 16:06:35.000000 multirotor-0.4.1/multirotor/vehicle.py
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)    14409 2023-05-04 15:21:26.000000 multirotor-0.4.1/multirotor/visualize.py
+drwxr-xr-x   0 ahmedi    (1001) ahmedi    (1001)        0 2023-06-02 16:13:33.071831 multirotor-0.4.1/multirotor.egg-info/
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)     1514 2023-06-02 16:13:33.000000 multirotor-0.4.1/multirotor.egg-info/PKG-INFO
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      430 2023-06-02 16:13:33.000000 multirotor-0.4.1/multirotor.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)        1 2023-06-02 16:13:33.000000 multirotor-0.4.1/multirotor.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      121 2023-06-02 16:13:33.000000 multirotor-0.4.1/multirotor.egg-info/requires.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       11 2023-06-02 16:13:33.000000 multirotor-0.4.1/multirotor.egg-info/top_level.txt
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)       81 2022-09-06 21:25:06.000000 multirotor-0.4.1/pyproject.toml
+-rw-r--r--   0 ahmedi    (1001) ahmedi    (1001)      507 2023-06-02 16:13:33.071831 multirotor-0.4.1/setup.cfg
```

### Comparing `multirotor-0.4.0/PKG-INFO` & `multirotor-0.4.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
 
 # multirotor
 
 Simulation of multi-rotor unmanned aerial vehicles in python.
 
+This package provides an object-oriented interface for modeling and simulating motors, propellers, and airframe of a UAV. Additionally, an OpenAI gym-compatible environment is provided for Reinforcement Learning experiments.
+
+See the [Detailed Demo](./Detailed%20Demo.ipynb) jupyter notebbok for a walkthrough.
+
 Please cite this as:
 
 ```
 @inproceedings{ahmed2022multirotor,
     title={A high-Fidelity Simulation test-Bed for fault-Tolerant octo-Rotor Control Using Reinforcement Learning},
     author={Ahmed, Ibrahim and Quinones-Grueiro, Marcos and Biswas, Gautam},
     booktitle={2022 IEEE/AIAA 41st Digital Avionics Systems Conference (DASC)},
@@ -24,18 +28,27 @@
 }
 ```
 
 ## Installation
 
 Install from the Python Package Index (PyPI):
 
-```
+```bash
 pip install multirotor
 ```
 
 Or, clone repository and install for development. This will allow you to change the code of the package so the changes show up when you `import multirotor` in other projects.
 
-```
+```bash
 git clone https://github.com/hazrmard/multirotor.git
 cd multirotor
 pip install -e .
+
+# to also install dependencies for building package/documentation
+pip install -e .[DEV]
+```
+
+## Usage
+
+```python
+
 ```
```

### Comparing `multirotor-0.4.0/README.md` & `multirotor-0.4.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # multirotor
 
 Simulation of multi-rotor unmanned aerial vehicles in python.
 
+This package provides an object-oriented interface for modeling and simulating motors, propellers, and airframe of a UAV. Additionally, an OpenAI gym-compatible environment is provided for Reinforcement Learning experiments.
+
+See the [Detailed Demo](./Detailed%20Demo.ipynb) jupyter notebbok for a walkthrough.
+
 Please cite this as:
 
 ```
 @inproceedings{ahmed2022multirotor,
     title={A high-Fidelity Simulation test-Bed for fault-Tolerant octo-Rotor Control Using Reinforcement Learning},
     author={Ahmed, Ibrahim and Quinones-Grueiro, Marcos and Biswas, Gautam},
     booktitle={2022 IEEE/AIAA 41st Digital Avionics Systems Conference (DASC)},
@@ -14,18 +18,27 @@
 }
 ```
 
 ## Installation
 
 Install from the Python Package Index (PyPI):
 
-```
+```bash
 pip install multirotor
 ```
 
 Or, clone repository and install for development. This will allow you to change the code of the package so the changes show up when you `import multirotor` in other projects.
 
-```
+```bash
 git clone https://github.com/hazrmard/multirotor.git
 cd multirotor
 pip install -e .
+
+# to also install dependencies for building package/documentation
+pip install -e .[DEV]
+```
+
+## Usage
+
+```python
+
 ```
```

### Comparing `multirotor-0.4.0/multirotor/coords.py` & `multirotor-0.4.1/multirotor/coords.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/env.py` & `multirotor-0.4.1/multirotor/env.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/helpers.py` & `multirotor-0.4.1/multirotor/helpers.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/optimize.py` & `multirotor-0.4.1/multirotor/optimize.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/physics.py` & `multirotor-0.4.1/multirotor/physics.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/simulation.py` & `multirotor-0.4.1/multirotor/simulation.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/trajectories.py` & `multirotor-0.4.1/multirotor/trajectories.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor/vehicle.py` & `multirotor-0.4.1/multirotor/vehicle.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,30 +95,30 @@
     "Maximum voltage of the battery"
 
 
 
 @dataclass
 class VehicleParams:
 
+    mass: float
+    "The total mass of the vehicle"
+    # TODO: Should moments of inertia of propeller motors be added to this matrix
+    # manually? Currently we assume this represents the whole vehicle.
+    inertia_matrix: np.ndarray
+    "3x3 intertia matrix describing the rotational properties of the body."
     propellers: List[PropellerParams]
     angles: np.ndarray
     "Angle (radians) of propeller arm from the positive x-axis (forward) of the body frame."
     distances: np.ndarray
     "Distance (m) of each propeller from the centre of mass."
     clockwise: np.ndarray = None
     """1 if motor spins clockwise, -1 if anti-clockwise, looking from the top.
     Defaults to alternating clockwise/anti-clockwise."""
-
     battery: BatteryParams = None
     "The battery parameters"
-    mass: float = 1.
-    # TODO: Should moments of inertia of propeller motors be added to this matrix
-    # manually? Currently we assume this represents the whole vehicle.
-    inertia_matrix: np.matrix = np.eye(3)
-    "3x3 intertia matrix describing the rotational properties of the body."
 
 
     def __post_init__(self):
         self.nprops = len(self.propellers)
         "Number of propellers"
         self.distances = self.distances.astype(float)
         self.inertia_matrix_inverse = np.linalg.inv(self.inertia_matrix)
```

### Comparing `multirotor-0.4.0/multirotor/visualize.py` & `multirotor-0.4.1/multirotor/visualize.py`

 * *Files identical despite different names*

### Comparing `multirotor-0.4.0/multirotor.egg-info/PKG-INFO` & `multirotor-0.4.1/multirotor.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: multirotor
-Version: 0.4.0
+Version: 0.4.1
 Summary: Simulation testbed for multirotor vehicles.
 Keywords: multirotor,simulation,gym,uav
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: DEV
 Provides-Extra: CONTROL
 
 # multirotor
 
 Simulation of multi-rotor unmanned aerial vehicles in python.
 
+This package provides an object-oriented interface for modeling and simulating motors, propellers, and airframe of a UAV. Additionally, an OpenAI gym-compatible environment is provided for Reinforcement Learning experiments.
+
+See the [Detailed Demo](./Detailed%20Demo.ipynb) jupyter notebbok for a walkthrough.
+
 Please cite this as:
 
 ```
 @inproceedings{ahmed2022multirotor,
     title={A high-Fidelity Simulation test-Bed for fault-Tolerant octo-Rotor Control Using Reinforcement Learning},
     author={Ahmed, Ibrahim and Quinones-Grueiro, Marcos and Biswas, Gautam},
     booktitle={2022 IEEE/AIAA 41st Digital Avionics Systems Conference (DASC)},
@@ -24,18 +28,27 @@
 }
 ```
 
 ## Installation
 
 Install from the Python Package Index (PyPI):
 
-```
+```bash
 pip install multirotor
 ```
 
 Or, clone repository and install for development. This will allow you to change the code of the package so the changes show up when you `import multirotor` in other projects.
 
-```
+```bash
 git clone https://github.com/hazrmard/multirotor.git
 cd multirotor
 pip install -e .
+
+# to also install dependencies for building package/documentation
+pip install -e .[DEV]
+```
+
+## Usage
+
+```python
+
 ```
```

