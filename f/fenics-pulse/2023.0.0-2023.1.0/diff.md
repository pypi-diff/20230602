# Comparing `tmp/fenics_pulse-2023.0.0.tar.gz` & `tmp/fenics_pulse-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenics_pulse-2023.0.0.tar", last modified: Fri Mar 31 08:13:42 2023, max compression
+gzip compressed data, was "fenics_pulse-2023.1.0.tar", last modified: Fri Jun  2 18:00:53 2023, max compression
```

## Comparing `fenics_pulse-2023.0.0.tar` & `fenics_pulse-2023.1.0.tar`

### file list

```diff
@@ -1,52 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.057420 fenics_pulse-2023.0.0/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5139 2023-03-31 08:13:42.057420 fenics_pulse-2023.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4406 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.045420 fenics_pulse-2023.0.0/fenics_pulse.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5139 2023-03-31 08:13:42.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1160 2023-03-31 08:13:42.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 08:13:42.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 08:13:01.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      331 2023-03-31 08:13:42.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-31 08:13:42.000000 fenics_pulse-2023.0.0/fenics_pulse.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.049420 fenics_pulse-2023.0.0/pulse/
--rw-r--r--   0 root         (0) root         (0)     5811 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/__init__.py
--rw-r--r--   0 root         (0) root         (0)      202 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/__version__.py
--rw-r--r--   0 root         (0) root         (0)    12668 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.053420 fenics_pulse-2023.0.0/pulse/example_meshes/
--rw-r--r--   0 root         (0) root         (0)      367 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1759856 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/benchmark.h5
--rw-r--r--   0 root         (0) root         (0)   841888 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/biv_ellipsoid.h5
--rw-r--r--   0 root         (0) root         (0)  1321872 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/ellipsoid.h5
--rw-r--r--   0 root         (0) root         (0)   167056 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/prolate_ellipsoid.h5
--rw-r--r--   0 root         (0) root         (0)   749768 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/example_meshes/simple_ellipsoid.h5
--rw-r--r--   0 root         (0) root         (0)    12661 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/geometry.py
--rw-r--r--   0 root         (0) root         (0)    13852 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/geometry_utils.py
--rw-r--r--   0 root         (0) root         (0)     2177 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/io_utils.py
--rw-r--r--   0 root         (0) root         (0)    19368 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/iterate.py
--rw-r--r--   0 root         (0) root         (0)     3132 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/kinematics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.053420 fenics_pulse-2023.0.0/pulse/material/
--rw-r--r--   0 root         (0) root         (0)     1015 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7307 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/active_model.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/guccione.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/holzapfelogden.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/linearelastic.py
--rw-r--r--   0 root         (0) root         (0)     9424 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/material_model.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/neohookean.py
--rw-r--r--   0 root         (0) root         (0)      601 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/material/stvenantkirchhoff.py
--rw-r--r--   0 root         (0) root         (0)    11518 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/mechanicsproblem.py
--rw-r--r--   0 root         (0) root         (0)     6885 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/numpy_mpi.py
--rw-r--r--   0 root         (0) root         (0)     5488 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/solver.py
--rw-r--r--   0 root         (0) root         (0)    13770 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/unloader.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/unloading_utils.py
--rw-r--r--   0 root         (0) root         (0)     2976 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/pulse/utils.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-03-31 08:13:42.057420 fenics_pulse-2023.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1243 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 08:13:42.057420 fenics_pulse-2023.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_demos.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_dolfin_utils.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     4414 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_iterate.py
--rw-r--r--   0 root         (0) root         (0)     4977 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_kinematics.py
--rw-r--r--   0 root         (0) root         (0)     6945 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_material.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-03-31 08:12:39.000000 fenics_pulse-2023.0.0/tests/test_unloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.703606 fenics_pulse-2023.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-02 18:00:53.699606 fenics_pulse-2023.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:00:53.703606 fenics_pulse-2023.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.691605 fenics_pulse-2023.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.691605 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-02 18:00:53.000000 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-02 18:00:53.000000 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:00:53.000000 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 18:00:53.000000 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 18:00:53.000000 fenics_pulse-2023.1.0/src/fenics_pulse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.695606 fenics_pulse-2023.1.0/src/pulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/dolfin_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.695606 fenics_pulse-2023.1.0/src/pulse/example_meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/example_meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/kinematics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.699606 fenics_pulse-2023.1.0/src/pulse/material/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/active_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/guccione.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/holzapfelogden.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/linearelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/material_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/neohookean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/material/stvenantkirchhoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/mechanicsproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/numpy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/unloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/unloading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/src/pulse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:00:53.699606 fenics_pulse-2023.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_dolfin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-02 18:00:38.000000 fenics_pulse-2023.1.0/tests/test_unloader.py
```

### Comparing `fenics_pulse-2023.0.0/LICENSE` & `fenics_pulse-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/PKG-INFO` & `fenics_pulse-2023.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: fenics_pulse
-Version: 2023.0.0
-Summary: A python library based on FEniCS that aims to solve problems in continuum mechanics, in particular cardiac mechanics
-Home-page: https://github.com/finsberg/pulse
-Author: Henrik Finsberg
-Author-email: henriknf@simula.no
-License: LGPL-3.0
-Keywords: finite element,mechanics,cardiac,heart
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: mesh
-Provides-Extra: plot
-Provides-Extra: test
-License-File: LICENSE
-
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pulse/badges/version.svg)](https://anaconda.org/conda-forge/pulse)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/pulse/badges/downloads.svg)](https://anaconda.org/conda-forge/pulse)
 [![CI](https://github.com/finsberg/pulse/actions/workflows/main.yml/badge.svg)](https://github.com/finsberg/pulse/actions/workflows/main.yml)
 [![Platform](https://anaconda.org/finsberg/pulse/badges/platforms.svg)](https://anaconda.org/finsberg/pulse)
 [![status](http://joss.theoj.org/papers/9abee735e6abadabe9252d5fcc84fd40/status.svg)](http://joss.theoj.org/papers/9abee735e6abadabe9252d5fcc84fd40)
 [![codecov](https://codecov.io/gh/finsberg/pulse/branch/master/graph/badge.svg?token=cZEkiXSOKm)](https://codecov.io/gh/finsberg/pulse)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/finsberg/pulse/master.svg)](https://results.pre-commit.ci/latest/github/finsberg/pulse/master)
```

### Comparing `fenics_pulse-2023.0.0/pulse/__init__.py` & `fenics_pulse-2023.1.0/src/pulse/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import logging as _logging
 import os
+from importlib.metadata import metadata
 
 from dolfin import as_backend_type
 from dolfin import assemble
 from dolfin import Constant
 from dolfin import DirichletBC
 from dolfin import Function
 from dolfin import FunctionAssigner
 from dolfin import interpolate
 from dolfin import Mesh
 from dolfin import project
 
 
+meta = metadata("fenics-pulse")
+__version__ = meta["Version"]
+__author__ = meta["Author"]
+__license__ = meta["License"]
+__email__ = meta["Author-email"]
+__program_name__ = meta["Name"]
+
+
 Constants = Constant
 Functions = Function
 # Check if dolfin-adjoint is installed, and if
 # the 'DOLFIN_ADJOINT' flag is set to 0, then
 # we remove it from sys.modules
 try:
     import dolfin_adjoint  # noqa: F401
@@ -57,15 +66,14 @@
 from . import kinematics
 from . import material
 from . import mechanicsproblem
 from . import numpy_mpi
 from . import solver
 from . import unloader
 from . import utils
-from .__version__ import __version__
 from .dolfin_utils import MixedParameter
 from .dolfin_utils import QuadratureSpace
 from .dolfin_utils import RegionalParameter
 from .example_meshes import mesh_paths
 from .geometry import CRLBasis
 from .geometry import Geometry
 from .geometry import HeartGeometry
@@ -186,15 +194,14 @@
     "GreenLagrangeStrain",
     "LeftCauchyGreen",
     "RightCauchyGreen",
     "EulerAlmansiStrain",
     "PiolaTransform",
     "InversePiolaTransform",
     "set_log_level",
-    "__version__",
     "solver",
     "mesh_paths",
     "NonlinearProblem",
     "NonlinearSolver",
     "geometry",
     "geometry_utils",
     "ActiveModel",
```

### Comparing `fenics_pulse-2023.0.0/pulse/dolfin_utils.py` & `fenics_pulse-2023.1.0/src/pulse/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/geometry.py` & `fenics_pulse-2023.1.0/src/pulse/geometry.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/geometry_utils.py` & `fenics_pulse-2023.1.0/src/pulse/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/io_utils.py` & `fenics_pulse-2023.1.0/src/pulse/io_utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/iterate.py` & `fenics_pulse-2023.1.0/src/pulse/iterate.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/kinematics.py` & `fenics_pulse-2023.1.0/src/pulse/kinematics.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/__init__.py` & `fenics_pulse-2023.1.0/src/pulse/material/__init__.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/active_model.py` & `fenics_pulse-2023.1.0/src/pulse/material/active_model.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/guccione.py` & `fenics_pulse-2023.1.0/src/pulse/material/guccione.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/holzapfelogden.py` & `fenics_pulse-2023.1.0/src/pulse/material/holzapfelogden.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/linearelastic.py` & `fenics_pulse-2023.1.0/src/pulse/material/linearelastic.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/material_model.py` & `fenics_pulse-2023.1.0/src/pulse/material/material_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,17 @@
         return incompressible(*args, **kwargs)
 
 
 def incompressible(p, J):
     return -p * (J - 1.0)
 
 
+_t = _active_model.ActiveStressModels.transversally
+
+
 class Material(ABC):
     """
     Initialize material model
 
     Parameters
     ----------
 
@@ -94,15 +97,15 @@
         eta: float = 0.0,
         isochoric: bool = True,
         compressible_model="incompressible",
         geometry=None,
         f0=None,
         s0=None,
         n0=None,
-        active_isotropy: _active_model.ActiveStressModels = _active_model.ActiveStressModels.transversally,
+        active_isotropy: _active_model.ActiveStressModels = _t,
         *args,
         **kwargs
     ):
         # Parameters
         self.parameters = self.__class__.default_parameters()
         if parameters is not None:
             self.parameters.update(parameters)
```

### Comparing `fenics_pulse-2023.0.0/pulse/material/neohookean.py` & `fenics_pulse-2023.1.0/src/pulse/material/neohookean.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/material/stvenantkirchhoff.py` & `fenics_pulse-2023.1.0/src/pulse/material/stvenantkirchhoff.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/mechanicsproblem.py` & `fenics_pulse-2023.1.0/src/pulse/mechanicsproblem.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/numpy_mpi.py` & `fenics_pulse-2023.1.0/src/pulse/numpy_mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 
 def broadcast(array, from_process):
     "Broadcast array to all processes"
     if not hasattr(broadcast, "cpp_module"):
         cpp_code = """
 
         namespace dolfin {
-            std::vector<double> broadcast(const MPI_Comm mpi_comm, const Array<double>& inarray, int from_process)
+            std::vector<double> broadcast(
+                const MPI_Comm mpi_comm,
+                const Array<double>& inarray, int from_process)
             {
                 int this_process = dolfin::MPI::rank(mpi_comm);
                 std::vector<double> outvector(inarray.size());
 
                 if(this_process == from_process) {
                     for(int i=0; i<inarray.size(); i++)
                     {
@@ -115,19 +117,23 @@
 
 
 def gather(array, on_process=0, flatten=False):
     "Gather array from all processes on a single process"
     if not hasattr(gather, "cpp_module"):
         cpp_code = """
         namespace dolfin {
-            std::vector<double> gather(const MPI_Comm mpi_comm, const Array<double>& inarray, int on_process)
+            std::vector<double> gather(
+                const MPI_Comm mpi_comm,
+                const Array<double>& inarray, int on_process)
             {
                 int this_process = dolfin::MPI::rank(mpi_comm);
 
-                std::vector<double> outvector(dolfin::MPI::size(mpi_comm)*dolfin::MPI::sum(mpi_comm, inarray.size()));
+                std::vector<double> outvector(
+                    dolfin::MPI::size(mpi_comm)*dolfin::MPI::sum(mpi_comm, inarray.size())
+                );
                 std::vector<double> invector(inarray.size());
 
                 for(int i=0; i<inarray.size(); i++)
                 {
                     invector[i] = inarray[i];
                 }
```

### Comparing `fenics_pulse-2023.0.0/pulse/solver.py` & `fenics_pulse-2023.1.0/src/pulse/solver.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/unloader.py` & `fenics_pulse-2023.1.0/src/pulse/unloader.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/unloading_utils.py` & `fenics_pulse-2023.1.0/src/pulse/unloading_utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/pulse/utils.py` & `fenics_pulse-2023.1.0/src/pulse/utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_demos.py` & `fenics_pulse-2023.1.0/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_dolfin_utils.py` & `fenics_pulse-2023.1.0/tests/test_dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_geometry.py` & `fenics_pulse-2023.1.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_iterate.py` & `fenics_pulse-2023.1.0/tests/test_iterate.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_kinematics.py` & `fenics_pulse-2023.1.0/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_material.py` & `fenics_pulse-2023.1.0/tests/test_material.py`

 * *Files identical despite different names*

### Comparing `fenics_pulse-2023.0.0/tests/test_unloader.py` & `fenics_pulse-2023.1.0/tests/test_unloader.py`

 * *Files identical despite different names*

