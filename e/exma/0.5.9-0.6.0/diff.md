# Comparing `tmp/exma-0.5.9.tar.gz` & `tmp/exma-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exma-0.5.9.tar", last modified: Tue Jan 24 12:47:37 2023, max compression
+gzip compressed data, was "exma-0.6.0.tar", last modified: Fri Jun  2 15:49:31 2023, max compression
```

## Comparing `exma-0.5.9.tar` & `exma-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-24 12:47:24.000000 exma-0.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-01-24 12:47:24.000000 exma-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-24 12:47:37.082202 exma-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-01-24 12:47:24.000000 exma-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.078202 exma-0.5.9/exma/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-01-24 12:47:24.000000 exma-0.5.9/exma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-01-24 12:47:24.000000 exma-0.5.9/exma/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-01-24 12:47:24.000000 exma-0.5.9/exma/cn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-01-24 12:47:24.000000 exma-0.5.9/exma/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-01-24 12:47:24.000000 exma-0.5.9/exma/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-01-24 12:47:24.000000 exma-0.5.9/exma/electrochemistry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/exma/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-01-24 12:47:24.000000 exma-0.5.9/exma/io/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.082202 exma-0.5.9/exma/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/cn.c
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/cn.h
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/pbc_distances.c
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/pbc_distances.h
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/rdf.c
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-24 12:47:24.000000 exma-0.5.9/exma/lib/rdf.h
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-01-24 12:47:24.000000 exma-0.5.9/exma/msd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-01-24 12:47:24.000000 exma-0.5.9/exma/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-01-24 12:47:24.000000 exma-0.5.9/exma/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 12:47:37.078202 exma-0.5.9/exma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-01-24 12:47:37.000000 exma-0.5.9/exma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-24 12:47:36.000000 exma-0.5.9/exma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 12:47:37.082202 exma-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-01-24 12:47:24.000000 exma-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-02 15:49:18.000000 exma-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 15:49:18.000000 exma-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-02 15:49:31.141818 exma-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-02 15:49:18.000000 exma-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-02 15:49:18.000000 exma-0.6.0/exma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-06-02 15:49:18.000000 exma-0.6.0/exma/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-06-02 15:49:18.000000 exma-0.6.0/exma/cn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-02 15:49:18.000000 exma-0.6.0/exma/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-02 15:49:18.000000 exma-0.6.0/exma/distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-02 15:49:18.000000 exma-0.6.0/exma/electrochemistry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-06-02 15:49:18.000000 exma-0.6.0/exma/io/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/cn.c
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/cn.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/pbc_distances.c
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/pbc_distances.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/rdf.c
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 15:49:18.000000 exma-0.6.0/exma/lib/rdf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-02 15:49:18.000000 exma-0.6.0/exma/msd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-06-02 15:49:18.000000 exma-0.6.0/exma/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-02 15:49:18.000000 exma-0.6.0/exma/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-02 15:49:18.000000 exma-0.6.0/exma/vacf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:49:31.141818 exma-0.6.0/exma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 15:49:31.000000 exma-0.6.0/exma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:49:31.141818 exma-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-02 15:49:18.000000 exma-0.6.0/setup.py
```

### Comparing `exma-0.5.9/LICENSE` & `exma-0.6.0/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Francisco Fernandez
+Copyright (c) 2021-2023 Francisco Fernandez
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `exma-0.5.9/PKG-INFO` & `exma-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.5.9
+Version: 0.6.0
 Summary: extendable molecular dynamics analyzer
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
-Author-email: fernandezfrancisco2195@gmail.com
+Author-email: ffernandev@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -19,27 +19,28 @@
 License-File: LICENSE
 
 # exma
 
 [![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
 
 Some of the main calculations that can be performed are listed below:
 
 * mean square displacement,
+* velocity autocorrelation function,
 * radial distribution function,
 * coordination number, the ligancy or in a shell,
 
 among others.
 
 For more precise information, see the [tutorials](https://exma.readthedocs.io/en/latest/tutorial.html)
 and the [API](https://exma.readthedocs.io/en/latest/api.html) in the documentation.
```

### Comparing `exma-0.5.9/README.md` & `exma-0.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # exma
 
 [![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
 
 Some of the main calculations that can be performed are listed below:
 
 * mean square displacement,
+* velocity autocorrelation function,
 * radial distribution function,
 * coordination number, the ligancy or in a shell,
 
 among others.
 
 For more precise information, see the [tutorials](https://exma.readthedocs.io/en/latest/tutorial.html)
 and the [API](https://exma.readthedocs.io/en/latest/api.html) in the documentation.
```

### Comparing `exma-0.5.9/exma/__init__.py` & `exma-0.6.0/exma/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
 
-"""An extendable molecular analyzer."""
+"""A Python library with C extensions to analyze and manipulate molecular \
+dynamics trajectories and electrochemical data."""
 
 # ============================================================================
 # CONSTANTS
 # ============================================================================
 
 __author__ = """Francisco Fernandez"""
-__email__ = "fernandezfrancisco2195@gmail.com"
-__version__ = "0.5.9"
+__email__ = "ffernandev@gmail.com"
+__version__ = "0.6.0"
 
 
 # ============================================================================
 # IMPORTS
 # ============================================================================
 
 # core
 from .core import AtomicSystem  # noqa
 
 # distances
 from .distances import pbc_distances  # noqa
 
 # molecular dynamics observables
 from .msd import MeanSquareDisplacement  # noqa
+from .vacf import VelocityAutocorrelationFunction  # noqa
 from .rdf import RadialDistributionFunction  # noqa
 from .cn import CoordinationNumber  # noqa
 from .cluster import EffectiveNeighbors, DBSCAN, sro  # noqa
 
 # electrochemistry
 from .electrochemistry import (  # noqa
     fractional_volume_change,  # noqa
```

### Comparing `exma-0.5.9/exma/cluster.py` & `exma-0.6.0/exma/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/cn.py` & `exma-0.6.0/exma/cn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/core.py` & `exma-0.6.0/exma/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
 
@@ -59,14 +59,23 @@
     iy : np.array, default=None
         the corresponding image of the positions of the atoms in the y
         direction
 
     iz : np.array, default=None
         the corresponding image of the positions of the atoms in the z
         direction
+
+    vx : np.array, default=None
+        the velocities of the atoms in the x direction
+
+    vy : np.array, default=None
+        the velocities of the atoms in the y direction
+
+    vz : np.array, default=None
+        the velocities of the atoms in the z direction
     """
 
     def __init__(
         self,
         natoms=None,
         box=None,
         types=None,
@@ -74,14 +83,17 @@
         q=None,
         x=None,
         y=None,
         z=None,
         ix=None,
         iy=None,
         iz=None,
+        vx=None,
+        vy=None,
+        vz=None,
     ):
         self.natoms = natoms
         self.box = box
 
         self.idx = idx
         self.types = types
 
@@ -91,14 +103,18 @@
         self.y = y
         self.z = z
 
         self.ix = ix
         self.iy = iy
         self.iz = iz
 
+        self.vx = vx
+        self.vy = vy
+        self.vz = vz
+
     def _mask_type(self, atom_type):
         """Get a masked array by an specific type of atom."""
         return self.types == atom_type
 
     def _natoms_type(self, mask_type):
         """Count the number of atoms of an specific type."""
         return np.count_nonzero(mask_type)
```

### Comparing `exma-0.5.9/exma/distances.py` & `exma-0.6.0/exma/distances.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/electrochemistry.py` & `exma-0.6.0/exma/electrochemistry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/io/__init__.py` & `exma-0.6.0/exma/io/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/io/positions.py` & `exma-0.6.0/exma/io/positions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
 
@@ -51,15 +51,14 @@
         {\rho} = {\frac{N}{L^3}}
 
     where `N` is the number of atoms and `L` the box lenght in each
     direction.
     """
 
     def __init__(self, natoms, box_size):
-
         self.natoms = natoms
         self.box_size = box_size
 
     def sc(self):
         """Simple-cubic crystal.
 
         This cell is characterized by having an atom in each of its vertices.
```

### Comparing `exma-0.5.9/exma/io/reader.py` & `exma-0.6.0/exma/io/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
 
@@ -33,18 +33,20 @@
 
     Parameters
     ----------
     filename : str
         name of the file where the trajectories in xyz format are
 
     ftype : str, default="xyz"
-        the possible values are `xyz`, `property` and `image`.
+        the possible values are `xyz`, `property`, `image` and `velocity`.
         `xyz` if is the usual xyz file. `property` if in the last
         column there is a property. `image` if in the last three columns
-        there are the image box of the corresponding atom.
+        there are the image box of the corresponding atom. `velocity` if in
+        the last three columns there are the velocities in each direction of
+        the corresponding atoms.
 
     Returns
     -------
     list
         A list with an exma.core.AtomicSystem for each frame.
     """
     with XYZ(filename, ftype) as xyz:
@@ -88,15 +90,14 @@
     pd.DataFrame
         A `pd.DataFrame` with the columns corresponding to the thermodynamic
         info.
 
     Notes
     -----
     It only works if the first thermo parameter is `Step`.
-
     """
     with open(logname, "r") as flog:
         # ignore all previous info
         line = flog.readline()
         while line.strip().startswith("Step ") is False:
             line = flog.readline()
 
@@ -128,28 +129,32 @@
 
     Parameters
     ----------
     filename : str
         name of the file where the trajectories in xyz format are
 
     ftype : str, default="xyz"
-        the possible values are `xyz`, `property` and `image`.
+        the possible values are `xyz`, `property`, `image` and `velocity`.
         `xyz` if is the usual xyz file. `property` if in the last
         column there is a property. `image` if in the last three columns
-        there are the image box of the corresponding atom.
+        there are the image box of the corresponding atom. `velocity` if in
+        the last three columns there are the velocities in each direction of
+        the corresponding atoms.
 
     Raises
     ------
     ValueError
         If xyz file type is not among the possible values
     """
 
     def __init__(self, filename, ftype="xyz"):
-        if ftype not in ("xyz", "property", "image"):
-            raise ValueError("ftype must be 'xyz', 'property' or 'image'")
+        if ftype not in ("xyz", "property", "image", "velocity"):
+            raise ValueError(
+                "ftype must be 'xyz', 'property', 'image' or 'velocity'"
+            )
 
         super().__init__(filename, ftype)
 
     def read_frame(self):
         """Read the actual frame of an .xyz file.
 
         Returns
@@ -163,59 +168,66 @@
             If there are no more frames to read
         """
         natoms = self.file_traj_.readline()
         if not natoms or natoms == "\n":
             raise EOFError("There is no more frames to read")
 
         natoms = np.intc(natoms)
+
         self.file_traj_.readline()  # usually a comment in .xyz files
 
         atom_type = []
         x, y, z = [], [], []
         q = [] if self.ftype == "property" else None
         ix, iy, iz = [], [], [] if self.ftype == "image" else None
+        vx, vy, vz = [], [], [] if self.ftype == "velocity" else None
         for i in range(natoms):
             xyzline = self.file_traj_.readline().split()
 
             atom_type.append(xyzline[0])
 
             x.append(xyzline[1])
             y.append(xyzline[2])
             z.append(xyzline[3])
 
             if self.ftype == "property":
                 q.append(xyzline[4])
+
             elif self.ftype == "image":
                 ix.append(xyzline[4])
                 iy.append(xyzline[5])
                 iz.append(xyzline[6])
 
+            elif self.ftype == "velocity":
+                vx.append(xyzline[4])
+                vy.append(xyzline[5])
+                vz.append(xyzline[6])
+
         frame = AtomicSystem()
 
         frame.natoms = natoms
+
         frame.types = np.asarray(atom_type, dtype=str)
+
         frame.x = np.asarray(x, dtype=np.float32)
         frame.y = np.asarray(y, dtype=np.float32)
         frame.z = np.asarray(z, dtype=np.float32)
 
-        frame.ix = (
-            np.asarray(ix, dtype=np.intc) if self.ftype == "image" else None
-        )
-        frame.iy = (
-            np.asarray(iy, dtype=np.intc) if self.ftype == "image" else None
-        )
-        frame.iz = (
-            np.asarray(iz, dtype=np.intc) if self.ftype == "image" else None
-        )
-
-        frame.q = (
-            np.asarray(q, dtype=np.float32)
-            if self.ftype == "property"
-            else None
-        )
+        if self.ftype == "property":
+            frame.q = np.asarray(q, dtype=np.float32)
+
+        elif self.ftype == "image":
+            frame.ix = np.asarray(ix, dtype=np.intc)
+            frame.iy = np.asarray(iy, dtype=np.intc)
+            frame.iz = np.asarray(iz, dtype=np.intc)
+
+        elif self.ftype == "velocity":
+            frame.vx = np.asarray(vx, dtype=np.float32)
+            frame.vy = np.asarray(vy, dtype=np.float32)
+            frame.vz = np.asarray(vz, dtype=np.float32)
 
         return frame
 
 
 class LAMMPS(TrajectoryReader):
     """Class to read lammpstrj files.
```

### Comparing `exma-0.5.9/exma/io/writer.py` & `exma-0.6.0/exma/io/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
 
@@ -73,15 +73,14 @@
         This have all the information of the configurations of the system.
 
     file_in : str
         name of the file where you want to write the input info
     """
     header = ("natoms", "box")
     with open(file_in, "w") as f_in:
-
         f_in.write("# the first three lines are comments...\n")
 
         f_in_header = "# columns in order:"
         for key in frame.__dict__.keys():
             if key.startswith("_") or key in ("natoms", "box"):
                 continue
             elif frame.__dict__[key] is not None:
```

### Comparing `exma-0.5.9/exma/lib/cn.c` & `exma-0.6.0/exma/lib/cn.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // This file is part of exma (https://github.com/fernandezfran/exma/)
-// Copyright (c) 2021, Francisco Fernandez
+// Copyright (c) 2021-2023, Francisco Fernandez
 // License: MIT
 //     Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 #include "cn.h"
 
 #include <math.h>
 
 void cn_accumulate(const int natoms_c, const int natoms_i, const float *box,
```

### Comparing `exma-0.5.9/exma/lib/pbc_distances.c` & `exma-0.6.0/exma/lib/pbc_distances.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // This file is part of exma (https://github.com/fernandezfran/exma/)
-// Copyright (c) 2021, Francisco Fernandez
+// Copyright (c) 2021-2023, Francisco Fernandez
 // License: MIT
 //     Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 #include "pbc_distances.h"
 
 #include <math.h>
 
 void distance_matrix(const int natoms_c, const int natoms_i, const float *box,
```

### Comparing `exma-0.5.9/exma/lib/rdf.c` & `exma-0.6.0/exma/lib/rdf.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // This file is part of exma (https://github.com/fernandezfran/exma/)
-// Copyright (c) 2021, Francisco Fernandez
+// Copyright (c) 2021-2023, Francisco Fernandez
 // License: MIT
 //     Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 #include "rdf.h"
 
 #include <math.h>
 
 void rdf_accumulate(const int natoms_c, const int natoms_i, const float *box,
```

### Comparing `exma-0.5.9/exma/msd.py` & `exma-0.6.0/exma/msd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/rdf.py` & `exma-0.6.0/exma/rdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma/statistics.py` & `exma-0.6.0/exma/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # ============================================================================
 # DOCS
 # ============================================================================
```

### Comparing `exma-0.5.9/exma.egg-info/PKG-INFO` & `exma-0.6.0/exma.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: exma
-Version: 0.5.9
+Version: 0.6.0
 Summary: extendable molecular dynamics analyzer
 Home-page: https://github.com/fernandezfran/exma
 Author: Francisco Fernandez
-Author-email: fernandezfrancisco2195@gmail.com
+Author-email: ffernandev@gmail.com
 License: MIT
 Keywords: exma,molecular-dynamics,data-analysis
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -19,27 +19,28 @@
 License-File: LICENSE
 
 # exma
 
 [![exma CI](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml/badge.svg)](https://github.com/fernandezfran/exma/actions/workflows/exma_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/exma/badge/?version=latest)](https://exma.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/exma)](https://pypi.org/project/exma/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/galpynostatic/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/exma?period=total&units=international_system&left_color=black&right_color=black&left_text=downloads)](https://pepy.tech/project/exma)
 
 **exma** is a Python library with C extensions to analyze and manipulate 
 molecular dynamics trajectories and electrochemical data.
 
 
 ## Main Features
 
 Some of the main calculations that can be performed are listed below:
 
 * mean square displacement,
+* velocity autocorrelation function,
 * radial distribution function,
 * coordination number, the ligancy or in a shell,
 
 among others.
 
 For more precise information, see the [tutorials](https://exma.readthedocs.io/en/latest/tutorial.html)
 and the [API](https://exma.readthedocs.io/en/latest/api.html) in the documentation.
```

### Comparing `exma-0.5.9/exma.egg-info/SOURCES.txt` & `exma-0.6.0/exma.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 exma/cn.py
 exma/core.py
 exma/distances.py
 exma/electrochemistry.py
 exma/msd.py
 exma/rdf.py
 exma/statistics.py
+exma/vacf.py
 exma.egg-info/PKG-INFO
 exma.egg-info/SOURCES.txt
 exma.egg-info/dependency_links.txt
 exma.egg-info/requires.txt
 exma.egg-info/top_level.txt
 exma/io/__init__.py
 exma/io/positions.py
```

### Comparing `exma-0.5.9/setup.py` & `exma-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # This file is part of exma (https://github.com/fernandezfran/exma/).
-# Copyright (c) 2021, Francisco Fernandez
+# Copyright (c) 2021-2023, Francisco Fernandez
 # License: MIT
 #   Full Text: https://github.com/fernandezfran/exma/blob/master/LICENSE
 
 # =============================================================================
 # DOCS
 # =============================================================================
 
@@ -70,15 +70,15 @@
     name="exma",
     version=VERSION,
     description="extendable molecular dynamics analyzer",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     author="Francisco Fernandez",
-    author_email="fernandezfrancisco2195@gmail.com",
+    author_email="ffernandev@gmail.com",
     url="https://github.com/fernandezfran/exma",
     license="MIT",
     install_requires=REQUIREMENTS,
     setup_requires=REQUIREMENTS,
     keywords=["exma", "molecular-dynamics", "data-analysis"],
     classifiers=[
         "Development Status :: 4 - Beta",
```

