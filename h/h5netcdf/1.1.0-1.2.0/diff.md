# Comparing `tmp/h5netcdf-1.1.0.tar.gz` & `tmp/h5netcdf-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5netcdf-1.1.0.tar", last modified: Wed Nov 23 06:40:28 2022, max compression
+gzip compressed data, was "h5netcdf-1.2.0.tar", last modified: Fri Jun  2 05:40:33 2023, max compression
```

## Comparing `h5netcdf-1.1.0.tar` & `h5netcdf-1.2.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9117 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    11201 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10366 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      642 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      317 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       30 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4004 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     5326 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/devguide.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3399 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/feature.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2338 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      354 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/doc/legacyapi.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/h5netcdf/
--rw-r--r--   0 runner    (1001) docker     (122)      455 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      176 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3607 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/attrs.py
--rw-r--r--   0 runner    (1001) docker     (122)    46135 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     8060 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     7140 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/legacyapi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/h5netcdf/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     5022 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)      172 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (122)    84344 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/tests/test_h5netcdf.py
--rw-r--r--   0 runner    (1001) docker     (122)      678 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/h5netcdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/h5netcdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    11201 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      633 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2022-11-23 06:40:28.000000 h5netcdf-1.1.0/h5netcdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-23 06:40:28.608608 h5netcdf-1.1.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (122)     1520 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/licenses/H5PY_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)    12760 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/licenses/PSF_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      294 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      484 2022-11-23 06:40:28.612608 h5netcdf-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2022-11-23 06:40:05.000000 h5netcdf-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.135741 h5netcdf-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-02 05:40:33.135741 h5netcdf-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.131741 h5netcdf-1.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/devguide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/feature.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/doc/legacyapi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.131741 h5netcdf-1.2.0/h5netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45587 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7826 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/legacyapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.135741 h5netcdf-1.2.0/h5netcdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    84177 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/tests/test_h5netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/h5netcdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.131741 h5netcdf-1.2.0/h5netcdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 05:40:33.000000 h5netcdf-1.2.0/h5netcdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:40:33.135741 h5netcdf-1.2.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/licenses/H5PY_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12761 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/licenses/PSF_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-02 05:40:13.000000 h5netcdf-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 05:40:33.135741 h5netcdf-1.2.0/setup.cfg
```

### Comparing `h5netcdf-1.1.0/CHANGELOG.rst` & `h5netcdf-1.2.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 Change Log
 ----------
+
+Version 1.2.0 (June 2nd, 2023):
+
+- Remove h5py2 compatibility code, remove h5py2 CI runs, mention NEP29 as
+  upstream dependency support strategy.
+  By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_ and
+  `Mark Harfouche <https://github.com/hmaarrfk>`_.
+- Update to pyproject.toml-only build process, adapt CI, use `ruff` for linting, add .pre-commit-config.yaml.
+  By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
+- Maintenance CI (use setup-micromamba), fix hsds, fix tests, fix license.
+  By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
+- Raise early with h5py-error.
+  By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
+- Add simple test to ensure that the shape is stored in the coordinates.
+  By `Mark Harfouche <https://github.com/hmaarrfk>`_.
+
 Version 1.1.0 (November 23rd, 2022):
 
 - Rework adding _FillValue-attribute, add tests.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
 - Add special add_phony method for creating phony dimensions, add test.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
 - Rewrite _unlabeled_dimension_mix (labeled/unlabeled), add tests.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
 - Add default netcdf fillvalues, pad only if necessary, adapt tests.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
 - Fix regression in padding algorithm, add test.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
-- Set ``track_order=True`` by default in created files if h5py 3.7.0 or 
+- Set ``track_order=True`` by default in created files if h5py 3.7.0 or
   greater is detected to help compatibility with netCDF4-c programs.
   By `Mark Harfouche <https://github.com/hmaarrfk>`_.
 
 Version 1.0.2 (August 2nd, 2022):
 
 - Adapt boolean indexing as h5py 3.7.0 started supporting it.
   By `Kai Mühlbauer <https://github.com/kmuehlbauer>`_.
```

### Comparing `h5netcdf-1.1.0/LICENSE` & `h5netcdf-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5netcdf-1.1.0/PKG-INFO` & `h5netcdf-1.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: h5netcdf
-Version: 1.1.0
-Summary: netCDF4 via h5py
-Home-page: https://h5netcdf.org
-Author: h5netcdf developers
-Author-email: devteam@h5netcdf.org
-License: BSD
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.txt
-
 h5netcdf
 ========
 
 .. image:: https://github.com/h5netcdf/h5netcdf/workflows/CI/badge.svg
     :target: https://github.com/h5netcdf/h5netcdf/actions
 .. image:: https://badge.fury.io/py/h5netcdf.svg
     :target: https://pypi.org/project/h5netcdf/
@@ -63,25 +39,30 @@
 .. _xarray: https://github.com/pydata/xarray/
 
 Install
 -------
 
 Ensure you have a recent version of h5py installed (I recommend using `conda`_ or
 the community effort `conda-forge`_).
-At least version 2.1 is required (for dimension scales); versions 2.3 and newer
-have been verified to work, though some tests only pass on h5py 2.6. Then::
+At least version 3.0 is required. Then::
 
     $ pip install h5netcdf
 
 Or if you are already using conda::
 
     $ conda install h5netcdf
 
+Note:
+
+From version 1.2. h5netcdf tries to align with a `nep29`_-like support policy with regard
+to it's upstream dependencies.
+
 .. _conda: https://conda.io/
 .. _conda-forge: https://conda-forge.org/
+.. _nep29: https://numpy.org/neps/nep-0029-deprecation_policy.html
 
 Usage
 -----
 
 h5netcdf has two APIs, a new API and a legacy API. Both interfaces currently
 reproduce most of the features of the netCDF interface, with the notable
 exception of support for operations that rename or delete existing objects.
```

### Comparing `h5netcdf-1.1.0/README.rst` & `h5netcdf-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,61 @@
+Metadata-Version: 2.1
+Name: h5netcdf
+Version: 1.2.0
+Summary: netCDF4 via h5py
+Author-email: Stephan Hoyer <shoyer@gmail.com>, Kai Mühlbauer <kmuehlbauer@wradlib.org>
+Maintainer-email: h5netcdf developers <devteam@h5netcdf.org>
+License: Copyright (c) 2015, h5netcdf developers
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors
+           may be used to endorse or promote products derived from this software
+           without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://h5netcdf.org
+Project-URL: documentation, https://h5netcdf.org
+Project-URL: repository, https://github.com/h5netcdf/h5netcdf
+Project-URL: changelog, https://github.com/h5netcdf/h5netcdf/blob/main/CHANGELOG.rst
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+License-File: LICENSE
+License-File: AUTHORS.txt
+
 h5netcdf
 ========
 
 .. image:: https://github.com/h5netcdf/h5netcdf/workflows/CI/badge.svg
     :target: https://github.com/h5netcdf/h5netcdf/actions
 .. image:: https://badge.fury.io/py/h5netcdf.svg
     :target: https://pypi.org/project/h5netcdf/
@@ -39,25 +93,30 @@
 .. _xarray: https://github.com/pydata/xarray/
 
 Install
 -------
 
 Ensure you have a recent version of h5py installed (I recommend using `conda`_ or
 the community effort `conda-forge`_).
-At least version 2.1 is required (for dimension scales); versions 2.3 and newer
-have been verified to work, though some tests only pass on h5py 2.6. Then::
+At least version 3.0 is required. Then::
 
     $ pip install h5netcdf
 
 Or if you are already using conda::
 
     $ conda install h5netcdf
 
+Note:
+
+From version 1.2. h5netcdf tries to align with a `nep29`_-like support policy with regard
+to it's upstream dependencies.
+
 .. _conda: https://conda.io/
 .. _conda-forge: https://conda-forge.org/
+.. _nep29: https://numpy.org/neps/nep-0029-deprecation_policy.html
 
 Usage
 -----
 
 h5netcdf has two APIs, a new API and a legacy API. Both interfaces currently
 reproduce most of the features of the netCDF interface, with the notable
 exception of support for operations that rename or delete existing objects.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `h5netcdf-1.1.0/doc/Makefile` & `h5netcdf-1.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `h5netcdf-1.1.0/doc/conf.py` & `h5netcdf-1.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     "sphinx.ext.mathjax",
     "sphinx.ext.todo",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.githubpages",
 ]
 
 extlinks = {
-    "issue": ("https://github.com/h5netcdf/h5netcdf/issues/%s", "GH"),
-    "pull": ("https://github.com/h5netcdf/h5netcdf/pull/%s", "PR"),
+    "issue": ("https://github.com/h5netcdf/h5netcdf/issues/%s", "GH%s"),
+    "pull": ("https://github.com/h5netcdf/h5netcdf/pull/%s", "PR%s"),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
```

### Comparing `h5netcdf-1.1.0/doc/devguide.rst` & `h5netcdf-1.2.0/doc/devguide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,17 @@
 
 Continuous Integration
 ----------------------
 
 ``h5netcdf`` uses GitHub Actions for Continuous Integration (CI). On every ``push`` to a repository branch
 or a PullRequest branch several checks are performed:
 
-- Lint checks (``flake8``, ``isort``, ``black``)
-- Unit tests with ``h5py2=2.10.0`` (Python 3.7, 3.8, 3.9) on Ubuntu
-- Unit tests with latest ``h5py3`` (Python 3.7, 3.8, 3.9, 3.10) on Ubuntu
-- Documentation build, artifacts are made availabe to download
+- Lint and style checks (``ruff``, ``black``)
+- Unit tests with latest ``h5py3`` (Python 3.9, 3.10, 3.11) facilitating GitHub Ubuntu worker
+- Documentation build, artifacts are made available to download
 - On release, source-tarball and universal wheel is uploaded to PyPI and documentation is made available
   on `h5netcdf GitHub Pages`_
 
 .. _h5netcdf GitHub Pages: https://h5netcdf.github.io/h5netcdf
 
 Documentation
 -------------
@@ -74,16 +73,16 @@
 1. Create release commit (can be done per PullRequest for more visibility)
     * versioning is done via `setuptools_scm`
     * update CHANGELOG.rst if necessary
     * add/update sections to README.rst (or documentation) if necessary
     * check all needed dependencies are listed in setup.py
 2. Create release
     * draft `new github release`_
-    * tag version (eg `v0.11.0`) `@ Target: main`
-    * set release title (eg. `release 0.11.0`)
+    * tag version (eg `v1.2.0`) `@ Target: main`
+    * set release title (eg. `release 1.2.0`)
     * add release description (eg. `bugfix-release`), tbd.
 
 This will start the CI workflow once again. The workflow creates `sdist` and universal `wheel` and uploads it to PyPI.
 
 .. _new github release: https://github.com/h5netcdf/h5netcdf/releases/new
 
 References
```

### Comparing `h5netcdf-1.1.0/doc/feature.rst` & `h5netcdf-1.2.0/doc/feature.rst`

 * *Files identical despite different names*

### Comparing `h5netcdf-1.1.0/doc/index.rst` & `h5netcdf-1.2.0/doc/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 .. include:: ../README.rst
    :start-after: .. why-h5netcdf
    :end-before:  .. changelog
 
 History
 -------
 
-The project was started in early 2015. The first commit was made on on 7th of April in 2015
+The project was started in early 2015. The first commit was made on 7th of April in 2015
 by Stephan Hoyer. The first `official` ``h5netcdf`` announcement was made by Stephan on the
 `xarray issue tracker`_ only one day later.
 
 The library evolved constantly over the years (fixing bugs and adding enhancements)
 and gained contributions from 15 other :ref:`contributors` so far. The library is widely used,
 especially as backend within `xarray`_.
```

### Comparing `h5netcdf-1.1.0/h5netcdf/attrs.py` & `h5netcdf-1.2.0/h5netcdf/attrs.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,10 +94,8 @@
                 yield key
 
     def __len__(self):
         hidden_count = sum(1 if attr in self._h5attrs else 0 for attr in _HIDDEN_ATTRS)
         return len(self._h5attrs) - hidden_count
 
     def __repr__(self):
-        return "\n".join(
-            ["%r" % type(self)] + ["%s: %r" % (k, v) for k, v in self.items()]
-        )
+        return "\n".join(["%r" % type(self)] + [f"{k}: {v!r}" for k, v in self.items()])
```

### Comparing `h5netcdf-1.1.0/h5netcdf/core.py` & `h5netcdf-1.2.0/h5netcdf/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     # slices to build resulting key
     k1 = slice(ellipsis)
     k2 = slice(len_key, None) if ellipsis is None else slice(ellipsis + 1, None)
     return key[k1] + res_dims + key[k2]
 
 
-class BaseVariable(object):
+class BaseVariable:
     def __init__(self, parent, name, dimensions=None):
         self._parent_ref = weakref.ref(parent)
         self._root_ref = weakref.ref(parent._root)
         self._h5path = _join_h5paths(parent.name, name)
         self._dimensions = dimensions
         self._initialized = True
 
@@ -169,19 +169,18 @@
         for axis, dim in enumerate(self._h5ds.dims):
             if len(dim):
                 name = _name_from_dimension(dim)
             else:
                 # if unlabeled dimensions are found
                 if self._root._phony_dims_mode is None:
                     raise ValueError(
-                        "variable %r has no dimension scale "
-                        "associated with axis %s. \n"
-                        "Use phony_dims=%r for sorted naming or "
-                        "phony_dims=%r for per access naming."
-                        % (self.name, axis, "sort", "access")
+                        f"variable {self.name!r} has no dimension scale "
+                        f"associated with axis {axis}. \n"
+                        f"Use phony_dims='sort' for sorted naming or "
+                        f"phony_dims='access' for per access naming."
                     )
                 else:
                     # get current dimension
                     dimsize = self._h5ds.shape[axis]
                     # get dimension names
                     dim_names = [
                         d.name
@@ -366,25 +365,25 @@
         )
 
     _cls_name = "h5netcdf.Variable"
 
     def __repr__(self):
         if self._parent._root._closed:
             return "<Closed %s>" % self._cls_name
-        header = "<%s %r: dimensions %s, shape %s, dtype %s>" % (
+        header = "<{} {!r}: dimensions {}, shape {}, dtype {}>".format(
             self._cls_name,
             self.name,
             self.dimensions,
             self.shape,
             self.dtype,
         )
         return "\n".join(
             [header]
             + ["Attributes:"]
-            + ["    %s: %r" % (k, v) for k, v in self.attrs.items()]
+            + [f"    {k}: {v!r}" for k, v in self.attrs.items()]
         )
 
 
 class Variable(BaseVariable):
     @property
     def chunks(self):
         return self._h5ds.chunks
@@ -455,16 +454,16 @@
         # either all dimensions have exactly one scale
         # or all dimensions have no scale
         if dimset ^ {0} == set():
             status = "unlabeled"
         elif dimset & {0}:
             name = h5py_dataset.name.split("/")[-1]
             raise ValueError(
-                "malformed variable {0} has mixing of labeled and "
-                "unlabeled dimensions.".format(name)
+                f"malformed variable {name} has mixing of labeled and "
+                "unlabeled dimensions."
             )
         else:
             status = "labeled"
 
     return status
 
 
@@ -531,15 +530,15 @@
             for size, cnt in phony_dims.items():
                 # only create missing dimensions
                 for pcnt in range(labeled_dims[size], cnt):
                     name = self._root._phony_dim_count
                     # for sort mode, we need to add precalculated max_dim_id + 1
                     if self._root._phony_dims_mode == "sort":
                         name += self._root._max_dim_id + 1
-                    name = "phony_dim_{}".format(name)
+                    name = f"phony_dim_{name}"
                     self._dimensions.add_phony(name, size)
 
         self._initialized = True
 
     @property
     def _root(self):
         return self._root_ref()
@@ -858,14 +857,16 @@
                 fillvalue,
                 chunks,
                 chunking_heuristic,
                 **kwargs,
             )
         # else split groups and iterate child groups
         keys = name.split("/")
+        if not keys[-1]:
+            raise ValueError("name parameter cannot be an empty string")
         group = self
         for k in keys[:-1]:
             group = group._require_child_group(k)
         return group._create_child_variable(
             keys[-1],
             dimensions,
             dtype,
@@ -929,38 +930,37 @@
 
     _cls_name = "h5netcdf.Group"
 
     def _repr_body(self):
         return (
             ["Dimensions:"]
             + [
-                "    %s: %s"
-                % (
+                "    {}: {}".format(
                     k,
-                    ("Unlimited (current: %s)" % self._dimensions[k].size)
+                    f"Unlimited (current: {self._dimensions[k].size})"
                     if v is None
                     else v,
                 )
                 for k, v in self.dimensions.items()
             ]
             + ["Groups:"]
-            + ["    %s" % g for g in self.groups]
+            + [f"    {g}" for g in self.groups]
             + ["Variables:"]
             + [
-                "    %s: %r %s" % (k, v.dimensions, v.dtype)
+                f"    {k}: {v.dimensions!r} {v.dtype}"
                 for k, v in self.variables.items()
             ]
             + ["Attributes:"]
-            + ["    %s: %r" % (k, v) for k, v in self.attrs.items()]
+            + [f"    {k}: {v!r}" for k, v in self.attrs.items()]
         )
 
     def __repr__(self):
         if self._root._closed:
-            return "<Closed %s>" % self._cls_name
-        header = "<%s %r (%s members)>" % (self._cls_name, self.name, len(self))
+            return f"<Closed {self._cls_name}>"
+        header = f"<{self._cls_name} {self.name!r} ({len(self)} members)>"
         return "\n".join([header] + self._repr_body())
 
     def resize_dimension(self, dim, size):
         """Resize a dimension to a certain size.
 
         It will pad with the underlying HDF5 data sets' fill values (usually
         zero) where necessary.
@@ -1022,52 +1022,45 @@
         # However, setting track_order to True helps with compatibility
         # with netcdf4-c and generally, keeping track of how things were added
         # to the dataset.
         # https://github.com/h5netcdf/h5netcdf/issues/136#issuecomment-1017457067
         track_order_default = version.parse(h5py.__version__) >= version.parse("3.7.0")
         track_order = kwargs.pop("track_order", track_order_default)
 
-        if version.parse(h5py.__version__) >= version.parse("3.0.0"):
-            self.decode_vlen_strings = kwargs.pop("decode_vlen_strings", None)
+        self.decode_vlen_strings = kwargs.pop("decode_vlen_strings", None)
         try:
             if isinstance(path, str):
                 if path.startswith(("http://", "https://", "hdf5://")):
                     if no_h5pyd:
                         raise ImportError(
                             "No module named 'h5pyd'. h5pyd is required for "
                             "opening urls: {}".format(path)
                         )
                     try:
                         with h5pyd.File(path, "r", **kwargs) as f:  # noqa
                             pass
                         self._preexisting_file = True
-                    except IOError:
+                    except OSError:
                         self._preexisting_file = False
                     self._h5py = h5pyd
                     self._h5file = self._h5py.File(
                         path, mode, track_order=track_order, **kwargs
                     )
                 else:
                     self._preexisting_file = os.path.exists(path) and mode != "w"
                     self._h5py = h5py
                     self._h5file = self._h5py.File(
                         path, mode, track_order=track_order, **kwargs
                     )
             else:  # file-like object
-                if version.parse(h5py.__version__) < version.parse("2.9.0"):
-                    raise TypeError(
-                        "h5py version ({}) must be greater than 2.9.0 to load "
-                        "file-like objects.".format(h5py.__version__)
-                    )
-                else:
-                    self._preexisting_file = mode in {"r", "r+", "a"}
-                    self._h5py = h5py
-                    self._h5file = self._h5py.File(
-                        path, mode, track_order=track_order, **kwargs
-                    )
+                self._preexisting_file = mode in {"r", "r+", "a"}
+                self._h5py = h5py
+                self._h5file = self._h5py.File(
+                    path, mode, track_order=track_order, **kwargs
+                )
         except Exception:
             self._closed = True
             raise
         else:
             self._closed = False
 
         self._mode = mode
@@ -1078,38 +1071,36 @@
 
         # phony dimension handling
         self._phony_dims_mode = phony_dims
         if phony_dims is not None:
             self._phony_dim_count = 0
             if phony_dims not in ["sort", "access"]:
                 raise ValueError(
-                    "unknown value %r for phony_dims\n"
-                    "Use phony_dims=%r for sorted naming, "
-                    "phony_dims=%r for per access naming."
-                    % (phony_dims, "sort", "access")
+                    f"unknown value {phony_dims!r} for phony_dims\n"
+                    "Use phony_dims='sort' for sorted naming, "
+                    "phony_dims='access' for per access naming."
                 )
 
         # string decoding
-        if version.parse(h5py.__version__) >= version.parse("3.0.0"):
-            if "legacy" in self._cls_name:
-                if self.decode_vlen_strings is not None:
-                    msg = (
-                        "'decode_vlen_strings' keyword argument is not allowed in h5netcdf "
-                        "legacy API."
-                    )
-                    raise TypeError(msg)
-                self.decode_vlen_strings = True
-            else:
-                if self.decode_vlen_strings is None:
-                    self.decode_vlen_strings = False
+        if "legacy" in self._cls_name:
+            if self.decode_vlen_strings is not None:
+                msg = (
+                    "'decode_vlen_strings' keyword argument is not allowed in h5netcdf "
+                    "legacy API."
+                )
+                raise TypeError(msg)
+            self.decode_vlen_strings = True
+        else:
+            if self.decode_vlen_strings is None:
+                self.decode_vlen_strings = False
 
         self._max_dim_id = -1
         # This maps keeps track of all HDF5 datasets corresponding to this group.
         self._all_h5groups = ChainMap(self._h5group)
-        super(File, self).__init__(self, self._h5path)
+        super().__init__(self, self._h5path)
         # get maximum dimension id and count of labeled dimensions
         if self._writable:
             self._max_dim_id = self._get_maximum_dimension_id()
         # initialize all groups to detect/create phony dimensions
         # mimics netcdf-c style naming
         if phony_dims == "sort":
             self._determine_phony_dimensions()
@@ -1146,15 +1137,15 @@
         elif h5py.check_dtype(vlen=dtype) not in {None, str, bytes}:
             description = "non-string variable length"
         else:
             description = None
 
         if description is not None:
             _invalid_netcdf_feature(
-                "{} dtypes".format(description),
+                f"{description} dtypes",
                 self.invalid_netcdf,
             )
 
     @property
     def mode(self):
         return self._h5file.mode
 
@@ -1170,15 +1161,15 @@
     def _root(self):
         return self
 
     def flush(self):
         if self._writable:
             # only write `_NCProperties` in newly created files
             if not self._preexisting_file and not self.invalid_netcdf:
-                _NC_PROPERTIES = "version=2,h5netcdf=%s,hdf5=%s,%s=%s" % (
+                _NC_PROPERTIES = "version=2,h5netcdf={},hdf5={},{}={}".format(
                     __version__,
                     self._h5py.version.hdf5_version,
                     self._h5py.__name__,
                     self._h5py.__version__,
                 )
                 self.attrs._h5attrs["_NCProperties"] = np.array(
                     _NC_PROPERTIES,
@@ -1218,15 +1209,15 @@
         self.close()
 
     _cls_name = "h5netcdf.File"
 
     def __repr__(self):
         if self._closed:
             return "<Closed %s>" % self._cls_name
-        header = "<%s %r (mode %s)>" % (
+        header = "<{} {!r} (mode {})>".format(
             self._cls_name,
             self.filename.split("/")[-1],
             self.mode,
         )
         return "\n".join([header] + self._repr_body())
```

### Comparing `h5netcdf-1.1.0/h5netcdf/dimensions.py` & `h5netcdf-1.2.0/h5netcdf/dimensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import weakref
 from collections import OrderedDict
 from collections.abc import MutableMapping
 
 import h5py
 import numpy as np
-from packaging.version import Version
 
 
 class Dimensions(MutableMapping):
     def __init__(self, group):
         self._group_ref = weakref.ref(group)
         self._objects = OrderedDict()
 
@@ -37,33 +36,32 @@
         # adding dimensions which are already created in the file
         self._objects[name] = Dimension(self._group, name)
 
     def __delitem__(self, key):
         raise NotImplementedError("cannot yet delete dimensions")
 
     def __iter__(self):
-        for key in self._objects:
-            yield key
+        yield from self._objects
 
     def __len__(self):
         return len(self._objects)
 
     def __repr__(self):
         if self._group._root._closed:
             return "<Closed h5netcdf.Dimensions>"
         return "<h5netcdf.Dimensions: %s>" % ", ".join(
-            "%s=%r" % (k, v) for k, v in self._objects.items()
+            f"{k}={v!r}" for k, v in self._objects.items()
         )
 
 
 def _join_h5paths(parent_path, child_path):
     return "/".join([parent_path.rstrip("/"), child_path.lstrip("/")])
 
 
-class Dimension(object):
+class Dimension:
     def __init__(self, parent, name, size=None, create_h5ds=False, phony=False):
         """NetCDF4 Dimension constructor.
 
         Parameters
         ----------
         parent: h5netcdf.Group
             Parent group.
@@ -205,18 +203,15 @@
         scale_name = (
             self.name
             if self.name in self._parent._variables
             else NOT_A_VARIABLE + dimlen
         )
         # don't re-create scales if they already exist.
         if not self._root._h5py.h5ds.is_scale(self._h5ds.id):
-            if Version(h5py.__version__) < Version("2.10.0"):
-                self._h5ds.dims.create_scale(self._h5ds, scale_name)
-            else:
-                self._h5ds.make_scale(scale_name)
+            self._h5ds.make_scale(scale_name)
 
     def _attach_scale(self, refs):
         """Attach dimension scale to references"""
         for var, dim in refs:
             self._parent._all_h5groups[var].dims[dim].attach_scale(self._h5ds)
 
     def _detach_scale(self):
@@ -241,9 +236,9 @@
         if not self._phony and self._parent._root._closed:
             return "<Closed %s>" % self._cls_name
         special = ""
         if self._phony:
             special += " (phony_dim)"
         if self.isunlimited():
             special += " (unlimited)"
-        header = "<%s %r: size %s%s>" % (self._cls_name, self.name, self.size, special)
+        header = f"<{self._cls_name} {self.name!r}: size {self.size}{special}>"
         return "\n".join([header])
```

### Comparing `h5netcdf-1.1.0/h5netcdf/legacyapi.py` & `h5netcdf-1.2.0/h5netcdf/legacyapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         raise ValueError(
             "'endian' keyword argument must be 'little','big' or 'native', got '%s'"
             % endian
         )
     return endianess
 
 
-class HasAttributesMixin(object):
+class HasAttributesMixin:
     _initialized = False
 
     def getncattr(self, name):
         """Retrieve a netCDF4 attribute."""
         return self.attrs[name]
 
     def setncattr(self, name, value):
@@ -63,15 +63,15 @@
         return list(self.attrs)
 
     def __getattr__(self, name):
         try:
             return self.attrs[name]
         except KeyError:
             raise AttributeError(
-                "NetCDF: attribute {0}:{1} not found".format(type(self).__name__, name)
+                f"NetCDF: attribute {type(self).__name__}:{name} not found"
             )
 
     def __setattr__(self, name, value):
         if self._initialized and name not in self.__dict__:
             self.attrs[name] = value
         else:
             object.__setattr__(self, name, value)
@@ -217,15 +217,15 @@
             dtype = np.dtype(datatype)
             if dtype.byteorder != "|":
                 datatype = dtype.newbyteorder("S")
 
         # closer to netCDF4 chunking behavior
         kwds["chunking_heuristic"] = "h5netcdf"
 
-        return super(Group, self).create_variable(
+        return super().create_variable(
             varname,
             dimensions,
             dtype=datatype,
             fletcher32=fletcher32,
             chunks=chunksizes,
             fillvalue=fill_value,
             **kwds,
```

### Comparing `h5netcdf-1.1.0/h5netcdf/tests/conftest.py` & `h5netcdf-1.2.0/h5netcdf/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,23 @@
         rmtree(hsds_root)
 
     old_sysargv = sys.argv
     sys.argv = [""]
     sys.argv.extend(["-e", os.environ["HS_ENDPOINT"]])
     sys.argv.extend(["-u", "admin"])
     sys.argv.extend(["-p", "admin"])
-    sys.argv.extend(["-b", os.environ["BUCKET_NAME"]])
+    sys.argv.extend(["--bucket", os.environ["BUCKET_NAME"]])
     sys.argv.append("/home/")
     hstouch()
 
     sys.argv = [""]
     sys.argv.extend(["-e", os.environ["HS_ENDPOINT"]])
     sys.argv.extend(["-u", "admin"])
     sys.argv.extend(["-p", "admin"])
-    sys.argv.extend(["-b", os.environ["BUCKET_NAME"]])
+    sys.argv.extend(["--bucket", os.environ["BUCKET_NAME"]])
     sys.argv.extend(["-o", os.environ["HS_USERNAME"]])
     sys.argv.append(f'/home/{os.environ["HS_USERNAME"]}/')
     hstouch()
     sys.argv = old_sysargv
 
 
 @pytest.fixture(scope="session")
```

### Comparing `h5netcdf-1.1.0/h5netcdf/tests/test_h5netcdf.py` & `h5netcdf-1.2.0/h5netcdf/tests/test_h5netcdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,5199 +74,5189 @@
 00000490: 2020 7265 7475 726e 2073 7472 2874 6d70    return str(tmp
 000004a0: 6469 722e 6a6f 696e 2872 6571 7565 7374  dir.join(request
 000004b0: 2e70 6172 616d 2929 0a0a 0a40 7079 7465  .param))...@pyte
 000004c0: 7374 2e66 6978 7475 7265 2870 6172 616d  st.fixture(param
 000004d0: 733d 5b54 7275 652c 2046 616c 7365 5d29  s=[True, False])
 000004e0: 0a64 6566 2064 6563 6f64 655f 766c 656e  .def decode_vlen
 000004f0: 5f73 7472 696e 6773 2872 6571 7565 7374  _strings(request
-00000500: 293a 0a20 2020 2069 6620 7665 7273 696f  ):.    if versio
-00000510: 6e2e 7061 7273 6528 6835 7079 2e5f 5f76  n.parse(h5py.__v
-00000520: 6572 7369 6f6e 5f5f 2920 3e3d 2076 6572  ersion__) >= ver
-00000530: 7369 6f6e 2e70 6172 7365 2822 332e 302e  sion.parse("3.0.
-00000540: 3022 293a 0a20 2020 2020 2020 2072 6574  0"):.        ret
-00000550: 7572 6e20 6469 6374 2864 6563 6f64 655f  urn dict(decode_
-00000560: 766c 656e 5f73 7472 696e 6773 3d72 6571  vlen_strings=req
-00000570: 7565 7374 2e70 6172 616d 290a 2020 2020  uest.param).    
-00000580: 656c 7365 3a0a 2020 2020 2020 2020 7265  else:.        re
-00000590: 7475 726e 207b 7d0a 0a0a 4070 7974 6573  turn {}...@pytes
-000005a0: 742e 6669 7874 7572 6528 7061 7261 6d73  t.fixture(params
-000005b0: 3d5b 6e65 7443 4446 342c 206c 6567 6163  =[netCDF4, legac
-000005c0: 7961 7069 5d29 0a64 6566 206e 6574 6364  yapi]).def netcd
-000005d0: 665f 7772 6974 655f 6d6f 6475 6c65 2872  f_write_module(r
-000005e0: 6571 7565 7374 293a 0a20 2020 2072 6574  equest):.    ret
-000005f0: 7572 6e20 7265 7175 6573 742e 7061 7261  urn request.para
-00000600: 6d0a 0a0a 6465 6620 6765 745f 6864 6635  m...def get_hdf5
-00000610: 5f6d 6f64 756c 6528 7265 736f 7572 6365  _module(resource
-00000620: 293a 0a20 2020 2022 2222 5265 7475 726e  ):.    """Return
-00000630: 2074 6865 2063 6f72 7265 6374 2068 3570   the correct h5p
-00000640: 7920 6d6f 6475 6c65 2062 6173 6564 206f  y module based o
-00000650: 6e20 7468 6520 696e 7075 7420 7265 736f  n the input reso
-00000660: 7572 6365 2e22 2222 0a20 2020 2069 6620  urce.""".    if 
-00000670: 6973 696e 7374 616e 6365 2872 6573 6f75  isinstance(resou
-00000680: 7263 652c 2073 7472 2920 616e 6420 7265  rce, str) and re
-00000690: 736f 7572 6365 2e73 7461 7274 7377 6974  source.startswit
-000006a0: 6828 7265 6d6f 7465 5f68 3529 3a0a 2020  h(remote_h5):.  
-000006b0: 2020 2020 2020 7265 7475 726e 2068 3570        return h5p
-000006c0: 7964 0a20 2020 2065 6c73 653a 0a20 2020  yd.    else:.   
-000006d0: 2020 2020 2072 6574 7572 6e20 6835 7079       return h5py
-000006e0: 0a0a 0a64 6566 2073 7472 696e 675f 746f  ...def string_to
-000006f0: 5f63 6861 7228 6172 7229 3a0a 2020 2020  _char(arr):.    
-00000700: 2222 224c 696b 6520 6e63 342e 7374 7269  """Like nc4.stri
-00000710: 6e67 746f 6368 6172 2c20 6275 7420 6661  ngtochar, but fa
-00000720: 7374 6572 2061 6e64 206d 6f72 6520 666c  ster and more fl
-00000730: 6578 6962 6c65 2e22 2222 0a20 2020 2023  exible.""".    #
-00000740: 2065 6e73 7572 6520 7468 6520 6172 7261   ensure the arra
-00000750: 7920 6973 2063 6f6e 7469 6775 6f75 730a  y is contiguous.
-00000760: 2020 2020 6172 7220 3d20 6e70 2e61 7272      arr = np.arr
-00000770: 6179 2861 7272 2c20 636f 7079 3d46 616c  ay(arr, copy=Fal
-00000780: 7365 2c20 6f72 6465 723d 2243 2229 0a20  se, order="C"). 
-00000790: 2020 206b 696e 6420 3d20 6172 722e 6474     kind = arr.dt
-000007a0: 7970 652e 6b69 6e64 0a20 2020 2069 6620  ype.kind.    if 
-000007b0: 6b69 6e64 206e 6f74 2069 6e20 5b22 5522  kind not in ["U"
-000007c0: 2c20 2253 225d 3a0a 2020 2020 2020 2020  , "S"]:.        
-000007d0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-000007e0: 2822 6172 6775 6d65 6e74 206d 7573 7420  ("argument must 
-000007f0: 6265 2061 2073 7472 696e 6722 290a 2020  be a string").  
-00000800: 2020 7265 7475 726e 2061 7272 2e72 6573    return arr.res
-00000810: 6861 7065 2861 7272 2e73 6861 7065 202b  hape(arr.shape +
-00000820: 2028 312c 2929 2e76 6965 7728 6b69 6e64   (1,)).view(kind
-00000830: 202b 2022 3122 290a 0a0a 6465 6620 6172   + "1")...def ar
-00000840: 7261 795f 6571 7561 6c28 612c 2062 293a  ray_equal(a, b):
-00000850: 0a20 2020 2061 2c20 6220 3d20 6d61 7028  .    a, b = map(
-00000860: 6e70 2e61 7272 6179 2c20 2861 5b2e 2e2e  np.array, (a[...
-00000870: 5d2c 2062 5b2e 2e2e 5d29 290a 2020 2020  ], b[...])).    
-00000880: 6966 2061 2e73 6861 7065 2021 3d20 622e  if a.shape != b.
-00000890: 7368 6170 653a 0a20 2020 2020 2020 2072  shape:.        r
-000008a0: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
-000008b0: 7472 793a 0a20 2020 2020 2020 2072 6574  try:.        ret
-000008c0: 7572 6e20 6e70 2e61 6c6c 636c 6f73 6528  urn np.allclose(
-000008d0: 612c 2062 290a 2020 2020 6578 6365 7074  a, b).    except
-000008e0: 2054 7970 6545 7272 6f72 3a0a 2020 2020   TypeError:.    
-000008f0: 2020 2020 7265 7475 726e 2028 6120 3d3d      return (a ==
-00000900: 2062 292e 616c 6c28 290a 0a0a 5f63 6861   b).all()..._cha
-00000910: 725f 6172 7261 7920 3d20 7374 7269 6e67  r_array = string
-00000920: 5f74 6f5f 6368 6172 286e 702e 6172 7261  _to_char(np.arra
-00000930: 7928 5b22 6122 2c20 2262 222c 2022 6322  y(["a", "b", "c"
-00000940: 2c20 2266 6f6f 222c 2022 6261 7222 2c20  , "foo", "bar", 
-00000950: 2262 617a 225d 2c20 6474 7970 653d 2253  "baz"], dtype="S
-00000960: 2229 290a 0a5f 7374 7269 6e67 5f61 7272  ")).._string_arr
-00000970: 6179 203d 206e 702e 6172 7261 7928 0a20  ay = np.array(. 
-00000980: 2020 205b 5b22 666f 6f62 6172 3022 2c20     [["foobar0", 
-00000990: 2266 6f6f 6261 7231 222c 2022 666f 6f62  "foobar1", "foob
-000009a0: 6172 3322 5d2c 205b 2266 6f6f 666f 6f66  ar3"], ["foofoof
-000009b0: 6f6f 222c 2022 666f 6f66 6f6f 6261 7222  oo", "foofoobar"
-000009c0: 2c20 2266 6f6f 6261 7262 6172 225d 5d0a  , "foobarbar"]].
-000009d0: 290a 0a5f 766c 656e 5f73 7472 696e 6720  ).._vlen_string 
-000009e0: 3d20 2266 6f6f 220a 0a0a 6465 6620 6973  = "foo"...def is
-000009f0: 5f68 3570 795f 6368 6172 5f77 6f72 6b69  _h5py_char_worki
-00000a00: 6e67 2874 6d70 5f6e 6574 6364 662c 206e  ng(tmp_netcdf, n
-00000a10: 616d 6529 3a0a 2020 2020 6835 203d 2067  ame):.    h5 = g
-00000a20: 6574 5f68 6466 355f 6d6f 6475 6c65 2874  et_hdf5_module(t
-00000a30: 6d70 5f6e 6574 6364 6629 0a20 2020 2023  mp_netcdf).    #
-00000a40: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000a50: 636f 6d2f 556e 6964 6174 612f 6e65 7463  com/Unidata/netc
-00000a60: 6466 2d63 2f69 7373 7565 732f 3239 380a  df-c/issues/298.
-00000a70: 2020 2020 7769 7468 2068 352e 4669 6c65      with h5.File
-00000a80: 2874 6d70 5f6e 6574 6364 662c 2022 7222  (tmp_netcdf, "r"
-00000a90: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-00000aa0: 2076 203d 2064 735b 6e61 6d65 5d0a 2020   v = ds[name].  
-00000ab0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00000ac0: 2020 2020 2020 2061 7373 6572 7420 6172         assert ar
-00000ad0: 7261 795f 6571 7561 6c28 762c 205f 6368  ray_equal(v, _ch
-00000ae0: 6172 5f61 7272 6179 290a 2020 2020 2020  ar_array).      
-00000af0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00000b00: 650a 2020 2020 2020 2020 6578 6365 7074  e.        except
-00000b10: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00000b20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000b30: 7265 2e6d 6174 6368 2822 5e43 616e 2774  re.match("^Can't
-00000b40: 2072 6561 6420 6461 7461 222c 2065 2e61   read data", e.a
-00000b50: 7267 735b 305d 293a 0a20 2020 2020 2020  rgs[0]):.       
-00000b60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000b70: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00000b80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00000b90: 2020 2020 2020 2020 7261 6973 650a 0a0a          raise...
-00000ba0: 6465 6620 7772 6974 655f 6c65 6761 6379  def write_legacy
-00000bb0: 5f6e 6574 6364 6628 746d 705f 6e65 7463  _netcdf(tmp_netc
-00000bc0: 6466 2c20 7772 6974 655f 6d6f 6475 6c65  df, write_module
-00000bd0: 293a 0a20 2020 2064 7320 3d20 7772 6974  ):.    ds = writ
-00000be0: 655f 6d6f 6475 6c65 2e44 6174 6173 6574  e_module.Dataset
-00000bf0: 2874 6d70 5f6e 6574 6364 662c 2022 7722  (tmp_netcdf, "w"
-00000c00: 290a 2020 2020 6473 2e73 6574 6e63 6174  ).    ds.setncat
-00000c10: 7472 2822 676c 6f62 616c 222c 2034 3229  tr("global", 42)
-00000c20: 0a20 2020 2064 732e 6f74 6865 725f 6174  .    ds.other_at
-00000c30: 7472 203d 2022 7965 7322 0a20 2020 2064  tr = "yes".    d
-00000c40: 732e 6372 6561 7465 4469 6d65 6e73 696f  s.createDimensio
-00000c50: 6e28 2278 222c 2034 290a 2020 2020 6473  n("x", 4).    ds
-00000c60: 2e63 7265 6174 6544 696d 656e 7369 6f6e  .createDimension
-00000c70: 2822 7922 2c20 3529 0a20 2020 2064 732e  ("y", 5).    ds.
-00000c80: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
-00000c90: 227a 222c 2036 290a 2020 2020 6473 2e63  "z", 6).    ds.c
-00000ca0: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
-00000cb0: 656d 7074 7922 2c20 3029 0a20 2020 2064  empty", 0).    d
-00000cc0: 732e 6372 6561 7465 4469 6d65 6e73 696f  s.createDimensio
-00000cd0: 6e28 2273 7472 696e 6733 222c 2033 290a  n("string3", 3).
-00000ce0: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-00000cf0: 656e 7369 6f6e 2822 756e 6c69 6d69 7465  ension("unlimite
-00000d00: 6422 2c20 4e6f 6e65 290a 0a20 2020 2076  d", None)..    v
-00000d10: 203d 2064 732e 6372 6561 7465 5661 7269   = ds.createVari
-00000d20: 6162 6c65 2822 666f 6f22 2c20 666c 6f61  able("foo", floa
-00000d30: 742c 2028 2278 222c 2022 7922 292c 2063  t, ("x", "y"), c
-00000d40: 6875 6e6b 7369 7a65 733d 2834 2c20 3529  hunksizes=(4, 5)
-00000d50: 2c20 7a6c 6962 3d54 7275 6529 0a20 2020  , zlib=True).   
-00000d60: 2076 5b2e 2e2e 5d20 3d20 310a 2020 2020   v[...] = 1.    
-00000d70: 762e 7365 746e 6361 7474 7228 2275 6e69  v.setncattr("uni
-00000d80: 7473 222c 2022 6d65 7465 7273 2229 0a0a  ts", "meters")..
-00000d90: 2020 2020 7620 3d20 6473 2e63 7265 6174      v = ds.creat
-00000da0: 6556 6172 6961 626c 6528 2279 222c 2069  eVariable("y", i
-00000db0: 6e74 2c20 2822 7922 2c29 2c20 6669 6c6c  nt, ("y",), fill
-00000dc0: 5f76 616c 7565 3d2d 3129 0a20 2020 2076  _value=-1).    v
-00000dd0: 5b3a 345d 203d 206e 702e 6172 616e 6765  [:4] = np.arange
-00000de0: 2834 290a 0a20 2020 2076 203d 2064 732e  (4)..    v = ds.
+00000500: 293a 0a20 2020 2072 6574 7572 6e20 6469  ):.    return di
+00000510: 6374 2864 6563 6f64 655f 766c 656e 5f73  ct(decode_vlen_s
+00000520: 7472 696e 6773 3d72 6571 7565 7374 2e70  trings=request.p
+00000530: 6172 616d 290a 0a0a 4070 7974 6573 742e  aram)...@pytest.
+00000540: 6669 7874 7572 6528 7061 7261 6d73 3d5b  fixture(params=[
+00000550: 6e65 7443 4446 342c 206c 6567 6163 7961  netCDF4, legacya
+00000560: 7069 5d29 0a64 6566 206e 6574 6364 665f  pi]).def netcdf_
+00000570: 7772 6974 655f 6d6f 6475 6c65 2872 6571  write_module(req
+00000580: 7565 7374 293a 0a20 2020 2072 6574 7572  uest):.    retur
+00000590: 6e20 7265 7175 6573 742e 7061 7261 6d0a  n request.param.
+000005a0: 0a0a 6465 6620 6765 745f 6864 6635 5f6d  ..def get_hdf5_m
+000005b0: 6f64 756c 6528 7265 736f 7572 6365 293a  odule(resource):
+000005c0: 0a20 2020 2022 2222 5265 7475 726e 2074  .    """Return t
+000005d0: 6865 2063 6f72 7265 6374 2068 3570 7920  he correct h5py 
+000005e0: 6d6f 6475 6c65 2062 6173 6564 206f 6e20  module based on 
+000005f0: 7468 6520 696e 7075 7420 7265 736f 7572  the input resour
+00000600: 6365 2e22 2222 0a20 2020 2069 6620 6973  ce.""".    if is
+00000610: 696e 7374 616e 6365 2872 6573 6f75 7263  instance(resourc
+00000620: 652c 2073 7472 2920 616e 6420 7265 736f  e, str) and reso
+00000630: 7572 6365 2e73 7461 7274 7377 6974 6828  urce.startswith(
+00000640: 7265 6d6f 7465 5f68 3529 3a0a 2020 2020  remote_h5):.    
+00000650: 2020 2020 7265 7475 726e 2068 3570 7964      return h5pyd
+00000660: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00000670: 2020 2072 6574 7572 6e20 6835 7079 0a0a     return h5py..
+00000680: 0a64 6566 2073 7472 696e 675f 746f 5f63  .def string_to_c
+00000690: 6861 7228 6172 7229 3a0a 2020 2020 2222  har(arr):.    ""
+000006a0: 224c 696b 6520 6e63 342e 7374 7269 6e67  "Like nc4.string
+000006b0: 746f 6368 6172 2c20 6275 7420 6661 7374  tochar, but fast
+000006c0: 6572 2061 6e64 206d 6f72 6520 666c 6578  er and more flex
+000006d0: 6962 6c65 2e22 2222 0a20 2020 2023 2065  ible.""".    # e
+000006e0: 6e73 7572 6520 7468 6520 6172 7261 7920  nsure the array 
+000006f0: 6973 2063 6f6e 7469 6775 6f75 730a 2020  is contiguous.  
+00000700: 2020 6172 7220 3d20 6e70 2e61 7272 6179    arr = np.array
+00000710: 2861 7272 2c20 636f 7079 3d46 616c 7365  (arr, copy=False
+00000720: 2c20 6f72 6465 723d 2243 2229 0a20 2020  , order="C").   
+00000730: 206b 696e 6420 3d20 6172 722e 6474 7970   kind = arr.dtyp
+00000740: 652e 6b69 6e64 0a20 2020 2069 6620 6b69  e.kind.    if ki
+00000750: 6e64 206e 6f74 2069 6e20 5b22 5522 2c20  nd not in ["U", 
+00000760: 2253 225d 3a0a 2020 2020 2020 2020 7261  "S"]:.        ra
+00000770: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00000780: 6172 6775 6d65 6e74 206d 7573 7420 6265  argument must be
+00000790: 2061 2073 7472 696e 6722 290a 2020 2020   a string").    
+000007a0: 7265 7475 726e 2061 7272 2e72 6573 6861  return arr.resha
+000007b0: 7065 2861 7272 2e73 6861 7065 202b 2028  pe(arr.shape + (
+000007c0: 312c 2929 2e76 6965 7728 6b69 6e64 202b  1,)).view(kind +
+000007d0: 2022 3122 290a 0a0a 6465 6620 6172 7261   "1")...def arra
+000007e0: 795f 6571 7561 6c28 612c 2062 293a 0a20  y_equal(a, b):. 
+000007f0: 2020 2061 2c20 6220 3d20 6d61 7028 6e70     a, b = map(np
+00000800: 2e61 7272 6179 2c20 2861 5b2e 2e2e 5d2c  .array, (a[...],
+00000810: 2062 5b2e 2e2e 5d29 290a 2020 2020 6966   b[...])).    if
+00000820: 2061 2e73 6861 7065 2021 3d20 622e 7368   a.shape != b.sh
+00000830: 6170 653a 0a20 2020 2020 2020 2072 6574  ape:.        ret
+00000840: 7572 6e20 4661 6c73 650a 2020 2020 7472  urn False.    tr
+00000850: 793a 0a20 2020 2020 2020 2072 6574 7572  y:.        retur
+00000860: 6e20 6e70 2e61 6c6c 636c 6f73 6528 612c  n np.allclose(a,
+00000870: 2062 290a 2020 2020 6578 6365 7074 2054   b).    except T
+00000880: 7970 6545 7272 6f72 3a0a 2020 2020 2020  ypeError:.      
+00000890: 2020 7265 7475 726e 2028 6120 3d3d 2062    return (a == b
+000008a0: 292e 616c 6c28 290a 0a0a 5f63 6861 725f  ).all()..._char_
+000008b0: 6172 7261 7920 3d20 7374 7269 6e67 5f74  array = string_t
+000008c0: 6f5f 6368 6172 286e 702e 6172 7261 7928  o_char(np.array(
+000008d0: 5b22 6122 2c20 2262 222c 2022 6322 2c20  ["a", "b", "c", 
+000008e0: 2266 6f6f 222c 2022 6261 7222 2c20 2262  "foo", "bar", "b
+000008f0: 617a 225d 2c20 6474 7970 653d 2253 2229  az"], dtype="S")
+00000900: 290a 0a5f 7374 7269 6e67 5f61 7272 6179  ).._string_array
+00000910: 203d 206e 702e 6172 7261 7928 0a20 2020   = np.array(.   
+00000920: 205b 5b22 666f 6f62 6172 3022 2c20 2266   [["foobar0", "f
+00000930: 6f6f 6261 7231 222c 2022 666f 6f62 6172  oobar1", "foobar
+00000940: 3322 5d2c 205b 2266 6f6f 666f 6f66 6f6f  3"], ["foofoofoo
+00000950: 222c 2022 666f 6f66 6f6f 6261 7222 2c20  ", "foofoobar", 
+00000960: 2266 6f6f 6261 7262 6172 225d 5d0a 290a  "foobarbar"]].).
+00000970: 0a5f 766c 656e 5f73 7472 696e 6720 3d20  ._vlen_string = 
+00000980: 2266 6f6f 220a 0a0a 6465 6620 6973 5f68  "foo"...def is_h
+00000990: 3570 795f 6368 6172 5f77 6f72 6b69 6e67  5py_char_working
+000009a0: 2874 6d70 5f6e 6574 6364 662c 206e 616d  (tmp_netcdf, nam
+000009b0: 6529 3a0a 2020 2020 6835 203d 2067 6574  e):.    h5 = get
+000009c0: 5f68 6466 355f 6d6f 6475 6c65 2874 6d70  _hdf5_module(tmp
+000009d0: 5f6e 6574 6364 6629 0a20 2020 2023 2068  _netcdf).    # h
+000009e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000009f0: 6d2f 556e 6964 6174 612f 6e65 7463 6466  m/Unidata/netcdf
+00000a00: 2d63 2f69 7373 7565 732f 3239 380a 2020  -c/issues/298.  
+00000a10: 2020 7769 7468 2068 352e 4669 6c65 2874    with h5.File(t
+00000a20: 6d70 5f6e 6574 6364 662c 2022 7222 2920  mp_netcdf, "r") 
+00000a30: 6173 2064 733a 0a20 2020 2020 2020 2076  as ds:.        v
+00000a40: 203d 2064 735b 6e61 6d65 5d0a 2020 2020   = ds[name].    
+00000a50: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00000a60: 2020 2020 2061 7373 6572 7420 6172 7261       assert arra
+00000a70: 795f 6571 7561 6c28 762c 205f 6368 6172  y_equal(v, _char
+00000a80: 5f61 7272 6179 290a 2020 2020 2020 2020  _array).        
+00000a90: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00000aa0: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00000ab0: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+00000ac0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+00000ad0: 2e6d 6174 6368 2822 5e43 616e 2774 2072  .match("^Can't r
+00000ae0: 6561 6420 6461 7461 222c 2065 2e61 7267  ead data", e.arg
+00000af0: 735b 305d 293a 0a20 2020 2020 2020 2020  s[0]):.         
+00000b00: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00000b10: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00000b20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00000b30: 2020 2020 2020 7261 6973 650a 0a0a 6465        raise...de
+00000b40: 6620 7772 6974 655f 6c65 6761 6379 5f6e  f write_legacy_n
+00000b50: 6574 6364 6628 746d 705f 6e65 7463 6466  etcdf(tmp_netcdf
+00000b60: 2c20 7772 6974 655f 6d6f 6475 6c65 293a  , write_module):
+00000b70: 0a20 2020 2064 7320 3d20 7772 6974 655f  .    ds = write_
+00000b80: 6d6f 6475 6c65 2e44 6174 6173 6574 2874  module.Dataset(t
+00000b90: 6d70 5f6e 6574 6364 662c 2022 7722 290a  mp_netcdf, "w").
+00000ba0: 2020 2020 6473 2e73 6574 6e63 6174 7472      ds.setncattr
+00000bb0: 2822 676c 6f62 616c 222c 2034 3229 0a20  ("global", 42). 
+00000bc0: 2020 2064 732e 6f74 6865 725f 6174 7472     ds.other_attr
+00000bd0: 203d 2022 7965 7322 0a20 2020 2064 732e   = "yes".    ds.
+00000be0: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+00000bf0: 2278 222c 2034 290a 2020 2020 6473 2e63  "x", 4).    ds.c
+00000c00: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
+00000c10: 7922 2c20 3529 0a20 2020 2064 732e 6372  y", 5).    ds.cr
+00000c20: 6561 7465 4469 6d65 6e73 696f 6e28 227a  eateDimension("z
+00000c30: 222c 2036 290a 2020 2020 6473 2e63 7265  ", 6).    ds.cre
+00000c40: 6174 6544 696d 656e 7369 6f6e 2822 656d  ateDimension("em
+00000c50: 7074 7922 2c20 3029 0a20 2020 2064 732e  pty", 0).    ds.
+00000c60: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+00000c70: 2273 7472 696e 6733 222c 2033 290a 2020  "string3", 3).  
+00000c80: 2020 6473 2e63 7265 6174 6544 696d 656e    ds.createDimen
+00000c90: 7369 6f6e 2822 756e 6c69 6d69 7465 6422  sion("unlimited"
+00000ca0: 2c20 4e6f 6e65 290a 0a20 2020 2076 203d  , None)..    v =
+00000cb0: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
+00000cc0: 6c65 2822 666f 6f22 2c20 666c 6f61 742c  le("foo", float,
+00000cd0: 2028 2278 222c 2022 7922 292c 2063 6875   ("x", "y"), chu
+00000ce0: 6e6b 7369 7a65 733d 2834 2c20 3529 2c20  nksizes=(4, 5), 
+00000cf0: 7a6c 6962 3d54 7275 6529 0a20 2020 2076  zlib=True).    v
+00000d00: 5b2e 2e2e 5d20 3d20 310a 2020 2020 762e  [...] = 1.    v.
+00000d10: 7365 746e 6361 7474 7228 2275 6e69 7473  setncattr("units
+00000d20: 222c 2022 6d65 7465 7273 2229 0a0a 2020  ", "meters")..  
+00000d30: 2020 7620 3d20 6473 2e63 7265 6174 6556    v = ds.createV
+00000d40: 6172 6961 626c 6528 2279 222c 2069 6e74  ariable("y", int
+00000d50: 2c20 2822 7922 2c29 2c20 6669 6c6c 5f76  , ("y",), fill_v
+00000d60: 616c 7565 3d2d 3129 0a20 2020 2076 5b3a  alue=-1).    v[:
+00000d70: 345d 203d 206e 702e 6172 616e 6765 2834  4] = np.arange(4
+00000d80: 290a 0a20 2020 2076 203d 2064 732e 6372  )..    v = ds.cr
+00000d90: 6561 7465 5661 7269 6162 6c65 2822 7a22  eateVariable("z"
+00000da0: 2c20 2253 3122 2c20 2822 7a22 2c20 2273  , "S1", ("z", "s
+00000db0: 7472 696e 6733 2229 2c20 6669 6c6c 5f76  tring3"), fill_v
+00000dc0: 616c 7565 3d62 2258 2229 0a20 2020 2076  alue=b"X").    v
+00000dd0: 5b2e 2e2e 5d20 3d20 5f63 6861 725f 6172  [...] = _char_ar
+00000de0: 7261 790a 0a20 2020 2076 203d 2064 732e  ray..    v = ds.
 00000df0: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
-00000e00: 7a22 2c20 2253 3122 2c20 2822 7a22 2c20  z", "S1", ("z", 
-00000e10: 2273 7472 696e 6733 2229 2c20 6669 6c6c  "string3"), fill
-00000e20: 5f76 616c 7565 3d62 2258 2229 0a20 2020  _value=b"X").   
-00000e30: 2076 5b2e 2e2e 5d20 3d20 5f63 6861 725f   v[...] = _char_
-00000e40: 6172 7261 790a 0a20 2020 2076 203d 2064  array..    v = d
-00000e50: 732e 6372 6561 7465 5661 7269 6162 6c65  s.createVariable
-00000e60: 2822 7363 616c 6172 222c 206e 702e 666c  ("scalar", np.fl
-00000e70: 6f61 7433 322c 2028 2929 0a20 2020 2076  oat32, ()).    v
-00000e80: 5b2e 2e2e 5d20 3d20 322e 300a 0a20 2020  [...] = 2.0..   
-00000e90: 2023 2074 6573 7420 6372 6561 7469 6e67   # test creating
-00000ea0: 2061 2073 6361 6c61 7220 7769 7468 2063   a scalar with c
-00000eb0: 6f6d 7072 6573 7369 6f6e 206f 7074 696f  ompression optio
-00000ec0: 6e20 2877 6974 6820 7368 6f75 6c64 2062  n (with should b
-00000ed0: 6520 6967 6e6f 7265 6429 0a20 2020 2076  e ignored).    v
-00000ee0: 203d 2064 732e 6372 6561 7465 5661 7269   = ds.createVari
-00000ef0: 6162 6c65 2822 696e 7473 6361 6c61 7222  able("intscalar"
-00000f00: 2c20 6e70 2e69 6e74 3634 2c20 2829 2c20  , np.int64, (), 
-00000f10: 7a6c 6962 3d36 2c20 6669 6c6c 5f76 616c  zlib=6, fill_val
-00000f20: 7565 3d4e 6f6e 6529 0a20 2020 2076 5b2e  ue=None).    v[.
-00000f30: 2e2e 5d20 3d20 320a 0a20 2020 2076 203d  ..] = 2..    v =
-00000f40: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
-00000f50: 6c65 2822 666f 6f5f 756e 6c69 6d69 7465  le("foo_unlimite
-00000f60: 6422 2c20 666c 6f61 742c 2028 2278 222c  d", float, ("x",
-00000f70: 2022 756e 6c69 6d69 7465 6422 2929 0a20   "unlimited")). 
-00000f80: 2020 2076 5b2e 2e2e 5d20 3d20 310a 0a20     v[...] = 1.. 
-00000f90: 2020 2077 6974 6820 7261 6973 6573 2828     with raises((
-00000fa0: 6835 6e65 7463 6466 2e43 6f6d 7061 7469  h5netcdf.Compati
-00000fb0: 6269 6c69 7479 4572 726f 722c 2054 7970  bilityError, Typ
-00000fc0: 6545 7272 6f72 2929 3a0a 2020 2020 2020  eError)):.      
-00000fd0: 2020 6473 2e63 7265 6174 6556 6172 6961    ds.createVaria
-00000fe0: 626c 6528 2262 6f6f 6c65 616e 222c 206e  ble("boolean", n
-00000ff0: 702e 626f 6f6c 5f2c 2028 2278 2229 290a  p.bool_, ("x")).
-00001000: 0a20 2020 2067 203d 2064 732e 6372 6561  .    g = ds.crea
-00001010: 7465 4772 6f75 7028 2273 7562 6772 6f75  teGroup("subgrou
-00001020: 7022 290a 2020 2020 7620 3d20 672e 6372  p").    v = g.cr
-00001030: 6561 7465 5661 7269 6162 6c65 2822 7375  eateVariable("su
-00001040: 6276 6172 222c 206e 702e 696e 7433 322c  bvar", np.int32,
-00001050: 2028 2278 222c 2929 0a20 2020 2076 5b2e   ("x",)).    v[.
-00001060: 2e2e 5d20 3d20 6e70 2e61 7261 6e67 6528  ..] = np.arange(
-00001070: 342e 3029 0a0a 2020 2020 672e 6372 6561  4.0)..    g.crea
-00001080: 7465 4469 6d65 6e73 696f 6e28 2279 222c  teDimension("y",
-00001090: 2031 3029 0a20 2020 2067 2e63 7265 6174   10).    g.creat
-000010a0: 6556 6172 6961 626c 6528 2279 5f76 6172  eVariable("y_var
-000010b0: 222c 2066 6c6f 6174 2c20 2822 7922 2c29  ", float, ("y",)
-000010c0: 290a 0a20 2020 2064 732e 6372 6561 7465  )..    ds.create
-000010d0: 4469 6d65 6e73 696f 6e28 226d 6973 6d61  Dimension("misma
-000010e0: 7463 6865 645f 6469 6d22 2c20 3129 0a20  tched_dim", 1). 
-000010f0: 2020 2064 732e 6372 6561 7465 5661 7269     ds.createVari
-00001100: 6162 6c65 2822 6d69 736d 6174 6368 6564  able("mismatched
-00001110: 5f64 696d 222c 2069 6e74 2c20 2829 290a  _dim", int, ()).
-00001120: 0a20 2020 2076 203d 2064 732e 6372 6561  .    v = ds.crea
-00001130: 7465 5661 7269 6162 6c65 2822 7661 725f  teVariable("var_
-00001140: 6c65 6e5f 7374 7222 2c20 7374 722c 2028  len_str", str, (
-00001150: 2278 2229 290a 2020 2020 765b 305d 203d  "x")).    v[0] =
-00001160: 2022 666f 6f22 0a0a 2020 2020 6473 2e63   "foo"..    ds.c
-00001170: 6c6f 7365 2829 0a0a 0a64 6566 2077 7269  lose()...def wri
-00001180: 7465 5f68 356e 6574 6364 6628 746d 705f  te_h5netcdf(tmp_
-00001190: 6e65 7463 6466 293a 0a20 2020 2064 7320  netcdf):.    ds 
-000011a0: 3d20 6835 6e65 7463 6466 2e46 696c 6528  = h5netcdf.File(
-000011b0: 746d 705f 6e65 7463 6466 2c20 2277 2229  tmp_netcdf, "w")
-000011c0: 0a20 2020 2064 732e 6174 7472 735b 2267  .    ds.attrs["g
-000011d0: 6c6f 6261 6c22 5d20 3d20 3432 0a20 2020  lobal"] = 42.   
-000011e0: 2064 732e 6174 7472 735b 226f 7468 6572   ds.attrs["other
-000011f0: 5f61 7474 7222 5d20 3d20 2279 6573 220a  _attr"] = "yes".
-00001200: 2020 2020 6473 2e64 696d 656e 7369 6f6e      ds.dimension
-00001210: 7320 3d20 7b22 7822 3a20 342c 2022 7922  s = {"x": 4, "y"
-00001220: 3a20 352c 2022 7a22 3a20 362c 2022 656d  : 5, "z": 6, "em
-00001230: 7074 7922 3a20 302c 2022 756e 6c69 6d69  pty": 0, "unlimi
-00001240: 7465 6422 3a20 4e6f 6e65 7d0a 0a20 2020  ted": None}..   
-00001250: 2076 203d 2064 732e 6372 6561 7465 5f76   v = ds.create_v
-00001260: 6172 6961 626c 6528 0a20 2020 2020 2020  ariable(.       
-00001270: 2022 666f 6f22 2c20 2822 7822 2c20 2279   "foo", ("x", "y
-00001280: 2229 2c20 666c 6f61 742c 2063 6875 6e6b  "), float, chunk
-00001290: 733d 2834 2c20 3529 2c20 636f 6d70 7265  s=(4, 5), compre
-000012a0: 7373 696f 6e3d 2267 7a69 7022 2c20 7368  ssion="gzip", sh
-000012b0: 7566 666c 653d 5472 7565 0a20 2020 2029  uffle=True.    )
-000012c0: 0a20 2020 2076 5b2e 2e2e 5d20 3d20 310a  .    v[...] = 1.
-000012d0: 2020 2020 762e 6174 7472 735b 2275 6e69      v.attrs["uni
-000012e0: 7473 225d 203d 2022 6d65 7465 7273 220a  ts"] = "meters".
-000012f0: 0a20 2020 2072 656d 6f74 655f 6669 6c65  .    remote_file
-00001300: 203d 2069 7369 6e73 7461 6e63 6528 746d   = isinstance(tm
-00001310: 705f 6e65 7463 6466 2c20 7374 7229 2061  p_netcdf, str) a
-00001320: 6e64 2074 6d70 5f6e 6574 6364 662e 7374  nd tmp_netcdf.st
-00001330: 6172 7473 7769 7468 2872 656d 6f74 655f  artswith(remote_
-00001340: 6835 290a 2020 2020 6966 206e 6f74 2072  h5).    if not r
-00001350: 656d 6f74 655f 6669 6c65 3a0a 2020 2020  emote_file:.    
-00001360: 2020 2020 7620 3d20 6473 2e63 7265 6174      v = ds.creat
-00001370: 655f 7661 7269 6162 6c65 2822 7922 2c20  e_variable("y", 
-00001380: 2822 7922 2c29 2c20 696e 742c 2066 696c  ("y",), int, fil
-00001390: 6c76 616c 7565 3d2d 3129 0a20 2020 2020  lvalue=-1).     
-000013a0: 2020 2076 5b3a 345d 203d 206e 702e 6172     v[:4] = np.ar
-000013b0: 616e 6765 2834 290a 0a20 2020 2076 203d  ange(4)..    v =
-000013c0: 2064 732e 6372 6561 7465 5f76 6172 6961   ds.create_varia
-000013d0: 626c 6528 227a 222c 2028 227a 222c 2022  ble("z", ("z", "
-000013e0: 7374 7269 6e67 3322 292c 2064 6174 613d  string3"), data=
-000013f0: 5f63 6861 725f 6172 7261 792c 2066 696c  _char_array, fil
-00001400: 6c76 616c 7565 3d62 2258 2229 0a0a 2020  lvalue=b"X")..  
-00001410: 2020 7620 3d20 6473 2e63 7265 6174 655f    v = ds.create_
-00001420: 7661 7269 6162 6c65 2822 7363 616c 6172  variable("scalar
-00001430: 222c 2064 6174 613d 6e70 2e66 6c6f 6174  ", data=np.float
-00001440: 3332 2832 2e30 2929 0a0a 2020 2020 7620  32(2.0))..    v 
-00001450: 3d20 6473 2e63 7265 6174 655f 7661 7269  = ds.create_vari
-00001460: 6162 6c65 2822 696e 7473 6361 6c61 7222  able("intscalar"
-00001470: 2c20 6461 7461 3d6e 702e 696e 7436 3428  , data=np.int64(
-00001480: 3229 290a 0a20 2020 2076 203d 2064 732e  2))..    v = ds.
-00001490: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
-000014a0: 2266 6f6f 5f75 6e6c 696d 6974 6564 222c  "foo_unlimited",
-000014b0: 2028 2278 222c 2022 756e 6c69 6d69 7465   ("x", "unlimite
-000014c0: 6422 292c 2066 6c6f 6174 290a 2020 2020  d"), float).    
-000014d0: 765b 2e2e 2e5d 203d 2031 0a0a 2020 2020  v[...] = 1..    
-000014e0: 7769 7468 2072 6169 7365 7328 2868 356e  with raises((h5n
-000014f0: 6574 6364 662e 436f 6d70 6174 6962 696c  etcdf.Compatibil
-00001500: 6974 7945 7272 6f72 2c20 5479 7065 4572  ityError, TypeEr
-00001510: 726f 7229 293a 0a20 2020 2020 2020 2064  ror)):.        d
-00001520: 732e 6372 6561 7465 5f76 6172 6961 626c  s.create_variabl
-00001530: 6528 2262 6f6f 6c65 616e 222c 2064 6174  e("boolean", dat
-00001540: 613d 5472 7565 290a 0a20 2020 2067 203d  a=True)..    g =
-00001550: 2064 732e 6372 6561 7465 5f67 726f 7570   ds.create_group
-00001560: 2822 7375 6267 726f 7570 2229 0a20 2020  ("subgroup").   
-00001570: 2076 203d 2067 2e63 7265 6174 655f 7661   v = g.create_va
-00001580: 7269 6162 6c65 2822 7375 6276 6172 222c  riable("subvar",
-00001590: 2028 2278 222c 292c 206e 702e 696e 7433   ("x",), np.int3
-000015a0: 3229 0a20 2020 2076 5b2e 2e2e 5d20 3d20  2).    v[...] = 
-000015b0: 6e70 2e61 7261 6e67 6528 342e 3029 0a20  np.arange(4.0). 
-000015c0: 2020 2077 6974 6820 7261 6973 6573 2841     with raises(A
-000015d0: 7474 7269 6275 7465 4572 726f 7229 3a0a  ttributeError):.
-000015e0: 2020 2020 2020 2020 762e 6174 7472 735b          v.attrs[
-000015f0: 225f 4e65 7463 6466 3444 696d 6964 225d  "_Netcdf4Dimid"]
-00001600: 203d 202d 310a 0a20 2020 2067 2e64 696d   = -1..    g.dim
-00001610: 656e 7369 6f6e 735b 2279 225d 203d 2031  ensions["y"] = 1
-00001620: 300a 2020 2020 672e 6372 6561 7465 5f76  0.    g.create_v
-00001630: 6172 6961 626c 6528 2279 5f76 6172 222c  ariable("y_var",
-00001640: 2028 2279 222c 292c 2066 6c6f 6174 290a   ("y",), float).
-00001650: 2020 2020 672e 666c 7573 6828 290a 0a20      g.flush().. 
-00001660: 2020 2064 732e 6469 6d65 6e73 696f 6e73     ds.dimensions
-00001670: 5b22 6d69 736d 6174 6368 6564 5f64 696d  ["mismatched_dim
-00001680: 225d 203d 2031 0a20 2020 2064 732e 6372  "] = 1.    ds.cr
-00001690: 6561 7465 5f76 6172 6961 626c 6528 226d  eate_variable("m
-000016a0: 6973 6d61 7463 6865 645f 6469 6d22 2c20  ismatched_dim", 
-000016b0: 6474 7970 653d 696e 7429 0a20 2020 2064  dtype=int).    d
-000016c0: 732e 666c 7573 6828 290a 0a20 2020 2064  s.flush()..    d
-000016d0: 7420 3d20 6835 7079 2e73 7065 6369 616c  t = h5py.special
-000016e0: 5f64 7479 7065 2876 6c65 6e3d 7374 7229  _dtype(vlen=str)
-000016f0: 0a20 2020 2076 203d 2064 732e 6372 6561  .    v = ds.crea
-00001700: 7465 5f76 6172 6961 626c 6528 2276 6172  te_variable("var
-00001710: 5f6c 656e 5f73 7472 222c 2028 2278 222c  _len_str", ("x",
-00001720: 292c 2064 7479 7065 3d64 7429 0a20 2020  ), dtype=dt).   
-00001730: 2076 5b30 5d20 3d20 5f76 6c65 6e5f 7374   v[0] = _vlen_st
-00001740: 7269 6e67 0a0a 2020 2020 6473 2e63 6c6f  ring..    ds.clo
-00001750: 7365 2829 0a0a 0a64 6566 2072 6561 645f  se()...def read_
-00001760: 6c65 6761 6379 5f6e 6574 6364 6628 746d  legacy_netcdf(tm
-00001770: 705f 6e65 7463 6466 2c20 7265 6164 5f6d  p_netcdf, read_m
-00001780: 6f64 756c 652c 2077 7269 7465 5f6d 6f64  odule, write_mod
-00001790: 756c 6529 3a0a 2020 2020 6473 203d 2072  ule):.    ds = r
-000017a0: 6561 645f 6d6f 6475 6c65 2e44 6174 6173  ead_module.Datas
-000017b0: 6574 2874 6d70 5f6e 6574 6364 662c 2022  et(tmp_netcdf, "
-000017c0: 7222 290a 2020 2020 6173 7365 7274 2064  r").    assert d
-000017d0: 732e 6e63 6174 7472 7328 2920 3d3d 205b  s.ncattrs() == [
-000017e0: 2267 6c6f 6261 6c22 2c20 226f 7468 6572  "global", "other
-000017f0: 5f61 7474 7222 5d0a 2020 2020 6173 7365  _attr"].    asse
-00001800: 7274 2064 732e 6765 746e 6361 7474 7228  rt ds.getncattr(
-00001810: 2267 6c6f 6261 6c22 2920 3d3d 2034 320a  "global") == 42.
-00001820: 2020 2020 6966 2077 7269 7465 5f6d 6f64      if write_mod
-00001830: 756c 6520 6973 206e 6f74 206e 6574 4344  ule is not netCD
-00001840: 4634 3a0a 2020 2020 2020 2020 2320 736b  F4:.        # sk
-00001850: 6970 2066 6f72 206e 6f77 3a20 6874 7470  ip for now: http
-00001860: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f55  s://github.com/U
-00001870: 6e69 6461 7461 2f6e 6574 6364 6634 2d70  nidata/netcdf4-p
-00001880: 7974 686f 6e2f 6973 7375 6573 2f33 3838  ython/issues/388
-00001890: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000018a0: 6473 2e6f 7468 6572 5f61 7474 7220 3d3d  ds.other_attr ==
-000018b0: 2022 7965 7322 0a20 2020 2077 6974 6820   "yes".    with 
-000018c0: 7079 7465 7374 2e72 6169 7365 7328 4174  pytest.raises(At
-000018d0: 7472 6962 7574 6545 7272 6f72 293a 0a20  tributeError):. 
-000018e0: 2020 2020 2020 2064 732e 646f 6573 5f6e         ds.does_n
-000018f0: 6f74 5f65 7869 7374 0a20 2020 2061 7373  ot_exist.    ass
-00001900: 6572 7420 7365 7428 6473 2e64 696d 656e  ert set(ds.dimen
-00001910: 7369 6f6e 7329 203d 3d20 7365 7428 0a20  sions) == set(. 
-00001920: 2020 2020 2020 205b 2278 222c 2022 7922         ["x", "y"
-00001930: 2c20 227a 222c 2022 656d 7074 7922 2c20  , "z", "empty", 
-00001940: 2273 7472 696e 6733 222c 2022 6d69 736d  "string3", "mism
-00001950: 6174 6368 6564 5f64 696d 222c 2022 756e  atched_dim", "un
-00001960: 6c69 6d69 7465 6422 5d0a 2020 2020 290a  limited"].    ).
-00001970: 2020 2020 6173 7365 7274 2073 6574 2864      assert set(d
-00001980: 732e 7661 7269 6162 6c65 7329 203d 3d20  s.variables) == 
-00001990: 7365 7428 0a20 2020 2020 2020 205b 0a20  set(.        [. 
-000019a0: 2020 2020 2020 2020 2020 2022 666f 6f22             "foo"
-000019b0: 2c0a 2020 2020 2020 2020 2020 2020 2279  ,.            "y
-000019c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-000019d0: 7a22 2c0a 2020 2020 2020 2020 2020 2020  z",.            
-000019e0: 2269 6e74 7363 616c 6172 222c 0a20 2020  "intscalar",.   
-000019f0: 2020 2020 2020 2020 2022 7363 616c 6172           "scalar
-00001a00: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00001a10: 7661 725f 6c65 6e5f 7374 7222 2c0a 2020  var_len_str",.  
-00001a20: 2020 2020 2020 2020 2020 226d 6973 6d61            "misma
-00001a30: 7463 6865 645f 6469 6d22 2c0a 2020 2020  tched_dim",.    
-00001a40: 2020 2020 2020 2020 2266 6f6f 5f75 6e6c          "foo_unl
-00001a50: 696d 6974 6564 222c 0a20 2020 2020 2020  imited",.       
-00001a60: 205d 0a20 2020 2029 0a0a 2020 2020 6173   ].    )..    as
-00001a70: 7365 7274 2073 6574 2864 732e 6772 6f75  sert set(ds.grou
-00001a80: 7073 2920 3d3d 2073 6574 285b 2273 7562  ps) == set(["sub
-00001a90: 6772 6f75 7022 5d29 0a20 2020 2061 7373  group"]).    ass
-00001aa0: 6572 7420 6473 2e70 6172 656e 7420 6973  ert ds.parent is
-00001ab0: 204e 6f6e 650a 2020 2020 7620 3d20 6473   None.    v = ds
-00001ac0: 2e76 6172 6961 626c 6573 5b22 666f 6f22  .variables["foo"
-00001ad0: 5d0a 2020 2020 6173 7365 7274 2061 7272  ].    assert arr
-00001ae0: 6179 5f65 7175 616c 2876 2c20 6e70 2e6f  ay_equal(v, np.o
-00001af0: 6e65 7328 2834 2c20 3529 2929 0a20 2020  nes((4, 5))).   
-00001b00: 2061 7373 6572 7420 762e 6474 7970 6520   assert v.dtype 
-00001b10: 3d3d 2066 6c6f 6174 0a20 2020 2061 7373  == float.    ass
-00001b20: 6572 7420 762e 6469 6d65 6e73 696f 6e73  ert v.dimensions
-00001b30: 203d 3d20 2822 7822 2c20 2279 2229 0a20   == ("x", "y"). 
-00001b40: 2020 2061 7373 6572 7420 762e 6e64 696d     assert v.ndim
-00001b50: 203d 3d20 320a 2020 2020 6173 7365 7274   == 2.    assert
-00001b60: 2076 2e6e 6361 7474 7273 2829 203d 3d20   v.ncattrs() == 
-00001b70: 5b22 756e 6974 7322 5d0a 2020 2020 6966  ["units"].    if
-00001b80: 2077 7269 7465 5f6d 6f64 756c 6520 6973   write_module is
-00001b90: 206e 6f74 206e 6574 4344 4634 3a0a 2020   not netCDF4:.  
-00001ba0: 2020 2020 2020 6173 7365 7274 2076 2e67        assert v.g
-00001bb0: 6574 6e63 6174 7472 2822 756e 6974 7322  etncattr("units"
-00001bc0: 2920 3d3d 2022 6d65 7465 7273 220a 2020  ) == "meters".  
-00001bd0: 2020 6173 7365 7274 2074 7570 6c65 2876    assert tuple(v
-00001be0: 2e63 6875 6e6b 696e 6728 2929 203d 3d20  .chunking()) == 
-00001bf0: 2834 2c20 3529 0a0a 2020 2020 2320 6368  (4, 5)..    # ch
-00001c00: 6563 6b20 666f 7220 6469 6374 2069 7465  eck for dict ite
-00001c10: 6d73 2073 6570 6172 6174 656c 790a 2020  ms separately.  
-00001c20: 2020 2320 7365 6520 6874 7470 733a 2f2f    # see https://
-00001c30: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
-00001c40: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
-00001c50: 7565 732f 3137 310a 2020 2020 6669 6c74  ues/171.    filt
-00001c60: 6572 7320 3d20 762e 6669 6c74 6572 7328  ers = v.filters(
-00001c70: 290a 2020 2020 6173 7365 7274 2066 696c  ).    assert fil
-00001c80: 7465 7273 5b22 636f 6d70 6c65 7665 6c22  ters["complevel"
-00001c90: 5d20 3d3d 2034 0a20 2020 2061 7373 6572  ] == 4.    asser
-00001ca0: 7420 6669 6c74 6572 735b 2266 6c65 7463  t filters["fletc
-00001cb0: 6865 7233 3222 5d20 6973 2046 616c 7365  her32"] is False
-00001cc0: 0a20 2020 2061 7373 6572 7420 6669 6c74  .    assert filt
-00001cd0: 6572 735b 2273 6875 6666 6c65 225d 2069  ers["shuffle"] i
-00001ce0: 7320 5472 7565 0a20 2020 2061 7373 6572  s True.    asser
-00001cf0: 7420 6669 6c74 6572 735b 227a 6c69 6222  t filters["zlib"
-00001d00: 5d20 6973 2054 7275 650a 0a20 2020 2076  ] is True..    v
-00001d10: 203d 2064 732e 7661 7269 6162 6c65 735b   = ds.variables[
-00001d20: 2279 225d 0a20 2020 2061 7373 6572 7420  "y"].    assert 
-00001d30: 6172 7261 795f 6571 7561 6c28 762c 206e  array_equal(v, n
-00001d40: 702e 725f 5b6e 702e 6172 616e 6765 2834  p.r_[np.arange(4
-00001d50: 292c 205b 2d31 5d5d 290a 2020 2020 6173  ), [-1]]).    as
-00001d60: 7365 7274 2076 2e64 7479 7065 203d 3d20  sert v.dtype == 
-00001d70: 696e 740a 2020 2020 6173 7365 7274 2076  int.    assert v
-00001d80: 2e64 696d 656e 7369 6f6e 7320 3d3d 2028  .dimensions == (
-00001d90: 2279 222c 290a 2020 2020 6173 7365 7274  "y",).    assert
-00001da0: 2076 2e6e 6469 6d20 3d3d 2031 0a20 2020   v.ndim == 1.   
-00001db0: 2061 7373 6572 7420 762e 6e63 6174 7472   assert v.ncattr
-00001dc0: 7328 2920 3d3d 205b 225f 4669 6c6c 5661  s() == ["_FillVa
-00001dd0: 6c75 6522 5d0a 2020 2020 6173 7365 7274  lue"].    assert
-00001de0: 2076 2e67 6574 6e63 6174 7472 2822 5f46   v.getncattr("_F
-00001df0: 696c 6c56 616c 7565 2229 203d 3d20 2d31  illValue") == -1
-00001e00: 0a20 2020 2061 7373 6572 7420 762e 6368  .    assert v.ch
-00001e10: 756e 6b69 6e67 2829 203d 3d20 2263 6f6e  unking() == "con
-00001e20: 7469 6775 6f75 7322 0a0a 2020 2020 2320  tiguous"..    # 
-00001e30: 6368 6563 6b20 666f 7220 6469 6374 2069  check for dict i
-00001e40: 7465 6d73 2073 6570 6172 6174 656c 790a  tems separately.
-00001e50: 2020 2020 2320 7365 6520 6874 7470 733a      # see https:
-00001e60: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
-00001e70: 6574 6364 662f 6835 6e65 7463 6466 2f69  etcdf/h5netcdf/i
-00001e80: 7373 7565 732f 3137 310a 2020 2020 6669  ssues/171.    fi
-00001e90: 6c74 6572 7320 3d20 762e 6669 6c74 6572  lters = v.filter
-00001ea0: 7328 290a 2020 2020 6173 7365 7274 2066  s().    assert f
-00001eb0: 696c 7465 7273 5b22 636f 6d70 6c65 7665  ilters["compleve
-00001ec0: 6c22 5d20 3d3d 2030 0a20 2020 2061 7373  l"] == 0.    ass
-00001ed0: 6572 7420 6669 6c74 6572 735b 2266 6c65  ert filters["fle
-00001ee0: 7463 6865 7233 3222 5d20 6973 2046 616c  tcher32"] is Fal
-00001ef0: 7365 0a20 2020 2061 7373 6572 7420 6669  se.    assert fi
-00001f00: 6c74 6572 735b 2273 6875 6666 6c65 225d  lters["shuffle"]
-00001f10: 2069 7320 4661 6c73 650a 2020 2020 6173   is False.    as
-00001f20: 7365 7274 2066 696c 7465 7273 5b22 7a6c  sert filters["zl
-00001f30: 6962 225d 2069 7320 4661 6c73 650a 0a20  ib"] is False.. 
-00001f40: 2020 2064 732e 636c 6f73 6528 290a 0a20     ds.close().. 
-00001f50: 2020 2023 2043 6865 636b 2074 6865 2062     # Check the b
-00001f60: 6568 6176 696f 7220 6966 2068 3570 792e  ehavior if h5py.
-00001f70: 2043 616e 6e6f 7420 6578 7065 6374 2068   Cannot expect h
-00001f80: 356e 6574 6364 6620 746f 206f 7665 7263  5netcdf to overc
-00001f90: 6f6d 6520 7468 6573 650a 2020 2020 2320  ome these.    # 
-00001fa0: 6572 726f 7273 3a0a 2020 2020 6966 2069  errors:.    if i
-00001fb0: 735f 6835 7079 5f63 6861 725f 776f 726b  s_h5py_char_work
-00001fc0: 696e 6728 746d 705f 6e65 7463 6466 2c20  ing(tmp_netcdf, 
-00001fd0: 227a 2229 3a0a 2020 2020 2020 2020 6473  "z"):.        ds
-00001fe0: 203d 2072 6561 645f 6d6f 6475 6c65 2e44   = read_module.D
-00001ff0: 6174 6173 6574 2874 6d70 5f6e 6574 6364  ataset(tmp_netcd
-00002000: 662c 2022 7222 290a 2020 2020 2020 2020  f, "r").        
-00002010: 7620 3d20 6473 2e76 6172 6961 626c 6573  v = ds.variables
-00002020: 5b22 7a22 5d0a 2020 2020 2020 2020 6173  ["z"].        as
-00002030: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
-00002040: 2876 2c20 5f63 6861 725f 6172 7261 7929  (v, _char_array)
-00002050: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002060: 762e 6474 7970 6520 3d3d 2022 5331 220a  v.dtype == "S1".
-00002070: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-00002080: 2e6e 6469 6d20 3d3d 2032 0a20 2020 2020  .ndim == 2.     
-00002090: 2020 2061 7373 6572 7420 762e 6469 6d65     assert v.dime
-000020a0: 6e73 696f 6e73 203d 3d20 2822 7a22 2c20  nsions == ("z", 
-000020b0: 2273 7472 696e 6733 2229 0a20 2020 2020  "string3").     
-000020c0: 2020 2061 7373 6572 7420 762e 6e63 6174     assert v.ncat
-000020d0: 7472 7328 2920 3d3d 205b 225f 4669 6c6c  trs() == ["_Fill
-000020e0: 5661 6c75 6522 5d0a 2020 2020 2020 2020  Value"].        
-000020f0: 6173 7365 7274 2076 2e67 6574 6e63 6174  assert v.getncat
-00002100: 7472 2822 5f46 696c 6c56 616c 7565 2229  tr("_FillValue")
-00002110: 203d 3d20 6222 5822 0a20 2020 2065 6c73   == b"X".    els
-00002120: 653a 0a20 2020 2020 2020 2064 7320 3d20  e:.        ds = 
-00002130: 7265 6164 5f6d 6f64 756c 652e 4461 7461  read_module.Data
-00002140: 7365 7428 746d 705f 6e65 7463 6466 2c20  set(tmp_netcdf, 
-00002150: 2272 2229 0a0a 2020 2020 7620 3d20 6473  "r")..    v = ds
-00002160: 2e76 6172 6961 626c 6573 5b22 7363 616c  .variables["scal
-00002170: 6172 225d 0a20 2020 2061 7373 6572 7420  ar"].    assert 
-00002180: 6172 7261 795f 6571 7561 6c28 762c 206e  array_equal(v, n
-00002190: 702e 6172 7261 7928 322e 3029 290a 2020  p.array(2.0)).  
-000021a0: 2020 6173 7365 7274 2076 2e64 7479 7065    assert v.dtype
-000021b0: 203d 3d20 2266 6c6f 6174 3332 220a 2020   == "float32".  
-000021c0: 2020 6173 7365 7274 2076 2e6e 6469 6d20    assert v.ndim 
-000021d0: 3d3d 2030 0a20 2020 2061 7373 6572 7420  == 0.    assert 
-000021e0: 762e 6469 6d65 6e73 696f 6e73 203d 3d20  v.dimensions == 
-000021f0: 2829 0a20 2020 2061 7373 6572 7420 762e  ().    assert v.
-00002200: 6e63 6174 7472 7328 2920 3d3d 205b 5d0a  ncattrs() == [].
-00002210: 0a20 2020 2076 203d 2064 732e 7661 7269  .    v = ds.vari
-00002220: 6162 6c65 735b 2269 6e74 7363 616c 6172  ables["intscalar
-00002230: 225d 0a20 2020 2061 7373 6572 7420 6172  "].    assert ar
-00002240: 7261 795f 6571 7561 6c28 762c 206e 702e  ray_equal(v, np.
-00002250: 6172 7261 7928 3229 290a 2020 2020 6173  array(2)).    as
-00002260: 7365 7274 2076 2e64 7479 7065 203d 3d20  sert v.dtype == 
-00002270: 2269 6e74 3634 220a 2020 2020 6173 7365  "int64".    asse
-00002280: 7274 2076 2e6e 6469 6d20 3d3d 2030 0a20  rt v.ndim == 0. 
-00002290: 2020 2061 7373 6572 7420 762e 6469 6d65     assert v.dime
-000022a0: 6e73 696f 6e73 203d 3d20 2829 0a20 2020  nsions == ().   
-000022b0: 2061 7373 6572 7420 762e 6e63 6174 7472   assert v.ncattr
-000022c0: 7328 2920 3d3d 205b 5d0a 0a20 2020 2076  s() == []..    v
-000022d0: 203d 2064 732e 7661 7269 6162 6c65 735b   = ds.variables[
-000022e0: 2276 6172 5f6c 656e 5f73 7472 225d 0a20  "var_len_str"]. 
-000022f0: 2020 2061 7373 6572 7420 762e 6474 7970     assert v.dtyp
-00002300: 6520 3d3d 2073 7472 0a20 2020 2061 7373  e == str.    ass
-00002310: 6572 7420 765b 305d 203d 3d20 5f76 6c65  ert v[0] == _vle
-00002320: 6e5f 7374 7269 6e67 0a0a 2020 2020 7620  n_string..    v 
-00002330: 3d20 6473 2e67 726f 7570 735b 2273 7562  = ds.groups["sub
-00002340: 6772 6f75 7022 5d2e 7661 7269 6162 6c65  group"].variable
-00002350: 735b 2273 7562 7661 7222 5d0a 2020 2020  s["subvar"].    
-00002360: 6173 7365 7274 2064 732e 6772 6f75 7073  assert ds.groups
-00002370: 5b22 7375 6267 726f 7570 225d 2e70 6172  ["subgroup"].par
-00002380: 656e 7420 6973 2064 730a 2020 2020 6173  ent is ds.    as
-00002390: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
-000023a0: 2876 2c20 6e70 2e61 7261 6e67 6528 342e  (v, np.arange(4.
-000023b0: 3029 290a 2020 2020 6173 7365 7274 2076  0)).    assert v
-000023c0: 2e64 7479 7065 203d 3d20 2269 6e74 3332  .dtype == "int32
-000023d0: 220a 2020 2020 6173 7365 7274 2076 2e6e  ".    assert v.n
-000023e0: 6469 6d20 3d3d 2031 0a20 2020 2061 7373  dim == 1.    ass
-000023f0: 6572 7420 762e 6469 6d65 6e73 696f 6e73  ert v.dimensions
-00002400: 203d 3d20 2822 7822 2c29 0a20 2020 2061   == ("x",).    a
-00002410: 7373 6572 7420 762e 6e63 6174 7472 7328  ssert v.ncattrs(
-00002420: 2920 3d3d 205b 5d0a 0a20 2020 2076 203d  ) == []..    v =
-00002430: 2064 732e 6772 6f75 7073 5b22 7375 6267   ds.groups["subg
-00002440: 726f 7570 225d 2e76 6172 6961 626c 6573  roup"].variables
-00002450: 5b22 795f 7661 7222 5d0a 2020 2020 6173  ["y_var"].    as
-00002460: 7365 7274 2076 2e73 6861 7065 203d 3d20  sert v.shape == 
-00002470: 2831 302c 290a 2020 2020 6173 7365 7274  (10,).    assert
-00002480: 2022 7922 2069 6e20 6473 2e67 726f 7570   "y" in ds.group
-00002490: 735b 2273 7562 6772 6f75 7022 5d2e 6469  s["subgroup"].di
-000024a0: 6d65 6e73 696f 6e73 0a0a 2020 2020 6473  mensions..    ds
-000024b0: 2e63 6c6f 7365 2829 0a0a 0a64 6566 2072  .close()...def r
-000024c0: 6561 645f 6835 6e65 7463 6466 2874 6d70  ead_h5netcdf(tmp
-000024d0: 5f6e 6574 6364 662c 2077 7269 7465 5f6d  _netcdf, write_m
-000024e0: 6f64 756c 652c 2064 6563 6f64 655f 766c  odule, decode_vl
-000024f0: 656e 5f73 7472 696e 6773 293a 0a20 2020  en_strings):.   
-00002500: 2072 656d 6f74 655f 6669 6c65 203d 2069   remote_file = i
-00002510: 7369 6e73 7461 6e63 6528 746d 705f 6e65  sinstance(tmp_ne
-00002520: 7463 6466 2c20 7374 7229 2061 6e64 2074  tcdf, str) and t
-00002530: 6d70 5f6e 6574 6364 662e 7374 6172 7473  mp_netcdf.starts
-00002540: 7769 7468 2872 656d 6f74 655f 6835 290a  with(remote_h5).
-00002550: 2020 2020 6473 203d 2068 356e 6574 6364      ds = h5netcd
-00002560: 662e 4669 6c65 2874 6d70 5f6e 6574 6364  f.File(tmp_netcd
-00002570: 662c 2022 7222 2c20 2a2a 6465 636f 6465  f, "r", **decode
-00002580: 5f76 6c65 6e5f 7374 7269 6e67 7329 0a20  _vlen_strings). 
-00002590: 2020 2061 7373 6572 7420 6473 2e6e 616d     assert ds.nam
-000025a0: 6520 3d3d 2022 2f22 0a20 2020 2061 7373  e == "/".    ass
-000025b0: 6572 7420 6c69 7374 2864 732e 6174 7472  ert list(ds.attr
-000025c0: 7329 203d 3d20 5b22 676c 6f62 616c 222c  s) == ["global",
-000025d0: 2022 6f74 6865 725f 6174 7472 225d 0a20   "other_attr"]. 
-000025e0: 2020 2061 7373 6572 7420 6473 2e61 7474     assert ds.att
-000025f0: 7273 5b22 676c 6f62 616c 225d 203d 3d20  rs["global"] == 
-00002600: 3432 0a20 2020 2069 6620 7772 6974 655f  42.    if write_
-00002610: 6d6f 6475 6c65 2069 7320 6e6f 7420 6e65  module is not ne
-00002620: 7443 4446 343a 0a20 2020 2020 2020 2023  tCDF4:.        #
-00002630: 2073 6b69 7020 666f 7220 6e6f 773a 2068   skip for now: h
-00002640: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002650: 6d2f 556e 6964 6174 612f 6e65 7463 6466  m/Unidata/netcdf
-00002660: 342d 7079 7468 6f6e 2f69 7373 7565 732f  4-python/issues/
-00002670: 3338 380a 2020 2020 2020 2020 6173 7365  388.        asse
-00002680: 7274 2064 732e 6174 7472 735b 226f 7468  rt ds.attrs["oth
-00002690: 6572 5f61 7474 7222 5d20 3d3d 2022 7965  er_attr"] == "ye
-000026a0: 7322 0a20 2020 2061 7373 6572 7420 7365  s".    assert se
-000026b0: 7428 6473 2e64 696d 656e 7369 6f6e 7329  t(ds.dimensions)
-000026c0: 203d 3d20 7365 7428 0a20 2020 2020 2020   == set(.       
-000026d0: 205b 2278 222c 2022 7922 2c20 227a 222c   ["x", "y", "z",
-000026e0: 2022 656d 7074 7922 2c20 2273 7472 696e   "empty", "strin
-000026f0: 6733 222c 2022 6d69 736d 6174 6368 6564  g3", "mismatched
-00002700: 5f64 696d 222c 2022 756e 6c69 6d69 7465  _dim", "unlimite
-00002710: 6422 5d0a 2020 2020 290a 2020 2020 7661  d"].    ).    va
-00002720: 7269 6162 6c65 7320 3d20 7365 7428 0a20  riables = set(. 
-00002730: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00002740: 2020 2020 2022 666f 6f22 2c0a 2020 2020       "foo",.    
-00002750: 2020 2020 2020 2020 227a 222c 0a20 2020          "z",.   
-00002760: 2020 2020 2020 2020 2022 696e 7473 6361           "intsca
-00002770: 6c61 7222 2c0a 2020 2020 2020 2020 2020  lar",.          
-00002780: 2020 2273 6361 6c61 7222 2c0a 2020 2020    "scalar",.    
-00002790: 2020 2020 2020 2020 2276 6172 5f6c 656e          "var_len
-000027a0: 5f73 7472 222c 0a20 2020 2020 2020 2020  _str",.         
-000027b0: 2020 2022 6d69 736d 6174 6368 6564 5f64     "mismatched_d
-000027c0: 696d 222c 0a20 2020 2020 2020 2020 2020  im",.           
-000027d0: 2022 666f 6f5f 756e 6c69 6d69 7465 6422   "foo_unlimited"
-000027e0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
-000027f0: 290a 2020 2020 2320 6669 7820 6375 7272  ).    # fix curr
-00002800: 656e 7420 6661 696c 7572 6520 6f66 2068  ent failure of h
-00002810: 7364 732f 6835 7079 640a 2020 2020 6966  sds/h5pyd.    if
-00002820: 206e 6f74 2072 656d 6f74 655f 6669 6c65   not remote_file
-00002830: 3a0a 2020 2020 2020 2020 7661 7269 6162  :.        variab
-00002840: 6c65 7320 7c3d 2073 6574 285b 2279 225d  les |= set(["y"]
-00002850: 290a 2020 2020 6173 7365 7274 2073 6574  ).    assert set
-00002860: 2864 732e 7661 7269 6162 6c65 7329 203d  (ds.variables) =
-00002870: 3d20 7661 7269 6162 6c65 730a 0a20 2020  = variables..   
-00002880: 2061 7373 6572 7420 7365 7428 6473 2e67   assert set(ds.g
-00002890: 726f 7570 7329 203d 3d20 7365 7428 5b22  roups) == set(["
-000028a0: 7375 6267 726f 7570 225d 290a 2020 2020  subgroup"]).    
-000028b0: 6173 7365 7274 2064 732e 7061 7265 6e74  assert ds.parent
-000028c0: 2069 7320 4e6f 6e65 0a0a 2020 2020 7620   is None..    v 
-000028d0: 3d20 6473 5b22 666f 6f22 5d0a 2020 2020  = ds["foo"].    
-000028e0: 6173 7365 7274 2076 2e6e 616d 6520 3d3d  assert v.name ==
-000028f0: 2022 2f66 6f6f 220a 2020 2020 6173 7365   "/foo".    asse
-00002900: 7274 2061 7272 6179 5f65 7175 616c 2876  rt array_equal(v
-00002910: 2c20 6e70 2e6f 6e65 7328 2834 2c20 3529  , np.ones((4, 5)
-00002920: 2929 0a20 2020 2061 7373 6572 7420 762e  )).    assert v.
-00002930: 6474 7970 6520 3d3d 2066 6c6f 6174 0a20  dtype == float. 
-00002940: 2020 2061 7373 6572 7420 762e 6469 6d65     assert v.dime
-00002950: 6e73 696f 6e73 203d 3d20 2822 7822 2c20  nsions == ("x", 
-00002960: 2279 2229 0a20 2020 2061 7373 6572 7420  "y").    assert 
-00002970: 762e 6e64 696d 203d 3d20 320a 2020 2020  v.ndim == 2.    
-00002980: 6173 7365 7274 206c 6973 7428 762e 6174  assert list(v.at
-00002990: 7472 7329 203d 3d20 5b22 756e 6974 7322  trs) == ["units"
-000029a0: 5d0a 2020 2020 6966 2077 7269 7465 5f6d  ].    if write_m
-000029b0: 6f64 756c 6520 6973 206e 6f74 206e 6574  odule is not net
-000029c0: 4344 4634 3a0a 2020 2020 2020 2020 6173  CDF4:.        as
-000029d0: 7365 7274 2076 2e61 7474 7273 5b22 756e  sert v.attrs["un
-000029e0: 6974 7322 5d20 3d3d 2022 6d65 7465 7273  its"] == "meters
-000029f0: 220a 2020 2020 6173 7365 7274 2076 2e63  ".    assert v.c
-00002a00: 6875 6e6b 7320 3d3d 2028 342c 2035 290a  hunks == (4, 5).
-00002a10: 2020 2020 6173 7365 7274 2076 2e63 6f6d      assert v.com
-00002a20: 7072 6573 7369 6f6e 203d 3d20 2267 7a69  pression == "gzi
-00002a30: 7022 0a20 2020 2061 7373 6572 7420 762e  p".    assert v.
-00002a40: 636f 6d70 7265 7373 696f 6e5f 6f70 7473  compression_opts
-00002a50: 203d 3d20 340a 2020 2020 6173 7365 7274   == 4.    assert
-00002a60: 206e 6f74 2076 2e66 6c65 7463 6865 7233   not v.fletcher3
-00002a70: 320a 2020 2020 6173 7365 7274 2076 2e73  2.    assert v.s
-00002a80: 6875 6666 6c65 0a0a 2020 2020 2320 6669  huffle..    # fi
-00002a90: 7820 6375 7272 656e 7420 6661 696c 7572  x current failur
-00002aa0: 6520 6f66 2068 7364 732f 6835 7079 640a  e of hsds/h5pyd.
-00002ab0: 2020 2020 6966 206e 6f74 2072 656d 6f74      if not remot
-00002ac0: 655f 6669 6c65 3a0a 2020 2020 2020 2020  e_file:.        
-00002ad0: 7620 3d20 6473 5b22 7922 5d0a 2020 2020  v = ds["y"].    
-00002ae0: 2020 2020 6173 7365 7274 2061 7272 6179      assert array
-00002af0: 5f65 7175 616c 2876 2c20 6e70 2e72 5f5b  _equal(v, np.r_[
-00002b00: 6e70 2e61 7261 6e67 6528 3429 2c20 5b2d  np.arange(4), [-
-00002b10: 315d 5d29 0a20 2020 2020 2020 2061 7373  1]]).        ass
-00002b20: 6572 7420 762e 6474 7970 6520 3d3d 2069  ert v.dtype == i
-00002b30: 6e74 0a20 2020 2020 2020 2061 7373 6572  nt.        asser
-00002b40: 7420 762e 6469 6d65 6e73 696f 6e73 203d  t v.dimensions =
-00002b50: 3d20 2822 7922 2c29 0a20 2020 2020 2020  = ("y",).       
-00002b60: 2061 7373 6572 7420 762e 6e64 696d 203d   assert v.ndim =
-00002b70: 3d20 310a 2020 2020 2020 2020 6173 7365  = 1.        asse
-00002b80: 7274 206c 6973 7428 762e 6174 7472 7329  rt list(v.attrs)
-00002b90: 203d 3d20 5b22 5f46 696c 6c56 616c 7565   == ["_FillValue
-00002ba0: 225d 0a20 2020 2020 2020 2061 7373 6572  "].        asser
-00002bb0: 7420 762e 6174 7472 735b 225f 4669 6c6c  t v.attrs["_Fill
-00002bc0: 5661 6c75 6522 5d20 3d3d 202d 310a 2020  Value"] == -1.  
-00002bd0: 2020 2020 2020 6966 206e 6f74 2072 656d        if not rem
-00002be0: 6f74 655f 6669 6c65 3a0a 2020 2020 2020  ote_file:.      
-00002bf0: 2020 2020 2020 6173 7365 7274 2076 2e63        assert v.c
-00002c00: 6875 6e6b 7320 6973 204e 6f6e 650a 2020  hunks is None.  
-00002c10: 2020 2020 2020 6173 7365 7274 2076 2e63        assert v.c
-00002c20: 6f6d 7072 6573 7369 6f6e 2069 7320 4e6f  ompression is No
-00002c30: 6e65 0a20 2020 2020 2020 2061 7373 6572  ne.        asser
-00002c40: 7420 762e 636f 6d70 7265 7373 696f 6e5f  t v.compression_
-00002c50: 6f70 7473 2069 7320 4e6f 6e65 0a20 2020  opts is None.   
-00002c60: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
-00002c70: 762e 666c 6574 6368 6572 3332 0a20 2020  v.fletcher32.   
-00002c80: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
-00002c90: 762e 7368 7566 666c 650a 2020 2020 6473  v.shuffle.    ds
-00002ca0: 2e63 6c6f 7365 2829 0a0a 2020 2020 6966  .close()..    if
-00002cb0: 2069 735f 6835 7079 5f63 6861 725f 776f   is_h5py_char_wo
-00002cc0: 726b 696e 6728 746d 705f 6e65 7463 6466  rking(tmp_netcdf
-00002cd0: 2c20 227a 2229 3a0a 2020 2020 2020 2020  , "z"):.        
-00002ce0: 6473 203d 2068 356e 6574 6364 662e 4669  ds = h5netcdf.Fi
-00002cf0: 6c65 2874 6d70 5f6e 6574 6364 662c 2022  le(tmp_netcdf, "
-00002d00: 7222 290a 2020 2020 2020 2020 7620 3d20  r").        v = 
-00002d10: 6473 5b22 7a22 5d0a 2020 2020 2020 2020  ds["z"].        
-00002d20: 6173 7365 7274 2061 7272 6179 5f65 7175  assert array_equ
-00002d30: 616c 2876 2c20 5f63 6861 725f 6172 7261  al(v, _char_arra
-00002d40: 7929 0a20 2020 2020 2020 2061 7373 6572  y).        asser
-00002d50: 7420 762e 6474 7970 6520 3d3d 2022 5331  t v.dtype == "S1
-00002d60: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00002d70: 2076 2e6e 6469 6d20 3d3d 2032 0a20 2020   v.ndim == 2.   
-00002d80: 2020 2020 2061 7373 6572 7420 762e 6469       assert v.di
-00002d90: 6d65 6e73 696f 6e73 203d 3d20 2822 7a22  mensions == ("z"
-00002da0: 2c20 2273 7472 696e 6733 2229 0a20 2020  , "string3").   
-00002db0: 2020 2020 2061 7373 6572 7420 6c69 7374       assert list
-00002dc0: 2876 2e61 7474 7273 2920 3d3d 205b 225f  (v.attrs) == ["_
-00002dd0: 4669 6c6c 5661 6c75 6522 5d0a 2020 2020  FillValue"].    
-00002de0: 2020 2020 6173 7365 7274 2076 2e61 7474      assert v.att
-00002df0: 7273 5b22 5f46 696c 6c56 616c 7565 225d  rs["_FillValue"]
-00002e00: 203d 3d20 6222 5822 0a20 2020 2065 6c73   == b"X".    els
-00002e10: 653a 0a20 2020 2020 2020 2064 7320 3d20  e:.        ds = 
-00002e20: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
-00002e30: 705f 6e65 7463 6466 2c20 2272 222c 202a  p_netcdf, "r", *
-00002e40: 2a64 6563 6f64 655f 766c 656e 5f73 7472  *decode_vlen_str
-00002e50: 696e 6773 290a 0a20 2020 2076 203d 2064  ings)..    v = d
-00002e60: 735b 2273 6361 6c61 7222 5d0a 2020 2020  s["scalar"].    
-00002e70: 6173 7365 7274 2061 7272 6179 5f65 7175  assert array_equ
-00002e80: 616c 2876 2c20 6e70 2e61 7272 6179 2832  al(v, np.array(2
-00002e90: 2e30 2929 0a20 2020 2061 7373 6572 7420  .0)).    assert 
-00002ea0: 762e 6474 7970 6520 3d3d 2022 666c 6f61  v.dtype == "floa
-00002eb0: 7433 3222 0a20 2020 2061 7373 6572 7420  t32".    assert 
-00002ec0: 762e 6e64 696d 203d 3d20 300a 2020 2020  v.ndim == 0.    
-00002ed0: 6173 7365 7274 2076 2e64 696d 656e 7369  assert v.dimensi
-00002ee0: 6f6e 7320 3d3d 2028 290a 2020 2020 6173  ons == ().    as
-00002ef0: 7365 7274 206c 6973 7428 762e 6174 7472  sert list(v.attr
-00002f00: 7329 203d 3d20 5b5d 0a0a 2020 2020 7620  s) == []..    v 
-00002f10: 3d20 6473 2e76 6172 6961 626c 6573 5b22  = ds.variables["
-00002f20: 696e 7473 6361 6c61 7222 5d0a 2020 2020  intscalar"].    
-00002f30: 6173 7365 7274 2061 7272 6179 5f65 7175  assert array_equ
-00002f40: 616c 2876 2c20 6e70 2e61 7272 6179 2832  al(v, np.array(2
-00002f50: 2929 0a20 2020 2061 7373 6572 7420 762e  )).    assert v.
-00002f60: 6474 7970 6520 3d3d 2022 696e 7436 3422  dtype == "int64"
-00002f70: 0a20 2020 2061 7373 6572 7420 762e 6e64  .    assert v.nd
-00002f80: 696d 203d 3d20 300a 2020 2020 6173 7365  im == 0.    asse
-00002f90: 7274 2076 2e64 696d 656e 7369 6f6e 7320  rt v.dimensions 
-00002fa0: 3d3d 2028 290a 2020 2020 6173 7365 7274  == ().    assert
-00002fb0: 206c 6973 7428 762e 6174 7472 7329 203d   list(v.attrs) =
-00002fc0: 3d20 5b5d 0a0a 2020 2020 7620 3d20 6473  = []..    v = ds
-00002fd0: 5b22 7661 725f 6c65 6e5f 7374 7222 5d0a  ["var_len_str"].
-00002fe0: 2020 2020 6173 7365 7274 2068 3570 792e      assert h5py.
-00002ff0: 6368 6563 6b5f 6474 7970 6528 766c 656e  check_dtype(vlen
-00003000: 3d76 2e64 7479 7065 2920 3d3d 2073 7472  =v.dtype) == str
-00003010: 0a20 2020 2069 6620 6765 7461 7474 7228  .    if getattr(
-00003020: 6473 2c20 2264 6563 6f64 655f 766c 656e  ds, "decode_vlen
-00003030: 5f73 7472 696e 6773 222c 2054 7275 6529  _strings", True)
-00003040: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
-00003050: 2076 5b30 5d20 3d3d 205f 766c 656e 5f73   v[0] == _vlen_s
-00003060: 7472 696e 670a 2020 2020 656c 7365 3a0a  tring.    else:.
-00003070: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
-00003080: 5b30 5d20 3d3d 205f 766c 656e 5f73 7472  [0] == _vlen_str
-00003090: 696e 672e 656e 636f 6465 2822 7574 665f  ing.encode("utf_
-000030a0: 3822 290a 0a20 2020 2076 203d 2064 735b  8")..    v = ds[
-000030b0: 222f 7375 6267 726f 7570 2f73 7562 7661  "/subgroup/subva
-000030c0: 7222 5d0a 2020 2020 6173 7365 7274 2076  r"].    assert v
-000030d0: 2069 7320 6473 5b22 7375 6267 726f 7570   is ds["subgroup
-000030e0: 225d 5b22 7375 6276 6172 225d 0a20 2020  "]["subvar"].   
-000030f0: 2061 7373 6572 7420 7620 6973 2064 735b   assert v is ds[
-00003100: 2273 7562 6772 6f75 702f 7375 6276 6172  "subgroup/subvar
-00003110: 225d 0a20 2020 2061 7373 6572 7420 7620  "].    assert v 
-00003120: 6973 2064 735b 2273 7562 6772 6f75 7022  is ds["subgroup"
-00003130: 5d5b 222f 7375 6267 726f 7570 2f73 7562  ]["/subgroup/sub
-00003140: 7661 7222 5d0a 2020 2020 6173 7365 7274  var"].    assert
-00003150: 2076 2e6e 616d 6520 3d3d 2022 2f73 7562   v.name == "/sub
-00003160: 6772 6f75 702f 7375 6276 6172 220a 2020  group/subvar".  
-00003170: 2020 6173 7365 7274 2064 735b 2273 7562    assert ds["sub
-00003180: 6772 6f75 7022 5d2e 6e61 6d65 203d 3d20  group"].name == 
-00003190: 222f 7375 6267 726f 7570 220a 2020 2020  "/subgroup".    
-000031a0: 6173 7365 7274 2064 735b 2273 7562 6772  assert ds["subgr
-000031b0: 6f75 7022 5d2e 7061 7265 6e74 2069 7320  oup"].parent is 
-000031c0: 6473 0a20 2020 2061 7373 6572 7420 6172  ds.    assert ar
-000031d0: 7261 795f 6571 7561 6c28 762c 206e 702e  ray_equal(v, np.
-000031e0: 6172 616e 6765 2834 2e30 2929 0a20 2020  arange(4.0)).   
-000031f0: 2061 7373 6572 7420 762e 6474 7970 6520   assert v.dtype 
-00003200: 3d3d 2022 696e 7433 3222 0a20 2020 2061  == "int32".    a
-00003210: 7373 6572 7420 762e 6e64 696d 203d 3d20  ssert v.ndim == 
-00003220: 310a 2020 2020 6173 7365 7274 2076 2e64  1.    assert v.d
-00003230: 696d 656e 7369 6f6e 7320 3d3d 2028 2278  imensions == ("x
-00003240: 222c 290a 2020 2020 6173 7365 7274 206c  ",).    assert l
-00003250: 6973 7428 762e 6174 7472 7329 203d 3d20  ist(v.attrs) == 
-00003260: 5b5d 0a0a 2020 2020 6173 7365 7274 2064  []..    assert d
-00003270: 735b 222f 7375 6267 726f 7570 2f79 5f76  s["/subgroup/y_v
-00003280: 6172 225d 2e73 6861 7065 203d 3d20 2831  ar"].shape == (1
-00003290: 302c 290a 2020 2020 6173 7365 7274 2064  0,).    assert d
-000032a0: 735b 222f 7375 6267 726f 7570 225d 2e64  s["/subgroup"].d
-000032b0: 696d 656e 7369 6f6e 735b 2279 225d 2e73  imensions["y"].s
-000032c0: 697a 6520 3d3d 2031 300a 0a20 2020 2064  ize == 10..    d
-000032d0: 732e 636c 6f73 6528 290a 0a0a 6465 6620  s.close()...def 
-000032e0: 726f 756e 6474 7269 705f 6c65 6761 6379  roundtrip_legacy
-000032f0: 5f6e 6574 6364 6628 746d 705f 6e65 7463  _netcdf(tmp_netc
-00003300: 6466 2c20 7265 6164 5f6d 6f64 756c 652c  df, read_module,
-00003310: 2077 7269 7465 5f6d 6f64 756c 6529 3a0a   write_module):.
-00003320: 2020 2020 7772 6974 655f 6c65 6761 6379      write_legacy
-00003330: 5f6e 6574 6364 6628 746d 705f 6e65 7463  _netcdf(tmp_netc
-00003340: 6466 2c20 7772 6974 655f 6d6f 6475 6c65  df, write_module
-00003350: 290a 2020 2020 7265 6164 5f6c 6567 6163  ).    read_legac
-00003360: 795f 6e65 7463 6466 2874 6d70 5f6e 6574  y_netcdf(tmp_net
-00003370: 6364 662c 2072 6561 645f 6d6f 6475 6c65  cdf, read_module
-00003380: 2c20 7772 6974 655f 6d6f 6475 6c65 290a  , write_module).
-00003390: 0a0a 6465 6620 7465 7374 5f77 7269 7465  ..def test_write
-000033a0: 5f6c 6567 6163 7961 7069 5f72 6561 645f  _legacyapi_read_
-000033b0: 6e65 7443 4446 3428 746d 705f 6c6f 6361  netCDF4(tmp_loca
-000033c0: 6c5f 6e65 7463 6466 293a 0a20 2020 2072  l_netcdf):.    r
-000033d0: 6f75 6e64 7472 6970 5f6c 6567 6163 795f  oundtrip_legacy_
-000033e0: 6e65 7463 6466 2874 6d70 5f6c 6f63 616c  netcdf(tmp_local
-000033f0: 5f6e 6574 6364 662c 206e 6574 4344 4634  _netcdf, netCDF4
-00003400: 2c20 6c65 6761 6379 6170 6929 0a0a 0a64  , legacyapi)...d
-00003410: 6566 2074 6573 745f 726f 756e 6474 7269  ef test_roundtri
-00003420: 705f 6835 6e65 7463 6466 5f6c 6567 6163  p_h5netcdf_legac
-00003430: 7961 7069 2874 6d70 5f6c 6f63 616c 5f6e  yapi(tmp_local_n
-00003440: 6574 6364 6629 3a0a 2020 2020 726f 756e  etcdf):.    roun
-00003450: 6474 7269 705f 6c65 6761 6379 5f6e 6574  dtrip_legacy_net
-00003460: 6364 6628 746d 705f 6c6f 6361 6c5f 6e65  cdf(tmp_local_ne
-00003470: 7463 6466 2c20 6c65 6761 6379 6170 692c  tcdf, legacyapi,
-00003480: 206c 6567 6163 7961 7069 290a 0a0a 6465   legacyapi)...de
-00003490: 6620 7465 7374 5f77 7269 7465 5f6e 6574  f test_write_net
-000034a0: 4344 4634 5f72 6561 645f 6c65 6761 6379  CDF4_read_legacy
-000034b0: 6170 6928 746d 705f 6c6f 6361 6c5f 6e65  api(tmp_local_ne
-000034c0: 7463 6466 293a 0a20 2020 2072 6f75 6e64  tcdf):.    round
-000034d0: 7472 6970 5f6c 6567 6163 795f 6e65 7463  trip_legacy_netc
-000034e0: 6466 2874 6d70 5f6c 6f63 616c 5f6e 6574  df(tmp_local_net
-000034f0: 6364 662c 206c 6567 6163 7961 7069 2c20  cdf, legacyapi, 
-00003500: 6e65 7443 4446 3429 0a0a 0a64 6566 2074  netCDF4)...def t
-00003510: 6573 745f 7772 6974 655f 6835 6e65 7463  est_write_h5netc
-00003520: 6466 5f72 6561 645f 6c65 6761 6379 6170  df_read_legacyap
-00003530: 6928 746d 705f 6c6f 6361 6c5f 6e65 7463  i(tmp_local_netc
-00003540: 6466 293a 0a20 2020 2077 7269 7465 5f68  df):.    write_h
-00003550: 356e 6574 6364 6628 746d 705f 6c6f 6361  5netcdf(tmp_loca
-00003560: 6c5f 6e65 7463 6466 290a 2020 2020 7265  l_netcdf).    re
-00003570: 6164 5f6c 6567 6163 795f 6e65 7463 6466  ad_legacy_netcdf
-00003580: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
-00003590: 662c 206c 6567 6163 7961 7069 2c20 6835  f, legacyapi, h5
-000035a0: 6e65 7463 6466 290a 0a0a 6465 6620 7465  netcdf)...def te
-000035b0: 7374 5f77 7269 7465 5f68 356e 6574 6364  st_write_h5netcd
-000035c0: 665f 7265 6164 5f6e 6574 4344 4634 2874  f_read_netCDF4(t
-000035d0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 6629  mp_local_netcdf)
-000035e0: 3a0a 2020 2020 7772 6974 655f 6835 6e65  :.    write_h5ne
-000035f0: 7463 6466 2874 6d70 5f6c 6f63 616c 5f6e  tcdf(tmp_local_n
-00003600: 6574 6364 6629 0a20 2020 2072 6561 645f  etcdf).    read_
-00003610: 6c65 6761 6379 5f6e 6574 6364 6628 746d  legacy_netcdf(tm
-00003620: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-00003630: 6e65 7443 4446 342c 2068 356e 6574 6364  netCDF4, h5netcd
-00003640: 6629 0a0a 0a64 6566 2074 6573 745f 726f  f)...def test_ro
-00003650: 756e 6474 7269 705f 6835 6e65 7463 6466  undtrip_h5netcdf
-00003660: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
-00003670: 6d6f 7465 5f6e 6574 6364 662c 2064 6563  mote_netcdf, dec
-00003680: 6f64 655f 766c 656e 5f73 7472 696e 6773  ode_vlen_strings
-00003690: 293a 0a20 2020 2077 7269 7465 5f68 356e  ):.    write_h5n
-000036a0: 6574 6364 6628 746d 705f 6c6f 6361 6c5f  etcdf(tmp_local_
-000036b0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-000036c0: 290a 2020 2020 7265 6164 5f68 356e 6574  ).    read_h5net
-000036d0: 6364 6628 746d 705f 6c6f 6361 6c5f 6f72  cdf(tmp_local_or
-000036e0: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
-000036f0: 6835 6e65 7463 6466 2c20 6465 636f 6465  h5netcdf, decode
-00003700: 5f76 6c65 6e5f 7374 7269 6e67 7329 0a0a  _vlen_strings)..
-00003710: 0a64 6566 2074 6573 745f 7772 6974 655f  .def test_write_
-00003720: 6e65 7443 4446 345f 7265 6164 5f68 356e  netCDF4_read_h5n
-00003730: 6574 6364 6628 746d 705f 6c6f 6361 6c5f  etcdf(tmp_local_
-00003740: 6e65 7463 6466 2c20 6465 636f 6465 5f76  netcdf, decode_v
-00003750: 6c65 6e5f 7374 7269 6e67 7329 3a0a 2020  len_strings):.  
-00003760: 2020 7772 6974 655f 6c65 6761 6379 5f6e    write_legacy_n
-00003770: 6574 6364 6628 746d 705f 6c6f 6361 6c5f  etcdf(tmp_local_
-00003780: 6e65 7463 6466 2c20 6e65 7443 4446 3429  netcdf, netCDF4)
-00003790: 0a20 2020 2072 6561 645f 6835 6e65 7463  .    read_h5netc
-000037a0: 6466 2874 6d70 5f6c 6f63 616c 5f6e 6574  df(tmp_local_net
-000037b0: 6364 662c 206e 6574 4344 4634 2c20 6465  cdf, netCDF4, de
-000037c0: 636f 6465 5f76 6c65 6e5f 7374 7269 6e67  code_vlen_string
-000037d0: 7329 0a0a 0a64 6566 2074 6573 745f 7772  s)...def test_wr
-000037e0: 6974 655f 6c65 6761 6379 6170 695f 7265  ite_legacyapi_re
-000037f0: 6164 5f68 356e 6574 6364 6628 746d 705f  ad_h5netcdf(tmp_
-00003800: 6c6f 6361 6c5f 6e65 7463 6466 2c20 6465  local_netcdf, de
-00003810: 636f 6465 5f76 6c65 6e5f 7374 7269 6e67  code_vlen_string
-00003820: 7329 3a0a 2020 2020 7772 6974 655f 6c65  s):.    write_le
-00003830: 6761 6379 5f6e 6574 6364 6628 746d 705f  gacy_netcdf(tmp_
-00003840: 6c6f 6361 6c5f 6e65 7463 6466 2c20 6c65  local_netcdf, le
-00003850: 6761 6379 6170 6929 0a20 2020 2072 6561  gacyapi).    rea
-00003860: 645f 6835 6e65 7463 6466 2874 6d70 5f6c  d_h5netcdf(tmp_l
-00003870: 6f63 616c 5f6e 6574 6364 662c 206c 6567  ocal_netcdf, leg
-00003880: 6163 7961 7069 2c20 6465 636f 6465 5f76  acyapi, decode_v
-00003890: 6c65 6e5f 7374 7269 6e67 7329 0a0a 0a64  len_strings)...d
-000038a0: 6566 2074 6573 745f 6669 6c65 6f62 6a28  ef test_fileobj(
-000038b0: 6465 636f 6465 5f76 6c65 6e5f 7374 7269  decode_vlen_stri
-000038c0: 6e67 7329 3a0a 2020 2020 6966 2076 6572  ngs):.    if ver
-000038d0: 7369 6f6e 2e70 6172 7365 2868 3570 792e  sion.parse(h5py.
-000038e0: 5f5f 7665 7273 696f 6e5f 5f29 203c 2076  __version__) < v
-000038f0: 6572 7369 6f6e 2e70 6172 7365 2822 322e  ersion.parse("2.
-00003900: 392e 3022 293a 0a20 2020 2020 2020 2070  9.0"):.        p
-00003910: 7974 6573 742e 736b 6970 2822 6835 7079  ytest.skip("h5py
-00003920: 203e 2032 2e39 2e30 2072 6571 7569 7265   > 2.9.0 require
-00003930: 6420 746f 2074 6573 7420 6669 6c65 2d6c  d to test file-l
-00003940: 696b 6520 6f62 6a65 6374 7322 290a 2020  ike objects").  
-00003950: 2020 6669 6c65 6f62 6a20 3d20 7465 6d70    fileobj = temp
-00003960: 6669 6c65 2e54 656d 706f 7261 7279 4669  file.TemporaryFi
-00003970: 6c65 2829 0a20 2020 2077 7269 7465 5f68  le().    write_h
-00003980: 356e 6574 6364 6628 6669 6c65 6f62 6a29  5netcdf(fileobj)
-00003990: 0a20 2020 2072 6561 645f 6835 6e65 7463  .    read_h5netc
-000039a0: 6466 2866 696c 656f 626a 2c20 6835 6e65  df(fileobj, h5ne
-000039b0: 7463 6466 2c20 6465 636f 6465 5f76 6c65  tcdf, decode_vle
-000039c0: 6e5f 7374 7269 6e67 7329 0a20 2020 2066  n_strings).    f
-000039d0: 696c 656f 626a 203d 2069 6f2e 4279 7465  ileobj = io.Byte
-000039e0: 7349 4f28 290a 2020 2020 7772 6974 655f  sIO().    write_
-000039f0: 6835 6e65 7463 6466 2866 696c 656f 626a  h5netcdf(fileobj
-00003a00: 290a 2020 2020 7265 6164 5f68 356e 6574  ).    read_h5net
-00003a10: 6364 6628 6669 6c65 6f62 6a2c 2068 356e  cdf(fileobj, h5n
-00003a20: 6574 6364 662c 2064 6563 6f64 655f 766c  etcdf, decode_vl
-00003a30: 656e 5f73 7472 696e 6773 290a 0a0a 6465  en_strings)...de
-00003a40: 6620 7465 7374 5f72 6570 7228 746d 705f  f test_repr(tmp_
-00003a50: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-00003a60: 6e65 7463 6466 293a 0a20 2020 2077 7269  netcdf):.    wri
-00003a70: 7465 5f68 356e 6574 6364 6628 746d 705f  te_h5netcdf(tmp_
-00003a80: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-00003a90: 6e65 7463 6466 290a 2020 2020 6620 3d20  netcdf).    f = 
-00003aa0: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
-00003ab0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
-00003ac0: 655f 6e65 7463 6466 2c20 2261 2229 0a20  e_netcdf, "a"). 
-00003ad0: 2020 2061 7373 6572 7420 2268 356e 6574     assert "h5net
-00003ae0: 6364 662e 4669 6c65 2220 696e 2072 6570  cdf.File" in rep
-00003af0: 7228 6629 0a20 2020 2061 7373 6572 7420  r(f).    assert 
-00003b00: 2273 7562 6772 6f75 7022 2069 6e20 7265  "subgroup" in re
-00003b10: 7072 2866 290a 2020 2020 6173 7365 7274  pr(f).    assert
-00003b20: 2022 666f 6f22 2069 6e20 7265 7072 2866   "foo" in repr(f
-00003b30: 290a 2020 2020 6173 7365 7274 2022 6f74  ).    assert "ot
-00003b40: 6865 725f 6174 7472 2220 696e 2072 6570  her_attr" in rep
-00003b50: 7228 6629 0a0a 2020 2020 6173 7365 7274  r(f)..    assert
-00003b60: 2022 6835 6e65 7463 6466 2e61 7474 7273   "h5netcdf.attrs
-00003b70: 2e41 7474 7269 6275 7465 7322 2069 6e20  .Attributes" in 
-00003b80: 7265 7072 2866 2e61 7474 7273 290a 2020  repr(f.attrs).  
-00003b90: 2020 6173 7365 7274 2022 676c 6f62 616c    assert "global
-00003ba0: 2220 696e 2072 6570 7228 662e 6174 7472  " in repr(f.attr
-00003bb0: 7329 0a0a 2020 2020 6420 3d20 662e 6469  s)..    d = f.di
-00003bc0: 6d65 6e73 696f 6e73 0a20 2020 2061 7373  mensions.    ass
-00003bd0: 6572 7420 2268 356e 6574 6364 662e 4469  ert "h5netcdf.Di
-00003be0: 6d65 6e73 696f 6e73 2220 696e 2072 6570  mensions" in rep
-00003bf0: 7228 6429 0a20 2020 2061 7373 6572 7420  r(d).    assert 
-00003c00: 2278 3d3c 6835 6e65 7463 6466 2e44 696d  "x=<h5netcdf.Dim
-00003c10: 656e 7369 6f6e 2027 7827 3a20 7369 7a65  ension 'x': size
-00003c20: 2034 3e22 2069 6e20 7265 7072 2864 290a   4>" in repr(d).
-00003c30: 0a20 2020 2067 203d 2066 5b22 7375 6267  .    g = f["subg
-00003c40: 726f 7570 225d 0a20 2020 2061 7373 6572  roup"].    asser
-00003c50: 7420 2268 356e 6574 6364 662e 4772 6f75  t "h5netcdf.Grou
-00003c60: 7022 2069 6e20 7265 7072 2867 290a 2020  p" in repr(g).  
-00003c70: 2020 6173 7365 7274 2022 7375 6276 6172    assert "subvar
-00003c80: 2220 696e 2072 6570 7228 6729 0a0a 2020  " in repr(g)..  
-00003c90: 2020 7620 3d20 665b 2266 6f6f 225d 0a20    v = f["foo"]. 
-00003ca0: 2020 2061 7373 6572 7420 2268 356e 6574     assert "h5net
-00003cb0: 6364 662e 5661 7269 6162 6c65 2220 696e  cdf.Variable" in
-00003cc0: 2072 6570 7228 7629 0a20 2020 2061 7373   repr(v).    ass
-00003cd0: 6572 7420 2266 6c6f 6174 2220 696e 2072  ert "float" in r
-00003ce0: 6570 7228 7629 0a20 2020 2061 7373 6572  epr(v).    asser
-00003cf0: 7420 2275 6e69 7473 2220 696e 2072 6570  t "units" in rep
-00003d00: 7228 7629 0a0a 2020 2020 662e 6469 6d65  r(v)..    f.dime
-00003d10: 6e73 696f 6e73 5b22 7465 6d70 225d 203d  nsions["temp"] =
-00003d20: 204e 6f6e 650a 2020 2020 6173 7365 7274   None.    assert
-00003d30: 2022 7465 6d70 3a20 3c68 356e 6574 6364   "temp: <h5netcd
-00003d40: 662e 4469 6d65 6e73 696f 6e20 2774 656d  f.Dimension 'tem
-00003d50: 7027 3a20 7369 7a65 2030 2028 756e 6c69  p': size 0 (unli
-00003d60: 6d69 7465 6429 3e22 2069 6e20 7265 7072  mited)>" in repr
-00003d70: 2866 290a 2020 2020 662e 7265 7369 7a65  (f).    f.resize
-00003d80: 5f64 696d 656e 7369 6f6e 2822 7465 6d70  _dimension("temp
-00003d90: 222c 2035 290a 2020 2020 6173 7365 7274  ", 5).    assert
-00003da0: 2022 7465 6d70 3a20 3c68 356e 6574 6364   "temp: <h5netcd
-00003db0: 662e 4469 6d65 6e73 696f 6e20 2774 656d  f.Dimension 'tem
-00003dc0: 7027 3a20 7369 7a65 2035 2028 756e 6c69  p': size 5 (unli
-00003dd0: 6d69 7465 6429 3e22 2069 6e20 7265 7072  mited)>" in repr
-00003de0: 2866 290a 0a20 2020 2066 2e63 6c6f 7365  (f)..    f.close
-00003df0: 2829 0a0a 2020 2020 6173 7365 7274 2022  ()..    assert "
-00003e00: 436c 6f73 6564 2220 696e 2072 6570 7228  Closed" in repr(
-00003e10: 6629 0a20 2020 2061 7373 6572 7420 2243  f).    assert "C
-00003e20: 6c6f 7365 6422 2069 6e20 7265 7072 2864  losed" in repr(d
-00003e30: 290a 2020 2020 6173 7365 7274 2022 436c  ).    assert "Cl
-00003e40: 6f73 6564 2220 696e 2072 6570 7228 6729  osed" in repr(g)
-00003e50: 0a20 2020 2061 7373 6572 7420 2243 6c6f  .    assert "Clo
-00003e60: 7365 6422 2069 6e20 7265 7072 2876 290a  sed" in repr(v).
-00003e70: 0a0a 6465 6620 7465 7374 5f61 7474 7273  ..def test_attrs
-00003e80: 5f61 7069 2874 6d70 5f6c 6f63 616c 5f6f  _api(tmp_local_o
-00003e90: 725f 7265 6d6f 7465 5f6e 6574 6364 6629  r_remote_netcdf)
-00003ea0: 3a0a 2020 2020 6835 203d 2067 6574 5f68  :.    h5 = get_h
-00003eb0: 6466 355f 6d6f 6475 6c65 2874 6d70 5f6c  df5_module(tmp_l
-00003ec0: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
-00003ed0: 6574 6364 6629 0a20 2020 2077 6974 6820  etcdf).    with 
-00003ee0: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
-00003ef0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
-00003f00: 655f 6e65 7463 6466 2c20 2277 2229 2061  e_netcdf, "w") a
-00003f10: 7320 6473 3a0a 2020 2020 2020 2020 6473  s ds:.        ds
-00003f20: 2e61 7474 7273 5b22 636f 6e76 656e 7469  .attrs["conventi
-00003f30: 6f6e 7322 5d20 3d20 2243 4622 0a20 2020  ons"] = "CF".   
-00003f40: 2020 2020 2064 732e 6174 7472 735b 2265       ds.attrs["e
-00003f50: 6d70 7479 5f73 7472 696e 6722 5d20 3d20  mpty_string"] = 
-00003f60: 6835 2e45 6d70 7479 2864 7479 7065 3d6e  h5.Empty(dtype=n
-00003f70: 702e 6474 7970 6528 227c 5331 2229 290a  p.dtype("|S1")).
-00003f80: 2020 2020 2020 2020 6473 2e64 696d 656e          ds.dimen
-00003f90: 7369 6f6e 735b 2278 225d 203d 2031 0a20  sions["x"] = 1. 
-00003fa0: 2020 2020 2020 2076 203d 2064 732e 6372         v = ds.cr
-00003fb0: 6561 7465 5f76 6172 6961 626c 6528 2278  eate_variable("x
-00003fc0: 222c 2028 2278 222c 292c 2022 6934 2229  ", ("x",), "i4")
-00003fd0: 0a20 2020 2020 2020 2076 2e61 7474 7273  .        v.attrs
-00003fe0: 2e75 7064 6174 6528 7b22 756e 6974 7322  .update({"units"
-00003ff0: 3a20 226d 6574 6572 7322 2c20 2266 6f6f  : "meters", "foo
-00004000: 223a 2022 6261 7222 7d29 0a20 2020 2061  ": "bar"}).    a
-00004010: 7373 6572 7420 6473 2e5f 636c 6f73 6564  ssert ds._closed
-00004020: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-00004030: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-00004040: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
-00004050: 6466 2c20 2272 2229 2061 7320 6473 3a0a  df, "r") as ds:.
-00004060: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
-00004070: 656e 2864 732e 6174 7472 7329 203d 3d20  en(ds.attrs) == 
-00004080: 320a 2020 2020 2020 2020 6173 7365 7274  2.        assert
-00004090: 2064 6963 7428 6473 2e61 7474 7273 2920   dict(ds.attrs) 
-000040a0: 3d3d 207b 2263 6f6e 7665 6e74 696f 6e73  == {"conventions
-000040b0: 223a 2022 4346 222c 2022 656d 7074 795f  ": "CF", "empty_
-000040c0: 7374 7269 6e67 223a 2062 2222 7d0a 2020  string": b""}.  
-000040d0: 2020 2020 2020 6173 7365 7274 206c 6973        assert lis
-000040e0: 7428 6473 2e61 7474 7273 2920 3d3d 205b  t(ds.attrs) == [
-000040f0: 2263 6f6e 7665 6e74 696f 6e73 222c 2022  "conventions", "
-00004100: 656d 7074 795f 7374 7269 6e67 225d 0a20  empty_string"]. 
-00004110: 2020 2020 2020 2061 7373 6572 7420 6469         assert di
-00004120: 6374 2864 735b 2278 225d 2e61 7474 7273  ct(ds["x"].attrs
-00004130: 2920 3d3d 207b 2275 6e69 7473 223a 2022  ) == {"units": "
-00004140: 6d65 7465 7273 222c 2022 666f 6f22 3a20  meters", "foo": 
-00004150: 2262 6172 227d 0a20 2020 2020 2020 2061  "bar"}.        a
-00004160: 7373 6572 7420 6c65 6e28 6473 5b22 7822  ssert len(ds["x"
-00004170: 5d2e 6174 7472 7329 203d 3d20 320a 2020  ].attrs) == 2.  
-00004180: 2020 2020 2020 6173 7365 7274 2073 6f72        assert sor
-00004190: 7465 6428 6473 5b22 7822 5d2e 6174 7472  ted(ds["x"].attr
-000041a0: 7329 203d 3d20 5b22 666f 6f22 2c20 2275  s) == ["foo", "u
-000041b0: 6e69 7473 225d 0a0a 0a64 6566 2074 6573  nits"]...def tes
-000041c0: 745f 6f70 7469 6f6e 616c 5f6e 6574 6364  t_optional_netcd
-000041d0: 6634 5f61 7474 7273 2874 6d70 5f6c 6f63  f4_attrs(tmp_loc
-000041e0: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-000041f0: 6364 6629 3a0a 2020 2020 6835 203d 2067  cdf):.    h5 = g
-00004200: 6574 5f68 6466 355f 6d6f 6475 6c65 2874  et_hdf5_module(t
-00004210: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
-00004220: 7465 5f6e 6574 6364 6629 0a20 2020 2077  te_netcdf).    w
-00004230: 6974 6820 6835 2e46 696c 6528 746d 705f  ith h5.File(tmp_
-00004240: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-00004250: 6e65 7463 6466 2c20 2277 2229 2061 7320  netcdf, "w") as 
-00004260: 663a 0a20 2020 2020 2020 2066 6f6f 5f64  f:.        foo_d
-00004270: 6174 6120 3d20 6e70 2e61 7261 6e67 6528  ata = np.arange(
-00004280: 3530 292e 7265 7368 6170 6528 352c 2031  50).reshape(5, 1
-00004290: 3029 0a20 2020 2020 2020 2066 2e63 7265  0).        f.cre
-000042a0: 6174 655f 6461 7461 7365 7428 2266 6f6f  ate_dataset("foo
-000042b0: 222c 2064 6174 613d 666f 6f5f 6461 7461  ", data=foo_data
-000042c0: 290a 2020 2020 2020 2020 662e 6372 6561  ).        f.crea
-000042d0: 7465 5f64 6174 6173 6574 2822 7822 2c20  te_dataset("x", 
-000042e0: 6461 7461 3d6e 702e 6172 616e 6765 2835  data=np.arange(5
-000042f0: 2929 0a20 2020 2020 2020 2066 2e63 7265  )).        f.cre
-00004300: 6174 655f 6461 7461 7365 7428 2279 222c  ate_dataset("y",
-00004310: 2064 6174 613d 6e70 2e61 7261 6e67 6528   data=np.arange(
-00004320: 3130 2929 0a20 2020 2020 2020 2069 6620  10)).        if 
-00004330: 7665 7273 696f 6e2e 7061 7273 6528 6835  version.parse(h5
-00004340: 7079 2e5f 5f76 6572 7369 6f6e 5f5f 2920  py.__version__) 
-00004350: 3c20 7665 7273 696f 6e2e 7061 7273 6528  < version.parse(
-00004360: 2232 2e31 302e 3022 293a 0a20 2020 2020  "2.10.0"):.     
-00004370: 2020 2020 2020 2066 5b22 666f 6f22 5d2e         f["foo"].
-00004380: 6469 6d73 2e63 7265 6174 655f 7363 616c  dims.create_scal
-00004390: 6528 665b 2278 225d 290a 2020 2020 2020  e(f["x"]).      
-000043a0: 2020 2020 2020 665b 2266 6f6f 225d 2e64        f["foo"].d
-000043b0: 696d 732e 6372 6561 7465 5f73 6361 6c65  ims.create_scale
-000043c0: 2866 5b22 7922 5d29 0a20 2020 2020 2020  (f["y"]).       
-000043d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000043e0: 2020 2066 5b22 7822 5d2e 6d61 6b65 5f73     f["x"].make_s
-000043f0: 6361 6c65 2829 0a20 2020 2020 2020 2020  cale().         
-00004400: 2020 2066 5b22 7922 5d2e 6d61 6b65 5f73     f["y"].make_s
-00004410: 6361 6c65 2829 0a20 2020 2020 2020 2066  cale().        f
-00004420: 5b22 666f 6f22 5d2e 6469 6d73 5b30 5d2e  ["foo"].dims[0].
-00004430: 6174 7461 6368 5f73 6361 6c65 2866 5b22  attach_scale(f["
-00004440: 7822 5d29 0a20 2020 2020 2020 2066 5b22  x"]).        f["
-00004450: 666f 6f22 5d2e 6469 6d73 5b31 5d2e 6174  foo"].dims[1].at
-00004460: 7461 6368 5f73 6361 6c65 2866 5b22 7922  tach_scale(f["y"
-00004470: 5d29 0a20 2020 2077 6974 6820 6835 6e65  ]).    with h5ne
-00004480: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
-00004490: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
-000044a0: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
-000044b0: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
-000044c0: 2064 735b 2266 6f6f 225d 2e64 696d 656e   ds["foo"].dimen
-000044d0: 7369 6f6e 7320 3d3d 2028 2278 222c 2022  sions == ("x", "
-000044e0: 7922 290a 2020 2020 2020 2020 6173 7365  y").        asse
-000044f0: 7274 2064 732e 6469 6d65 6e73 696f 6e73  rt ds.dimensions
-00004500: 2e6b 6579 7328 2920 3d3d 207b 2278 222c  .keys() == {"x",
-00004510: 2022 7922 7d0a 2020 2020 2020 2020 6173   "y"}.        as
-00004520: 7365 7274 2064 732e 6469 6d65 6e73 696f  sert ds.dimensio
-00004530: 6e73 5b22 7822 5d2e 7369 7a65 203d 3d20  ns["x"].size == 
-00004540: 350a 2020 2020 2020 2020 6173 7365 7274  5.        assert
-00004550: 2064 732e 6469 6d65 6e73 696f 6e73 5b22   ds.dimensions["
-00004560: 7922 5d2e 7369 7a65 203d 3d20 3130 0a20  y"].size == 10. 
-00004570: 2020 2020 2020 2061 7373 6572 7420 6172         assert ar
-00004580: 7261 795f 6571 7561 6c28 6473 5b22 666f  ray_equal(ds["fo
-00004590: 6f22 5d2c 2066 6f6f 5f64 6174 6129 0a0a  o"], foo_data)..
-000045a0: 0a64 6566 2074 6573 745f 6572 726f 725f  .def test_error_
-000045b0: 6861 6e64 6c69 6e67 2874 6d70 5f6c 6f63  handling(tmp_loc
-000045c0: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-000045d0: 6364 6629 3a0a 2020 2020 7769 7468 2068  cdf):.    with h
-000045e0: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-000045f0: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00004600: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
-00004610: 2064 733a 0a20 2020 2020 2020 2064 732e   ds:.        ds.
-00004620: 6469 6d65 6e73 696f 6e73 5b22 7822 5d20  dimensions["x"] 
-00004630: 3d20 310a 2020 2020 2020 2020 7769 7468  = 1.        with
-00004640: 2072 6169 7365 7328 5661 6c75 6545 7272   raises(ValueErr
-00004650: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
-00004660: 2064 732e 6469 6d65 6e73 696f 6e73 5b22   ds.dimensions["
-00004670: 7822 5d20 3d20 320a 2020 2020 2020 2020  x"] = 2.        
-00004680: 7769 7468 2072 6169 7365 7328 5661 6c75  with raises(Valu
-00004690: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
-000046a0: 2020 2020 2064 732e 6469 6d65 6e73 696f       ds.dimensio
-000046b0: 6e73 203d 207b 2278 223a 2032 7d0a 2020  ns = {"x": 2}.  
-000046c0: 2020 2020 2020 7769 7468 2072 6169 7365        with raise
-000046d0: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
-000046e0: 2020 2020 2020 2020 2020 2064 732e 6469             ds.di
-000046f0: 6d65 6e73 696f 6e73 203d 207b 2279 223a  mensions = {"y":
-00004700: 2033 7d0a 2020 2020 2020 2020 6473 2e63   3}.        ds.c
-00004710: 7265 6174 655f 7661 7269 6162 6c65 2822  reate_variable("
-00004720: 7822 2c20 2822 7822 2c29 2c20 6474 7970  x", ("x",), dtyp
-00004730: 653d 666c 6f61 7429 0a20 2020 2020 2020  e=float).       
-00004740: 2077 6974 6820 7261 6973 6573 2856 616c   with raises(Val
-00004750: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
-00004760: 2020 2020 2020 6473 2e63 7265 6174 655f        ds.create_
-00004770: 7661 7269 6162 6c65 2822 7822 2c20 2822  variable("x", ("
-00004780: 7822 2c29 2c20 6474 7970 653d 666c 6f61  x",), dtype=floa
-00004790: 7429 0a20 2020 2020 2020 2064 732e 6372  t).        ds.cr
-000047a0: 6561 7465 5f67 726f 7570 2822 7375 6267  eate_group("subg
-000047b0: 726f 7570 2229 0a20 2020 2020 2020 2077  roup").        w
-000047c0: 6974 6820 7261 6973 6573 2856 616c 7565  ith raises(Value
-000047d0: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-000047e0: 2020 2020 6473 2e63 7265 6174 655f 6772      ds.create_gr
-000047f0: 6f75 7028 2273 7562 6772 6f75 7022 290a  oup("subgroup").
-00004800: 0a0a 4070 7974 6573 742e 6d61 726b 2e73  ..@pytest.mark.s
-00004810: 6b69 7069 6628 0a20 2020 2076 6572 7369  kipif(.    versi
-00004820: 6f6e 2e70 6172 7365 2868 3570 792e 5f5f  on.parse(h5py.__
-00004830: 7665 7273 696f 6e5f 5f29 203c 2076 6572  version__) < ver
-00004840: 7369 6f6e 2e70 6172 7365 2822 332e 302e  sion.parse("3.0.
-00004850: 3022 292c 0a20 2020 2072 6561 736f 6e3d  0"),.    reason=
-00004860: 226e 6f74 206e 6565 6465 6420 7769 7468  "not needed with
-00004870: 2068 3570 7920 3c20 332e 3022 2c0a 290a   h5py < 3.0",.).
-00004880: 6465 6620 7465 7374 5f64 6563 6f64 655f  def test_decode_
-00004890: 7374 7269 6e67 5f65 7272 6f72 2874 6d70  string_error(tmp
-000048a0: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-000048b0: 5f6e 6574 6364 6629 3a0a 2020 2020 7772  _netcdf):.    wr
-000048c0: 6974 655f 6835 6e65 7463 6466 2874 6d70  ite_h5netcdf(tmp
-000048d0: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-000048e0: 5f6e 6574 6364 6629 0a20 2020 2077 6974  _netcdf).    wit
-000048f0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-00004900: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
-00004910: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
-00004920: 662e 6c65 6761 6379 6170 692e 4461 7461  f.legacyapi.Data
-00004930: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
-00004940: 2074 6d70 5f6c 6f63 616c 5f6f 725f 7265   tmp_local_or_re
-00004950: 6d6f 7465 5f6e 6574 6364 662c 2022 7222  mote_netcdf, "r"
-00004960: 2c20 6465 636f 6465 5f76 6c65 6e5f 7374  , decode_vlen_st
-00004970: 7269 6e67 733d 5472 7565 0a20 2020 2020  rings=True.     
-00004980: 2020 2029 2061 7320 6473 3a0a 2020 2020     ) as ds:.    
-00004990: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-000049a0: 732e 6e61 6d65 203d 3d20 222f 220a 0a0a  s.name == "/"...
-000049b0: 6465 6620 6372 6561 7465 5f69 6e76 616c  def create_inval
-000049c0: 6964 5f6e 6574 6364 665f 6461 7461 2829  id_netcdf_data()
-000049d0: 3a0a 2020 2020 666f 6f5f 6461 7461 203d  :.    foo_data =
-000049e0: 206e 702e 6172 616e 6765 2831 3235 292e   np.arange(125).
-000049f0: 7265 7368 6170 6528 352c 2035 2c20 3529  reshape(5, 5, 5)
-00004a00: 0a20 2020 2062 6172 5f64 6174 6120 3d20  .    bar_data = 
-00004a10: 6e70 2e61 7261 6e67 6528 3632 3529 2e72  np.arange(625).r
-00004a20: 6573 6861 7065 2832 352c 2035 2c20 3529  eshape(25, 5, 5)
-00004a30: 0a20 2020 2076 6172 203d 207b 2266 6f6f  .    var = {"foo
-00004a40: 3122 3a20 666f 6f5f 6461 7461 2c20 2266  1": foo_data, "f
-00004a50: 6f6f 3222 3a20 6261 725f 6461 7461 2c20  oo2": bar_data, 
-00004a60: 2266 6f6f 3322 3a20 666f 6f5f 6461 7461  "foo3": foo_data
-00004a70: 2c20 2266 6f6f 3422 3a20 6261 725f 6461  , "foo4": bar_da
-00004a80: 7461 7d0a 2020 2020 7661 7232 203d 207b  ta}.    var2 = {
-00004a90: 2278 223a 2035 2c20 2279 223a 2035 2c20  "x": 5, "y": 5, 
-00004aa0: 227a 223a 2035 2c20 2278 3122 3a20 3235  "z": 5, "x1": 25
-00004ab0: 2c20 2279 3122 3a20 352c 2022 7a31 223a  , "y1": 5, "z1":
-00004ac0: 2035 7d0a 2020 2020 7265 7475 726e 2076   5}.    return v
-00004ad0: 6172 2c20 7661 7232 0a0a 0a64 6566 2063  ar, var2...def c
-00004ae0: 6865 636b 5f69 6e76 616c 6964 5f6e 6574  heck_invalid_net
-00004af0: 6364 6634 2876 6172 2c20 6929 3a0a 2020  cdf4(var, i):.  
-00004b00: 2020 7064 696d 203d 2022 7068 6f6e 795f    pdim = "phony_
-00004b10: 6469 6d5f 7b7d 220a 2020 2020 6173 7365  dim_{}".    asse
-00004b20: 7274 2076 6172 5b22 666f 6f31 225d 2e64  rt var["foo1"].d
-00004b30: 696d 656e 7369 6f6e 735b 305d 203d 3d20  imensions[0] == 
-00004b40: 7064 696d 2e66 6f72 6d61 7428 6920 2a20  pdim.format(i * 
-00004b50: 3429 0a20 2020 2061 7373 6572 7420 7661  4).    assert va
-00004b60: 725b 2266 6f6f 3122 5d2e 6469 6d65 6e73  r["foo1"].dimens
-00004b70: 696f 6e73 5b31 5d20 3d3d 2070 6469 6d2e  ions[1] == pdim.
-00004b80: 666f 726d 6174 2831 202b 2069 202a 2034  format(1 + i * 4
-00004b90: 290a 2020 2020 6173 7365 7274 2076 6172  ).    assert var
-00004ba0: 5b22 666f 6f31 225d 2e64 696d 656e 7369  ["foo1"].dimensi
-00004bb0: 6f6e 735b 325d 203d 3d20 7064 696d 2e66  ons[2] == pdim.f
-00004bc0: 6f72 6d61 7428 3220 2b20 6920 2a20 3429  ormat(2 + i * 4)
-00004bd0: 0a20 2020 2061 7373 6572 7420 7661 725b  .    assert var[
-00004be0: 2266 6f6f 3222 5d2e 6469 6d65 6e73 696f  "foo2"].dimensio
-00004bf0: 6e73 5b30 5d20 3d3d 2070 6469 6d2e 666f  ns[0] == pdim.fo
-00004c00: 726d 6174 2833 202b 2069 202a 2034 290a  rmat(3 + i * 4).
-00004c10: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
-00004c20: 666f 6f32 225d 2e64 696d 656e 7369 6f6e  foo2"].dimension
-00004c30: 735b 315d 203d 3d20 7064 696d 2e66 6f72  s[1] == pdim.for
-00004c40: 6d61 7428 3020 2b20 6920 2a20 3429 0a20  mat(0 + i * 4). 
-00004c50: 2020 2061 7373 6572 7420 7661 725b 2266     assert var["f
-00004c60: 6f6f 3222 5d2e 6469 6d65 6e73 696f 6e73  oo2"].dimensions
-00004c70: 5b32 5d20 3d3d 2070 6469 6d2e 666f 726d  [2] == pdim.form
-00004c80: 6174 2831 202b 2069 202a 2034 290a 2020  at(1 + i * 4).  
-00004c90: 2020 6173 7365 7274 2076 6172 5b22 666f    assert var["fo
-00004ca0: 6f33 225d 2e64 696d 656e 7369 6f6e 735b  o3"].dimensions[
-00004cb0: 305d 203d 3d20 7064 696d 2e66 6f72 6d61  0] == pdim.forma
-00004cc0: 7428 6920 2a20 3429 0a20 2020 2061 7373  t(i * 4).    ass
-00004cd0: 6572 7420 7661 725b 2266 6f6f 3322 5d2e  ert var["foo3"].
-00004ce0: 6469 6d65 6e73 696f 6e73 5b31 5d20 3d3d  dimensions[1] ==
-00004cf0: 2070 6469 6d2e 666f 726d 6174 2831 202b   pdim.format(1 +
-00004d00: 2069 202a 2034 290a 2020 2020 6173 7365   i * 4).    asse
-00004d10: 7274 2076 6172 5b22 666f 6f33 225d 2e64  rt var["foo3"].d
-00004d20: 696d 656e 7369 6f6e 735b 325d 203d 3d20  imensions[2] == 
-00004d30: 7064 696d 2e66 6f72 6d61 7428 3220 2b20  pdim.format(2 + 
-00004d40: 6920 2a20 3429 0a20 2020 2061 7373 6572  i * 4).    asser
-00004d50: 7420 7661 725b 2266 6f6f 3422 5d2e 6469  t var["foo4"].di
-00004d60: 6d65 6e73 696f 6e73 5b30 5d20 3d3d 2070  mensions[0] == p
-00004d70: 6469 6d2e 666f 726d 6174 2833 202b 2069  dim.format(3 + i
-00004d80: 202a 2034 290a 2020 2020 6173 7365 7274   * 4).    assert
-00004d90: 2076 6172 5b22 666f 6f34 225d 2e64 696d   var["foo4"].dim
-00004da0: 656e 7369 6f6e 735b 315d 203d 3d20 7064  ensions[1] == pd
-00004db0: 696d 2e66 6f72 6d61 7428 6920 2a20 3429  im.format(i * 4)
-00004dc0: 0a20 2020 2061 7373 6572 7420 7661 725b  .    assert var[
-00004dd0: 2266 6f6f 3422 5d2e 6469 6d65 6e73 696f  "foo4"].dimensio
-00004de0: 6e73 5b32 5d20 3d3d 2070 6469 6d2e 666f  ns[2] == pdim.fo
-00004df0: 726d 6174 2831 202b 2069 202a 2034 290a  rmat(1 + i * 4).
-00004e00: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
-00004e10: 7822 5d2e 6469 6d65 6e73 696f 6e73 5b30  x"].dimensions[0
-00004e20: 5d20 3d3d 2070 6469 6d2e 666f 726d 6174  ] == pdim.format
-00004e30: 2869 202a 2034 290a 2020 2020 6173 7365  (i * 4).    asse
-00004e40: 7274 2076 6172 5b22 7922 5d2e 6469 6d65  rt var["y"].dime
-00004e50: 6e73 696f 6e73 5b30 5d20 3d3d 2070 6469  nsions[0] == pdi
-00004e60: 6d2e 666f 726d 6174 2869 202a 2034 290a  m.format(i * 4).
-00004e70: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
-00004e80: 7a22 5d2e 6469 6d65 6e73 696f 6e73 5b30  z"].dimensions[0
-00004e90: 5d20 3d3d 2070 6469 6d2e 666f 726d 6174  ] == pdim.format
-00004ea0: 2869 202a 2034 290a 2020 2020 6173 7365  (i * 4).    asse
-00004eb0: 7274 2076 6172 5b22 7831 225d 2e64 696d  rt var["x1"].dim
-00004ec0: 656e 7369 6f6e 735b 305d 203d 3d20 7064  ensions[0] == pd
-00004ed0: 696d 2e66 6f72 6d61 7428 3320 2b20 6920  im.format(3 + i 
-00004ee0: 2a20 3429 0a20 2020 2061 7373 6572 7420  * 4).    assert 
-00004ef0: 7661 725b 2279 3122 5d2e 6469 6d65 6e73  var["y1"].dimens
-00004f00: 696f 6e73 5b30 5d20 3d3d 2070 6469 6d2e  ions[0] == pdim.
-00004f10: 666f 726d 6174 2869 202a 2034 290a 2020  format(i * 4).  
-00004f20: 2020 6173 7365 7274 2076 6172 5b22 7a31    assert var["z1
-00004f30: 225d 2e64 696d 656e 7369 6f6e 735b 305d  "].dimensions[0]
-00004f40: 203d 3d20 7064 696d 2e66 6f72 6d61 7428   == pdim.format(
-00004f50: 6920 2a20 3429 0a0a 0a64 6566 2074 6573  i * 4)...def tes
-00004f60: 745f 696e 7661 6c69 645f 6e65 7463 6466  t_invalid_netcdf
-00004f70: 3428 746d 705f 6c6f 6361 6c5f 6f72 5f72  4(tmp_local_or_r
-00004f80: 656d 6f74 655f 6e65 7463 6466 293a 0a20  emote_netcdf):. 
-00004f90: 2020 2069 6620 746d 705f 6c6f 6361 6c5f     if tmp_local_
-00004fa0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-00004fb0: 2e73 7461 7274 7377 6974 6828 7265 6d6f  .startswith(remo
-00004fc0: 7465 5f68 3529 3a0a 2020 2020 2020 2020  te_h5):.        
-00004fd0: 7079 7465 7374 2e73 6b69 7028 226e 6574  pytest.skip("net
-00004fe0: 4344 4634 2070 6163 6b61 6765 2064 6f65  CDF4 package doe
-00004ff0: 7320 6e6f 7420 776f 726b 2077 6974 6820  s not work with 
-00005000: 7265 6d6f 7465 2048 4446 3520 6669 6c65  remote HDF5 file
-00005010: 7322 290a 2020 2020 6835 203d 2067 6574  s").    h5 = get
-00005020: 5f68 6466 355f 6d6f 6475 6c65 2874 6d70  _hdf5_module(tmp
-00005030: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00005040: 5f6e 6574 6364 6629 0a20 2020 2077 6974  _netcdf).    wit
-00005050: 6820 6835 2e46 696c 6528 746d 705f 6c6f  h h5.File(tmp_lo
-00005060: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
-00005070: 7463 6466 2c20 2277 2229 2061 7320 663a  tcdf, "w") as f:
-00005080: 0a20 2020 2020 2020 2076 6172 2c20 7661  .        var, va
-00005090: 7232 203d 2063 7265 6174 655f 696e 7661  r2 = create_inva
-000050a0: 6c69 645f 6e65 7463 6466 5f64 6174 6128  lid_netcdf_data(
-000050b0: 290a 2020 2020 2020 2020 6772 7073 203d  ).        grps =
-000050c0: 205b 2262 6172 222c 2022 6261 7a22 5d0a   ["bar", "baz"].
-000050d0: 2020 2020 2020 2020 666f 7220 6772 7020          for grp 
-000050e0: 696e 2067 7270 733a 0a20 2020 2020 2020  in grps:.       
-000050f0: 2020 2020 2066 7820 3d20 662e 6372 6561       fx = f.crea
-00005100: 7465 5f67 726f 7570 2867 7270 290a 2020  te_group(grp).  
-00005110: 2020 2020 2020 2020 2020 666f 7220 6b2c            for k,
-00005120: 2076 2069 6e20 7661 722e 6974 656d 7328   v in var.items(
-00005130: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00005140: 2020 2066 782e 6372 6561 7465 5f64 6174     fx.create_dat
-00005150: 6173 6574 286b 2c20 6461 7461 3d76 290a  aset(k, data=v).
-00005160: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00005170: 6b2c 2076 2069 6e20 7661 7232 2e69 7465  k, v in var2.ite
-00005180: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00005190: 2020 2020 2020 6678 2e63 7265 6174 655f        fx.create_
-000051a0: 6461 7461 7365 7428 6b2c 2064 6174 613d  dataset(k, data=
-000051b0: 6e70 2e61 7261 6e67 6528 7629 290a 0a20  np.arange(v)).. 
-000051c0: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-000051d0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-000051e0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-000051f0: 2c20 2272 222c 2070 686f 6e79 5f64 696d  , "r", phony_dim
-00005200: 733d 2273 6f72 7422 2920 6173 2064 7372  s="sort") as dsr
-00005210: 3a0a 2020 2020 2020 2020 666f 7220 692c  :.        for i,
-00005220: 2067 7270 2069 6e20 656e 756d 6572 6174   grp in enumerat
-00005230: 6528 6772 7073 293a 0a20 2020 2020 2020  e(grps):.       
-00005240: 2020 2020 2076 6172 203d 2064 7372 5b67       var = dsr[g
-00005250: 7270 5d2e 7661 7269 6162 6c65 730a 2020  rp].variables.  
-00005260: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
-00005270: 696e 7661 6c69 645f 6e65 7463 6466 3428  invalid_netcdf4(
-00005280: 7661 722c 2069 290a 0a20 2020 2077 6974  var, i)..    wit
-00005290: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-000052a0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-000052b0: 6f74 655f 6e65 7463 6466 2c20 2272 222c  ote_netcdf, "r",
-000052c0: 2070 686f 6e79 5f64 696d 733d 2261 6363   phony_dims="acc
-000052d0: 6573 7322 2920 6173 2064 7372 3a0a 2020  ess") as dsr:.  
-000052e0: 2020 2020 2020 666f 7220 692c 2067 7270        for i, grp
-000052f0: 2069 6e20 656e 756d 6572 6174 6528 6772   in enumerate(gr
-00005300: 7073 293a 0a20 2020 2020 2020 2020 2020  ps):.           
-00005310: 2076 6172 203d 2064 7372 5b67 7270 5d2e   var = dsr[grp].
-00005320: 7661 7269 6162 6c65 730a 2020 2020 2020  variables.      
-00005330: 2020 2020 2020 6368 6563 6b5f 696e 7661        check_inva
-00005340: 6c69 645f 6e65 7463 6466 3428 7661 722c  lid_netcdf4(var,
-00005350: 2069 290a 0a20 2020 2069 6620 6e6f 7420   i)..    if not 
-00005360: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00005370: 6f74 655f 6e65 7463 6466 2e73 7461 7274  ote_netcdf.start
-00005380: 7377 6974 6828 7265 6d6f 7465 5f68 3529  swith(remote_h5)
-00005390: 3a0a 2020 2020 2020 2020 2320 6e65 7463  :.        # netc
-000053a0: 6466 3420 7061 636b 6167 6520 646f 6573  df4 package does
-000053b0: 206e 6f74 2077 6f72 6b20 7769 7468 2072   not work with r
-000053c0: 656d 6f74 6520 4844 4635 2066 696c 6573  emote HDF5 files
-000053d0: 0a20 2020 2020 2020 2077 6974 6820 6e65  .        with ne
-000053e0: 7443 4446 342e 4461 7461 7365 7428 746d  tCDF4.Dataset(tm
-000053f0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
-00005400: 655f 6e65 7463 6466 2c20 2272 2229 2061  e_netcdf, "r") a
-00005410: 7320 6473 723a 0a20 2020 2020 2020 2020  s dsr:.         
-00005420: 2020 2066 6f72 2069 2c20 6772 7020 696e     for i, grp in
-00005430: 2065 6e75 6d65 7261 7465 2867 7270 7329   enumerate(grps)
-00005440: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005450: 2020 7661 7220 3d20 6473 725b 6772 705d    var = dsr[grp]
-00005460: 2e76 6172 6961 626c 6573 0a20 2020 2020  .variables.     
-00005470: 2020 2020 2020 2020 2020 2063 6865 636b             check
-00005480: 5f69 6e76 616c 6964 5f6e 6574 6364 6634  _invalid_netcdf4
-00005490: 2876 6172 2c20 6929 0a0a 2020 2020 7769  (var, i)..    wi
-000054a0: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-000054b0: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
-000054c0: 6d6f 7465 5f6e 6574 6364 662c 2022 7222  mote_netcdf, "r"
-000054d0: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-000054e0: 2077 6974 6820 7261 6973 6573 2856 616c   with raises(Val
-000054f0: 7565 4572 726f 7229 3a0a 2020 2020 2020  ueError):.      
-00005500: 2020 2020 2020 6473 5b22 6261 7222 5d2e        ds["bar"].
-00005510: 7661 7269 6162 6c65 735b 2266 6f6f 3122  variables["foo1"
-00005520: 5d2e 6469 6d65 6e73 696f 6e73 0a0a 2020  ].dimensions..  
-00005530: 2020 7769 7468 2072 6169 7365 7328 5661    with raises(Va
-00005540: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+00000e00: 7363 616c 6172 222c 206e 702e 666c 6f61  scalar", np.floa
+00000e10: 7433 322c 2028 2929 0a20 2020 2076 5b2e  t32, ()).    v[.
+00000e20: 2e2e 5d20 3d20 322e 300a 0a20 2020 2023  ..] = 2.0..    #
+00000e30: 2074 6573 7420 6372 6561 7469 6e67 2061   test creating a
+00000e40: 2073 6361 6c61 7220 7769 7468 2063 6f6d   scalar with com
+00000e50: 7072 6573 7369 6f6e 206f 7074 696f 6e20  pression option 
+00000e60: 2877 6974 6820 7368 6f75 6c64 2062 6520  (with should be 
+00000e70: 6967 6e6f 7265 6429 0a20 2020 2076 203d  ignored).    v =
+00000e80: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
+00000e90: 6c65 2822 696e 7473 6361 6c61 7222 2c20  le("intscalar", 
+00000ea0: 6e70 2e69 6e74 3634 2c20 2829 2c20 7a6c  np.int64, (), zl
+00000eb0: 6962 3d36 2c20 6669 6c6c 5f76 616c 7565  ib=6, fill_value
+00000ec0: 3d4e 6f6e 6529 0a20 2020 2076 5b2e 2e2e  =None).    v[...
+00000ed0: 5d20 3d20 320a 0a20 2020 2076 203d 2064  ] = 2..    v = d
+00000ee0: 732e 6372 6561 7465 5661 7269 6162 6c65  s.createVariable
+00000ef0: 2822 666f 6f5f 756e 6c69 6d69 7465 6422  ("foo_unlimited"
+00000f00: 2c20 666c 6f61 742c 2028 2278 222c 2022  , float, ("x", "
+00000f10: 756e 6c69 6d69 7465 6422 2929 0a20 2020  unlimited")).   
+00000f20: 2076 5b2e 2e2e 5d20 3d20 310a 0a20 2020   v[...] = 1..   
+00000f30: 2077 6974 6820 7261 6973 6573 2828 6835   with raises((h5
+00000f40: 6e65 7463 6466 2e43 6f6d 7061 7469 6269  netcdf.Compatibi
+00000f50: 6c69 7479 4572 726f 722c 2054 7970 6545  lityError, TypeE
+00000f60: 7272 6f72 2929 3a0a 2020 2020 2020 2020  rror)):.        
+00000f70: 6473 2e63 7265 6174 6556 6172 6961 626c  ds.createVariabl
+00000f80: 6528 2262 6f6f 6c65 616e 222c 206e 702e  e("boolean", np.
+00000f90: 626f 6f6c 5f2c 2028 2278 2229 290a 0a20  bool_, ("x")).. 
+00000fa0: 2020 2067 203d 2064 732e 6372 6561 7465     g = ds.create
+00000fb0: 4772 6f75 7028 2273 7562 6772 6f75 7022  Group("subgroup"
+00000fc0: 290a 2020 2020 7620 3d20 672e 6372 6561  ).    v = g.crea
+00000fd0: 7465 5661 7269 6162 6c65 2822 7375 6276  teVariable("subv
+00000fe0: 6172 222c 206e 702e 696e 7433 322c 2028  ar", np.int32, (
+00000ff0: 2278 222c 2929 0a20 2020 2076 5b2e 2e2e  "x",)).    v[...
+00001000: 5d20 3d20 6e70 2e61 7261 6e67 6528 342e  ] = np.arange(4.
+00001010: 3029 0a0a 2020 2020 672e 6372 6561 7465  0)..    g.create
+00001020: 4469 6d65 6e73 696f 6e28 2279 222c 2031  Dimension("y", 1
+00001030: 3029 0a20 2020 2067 2e63 7265 6174 6556  0).    g.createV
+00001040: 6172 6961 626c 6528 2279 5f76 6172 222c  ariable("y_var",
+00001050: 2066 6c6f 6174 2c20 2822 7922 2c29 290a   float, ("y",)).
+00001060: 0a20 2020 2064 732e 6372 6561 7465 4469  .    ds.createDi
+00001070: 6d65 6e73 696f 6e28 226d 6973 6d61 7463  mension("mismatc
+00001080: 6865 645f 6469 6d22 2c20 3129 0a20 2020  hed_dim", 1).   
+00001090: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
+000010a0: 6c65 2822 6d69 736d 6174 6368 6564 5f64  le("mismatched_d
+000010b0: 696d 222c 2069 6e74 2c20 2829 290a 0a20  im", int, ()).. 
+000010c0: 2020 2076 203d 2064 732e 6372 6561 7465     v = ds.create
+000010d0: 5661 7269 6162 6c65 2822 7661 725f 6c65  Variable("var_le
+000010e0: 6e5f 7374 7222 2c20 7374 722c 2028 2278  n_str", str, ("x
+000010f0: 2229 290a 2020 2020 765b 305d 203d 2022  ")).    v[0] = "
+00001100: 666f 6f22 0a0a 2020 2020 6473 2e63 6c6f  foo"..    ds.clo
+00001110: 7365 2829 0a0a 0a64 6566 2077 7269 7465  se()...def write
+00001120: 5f68 356e 6574 6364 6628 746d 705f 6e65  _h5netcdf(tmp_ne
+00001130: 7463 6466 293a 0a20 2020 2064 7320 3d20  tcdf):.    ds = 
+00001140: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
+00001150: 705f 6e65 7463 6466 2c20 2277 2229 0a20  p_netcdf, "w"). 
+00001160: 2020 2064 732e 6174 7472 735b 2267 6c6f     ds.attrs["glo
+00001170: 6261 6c22 5d20 3d20 3432 0a20 2020 2064  bal"] = 42.    d
+00001180: 732e 6174 7472 735b 226f 7468 6572 5f61  s.attrs["other_a
+00001190: 7474 7222 5d20 3d20 2279 6573 220a 2020  ttr"] = "yes".  
+000011a0: 2020 6473 2e64 696d 656e 7369 6f6e 7320    ds.dimensions 
+000011b0: 3d20 7b22 7822 3a20 342c 2022 7922 3a20  = {"x": 4, "y": 
+000011c0: 352c 2022 7a22 3a20 362c 2022 656d 7074  5, "z": 6, "empt
+000011d0: 7922 3a20 302c 2022 756e 6c69 6d69 7465  y": 0, "unlimite
+000011e0: 6422 3a20 4e6f 6e65 7d0a 0a20 2020 2076  d": None}..    v
+000011f0: 203d 2064 732e 6372 6561 7465 5f76 6172   = ds.create_var
+00001200: 6961 626c 6528 0a20 2020 2020 2020 2022  iable(.        "
+00001210: 666f 6f22 2c20 2822 7822 2c20 2279 2229  foo", ("x", "y")
+00001220: 2c20 666c 6f61 742c 2063 6875 6e6b 733d  , float, chunks=
+00001230: 2834 2c20 3529 2c20 636f 6d70 7265 7373  (4, 5), compress
+00001240: 696f 6e3d 2267 7a69 7022 2c20 7368 7566  ion="gzip", shuf
+00001250: 666c 653d 5472 7565 0a20 2020 2029 0a20  fle=True.    ). 
+00001260: 2020 2076 5b2e 2e2e 5d20 3d20 310a 2020     v[...] = 1.  
+00001270: 2020 762e 6174 7472 735b 2275 6e69 7473    v.attrs["units
+00001280: 225d 203d 2022 6d65 7465 7273 220a 0a20  "] = "meters".. 
+00001290: 2020 2072 656d 6f74 655f 6669 6c65 203d     remote_file =
+000012a0: 2069 7369 6e73 7461 6e63 6528 746d 705f   isinstance(tmp_
+000012b0: 6e65 7463 6466 2c20 7374 7229 2061 6e64  netcdf, str) and
+000012c0: 2074 6d70 5f6e 6574 6364 662e 7374 6172   tmp_netcdf.star
+000012d0: 7473 7769 7468 2872 656d 6f74 655f 6835  tswith(remote_h5
+000012e0: 290a 2020 2020 6966 206e 6f74 2072 656d  ).    if not rem
+000012f0: 6f74 655f 6669 6c65 3a0a 2020 2020 2020  ote_file:.      
+00001300: 2020 7620 3d20 6473 2e63 7265 6174 655f    v = ds.create_
+00001310: 7661 7269 6162 6c65 2822 7922 2c20 2822  variable("y", ("
+00001320: 7922 2c29 2c20 696e 742c 2066 696c 6c76  y",), int, fillv
+00001330: 616c 7565 3d2d 3129 0a20 2020 2020 2020  alue=-1).       
+00001340: 2076 5b3a 345d 203d 206e 702e 6172 616e   v[:4] = np.aran
+00001350: 6765 2834 290a 0a20 2020 2076 203d 2064  ge(4)..    v = d
+00001360: 732e 6372 6561 7465 5f76 6172 6961 626c  s.create_variabl
+00001370: 6528 227a 222c 2028 227a 222c 2022 7374  e("z", ("z", "st
+00001380: 7269 6e67 3322 292c 2064 6174 613d 5f63  ring3"), data=_c
+00001390: 6861 725f 6172 7261 792c 2066 696c 6c76  har_array, fillv
+000013a0: 616c 7565 3d62 2258 2229 0a0a 2020 2020  alue=b"X")..    
+000013b0: 7620 3d20 6473 2e63 7265 6174 655f 7661  v = ds.create_va
+000013c0: 7269 6162 6c65 2822 7363 616c 6172 222c  riable("scalar",
+000013d0: 2064 6174 613d 6e70 2e66 6c6f 6174 3332   data=np.float32
+000013e0: 2832 2e30 2929 0a0a 2020 2020 7620 3d20  (2.0))..    v = 
+000013f0: 6473 2e63 7265 6174 655f 7661 7269 6162  ds.create_variab
+00001400: 6c65 2822 696e 7473 6361 6c61 7222 2c20  le("intscalar", 
+00001410: 6461 7461 3d6e 702e 696e 7436 3428 3229  data=np.int64(2)
+00001420: 290a 0a20 2020 2076 203d 2064 732e 6372  )..    v = ds.cr
+00001430: 6561 7465 5f76 6172 6961 626c 6528 2266  eate_variable("f
+00001440: 6f6f 5f75 6e6c 696d 6974 6564 222c 2028  oo_unlimited", (
+00001450: 2278 222c 2022 756e 6c69 6d69 7465 6422  "x", "unlimited"
+00001460: 292c 2066 6c6f 6174 290a 2020 2020 765b  ), float).    v[
+00001470: 2e2e 2e5d 203d 2031 0a0a 2020 2020 7769  ...] = 1..    wi
+00001480: 7468 2072 6169 7365 7328 2868 356e 6574  th raises((h5net
+00001490: 6364 662e 436f 6d70 6174 6962 696c 6974  cdf.Compatibilit
+000014a0: 7945 7272 6f72 2c20 5479 7065 4572 726f  yError, TypeErro
+000014b0: 7229 293a 0a20 2020 2020 2020 2064 732e  r)):.        ds.
+000014c0: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+000014d0: 2262 6f6f 6c65 616e 222c 2064 6174 613d  "boolean", data=
+000014e0: 5472 7565 290a 0a20 2020 2067 203d 2064  True)..    g = d
+000014f0: 732e 6372 6561 7465 5f67 726f 7570 2822  s.create_group("
+00001500: 7375 6267 726f 7570 2229 0a20 2020 2076  subgroup").    v
+00001510: 203d 2067 2e63 7265 6174 655f 7661 7269   = g.create_vari
+00001520: 6162 6c65 2822 7375 6276 6172 222c 2028  able("subvar", (
+00001530: 2278 222c 292c 206e 702e 696e 7433 3229  "x",), np.int32)
+00001540: 0a20 2020 2076 5b2e 2e2e 5d20 3d20 6e70  .    v[...] = np
+00001550: 2e61 7261 6e67 6528 342e 3029 0a20 2020  .arange(4.0).   
+00001560: 2077 6974 6820 7261 6973 6573 2841 7474   with raises(Att
+00001570: 7269 6275 7465 4572 726f 7229 3a0a 2020  ributeError):.  
+00001580: 2020 2020 2020 762e 6174 7472 735b 225f        v.attrs["_
+00001590: 4e65 7463 6466 3444 696d 6964 225d 203d  Netcdf4Dimid"] =
+000015a0: 202d 310a 0a20 2020 2067 2e64 696d 656e   -1..    g.dimen
+000015b0: 7369 6f6e 735b 2279 225d 203d 2031 300a  sions["y"] = 10.
+000015c0: 2020 2020 672e 6372 6561 7465 5f76 6172      g.create_var
+000015d0: 6961 626c 6528 2279 5f76 6172 222c 2028  iable("y_var", (
+000015e0: 2279 222c 292c 2066 6c6f 6174 290a 2020  "y",), float).  
+000015f0: 2020 672e 666c 7573 6828 290a 0a20 2020    g.flush()..   
+00001600: 2064 732e 6469 6d65 6e73 696f 6e73 5b22   ds.dimensions["
+00001610: 6d69 736d 6174 6368 6564 5f64 696d 225d  mismatched_dim"]
+00001620: 203d 2031 0a20 2020 2064 732e 6372 6561   = 1.    ds.crea
+00001630: 7465 5f76 6172 6961 626c 6528 226d 6973  te_variable("mis
+00001640: 6d61 7463 6865 645f 6469 6d22 2c20 6474  matched_dim", dt
+00001650: 7970 653d 696e 7429 0a20 2020 2064 732e  ype=int).    ds.
+00001660: 666c 7573 6828 290a 0a20 2020 2064 7420  flush()..    dt 
+00001670: 3d20 6835 7079 2e73 7065 6369 616c 5f64  = h5py.special_d
+00001680: 7479 7065 2876 6c65 6e3d 7374 7229 0a20  type(vlen=str). 
+00001690: 2020 2076 203d 2064 732e 6372 6561 7465     v = ds.create
+000016a0: 5f76 6172 6961 626c 6528 2276 6172 5f6c  _variable("var_l
+000016b0: 656e 5f73 7472 222c 2028 2278 222c 292c  en_str", ("x",),
+000016c0: 2064 7479 7065 3d64 7429 0a20 2020 2076   dtype=dt).    v
+000016d0: 5b30 5d20 3d20 5f76 6c65 6e5f 7374 7269  [0] = _vlen_stri
+000016e0: 6e67 0a0a 2020 2020 6473 2e63 6c6f 7365  ng..    ds.close
+000016f0: 2829 0a0a 0a64 6566 2072 6561 645f 6c65  ()...def read_le
+00001700: 6761 6379 5f6e 6574 6364 6628 746d 705f  gacy_netcdf(tmp_
+00001710: 6e65 7463 6466 2c20 7265 6164 5f6d 6f64  netcdf, read_mod
+00001720: 756c 652c 2077 7269 7465 5f6d 6f64 756c  ule, write_modul
+00001730: 6529 3a0a 2020 2020 6473 203d 2072 6561  e):.    ds = rea
+00001740: 645f 6d6f 6475 6c65 2e44 6174 6173 6574  d_module.Dataset
+00001750: 2874 6d70 5f6e 6574 6364 662c 2022 7222  (tmp_netcdf, "r"
+00001760: 290a 2020 2020 6173 7365 7274 2064 732e  ).    assert ds.
+00001770: 6e63 6174 7472 7328 2920 3d3d 205b 2267  ncattrs() == ["g
+00001780: 6c6f 6261 6c22 2c20 226f 7468 6572 5f61  lobal", "other_a
+00001790: 7474 7222 5d0a 2020 2020 6173 7365 7274  ttr"].    assert
+000017a0: 2064 732e 6765 746e 6361 7474 7228 2267   ds.getncattr("g
+000017b0: 6c6f 6261 6c22 2920 3d3d 2034 320a 2020  lobal") == 42.  
+000017c0: 2020 6966 2077 7269 7465 5f6d 6f64 756c    if write_modul
+000017d0: 6520 6973 206e 6f74 206e 6574 4344 4634  e is not netCDF4
+000017e0: 3a0a 2020 2020 2020 2020 2320 736b 6970  :.        # skip
+000017f0: 2066 6f72 206e 6f77 3a20 6874 7470 733a   for now: https:
+00001800: 2f2f 6769 7468 7562 2e63 6f6d 2f55 6e69  //github.com/Uni
+00001810: 6461 7461 2f6e 6574 6364 6634 2d70 7974  data/netcdf4-pyt
+00001820: 686f 6e2f 6973 7375 6573 2f33 3838 0a20  hon/issues/388. 
+00001830: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00001840: 2e6f 7468 6572 5f61 7474 7220 3d3d 2022  .other_attr == "
+00001850: 7965 7322 0a20 2020 2077 6974 6820 7079  yes".    with py
+00001860: 7465 7374 2e72 6169 7365 7328 4174 7472  test.raises(Attr
+00001870: 6962 7574 6545 7272 6f72 293a 0a20 2020  ibuteError):.   
+00001880: 2020 2020 2064 732e 646f 6573 5f6e 6f74       ds.does_not
+00001890: 5f65 7869 7374 0a20 2020 2061 7373 6572  _exist.    asser
+000018a0: 7420 7365 7428 6473 2e64 696d 656e 7369  t set(ds.dimensi
+000018b0: 6f6e 7329 203d 3d20 7365 7428 0a20 2020  ons) == set(.   
+000018c0: 2020 2020 205b 2278 222c 2022 7922 2c20       ["x", "y", 
+000018d0: 227a 222c 2022 656d 7074 7922 2c20 2273  "z", "empty", "s
+000018e0: 7472 696e 6733 222c 2022 6d69 736d 6174  tring3", "mismat
+000018f0: 6368 6564 5f64 696d 222c 2022 756e 6c69  ched_dim", "unli
+00001900: 6d69 7465 6422 5d0a 2020 2020 290a 2020  mited"].    ).  
+00001910: 2020 6173 7365 7274 2073 6574 2864 732e    assert set(ds.
+00001920: 7661 7269 6162 6c65 7329 203d 3d20 7365  variables) == se
+00001930: 7428 0a20 2020 2020 2020 205b 0a20 2020  t(.        [.   
+00001940: 2020 2020 2020 2020 2022 666f 6f22 2c0a           "foo",.
+00001950: 2020 2020 2020 2020 2020 2020 2279 222c              "y",
+00001960: 0a20 2020 2020 2020 2020 2020 2022 7a22  .            "z"
+00001970: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+00001980: 6e74 7363 616c 6172 222c 0a20 2020 2020  ntscalar",.     
+00001990: 2020 2020 2020 2022 7363 616c 6172 222c         "scalar",
+000019a0: 0a20 2020 2020 2020 2020 2020 2022 7661  .            "va
+000019b0: 725f 6c65 6e5f 7374 7222 2c0a 2020 2020  r_len_str",.    
+000019c0: 2020 2020 2020 2020 226d 6973 6d61 7463          "mismatc
+000019d0: 6865 645f 6469 6d22 2c0a 2020 2020 2020  hed_dim",.      
+000019e0: 2020 2020 2020 2266 6f6f 5f75 6e6c 696d        "foo_unlim
+000019f0: 6974 6564 222c 0a20 2020 2020 2020 205d  ited",.        ]
+00001a00: 0a20 2020 2029 0a0a 2020 2020 6173 7365  .    )..    asse
+00001a10: 7274 2073 6574 2864 732e 6772 6f75 7073  rt set(ds.groups
+00001a20: 2920 3d3d 2073 6574 285b 2273 7562 6772  ) == set(["subgr
+00001a30: 6f75 7022 5d29 0a20 2020 2061 7373 6572  oup"]).    asser
+00001a40: 7420 6473 2e70 6172 656e 7420 6973 204e  t ds.parent is N
+00001a50: 6f6e 650a 2020 2020 7620 3d20 6473 2e76  one.    v = ds.v
+00001a60: 6172 6961 626c 6573 5b22 666f 6f22 5d0a  ariables["foo"].
+00001a70: 2020 2020 6173 7365 7274 2061 7272 6179      assert array
+00001a80: 5f65 7175 616c 2876 2c20 6e70 2e6f 6e65  _equal(v, np.one
+00001a90: 7328 2834 2c20 3529 2929 0a20 2020 2061  s((4, 5))).    a
+00001aa0: 7373 6572 7420 762e 6474 7970 6520 3d3d  ssert v.dtype ==
+00001ab0: 2066 6c6f 6174 0a20 2020 2061 7373 6572   float.    asser
+00001ac0: 7420 762e 6469 6d65 6e73 696f 6e73 203d  t v.dimensions =
+00001ad0: 3d20 2822 7822 2c20 2279 2229 0a20 2020  = ("x", "y").   
+00001ae0: 2061 7373 6572 7420 762e 6e64 696d 203d   assert v.ndim =
+00001af0: 3d20 320a 2020 2020 6173 7365 7274 2076  = 2.    assert v
+00001b00: 2e6e 6361 7474 7273 2829 203d 3d20 5b22  .ncattrs() == ["
+00001b10: 756e 6974 7322 5d0a 2020 2020 6966 2077  units"].    if w
+00001b20: 7269 7465 5f6d 6f64 756c 6520 6973 206e  rite_module is n
+00001b30: 6f74 206e 6574 4344 4634 3a0a 2020 2020  ot netCDF4:.    
+00001b40: 2020 2020 6173 7365 7274 2076 2e67 6574      assert v.get
+00001b50: 6e63 6174 7472 2822 756e 6974 7322 2920  ncattr("units") 
+00001b60: 3d3d 2022 6d65 7465 7273 220a 2020 2020  == "meters".    
+00001b70: 6173 7365 7274 2074 7570 6c65 2876 2e63  assert tuple(v.c
+00001b80: 6875 6e6b 696e 6728 2929 203d 3d20 2834  hunking()) == (4
+00001b90: 2c20 3529 0a0a 2020 2020 2320 6368 6563  , 5)..    # chec
+00001ba0: 6b20 666f 7220 6469 6374 2069 7465 6d73  k for dict items
+00001bb0: 2073 6570 6172 6174 656c 790a 2020 2020   separately.    
+00001bc0: 2320 7365 6520 6874 7470 733a 2f2f 6769  # see https://gi
+00001bd0: 7468 7562 2e63 6f6d 2f68 356e 6574 6364  thub.com/h5netcd
+00001be0: 662f 6835 6e65 7463 6466 2f69 7373 7565  f/h5netcdf/issue
+00001bf0: 732f 3137 310a 2020 2020 6669 6c74 6572  s/171.    filter
+00001c00: 7320 3d20 762e 6669 6c74 6572 7328 290a  s = v.filters().
+00001c10: 2020 2020 6173 7365 7274 2066 696c 7465      assert filte
+00001c20: 7273 5b22 636f 6d70 6c65 7665 6c22 5d20  rs["complevel"] 
+00001c30: 3d3d 2034 0a20 2020 2061 7373 6572 7420  == 4.    assert 
+00001c40: 6669 6c74 6572 735b 2266 6c65 7463 6865  filters["fletche
+00001c50: 7233 3222 5d20 6973 2046 616c 7365 0a20  r32"] is False. 
+00001c60: 2020 2061 7373 6572 7420 6669 6c74 6572     assert filter
+00001c70: 735b 2273 6875 6666 6c65 225d 2069 7320  s["shuffle"] is 
+00001c80: 5472 7565 0a20 2020 2061 7373 6572 7420  True.    assert 
+00001c90: 6669 6c74 6572 735b 227a 6c69 6222 5d20  filters["zlib"] 
+00001ca0: 6973 2054 7275 650a 0a20 2020 2076 203d  is True..    v =
+00001cb0: 2064 732e 7661 7269 6162 6c65 735b 2279   ds.variables["y
+00001cc0: 225d 0a20 2020 2061 7373 6572 7420 6172  "].    assert ar
+00001cd0: 7261 795f 6571 7561 6c28 762c 206e 702e  ray_equal(v, np.
+00001ce0: 725f 5b6e 702e 6172 616e 6765 2834 292c  r_[np.arange(4),
+00001cf0: 205b 2d31 5d5d 290a 2020 2020 6173 7365   [-1]]).    asse
+00001d00: 7274 2076 2e64 7479 7065 203d 3d20 696e  rt v.dtype == in
+00001d10: 740a 2020 2020 6173 7365 7274 2076 2e64  t.    assert v.d
+00001d20: 696d 656e 7369 6f6e 7320 3d3d 2028 2279  imensions == ("y
+00001d30: 222c 290a 2020 2020 6173 7365 7274 2076  ",).    assert v
+00001d40: 2e6e 6469 6d20 3d3d 2031 0a20 2020 2061  .ndim == 1.    a
+00001d50: 7373 6572 7420 762e 6e63 6174 7472 7328  ssert v.ncattrs(
+00001d60: 2920 3d3d 205b 225f 4669 6c6c 5661 6c75  ) == ["_FillValu
+00001d70: 6522 5d0a 2020 2020 6173 7365 7274 2076  e"].    assert v
+00001d80: 2e67 6574 6e63 6174 7472 2822 5f46 696c  .getncattr("_Fil
+00001d90: 6c56 616c 7565 2229 203d 3d20 2d31 0a20  lValue") == -1. 
+00001da0: 2020 2061 7373 6572 7420 762e 6368 756e     assert v.chun
+00001db0: 6b69 6e67 2829 203d 3d20 2263 6f6e 7469  king() == "conti
+00001dc0: 6775 6f75 7322 0a0a 2020 2020 2320 6368  guous"..    # ch
+00001dd0: 6563 6b20 666f 7220 6469 6374 2069 7465  eck for dict ite
+00001de0: 6d73 2073 6570 6172 6174 656c 790a 2020  ms separately.  
+00001df0: 2020 2320 7365 6520 6874 7470 733a 2f2f    # see https://
+00001e00: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
+00001e10: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
+00001e20: 7565 732f 3137 310a 2020 2020 6669 6c74  ues/171.    filt
+00001e30: 6572 7320 3d20 762e 6669 6c74 6572 7328  ers = v.filters(
+00001e40: 290a 2020 2020 6173 7365 7274 2066 696c  ).    assert fil
+00001e50: 7465 7273 5b22 636f 6d70 6c65 7665 6c22  ters["complevel"
+00001e60: 5d20 3d3d 2030 0a20 2020 2061 7373 6572  ] == 0.    asser
+00001e70: 7420 6669 6c74 6572 735b 2266 6c65 7463  t filters["fletc
+00001e80: 6865 7233 3222 5d20 6973 2046 616c 7365  her32"] is False
+00001e90: 0a20 2020 2061 7373 6572 7420 6669 6c74  .    assert filt
+00001ea0: 6572 735b 2273 6875 6666 6c65 225d 2069  ers["shuffle"] i
+00001eb0: 7320 4661 6c73 650a 2020 2020 6173 7365  s False.    asse
+00001ec0: 7274 2066 696c 7465 7273 5b22 7a6c 6962  rt filters["zlib
+00001ed0: 225d 2069 7320 4661 6c73 650a 0a20 2020  "] is False..   
+00001ee0: 2064 732e 636c 6f73 6528 290a 0a20 2020   ds.close()..   
+00001ef0: 2023 2043 6865 636b 2074 6865 2062 6568   # Check the beh
+00001f00: 6176 696f 7220 6966 2068 3570 792e 2043  avior if h5py. C
+00001f10: 616e 6e6f 7420 6578 7065 6374 2068 356e  annot expect h5n
+00001f20: 6574 6364 6620 746f 206f 7665 7263 6f6d  etcdf to overcom
+00001f30: 6520 7468 6573 650a 2020 2020 2320 6572  e these.    # er
+00001f40: 726f 7273 3a0a 2020 2020 6966 2069 735f  rors:.    if is_
+00001f50: 6835 7079 5f63 6861 725f 776f 726b 696e  h5py_char_workin
+00001f60: 6728 746d 705f 6e65 7463 6466 2c20 227a  g(tmp_netcdf, "z
+00001f70: 2229 3a0a 2020 2020 2020 2020 6473 203d  "):.        ds =
+00001f80: 2072 6561 645f 6d6f 6475 6c65 2e44 6174   read_module.Dat
+00001f90: 6173 6574 2874 6d70 5f6e 6574 6364 662c  aset(tmp_netcdf,
+00001fa0: 2022 7222 290a 2020 2020 2020 2020 7620   "r").        v 
+00001fb0: 3d20 6473 2e76 6172 6961 626c 6573 5b22  = ds.variables["
+00001fc0: 7a22 5d0a 2020 2020 2020 2020 6173 7365  z"].        asse
+00001fd0: 7274 2061 7272 6179 5f65 7175 616c 2876  rt array_equal(v
+00001fe0: 2c20 5f63 6861 725f 6172 7261 7929 0a20  , _char_array). 
+00001ff0: 2020 2020 2020 2061 7373 6572 7420 762e         assert v.
+00002000: 6474 7970 6520 3d3d 2022 5331 220a 2020  dtype == "S1".  
+00002010: 2020 2020 2020 6173 7365 7274 2076 2e6e        assert v.n
+00002020: 6469 6d20 3d3d 2032 0a20 2020 2020 2020  dim == 2.       
+00002030: 2061 7373 6572 7420 762e 6469 6d65 6e73   assert v.dimens
+00002040: 696f 6e73 203d 3d20 2822 7a22 2c20 2273  ions == ("z", "s
+00002050: 7472 696e 6733 2229 0a20 2020 2020 2020  tring3").       
+00002060: 2061 7373 6572 7420 762e 6e63 6174 7472   assert v.ncattr
+00002070: 7328 2920 3d3d 205b 225f 4669 6c6c 5661  s() == ["_FillVa
+00002080: 6c75 6522 5d0a 2020 2020 2020 2020 6173  lue"].        as
+00002090: 7365 7274 2076 2e67 6574 6e63 6174 7472  sert v.getncattr
+000020a0: 2822 5f46 696c 6c56 616c 7565 2229 203d  ("_FillValue") =
+000020b0: 3d20 6222 5822 0a20 2020 2065 6c73 653a  = b"X".    else:
+000020c0: 0a20 2020 2020 2020 2064 7320 3d20 7265  .        ds = re
+000020d0: 6164 5f6d 6f64 756c 652e 4461 7461 7365  ad_module.Datase
+000020e0: 7428 746d 705f 6e65 7463 6466 2c20 2272  t(tmp_netcdf, "r
+000020f0: 2229 0a0a 2020 2020 7620 3d20 6473 2e76  ")..    v = ds.v
+00002100: 6172 6961 626c 6573 5b22 7363 616c 6172  ariables["scalar
+00002110: 225d 0a20 2020 2061 7373 6572 7420 6172  "].    assert ar
+00002120: 7261 795f 6571 7561 6c28 762c 206e 702e  ray_equal(v, np.
+00002130: 6172 7261 7928 322e 3029 290a 2020 2020  array(2.0)).    
+00002140: 6173 7365 7274 2076 2e64 7479 7065 203d  assert v.dtype =
+00002150: 3d20 2266 6c6f 6174 3332 220a 2020 2020  = "float32".    
+00002160: 6173 7365 7274 2076 2e6e 6469 6d20 3d3d  assert v.ndim ==
+00002170: 2030 0a20 2020 2061 7373 6572 7420 762e   0.    assert v.
+00002180: 6469 6d65 6e73 696f 6e73 203d 3d20 2829  dimensions == ()
+00002190: 0a20 2020 2061 7373 6572 7420 762e 6e63  .    assert v.nc
+000021a0: 6174 7472 7328 2920 3d3d 205b 5d0a 0a20  attrs() == [].. 
+000021b0: 2020 2076 203d 2064 732e 7661 7269 6162     v = ds.variab
+000021c0: 6c65 735b 2269 6e74 7363 616c 6172 225d  les["intscalar"]
+000021d0: 0a20 2020 2061 7373 6572 7420 6172 7261  .    assert arra
+000021e0: 795f 6571 7561 6c28 762c 206e 702e 6172  y_equal(v, np.ar
+000021f0: 7261 7928 3229 290a 2020 2020 6173 7365  ray(2)).    asse
+00002200: 7274 2076 2e64 7479 7065 203d 3d20 2269  rt v.dtype == "i
+00002210: 6e74 3634 220a 2020 2020 6173 7365 7274  nt64".    assert
+00002220: 2076 2e6e 6469 6d20 3d3d 2030 0a20 2020   v.ndim == 0.   
+00002230: 2061 7373 6572 7420 762e 6469 6d65 6e73   assert v.dimens
+00002240: 696f 6e73 203d 3d20 2829 0a20 2020 2061  ions == ().    a
+00002250: 7373 6572 7420 762e 6e63 6174 7472 7328  ssert v.ncattrs(
+00002260: 2920 3d3d 205b 5d0a 0a20 2020 2076 203d  ) == []..    v =
+00002270: 2064 732e 7661 7269 6162 6c65 735b 2276   ds.variables["v
+00002280: 6172 5f6c 656e 5f73 7472 225d 0a20 2020  ar_len_str"].   
+00002290: 2061 7373 6572 7420 762e 6474 7970 6520   assert v.dtype 
+000022a0: 3d3d 2073 7472 0a20 2020 2061 7373 6572  == str.    asser
+000022b0: 7420 765b 305d 203d 3d20 5f76 6c65 6e5f  t v[0] == _vlen_
+000022c0: 7374 7269 6e67 0a0a 2020 2020 7620 3d20  string..    v = 
+000022d0: 6473 2e67 726f 7570 735b 2273 7562 6772  ds.groups["subgr
+000022e0: 6f75 7022 5d2e 7661 7269 6162 6c65 735b  oup"].variables[
+000022f0: 2273 7562 7661 7222 5d0a 2020 2020 6173  "subvar"].    as
+00002300: 7365 7274 2064 732e 6772 6f75 7073 5b22  sert ds.groups["
+00002310: 7375 6267 726f 7570 225d 2e70 6172 656e  subgroup"].paren
+00002320: 7420 6973 2064 730a 2020 2020 6173 7365  t is ds.    asse
+00002330: 7274 2061 7272 6179 5f65 7175 616c 2876  rt array_equal(v
+00002340: 2c20 6e70 2e61 7261 6e67 6528 342e 3029  , np.arange(4.0)
+00002350: 290a 2020 2020 6173 7365 7274 2076 2e64  ).    assert v.d
+00002360: 7479 7065 203d 3d20 2269 6e74 3332 220a  type == "int32".
+00002370: 2020 2020 6173 7365 7274 2076 2e6e 6469      assert v.ndi
+00002380: 6d20 3d3d 2031 0a20 2020 2061 7373 6572  m == 1.    asser
+00002390: 7420 762e 6469 6d65 6e73 696f 6e73 203d  t v.dimensions =
+000023a0: 3d20 2822 7822 2c29 0a20 2020 2061 7373  = ("x",).    ass
+000023b0: 6572 7420 762e 6e63 6174 7472 7328 2920  ert v.ncattrs() 
+000023c0: 3d3d 205b 5d0a 0a20 2020 2076 203d 2064  == []..    v = d
+000023d0: 732e 6772 6f75 7073 5b22 7375 6267 726f  s.groups["subgro
+000023e0: 7570 225d 2e76 6172 6961 626c 6573 5b22  up"].variables["
+000023f0: 795f 7661 7222 5d0a 2020 2020 6173 7365  y_var"].    asse
+00002400: 7274 2076 2e73 6861 7065 203d 3d20 2831  rt v.shape == (1
+00002410: 302c 290a 2020 2020 6173 7365 7274 2022  0,).    assert "
+00002420: 7922 2069 6e20 6473 2e67 726f 7570 735b  y" in ds.groups[
+00002430: 2273 7562 6772 6f75 7022 5d2e 6469 6d65  "subgroup"].dime
+00002440: 6e73 696f 6e73 0a0a 2020 2020 6473 2e63  nsions..    ds.c
+00002450: 6c6f 7365 2829 0a0a 0a64 6566 2072 6561  lose()...def rea
+00002460: 645f 6835 6e65 7463 6466 2874 6d70 5f6e  d_h5netcdf(tmp_n
+00002470: 6574 6364 662c 2077 7269 7465 5f6d 6f64  etcdf, write_mod
+00002480: 756c 652c 2064 6563 6f64 655f 766c 656e  ule, decode_vlen
+00002490: 5f73 7472 696e 6773 293a 0a20 2020 2072  _strings):.    r
+000024a0: 656d 6f74 655f 6669 6c65 203d 2069 7369  emote_file = isi
+000024b0: 6e73 7461 6e63 6528 746d 705f 6e65 7463  nstance(tmp_netc
+000024c0: 6466 2c20 7374 7229 2061 6e64 2074 6d70  df, str) and tmp
+000024d0: 5f6e 6574 6364 662e 7374 6172 7473 7769  _netcdf.startswi
+000024e0: 7468 2872 656d 6f74 655f 6835 290a 2020  th(remote_h5).  
+000024f0: 2020 6473 203d 2068 356e 6574 6364 662e    ds = h5netcdf.
+00002500: 4669 6c65 2874 6d70 5f6e 6574 6364 662c  File(tmp_netcdf,
+00002510: 2022 7222 2c20 2a2a 6465 636f 6465 5f76   "r", **decode_v
+00002520: 6c65 6e5f 7374 7269 6e67 7329 0a20 2020  len_strings).   
+00002530: 2061 7373 6572 7420 6473 2e6e 616d 6520   assert ds.name 
+00002540: 3d3d 2022 2f22 0a20 2020 2061 7373 6572  == "/".    asser
+00002550: 7420 6c69 7374 2864 732e 6174 7472 7329  t list(ds.attrs)
+00002560: 203d 3d20 5b22 676c 6f62 616c 222c 2022   == ["global", "
+00002570: 6f74 6865 725f 6174 7472 225d 0a20 2020  other_attr"].   
+00002580: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
+00002590: 5b22 676c 6f62 616c 225d 203d 3d20 3432  ["global"] == 42
+000025a0: 0a20 2020 2069 6620 7772 6974 655f 6d6f  .    if write_mo
+000025b0: 6475 6c65 2069 7320 6e6f 7420 6e65 7443  dule is not netC
+000025c0: 4446 343a 0a20 2020 2020 2020 2023 2073  DF4:.        # s
+000025d0: 6b69 7020 666f 7220 6e6f 773a 2068 7474  kip for now: htt
+000025e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000025f0: 556e 6964 6174 612f 6e65 7463 6466 342d  Unidata/netcdf4-
+00002600: 7079 7468 6f6e 2f69 7373 7565 732f 3338  python/issues/38
+00002610: 380a 2020 2020 2020 2020 6173 7365 7274  8.        assert
+00002620: 2064 732e 6174 7472 735b 226f 7468 6572   ds.attrs["other
+00002630: 5f61 7474 7222 5d20 3d3d 2022 7965 7322  _attr"] == "yes"
+00002640: 0a20 2020 2061 7373 6572 7420 7365 7428  .    assert set(
+00002650: 6473 2e64 696d 656e 7369 6f6e 7329 203d  ds.dimensions) =
+00002660: 3d20 7365 7428 0a20 2020 2020 2020 205b  = set(.        [
+00002670: 2278 222c 2022 7922 2c20 227a 222c 2022  "x", "y", "z", "
+00002680: 656d 7074 7922 2c20 2273 7472 696e 6733  empty", "string3
+00002690: 222c 2022 6d69 736d 6174 6368 6564 5f64  ", "mismatched_d
+000026a0: 696d 222c 2022 756e 6c69 6d69 7465 6422  im", "unlimited"
+000026b0: 5d0a 2020 2020 290a 2020 2020 7661 7269  ].    ).    vari
+000026c0: 6162 6c65 7320 3d20 7365 7428 0a20 2020  ables = set(.   
+000026d0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+000026e0: 2020 2022 666f 6f22 2c0a 2020 2020 2020     "foo",.      
+000026f0: 2020 2020 2020 227a 222c 0a20 2020 2020        "z",.     
+00002700: 2020 2020 2020 2022 696e 7473 6361 6c61         "intscala
+00002710: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00002720: 2273 6361 6c61 7222 2c0a 2020 2020 2020  "scalar",.      
+00002730: 2020 2020 2020 2276 6172 5f6c 656e 5f73        "var_len_s
+00002740: 7472 222c 0a20 2020 2020 2020 2020 2020  tr",.           
+00002750: 2022 6d69 736d 6174 6368 6564 5f64 696d   "mismatched_dim
+00002760: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00002770: 666f 6f5f 756e 6c69 6d69 7465 6422 2c0a  foo_unlimited",.
+00002780: 2020 2020 2020 2020 5d0a 2020 2020 290a          ].    ).
+00002790: 2020 2020 2320 6669 7820 6375 7272 656e      # fix curren
+000027a0: 7420 6661 696c 7572 6520 6f66 2068 7364  t failure of hsd
+000027b0: 732f 6835 7079 640a 2020 2020 6966 206e  s/h5pyd.    if n
+000027c0: 6f74 2072 656d 6f74 655f 6669 6c65 3a0a  ot remote_file:.
+000027d0: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+000027e0: 7320 7c3d 2073 6574 285b 2279 225d 290a  s |= set(["y"]).
+000027f0: 2020 2020 6173 7365 7274 2073 6574 2864      assert set(d
+00002800: 732e 7661 7269 6162 6c65 7329 203d 3d20  s.variables) == 
+00002810: 7661 7269 6162 6c65 730a 0a20 2020 2061  variables..    a
+00002820: 7373 6572 7420 7365 7428 6473 2e67 726f  ssert set(ds.gro
+00002830: 7570 7329 203d 3d20 7365 7428 5b22 7375  ups) == set(["su
+00002840: 6267 726f 7570 225d 290a 2020 2020 6173  bgroup"]).    as
+00002850: 7365 7274 2064 732e 7061 7265 6e74 2069  sert ds.parent i
+00002860: 7320 4e6f 6e65 0a0a 2020 2020 7620 3d20  s None..    v = 
+00002870: 6473 5b22 666f 6f22 5d0a 2020 2020 6173  ds["foo"].    as
+00002880: 7365 7274 2076 2e6e 616d 6520 3d3d 2022  sert v.name == "
+00002890: 2f66 6f6f 220a 2020 2020 6173 7365 7274  /foo".    assert
+000028a0: 2061 7272 6179 5f65 7175 616c 2876 2c20   array_equal(v, 
+000028b0: 6e70 2e6f 6e65 7328 2834 2c20 3529 2929  np.ones((4, 5)))
+000028c0: 0a20 2020 2061 7373 6572 7420 762e 6474  .    assert v.dt
+000028d0: 7970 6520 3d3d 2066 6c6f 6174 0a20 2020  ype == float.   
+000028e0: 2061 7373 6572 7420 762e 6469 6d65 6e73   assert v.dimens
+000028f0: 696f 6e73 203d 3d20 2822 7822 2c20 2279  ions == ("x", "y
+00002900: 2229 0a20 2020 2061 7373 6572 7420 762e  ").    assert v.
+00002910: 6e64 696d 203d 3d20 320a 2020 2020 6173  ndim == 2.    as
+00002920: 7365 7274 206c 6973 7428 762e 6174 7472  sert list(v.attr
+00002930: 7329 203d 3d20 5b22 756e 6974 7322 5d0a  s) == ["units"].
+00002940: 2020 2020 6966 2077 7269 7465 5f6d 6f64      if write_mod
+00002950: 756c 6520 6973 206e 6f74 206e 6574 4344  ule is not netCD
+00002960: 4634 3a0a 2020 2020 2020 2020 6173 7365  F4:.        asse
+00002970: 7274 2076 2e61 7474 7273 5b22 756e 6974  rt v.attrs["unit
+00002980: 7322 5d20 3d3d 2022 6d65 7465 7273 220a  s"] == "meters".
+00002990: 2020 2020 6173 7365 7274 2076 2e63 6875      assert v.chu
+000029a0: 6e6b 7320 3d3d 2028 342c 2035 290a 2020  nks == (4, 5).  
+000029b0: 2020 6173 7365 7274 2076 2e63 6f6d 7072    assert v.compr
+000029c0: 6573 7369 6f6e 203d 3d20 2267 7a69 7022  ession == "gzip"
+000029d0: 0a20 2020 2061 7373 6572 7420 762e 636f  .    assert v.co
+000029e0: 6d70 7265 7373 696f 6e5f 6f70 7473 203d  mpression_opts =
+000029f0: 3d20 340a 2020 2020 6173 7365 7274 206e  = 4.    assert n
+00002a00: 6f74 2076 2e66 6c65 7463 6865 7233 320a  ot v.fletcher32.
+00002a10: 2020 2020 6173 7365 7274 2076 2e73 6875      assert v.shu
+00002a20: 6666 6c65 0a0a 2020 2020 2320 6669 7820  ffle..    # fix 
+00002a30: 6375 7272 656e 7420 6661 696c 7572 6520  current failure 
+00002a40: 6f66 2068 7364 732f 6835 7079 640a 2020  of hsds/h5pyd.  
+00002a50: 2020 6966 206e 6f74 2072 656d 6f74 655f    if not remote_
+00002a60: 6669 6c65 3a0a 2020 2020 2020 2020 7620  file:.        v 
+00002a70: 3d20 6473 5b22 7922 5d0a 2020 2020 2020  = ds["y"].      
+00002a80: 2020 6173 7365 7274 2061 7272 6179 5f65    assert array_e
+00002a90: 7175 616c 2876 2c20 6e70 2e72 5f5b 6e70  qual(v, np.r_[np
+00002aa0: 2e61 7261 6e67 6528 3429 2c20 5b2d 315d  .arange(4), [-1]
+00002ab0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
+00002ac0: 7420 762e 6474 7970 6520 3d3d 2069 6e74  t v.dtype == int
+00002ad0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002ae0: 762e 6469 6d65 6e73 696f 6e73 203d 3d20  v.dimensions == 
+00002af0: 2822 7922 2c29 0a20 2020 2020 2020 2061  ("y",).        a
+00002b00: 7373 6572 7420 762e 6e64 696d 203d 3d20  ssert v.ndim == 
+00002b10: 310a 2020 2020 2020 2020 6173 7365 7274  1.        assert
+00002b20: 206c 6973 7428 762e 6174 7472 7329 203d   list(v.attrs) =
+00002b30: 3d20 5b22 5f46 696c 6c56 616c 7565 225d  = ["_FillValue"]
+00002b40: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002b50: 762e 6174 7472 735b 225f 4669 6c6c 5661  v.attrs["_FillVa
+00002b60: 6c75 6522 5d20 3d3d 202d 310a 2020 2020  lue"] == -1.    
+00002b70: 2020 2020 6966 206e 6f74 2072 656d 6f74      if not remot
+00002b80: 655f 6669 6c65 3a0a 2020 2020 2020 2020  e_file:.        
+00002b90: 2020 2020 6173 7365 7274 2076 2e63 6875      assert v.chu
+00002ba0: 6e6b 7320 6973 204e 6f6e 650a 2020 2020  nks is None.    
+00002bb0: 2020 2020 6173 7365 7274 2076 2e63 6f6d      assert v.com
+00002bc0: 7072 6573 7369 6f6e 2069 7320 4e6f 6e65  pression is None
+00002bd0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002be0: 762e 636f 6d70 7265 7373 696f 6e5f 6f70  v.compression_op
+00002bf0: 7473 2069 7320 4e6f 6e65 0a20 2020 2020  ts is None.     
+00002c00: 2020 2061 7373 6572 7420 6e6f 7420 762e     assert not v.
+00002c10: 666c 6574 6368 6572 3332 0a20 2020 2020  fletcher32.     
+00002c20: 2020 2061 7373 6572 7420 6e6f 7420 762e     assert not v.
+00002c30: 7368 7566 666c 650a 2020 2020 6473 2e63  shuffle.    ds.c
+00002c40: 6c6f 7365 2829 0a0a 2020 2020 6966 2069  lose()..    if i
+00002c50: 735f 6835 7079 5f63 6861 725f 776f 726b  s_h5py_char_work
+00002c60: 696e 6728 746d 705f 6e65 7463 6466 2c20  ing(tmp_netcdf, 
+00002c70: 227a 2229 3a0a 2020 2020 2020 2020 6473  "z"):.        ds
+00002c80: 203d 2068 356e 6574 6364 662e 4669 6c65   = h5netcdf.File
+00002c90: 2874 6d70 5f6e 6574 6364 662c 2022 7222  (tmp_netcdf, "r"
+00002ca0: 290a 2020 2020 2020 2020 7620 3d20 6473  ).        v = ds
+00002cb0: 5b22 7a22 5d0a 2020 2020 2020 2020 6173  ["z"].        as
+00002cc0: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
+00002cd0: 2876 2c20 5f63 6861 725f 6172 7261 7929  (v, _char_array)
+00002ce0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002cf0: 762e 6474 7970 6520 3d3d 2022 5331 220a  v.dtype == "S1".
+00002d00: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
+00002d10: 2e6e 6469 6d20 3d3d 2032 0a20 2020 2020  .ndim == 2.     
+00002d20: 2020 2061 7373 6572 7420 762e 6469 6d65     assert v.dime
+00002d30: 6e73 696f 6e73 203d 3d20 2822 7a22 2c20  nsions == ("z", 
+00002d40: 2273 7472 696e 6733 2229 0a20 2020 2020  "string3").     
+00002d50: 2020 2061 7373 6572 7420 6c69 7374 2876     assert list(v
+00002d60: 2e61 7474 7273 2920 3d3d 205b 225f 4669  .attrs) == ["_Fi
+00002d70: 6c6c 5661 6c75 6522 5d0a 2020 2020 2020  llValue"].      
+00002d80: 2020 6173 7365 7274 2076 2e61 7474 7273    assert v.attrs
+00002d90: 5b22 5f46 696c 6c56 616c 7565 225d 203d  ["_FillValue"] =
+00002da0: 3d20 6222 5822 0a20 2020 2065 6c73 653a  = b"X".    else:
+00002db0: 0a20 2020 2020 2020 2064 7320 3d20 6835  .        ds = h5
+00002dc0: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+00002dd0: 6e65 7463 6466 2c20 2272 222c 202a 2a64  netcdf, "r", **d
+00002de0: 6563 6f64 655f 766c 656e 5f73 7472 696e  ecode_vlen_strin
+00002df0: 6773 290a 0a20 2020 2076 203d 2064 735b  gs)..    v = ds[
+00002e00: 2273 6361 6c61 7222 5d0a 2020 2020 6173  "scalar"].    as
+00002e10: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
+00002e20: 2876 2c20 6e70 2e61 7272 6179 2832 2e30  (v, np.array(2.0
+00002e30: 2929 0a20 2020 2061 7373 6572 7420 762e  )).    assert v.
+00002e40: 6474 7970 6520 3d3d 2022 666c 6f61 7433  dtype == "float3
+00002e50: 3222 0a20 2020 2061 7373 6572 7420 762e  2".    assert v.
+00002e60: 6e64 696d 203d 3d20 300a 2020 2020 6173  ndim == 0.    as
+00002e70: 7365 7274 2076 2e64 696d 656e 7369 6f6e  sert v.dimension
+00002e80: 7320 3d3d 2028 290a 2020 2020 6173 7365  s == ().    asse
+00002e90: 7274 206c 6973 7428 762e 6174 7472 7329  rt list(v.attrs)
+00002ea0: 203d 3d20 5b5d 0a0a 2020 2020 7620 3d20   == []..    v = 
+00002eb0: 6473 2e76 6172 6961 626c 6573 5b22 696e  ds.variables["in
+00002ec0: 7473 6361 6c61 7222 5d0a 2020 2020 6173  tscalar"].    as
+00002ed0: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
+00002ee0: 2876 2c20 6e70 2e61 7272 6179 2832 2929  (v, np.array(2))
+00002ef0: 0a20 2020 2061 7373 6572 7420 762e 6474  .    assert v.dt
+00002f00: 7970 6520 3d3d 2022 696e 7436 3422 0a20  ype == "int64". 
+00002f10: 2020 2061 7373 6572 7420 762e 6e64 696d     assert v.ndim
+00002f20: 203d 3d20 300a 2020 2020 6173 7365 7274   == 0.    assert
+00002f30: 2076 2e64 696d 656e 7369 6f6e 7320 3d3d   v.dimensions ==
+00002f40: 2028 290a 2020 2020 6173 7365 7274 206c   ().    assert l
+00002f50: 6973 7428 762e 6174 7472 7329 203d 3d20  ist(v.attrs) == 
+00002f60: 5b5d 0a0a 2020 2020 7620 3d20 6473 5b22  []..    v = ds["
+00002f70: 7661 725f 6c65 6e5f 7374 7222 5d0a 2020  var_len_str"].  
+00002f80: 2020 6173 7365 7274 2068 3570 792e 6368    assert h5py.ch
+00002f90: 6563 6b5f 6474 7970 6528 766c 656e 3d76  eck_dtype(vlen=v
+00002fa0: 2e64 7479 7065 2920 3d3d 2073 7472 0a20  .dtype) == str. 
+00002fb0: 2020 2069 6620 6765 7461 7474 7228 6473     if getattr(ds
+00002fc0: 2c20 2264 6563 6f64 655f 766c 656e 5f73  , "decode_vlen_s
+00002fd0: 7472 696e 6773 222c 2054 7275 6529 3a0a  trings", True):.
+00002fe0: 2020 2020 2020 2020 6173 7365 7274 2076          assert v
+00002ff0: 5b30 5d20 3d3d 205f 766c 656e 5f73 7472  [0] == _vlen_str
+00003000: 696e 670a 2020 2020 656c 7365 3a0a 2020  ing.    else:.  
+00003010: 2020 2020 2020 6173 7365 7274 2076 5b30        assert v[0
+00003020: 5d20 3d3d 205f 766c 656e 5f73 7472 696e  ] == _vlen_strin
+00003030: 672e 656e 636f 6465 2822 7574 665f 3822  g.encode("utf_8"
+00003040: 290a 0a20 2020 2076 203d 2064 735b 222f  )..    v = ds["/
+00003050: 7375 6267 726f 7570 2f73 7562 7661 7222  subgroup/subvar"
+00003060: 5d0a 2020 2020 6173 7365 7274 2076 2069  ].    assert v i
+00003070: 7320 6473 5b22 7375 6267 726f 7570 225d  s ds["subgroup"]
+00003080: 5b22 7375 6276 6172 225d 0a20 2020 2061  ["subvar"].    a
+00003090: 7373 6572 7420 7620 6973 2064 735b 2273  ssert v is ds["s
+000030a0: 7562 6772 6f75 702f 7375 6276 6172 225d  ubgroup/subvar"]
+000030b0: 0a20 2020 2061 7373 6572 7420 7620 6973  .    assert v is
+000030c0: 2064 735b 2273 7562 6772 6f75 7022 5d5b   ds["subgroup"][
+000030d0: 222f 7375 6267 726f 7570 2f73 7562 7661  "/subgroup/subva
+000030e0: 7222 5d0a 2020 2020 6173 7365 7274 2076  r"].    assert v
+000030f0: 2e6e 616d 6520 3d3d 2022 2f73 7562 6772  .name == "/subgr
+00003100: 6f75 702f 7375 6276 6172 220a 2020 2020  oup/subvar".    
+00003110: 6173 7365 7274 2064 735b 2273 7562 6772  assert ds["subgr
+00003120: 6f75 7022 5d2e 6e61 6d65 203d 3d20 222f  oup"].name == "/
+00003130: 7375 6267 726f 7570 220a 2020 2020 6173  subgroup".    as
+00003140: 7365 7274 2064 735b 2273 7562 6772 6f75  sert ds["subgrou
+00003150: 7022 5d2e 7061 7265 6e74 2069 7320 6473  p"].parent is ds
+00003160: 0a20 2020 2061 7373 6572 7420 6172 7261  .    assert arra
+00003170: 795f 6571 7561 6c28 762c 206e 702e 6172  y_equal(v, np.ar
+00003180: 616e 6765 2834 2e30 2929 0a20 2020 2061  ange(4.0)).    a
+00003190: 7373 6572 7420 762e 6474 7970 6520 3d3d  ssert v.dtype ==
+000031a0: 2022 696e 7433 3222 0a20 2020 2061 7373   "int32".    ass
+000031b0: 6572 7420 762e 6e64 696d 203d 3d20 310a  ert v.ndim == 1.
+000031c0: 2020 2020 6173 7365 7274 2076 2e64 696d      assert v.dim
+000031d0: 656e 7369 6f6e 7320 3d3d 2028 2278 222c  ensions == ("x",
+000031e0: 290a 2020 2020 6173 7365 7274 206c 6973  ).    assert lis
+000031f0: 7428 762e 6174 7472 7329 203d 3d20 5b5d  t(v.attrs) == []
+00003200: 0a0a 2020 2020 6173 7365 7274 2064 735b  ..    assert ds[
+00003210: 222f 7375 6267 726f 7570 2f79 5f76 6172  "/subgroup/y_var
+00003220: 225d 2e73 6861 7065 203d 3d20 2831 302c  "].shape == (10,
+00003230: 290a 2020 2020 6173 7365 7274 2064 735b  ).    assert ds[
+00003240: 222f 7375 6267 726f 7570 225d 2e64 696d  "/subgroup"].dim
+00003250: 656e 7369 6f6e 735b 2279 225d 2e73 697a  ensions["y"].siz
+00003260: 6520 3d3d 2031 300a 0a20 2020 2064 732e  e == 10..    ds.
+00003270: 636c 6f73 6528 290a 0a0a 6465 6620 726f  close()...def ro
+00003280: 756e 6474 7269 705f 6c65 6761 6379 5f6e  undtrip_legacy_n
+00003290: 6574 6364 6628 746d 705f 6e65 7463 6466  etcdf(tmp_netcdf
+000032a0: 2c20 7265 6164 5f6d 6f64 756c 652c 2077  , read_module, w
+000032b0: 7269 7465 5f6d 6f64 756c 6529 3a0a 2020  rite_module):.  
+000032c0: 2020 7772 6974 655f 6c65 6761 6379 5f6e    write_legacy_n
+000032d0: 6574 6364 6628 746d 705f 6e65 7463 6466  etcdf(tmp_netcdf
+000032e0: 2c20 7772 6974 655f 6d6f 6475 6c65 290a  , write_module).
+000032f0: 2020 2020 7265 6164 5f6c 6567 6163 795f      read_legacy_
+00003300: 6e65 7463 6466 2874 6d70 5f6e 6574 6364  netcdf(tmp_netcd
+00003310: 662c 2072 6561 645f 6d6f 6475 6c65 2c20  f, read_module, 
+00003320: 7772 6974 655f 6d6f 6475 6c65 290a 0a0a  write_module)...
+00003330: 6465 6620 7465 7374 5f77 7269 7465 5f6c  def test_write_l
+00003340: 6567 6163 7961 7069 5f72 6561 645f 6e65  egacyapi_read_ne
+00003350: 7443 4446 3428 746d 705f 6c6f 6361 6c5f  tCDF4(tmp_local_
+00003360: 6e65 7463 6466 293a 0a20 2020 2072 6f75  netcdf):.    rou
+00003370: 6e64 7472 6970 5f6c 6567 6163 795f 6e65  ndtrip_legacy_ne
+00003380: 7463 6466 2874 6d70 5f6c 6f63 616c 5f6e  tcdf(tmp_local_n
+00003390: 6574 6364 662c 206e 6574 4344 4634 2c20  etcdf, netCDF4, 
+000033a0: 6c65 6761 6379 6170 6929 0a0a 0a64 6566  legacyapi)...def
+000033b0: 2074 6573 745f 726f 756e 6474 7269 705f   test_roundtrip_
+000033c0: 6835 6e65 7463 6466 5f6c 6567 6163 7961  h5netcdf_legacya
+000033d0: 7069 2874 6d70 5f6c 6f63 616c 5f6e 6574  pi(tmp_local_net
+000033e0: 6364 6629 3a0a 2020 2020 726f 756e 6474  cdf):.    roundt
+000033f0: 7269 705f 6c65 6761 6379 5f6e 6574 6364  rip_legacy_netcd
+00003400: 6628 746d 705f 6c6f 6361 6c5f 6e65 7463  f(tmp_local_netc
+00003410: 6466 2c20 6c65 6761 6379 6170 692c 206c  df, legacyapi, l
+00003420: 6567 6163 7961 7069 290a 0a0a 6465 6620  egacyapi)...def 
+00003430: 7465 7374 5f77 7269 7465 5f6e 6574 4344  test_write_netCD
+00003440: 4634 5f72 6561 645f 6c65 6761 6379 6170  F4_read_legacyap
+00003450: 6928 746d 705f 6c6f 6361 6c5f 6e65 7463  i(tmp_local_netc
+00003460: 6466 293a 0a20 2020 2072 6f75 6e64 7472  df):.    roundtr
+00003470: 6970 5f6c 6567 6163 795f 6e65 7463 6466  ip_legacy_netcdf
+00003480: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+00003490: 662c 206c 6567 6163 7961 7069 2c20 6e65  f, legacyapi, ne
+000034a0: 7443 4446 3429 0a0a 0a64 6566 2074 6573  tCDF4)...def tes
+000034b0: 745f 7772 6974 655f 6835 6e65 7463 6466  t_write_h5netcdf
+000034c0: 5f72 6561 645f 6c65 6761 6379 6170 6928  _read_legacyapi(
+000034d0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+000034e0: 293a 0a20 2020 2077 7269 7465 5f68 356e  ):.    write_h5n
+000034f0: 6574 6364 6628 746d 705f 6c6f 6361 6c5f  etcdf(tmp_local_
+00003500: 6e65 7463 6466 290a 2020 2020 7265 6164  netcdf).    read
+00003510: 5f6c 6567 6163 795f 6e65 7463 6466 2874  _legacy_netcdf(t
+00003520: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+00003530: 206c 6567 6163 7961 7069 2c20 6835 6e65   legacyapi, h5ne
+00003540: 7463 6466 290a 0a0a 6465 6620 7465 7374  tcdf)...def test
+00003550: 5f77 7269 7465 5f68 356e 6574 6364 665f  _write_h5netcdf_
+00003560: 7265 6164 5f6e 6574 4344 4634 2874 6d70  read_netCDF4(tmp
+00003570: 5f6c 6f63 616c 5f6e 6574 6364 6629 3a0a  _local_netcdf):.
+00003580: 2020 2020 7772 6974 655f 6835 6e65 7463      write_h5netc
+00003590: 6466 2874 6d70 5f6c 6f63 616c 5f6e 6574  df(tmp_local_net
+000035a0: 6364 6629 0a20 2020 2072 6561 645f 6c65  cdf).    read_le
+000035b0: 6761 6379 5f6e 6574 6364 6628 746d 705f  gacy_netcdf(tmp_
+000035c0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 6e65  local_netcdf, ne
+000035d0: 7443 4446 342c 2068 356e 6574 6364 6629  tCDF4, h5netcdf)
+000035e0: 0a0a 0a64 6566 2074 6573 745f 726f 756e  ...def test_roun
+000035f0: 6474 7269 705f 6835 6e65 7463 6466 2874  dtrip_h5netcdf(t
+00003600: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
+00003610: 7465 5f6e 6574 6364 662c 2064 6563 6f64  te_netcdf, decod
+00003620: 655f 766c 656e 5f73 7472 696e 6773 293a  e_vlen_strings):
+00003630: 0a20 2020 2077 7269 7465 5f68 356e 6574  .    write_h5net
+00003640: 6364 6628 746d 705f 6c6f 6361 6c5f 6f72  cdf(tmp_local_or
+00003650: 5f72 656d 6f74 655f 6e65 7463 6466 290a  _remote_netcdf).
+00003660: 2020 2020 7265 6164 5f68 356e 6574 6364      read_h5netcd
+00003670: 6628 746d 705f 6c6f 6361 6c5f 6f72 5f72  f(tmp_local_or_r
+00003680: 656d 6f74 655f 6e65 7463 6466 2c20 6835  emote_netcdf, h5
+00003690: 6e65 7463 6466 2c20 6465 636f 6465 5f76  netcdf, decode_v
+000036a0: 6c65 6e5f 7374 7269 6e67 7329 0a0a 0a64  len_strings)...d
+000036b0: 6566 2074 6573 745f 7772 6974 655f 6e65  ef test_write_ne
+000036c0: 7443 4446 345f 7265 6164 5f68 356e 6574  tCDF4_read_h5net
+000036d0: 6364 6628 746d 705f 6c6f 6361 6c5f 6e65  cdf(tmp_local_ne
+000036e0: 7463 6466 2c20 6465 636f 6465 5f76 6c65  tcdf, decode_vle
+000036f0: 6e5f 7374 7269 6e67 7329 3a0a 2020 2020  n_strings):.    
+00003700: 7772 6974 655f 6c65 6761 6379 5f6e 6574  write_legacy_net
+00003710: 6364 6628 746d 705f 6c6f 6361 6c5f 6e65  cdf(tmp_local_ne
+00003720: 7463 6466 2c20 6e65 7443 4446 3429 0a20  tcdf, netCDF4). 
+00003730: 2020 2072 6561 645f 6835 6e65 7463 6466     read_h5netcdf
+00003740: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+00003750: 662c 206e 6574 4344 4634 2c20 6465 636f  f, netCDF4, deco
+00003760: 6465 5f76 6c65 6e5f 7374 7269 6e67 7329  de_vlen_strings)
+00003770: 0a0a 0a64 6566 2074 6573 745f 7772 6974  ...def test_writ
+00003780: 655f 6c65 6761 6379 6170 695f 7265 6164  e_legacyapi_read
+00003790: 5f68 356e 6574 6364 6628 746d 705f 6c6f  _h5netcdf(tmp_lo
+000037a0: 6361 6c5f 6e65 7463 6466 2c20 6465 636f  cal_netcdf, deco
+000037b0: 6465 5f76 6c65 6e5f 7374 7269 6e67 7329  de_vlen_strings)
+000037c0: 3a0a 2020 2020 7772 6974 655f 6c65 6761  :.    write_lega
+000037d0: 6379 5f6e 6574 6364 6628 746d 705f 6c6f  cy_netcdf(tmp_lo
+000037e0: 6361 6c5f 6e65 7463 6466 2c20 6c65 6761  cal_netcdf, lega
+000037f0: 6379 6170 6929 0a20 2020 2072 6561 645f  cyapi).    read_
+00003800: 6835 6e65 7463 6466 2874 6d70 5f6c 6f63  h5netcdf(tmp_loc
+00003810: 616c 5f6e 6574 6364 662c 206c 6567 6163  al_netcdf, legac
+00003820: 7961 7069 2c20 6465 636f 6465 5f76 6c65  yapi, decode_vle
+00003830: 6e5f 7374 7269 6e67 7329 0a0a 0a64 6566  n_strings)...def
+00003840: 2074 6573 745f 6669 6c65 6f62 6a28 6465   test_fileobj(de
+00003850: 636f 6465 5f76 6c65 6e5f 7374 7269 6e67  code_vlen_string
+00003860: 7329 3a0a 2020 2020 6669 6c65 6f62 6a20  s):.    fileobj 
+00003870: 3d20 7465 6d70 6669 6c65 2e54 656d 706f  = tempfile.Tempo
+00003880: 7261 7279 4669 6c65 2829 0a20 2020 2077  raryFile().    w
+00003890: 7269 7465 5f68 356e 6574 6364 6628 6669  rite_h5netcdf(fi
+000038a0: 6c65 6f62 6a29 0a20 2020 2072 6561 645f  leobj).    read_
+000038b0: 6835 6e65 7463 6466 2866 696c 656f 626a  h5netcdf(fileobj
+000038c0: 2c20 6835 6e65 7463 6466 2c20 6465 636f  , h5netcdf, deco
+000038d0: 6465 5f76 6c65 6e5f 7374 7269 6e67 7329  de_vlen_strings)
+000038e0: 0a20 2020 2066 696c 656f 626a 203d 2069  .    fileobj = i
+000038f0: 6f2e 4279 7465 7349 4f28 290a 2020 2020  o.BytesIO().    
+00003900: 7772 6974 655f 6835 6e65 7463 6466 2866  write_h5netcdf(f
+00003910: 696c 656f 626a 290a 2020 2020 7265 6164  ileobj).    read
+00003920: 5f68 356e 6574 6364 6628 6669 6c65 6f62  _h5netcdf(fileob
+00003930: 6a2c 2068 356e 6574 6364 662c 2064 6563  j, h5netcdf, dec
+00003940: 6f64 655f 766c 656e 5f73 7472 696e 6773  ode_vlen_strings
+00003950: 290a 0a0a 6465 6620 7465 7374 5f72 6570  )...def test_rep
+00003960: 7228 746d 705f 6c6f 6361 6c5f 6f72 5f72  r(tmp_local_or_r
+00003970: 656d 6f74 655f 6e65 7463 6466 293a 0a20  emote_netcdf):. 
+00003980: 2020 2077 7269 7465 5f68 356e 6574 6364     write_h5netcd
+00003990: 6628 746d 705f 6c6f 6361 6c5f 6f72 5f72  f(tmp_local_or_r
+000039a0: 656d 6f74 655f 6e65 7463 6466 290a 2020  emote_netcdf).  
+000039b0: 2020 6620 3d20 6835 6e65 7463 6466 2e46    f = h5netcdf.F
+000039c0: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
+000039d0: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
+000039e0: 2261 2229 0a20 2020 2061 7373 6572 7420  "a").    assert 
+000039f0: 2268 356e 6574 6364 662e 4669 6c65 2220  "h5netcdf.File" 
+00003a00: 696e 2072 6570 7228 6629 0a20 2020 2061  in repr(f).    a
+00003a10: 7373 6572 7420 2273 7562 6772 6f75 7022  ssert "subgroup"
+00003a20: 2069 6e20 7265 7072 2866 290a 2020 2020   in repr(f).    
+00003a30: 6173 7365 7274 2022 666f 6f22 2069 6e20  assert "foo" in 
+00003a40: 7265 7072 2866 290a 2020 2020 6173 7365  repr(f).    asse
+00003a50: 7274 2022 6f74 6865 725f 6174 7472 2220  rt "other_attr" 
+00003a60: 696e 2072 6570 7228 6629 0a0a 2020 2020  in repr(f)..    
+00003a70: 6173 7365 7274 2022 6835 6e65 7463 6466  assert "h5netcdf
+00003a80: 2e61 7474 7273 2e41 7474 7269 6275 7465  .attrs.Attribute
+00003a90: 7322 2069 6e20 7265 7072 2866 2e61 7474  s" in repr(f.att
+00003aa0: 7273 290a 2020 2020 6173 7365 7274 2022  rs).    assert "
+00003ab0: 676c 6f62 616c 2220 696e 2072 6570 7228  global" in repr(
+00003ac0: 662e 6174 7472 7329 0a0a 2020 2020 6420  f.attrs)..    d 
+00003ad0: 3d20 662e 6469 6d65 6e73 696f 6e73 0a20  = f.dimensions. 
+00003ae0: 2020 2061 7373 6572 7420 2268 356e 6574     assert "h5net
+00003af0: 6364 662e 4469 6d65 6e73 696f 6e73 2220  cdf.Dimensions" 
+00003b00: 696e 2072 6570 7228 6429 0a20 2020 2061  in repr(d).    a
+00003b10: 7373 6572 7420 2278 3d3c 6835 6e65 7463  ssert "x=<h5netc
+00003b20: 6466 2e44 696d 656e 7369 6f6e 2027 7827  df.Dimension 'x'
+00003b30: 3a20 7369 7a65 2034 3e22 2069 6e20 7265  : size 4>" in re
+00003b40: 7072 2864 290a 0a20 2020 2067 203d 2066  pr(d)..    g = f
+00003b50: 5b22 7375 6267 726f 7570 225d 0a20 2020  ["subgroup"].   
+00003b60: 2061 7373 6572 7420 2268 356e 6574 6364   assert "h5netcd
+00003b70: 662e 4772 6f75 7022 2069 6e20 7265 7072  f.Group" in repr
+00003b80: 2867 290a 2020 2020 6173 7365 7274 2022  (g).    assert "
+00003b90: 7375 6276 6172 2220 696e 2072 6570 7228  subvar" in repr(
+00003ba0: 6729 0a0a 2020 2020 7620 3d20 665b 2266  g)..    v = f["f
+00003bb0: 6f6f 225d 0a20 2020 2061 7373 6572 7420  oo"].    assert 
+00003bc0: 2268 356e 6574 6364 662e 5661 7269 6162  "h5netcdf.Variab
+00003bd0: 6c65 2220 696e 2072 6570 7228 7629 0a20  le" in repr(v). 
+00003be0: 2020 2061 7373 6572 7420 2266 6c6f 6174     assert "float
+00003bf0: 2220 696e 2072 6570 7228 7629 0a20 2020  " in repr(v).   
+00003c00: 2061 7373 6572 7420 2275 6e69 7473 2220   assert "units" 
+00003c10: 696e 2072 6570 7228 7629 0a0a 2020 2020  in repr(v)..    
+00003c20: 662e 6469 6d65 6e73 696f 6e73 5b22 7465  f.dimensions["te
+00003c30: 6d70 225d 203d 204e 6f6e 650a 2020 2020  mp"] = None.    
+00003c40: 6173 7365 7274 2022 7465 6d70 3a20 3c68  assert "temp: <h
+00003c50: 356e 6574 6364 662e 4469 6d65 6e73 696f  5netcdf.Dimensio
+00003c60: 6e20 2774 656d 7027 3a20 7369 7a65 2030  n 'temp': size 0
+00003c70: 2028 756e 6c69 6d69 7465 6429 3e22 2069   (unlimited)>" i
+00003c80: 6e20 7265 7072 2866 290a 2020 2020 662e  n repr(f).    f.
+00003c90: 7265 7369 7a65 5f64 696d 656e 7369 6f6e  resize_dimension
+00003ca0: 2822 7465 6d70 222c 2035 290a 2020 2020  ("temp", 5).    
+00003cb0: 6173 7365 7274 2022 7465 6d70 3a20 3c68  assert "temp: <h
+00003cc0: 356e 6574 6364 662e 4469 6d65 6e73 696f  5netcdf.Dimensio
+00003cd0: 6e20 2774 656d 7027 3a20 7369 7a65 2035  n 'temp': size 5
+00003ce0: 2028 756e 6c69 6d69 7465 6429 3e22 2069   (unlimited)>" i
+00003cf0: 6e20 7265 7072 2866 290a 0a20 2020 2066  n repr(f)..    f
+00003d00: 2e63 6c6f 7365 2829 0a0a 2020 2020 6173  .close()..    as
+00003d10: 7365 7274 2022 436c 6f73 6564 2220 696e  sert "Closed" in
+00003d20: 2072 6570 7228 6629 0a20 2020 2061 7373   repr(f).    ass
+00003d30: 6572 7420 2243 6c6f 7365 6422 2069 6e20  ert "Closed" in 
+00003d40: 7265 7072 2864 290a 2020 2020 6173 7365  repr(d).    asse
+00003d50: 7274 2022 436c 6f73 6564 2220 696e 2072  rt "Closed" in r
+00003d60: 6570 7228 6729 0a20 2020 2061 7373 6572  epr(g).    asser
+00003d70: 7420 2243 6c6f 7365 6422 2069 6e20 7265  t "Closed" in re
+00003d80: 7072 2876 290a 0a0a 6465 6620 7465 7374  pr(v)...def test
+00003d90: 5f61 7474 7273 5f61 7069 2874 6d70 5f6c  _attrs_api(tmp_l
+00003da0: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+00003db0: 6574 6364 6629 3a0a 2020 2020 6835 203d  etcdf):.    h5 =
+00003dc0: 2067 6574 5f68 6466 355f 6d6f 6475 6c65   get_hdf5_module
+00003dd0: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+00003de0: 6d6f 7465 5f6e 6574 6364 6629 0a20 2020  mote_netcdf).   
+00003df0: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+00003e00: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
+00003e10: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
+00003e20: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
+00003e30: 2020 2020 6473 2e61 7474 7273 5b22 636f      ds.attrs["co
+00003e40: 6e76 656e 7469 6f6e 7322 5d20 3d20 2243  nventions"] = "C
+00003e50: 4622 0a20 2020 2020 2020 2064 732e 6174  F".        ds.at
+00003e60: 7472 735b 2265 6d70 7479 5f73 7472 696e  trs["empty_strin
+00003e70: 6722 5d20 3d20 6835 2e45 6d70 7479 2864  g"] = h5.Empty(d
+00003e80: 7479 7065 3d6e 702e 6474 7970 6528 227c  type=np.dtype("|
+00003e90: 5331 2229 290a 2020 2020 2020 2020 6473  S1")).        ds
+00003ea0: 2e64 696d 656e 7369 6f6e 735b 2278 225d  .dimensions["x"]
+00003eb0: 203d 2031 0a20 2020 2020 2020 2076 203d   = 1.        v =
+00003ec0: 2064 732e 6372 6561 7465 5f76 6172 6961   ds.create_varia
+00003ed0: 626c 6528 2278 222c 2028 2278 222c 292c  ble("x", ("x",),
+00003ee0: 2022 6934 2229 0a20 2020 2020 2020 2076   "i4").        v
+00003ef0: 2e61 7474 7273 2e75 7064 6174 6528 7b22  .attrs.update({"
+00003f00: 756e 6974 7322 3a20 226d 6574 6572 7322  units": "meters"
+00003f10: 2c20 2266 6f6f 223a 2022 6261 7222 7d29  , "foo": "bar"})
+00003f20: 0a20 2020 2061 7373 6572 7420 6473 2e5f  .    assert ds._
+00003f30: 636c 6f73 6564 0a20 2020 2077 6974 6820  closed.    with 
+00003f40: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
+00003f50: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+00003f60: 655f 6e65 7463 6466 2c20 2272 2229 2061  e_netcdf, "r") a
+00003f70: 7320 6473 3a0a 2020 2020 2020 2020 6173  s ds:.        as
+00003f80: 7365 7274 206c 656e 2864 732e 6174 7472  sert len(ds.attr
+00003f90: 7329 203d 3d20 320a 2020 2020 2020 2020  s) == 2.        
+00003fa0: 6173 7365 7274 2064 6963 7428 6473 2e61  assert dict(ds.a
+00003fb0: 7474 7273 2920 3d3d 207b 2263 6f6e 7665  ttrs) == {"conve
+00003fc0: 6e74 696f 6e73 223a 2022 4346 222c 2022  ntions": "CF", "
+00003fd0: 656d 7074 795f 7374 7269 6e67 223a 2062  empty_string": b
+00003fe0: 2222 7d0a 2020 2020 2020 2020 6173 7365  ""}.        asse
+00003ff0: 7274 206c 6973 7428 6473 2e61 7474 7273  rt list(ds.attrs
+00004000: 2920 3d3d 205b 2263 6f6e 7665 6e74 696f  ) == ["conventio
+00004010: 6e73 222c 2022 656d 7074 795f 7374 7269  ns", "empty_stri
+00004020: 6e67 225d 0a20 2020 2020 2020 2061 7373  ng"].        ass
+00004030: 6572 7420 6469 6374 2864 735b 2278 225d  ert dict(ds["x"]
+00004040: 2e61 7474 7273 2920 3d3d 207b 2275 6e69  .attrs) == {"uni
+00004050: 7473 223a 2022 6d65 7465 7273 222c 2022  ts": "meters", "
+00004060: 666f 6f22 3a20 2262 6172 227d 0a20 2020  foo": "bar"}.   
+00004070: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+00004080: 6473 5b22 7822 5d2e 6174 7472 7329 203d  ds["x"].attrs) =
+00004090: 3d20 320a 2020 2020 2020 2020 6173 7365  = 2.        asse
+000040a0: 7274 2073 6f72 7465 6428 6473 5b22 7822  rt sorted(ds["x"
+000040b0: 5d2e 6174 7472 7329 203d 3d20 5b22 666f  ].attrs) == ["fo
+000040c0: 6f22 2c20 2275 6e69 7473 225d 0a0a 0a64  o", "units"]...d
+000040d0: 6566 2074 6573 745f 7368 6170 655f 6973  ef test_shape_is
+000040e0: 5f74 6965 645f 746f 5f63 6f6f 7264 696e  _tied_to_coordin
+000040f0: 6174 6528 746d 705f 6c6f 6361 6c5f 6f72  ate(tmp_local_or
+00004100: 5f72 656d 6f74 655f 6e65 7463 6466 293a  _remote_netcdf):
+00004110: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
+00004120: 6466 2e6c 6567 6163 7961 7069 2e44 6174  df.legacyapi.Dat
+00004130: 6173 6574 280a 2020 2020 2020 2020 746d  aset(.        tm
+00004140: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+00004150: 655f 6e65 7463 6466 2c0a 2020 2020 2020  e_netcdf,.      
+00004160: 2020 2277 222c 0a20 2020 2029 2061 7320    "w",.    ) as 
+00004170: 6473 3a0a 2020 2020 2020 2020 6473 2e63  ds:.        ds.c
+00004180: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
+00004190: 7822 2c20 7369 7a65 3d4e 6f6e 6529 0a20  x", size=None). 
+000041a0: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+000041b0: 5661 7269 6162 6c65 2822 7876 6172 222c  Variable("xvar",
+000041c0: 2069 6e74 2c20 2822 7822 2c29 290a 2020   int, ("x",)).  
+000041d0: 2020 2020 2020 6473 5b22 7876 6172 225d        ds["xvar"]
+000041e0: 5b3a 355d 203d 206e 702e 6172 616e 6765  [:5] = np.arange
+000041f0: 2835 290a 2020 2020 2020 2020 6173 7365  (5).        asse
+00004200: 7274 2064 735b 2278 7661 7222 5d2e 7368  rt ds["xvar"].sh
+00004210: 6170 6520 3d3d 2028 352c 290a 2020 2020  ape == (5,).    
+00004220: 2020 2020 6473 2e63 7265 6174 6556 6172      ds.createVar
+00004230: 6961 626c 6528 2279 7661 7222 2c20 696e  iable("yvar", in
+00004240: 742c 2028 2278 222c 2929 0a20 2020 2020  t, ("x",)).     
+00004250: 2020 2064 735b 2279 7661 7222 5d5b 3a31     ds["yvar"][:1
+00004260: 305d 203d 206e 702e 6172 616e 6765 2831  0] = np.arange(1
+00004270: 3029 0a20 2020 2020 2020 2061 7373 6572  0).        asser
+00004280: 7420 6473 5b22 7976 6172 225d 2e73 6861  t ds["yvar"].sha
+00004290: 7065 203d 3d20 2831 302c 290a 2020 2020  pe == (10,).    
+000042a0: 2020 2020 2320 5468 6520 7368 6170 6520      # The shape 
+000042b0: 6f66 2074 6865 2078 7661 7220 7368 6f75  of the xvar shou
+000042c0: 6c64 2063 6861 6e67 6520 746f 6f0a 2020  ld change too.  
+000042d0: 2020 2020 2020 2320 7468 6973 2069 7320        # this is 
+000042e0: 696e 206f 7264 6572 2074 6f20 6265 2069  in order to be i
+000042f0: 6e20 6c69 6e65 2077 6974 6820 7468 6520  n line with the 
+00004300: 6265 6861 7669 6f72 0a20 2020 2020 2020  behavior.       
+00004310: 2023 206f 6620 6e65 7443 4446 342d 630a   # of netCDF4-c.
+00004320: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+00004330: 735b 2278 7661 7222 5d2e 7368 6170 6520  s["xvar"].shape 
+00004340: 3d3d 2028 3130 2c29 0a0a 0a64 6566 2074  == (10,)...def t
+00004350: 6573 745f 6f70 7469 6f6e 616c 5f6e 6574  est_optional_net
+00004360: 6364 6634 5f61 7474 7273 2874 6d70 5f6c  cdf4_attrs(tmp_l
+00004370: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+00004380: 6574 6364 6629 3a0a 2020 2020 6835 203d  etcdf):.    h5 =
+00004390: 2067 6574 5f68 6466 355f 6d6f 6475 6c65   get_hdf5_module
+000043a0: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+000043b0: 6d6f 7465 5f6e 6574 6364 6629 0a20 2020  mote_netcdf).   
+000043c0: 2077 6974 6820 6835 2e46 696c 6528 746d   with h5.File(tm
+000043d0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+000043e0: 655f 6e65 7463 6466 2c20 2277 2229 2061  e_netcdf, "w") a
+000043f0: 7320 663a 0a20 2020 2020 2020 2066 6f6f  s f:.        foo
+00004400: 5f64 6174 6120 3d20 6e70 2e61 7261 6e67  _data = np.arang
+00004410: 6528 3530 292e 7265 7368 6170 6528 352c  e(50).reshape(5,
+00004420: 2031 3029 0a20 2020 2020 2020 2066 2e63   10).        f.c
+00004430: 7265 6174 655f 6461 7461 7365 7428 2266  reate_dataset("f
+00004440: 6f6f 222c 2064 6174 613d 666f 6f5f 6461  oo", data=foo_da
+00004450: 7461 290a 2020 2020 2020 2020 662e 6372  ta).        f.cr
+00004460: 6561 7465 5f64 6174 6173 6574 2822 7822  eate_dataset("x"
+00004470: 2c20 6461 7461 3d6e 702e 6172 616e 6765  , data=np.arange
+00004480: 2835 2929 0a20 2020 2020 2020 2066 2e63  (5)).        f.c
+00004490: 7265 6174 655f 6461 7461 7365 7428 2279  reate_dataset("y
+000044a0: 222c 2064 6174 613d 6e70 2e61 7261 6e67  ", data=np.arang
+000044b0: 6528 3130 2929 0a20 2020 2020 2020 2066  e(10)).        f
+000044c0: 5b22 7822 5d2e 6d61 6b65 5f73 6361 6c65  ["x"].make_scale
+000044d0: 2829 0a20 2020 2020 2020 2066 5b22 7922  ().        f["y"
+000044e0: 5d2e 6d61 6b65 5f73 6361 6c65 2829 0a20  ].make_scale(). 
+000044f0: 2020 2020 2020 2066 5b22 666f 6f22 5d2e         f["foo"].
+00004500: 6469 6d73 5b30 5d2e 6174 7461 6368 5f73  dims[0].attach_s
+00004510: 6361 6c65 2866 5b22 7822 5d29 0a20 2020  cale(f["x"]).   
+00004520: 2020 2020 2066 5b22 666f 6f22 5d2e 6469       f["foo"].di
+00004530: 6d73 5b31 5d2e 6174 7461 6368 5f73 6361  ms[1].attach_sca
+00004540: 6c65 2866 5b22 7922 5d29 0a20 2020 2077  le(f["y"]).    w
+00004550: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
+00004560: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
+00004570: 656d 6f74 655f 6e65 7463 6466 2c20 2272  emote_netcdf, "r
+00004580: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
+00004590: 2020 6173 7365 7274 2064 735b 2266 6f6f    assert ds["foo
+000045a0: 225d 2e64 696d 656e 7369 6f6e 7320 3d3d  "].dimensions ==
+000045b0: 2028 2278 222c 2022 7922 290a 2020 2020   ("x", "y").    
+000045c0: 2020 2020 6173 7365 7274 2064 732e 6469      assert ds.di
+000045d0: 6d65 6e73 696f 6e73 2e6b 6579 7328 2920  mensions.keys() 
+000045e0: 3d3d 207b 2278 222c 2022 7922 7d0a 2020  == {"x", "y"}.  
+000045f0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+00004600: 6469 6d65 6e73 696f 6e73 5b22 7822 5d2e  dimensions["x"].
+00004610: 7369 7a65 203d 3d20 350a 2020 2020 2020  size == 5.      
+00004620: 2020 6173 7365 7274 2064 732e 6469 6d65    assert ds.dime
+00004630: 6e73 696f 6e73 5b22 7922 5d2e 7369 7a65  nsions["y"].size
+00004640: 203d 3d20 3130 0a20 2020 2020 2020 2061   == 10.        a
+00004650: 7373 6572 7420 6172 7261 795f 6571 7561  ssert array_equa
+00004660: 6c28 6473 5b22 666f 6f22 5d2c 2066 6f6f  l(ds["foo"], foo
+00004670: 5f64 6174 6129 0a0a 0a64 6566 2074 6573  _data)...def tes
+00004680: 745f 6572 726f 725f 6861 6e64 6c69 6e67  t_error_handling
+00004690: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+000046a0: 6d6f 7465 5f6e 6574 6364 6629 3a0a 2020  mote_netcdf):.  
+000046b0: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+000046c0: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6f  File(tmp_local_o
+000046d0: 725f 7265 6d6f 7465 5f6e 6574 6364 662c  r_remote_netcdf,
+000046e0: 2022 7722 2920 6173 2064 733a 0a20 2020   "w") as ds:.   
+000046f0: 2020 2020 2064 732e 6469 6d65 6e73 696f       ds.dimensio
+00004700: 6e73 5b22 7822 5d20 3d20 310a 2020 2020  ns["x"] = 1.    
+00004710: 2020 2020 7769 7468 2072 6169 7365 7328      with raises(
+00004720: 5661 6c75 6545 7272 6f72 293a 0a20 2020  ValueError):.   
+00004730: 2020 2020 2020 2020 2064 732e 6469 6d65           ds.dime
+00004740: 6e73 696f 6e73 5b22 7822 5d20 3d20 320a  nsions["x"] = 2.
+00004750: 2020 2020 2020 2020 7769 7468 2072 6169          with rai
+00004760: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
+00004770: 0a20 2020 2020 2020 2020 2020 2064 732e  .            ds.
+00004780: 6469 6d65 6e73 696f 6e73 203d 207b 2278  dimensions = {"x
+00004790: 223a 2032 7d0a 2020 2020 2020 2020 7769  ": 2}.        wi
+000047a0: 7468 2072 6169 7365 7328 5661 6c75 6545  th raises(ValueE
+000047b0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+000047c0: 2020 2064 732e 6469 6d65 6e73 696f 6e73     ds.dimensions
+000047d0: 203d 207b 2279 223a 2033 7d0a 2020 2020   = {"y": 3}.    
+000047e0: 2020 2020 6473 2e63 7265 6174 655f 7661      ds.create_va
+000047f0: 7269 6162 6c65 2822 7822 2c20 2822 7822  riable("x", ("x"
+00004800: 2c29 2c20 6474 7970 653d 666c 6f61 7429  ,), dtype=float)
+00004810: 0a20 2020 2020 2020 2077 6974 6820 7261  .        with ra
+00004820: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+00004830: 3a0a 2020 2020 2020 2020 2020 2020 6473  :.            ds
+00004840: 2e63 7265 6174 655f 7661 7269 6162 6c65  .create_variable
+00004850: 2822 7822 2c20 2822 7822 2c29 2c20 6474  ("x", ("x",), dt
+00004860: 7970 653d 666c 6f61 7429 0a20 2020 2020  ype=float).     
+00004870: 2020 2077 6974 6820 7261 6973 6573 2856     with raises(V
+00004880: 616c 7565 4572 726f 7229 3a0a 2020 2020  alueError):.    
+00004890: 2020 2020 2020 2020 6473 2e63 7265 6174          ds.creat
+000048a0: 655f 7661 7269 6162 6c65 2822 792f 222c  e_variable("y/",
+000048b0: 2028 2278 222c 292c 2064 7479 7065 3d66   ("x",), dtype=f
+000048c0: 6c6f 6174 290a 2020 2020 2020 2020 6473  loat).        ds
+000048d0: 2e63 7265 6174 655f 6772 6f75 7028 2273  .create_group("s
+000048e0: 7562 6772 6f75 7022 290a 2020 2020 2020  ubgroup").      
+000048f0: 2020 7769 7468 2072 6169 7365 7328 5661    with raises(Va
+00004900: 6c75 6545 7272 6f72 293a 0a20 2020 2020  lueError):.     
+00004910: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+00004920: 5f67 726f 7570 2822 7375 6267 726f 7570  _group("subgroup
+00004930: 2229 0a0a 0a64 6566 2074 6573 745f 6465  ")...def test_de
+00004940: 636f 6465 5f73 7472 696e 675f 6572 726f  code_string_erro
+00004950: 7228 746d 705f 6c6f 6361 6c5f 6f72 5f72  r(tmp_local_or_r
+00004960: 656d 6f74 655f 6e65 7463 6466 293a 0a20  emote_netcdf):. 
+00004970: 2020 2077 7269 7465 5f68 356e 6574 6364     write_h5netcd
+00004980: 6628 746d 705f 6c6f 6361 6c5f 6f72 5f72  f(tmp_local_or_r
+00004990: 656d 6f74 655f 6e65 7463 6466 290a 2020  emote_netcdf).  
+000049a0: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+000049b0: 6973 6573 2854 7970 6545 7272 6f72 293a  ises(TypeError):
+000049c0: 0a20 2020 2020 2020 2077 6974 6820 6835  .        with h5
+000049d0: 6e65 7463 6466 2e6c 6567 6163 7961 7069  netcdf.legacyapi
+000049e0: 2e44 6174 6173 6574 280a 2020 2020 2020  .Dataset(.      
+000049f0: 2020 2020 2020 746d 705f 6c6f 6361 6c5f        tmp_local_
+00004a00: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+00004a10: 2c20 2272 222c 2064 6563 6f64 655f 766c  , "r", decode_vl
+00004a20: 656e 5f73 7472 696e 6773 3d54 7275 650a  en_strings=True.
+00004a30: 2020 2020 2020 2020 2920 6173 2064 733a          ) as ds:
+00004a40: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00004a50: 6572 7420 6473 2e6e 616d 6520 3d3d 2022  ert ds.name == "
+00004a60: 2f22 0a0a 0a64 6566 2063 7265 6174 655f  /"...def create_
+00004a70: 696e 7661 6c69 645f 6e65 7463 6466 5f64  invalid_netcdf_d
+00004a80: 6174 6128 293a 0a20 2020 2066 6f6f 5f64  ata():.    foo_d
+00004a90: 6174 6120 3d20 6e70 2e61 7261 6e67 6528  ata = np.arange(
+00004aa0: 3132 3529 2e72 6573 6861 7065 2835 2c20  125).reshape(5, 
+00004ab0: 352c 2035 290a 2020 2020 6261 725f 6461  5, 5).    bar_da
+00004ac0: 7461 203d 206e 702e 6172 616e 6765 2836  ta = np.arange(6
+00004ad0: 3235 292e 7265 7368 6170 6528 3235 2c20  25).reshape(25, 
+00004ae0: 352c 2035 290a 2020 2020 7661 7220 3d20  5, 5).    var = 
+00004af0: 7b22 666f 6f31 223a 2066 6f6f 5f64 6174  {"foo1": foo_dat
+00004b00: 612c 2022 666f 6f32 223a 2062 6172 5f64  a, "foo2": bar_d
+00004b10: 6174 612c 2022 666f 6f33 223a 2066 6f6f  ata, "foo3": foo
+00004b20: 5f64 6174 612c 2022 666f 6f34 223a 2062  _data, "foo4": b
+00004b30: 6172 5f64 6174 617d 0a20 2020 2076 6172  ar_data}.    var
+00004b40: 3220 3d20 7b22 7822 3a20 352c 2022 7922  2 = {"x": 5, "y"
+00004b50: 3a20 352c 2022 7a22 3a20 352c 2022 7831  : 5, "z": 5, "x1
+00004b60: 223a 2032 352c 2022 7931 223a 2035 2c20  ": 25, "y1": 5, 
+00004b70: 227a 3122 3a20 357d 0a20 2020 2072 6574  "z1": 5}.    ret
+00004b80: 7572 6e20 7661 722c 2076 6172 320a 0a0a  urn var, var2...
+00004b90: 6465 6620 6368 6563 6b5f 696e 7661 6c69  def check_invali
+00004ba0: 645f 6e65 7463 6466 3428 7661 722c 2069  d_netcdf4(var, i
+00004bb0: 293a 0a20 2020 2070 6469 6d20 3d20 2270  ):.    pdim = "p
+00004bc0: 686f 6e79 5f64 696d 5f7b 7d22 0a20 2020  hony_dim_{}".   
+00004bd0: 2061 7373 6572 7420 7661 725b 2266 6f6f   assert var["foo
+00004be0: 3122 5d2e 6469 6d65 6e73 696f 6e73 5b30  1"].dimensions[0
+00004bf0: 5d20 3d3d 2070 6469 6d2e 666f 726d 6174  ] == pdim.format
+00004c00: 2869 202a 2034 290a 2020 2020 6173 7365  (i * 4).    asse
+00004c10: 7274 2076 6172 5b22 666f 6f31 225d 2e64  rt var["foo1"].d
+00004c20: 696d 656e 7369 6f6e 735b 315d 203d 3d20  imensions[1] == 
+00004c30: 7064 696d 2e66 6f72 6d61 7428 3120 2b20  pdim.format(1 + 
+00004c40: 6920 2a20 3429 0a20 2020 2061 7373 6572  i * 4).    asser
+00004c50: 7420 7661 725b 2266 6f6f 3122 5d2e 6469  t var["foo1"].di
+00004c60: 6d65 6e73 696f 6e73 5b32 5d20 3d3d 2070  mensions[2] == p
+00004c70: 6469 6d2e 666f 726d 6174 2832 202b 2069  dim.format(2 + i
+00004c80: 202a 2034 290a 2020 2020 6173 7365 7274   * 4).    assert
+00004c90: 2076 6172 5b22 666f 6f32 225d 2e64 696d   var["foo2"].dim
+00004ca0: 656e 7369 6f6e 735b 305d 203d 3d20 7064  ensions[0] == pd
+00004cb0: 696d 2e66 6f72 6d61 7428 3320 2b20 6920  im.format(3 + i 
+00004cc0: 2a20 3429 0a20 2020 2061 7373 6572 7420  * 4).    assert 
+00004cd0: 7661 725b 2266 6f6f 3222 5d2e 6469 6d65  var["foo2"].dime
+00004ce0: 6e73 696f 6e73 5b31 5d20 3d3d 2070 6469  nsions[1] == pdi
+00004cf0: 6d2e 666f 726d 6174 2830 202b 2069 202a  m.format(0 + i *
+00004d00: 2034 290a 2020 2020 6173 7365 7274 2076   4).    assert v
+00004d10: 6172 5b22 666f 6f32 225d 2e64 696d 656e  ar["foo2"].dimen
+00004d20: 7369 6f6e 735b 325d 203d 3d20 7064 696d  sions[2] == pdim
+00004d30: 2e66 6f72 6d61 7428 3120 2b20 6920 2a20  .format(1 + i * 
+00004d40: 3429 0a20 2020 2061 7373 6572 7420 7661  4).    assert va
+00004d50: 725b 2266 6f6f 3322 5d2e 6469 6d65 6e73  r["foo3"].dimens
+00004d60: 696f 6e73 5b30 5d20 3d3d 2070 6469 6d2e  ions[0] == pdim.
+00004d70: 666f 726d 6174 2869 202a 2034 290a 2020  format(i * 4).  
+00004d80: 2020 6173 7365 7274 2076 6172 5b22 666f    assert var["fo
+00004d90: 6f33 225d 2e64 696d 656e 7369 6f6e 735b  o3"].dimensions[
+00004da0: 315d 203d 3d20 7064 696d 2e66 6f72 6d61  1] == pdim.forma
+00004db0: 7428 3120 2b20 6920 2a20 3429 0a20 2020  t(1 + i * 4).   
+00004dc0: 2061 7373 6572 7420 7661 725b 2266 6f6f   assert var["foo
+00004dd0: 3322 5d2e 6469 6d65 6e73 696f 6e73 5b32  3"].dimensions[2
+00004de0: 5d20 3d3d 2070 6469 6d2e 666f 726d 6174  ] == pdim.format
+00004df0: 2832 202b 2069 202a 2034 290a 2020 2020  (2 + i * 4).    
+00004e00: 6173 7365 7274 2076 6172 5b22 666f 6f34  assert var["foo4
+00004e10: 225d 2e64 696d 656e 7369 6f6e 735b 305d  "].dimensions[0]
+00004e20: 203d 3d20 7064 696d 2e66 6f72 6d61 7428   == pdim.format(
+00004e30: 3320 2b20 6920 2a20 3429 0a20 2020 2061  3 + i * 4).    a
+00004e40: 7373 6572 7420 7661 725b 2266 6f6f 3422  ssert var["foo4"
+00004e50: 5d2e 6469 6d65 6e73 696f 6e73 5b31 5d20  ].dimensions[1] 
+00004e60: 3d3d 2070 6469 6d2e 666f 726d 6174 2869  == pdim.format(i
+00004e70: 202a 2034 290a 2020 2020 6173 7365 7274   * 4).    assert
+00004e80: 2076 6172 5b22 666f 6f34 225d 2e64 696d   var["foo4"].dim
+00004e90: 656e 7369 6f6e 735b 325d 203d 3d20 7064  ensions[2] == pd
+00004ea0: 696d 2e66 6f72 6d61 7428 3120 2b20 6920  im.format(1 + i 
+00004eb0: 2a20 3429 0a20 2020 2061 7373 6572 7420  * 4).    assert 
+00004ec0: 7661 725b 2278 225d 2e64 696d 656e 7369  var["x"].dimensi
+00004ed0: 6f6e 735b 305d 203d 3d20 7064 696d 2e66  ons[0] == pdim.f
+00004ee0: 6f72 6d61 7428 6920 2a20 3429 0a20 2020  ormat(i * 4).   
+00004ef0: 2061 7373 6572 7420 7661 725b 2279 225d   assert var["y"]
+00004f00: 2e64 696d 656e 7369 6f6e 735b 305d 203d  .dimensions[0] =
+00004f10: 3d20 7064 696d 2e66 6f72 6d61 7428 6920  = pdim.format(i 
+00004f20: 2a20 3429 0a20 2020 2061 7373 6572 7420  * 4).    assert 
+00004f30: 7661 725b 227a 225d 2e64 696d 656e 7369  var["z"].dimensi
+00004f40: 6f6e 735b 305d 203d 3d20 7064 696d 2e66  ons[0] == pdim.f
+00004f50: 6f72 6d61 7428 6920 2a20 3429 0a20 2020  ormat(i * 4).   
+00004f60: 2061 7373 6572 7420 7661 725b 2278 3122   assert var["x1"
+00004f70: 5d2e 6469 6d65 6e73 696f 6e73 5b30 5d20  ].dimensions[0] 
+00004f80: 3d3d 2070 6469 6d2e 666f 726d 6174 2833  == pdim.format(3
+00004f90: 202b 2069 202a 2034 290a 2020 2020 6173   + i * 4).    as
+00004fa0: 7365 7274 2076 6172 5b22 7931 225d 2e64  sert var["y1"].d
+00004fb0: 696d 656e 7369 6f6e 735b 305d 203d 3d20  imensions[0] == 
+00004fc0: 7064 696d 2e66 6f72 6d61 7428 6920 2a20  pdim.format(i * 
+00004fd0: 3429 0a20 2020 2061 7373 6572 7420 7661  4).    assert va
+00004fe0: 725b 227a 3122 5d2e 6469 6d65 6e73 696f  r["z1"].dimensio
+00004ff0: 6e73 5b30 5d20 3d3d 2070 6469 6d2e 666f  ns[0] == pdim.fo
+00005000: 726d 6174 2869 202a 2034 290a 0a0a 6465  rmat(i * 4)...de
+00005010: 6620 7465 7374 5f69 6e76 616c 6964 5f6e  f test_invalid_n
+00005020: 6574 6364 6634 2874 6d70 5f6c 6f63 616c  etcdf4(tmp_local
+00005030: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
+00005040: 6629 3a0a 2020 2020 6966 2074 6d70 5f6c  f):.    if tmp_l
+00005050: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+00005060: 6574 6364 662e 7374 6172 7473 7769 7468  etcdf.startswith
+00005070: 2872 656d 6f74 655f 6835 293a 0a20 2020  (remote_h5):.   
+00005080: 2020 2020 2070 7974 6573 742e 736b 6970       pytest.skip
+00005090: 2822 6e65 7443 4446 3420 7061 636b 6167  ("netCDF4 packag
+000050a0: 6520 646f 6573 206e 6f74 2077 6f72 6b20  e does not work 
+000050b0: 7769 7468 2072 656d 6f74 6520 4844 4635  with remote HDF5
+000050c0: 2066 696c 6573 2229 0a20 2020 2068 3520   files").    h5 
+000050d0: 3d20 6765 745f 6864 6635 5f6d 6f64 756c  = get_hdf5_modul
+000050e0: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
+000050f0: 656d 6f74 655f 6e65 7463 6466 290a 2020  emote_netcdf).  
+00005100: 2020 7769 7468 2068 352e 4669 6c65 2874    with h5.File(t
+00005110: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
+00005120: 7465 5f6e 6574 6364 662c 2022 7722 2920  te_netcdf, "w") 
+00005130: 6173 2066 3a0a 2020 2020 2020 2020 7661  as f:.        va
+00005140: 722c 2076 6172 3220 3d20 6372 6561 7465  r, var2 = create
+00005150: 5f69 6e76 616c 6964 5f6e 6574 6364 665f  _invalid_netcdf_
+00005160: 6461 7461 2829 0a20 2020 2020 2020 2067  data().        g
+00005170: 7270 7320 3d20 5b22 6261 7222 2c20 2262  rps = ["bar", "b
+00005180: 617a 225d 0a20 2020 2020 2020 2066 6f72  az"].        for
+00005190: 2067 7270 2069 6e20 6772 7073 3a0a 2020   grp in grps:.  
+000051a0: 2020 2020 2020 2020 2020 6678 203d 2066            fx = f
+000051b0: 2e63 7265 6174 655f 6772 6f75 7028 6772  .create_group(gr
+000051c0: 7029 0a20 2020 2020 2020 2020 2020 2066  p).            f
+000051d0: 6f72 206b 2c20 7620 696e 2076 6172 2e69  or k, v in var.i
+000051e0: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+000051f0: 2020 2020 2020 2020 6678 2e63 7265 6174          fx.creat
+00005200: 655f 6461 7461 7365 7428 6b2c 2064 6174  e_dataset(k, dat
+00005210: 613d 7629 0a20 2020 2020 2020 2020 2020  a=v).           
+00005220: 2066 6f72 206b 2c20 7620 696e 2076 6172   for k, v in var
+00005230: 322e 6974 656d 7328 293a 0a20 2020 2020  2.items():.     
+00005240: 2020 2020 2020 2020 2020 2066 782e 6372             fx.cr
+00005250: 6561 7465 5f64 6174 6173 6574 286b 2c20  eate_dataset(k, 
+00005260: 6461 7461 3d6e 702e 6172 616e 6765 2876  data=np.arange(v
+00005270: 2929 0a0a 2020 2020 7769 7468 2068 356e  ))..    with h5n
+00005280: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+00005290: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+000052a0: 6574 6364 662c 2022 7222 2c20 7068 6f6e  etcdf, "r", phon
+000052b0: 795f 6469 6d73 3d22 736f 7274 2229 2061  y_dims="sort") a
+000052c0: 7320 6473 723a 0a20 2020 2020 2020 2066  s dsr:.        f
+000052d0: 6f72 2069 2c20 6772 7020 696e 2065 6e75  or i, grp in enu
+000052e0: 6d65 7261 7465 2867 7270 7329 3a0a 2020  merate(grps):.  
+000052f0: 2020 2020 2020 2020 2020 7661 7220 3d20            var = 
+00005300: 6473 725b 6772 705d 2e76 6172 6961 626c  dsr[grp].variabl
+00005310: 6573 0a20 2020 2020 2020 2020 2020 2063  es.            c
+00005320: 6865 636b 5f69 6e76 616c 6964 5f6e 6574  heck_invalid_net
+00005330: 6364 6634 2876 6172 2c20 6929 0a0a 2020  cdf4(var, i)..  
+00005340: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+00005350: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6f  File(tmp_local_o
+00005360: 725f 7265 6d6f 7465 5f6e 6574 6364 662c  r_remote_netcdf,
+00005370: 2022 7222 2c20 7068 6f6e 795f 6469 6d73   "r", phony_dims
+00005380: 3d22 6163 6365 7373 2229 2061 7320 6473  ="access") as ds
+00005390: 723a 0a20 2020 2020 2020 2066 6f72 2069  r:.        for i
+000053a0: 2c20 6772 7020 696e 2065 6e75 6d65 7261  , grp in enumera
+000053b0: 7465 2867 7270 7329 3a0a 2020 2020 2020  te(grps):.      
+000053c0: 2020 2020 2020 7661 7220 3d20 6473 725b        var = dsr[
+000053d0: 6772 705d 2e76 6172 6961 626c 6573 0a20  grp].variables. 
+000053e0: 2020 2020 2020 2020 2020 2063 6865 636b             check
+000053f0: 5f69 6e76 616c 6964 5f6e 6574 6364 6634  _invalid_netcdf4
+00005400: 2876 6172 2c20 6929 0a0a 2020 2020 6966  (var, i)..    if
+00005410: 206e 6f74 2074 6d70 5f6c 6f63 616c 5f6f   not tmp_local_o
+00005420: 725f 7265 6d6f 7465 5f6e 6574 6364 662e  r_remote_netcdf.
+00005430: 7374 6172 7473 7769 7468 2872 656d 6f74  startswith(remot
+00005440: 655f 6835 293a 0a20 2020 2020 2020 2023  e_h5):.        #
+00005450: 206e 6574 6364 6634 2070 6163 6b61 6765   netcdf4 package
+00005460: 2064 6f65 7320 6e6f 7420 776f 726b 2077   does not work w
+00005470: 6974 6820 7265 6d6f 7465 2048 4446 3520  ith remote HDF5 
+00005480: 6669 6c65 730a 2020 2020 2020 2020 7769  files.        wi
+00005490: 7468 206e 6574 4344 4634 2e44 6174 6173  th netCDF4.Datas
+000054a0: 6574 2874 6d70 5f6c 6f63 616c 5f6f 725f  et(tmp_local_or_
+000054b0: 7265 6d6f 7465 5f6e 6574 6364 662c 2022  remote_netcdf, "
+000054c0: 7222 2920 6173 2064 7372 3a0a 2020 2020  r") as dsr:.    
+000054d0: 2020 2020 2020 2020 666f 7220 692c 2067          for i, g
+000054e0: 7270 2069 6e20 656e 756d 6572 6174 6528  rp in enumerate(
+000054f0: 6772 7073 293a 0a20 2020 2020 2020 2020  grps):.         
+00005500: 2020 2020 2020 2076 6172 203d 2064 7372         var = dsr
+00005510: 5b67 7270 5d2e 7661 7269 6162 6c65 730a  [grp].variables.
+00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005530: 6368 6563 6b5f 696e 7661 6c69 645f 6e65  check_invalid_ne
+00005540: 7463 6466 3428 7661 722c 2069 290a 0a20  tcdf4(var, i).. 
 00005550: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
 00005560: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
 00005570: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-00005580: 2c20 2272 222c 2070 686f 6e79 5f64 696d  , "r", phony_dim
-00005590: 733d 2273 7274 2229 2061 7320 6473 3a0a  s="srt") as ds:.
-000055a0: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-000055b0: 0a0a 0a64 6566 2074 6573 745f 6661 6b65  ...def test_fake
-000055c0: 5f70 686f 6e79 5f64 696d 7328 746d 705f  _phony_dims(tmp_
-000055d0: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-000055e0: 6e65 7463 6466 293a 0a20 2020 2023 2074  netcdf):.    # t
-000055f0: 6573 7473 2077 7269 7469 6e67 206f 6620  ests writing of 
-00005600: 6469 6d65 6e73 696f 6e20 7769 7468 2070  dimension with p
-00005610: 686f 6e79 206e 616d 696e 6720 7363 6865  hony naming sche
-00005620: 6d65 0a20 2020 2023 2073 6565 2068 7474  me.    # see htt
-00005630: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00005640: 6835 6e65 7463 6466 2f68 356e 6574 6364  h5netcdf/h5netcd
-00005650: 662f 6973 7375 6573 2f31 3738 0a20 2020  f/issues/178.   
-00005660: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
-00005670: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
-00005680: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
-00005690: 6d6f 6465 3d22 7722 2920 6173 2064 733a  mode="w") as ds:
-000056a0: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
-000056b0: 6e73 696f 6e73 5b22 7068 6f6e 795f 6469  nsions["phony_di
-000056c0: 6d5f 3022 5d20 3d20 330a 0a0a 6465 6620  m_0"] = 3...def 
-000056d0: 6368 6563 6b5f 696e 7661 6c69 645f 6e65  check_invalid_ne
-000056e0: 7463 6466 345f 6d69 7865 6428 7661 722c  tcdf4_mixed(var,
-000056f0: 2069 293a 0a20 2020 2070 6469 6d20 3d20   i):.    pdim = 
-00005700: 2270 686f 6e79 5f64 696d 5f7b 7d22 2e66  "phony_dim_{}".f
-00005710: 6f72 6d61 7428 6929 0a20 2020 2061 7373  ormat(i).    ass
-00005720: 6572 7420 7661 725b 2266 6f6f 3122 5d2e  ert var["foo1"].
-00005730: 6469 6d65 6e73 696f 6e73 5b30 5d20 3d3d  dimensions[0] ==
-00005740: 2022 7931 220a 2020 2020 6173 7365 7274   "y1".    assert
-00005750: 2076 6172 5b22 666f 6f31 225d 2e64 696d   var["foo1"].dim
-00005760: 656e 7369 6f6e 735b 315d 203d 3d20 227a  ensions[1] == "z
-00005770: 3122 0a20 2020 2061 7373 6572 7420 7661  1".    assert va
-00005780: 725b 2266 6f6f 3122 5d2e 6469 6d65 6e73  r["foo1"].dimens
-00005790: 696f 6e73 5b32 5d20 3d3d 2070 6469 6d0a  ions[2] == pdim.
-000057a0: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
-000057b0: 666f 6f32 225d 2e64 696d 656e 7369 6f6e  foo2"].dimension
-000057c0: 735b 305d 203d 3d20 2278 3122 0a20 2020  s[0] == "x1".   
-000057d0: 2061 7373 6572 7420 7661 725b 2266 6f6f   assert var["foo
-000057e0: 3222 5d2e 6469 6d65 6e73 696f 6e73 5b31  2"].dimensions[1
-000057f0: 5d20 3d3d 2022 7931 220a 2020 2020 6173  ] == "y1".    as
-00005800: 7365 7274 2076 6172 5b22 666f 6f32 225d  sert var["foo2"]
-00005810: 2e64 696d 656e 7369 6f6e 735b 325d 203d  .dimensions[2] =
-00005820: 3d20 227a 3122 0a20 2020 2061 7373 6572  = "z1".    asser
-00005830: 7420 7661 725b 2266 6f6f 3322 5d2e 6469  t var["foo3"].di
-00005840: 6d65 6e73 696f 6e73 5b30 5d20 3d3d 2022  mensions[0] == "
-00005850: 7931 220a 2020 2020 6173 7365 7274 2076  y1".    assert v
-00005860: 6172 5b22 666f 6f33 225d 2e64 696d 656e  ar["foo3"].dimen
-00005870: 7369 6f6e 735b 315d 203d 3d20 227a 3122  sions[1] == "z1"
-00005880: 0a20 2020 2061 7373 6572 7420 7661 725b  .    assert var[
-00005890: 2266 6f6f 3322 5d2e 6469 6d65 6e73 696f  "foo3"].dimensio
-000058a0: 6e73 5b32 5d20 3d3d 2070 6469 6d0a 2020  ns[2] == pdim.  
-000058b0: 2020 6173 7365 7274 2076 6172 5b22 666f    assert var["fo
-000058c0: 6f34 225d 2e64 696d 656e 7369 6f6e 735b  o4"].dimensions[
-000058d0: 305d 203d 3d20 2278 3122 0a20 2020 2061  0] == "x1".    a
-000058e0: 7373 6572 7420 7661 725b 2266 6f6f 3422  ssert var["foo4"
-000058f0: 5d2e 6469 6d65 6e73 696f 6e73 5b31 5d20  ].dimensions[1] 
-00005900: 3d3d 2022 7931 220a 2020 2020 6173 7365  == "y1".    asse
-00005910: 7274 2076 6172 5b22 666f 6f34 225d 2e64  rt var["foo4"].d
-00005920: 696d 656e 7369 6f6e 735b 325d 203d 3d20  imensions[2] == 
-00005930: 227a 3122 0a20 2020 2061 7373 6572 7420  "z1".    assert 
-00005940: 7661 725b 2278 225d 2e64 696d 656e 7369  var["x"].dimensi
-00005950: 6f6e 735b 305d 203d 3d20 2279 3122 0a20  ons[0] == "y1". 
-00005960: 2020 2061 7373 6572 7420 7661 725b 2279     assert var["y
-00005970: 225d 2e64 696d 656e 7369 6f6e 735b 305d  "].dimensions[0]
-00005980: 203d 3d20 2279 3122 0a20 2020 2061 7373   == "y1".    ass
-00005990: 6572 7420 7661 725b 227a 225d 2e64 696d  ert var["z"].dim
-000059a0: 656e 7369 6f6e 735b 305d 203d 3d20 2279  ensions[0] == "y
-000059b0: 3122 0a20 2020 2061 7373 6572 7420 7661  1".    assert va
-000059c0: 725b 2278 3122 5d2e 6469 6d65 6e73 696f  r["x1"].dimensio
-000059d0: 6e73 5b30 5d20 3d3d 2022 7831 220a 2020  ns[0] == "x1".  
-000059e0: 2020 6173 7365 7274 2076 6172 5b22 7931    assert var["y1
-000059f0: 225d 2e64 696d 656e 7369 6f6e 735b 305d  "].dimensions[0]
-00005a00: 203d 3d20 2279 3122 0a20 2020 2061 7373   == "y1".    ass
-00005a10: 6572 7420 7661 725b 227a 3122 5d2e 6469  ert var["z1"].di
-00005a20: 6d65 6e73 696f 6e73 5b30 5d20 3d3d 2022  mensions[0] == "
-00005a30: 7a31 220a 0a0a 6465 6620 7465 7374 5f69  z1"...def test_i
-00005a40: 6e76 616c 6964 5f6e 6574 6364 6634 5f6d  nvalid_netcdf4_m
-00005a50: 6978 6564 2874 6d70 5f6c 6f63 616c 5f6f  ixed(tmp_local_o
-00005a60: 725f 7265 6d6f 7465 5f6e 6574 6364 6629  r_remote_netcdf)
-00005a70: 3a0a 2020 2020 6966 2074 6d70 5f6c 6f63  :.    if tmp_loc
-00005a80: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-00005a90: 6364 662e 7374 6172 7473 7769 7468 2872  cdf.startswith(r
-00005aa0: 656d 6f74 655f 6835 293a 0a20 2020 2020  emote_h5):.     
-00005ab0: 2020 2070 7974 6573 742e 736b 6970 2822     pytest.skip("
-00005ac0: 6e65 7443 4446 3420 7061 636b 6167 6520  netCDF4 package 
-00005ad0: 646f 6573 206e 6f74 2077 6f72 6b20 7769  does not work wi
-00005ae0: 7468 2072 656d 6f74 6520 4844 4635 2066  th remote HDF5 f
-00005af0: 696c 6573 2229 0a20 2020 2068 3520 3d20  iles").    h5 = 
-00005b00: 6765 745f 6864 6635 5f6d 6f64 756c 6528  get_hdf5_module(
-00005b10: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00005b20: 6f74 655f 6e65 7463 6466 290a 2020 2020  ote_netcdf).    
-00005b30: 7769 7468 2068 352e 4669 6c65 2874 6d70  with h5.File(tmp
-00005b40: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00005b50: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
-00005b60: 2066 3a0a 2020 2020 2020 2020 7661 722c   f:.        var,
-00005b70: 2076 6172 3220 3d20 6372 6561 7465 5f69   var2 = create_i
-00005b80: 6e76 616c 6964 5f6e 6574 6364 665f 6461  nvalid_netcdf_da
-00005b90: 7461 2829 0a20 2020 2020 2020 2066 6f72  ta().        for
-00005ba0: 206b 2c20 7620 696e 2076 6172 2e69 7465   k, v in var.ite
-00005bb0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00005bc0: 2020 662e 6372 6561 7465 5f64 6174 6173    f.create_datas
-00005bd0: 6574 286b 2c20 6461 7461 3d76 290a 2020  et(k, data=v).  
-00005be0: 2020 2020 2020 666f 7220 6b2c 2076 2069        for k, v i
-00005bf0: 6e20 7661 7232 2e69 7465 6d73 2829 3a0a  n var2.items():.
-00005c00: 2020 2020 2020 2020 2020 2020 662e 6372              f.cr
-00005c10: 6561 7465 5f64 6174 6173 6574 286b 2c20  eate_dataset(k, 
-00005c20: 6461 7461 3d6e 702e 6172 616e 6765 2876  data=np.arange(v
-00005c30: 2929 0a0a 2020 2020 2020 2020 6966 2076  ))..        if v
-00005c40: 6572 7369 6f6e 2e70 6172 7365 2868 3570  ersion.parse(h5p
-00005c50: 792e 5f5f 7665 7273 696f 6e5f 5f29 203c  y.__version__) <
-00005c60: 2076 6572 7369 6f6e 2e70 6172 7365 2822   version.parse("
-00005c70: 322e 3130 2e30 2229 3a0a 2020 2020 2020  2.10.0"):.      
-00005c80: 2020 2020 2020 665b 2266 6f6f 3222 5d2e        f["foo2"].
-00005c90: 6469 6d73 2e63 7265 6174 655f 7363 616c  dims.create_scal
-00005ca0: 6528 665b 2278 3122 5d29 0a20 2020 2020  e(f["x1"]).     
-00005cb0: 2020 2020 2020 2066 5b22 666f 6f32 225d         f["foo2"]
-00005cc0: 2e64 696d 732e 6372 6561 7465 5f73 6361  .dims.create_sca
-00005cd0: 6c65 2866 5b22 7931 225d 290a 2020 2020  le(f["y1"]).    
-00005ce0: 2020 2020 2020 2020 665b 2266 6f6f 3222          f["foo2"
-00005cf0: 5d2e 6469 6d73 2e63 7265 6174 655f 7363  ].dims.create_sc
-00005d00: 616c 6528 665b 227a 3122 5d29 0a20 2020  ale(f["z1"]).   
-00005d10: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00005d20: 2020 2020 2020 2066 5b22 7831 225d 2e6d         f["x1"].m
-00005d30: 616b 655f 7363 616c 6528 290a 2020 2020  ake_scale().    
-00005d40: 2020 2020 2020 2020 665b 2279 3122 5d2e          f["y1"].
-00005d50: 6d61 6b65 5f73 6361 6c65 2829 0a20 2020  make_scale().   
-00005d60: 2020 2020 2020 2020 2066 5b22 7a31 225d           f["z1"]
-00005d70: 2e6d 616b 655f 7363 616c 6528 290a 2020  .make_scale().  
-00005d80: 2020 2020 2020 665b 2266 6f6f 3222 5d2e        f["foo2"].
-00005d90: 6469 6d73 5b30 5d2e 6174 7461 6368 5f73  dims[0].attach_s
-00005da0: 6361 6c65 2866 5b22 7831 225d 290a 2020  cale(f["x1"]).  
-00005db0: 2020 2020 2020 665b 2266 6f6f 3222 5d2e        f["foo2"].
-00005dc0: 6469 6d73 5b31 5d2e 6174 7461 6368 5f73  dims[1].attach_s
-00005dd0: 6361 6c65 2866 5b22 7931 225d 290a 2020  cale(f["y1"]).  
-00005de0: 2020 2020 2020 665b 2266 6f6f 3222 5d2e        f["foo2"].
-00005df0: 6469 6d73 5b32 5d2e 6174 7461 6368 5f73  dims[2].attach_s
-00005e00: 6361 6c65 2866 5b22 7a31 225d 290a 0a20  cale(f["z1"]).. 
-00005e10: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-00005e20: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-00005e30: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-00005e40: 2c20 2272 222c 2070 686f 6e79 5f64 696d  , "r", phony_dim
-00005e50: 733d 2273 6f72 7422 2920 6173 2064 733a  s="sort") as ds:
-00005e60: 0a20 2020 2020 2020 2076 6172 203d 2064  .        var = d
-00005e70: 732e 7661 7269 6162 6c65 730a 2020 2020  s.variables.    
-00005e80: 2020 2020 6368 6563 6b5f 696e 7661 6c69      check_invali
-00005e90: 645f 6e65 7463 6466 345f 6d69 7865 6428  d_netcdf4_mixed(
-00005ea0: 7661 722c 2033 290a 0a20 2020 2077 6974  var, 3)..    wit
-00005eb0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00005ec0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00005ed0: 6f74 655f 6e65 7463 6466 2c20 2272 222c  ote_netcdf, "r",
-00005ee0: 2070 686f 6e79 5f64 696d 733d 2261 6363   phony_dims="acc
-00005ef0: 6573 7322 2920 6173 2064 733a 0a20 2020  ess") as ds:.   
-00005f00: 2020 2020 2076 6172 203d 2064 732e 7661       var = ds.va
-00005f10: 7269 6162 6c65 730a 2020 2020 2020 2020  riables.        
-00005f20: 6368 6563 6b5f 696e 7661 6c69 645f 6e65  check_invalid_ne
-00005f30: 7463 6466 345f 6d69 7865 6428 7661 722c  tcdf4_mixed(var,
-00005f40: 2030 290a 0a20 2020 2069 6620 6e6f 7420   0)..    if not 
-00005f50: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00005f60: 6f74 655f 6e65 7463 6466 2e73 7461 7274  ote_netcdf.start
-00005f70: 7377 6974 6828 7265 6d6f 7465 5f68 3529  swith(remote_h5)
-00005f80: 3a0a 2020 2020 2020 2020 2320 6e65 7463  :.        # netc
-00005f90: 6466 3420 7061 636b 6167 6520 646f 6573  df4 package does
-00005fa0: 206e 6f74 2077 6f72 6b20 7769 7468 2072   not work with r
-00005fb0: 656d 6f74 6520 4844 4635 2066 696c 6573  emote HDF5 files
-00005fc0: 0a20 2020 2020 2020 2077 6974 6820 6e65  .        with ne
-00005fd0: 7443 4446 342e 4461 7461 7365 7428 746d  tCDF4.Dataset(tm
-00005fe0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
-00005ff0: 655f 6e65 7463 6466 2c20 2272 2229 2061  e_netcdf, "r") a
-00006000: 7320 6473 3a0a 2020 2020 2020 2020 2020  s ds:.          
-00006010: 2020 7661 7220 3d20 6473 2e76 6172 6961    var = ds.varia
-00006020: 626c 6573 0a20 2020 2020 2020 2020 2020  bles.           
-00006030: 2063 6865 636b 5f69 6e76 616c 6964 5f6e   check_invalid_n
-00006040: 6574 6364 6634 5f6d 6978 6564 2876 6172  etcdf4_mixed(var
-00006050: 2c20 3329 0a0a 2020 2020 7769 7468 2068  , 3)..    with h
-00006060: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-00006070: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00006080: 5f6e 6574 6364 662c 2022 7222 2920 6173  _netcdf, "r") as
-00006090: 2064 733a 0a20 2020 2020 2020 2077 6974   ds:.        wit
-000060a0: 6820 7261 6973 6573 2856 616c 7565 4572  h raises(ValueEr
-000060b0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-000060c0: 2020 6473 2e76 6172 6961 626c 6573 5b22    ds.variables["
-000060d0: 666f 6f31 225d 2e64 696d 656e 7369 6f6e  foo1"].dimension
-000060e0: 730a 0a0a 6465 6620 7465 7374 5f69 6e76  s...def test_inv
-000060f0: 616c 6964 5f6e 6574 6364 665f 6d61 6c66  alid_netcdf_malf
-00006100: 6f72 6d65 645f 6469 6d65 6e73 696f 6e5f  ormed_dimension_
-00006110: 7363 616c 6573 2874 6d70 5f6c 6f63 616c  scales(tmp_local
-00006120: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
-00006130: 6629 3a0a 2020 2020 6835 203d 2067 6574  f):.    h5 = get
-00006140: 5f68 6466 355f 6d6f 6475 6c65 2874 6d70  _hdf5_module(tmp
-00006150: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00006160: 5f6e 6574 6364 6629 0a20 2020 2077 6974  _netcdf).    wit
-00006170: 6820 6835 2e46 696c 6528 746d 705f 6c6f  h h5.File(tmp_lo
-00006180: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
-00006190: 7463 6466 2c20 2277 2229 2061 7320 663a  tcdf, "w") as f:
-000061a0: 0a20 2020 2020 2020 2066 6f6f 5f64 6174  .        foo_dat
-000061b0: 6120 3d20 6e70 2e61 7261 6e67 6528 3132  a = np.arange(12
-000061c0: 3529 2e72 6573 6861 7065 2835 2c20 352c  5).reshape(5, 5,
-000061d0: 2035 290a 2020 2020 2020 2020 662e 6372   5).        f.cr
-000061e0: 6561 7465 5f64 6174 6173 6574 2822 666f  eate_dataset("fo
-000061f0: 6f31 222c 2064 6174 613d 666f 6f5f 6461  o1", data=foo_da
-00006200: 7461 290a 2020 2020 2020 2020 662e 6372  ta).        f.cr
-00006210: 6561 7465 5f64 6174 6173 6574 2822 7822  eate_dataset("x"
-00006220: 2c20 6461 7461 3d6e 702e 6172 616e 6765  , data=np.arange
-00006230: 2835 2929 0a20 2020 2020 2020 2066 2e63  (5)).        f.c
-00006240: 7265 6174 655f 6461 7461 7365 7428 2279  reate_dataset("y
-00006250: 222c 2064 6174 613d 6e70 2e61 7261 6e67  ", data=np.arang
-00006260: 6528 3529 290a 2020 2020 2020 2020 662e  e(5)).        f.
-00006270: 6372 6561 7465 5f64 6174 6173 6574 2822  create_dataset("
-00006280: 7a22 2c20 6461 7461 3d6e 702e 6172 616e  z", data=np.aran
-00006290: 6765 2835 2929 0a0a 2020 2020 2020 2020  ge(5))..        
-000062a0: 6966 2076 6572 7369 6f6e 2e70 6172 7365  if version.parse
-000062b0: 2868 3570 792e 5f5f 7665 7273 696f 6e5f  (h5py.__version_
-000062c0: 5f29 203c 2076 6572 7369 6f6e 2e70 6172  _) < version.par
-000062d0: 7365 2822 322e 3130 2e30 2229 3a0a 2020  se("2.10.0"):.  
-000062e0: 2020 2020 2020 2020 2020 665b 2266 6f6f            f["foo
-000062f0: 3122 5d2e 6469 6d73 2e63 7265 6174 655f  1"].dims.create_
-00006300: 7363 616c 6528 665b 2278 225d 290a 2020  scale(f["x"]).  
-00006310: 2020 2020 2020 2020 2020 665b 2266 6f6f            f["foo
-00006320: 3122 5d2e 6469 6d73 2e63 7265 6174 655f  1"].dims.create_
-00006330: 7363 616c 6528 665b 2279 225d 290a 2020  scale(f["y"]).  
-00006340: 2020 2020 2020 2020 2020 665b 2266 6f6f            f["foo
-00006350: 3122 5d2e 6469 6d73 2e63 7265 6174 655f  1"].dims.create_
-00006360: 7363 616c 6528 665b 227a 225d 290a 2020  scale(f["z"]).  
-00006370: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00006380: 2020 2020 2020 2020 665b 2278 225d 2e6d          f["x"].m
-00006390: 616b 655f 7363 616c 6528 290a 2020 2020  ake_scale().    
-000063a0: 2020 2020 2020 2020 665b 2279 225d 2e6d          f["y"].m
-000063b0: 616b 655f 7363 616c 6528 290a 2020 2020  ake_scale().    
-000063c0: 2020 2020 2020 2020 665b 227a 225d 2e6d          f["z"].m
-000063d0: 616b 655f 7363 616c 6528 290a 2020 2020  ake_scale().    
-000063e0: 2020 2020 665b 2266 6f6f 3122 5d2e 6469      f["foo1"].di
-000063f0: 6d73 5b30 5d2e 6174 7461 6368 5f73 6361  ms[0].attach_sca
-00006400: 6c65 2866 5b22 7822 5d29 0a0a 2020 2020  le(f["x"])..    
-00006410: 7769 7468 2072 6169 7365 7328 5661 6c75  with raises(Valu
-00006420: 6545 7272 6f72 293a 0a20 2020 2020 2020  eError):.       
-00006430: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
-00006440: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
-00006450: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
-00006460: 2272 2229 2061 7320 6473 3a0a 2020 2020  "r") as ds:.    
-00006470: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00006480: 730a 2020 2020 2020 2020 2020 2020 7072  s.            pr
-00006490: 696e 7428 6473 290a 0a20 2020 2077 6974  int(ds)..    wit
-000064a0: 6820 7261 6973 6573 2856 616c 7565 4572  h raises(ValueEr
-000064b0: 726f 7229 3a0a 2020 2020 2020 2020 7769  ror):.        wi
-000064c0: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-000064d0: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
-000064e0: 6d6f 7465 5f6e 6574 6364 662c 2022 7222  mote_netcdf, "r"
-000064f0: 2c20 7068 6f6e 795f 6469 6d73 3d22 736f  , phony_dims="so
-00006500: 7274 2229 2061 7320 6473 3a0a 2020 2020  rt") as ds:.    
-00006510: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00006520: 730a 2020 2020 2020 2020 2020 2020 7072  s.            pr
-00006530: 696e 7428 6473 290a 0a0a 6465 6620 7465  int(ds)...def te
-00006540: 7374 5f68 6965 7261 7263 6869 6361 6c5f  st_hierarchical_
-00006550: 6163 6365 7373 5f61 7574 6f5f 6372 6561  access_auto_crea
-00006560: 7465 2874 6d70 5f6c 6f63 616c 5f6f 725f  te(tmp_local_or_
-00006570: 7265 6d6f 7465 5f6e 6574 6364 6629 3a0a  remote_netcdf):.
-00006580: 2020 2020 6473 203d 2068 356e 6574 6364      ds = h5netcd
-00006590: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
-000065a0: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
-000065b0: 662c 2022 7722 290a 2020 2020 6473 2e63  f, "w").    ds.c
-000065c0: 7265 6174 655f 7661 7269 6162 6c65 2822  reate_variable("
-000065d0: 2f66 6f6f 2f62 6172 222c 2064 6174 613d  /foo/bar", data=
-000065e0: 3129 0a20 2020 2067 203d 2064 732e 6372  1).    g = ds.cr
-000065f0: 6561 7465 5f67 726f 7570 2822 666f 6f2f  eate_group("foo/
-00006600: 6261 7a22 290a 2020 2020 672e 6372 6561  baz").    g.crea
-00006610: 7465 5f76 6172 6961 626c 6528 222f 666f  te_variable("/fo
-00006620: 6f2f 6865 6c6c 6f22 2c20 6461 7461 3d32  o/hello", data=2
-00006630: 290a 2020 2020 6173 7365 7274 2073 6574  ).    assert set
-00006640: 2864 7329 203d 3d20 7365 7428 5b22 666f  (ds) == set(["fo
-00006650: 6f22 5d29 0a20 2020 2061 7373 6572 7420  o"]).    assert 
-00006660: 7365 7428 6473 5b22 666f 6f22 5d29 203d  set(ds["foo"]) =
-00006670: 3d20 7365 7428 5b22 6261 7222 2c20 2262  = set(["bar", "b
-00006680: 617a 222c 2022 6865 6c6c 6f22 5d29 0a20  az", "hello"]). 
-00006690: 2020 2064 732e 636c 6f73 6528 290a 0a20     ds.close().. 
-000066a0: 2020 2064 7320 3d20 6835 6e65 7463 6466     ds = h5netcdf
-000066b0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-000066c0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-000066d0: 2c20 2272 2229 0a20 2020 2061 7373 6572  , "r").    asser
-000066e0: 7420 7365 7428 6473 2920 3d3d 2073 6574  t set(ds) == set
-000066f0: 285b 2266 6f6f 225d 290a 2020 2020 6173  (["foo"]).    as
-00006700: 7365 7274 2073 6574 2864 735b 2266 6f6f  sert set(ds["foo
-00006710: 225d 2920 3d3d 2073 6574 285b 2262 6172  "]) == set(["bar
-00006720: 222c 2022 6261 7a22 2c20 2268 656c 6c6f  ", "baz", "hello
-00006730: 225d 290a 2020 2020 6473 2e63 6c6f 7365  "]).    ds.close
-00006740: 2829 0a0a 0a64 6566 2074 6573 745f 4e65  ()...def test_Ne
-00006750: 7463 6466 3444 696d 6964 2874 6d70 5f6c  tcdf4Dimid(tmp_l
-00006760: 6f63 616c 5f6e 6574 6364 6629 3a0a 2020  ocal_netcdf):.  
-00006770: 2020 2320 7265 6772 6573 7369 6f6e 2074    # regression t
-00006780: 6573 7420 666f 7220 6874 7470 733a 2f2f  est for https://
-00006790: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
-000067a0: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
-000067b0: 7565 732f 3533 0a20 2020 2077 6974 6820  ues/53.    with 
-000067c0: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
-000067d0: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-000067e0: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
-000067f0: 2020 2066 2e64 696d 656e 7369 6f6e 735b     f.dimensions[
-00006800: 2278 225d 203d 2031 0a20 2020 2020 2020  "x"] = 1.       
-00006810: 2067 203d 2066 2e63 7265 6174 655f 6772   g = f.create_gr
-00006820: 6f75 7028 2266 6f6f 2229 0a20 2020 2020  oup("foo").     
-00006830: 2020 2067 2e64 696d 656e 7369 6f6e 735b     g.dimensions[
-00006840: 2278 225d 203d 2032 0a20 2020 2020 2020  "x"] = 2.       
-00006850: 2067 2e64 696d 656e 7369 6f6e 735b 2279   g.dimensions["y
-00006860: 225d 203d 2033 0a0a 2020 2020 7769 7468  "] = 3..    with
-00006870: 2068 3570 792e 4669 6c65 2874 6d70 5f6c   h5py.File(tmp_l
-00006880: 6f63 616c 5f6e 6574 6364 662c 2022 7222  ocal_netcdf, "r"
-00006890: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-000068a0: 2320 616c 6c20 6469 6d65 6e73 696f 6e20  # all dimension 
-000068b0: 4944 7320 7368 6f75 6c64 2062 6520 7072  IDs should be pr
-000068c0: 6573 656e 7420 6578 6163 746c 7920 6f6e  esent exactly on
-000068d0: 6365 0a20 2020 2020 2020 2064 696d 5f69  ce.        dim_i
-000068e0: 6473 203d 207b 665b 6e61 6d65 5d2e 6174  ds = {f[name].at
-000068f0: 7472 735b 225f 4e65 7463 6466 3444 696d  trs["_Netcdf4Dim
-00006900: 6964 225d 2066 6f72 206e 616d 6520 696e  id"] for name in
-00006910: 205b 2278 222c 2022 666f 6f2f 7822 2c20   ["x", "foo/x", 
-00006920: 2266 6f6f 2f79 225d 7d0a 2020 2020 2020  "foo/y"]}.      
-00006930: 2020 6173 7365 7274 2064 696d 5f69 6473    assert dim_ids
-00006940: 203d 3d20 7b30 2c20 312c 2032 7d0a 0a0a   == {0, 1, 2}...
-00006950: 6465 6620 7465 7374 5f72 6561 6469 6e67  def test_reading
-00006960: 5f73 7472 5f61 7272 6179 5f66 726f 6d5f  _str_array_from_
-00006970: 6e65 7443 4446 3428 746d 705f 6c6f 6361  netCDF4(tmp_loca
-00006980: 6c5f 6e65 7463 6466 2c20 6465 636f 6465  l_netcdf, decode
-00006990: 5f76 6c65 6e5f 7374 7269 6e67 7329 3a0a  _vlen_strings):.
-000069a0: 2020 2020 2320 5468 6973 2074 6573 7473      # This tests
-000069b0: 2072 6561 6469 6e67 2073 7472 696e 6720   reading string 
-000069c0: 7661 7269 6162 6c65 7320 6372 6561 7465  variables create
-000069d0: 6420 6279 206e 6574 4344 4634 0a20 2020  d by netCDF4.   
-000069e0: 2077 6974 6820 6e65 7443 4446 342e 4461   with netCDF4.Da
-000069f0: 7461 7365 7428 746d 705f 6c6f 6361 6c5f  taset(tmp_local_
-00006a00: 6e65 7463 6466 2c20 2277 2229 2061 7320  netcdf, "w") as 
-00006a10: 6473 3a0a 2020 2020 2020 2020 6473 2e63  ds:.        ds.c
-00006a20: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
-00006a30: 666f 6f31 222c 205f 7374 7269 6e67 5f61  foo1", _string_a
-00006a40: 7272 6179 2e73 6861 7065 5b30 5d29 0a20  rray.shape[0]). 
-00006a50: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
-00006a60: 4469 6d65 6e73 696f 6e28 2266 6f6f 3222  Dimension("foo2"
-00006a70: 2c20 5f73 7472 696e 675f 6172 7261 792e  , _string_array.
-00006a80: 7368 6170 655b 315d 290a 2020 2020 2020  shape[1]).      
-00006a90: 2020 6473 2e63 7265 6174 6556 6172 6961    ds.createVaria
-00006aa0: 626c 6528 2262 6172 222c 2073 7472 2c20  ble("bar", str, 
-00006ab0: 2822 666f 6f31 222c 2022 666f 6f32 2229  ("foo1", "foo2")
-00006ac0: 290a 2020 2020 2020 2020 6473 2e76 6172  ).        ds.var
-00006ad0: 6961 626c 6573 5b22 6261 7222 5d5b 3a5d  iables["bar"][:]
-00006ae0: 203d 205f 7374 7269 6e67 5f61 7272 6179   = _string_array
-00006af0: 0a0a 2020 2020 6473 203d 2068 356e 6574  ..    ds = h5net
-00006b00: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
-00006b10: 616c 5f6e 6574 6364 662c 2022 7222 2c20  al_netcdf, "r", 
-00006b20: 2a2a 6465 636f 6465 5f76 6c65 6e5f 7374  **decode_vlen_st
-00006b30: 7269 6e67 7329 0a0a 2020 2020 7620 3d20  rings)..    v = 
-00006b40: 6473 2e76 6172 6961 626c 6573 5b22 6261  ds.variables["ba
-00006b50: 7222 5d0a 2020 2020 6966 2067 6574 6174  r"].    if getat
-00006b60: 7472 2864 732c 2022 6465 636f 6465 5f76  tr(ds, "decode_v
-00006b70: 6c65 6e5f 7374 7269 6e67 7322 2c20 5472  len_strings", Tr
-00006b80: 7565 293a 0a20 2020 2020 2020 2061 7373  ue):.        ass
-00006b90: 6572 7420 6172 7261 795f 6571 7561 6c28  ert array_equal(
-00006ba0: 762c 205f 7374 7269 6e67 5f61 7272 6179  v, _string_array
-00006bb0: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00006bc0: 2020 2020 6173 7365 7274 2061 7272 6179      assert array
-00006bd0: 5f65 7175 616c 2876 2c20 6e70 2e63 6861  _equal(v, np.cha
-00006be0: 722e 656e 636f 6465 285f 7374 7269 6e67  r.encode(_string
-00006bf0: 5f61 7272 6179 2929 0a0a 2020 2020 6473  _array))..    ds
-00006c00: 2e63 6c6f 7365 2829 0a0a 0a64 6566 2074  .close()...def t
-00006c10: 6573 745f 6e63 5f70 726f 7065 7274 6965  est_nc_propertie
-00006c20: 735f 6e65 7728 746d 705f 6c6f 6361 6c5f  s_new(tmp_local_
-00006c30: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-00006c40: 293a 0a20 2020 2077 6974 6820 6835 6e65  ):.    with h5ne
-00006c50: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
-00006c60: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
-00006c70: 7463 6466 2c20 2277 2229 3a0a 2020 2020  tcdf, "w"):.    
-00006c80: 2020 2020 7061 7373 0a20 2020 2068 3520      pass.    h5 
-00006c90: 3d20 6765 745f 6864 6635 5f6d 6f64 756c  = get_hdf5_modul
-00006ca0: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
-00006cb0: 656d 6f74 655f 6e65 7463 6466 290a 2020  emote_netcdf).  
-00006cc0: 2020 7769 7468 2068 352e 4669 6c65 2874    with h5.File(t
-00006cd0: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
-00006ce0: 7465 5f6e 6574 6364 662c 2022 7222 2920  te_netcdf, "r") 
-00006cf0: 6173 2066 3a0a 2020 2020 2020 2020 6173  as f:.        as
-00006d00: 7365 7274 2062 2268 356e 6574 6364 6622  sert b"h5netcdf"
-00006d10: 2069 6e20 662e 6174 7472 735b 225f 4e43   in f.attrs["_NC
-00006d20: 5072 6f70 6572 7469 6573 225d 0a0a 0a64  Properties"]...d
-00006d30: 6566 2074 6573 745f 6661 696c 6564 5f72  ef test_failed_r
-00006d40: 6561 645f 6f70 656e 5f61 6e64 5f63 6c65  ead_open_and_cle
-00006d50: 616e 5f64 656c 6574 6528 746d 7064 6972  an_delete(tmpdir
-00006d60: 293a 0a20 2020 2023 2041 2066 696c 6520  ):.    # A file 
-00006d70: 7468 6174 2064 6f65 7320 6e6f 7420 6578  that does not ex
-00006d80: 6973 7420 6275 7420 6973 206f 7065 6e65  ist but is opene
-00006d90: 6420 666f 720a 2020 2020 2320 7265 6164  d for.    # read
-00006da0: 696e 6720 7368 6f75 6c64 206f 6e6c 7920  ing should only 
-00006db0: 7261 6973 6520 616e 2049 4f45 7272 6f72  raise an IOError
-00006dc0: 2061 6e64 0a20 2020 2023 206e 6f20 4174   and.    # no At
-00006dd0: 7472 6962 7574 6545 7272 6f72 2061 7420  tributeError at 
-00006de0: 6761 7262 6167 6520 636f 6c6c 6563 7469  garbage collecti
-00006df0: 6f6e 2e0a 2020 2020 7061 7468 203d 2073  on..    path = s
-00006e00: 7472 2874 6d70 6469 722e 6a6f 696e 2822  tr(tmpdir.join("
-00006e10: 7468 6973 5f66 696c 655f 646f 6573 5f6e  this_file_does_n
-00006e20: 6f74 5f65 7869 7374 2e6e 6322 2929 0a20  ot_exist.nc")). 
-00006e30: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006e40: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
-00006e50: 6c65 2870 6174 682c 2022 7222 2920 6173  le(path, "r") as
-00006e60: 2064 733a 0a20 2020 2020 2020 2020 2020   ds:.           
-00006e70: 2061 7373 6572 7420 6473 0a20 2020 2065   assert ds.    e
-00006e80: 7863 6570 7420 494f 4572 726f 723a 0a20  xcept IOError:. 
-00006e90: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00006ea0: 2023 204c 6f6f 6b20 6174 2067 6172 6261   # Look at garba
-00006eb0: 6765 2063 6f6c 6c65 6374 696f 6e3a 0a20  ge collection:. 
-00006ec0: 2020 2023 2041 2073 696d 706c 6520 6763     # A simple gc
-00006ed0: 2e63 6f6c 6c65 6374 2829 2064 6f65 7320  .collect() does 
-00006ee0: 6e6f 7420 7261 6973 6520 616e 2065 7863  not raise an exc
-00006ef0: 6570 7469 6f6e 2e0a 2020 2020 2320 4d75  eption..    # Mu
-00006f00: 7374 2073 6565 6b20 7468 6520 4669 6c65  st seek the File
-00006f10: 206f 626a 6563 7420 616e 6420 696d 6974   object and imit
-00006f20: 6174 6520 6974 7320 6465 6c20 636f 6d6d  ate its del comm
-00006f30: 616e 640a 2020 2020 2320 6279 2066 6f72  and.    # by for
-00006f40: 6369 6e67 2069 7420 746f 2063 6c6f 7365  cing it to close
-00006f50: 2e0a 2020 2020 6f62 6a5f 6c69 7374 203d  ..    obj_list =
-00006f60: 2067 632e 6765 745f 6f62 6a65 6374 7328   gc.get_objects(
-00006f70: 290a 2020 2020 666f 7220 6f62 6a20 696e  ).    for obj in
-00006f80: 206f 626a 5f6c 6973 743a 0a20 2020 2020   obj_list:.     
-00006f90: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00006fa0: 2020 2020 6973 5f68 356e 6574 6364 665f      is_h5netcdf_
-00006fb0: 4669 6c65 203d 2069 7369 6e73 7461 6e63  File = isinstanc
-00006fc0: 6528 6f62 6a2c 2068 356e 6574 6364 662e  e(obj, h5netcdf.
-00006fd0: 4669 6c65 290a 2020 2020 2020 2020 6578  File).        ex
-00006fe0: 6365 7074 2041 7474 7269 6275 7465 4572  cept AttributeEr
-00006ff0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
-00007000: 2069 735f 6835 6e65 7463 6466 5f46 696c   is_h5netcdf_Fil
-00007010: 6520 3d20 4661 6c73 650a 2020 2020 2020  e = False.      
-00007020: 2020 6966 2069 735f 6835 6e65 7463 6466    if is_h5netcdf
-00007030: 5f46 696c 653a 0a20 2020 2020 2020 2020  _File:.         
-00007040: 2020 206f 626a 2e63 6c6f 7365 2829 0a0a     obj.close()..
-00007050: 0a64 6566 2074 6573 745f 6372 6561 7465  .def test_create
-00007060: 5f76 6172 6961 626c 655f 6d61 7463 6869  _variable_matchi
-00007070: 6e67 5f73 6176 6564 5f64 696d 656e 7369  ng_saved_dimensi
-00007080: 6f6e 2874 6d70 5f6c 6f63 616c 5f6f 725f  on(tmp_local_or_
-00007090: 7265 6d6f 7465 5f6e 6574 6364 6629 3a0a  remote_netcdf):.
-000070a0: 2020 2020 6835 203d 2067 6574 5f68 6466      h5 = get_hdf
-000070b0: 355f 6d6f 6475 6c65 2874 6d70 5f6c 6f63  5_module(tmp_loc
-000070c0: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-000070d0: 6364 6629 0a0a 2020 2020 2320 6966 2068  cdf)..    # if h
-000070e0: 3520 6973 206e 6f74 2068 3570 793a 0a20  5 is not h5py:. 
-000070f0: 2020 2023 2020 2020 2070 7974 6573 742e     #     pytest.
-00007100: 7866 6169 6c28 2268 7474 7073 3a2f 2f67  xfail("https://g
-00007110: 6974 6875 622e 636f 6d2f 6835 6e65 7463  ithub.com/h5netc
-00007120: 6466 2f68 356e 6574 6364 662f 6973 7375  df/h5netcdf/issu
-00007130: 6573 2f34 3822 290a 0a20 2020 2077 6974  es/48")..    wit
-00007140: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00007150: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00007160: 6f74 655f 6e65 7463 6466 2c20 2277 2229  ote_netcdf, "w")
-00007170: 2061 7320 663a 0a20 2020 2020 2020 2066   as f:.        f
-00007180: 2e64 696d 656e 7369 6f6e 735b 2278 225d  .dimensions["x"]
-00007190: 203d 2032 0a20 2020 2020 2020 2066 2e63   = 2.        f.c
-000071a0: 7265 6174 655f 7661 7269 6162 6c65 2822  reate_variable("
-000071b0: 7922 2c20 6461 7461 3d5b 312c 2032 5d2c  y", data=[1, 2],
-000071c0: 2064 696d 656e 7369 6f6e 733d 2822 7822   dimensions=("x"
-000071d0: 2c29 290a 0a20 2020 2077 6974 6820 6835  ,))..    with h5
-000071e0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-000071f0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
-00007200: 2c20 2272 2229 2061 7320 663a 0a20 2020  , "r") as f:.   
-00007210: 2020 2020 2064 696d 6c65 6e20 3d20 6622       dimlen = f"
-00007220: 7b66 5b27 7927 5d2e 6469 6d73 5b30 5d2e  {f['y'].dims[0].
-00007230: 7661 6c75 6573 2829 5b30 5d2e 7369 7a65  values()[0].size
-00007240: 3a31 307d 220a 2020 2020 2020 2020 6173  :10}".        as
-00007250: 7365 7274 2066 5b22 7922 5d2e 6469 6d73  sert f["y"].dims
-00007260: 5b30 5d2e 6b65 7973 2829 203d 3d20 5b4e  [0].keys() == [N
-00007270: 4f54 5f41 5f56 4152 4941 424c 452e 6465  OT_A_VARIABLE.de
-00007280: 636f 6465 2822 6173 6369 6922 2920 2b20  code("ascii") + 
-00007290: 6469 6d6c 656e 5d0a 0a20 2020 2077 6974  dimlen]..    wit
-000072a0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-000072b0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-000072c0: 6f74 655f 6e65 7463 6466 2c20 2261 2229  ote_netcdf, "a")
-000072d0: 2061 7320 663a 0a20 2020 2020 2020 2066   as f:.        f
-000072e0: 2e63 7265 6174 655f 7661 7269 6162 6c65  .create_variable
-000072f0: 2822 7822 2c20 6461 7461 3d5b 302c 2031  ("x", data=[0, 1
-00007300: 5d2c 2064 696d 656e 7369 6f6e 733d 2822  ], dimensions=("
-00007310: 7822 2c29 290a 0a20 2020 2077 6974 6820  x",))..    with 
-00007320: 6835 2e46 696c 6528 746d 705f 6c6f 6361  h5.File(tmp_loca
-00007330: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
-00007340: 6466 2c20 2272 2229 2061 7320 663a 0a20  df, "r") as f:. 
-00007350: 2020 2020 2020 2061 7373 6572 7420 665b         assert f[
-00007360: 2279 225d 2e64 696d 735b 305d 2e6b 6579  "y"].dims[0].key
-00007370: 7328 2920 3d3d 205b 2278 225d 0a0a 0a64  s() == ["x"]...d
-00007380: 6566 2074 6573 745f 696e 7661 6c69 645f  ef test_invalid_
-00007390: 6e65 7463 6466 5f65 7272 6f72 2874 6d70  netcdf_error(tmp
-000073a0: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-000073b0: 5f6e 6574 6364 6629 3a0a 2020 2020 6966  _netcdf):.    if
-000073c0: 2074 6d70 5f6c 6f63 616c 5f6f 725f 7265   tmp_local_or_re
-000073d0: 6d6f 7465 5f6e 6574 6364 662e 7374 6172  mote_netcdf.star
-000073e0: 7473 7769 7468 2872 656d 6f74 655f 6835  tswith(remote_h5
-000073f0: 293a 0a20 2020 2020 2020 2070 7974 6573  ):.        pytes
-00007400: 742e 736b 6970 2822 5265 6d6f 7465 2048  t.skip("Remote H
-00007410: 4446 3520 646f 6573 206e 6f74 2079 6574  DF5 does not yet
-00007420: 2073 7570 706f 7274 204c 5a46 2063 6f6d   support LZF com
-00007430: 7072 6573 7369 6f6e 2229 0a20 2020 2077  pression").    w
-00007440: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-00007450: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
-00007460: 656d 6f74 655f 6e65 7463 6466 2c20 2277  emote_netcdf, "w
-00007470: 222c 2069 6e76 616c 6964 5f6e 6574 6364  ", invalid_netcd
-00007480: 663d 4661 6c73 6529 2061 7320 663a 0a20  f=False) as f:. 
-00007490: 2020 2020 2020 2023 2076 616c 6964 0a20         # valid. 
-000074a0: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
-000074b0: 7661 7269 6162 6c65 280a 2020 2020 2020  variable(.      
-000074c0: 2020 2020 2020 226c 7a66 5f63 6f6d 7072        "lzf_compr
-000074d0: 6573 7365 6422 2c20 6461 7461 3d5b 315d  essed", data=[1]
-000074e0: 2c20 6469 6d65 6e73 696f 6e73 3d28 2278  , dimensions=("x
-000074f0: 2229 2c20 636f 6d70 7265 7373 696f 6e3d  "), compression=
-00007500: 226c 7a66 220a 2020 2020 2020 2020 290a  "lzf".        ).
-00007510: 2020 2020 2020 2020 2320 696e 7661 6c69          # invali
-00007520: 640a 2020 2020 2020 2020 7769 7468 2070  d.        with p
-00007530: 7974 6573 742e 7261 6973 6573 2868 356e  ytest.raises(h5n
-00007540: 6574 6364 662e 436f 6d70 6174 6962 696c  etcdf.Compatibil
-00007550: 6974 7945 7272 6f72 293a 0a20 2020 2020  ityError):.     
-00007560: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
-00007570: 7661 7269 6162 6c65 2822 636f 6d70 6c65  variable("comple
-00007580: 7822 2c20 6461 7461 3d31 6a29 0a20 2020  x", data=1j).   
-00007590: 2020 2020 2077 6974 6820 7079 7465 7374       with pytest
-000075a0: 2e72 6169 7365 7328 6835 6e65 7463 6466  .raises(h5netcdf
-000075b0: 2e43 6f6d 7061 7469 6269 6c69 7479 4572  .CompatibilityEr
-000075c0: 726f 7229 3a0a 2020 2020 2020 2020 2020  ror):.          
-000075d0: 2020 662e 6174 7472 735b 2263 6f6d 706c    f.attrs["compl
-000075e0: 6578 5f61 7474 7222 5d20 3d20 316a 0a20  ex_attr"] = 1j. 
-000075f0: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
-00007600: 7374 2e72 6169 7365 7328 6835 6e65 7463  st.raises(h5netc
-00007610: 6466 2e43 6f6d 7061 7469 6269 6c69 7479  df.Compatibility
-00007620: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00007630: 2020 2020 662e 6372 6561 7465 5f76 6172      f.create_var
-00007640: 6961 626c 6528 2273 6361 6c65 6f66 6673  iable("scaleoffs
-00007650: 6574 222c 2064 6174 613d 5b31 5d2c 2064  et", data=[1], d
-00007660: 696d 656e 7369 6f6e 733d 2822 7822 2c29  imensions=("x",)
-00007670: 2c20 7363 616c 656f 6666 7365 743d 3029  , scaleoffset=0)
-00007680: 0a0a 0a64 6566 2074 6573 745f 696e 7661  ...def test_inva
-00007690: 6c69 645f 6e65 7463 6466 5f6f 6b61 7928  lid_netcdf_okay(
-000076a0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-000076b0: 6f74 655f 6e65 7463 6466 293a 0a20 2020  ote_netcdf):.   
-000076c0: 2069 6620 746d 705f 6c6f 6361 6c5f 6f72   if tmp_local_or
-000076d0: 5f72 656d 6f74 655f 6e65 7463 6466 2e73  _remote_netcdf.s
-000076e0: 7461 7274 7377 6974 6828 7265 6d6f 7465  tartswith(remote
-000076f0: 5f68 3529 3a0a 2020 2020 2020 2020 7079  _h5):.        py
-00007700: 7465 7374 2e73 6b69 7028 2268 3570 7964  test.skip("h5pyd
-00007710: 2064 6f65 7320 6e6f 7420 7375 7070 6f72   does not suppor
-00007720: 7420 4e75 6d50 7920 636f 6d70 6c65 7820  t NumPy complex 
-00007730: 6474 7970 6520 7965 7422 290a 2020 2020  dtype yet").    
-00007740: 7769 7468 2070 7974 6573 742e 7761 726e  with pytest.warn
-00007750: 7328 5573 6572 5761 726e 696e 672c 206d  s(UserWarning, m
-00007760: 6174 6368 3d22 696e 7661 6c69 6420 6e65  atch="invalid ne
-00007770: 7463 6466 2066 6561 7475 7265 7322 293a  tcdf features"):
-00007780: 0a20 2020 2020 2020 2077 6974 6820 6835  .        with h5
-00007790: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
-000077a0: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-000077b0: 6e65 7463 6466 2c20 2277 222c 2069 6e76  netcdf, "w", inv
-000077c0: 616c 6964 5f6e 6574 6364 663d 5472 7565  alid_netcdf=True
-000077d0: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-000077e0: 2020 2020 662e 6372 6561 7465 5f76 6172      f.create_var
-000077f0: 6961 626c 6528 0a20 2020 2020 2020 2020  iable(.         
-00007800: 2020 2020 2020 2022 6c7a 665f 636f 6d70         "lzf_comp
-00007810: 7265 7373 6564 222c 2064 6174 613d 5b31  ressed", data=[1
-00007820: 5d2c 2064 696d 656e 7369 6f6e 733d 2822  ], dimensions=("
-00007830: 7822 292c 2063 6f6d 7072 6573 7369 6f6e  x"), compression
-00007840: 3d22 6c7a 6622 0a20 2020 2020 2020 2020  ="lzf".         
-00007850: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00007860: 2066 2e63 7265 6174 655f 7661 7269 6162   f.create_variab
-00007870: 6c65 2822 636f 6d70 6c65 7822 2c20 6461  le("complex", da
-00007880: 7461 3d31 6a29 0a20 2020 2020 2020 2020  ta=1j).         
-00007890: 2020 2066 2e61 7474 7273 5b22 636f 6d70     f.attrs["comp
-000078a0: 6c65 785f 6174 7472 225d 203d 2031 6a0a  lex_attr"] = 1j.
-000078b0: 2020 2020 2020 2020 2020 2020 662e 6372              f.cr
-000078c0: 6561 7465 5f76 6172 6961 626c 6528 2273  eate_variable("s
-000078d0: 6361 6c65 6f66 6673 6574 222c 2064 6174  caleoffset", dat
-000078e0: 613d 5b31 5d2c 2064 696d 656e 7369 6f6e  a=[1], dimension
-000078f0: 733d 2822 7822 2c29 2c20 7363 616c 656f  s=("x",), scaleo
-00007900: 6666 7365 743d 3029 0a20 2020 2077 6974  ffset=0).    wit
-00007910: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00007920: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-00007930: 6f74 655f 6e65 7463 6466 2c20 2272 2229  ote_netcdf, "r")
-00007940: 2061 7320 663a 0a20 2020 2020 2020 206e   as f:.        n
-00007950: 702e 7465 7374 696e 672e 6173 7365 7274  p.testing.assert
-00007960: 5f65 7175 616c 2866 5b22 6c7a 665f 636f  _equal(f["lzf_co
-00007970: 6d70 7265 7373 6564 225d 5b3a 5d2c 205b  mpressed"][:], [
-00007980: 315d 290a 2020 2020 2020 2020 6173 7365  1]).        asse
-00007990: 7274 2066 5b22 636f 6d70 6c65 7822 5d5b  rt f["complex"][
-000079a0: 2e2e 2e5d 203d 3d20 316a 0a20 2020 2020  ...] == 1j.     
-000079b0: 2020 2061 7373 6572 7420 662e 6174 7472     assert f.attr
-000079c0: 735b 2263 6f6d 706c 6578 5f61 7474 7222  s["complex_attr"
-000079d0: 5d20 3d3d 2031 6a0a 2020 2020 2020 2020  ] == 1j.        
-000079e0: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
-000079f0: 745f 6571 7561 6c28 665b 2273 6361 6c65  t_equal(f["scale
-00007a00: 6f66 6673 6574 225d 5b3a 5d2c 205b 315d  offset"][:], [1]
-00007a10: 290a 2020 2020 6835 203d 2067 6574 5f68  ).    h5 = get_h
-00007a20: 6466 355f 6d6f 6475 6c65 2874 6d70 5f6c  df5_module(tmp_l
-00007a30: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
-00007a40: 6574 6364 6629 0a20 2020 2077 6974 6820  etcdf).    with 
-00007a50: 6835 2e46 696c 6528 746d 705f 6c6f 6361  h5.File(tmp_loca
-00007a60: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
-00007a70: 6466 2c20 2272 2229 2061 7320 663a 0a20  df, "r") as f:. 
-00007a80: 2020 2020 2020 2061 7373 6572 7420 225f         assert "_
-00007a90: 4e43 5072 6f70 6572 7469 6573 2220 6e6f  NCProperties" no
-00007aa0: 7420 696e 2066 2e61 7474 7273 0a0a 0a64  t in f.attrs...d
-00007ab0: 6566 2074 6573 745f 696e 7661 6c69 645f  ef test_invalid_
-00007ac0: 6e65 7463 6466 5f6f 7665 7277 7269 7465  netcdf_overwrite
-00007ad0: 5f76 616c 6964 2874 6d70 5f6c 6f63 616c  _valid(tmp_local
-00007ae0: 5f6e 6574 6364 6629 3a0a 2020 2020 2320  _netcdf):.    # 
-00007af0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00007b00: 6f6d 2f68 356e 6574 6364 662f 6835 6e65  om/h5netcdf/h5ne
-00007b10: 7463 6466 2f69 7373 7565 732f 3136 350a  tcdf/issues/165.
-00007b20: 2020 2020 7769 7468 206e 6574 4344 4634      with netCDF4
-00007b30: 2e44 6174 6173 6574 2874 6d70 5f6c 6f63  .Dataset(tmp_loc
-00007b40: 616c 5f6e 6574 6364 662c 206d 6f64 653d  al_netcdf, mode=
-00007b50: 2277 2229 3a0a 2020 2020 2020 2020 7061  "w"):.        pa
-00007b60: 7373 0a20 2020 2077 6974 6820 7079 7465  ss.    with pyte
-00007b70: 7374 2e77 6172 6e73 2855 7365 7257 6172  st.warns(UserWar
-00007b80: 6e69 6e67 293a 0a20 2020 2020 2020 2077  ning):.        w
-00007b90: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-00007ba0: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-00007bb0: 6466 2c20 2261 222c 2069 6e76 616c 6964  df, "a", invalid
-00007bc0: 5f6e 6574 6364 663d 5472 7565 2920 6173  _netcdf=True) as
-00007bd0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-00007be0: 662e 6372 6561 7465 5f76 6172 6961 626c  f.create_variabl
-00007bf0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00007c00: 2020 2022 6c7a 665f 636f 6d70 7265 7373     "lzf_compress
-00007c10: 6564 222c 2064 6174 613d 5b31 5d2c 2064  ed", data=[1], d
-00007c20: 696d 656e 7369 6f6e 733d 2822 7822 292c  imensions=("x"),
-00007c30: 2063 6f6d 7072 6573 7369 6f6e 3d22 6c7a   compression="lz
-00007c40: 6622 0a20 2020 2020 2020 2020 2020 2029  f".            )
-00007c50: 0a20 2020 2020 2020 2020 2020 2066 2e63  .            f.c
-00007c60: 7265 6174 655f 7661 7269 6162 6c65 2822  reate_variable("
-00007c70: 636f 6d70 6c65 7822 2c20 6461 7461 3d31  complex", data=1
-00007c80: 6a29 0a20 2020 2020 2020 2020 2020 2066  j).            f
-00007c90: 2e61 7474 7273 5b22 636f 6d70 6c65 785f  .attrs["complex_
-00007ca0: 6174 7472 225d 203d 2031 6a0a 2020 2020  attr"] = 1j.    
-00007cb0: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
-00007cc0: 5f76 6172 6961 626c 6528 2273 6361 6c65  _variable("scale
-00007cd0: 6f66 6673 6574 222c 2064 6174 613d 5b31  offset", data=[1
-00007ce0: 5d2c 2064 696d 656e 7369 6f6e 733d 2822  ], dimensions=("
-00007cf0: 7822 2c29 2c20 7363 616c 656f 6666 7365  x",), scaleoffse
-00007d00: 743d 3029 0a20 2020 2077 6974 6820 6835  t=0).    with h5
-00007d10: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
-00007d20: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
-00007d30: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
-00007d40: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-00007d50: 7274 5f65 7175 616c 2866 5b22 6c7a 665f  rt_equal(f["lzf_
-00007d60: 636f 6d70 7265 7373 6564 225d 5b3a 5d2c  compressed"][:],
-00007d70: 205b 315d 290a 2020 2020 2020 2020 6173   [1]).        as
-00007d80: 7365 7274 2066 5b22 636f 6d70 6c65 7822  sert f["complex"
-00007d90: 5d5b 2e2e 2e5d 203d 3d20 316a 0a20 2020  ][...] == 1j.   
-00007da0: 2020 2020 2061 7373 6572 7420 662e 6174       assert f.at
-00007db0: 7472 735b 2263 6f6d 706c 6578 5f61 7474  trs["complex_att
-00007dc0: 7222 5d20 3d3d 2031 6a0a 2020 2020 2020  r"] == 1j.      
-00007dd0: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
-00007de0: 6572 745f 6571 7561 6c28 665b 2273 6361  ert_equal(f["sca
-00007df0: 6c65 6f66 6673 6574 225d 5b3a 5d2c 205b  leoffset"][:], [
-00007e00: 315d 290a 2020 2020 6835 203d 2067 6574  1]).    h5 = get
-00007e10: 5f68 6466 355f 6d6f 6475 6c65 2874 6d70  _hdf5_module(tmp
-00007e20: 5f6c 6f63 616c 5f6e 6574 6364 6629 0a20  _local_netcdf). 
-00007e30: 2020 2077 6974 6820 6835 2e46 696c 6528     with h5.File(
-00007e40: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00007e50: 2c20 2272 2229 2061 7320 663a 0a20 2020  , "r") as f:.   
-00007e60: 2020 2020 2061 7373 6572 7420 225f 4e43       assert "_NC
-00007e70: 5072 6f70 6572 7469 6573 2220 6e6f 7420  Properties" not 
-00007e80: 696e 2066 2e61 7474 7273 0a0a 0a64 6566  in f.attrs...def
-00007e90: 2074 6573 745f 7265 6f70 656e 5f66 696c   test_reopen_fil
-00007ea0: 655f 6469 6666 6572 656e 745f 6469 6d65  e_different_dime
-00007eb0: 6e73 696f 6e5f 7369 7a65 7328 746d 705f  nsion_sizes(tmp_
-00007ec0: 6c6f 6361 6c5f 6e65 7463 6466 293a 0a20  local_netcdf):. 
-00007ed0: 2020 2023 2072 6567 7265 7373 696f 6e20     # regression 
-00007ee0: 7465 7374 2066 6f72 2068 7474 7073 3a2f  test for https:/
-00007ef0: 2f67 6974 6875 622e 636f 6d2f 6835 6e65  /github.com/h5ne
-00007f00: 7463 6466 2f68 356e 6574 6364 662f 6973  tcdf/h5netcdf/is
-00007f10: 7375 6573 2f35 350a 2020 2020 7769 7468  sues/55.    with
-00007f20: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
-00007f30: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-00007f40: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
-00007f50: 2020 2020 662e 6372 6561 7465 5f76 6172      f.create_var
-00007f60: 6961 626c 6528 222f 6f6e 652f 666f 6f22  iable("/one/foo"
-00007f70: 2c20 6461 7461 3d5b 315d 2c20 6469 6d65  , data=[1], dime
-00007f80: 6e73 696f 6e73 3d28 2278 222c 2929 0a20  nsions=("x",)). 
-00007f90: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-00007fa0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-00007fb0: 6e65 7463 6466 2c20 2261 2229 2061 7320  netcdf, "a") as 
-00007fc0: 663a 0a20 2020 2020 2020 2066 2e63 7265  f:.        f.cre
-00007fd0: 6174 655f 7661 7269 6162 6c65 2822 2f74  ate_variable("/t
-00007fe0: 776f 2f66 6f6f 222c 2064 6174 613d 5b31  wo/foo", data=[1
-00007ff0: 2c20 325d 2c20 6469 6d65 6e73 696f 6e73  , 2], dimensions
-00008000: 3d28 2278 222c 2929 0a20 2020 2077 6974  =("x",)).    wit
-00008010: 6820 6e65 7443 4446 342e 4461 7461 7365  h netCDF4.Datase
-00008020: 7428 746d 705f 6c6f 6361 6c5f 6e65 7463  t(tmp_local_netc
-00008030: 6466 2c20 2272 2229 2061 7320 663a 0a20  df, "r") as f:. 
-00008040: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
-00008050: 6772 6f75 7073 5b22 6f6e 6522 5d2e 7661  groups["one"].va
-00008060: 7269 6162 6c65 735b 2266 6f6f 225d 5b2e  riables["foo"][.
-00008070: 2e2e 5d2e 7368 6170 6520 3d3d 2028 312c  ..].shape == (1,
-00008080: 290a 0a0a 6465 6620 7465 7374 5f69 6e76  )...def test_inv
-00008090: 616c 6964 5f74 6865 6e5f 7661 6c69 645f  alid_then_valid_
-000080a0: 6e6f 5f6e 6370 726f 7065 7274 6965 7328  no_ncproperties(
-000080b0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
-000080c0: 6f74 655f 6e65 7463 6466 293a 0a20 2020  ote_netcdf):.   
-000080d0: 2077 6974 6820 7079 7465 7374 2e77 6172   with pytest.war
-000080e0: 6e73 2855 7365 7257 6172 6e69 6e67 2c20  ns(UserWarning, 
-000080f0: 6d61 7463 683d 2269 6e76 616c 6964 206e  match="invalid n
-00008100: 6574 6364 6620 6665 6174 7572 6573 2229  etcdf features")
-00008110: 3a0a 2020 2020 2020 2020 7769 7468 2068  :.        with h
-00008120: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-00008130: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
-00008140: 5f6e 6574 6364 662c 2022 7722 2c20 696e  _netcdf, "w", in
-00008150: 7661 6c69 645f 6e65 7463 6466 3d54 7275  valid_netcdf=Tru
-00008160: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00008170: 7061 7373 0a20 2020 2077 6974 6820 6835  pass.    with h5
-00008180: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
-00008190: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-000081a0: 6e65 7463 6466 2c20 2261 2229 3a0a 2020  netcdf, "a"):.  
-000081b0: 2020 2020 2020 7061 7373 0a20 2020 2068        pass.    h
-000081c0: 3520 3d20 6765 745f 6864 6635 5f6d 6f64  5 = get_hdf5_mod
-000081d0: 756c 6528 746d 705f 6c6f 6361 6c5f 6f72  ule(tmp_local_or
-000081e0: 5f72 656d 6f74 655f 6e65 7463 6466 290a  _remote_netcdf).
-000081f0: 2020 2020 7769 7468 2068 352e 4669 6c65      with h5.File
-00008200: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
-00008210: 6d6f 7465 5f6e 6574 6364 662c 2022 7222  mote_netcdf, "r"
-00008220: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00008230: 2320 7374 696c 6c20 6e6f 7420 6120 7661  # still not a va
-00008240: 6c69 6420 6e65 7463 6466 2066 696c 650a  lid netcdf file.
-00008250: 2020 2020 2020 2020 6173 7365 7274 2022          assert "
-00008260: 5f4e 4350 726f 7065 7274 6965 7322 206e  _NCProperties" n
-00008270: 6f74 2069 6e20 662e 6174 7472 730a 0a0a  ot in f.attrs...
-00008280: 6465 6620 7465 7374 5f63 7265 6174 696e  def test_creatin
-00008290: 675f 616e 645f 7265 7369 7a69 6e67 5f75  g_and_resizing_u
-000082a0: 6e6c 696d 6974 6564 5f64 696d 656e 7369  nlimited_dimensi
-000082b0: 6f6e 7328 746d 705f 6c6f 6361 6c5f 6f72  ons(tmp_local_or
-000082c0: 5f72 656d 6f74 655f 6e65 7463 6466 293a  _remote_netcdf):
-000082d0: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-000082e0: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-000082f0: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
-00008300: 6466 2c20 2277 2229 2061 7320 663a 0a20  df, "w") as f:. 
-00008310: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
-00008320: 6f6e 735b 2278 225d 203d 204e 6f6e 650a  ons["x"] = None.
-00008330: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
-00008340: 696f 6e73 5b22 7922 5d20 3d20 3135 0a20  ions["y"] = 15. 
-00008350: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
-00008360: 6f6e 735b 227a 225d 203d 204e 6f6e 650a  ons["z"] = None.
-00008370: 2020 2020 2020 2020 662e 7265 7369 7a65          f.resize
-00008380: 5f64 696d 656e 7369 6f6e 2822 7a22 2c20  _dimension("z", 
-00008390: 3230 290a 0a20 2020 2020 2020 2077 6974  20)..        wit
-000083a0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
-000083b0: 5661 6c75 6545 7272 6f72 2920 6173 2065  ValueError) as e
-000083c0: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
-000083d0: 7265 7369 7a65 5f64 696d 656e 7369 6f6e  resize_dimension
-000083e0: 2822 7922 2c20 3230 290a 2020 2020 2020  ("y", 20).      
-000083f0: 2020 6173 7365 7274 2065 2e76 616c 7565    assert e.value
-00008400: 2e61 7267 735b 305d 203d 3d20 280a 2020  .args[0] == (.  
-00008410: 2020 2020 2020 2020 2020 2244 696d 656e            "Dimen
-00008420: 7369 6f6e 2027 7927 2069 7320 6e6f 7420  sion 'y' is not 
-00008430: 756e 6c69 6d69 7465 6420 616e 6420 7468  unlimited and th
-00008440: 7573 2063 616e 6e6f 7420 6265 2072 6573  us cannot be res
-00008450: 697a 6564 2e22 0a20 2020 2020 2020 2029  ized.".        )
-00008460: 0a0a 2020 2020 6835 203d 2067 6574 5f68  ..    h5 = get_h
-00008470: 6466 355f 6d6f 6475 6c65 2874 6d70 5f6c  df5_module(tmp_l
-00008480: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
-00008490: 6574 6364 6629 0a20 2020 2023 2041 7373  etcdf).    # Ass
-000084a0: 6572 7420 736f 6d65 2062 6568 6176 696f  ert some behavio
-000084b0: 7220 6f62 7365 7276 6564 2062 7920 7573  r observed by us
-000084c0: 696e 6720 7468 6520 4320 6e65 7443 4446  ing the C netCDF
-000084d0: 2062 696e 6469 6e67 732e 0a20 2020 2077   bindings..    w
-000084e0: 6974 6820 6835 2e46 696c 6528 746d 705f  ith h5.File(tmp_
-000084f0: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
-00008500: 6e65 7463 6466 2c20 2272 2229 2061 7320  netcdf, "r") as 
-00008510: 663a 0a20 2020 2020 2020 2061 7373 6572  f:.        asser
-00008520: 7420 665b 2278 225d 2e73 6861 7065 203d  t f["x"].shape =
-00008530: 3d20 2830 2c29 0a20 2020 2020 2020 2061  = (0,).        a
-00008540: 7373 6572 7420 665b 2278 225d 2e6d 6178  ssert f["x"].max
-00008550: 7368 6170 6520 3d3d 2028 4e6f 6e65 2c29  shape == (None,)
-00008560: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00008570: 665b 2279 225d 2e73 6861 7065 203d 3d20  f["y"].shape == 
-00008580: 2831 352c 290a 2020 2020 2020 2020 6173  (15,).        as
-00008590: 7365 7274 2066 5b22 7922 5d2e 6d61 7873  sert f["y"].maxs
-000085a0: 6861 7065 203d 3d20 2831 352c 290a 2020  hape == (15,).  
-000085b0: 2020 2020 2020 6173 7365 7274 2066 5b22        assert f["
-000085c0: 7a22 5d2e 7368 6170 6520 3d3d 2028 3230  z"].shape == (20
-000085d0: 2c29 0a20 2020 2020 2020 2061 7373 6572  ,).        asser
-000085e0: 7420 665b 227a 225d 2e6d 6178 7368 6170  t f["z"].maxshap
-000085f0: 6520 3d3d 2028 4e6f 6e65 2c29 0a0a 0a64  e == (None,)...d
-00008600: 6566 2074 6573 745f 6372 6561 7469 6e67  ef test_creating
-00008610: 5f76 6172 6961 626c 6573 5f77 6974 685f  _variables_with_
-00008620: 756e 6c69 6d69 7465 645f 6469 6d65 6e73  unlimited_dimens
-00008630: 696f 6e73 2874 6d70 5f6c 6f63 616c 5f6f  ions(tmp_local_o
-00008640: 725f 7265 6d6f 7465 5f6e 6574 6364 6629  r_remote_netcdf)
-00008650: 3a0a 2020 2020 7769 7468 2068 356e 6574  :.    with h5net
-00008660: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
-00008670: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-00008680: 6364 662c 2022 7722 2920 6173 2066 3a0a  cdf, "w") as f:.
-00008690: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
-000086a0: 696f 6e73 5b22 7822 5d20 3d20 4e6f 6e65  ions["x"] = None
-000086b0: 0a20 2020 2020 2020 2066 2e64 696d 656e  .        f.dimen
-000086c0: 7369 6f6e 735b 2279 225d 203d 2032 0a0a  sions["y"] = 2..
-000086d0: 2020 2020 2020 2020 2320 4372 6561 7469          # Creati
-000086e0: 6e67 2061 2076 6172 6961 626c 6520 7769  ng a variable wi
-000086f0: 7468 6f75 7420 6461 7461 2077 696c 6c20  thout data will 
-00008700: 696e 6974 6961 6c69 7a65 2061 6e20 6172  initialize an ar
-00008710: 7261 7920 7769 7468 207a 6572 6f0a 2020  ray with zero.  
-00008720: 2020 2020 2020 2320 6c65 6e67 7468 2e0a        # length..
-00008730: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
-00008740: 5f76 6172 6961 626c 6528 2264 756d 6d79  _variable("dummy
-00008750: 222c 2064 696d 656e 7369 6f6e 733d 2822  ", dimensions=("
-00008760: 7822 2c20 2279 2229 2c20 6474 7970 653d  x", "y"), dtype=
-00008770: 6e70 2e69 6e74 3634 290a 2020 2020 2020  np.int64).      
-00008780: 2020 6173 7365 7274 2066 2e76 6172 6961    assert f.varia
-00008790: 626c 6573 5b22 6475 6d6d 7922 5d2e 7368  bles["dummy"].sh
-000087a0: 6170 6520 3d3d 2028 302c 2032 290a 2020  ape == (0, 2).  
-000087b0: 2020 2020 2020 6173 7365 7274 2066 2e76        assert f.v
-000087c0: 6172 6961 626c 6573 5b22 6475 6d6d 7922  ariables["dummy"
-000087d0: 5d2e 5f68 3564 732e 6d61 7873 6861 7065  ]._h5ds.maxshape
-000087e0: 203d 3d20 284e 6f6e 652c 2032 290a 0a20   == (None, 2).. 
-000087f0: 2020 2020 2020 2023 2054 7279 696e 6720         # Trying 
-00008800: 746f 2063 7265 6174 6520 6120 7661 7269  to create a vari
-00008810: 6162 6c65 2077 6869 6c65 2074 6865 2063  able while the c
-00008820: 7572 7265 6e74 2073 697a 6520 6f66 2074  urrent size of t
-00008830: 6865 2064 696d 656e 7369 6f6e 0a20 2020  he dimension.   
-00008840: 2020 2020 2023 2069 7320 7374 696c 6c20       # is still 
-00008850: 7a65 726f 2077 696c 6c20 6661 696c 2e0a  zero will fail..
-00008860: 2020 2020 2020 2020 7769 7468 2070 7974          with pyt
-00008870: 6573 742e 7261 6973 6573 2856 616c 7565  est.raises(Value
-00008880: 4572 726f 7229 2061 7320 653a 0a20 2020  Error) as e:.   
-00008890: 2020 2020 2020 2020 2066 2e63 7265 6174           f.creat
-000088a0: 655f 7661 7269 6162 6c65 280a 2020 2020  e_variable(.    
-000088b0: 2020 2020 2020 2020 2020 2020 2264 756d              "dum
-000088c0: 6d79 3222 2c20 6461 7461 3d6e 702e 6172  my2", data=np.ar
-000088d0: 7261 7928 5b5b 312c 2032 5d2c 205b 332c  ray([[1, 2], [3,
-000088e0: 2034 5d5d 292c 2064 696d 656e 7369 6f6e   4]]), dimension
-000088f0: 733d 2822 7822 2c20 2279 2229 0a20 2020  s=("x", "y").   
-00008900: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008910: 2020 2061 7373 6572 7420 652e 7661 6c75     assert e.valu
-00008920: 652e 6172 6773 5b30 5d20 3d3d 2022 5368  e.args[0] == "Sh
-00008930: 6170 6520 7475 706c 6520 6973 2069 6e63  ape tuple is inc
-00008940: 6f6d 7061 7469 626c 6520 7769 7468 2064  ompatible with d
-00008950: 6174 6122 0a0a 2020 2020 2020 2020 2320  ata"..        # 
-00008960: 4372 6561 7469 6e67 2061 2063 6f6f 7264  Creating a coord
-00008970: 696e 6174 6520 7661 7269 6162 6c65 0a20  inate variable. 
-00008980: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
-00008990: 7661 7269 6162 6c65 2822 7822 2c20 6469  variable("x", di
-000089a0: 6d65 6e73 696f 6e73 3d28 2278 222c 292c  mensions=("x",),
-000089b0: 2064 7479 7065 3d6e 702e 696e 7436 3429   dtype=np.int64)
-000089c0: 0a0a 2020 2020 2020 2020 2320 5265 7369  ..        # Resi
-000089d0: 7a65 2064 6174 612e 0a20 2020 2020 2020  ze data..       
-000089e0: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
-000089f0: 6c65 735b 2264 756d 6d79 225d 2e73 6861  les["dummy"].sha
-00008a00: 7065 203d 3d20 2830 2c20 3229 0a20 2020  pe == (0, 2).   
-00008a10: 2020 2020 2066 2e72 6573 697a 655f 6469       f.resize_di
-00008a20: 6d65 6e73 696f 6e28 2278 222c 2033 290a  mension("x", 3).
-00008a30: 2020 2020 2020 2020 2320 5468 6973 2077          # This w
-00008a40: 696c 6c20 616c 736f 2066 6f72 6365 2061  ill also force a
-00008a50: 2072 6573 697a 6520 6f66 2074 6865 2065   resize of the e
-00008a60: 7869 7374 696e 6720 7661 7269 6162 6c65  xisting variable
-00008a70: 7320 616e 6420 6974 2077 696c 6c0a 2020  s and it will.  
-00008a80: 2020 2020 2020 2320 6265 2070 6164 6465        # be padde
-00008a90: 6420 7769 7468 207a 6572 6f73 2e0a 2020  d with zeros..  
-00008aa0: 2020 2020 2020 6173 7365 7274 2066 2e64        assert f.d
-00008ab0: 696d 656e 7369 6f6e 735b 2278 225d 2e73  imensions["x"].s
-00008ac0: 697a 6520 3d3d 2033 0a20 2020 2020 2020  ize == 3.       
-00008ad0: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-00008ae0: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
-00008af0: 7269 6162 6c65 735b 2264 756d 6d79 225d  riables["dummy"]
-00008b00: 2c20 6e70 2e7a 6572 6f73 2828 332c 2032  , np.zeros((3, 2
-00008b10: 2929 290a 0a20 2020 2020 2020 2023 2043  )))..        # C
-00008b20: 7265 6174 696e 6720 616e 6f74 6865 7220  reating another 
-00008b30: 7661 7269 6162 6c65 2077 6974 6820 6e6f  variable with no
-00008b40: 2064 6174 6120 7769 6c6c 206e 6f77 2061   data will now a
-00008b50: 6c73 6f20 7461 6b65 2074 6865 2073 6861  lso take the sha
-00008b60: 7065 0a20 2020 2020 2020 2023 206f 6620  pe.        # of 
-00008b70: 7468 6520 6375 7272 656e 7420 6469 6d65  the current dime
-00008b80: 6e73 696f 6e73 2e0a 2020 2020 2020 2020  nsions..        
-00008b90: 662e 6372 6561 7465 5f76 6172 6961 626c  f.create_variabl
-00008ba0: 6528 2264 756d 6d79 3322 2c20 6469 6d65  e("dummy3", dime
-00008bb0: 6e73 696f 6e73 3d28 2278 222c 2022 7922  nsions=("x", "y"
-00008bc0: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
-00008bd0: 3429 0a20 2020 2020 2020 2061 7373 6572  4).        asser
-00008be0: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
-00008bf0: 756d 6d79 3322 5d2e 7368 6170 6520 3d3d  ummy3"].shape ==
-00008c00: 2028 332c 2032 290a 2020 2020 2020 2020   (3, 2).        
-00008c10: 6173 7365 7274 2066 2e76 6172 6961 626c  assert f.variabl
-00008c20: 6573 5b22 6475 6d6d 7933 225d 2e5f 6835  es["dummy3"]._h5
-00008c30: 6473 2e6d 6178 7368 6170 6520 3d3d 2028  ds.maxshape == (
-00008c40: 4e6f 6e65 2c20 3229 0a20 2020 2020 2020  None, 2).       
-00008c50: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-00008c60: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
-00008c70: 7269 6162 6c65 735b 2264 756d 6d79 3322  riables["dummy3"
-00008c80: 5d2c 206e 702e 7a65 726f 7328 2833 2c20  ], np.zeros((3, 
-00008c90: 3229 2929 0a0a 2020 2020 2020 2020 2320  2)))..        # 
-00008ca0: 5772 6974 696e 6720 746f 2061 2076 6172  Writing to a var
-00008cb0: 6961 626c 6520 7769 7468 2061 6e20 756e  iable with an un
-00008cc0: 6c69 6d69 7465 6420 6469 6d65 6e73 696f  limited dimensio
-00008cd0: 6e20 7261 6973 6573 0a20 2020 2020 2020  n raises.       
-00008ce0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00008cf0: 7365 7328 5479 7065 4572 726f 7229 2061  ses(TypeError) a
-00008d00: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
-00008d10: 2066 2e76 6172 6961 626c 6573 5b22 6475   f.variables["du
-00008d20: 6d6d 7933 225d 5b3a 5d20 3d20 6e70 2e6f  mmy3"][:] = np.o
-00008d30: 6e65 7328 2835 2c20 3229 290a 2020 2020  nes((5, 2)).    
-00008d40: 2020 2020 6173 7365 7274 2065 2e76 616c      assert e.val
-00008d50: 7565 2e61 7267 735b 305d 203d 3d20 2243  ue.args[0] == "C
-00008d60: 616e 2774 2062 726f 6164 6361 7374 2028  an't broadcast (
-00008d70: 352c 2032 2920 2d3e 2028 332c 2032 2922  5, 2) -> (3, 2)"
-00008d80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00008d90: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-00008da0: 6d79 3322 5d2e 7368 6170 6520 3d3d 2028  my3"].shape == (
-00008db0: 332c 2032 290a 2020 2020 2020 2020 6173  3, 2).        as
-00008dc0: 7365 7274 2066 2e76 6172 6961 626c 6573  sert f.variables
-00008dd0: 5b22 6475 6d6d 7933 225d 2e5f 6835 6473  ["dummy3"]._h5ds
-00008de0: 2e6d 6178 7368 6170 6520 3d3d 2028 4e6f  .maxshape == (No
-00008df0: 6e65 2c20 3229 0a20 2020 2020 2020 2061  ne, 2).        a
-00008e00: 7373 6572 7420 665b 2278 225d 2e73 6861  ssert f["x"].sha
-00008e10: 7065 203d 3d20 2833 2c29 0a20 2020 2020  pe == (3,).     
-00008e20: 2020 2061 7373 6572 7420 662e 6469 6d65     assert f.dime
-00008e30: 6e73 696f 6e73 5b22 7822 5d2e 7369 7a65  nsions["x"].size
-00008e40: 203d 3d20 330a 2020 2020 2020 2020 6e70   == 3.        np
-00008e50: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
-00008e60: 616c 6c63 6c6f 7365 2866 2e76 6172 6961  allclose(f.varia
-00008e70: 626c 6573 5b22 6475 6d6d 7933 225d 2c20  bles["dummy3"], 
-00008e80: 6e70 2e7a 6572 6f73 2828 332c 2032 2929  np.zeros((3, 2))
-00008e90: 290a 0a20 2020 2023 2043 6c6f 7365 2061  )..    # Close a
-00008ea0: 6e64 2072 6561 6420 6167 6169 6e20 746f  nd read again to
-00008eb0: 2061 6c73 6f20 7465 7374 2063 6f72 7265   also test corre
-00008ec0: 6374 2070 6172 7369 6e67 206f 6620 756e  ct parsing of un
-00008ed0: 6c69 6d69 7465 640a 2020 2020 2320 6469  limited.    # di
-00008ee0: 6d65 6e73 696f 6e73 2e0a 2020 2020 7769  mensions..    wi
-00008ef0: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-00008f00: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
-00008f10: 6d6f 7465 5f6e 6574 6364 662c 2022 7222  mote_netcdf, "r"
-00008f20: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00008f30: 6173 7365 7274 2066 2e64 696d 656e 7369  assert f.dimensi
-00008f40: 6f6e 735b 2278 225d 2e69 7375 6e6c 696d  ons["x"].isunlim
-00008f50: 6974 6564 2829 0a20 2020 2020 2020 2061  ited().        a
-00008f60: 7373 6572 7420 662e 6469 6d65 6e73 696f  ssert f.dimensio
-00008f70: 6e73 5b22 7822 5d2e 7369 7a65 203d 3d20  ns["x"].size == 
-00008f80: 330a 2020 2020 2020 2020 6173 7365 7274  3.        assert
-00008f90: 2066 2e5f 6835 6669 6c65 5b22 7822 5d2e   f._h5file["x"].
-00008fa0: 6d61 7873 6861 7065 203d 3d20 284e 6f6e  maxshape == (Non
-00008fb0: 652c 290a 2020 2020 2020 2020 6173 7365  e,).        asse
-00008fc0: 7274 2066 2e5f 6835 6669 6c65 5b22 7822  rt f._h5file["x"
-00008fd0: 5d2e 7368 6170 6520 3d3d 2028 332c 290a  ].shape == (3,).
-00008fe0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00008ff0: 662e 6469 6d65 6e73 696f 6e73 5b22 7922  f.dimensions["y"
-00009000: 5d2e 7369 7a65 203d 3d20 320a 2020 2020  ].size == 2.    
-00009010: 2020 2020 6173 7365 7274 2066 2e5f 6835      assert f._h5
-00009020: 6669 6c65 5b22 7922 5d2e 6d61 7873 6861  file["y"].maxsha
-00009030: 7065 203d 3d20 2832 2c29 0a20 2020 2020  pe == (2,).     
-00009040: 2020 2061 7373 6572 7420 662e 5f68 3566     assert f._h5f
-00009050: 696c 655b 2279 225d 2e73 6861 7065 203d  ile["y"].shape =
-00009060: 3d20 2832 2c29 0a0a 0a64 6566 2074 6573  = (2,)...def tes
-00009070: 745f 7772 6974 696e 675f 746f 5f61 6e5f  t_writing_to_an_
-00009080: 756e 6c69 6d69 7465 645f 6469 6d65 6e73  unlimited_dimens
-00009090: 696f 6e28 746d 705f 6c6f 6361 6c5f 6f72  ion(tmp_local_or
-000090a0: 5f72 656d 6f74 655f 6e65 7463 6466 293a  _remote_netcdf):
-000090b0: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-000090c0: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-000090d0: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
-000090e0: 6466 2c20 2277 2229 2061 7320 663a 0a20  df, "w") as f:. 
-000090f0: 2020 2020 2020 2023 2054 776f 2064 696d         # Two dim
-00009100: 656e 7369 6f6e 732c 206f 6e6c 7920 6f6e  ensions, only on
-00009110: 6520 6973 2075 6e6c 696d 6974 6564 2e0a  e is unlimited..
-00009120: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
-00009130: 696f 6e73 5b22 7822 5d20 3d20 4e6f 6e65  ions["x"] = None
-00009140: 0a20 2020 2020 2020 2066 2e64 696d 656e  .        f.dimen
-00009150: 7369 6f6e 735b 2279 225d 203d 2033 0a20  sions["y"] = 3. 
-00009160: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
-00009170: 6f6e 735b 227a 225d 203d 204e 6f6e 650a  ons["z"] = None.
-00009180: 0a20 2020 2020 2020 2023 2043 616e 6e6f  .        # Canno
-00009190: 7420 6372 6561 7465 2069 7420 7769 7468  t create it with
-000091a0: 6f75 7420 6669 7273 7420 7265 7369 7a69  out first resizi
-000091b0: 6e67 2069 742e 0a20 2020 2020 2020 2077  ng it..        w
-000091c0: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
-000091d0: 7328 5661 6c75 6545 7272 6f72 2920 6173  s(ValueError) as
-000091e0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-000091f0: 662e 6372 6561 7465 5f76 6172 6961 626c  f.create_variabl
-00009200: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00009210: 2020 2022 6475 6d6d 7931 222c 2064 6174     "dummy1", dat
-00009220: 613d 6e70 2e61 7272 6179 285b 5b31 2c20  a=np.array([[1, 
-00009230: 322c 2033 5d5d 292c 2064 696d 656e 7369  2, 3]]), dimensi
-00009240: 6f6e 733d 2822 7822 2c20 2279 2229 0a20  ons=("x", "y"). 
-00009250: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00009260: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00009270: 652e 7661 6c75 652e 6172 6773 5b30 5d20  e.value.args[0] 
-00009280: 3d3d 2022 5368 6170 6520 7475 706c 6520  == "Shape tuple 
-00009290: 6973 2069 6e63 6f6d 7061 7469 626c 6520  is incompatible 
-000092a0: 7769 7468 2064 6174 6122 0a0a 2020 2020  with data"..    
-000092b0: 2020 2020 2320 5769 7468 6f75 7420 6461      # Without da
-000092c0: 7461 2e0a 2020 2020 2020 2020 662e 6372  ta..        f.cr
-000092d0: 6561 7465 5f76 6172 6961 626c 6528 2264  eate_variable("d
-000092e0: 756d 6d79 3122 2c20 6469 6d65 6e73 696f  ummy1", dimensio
-000092f0: 6e73 3d28 2278 222c 2022 7922 292c 2064  ns=("x", "y"), d
-00009300: 7479 7065 3d6e 702e 696e 7436 3429 0a20  type=np.int64). 
-00009310: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
-00009320: 7661 7269 6162 6c65 2822 6475 6d6d 7932  variable("dummy2
-00009330: 222c 2064 696d 656e 7369 6f6e 733d 2822  ", dimensions=("
-00009340: 7822 2c20 2279 2229 2c20 6474 7970 653d  x", "y"), dtype=
-00009350: 6e70 2e69 6e74 3634 290a 2020 2020 2020  np.int64).      
-00009360: 2020 662e 6372 6561 7465 5f76 6172 6961    f.create_varia
-00009370: 626c 6528 2264 756d 6d79 3322 2c20 6469  ble("dummy3", di
-00009380: 6d65 6e73 696f 6e73 3d28 2278 222c 2022  mensions=("x", "
-00009390: 7922 292c 2064 7479 7065 3d6e 702e 696e  y"), dtype=np.in
-000093a0: 7436 3429 0a20 2020 2020 2020 2066 2e63  t64).        f.c
-000093b0: 7265 6174 655f 7661 7269 6162 6c65 2822  reate_variable("
-000093c0: 6475 6d6d 7958 222c 2064 696d 656e 7369  dummyX", dimensi
-000093d0: 6f6e 733d 2822 7822 2c20 2279 222c 2022  ons=("x", "y", "
-000093e0: 7a22 292c 2064 7479 7065 3d6e 702e 696e  z"), dtype=np.in
-000093f0: 7436 3429 0a20 2020 2020 2020 2067 203d  t64).        g =
-00009400: 2066 2e63 7265 6174 655f 6772 6f75 7028   f.create_group(
-00009410: 2274 6573 7422 290a 2020 2020 2020 2020  "test").        
-00009420: 672e 6372 6561 7465 5f76 6172 6961 626c  g.create_variabl
-00009430: 6528 2264 756d 6d79 3422 2c20 6469 6d65  e("dummy4", dime
-00009440: 6e73 696f 6e73 3d28 2279 222c 2022 7822  nsions=("y", "x"
-00009450: 2c20 2278 2229 2c20 6474 7970 653d 6e70  , "x"), dtype=np
-00009460: 2e69 6e74 3634 290a 2020 2020 2020 2020  .int64).        
-00009470: 672e 6372 6561 7465 5f76 6172 6961 626c  g.create_variabl
-00009480: 6528 2264 756d 6d79 3522 2c20 6469 6d65  e("dummy5", dime
-00009490: 6e73 696f 6e73 3d28 2279 222c 2022 7922  nsions=("y", "y"
-000094a0: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
-000094b0: 3429 0a0a 2020 2020 2020 2020 6173 7365  4)..        asse
-000094c0: 7274 2066 2e76 6172 6961 626c 6573 5b22  rt f.variables["
-000094d0: 6475 6d6d 7931 225d 2e73 6861 7065 203d  dummy1"].shape =
-000094e0: 3d20 2830 2c20 3329 0a20 2020 2020 2020  = (0, 3).       
-000094f0: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
-00009500: 6c65 735b 2264 756d 6d79 3222 5d2e 7368  les["dummy2"].sh
-00009510: 6170 6520 3d3d 2028 302c 2033 290a 2020  ape == (0, 3).  
-00009520: 2020 2020 2020 6173 7365 7274 2066 2e76        assert f.v
-00009530: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
-00009540: 225d 2e73 6861 7065 203d 3d20 2830 2c20  "].shape == (0, 
-00009550: 3329 0a20 2020 2020 2020 2061 7373 6572  3).        asser
-00009560: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
-00009570: 756d 6d79 5822 5d2e 7368 6170 6520 3d3d  ummyX"].shape ==
-00009580: 2028 302c 2033 2c20 3029 0a20 2020 2020   (0, 3, 0).     
-00009590: 2020 2061 7373 6572 7420 672e 7661 7269     assert g.vari
-000095a0: 6162 6c65 735b 2264 756d 6d79 3422 5d2e  ables["dummy4"].
-000095b0: 7368 6170 6520 3d3d 2028 332c 2030 2c20  shape == (3, 0, 
-000095c0: 3029 0a20 2020 2020 2020 2061 7373 6572  0).        asser
-000095d0: 7420 672e 7661 7269 6162 6c65 735b 2264  t g.variables["d
-000095e0: 756d 6d79 3522 5d2e 7368 6170 6520 3d3d  ummy5"].shape ==
-000095f0: 2028 332c 2033 290a 0a20 2020 2020 2020   (3, 3)..       
-00009600: 2023 2072 6573 697a 6520 6469 6d65 6e73   # resize dimens
-00009610: 696f 6e73 2061 6e64 2061 6c6c 2063 6f6e  ions and all con
-00009620: 6e65 6374 6564 2076 6172 6961 626c 6573  nected variables
-00009630: 0a20 2020 2020 2020 2066 2e72 6573 697a  .        f.resiz
-00009640: 655f 6469 6d65 6e73 696f 6e28 2278 222c  e_dimension("x",
-00009650: 2032 290a 2020 2020 2020 2020 6173 7365   2).        asse
-00009660: 7274 2066 2e76 6172 6961 626c 6573 5b22  rt f.variables["
-00009670: 6475 6d6d 7931 225d 2e73 6861 7065 203d  dummy1"].shape =
-00009680: 3d20 2832 2c20 3329 0a20 2020 2020 2020  = (2, 3).       
-00009690: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
-000096a0: 6c65 735b 2264 756d 6d79 3222 5d2e 7368  les["dummy2"].sh
-000096b0: 6170 6520 3d3d 2028 322c 2033 290a 2020  ape == (2, 3).  
-000096c0: 2020 2020 2020 6173 7365 7274 2066 2e76        assert f.v
-000096d0: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
-000096e0: 225d 2e73 6861 7065 203d 3d20 2832 2c20  "].shape == (2, 
-000096f0: 3329 0a20 2020 2020 2020 2061 7373 6572  3).        asser
-00009700: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
-00009710: 756d 6d79 5822 5d2e 7368 6170 6520 3d3d  ummyX"].shape ==
-00009720: 2028 322c 2033 2c20 3029 0a20 2020 2020   (2, 3, 0).     
-00009730: 2020 2061 7373 6572 7420 672e 7661 7269     assert g.vari
-00009740: 6162 6c65 735b 2264 756d 6d79 3422 5d2e  ables["dummy4"].
-00009750: 7368 6170 6520 3d3d 2028 332c 2032 2c20  shape == (3, 2, 
-00009760: 3229 0a20 2020 2020 2020 2061 7373 6572  2).        asser
-00009770: 7420 672e 7661 7269 6162 6c65 735b 2264  t g.variables["d
-00009780: 756d 6d79 3522 5d2e 7368 6170 6520 3d3d  ummy5"].shape ==
-00009790: 2028 332c 2033 290a 0a20 2020 2020 2020   (3, 3)..       
-000097a0: 2023 2062 726f 6164 6361 7374 2077 7269   # broadcast wri
-000097b0: 7469 6e67 0a20 2020 2020 2020 2066 2e76  ting.        f.v
-000097c0: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
-000097d0: 225d 5b2e 2e2e 5d20 3d20 5b5b 312c 2032  "][...] = [[1, 2
-000097e0: 2c20 335d 5d0a 2020 2020 2020 2020 6e70  , 3]].        np
-000097f0: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
-00009800: 616c 6c63 6c6f 7365 2866 2e76 6172 6961  allclose(f.varia
-00009810: 626c 6573 5b22 6475 6d6d 7933 225d 2c20  bles["dummy3"], 
-00009820: 5b5b 312c 2032 2c20 335d 2c20 5b31 2c20  [[1, 2, 3], [1, 
-00009830: 322c 2033 5d5d 290a 0a0a 6465 6620 7465  2, 3]])...def te
-00009840: 7374 5f63 5f61 7069 5f63 616e 5f72 6561  st_c_api_can_rea
-00009850: 645f 756e 6c69 6d69 7465 645f 6469 6d65  d_unlimited_dime
-00009860: 6e73 696f 6e73 2874 6d70 5f6c 6f63 616c  nsions(tmp_local
-00009870: 5f6e 6574 6364 6629 3a0a 2020 2020 7769  _netcdf):.    wi
-00009880: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-00009890: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
-000098a0: 662c 2022 7722 2920 6173 2066 3a0a 2020  f, "w") as f:.  
-000098b0: 2020 2020 2020 2320 5468 7265 6520 6469        # Three di
-000098c0: 6d65 6e73 696f 6e73 2c20 6f6e 6c79 206f  mensions, only o
-000098d0: 6e65 2069 7320 6c69 6d69 7465 642e 0a20  ne is limited.. 
-000098e0: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
-000098f0: 6f6e 735b 2278 225d 203d 204e 6f6e 650a  ons["x"] = None.
-00009900: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
-00009910: 696f 6e73 5b22 7922 5d20 3d20 330a 2020  ions["y"] = 3.  
-00009920: 2020 2020 2020 662e 6469 6d65 6e73 696f        f.dimensio
-00009930: 6e73 5b22 7a22 5d20 3d20 4e6f 6e65 0a20  ns["z"] = None. 
-00009940: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
-00009950: 7661 7269 6162 6c65 2822 6475 6d6d 7931  variable("dummy1
-00009960: 222c 2064 696d 656e 7369 6f6e 733d 2822  ", dimensions=("
-00009970: 7822 2c20 2279 2229 2c20 6474 7970 653d  x", "y"), dtype=
-00009980: 6e70 2e69 6e74 3634 290a 2020 2020 2020  np.int64).      
-00009990: 2020 662e 6372 6561 7465 5f76 6172 6961    f.create_varia
-000099a0: 626c 6528 2264 756d 6d79 3222 2c20 6469  ble("dummy2", di
-000099b0: 6d65 6e73 696f 6e73 3d28 2279 222c 2022  mensions=("y", "
-000099c0: 7822 2c20 2278 2229 2c20 6474 7970 653d  x", "x"), dtype=
-000099d0: 6e70 2e69 6e74 3634 290a 2020 2020 2020  np.int64).      
-000099e0: 2020 6720 3d20 662e 6372 6561 7465 5f67    g = f.create_g
-000099f0: 726f 7570 2822 7465 7374 2229 0a20 2020  roup("test").   
-00009a00: 2020 2020 2067 2e63 7265 6174 655f 7661       g.create_va
-00009a10: 7269 6162 6c65 2822 6475 6d6d 7933 222c  riable("dummy3",
-00009a20: 2064 696d 656e 7369 6f6e 733d 2822 7922   dimensions=("y"
-00009a30: 2c20 2279 2229 2c20 6474 7970 653d 6e70  , "y"), dtype=np
-00009a40: 2e69 6e74 3634 290a 2020 2020 2020 2020  .int64).        
-00009a50: 672e 6372 6561 7465 5f76 6172 6961 626c  g.create_variabl
-00009a60: 6528 2264 756d 6d79 3422 2c20 6469 6d65  e("dummy4", dime
-00009a70: 6e73 696f 6e73 3d28 227a 222c 2022 7a22  nsions=("z", "z"
-00009a80: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
-00009a90: 3429 0a20 2020 2020 2020 2066 2e72 6573  4).        f.res
-00009aa0: 697a 655f 6469 6d65 6e73 696f 6e28 2278  ize_dimension("x
-00009ab0: 222c 2032 290a 0a20 2020 2077 6974 6820  ", 2)..    with 
-00009ac0: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
-00009ad0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00009ae0: 2c20 2272 2229 2061 7320 663a 0a20 2020  , "r") as f:.   
-00009af0: 2020 2020 2061 7373 6572 7420 662e 6469       assert f.di
-00009b00: 6d65 6e73 696f 6e73 5b22 7822 5d2e 7369  mensions["x"].si
-00009b10: 7a65 203d 3d20 320a 2020 2020 2020 2020  ze == 2.        
-00009b20: 6173 7365 7274 2066 2e64 696d 656e 7369  assert f.dimensi
-00009b30: 6f6e 735b 2278 225d 2e69 7375 6e6c 696d  ons["x"].isunlim
-00009b40: 6974 6564 2829 2069 7320 5472 7565 0a20  ited() is True. 
-00009b50: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
-00009b60: 6469 6d65 6e73 696f 6e73 5b22 7922 5d2e  dimensions["y"].
-00009b70: 7369 7a65 203d 3d20 330a 2020 2020 2020  size == 3.      
-00009b80: 2020 6173 7365 7274 2066 2e64 696d 656e    assert f.dimen
-00009b90: 7369 6f6e 735b 2279 225d 2e69 7375 6e6c  sions["y"].isunl
-00009ba0: 696d 6974 6564 2829 2069 7320 4661 6c73  imited() is Fals
-00009bb0: 650a 2020 2020 2020 2020 6173 7365 7274  e.        assert
-00009bc0: 2066 2e64 696d 656e 7369 6f6e 735b 227a   f.dimensions["z
-00009bd0: 225d 2e73 697a 6520 3d3d 2030 0a20 2020  "].size == 0.   
-00009be0: 2020 2020 2061 7373 6572 7420 662e 6469       assert f.di
-00009bf0: 6d65 6e73 696f 6e73 5b22 7a22 5d2e 6973  mensions["z"].is
-00009c00: 756e 6c69 6d69 7465 6428 2920 6973 2054  unlimited() is T
-00009c10: 7275 650a 0a20 2020 2020 2020 2061 7373  rue..        ass
-00009c20: 6572 7420 662e 7661 7269 6162 6c65 735b  ert f.variables[
-00009c30: 2264 756d 6d79 3122 5d2e 7368 6170 6520  "dummy1"].shape 
-00009c40: 3d3d 2028 322c 2033 290a 2020 2020 2020  == (2, 3).      
-00009c50: 2020 6173 7365 7274 2066 2e76 6172 6961    assert f.varia
-00009c60: 626c 6573 5b22 6475 6d6d 7932 225d 2e73  bles["dummy2"].s
-00009c70: 6861 7065 203d 3d20 2833 2c20 322c 2032  hape == (3, 2, 2
-00009c80: 290a 2020 2020 2020 2020 6720 3d20 662e  ).        g = f.
-00009c90: 6772 6f75 7073 5b22 7465 7374 225d 0a20  groups["test"]. 
-00009ca0: 2020 2020 2020 2061 7373 6572 7420 672e         assert g.
-00009cb0: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
-00009cc0: 3322 5d2e 7368 6170 6520 3d3d 2028 332c  3"].shape == (3,
-00009cd0: 2033 290a 2020 2020 2020 2020 6173 7365   3).        asse
-00009ce0: 7274 2067 2e76 6172 6961 626c 6573 5b22  rt g.variables["
-00009cf0: 6475 6d6d 7934 225d 2e73 6861 7065 203d  dummy4"].shape =
-00009d00: 3d20 2830 2c20 3029 0a0a 0a64 6566 2074  = (0, 0)...def t
-00009d10: 6573 745f 7265 6164 696e 675f 756e 6c69  est_reading_unli
-00009d20: 6d69 7465 645f 6469 6d65 6e73 696f 6e73  mited_dimensions
-00009d30: 5f63 7265 6174 6564 5f77 6974 685f 635f  _created_with_c_
-00009d40: 6170 6928 746d 705f 6c6f 6361 6c5f 6e65  api(tmp_local_ne
-00009d50: 7463 6466 293a 0a20 2020 2077 6974 6820  tcdf):.    with 
-00009d60: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
-00009d70: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00009d80: 2c20 2277 2229 2061 7320 663a 0a20 2020  , "w") as f:.   
-00009d90: 2020 2020 2066 2e63 7265 6174 6544 696d       f.createDim
-00009da0: 656e 7369 6f6e 2822 7822 2c20 4e6f 6e65  ension("x", None
-00009db0: 290a 2020 2020 2020 2020 662e 6372 6561  ).        f.crea
-00009dc0: 7465 4469 6d65 6e73 696f 6e28 2279 222c  teDimension("y",
-00009dd0: 2033 290a 2020 2020 2020 2020 662e 6372   3).        f.cr
-00009de0: 6561 7465 4469 6d65 6e73 696f 6e28 227a  eateDimension("z
-00009df0: 222c 204e 6f6e 6529 0a0a 2020 2020 2020  ", None)..      
-00009e00: 2020 6475 6d6d 7931 203d 2066 2e63 7265    dummy1 = f.cre
-00009e10: 6174 6556 6172 6961 626c 6528 2264 756d  ateVariable("dum
-00009e20: 6d79 3122 2c20 666c 6f61 742c 2028 2278  my1", float, ("x
-00009e30: 222c 2022 7922 2929 0a20 2020 2020 2020  ", "y")).       
-00009e40: 2066 2e63 7265 6174 6556 6172 6961 626c   f.createVariabl
-00009e50: 6528 2264 756d 6d79 3222 2c20 666c 6f61  e("dummy2", floa
-00009e60: 742c 2028 2279 222c 2022 7822 2c20 2278  t, ("y", "x", "x
-00009e70: 2229 290a 2020 2020 2020 2020 6720 3d20  ")).        g = 
-00009e80: 662e 6372 6561 7465 4772 6f75 7028 2274  f.createGroup("t
-00009e90: 6573 7422 290a 2020 2020 2020 2020 672e  est").        g.
-00009ea0: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
-00009eb0: 6475 6d6d 7933 222c 2066 6c6f 6174 2c20  dummy3", float, 
-00009ec0: 2822 7922 2c20 2279 2229 290a 2020 2020  ("y", "y")).    
-00009ed0: 2020 2020 672e 6372 6561 7465 5661 7269      g.createVari
-00009ee0: 6162 6c65 2822 6475 6d6d 7934 222c 2066  able("dummy4", f
-00009ef0: 6c6f 6174 2c20 2822 7a22 2c20 227a 2229  loat, ("z", "z")
-00009f00: 290a 0a20 2020 2020 2020 2023 2041 7373  )..        # Ass
-00009f10: 6967 6e20 736f 6d65 7468 696e 6720 746f  ign something to
-00009f20: 2074 7269 6767 6572 2061 2072 6573 697a   trigger a resiz
-00009f30: 652e 0a20 2020 2020 2020 2064 756d 6d79  e..        dummy
-00009f40: 315b 3a5d 203d 205b 5b31 2c20 322c 2033  1[:] = [[1, 2, 3
-00009f50: 5d2c 205b 342c 2035 2c20 365d 5d0a 0a20  ], [4, 5, 6]].. 
-00009f60: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-00009f70: 616e 6f74 6865 7220 7661 7269 6162 6c65  another variable
-00009f80: 2077 6974 6820 7361 6d65 2064 696d 656e   with same dimen
-00009f90: 7369 6f6e 730a 2020 2020 2020 2020 662e  sions.        f.
-00009fa0: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
-00009fb0: 6475 6d6d 7935 222c 2066 6c6f 6174 2c20  dummy5", float, 
-00009fc0: 2822 7822 2c20 2279 2229 290a 0a20 2020  ("x", "y"))..   
-00009fd0: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
-00009fe0: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
-00009ff0: 7463 6466 2c20 2272 2229 2061 7320 663a  tcdf, "r") as f:
-0000a000: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000a010: 662e 6469 6d65 6e73 696f 6e73 5b22 7822  f.dimensions["x"
-0000a020: 5d2e 6973 756e 6c69 6d69 7465 6428 290a  ].isunlimited().
-0000a030: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
-0000a040: 2e64 696d 656e 7369 6f6e 735b 2279 225d  .dimensions["y"]
-0000a050: 2e73 697a 6520 3d3d 2033 0a20 2020 2020  .size == 3.     
-0000a060: 2020 2061 7373 6572 7420 662e 6469 6d65     assert f.dime
-0000a070: 6e73 696f 6e73 5b22 7a22 5d2e 6973 756e  nsions["z"].isun
-0000a080: 6c69 6d69 7465 6428 290a 0a20 2020 2020  limited()..     
-0000a090: 2020 2023 2054 6869 7320 6973 2070 6172     # This is par
-0000a0a0: 7365 6420 636f 7272 6563 746c 7920 6475  sed correctly du
-0000a0b0: 6520 746f 2068 356e 6574 6364 6627 7320  e to h5netcdf's 
-0000a0c0: 696e 6974 2074 7269 636b 6572 792e 0a20  init trickery.. 
-0000a0d0: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
-0000a0e0: 6469 6d65 6e73 696f 6e73 5b22 7822 5d2e  dimensions["x"].
-0000a0f0: 7369 7a65 203d 3d20 320a 2020 2020 2020  size == 2.      
-0000a100: 2020 6173 7365 7274 2066 2e64 696d 656e    assert f.dimen
-0000a110: 7369 6f6e 735b 2279 225d 2e73 697a 6520  sions["y"].size 
-0000a120: 3d3d 2033 0a20 2020 2020 2020 2061 7373  == 3.        ass
-0000a130: 6572 7420 662e 6469 6d65 6e73 696f 6e73  ert f.dimensions
-0000a140: 5b22 7a22 5d2e 7369 7a65 203d 3d20 300a  ["z"].size == 0.
-0000a150: 0a20 2020 2020 2020 2023 2042 7574 2074  .        # But t
-0000a160: 6865 2061 6374 7561 6c20 6461 7461 2d73  he actual data-s
-0000a170: 6574 2061 6e64 2061 7272 6179 7320 6172  et and arrays ar
-0000a180: 6520 6e6f 7420 636f 7272 6563 742e 0a20  e not correct.. 
-0000a190: 2020 2020 2020 2023 2061 7373 6572 7420         # assert 
-0000a1a0: 665b 2264 756d 6d79 3122 5d2e 7368 6170  f["dummy1"].shap
-0000a1b0: 6520 3d3d 2028 322c 2033 290a 2020 2020  e == (2, 3).    
-0000a1c0: 2020 2020 2320 5858 583a 2054 6869 7320      # XXX: This 
-0000a1d0: 6172 7261 7920 6861 7320 736f 6d65 2064  array has some d
-0000a1e0: 6174 6120 7769 7468 2064 696d 656e 7369  ata with dimensi
-0000a1f0: 6f6e 2078 202d 206e 6574 6364 6620 646f  on x - netcdf do
-0000a200: 6573 206e 6f74 0a20 2020 2020 2020 2023  es not.        #
-0000a210: 2061 7070 6561 7220 746f 206b 6565 7020   appear to keep 
-0000a220: 6469 6d65 6e73 696f 6e73 2063 6f6e 7369  dimensions consi
-0000a230: 7374 656e 742e 0a20 2020 2020 2020 2023  stent..        #
-0000a240: 2057 6974 6820 6874 7470 733a 2f2f 6769   With https://gi
-0000a250: 7468 7562 2e63 6f6d 2f68 356e 6574 6364  thub.com/h5netcd
-0000a260: 662f 6835 6e65 7463 6466 2f70 756c 6c2f  f/h5netcdf/pull/
-0000a270: 3130 3320 6835 6e65 7463 6466 2077 696c  103 h5netcdf wil
-0000a280: 6c0a 2020 2020 2020 2020 2320 7265 7475  l.        # retu
-0000a290: 726e 2061 2070 6164 6465 6420 6172 7261  rn a padded arra
-0000a2a0: 790a 2020 2020 2020 2020 6173 7365 7274  y.        assert
-0000a2b0: 2066 5b22 6475 6d6d 7932 225d 2e73 6861   f["dummy2"].sha
-0000a2c0: 7065 203d 3d20 2833 2c20 322c 2032 290a  pe == (3, 2, 2).
-0000a2d0: 2020 2020 2020 2020 662e 6772 6f75 7073          f.groups
-0000a2e0: 5b22 7465 7374 225d 5b22 6475 6d6d 7933  ["test"]["dummy3
-0000a2f0: 225d 2e73 6861 7065 203d 3d20 2833 2c20  "].shape == (3, 
-0000a300: 3329 0a20 2020 2020 2020 2066 2e67 726f  3).        f.gro
-0000a310: 7570 735b 2274 6573 7422 5d5b 2264 756d  ups["test"]["dum
-0000a320: 6d79 3422 5d2e 7368 6170 6520 3d3d 2028  my4"].shape == (
-0000a330: 302c 2030 290a 2020 2020 2020 2020 6173  0, 0).        as
-0000a340: 7365 7274 2066 5b22 6475 6d6d 7935 225d  sert f["dummy5"]
-0000a350: 2e73 6861 7065 203d 3d20 2832 2c20 3329  .shape == (2, 3)
-0000a360: 0a0a 0a64 6566 2074 6573 745f 7265 6164  ...def test_read
-0000a370: 696e 675f 756e 7573 6564 5f75 6e6c 696d  ing_unused_unlim
-0000a380: 6974 6564 5f64 696d 656e 7369 6f6e 2874  ited_dimension(t
-0000a390: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
-0000a3a0: 7465 5f6e 6574 6364 6629 3a0a 2020 2020  te_netcdf):.    
-0000a3b0: 2222 2254 6573 7420 7265 6164 696e 6720  """Test reading 
-0000a3c0: 6120 6669 6c65 2077 6974 6820 756e 7573  a file with unus
-0000a3d0: 6564 2064 696d 656e 7369 6f6e 206f 6620  ed dimension of 
-0000a3e0: 756e 6c69 6d69 7465 6420 7369 7a65 2222  unlimited size""
-0000a3f0: 220a 2020 2020 7769 7468 2068 356e 6574  ".    with h5net
-0000a400: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
-0000a410: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
-0000a420: 6364 662c 2022 7722 2920 6173 2066 3a0a  cdf, "w") as f:.
-0000a430: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
-0000a440: 696f 6e73 203d 207b 2278 223a 204e 6f6e  ions = {"x": Non
-0000a450: 657d 0a20 2020 2020 2020 2066 2e72 6573  e}.        f.res
-0000a460: 697a 655f 6469 6d65 6e73 696f 6e28 2278  ize_dimension("x
-0000a470: 222c 2035 290a 2020 2020 2020 2020 6173  ", 5).        as
-0000a480: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
-0000a490: 735b 2278 225d 2e69 7375 6e6c 696d 6974  s["x"].isunlimit
-0000a4a0: 6564 2829 0a20 2020 2020 2020 2061 7373  ed().        ass
-0000a4b0: 6572 7420 662e 6469 6d65 6e73 696f 6e73  ert f.dimensions
-0000a4c0: 5b22 7822 5d2e 7369 7a65 203d 3d20 350a  ["x"].size == 5.
-0000a4d0: 0a0a 6465 6620 7465 7374 5f72 6561 6469  ..def test_readi
-0000a4e0: 6e67 5f73 7065 6369 616c 5f64 6174 6174  ng_special_datat
-0000a4f0: 7970 655f 6372 6561 7465 645f 7769 7468  ype_created_with
-0000a500: 5f63 5f61 7069 2874 6d70 5f6c 6f63 616c  _c_api(tmp_local
-0000a510: 5f6e 6574 6364 6629 3a0a 2020 2020 2222  _netcdf):.    ""
-0000a520: 2254 6573 7420 7265 6164 696e 6720 6120  "Test reading a 
-0000a530: 6669 6c65 2077 6974 6820 756e 7375 7070  file with unsupp
-0000a540: 6f72 7465 6420 4461 7461 7479 7065 2222  orted Datatype""
-0000a550: 220a 2020 2020 7769 7468 206e 6574 4344  ".    with netCD
-0000a560: 4634 2e44 6174 6173 6574 2874 6d70 5f6c  F4.Dataset(tmp_l
-0000a570: 6f63 616c 5f6e 6574 6364 662c 2022 7722  ocal_netcdf, "w"
-0000a580: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-0000a590: 636f 6d70 6c65 7831 3238 203d 206e 702e  complex128 = np.
-0000a5a0: 6474 7970 6528 5b28 2272 6561 6c22 2c20  dtype([("real", 
-0000a5b0: 6e70 2e66 6c6f 6174 3634 292c 2028 2269  np.float64), ("i
-0000a5c0: 6d61 6722 2c20 6e70 2e66 6c6f 6174 3634  mag", np.float64
-0000a5d0: 295d 290a 2020 2020 2020 2020 662e 6372  )]).        f.cr
-0000a5e0: 6561 7465 436f 6d70 6f75 6e64 5479 7065  eateCompoundType
-0000a5f0: 2863 6f6d 706c 6578 3132 382c 2022 636f  (complex128, "co
-0000a600: 6d70 6c65 7831 3238 2229 0a20 2020 2077  mplex128").    w
-0000a610: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-0000a620: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-0000a630: 6466 2c20 2272 2229 2061 7320 663a 0a20  df, "r") as f:. 
-0000a640: 2020 2020 2020 2070 6173 730a 0a0a 6465         pass...de
-0000a650: 6620 7465 7374 5f6e 6334 5f6e 6f6e 5f63  f test_nc4_non_c
-0000a660: 6f6f 7264 2874 6d70 5f6c 6f63 616c 5f6e  oord(tmp_local_n
-0000a670: 6574 6364 6629 3a0a 2020 2020 2320 4865  etcdf):.    # He
-0000a680: 7265 2077 6520 6765 6e65 7261 7465 2061  re we generate a
-0000a690: 2066 6577 2076 6172 6961 626c 6573 2061   few variables a
-0000a6a0: 6e64 2063 6f6f 7264 696e 6174 6573 0a20  nd coordinates. 
-0000a6b0: 2020 2023 2054 6865 2064 6566 6175 6c74     # The default
-0000a6c0: 2073 686f 756c 6420 6265 2074 6f20 7472   should be to tr
-0000a6d0: 6163 6b20 7468 6520 6f72 6465 7220 6f66  ack the order of
-0000a6e0: 2063 7265 6174 696f 6e0a 2020 2020 2320   creation.    # 
-0000a6f0: 5468 7573 2c20 6f6e 2072 656f 7065 6e69  Thus, on reopeni
-0000a700: 6e67 2074 6865 2066 696c 652c 2074 6865  ng the file, the
-0000a710: 206f 7264 6572 2069 6e20 7768 6963 680a   order in which.
-0000a720: 2020 2020 2320 7468 6520 7661 7269 6162      # the variab
-0000a730: 6c65 7320 6172 6520 6c69 7374 6564 2073  les are listed s
-0000a740: 686f 756c 6420 6265 206d 6169 6e74 6169  hould be maintai
-0000a750: 6e65 640a 2020 2020 2320 7920 2020 2d2d  ned.    # y   --
-0000a760: 2020 2072 6566 6572 7320 746f 2074 6865     refers to the
-0000a770: 2063 6f6f 7264 696e 6174 6520 790a 2020   coordinate y.  
-0000a780: 2020 2320 5f6e 6334 5f6e 6f6e 5f63 6f6f    # _nc4_non_coo
-0000a790: 7264 5f79 2020 2d2d 2020 7265 6665 7273  rd_y  --  refers
-0000a7a0: 2074 6f20 7468 6520 6461 7461 2079 0a20   to the data y. 
-0000a7b0: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-0000a7c0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-0000a7d0: 6e65 7463 6466 2c20 2277 2229 2061 7320  netcdf, "w") as 
-0000a7e0: 663a 0a20 2020 2020 2020 2066 2e64 696d  f:.        f.dim
-0000a7f0: 656e 7369 6f6e 7320 3d20 7b22 7822 3a20  ensions = {"x": 
-0000a800: 4e6f 6e65 2c20 2279 223a 2032 7d0a 2020  None, "y": 2}.  
-0000a810: 2020 2020 2020 662e 6372 6561 7465 5f76        f.create_v
-0000a820: 6172 6961 626c 6528 2274 6573 7422 2c20  ariable("test", 
-0000a830: 6469 6d65 6e73 696f 6e73 3d28 2278 222c  dimensions=("x",
-0000a840: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
-0000a850: 3429 0a20 2020 2020 2020 2066 2e63 7265  4).        f.cre
-0000a860: 6174 655f 7661 7269 6162 6c65 2822 7922  ate_variable("y"
-0000a870: 2c20 6469 6d65 6e73 696f 6e73 3d28 2278  , dimensions=("x
-0000a880: 222c 292c 2064 7479 7065 3d6e 702e 696e  ",), dtype=np.in
-0000a890: 7436 3429 0a0a 2020 2020 7769 7468 2068  t64)..    with h
-0000a8a0: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-0000a8b0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-0000a8c0: 7222 2920 6173 2066 3a0a 2020 2020 2020  r") as f:.      
-0000a8d0: 2020 6173 7365 7274 206c 6973 7428 662e    assert list(f.
-0000a8e0: 6469 6d65 6e73 696f 6e73 2920 3d3d 205b  dimensions) == [
-0000a8f0: 2278 222c 2022 7922 5d0a 2020 2020 2020  "x", "y"].      
-0000a900: 2020 6173 7365 7274 2066 2e64 696d 656e    assert f.dimen
-0000a910: 7369 6f6e 735b 2278 225d 2e73 697a 6520  sions["x"].size 
-0000a920: 3d3d 2030 0a20 2020 2020 2020 2061 7373  == 0.        ass
-0000a930: 6572 7420 662e 6469 6d65 6e73 696f 6e73  ert f.dimensions
-0000a940: 5b22 7822 5d2e 6973 756e 6c69 6d69 7465  ["x"].isunlimite
-0000a950: 6428 290a 2020 2020 2020 2020 6173 7365  d().        asse
-0000a960: 7274 2066 2e64 696d 656e 7369 6f6e 735b  rt f.dimensions[
-0000a970: 2279 225d 2e73 697a 6520 3d3d 2032 0a20  "y"].size == 2. 
-0000a980: 2020 2020 2020 2069 6620 7665 7273 696f         if versio
-0000a990: 6e2e 7061 7273 6528 6835 7079 2e5f 5f76  n.parse(h5py.__v
-0000a9a0: 6572 7369 6f6e 5f5f 2920 3e3d 2076 6572  ersion__) >= ver
-0000a9b0: 7369 6f6e 2e70 6172 7365 2822 332e 372e  sion.parse("3.7.
-0000a9c0: 3022 293a 0a20 2020 2020 2020 2020 2020  0"):.           
-0000a9d0: 2061 7373 6572 7420 6c69 7374 2866 2e76   assert list(f.v
-0000a9e0: 6172 6961 626c 6573 2920 3d3d 205b 2274  ariables) == ["t
-0000a9f0: 6573 7422 2c20 2279 225d 0a20 2020 2020  est", "y"].     
-0000aa00: 2020 2020 2020 2061 7373 6572 7420 6c69         assert li
-0000aa10: 7374 2866 2e5f 6835 6772 6f75 702e 6b65  st(f._h5group.ke
-0000aa20: 7973 2829 2920 3d3d 205b 2278 222c 2022  ys()) == ["x", "
-0000aa30: 7922 2c20 2274 6573 7422 2c20 225f 6e63  y", "test", "_nc
-0000aa40: 345f 6e6f 6e5f 636f 6f72 645f 7922 5d0a  4_non_coord_y"].
-0000aa50: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-0000aa60: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-0000aa70: 6c5f 6e65 7463 6466 2c20 2277 2229 2061  l_netcdf, "w") a
-0000aa80: 7320 663a 0a20 2020 2020 2020 2066 2e64  s f:.        f.d
-0000aa90: 696d 656e 7369 6f6e 7320 3d20 7b22 7822  imensions = {"x"
-0000aaa0: 3a20 4e6f 6e65 2c20 2279 223a 2032 7d0a  : None, "y": 2}.
-0000aab0: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
-0000aac0: 5f76 6172 6961 626c 6528 2279 222c 2064  _variable("y", d
-0000aad0: 696d 656e 7369 6f6e 733d 2822 7822 2c29  imensions=("x",)
-0000aae0: 2c20 6474 7970 653d 6e70 2e69 6e74 3634  , dtype=np.int64
-0000aaf0: 290a 2020 2020 2020 2020 662e 6372 6561  ).        f.crea
-0000ab00: 7465 5f76 6172 6961 626c 6528 2274 6573  te_variable("tes
-0000ab10: 7422 2c20 6469 6d65 6e73 696f 6e73 3d28  t", dimensions=(
-0000ab20: 2278 222c 292c 2064 7479 7065 3d6e 702e  "x",), dtype=np.
-0000ab30: 696e 7436 3429 0a0a 2020 2020 7769 7468  int64)..    with
-0000ab40: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
-0000ab50: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-0000ab60: 2022 7222 2920 6173 2066 3a0a 2020 2020   "r") as f:.    
-0000ab70: 2020 2020 6173 7365 7274 206c 6973 7428      assert list(
-0000ab80: 662e 6469 6d65 6e73 696f 6e73 2920 3d3d  f.dimensions) ==
-0000ab90: 205b 2278 222c 2022 7922 5d0a 2020 2020   ["x", "y"].    
-0000aba0: 2020 2020 6173 7365 7274 2066 2e64 696d      assert f.dim
-0000abb0: 656e 7369 6f6e 735b 2278 225d 2e73 697a  ensions["x"].siz
-0000abc0: 6520 3d3d 2030 0a20 2020 2020 2020 2061  e == 0.        a
-0000abd0: 7373 6572 7420 662e 6469 6d65 6e73 696f  ssert f.dimensio
-0000abe0: 6e73 5b22 7822 5d2e 6973 756e 6c69 6d69  ns["x"].isunlimi
-0000abf0: 7465 6428 290a 2020 2020 2020 2020 6173  ted().        as
+00005580: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+00005590: 2020 2020 2020 7769 7468 2072 6169 7365        with raise
+000055a0: 7328 5661 6c75 6545 7272 6f72 293a 0a20  s(ValueError):. 
+000055b0: 2020 2020 2020 2020 2020 2064 735b 2262             ds["b
+000055c0: 6172 225d 2e76 6172 6961 626c 6573 5b22  ar"].variables["
+000055d0: 666f 6f31 225d 2e64 696d 656e 7369 6f6e  foo1"].dimension
+000055e0: 730a 0a20 2020 2077 6974 6820 7261 6973  s..    with rais
+000055f0: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00005600: 2020 2020 2020 2020 7769 7468 2068 356e          with h5n
+00005610: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+00005620: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+00005630: 6574 6364 662c 2022 7222 2c20 7068 6f6e  etcdf, "r", phon
+00005640: 795f 6469 6d73 3d22 7372 7422 2920 6173  y_dims="srt") as
+00005650: 2064 733a 0a20 2020 2020 2020 2020 2020   ds:.           
+00005660: 2070 6173 730a 0a0a 6465 6620 7465 7374   pass...def test
+00005670: 5f66 616b 655f 7068 6f6e 795f 6469 6d73  _fake_phony_dims
+00005680: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+00005690: 6d6f 7465 5f6e 6574 6364 6629 3a0a 2020  mote_netcdf):.  
+000056a0: 2020 2320 7465 7374 7320 7772 6974 696e    # tests writin
+000056b0: 6720 6f66 2064 696d 656e 7369 6f6e 2077  g of dimension w
+000056c0: 6974 6820 7068 6f6e 7920 6e61 6d69 6e67  ith phony naming
+000056d0: 2073 6368 656d 650a 2020 2020 2320 7365   scheme.    # se
+000056e0: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+000056f0: 2e63 6f6d 2f68 356e 6574 6364 662f 6835  .com/h5netcdf/h5
+00005700: 6e65 7463 6466 2f69 7373 7565 732f 3137  netcdf/issues/17
+00005710: 380a 2020 2020 7769 7468 2068 356e 6574  8.    with h5net
+00005720: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
+00005730: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
+00005740: 6364 662c 206d 6f64 653d 2277 2229 2061  cdf, mode="w") a
+00005750: 7320 6473 3a0a 2020 2020 2020 2020 6473  s ds:.        ds
+00005760: 2e64 696d 656e 7369 6f6e 735b 2270 686f  .dimensions["pho
+00005770: 6e79 5f64 696d 5f30 225d 203d 2033 0a0a  ny_dim_0"] = 3..
+00005780: 0a64 6566 2063 6865 636b 5f69 6e76 616c  .def check_inval
+00005790: 6964 5f6e 6574 6364 6634 5f6d 6978 6564  id_netcdf4_mixed
+000057a0: 2876 6172 2c20 6929 3a0a 2020 2020 7064  (var, i):.    pd
+000057b0: 696d 203d 2066 2270 686f 6e79 5f64 696d  im = f"phony_dim
+000057c0: 5f7b 697d 220a 2020 2020 6173 7365 7274  _{i}".    assert
+000057d0: 2076 6172 5b22 666f 6f31 225d 2e64 696d   var["foo1"].dim
+000057e0: 656e 7369 6f6e 735b 305d 203d 3d20 2279  ensions[0] == "y
+000057f0: 3122 0a20 2020 2061 7373 6572 7420 7661  1".    assert va
+00005800: 725b 2266 6f6f 3122 5d2e 6469 6d65 6e73  r["foo1"].dimens
+00005810: 696f 6e73 5b31 5d20 3d3d 2022 7a31 220a  ions[1] == "z1".
+00005820: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
+00005830: 666f 6f31 225d 2e64 696d 656e 7369 6f6e  foo1"].dimension
+00005840: 735b 325d 203d 3d20 7064 696d 0a20 2020  s[2] == pdim.   
+00005850: 2061 7373 6572 7420 7661 725b 2266 6f6f   assert var["foo
+00005860: 3222 5d2e 6469 6d65 6e73 696f 6e73 5b30  2"].dimensions[0
+00005870: 5d20 3d3d 2022 7831 220a 2020 2020 6173  ] == "x1".    as
+00005880: 7365 7274 2076 6172 5b22 666f 6f32 225d  sert var["foo2"]
+00005890: 2e64 696d 656e 7369 6f6e 735b 315d 203d  .dimensions[1] =
+000058a0: 3d20 2279 3122 0a20 2020 2061 7373 6572  = "y1".    asser
+000058b0: 7420 7661 725b 2266 6f6f 3222 5d2e 6469  t var["foo2"].di
+000058c0: 6d65 6e73 696f 6e73 5b32 5d20 3d3d 2022  mensions[2] == "
+000058d0: 7a31 220a 2020 2020 6173 7365 7274 2076  z1".    assert v
+000058e0: 6172 5b22 666f 6f33 225d 2e64 696d 656e  ar["foo3"].dimen
+000058f0: 7369 6f6e 735b 305d 203d 3d20 2279 3122  sions[0] == "y1"
+00005900: 0a20 2020 2061 7373 6572 7420 7661 725b  .    assert var[
+00005910: 2266 6f6f 3322 5d2e 6469 6d65 6e73 696f  "foo3"].dimensio
+00005920: 6e73 5b31 5d20 3d3d 2022 7a31 220a 2020  ns[1] == "z1".  
+00005930: 2020 6173 7365 7274 2076 6172 5b22 666f    assert var["fo
+00005940: 6f33 225d 2e64 696d 656e 7369 6f6e 735b  o3"].dimensions[
+00005950: 325d 203d 3d20 7064 696d 0a20 2020 2061  2] == pdim.    a
+00005960: 7373 6572 7420 7661 725b 2266 6f6f 3422  ssert var["foo4"
+00005970: 5d2e 6469 6d65 6e73 696f 6e73 5b30 5d20  ].dimensions[0] 
+00005980: 3d3d 2022 7831 220a 2020 2020 6173 7365  == "x1".    asse
+00005990: 7274 2076 6172 5b22 666f 6f34 225d 2e64  rt var["foo4"].d
+000059a0: 696d 656e 7369 6f6e 735b 315d 203d 3d20  imensions[1] == 
+000059b0: 2279 3122 0a20 2020 2061 7373 6572 7420  "y1".    assert 
+000059c0: 7661 725b 2266 6f6f 3422 5d2e 6469 6d65  var["foo4"].dime
+000059d0: 6e73 696f 6e73 5b32 5d20 3d3d 2022 7a31  nsions[2] == "z1
+000059e0: 220a 2020 2020 6173 7365 7274 2076 6172  ".    assert var
+000059f0: 5b22 7822 5d2e 6469 6d65 6e73 696f 6e73  ["x"].dimensions
+00005a00: 5b30 5d20 3d3d 2022 7931 220a 2020 2020  [0] == "y1".    
+00005a10: 6173 7365 7274 2076 6172 5b22 7922 5d2e  assert var["y"].
+00005a20: 6469 6d65 6e73 696f 6e73 5b30 5d20 3d3d  dimensions[0] ==
+00005a30: 2022 7931 220a 2020 2020 6173 7365 7274   "y1".    assert
+00005a40: 2076 6172 5b22 7a22 5d2e 6469 6d65 6e73   var["z"].dimens
+00005a50: 696f 6e73 5b30 5d20 3d3d 2022 7931 220a  ions[0] == "y1".
+00005a60: 2020 2020 6173 7365 7274 2076 6172 5b22      assert var["
+00005a70: 7831 225d 2e64 696d 656e 7369 6f6e 735b  x1"].dimensions[
+00005a80: 305d 203d 3d20 2278 3122 0a20 2020 2061  0] == "x1".    a
+00005a90: 7373 6572 7420 7661 725b 2279 3122 5d2e  ssert var["y1"].
+00005aa0: 6469 6d65 6e73 696f 6e73 5b30 5d20 3d3d  dimensions[0] ==
+00005ab0: 2022 7931 220a 2020 2020 6173 7365 7274   "y1".    assert
+00005ac0: 2076 6172 5b22 7a31 225d 2e64 696d 656e   var["z1"].dimen
+00005ad0: 7369 6f6e 735b 305d 203d 3d20 227a 3122  sions[0] == "z1"
+00005ae0: 0a0a 0a64 6566 2074 6573 745f 696e 7661  ...def test_inva
+00005af0: 6c69 645f 6e65 7463 6466 345f 6d69 7865  lid_netcdf4_mixe
+00005b00: 6428 746d 705f 6c6f 6361 6c5f 6f72 5f72  d(tmp_local_or_r
+00005b10: 656d 6f74 655f 6e65 7463 6466 293a 0a20  emote_netcdf):. 
+00005b20: 2020 2069 6620 746d 705f 6c6f 6361 6c5f     if tmp_local_
+00005b30: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+00005b40: 2e73 7461 7274 7377 6974 6828 7265 6d6f  .startswith(remo
+00005b50: 7465 5f68 3529 3a0a 2020 2020 2020 2020  te_h5):.        
+00005b60: 7079 7465 7374 2e73 6b69 7028 226e 6574  pytest.skip("net
+00005b70: 4344 4634 2070 6163 6b61 6765 2064 6f65  CDF4 package doe
+00005b80: 7320 6e6f 7420 776f 726b 2077 6974 6820  s not work with 
+00005b90: 7265 6d6f 7465 2048 4446 3520 6669 6c65  remote HDF5 file
+00005ba0: 7322 290a 2020 2020 6835 203d 2067 6574  s").    h5 = get
+00005bb0: 5f68 6466 355f 6d6f 6475 6c65 2874 6d70  _hdf5_module(tmp
+00005bc0: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
+00005bd0: 5f6e 6574 6364 6629 0a20 2020 2077 6974  _netcdf).    wit
+00005be0: 6820 6835 2e46 696c 6528 746d 705f 6c6f  h h5.File(tmp_lo
+00005bf0: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00005c00: 7463 6466 2c20 2277 2229 2061 7320 663a  tcdf, "w") as f:
+00005c10: 0a20 2020 2020 2020 2076 6172 2c20 7661  .        var, va
+00005c20: 7232 203d 2063 7265 6174 655f 696e 7661  r2 = create_inva
+00005c30: 6c69 645f 6e65 7463 6466 5f64 6174 6128  lid_netcdf_data(
+00005c40: 290a 2020 2020 2020 2020 666f 7220 6b2c  ).        for k,
+00005c50: 2076 2069 6e20 7661 722e 6974 656d 7328   v in var.items(
+00005c60: 293a 0a20 2020 2020 2020 2020 2020 2066  ):.            f
+00005c70: 2e63 7265 6174 655f 6461 7461 7365 7428  .create_dataset(
+00005c80: 6b2c 2064 6174 613d 7629 0a20 2020 2020  k, data=v).     
+00005c90: 2020 2066 6f72 206b 2c20 7620 696e 2076     for k, v in v
+00005ca0: 6172 322e 6974 656d 7328 293a 0a20 2020  ar2.items():.   
+00005cb0: 2020 2020 2020 2020 2066 2e63 7265 6174           f.creat
+00005cc0: 655f 6461 7461 7365 7428 6b2c 2064 6174  e_dataset(k, dat
+00005cd0: 613d 6e70 2e61 7261 6e67 6528 7629 290a  a=np.arange(v)).
+00005ce0: 0a20 2020 2020 2020 2066 5b22 7831 225d  .        f["x1"]
+00005cf0: 2e6d 616b 655f 7363 616c 6528 290a 2020  .make_scale().  
+00005d00: 2020 2020 2020 665b 2279 3122 5d2e 6d61        f["y1"].ma
+00005d10: 6b65 5f73 6361 6c65 2829 0a20 2020 2020  ke_scale().     
+00005d20: 2020 2066 5b22 7a31 225d 2e6d 616b 655f     f["z1"].make_
+00005d30: 7363 616c 6528 290a 2020 2020 2020 2020  scale().        
+00005d40: 665b 2266 6f6f 3222 5d2e 6469 6d73 5b30  f["foo2"].dims[0
+00005d50: 5d2e 6174 7461 6368 5f73 6361 6c65 2866  ].attach_scale(f
+00005d60: 5b22 7831 225d 290a 2020 2020 2020 2020  ["x1"]).        
+00005d70: 665b 2266 6f6f 3222 5d2e 6469 6d73 5b31  f["foo2"].dims[1
+00005d80: 5d2e 6174 7461 6368 5f73 6361 6c65 2866  ].attach_scale(f
+00005d90: 5b22 7931 225d 290a 2020 2020 2020 2020  ["y1"]).        
+00005da0: 665b 2266 6f6f 3222 5d2e 6469 6d73 5b32  f["foo2"].dims[2
+00005db0: 5d2e 6174 7461 6368 5f73 6361 6c65 2866  ].attach_scale(f
+00005dc0: 5b22 7a31 225d 290a 0a20 2020 2077 6974  ["z1"])..    wit
+00005dd0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+00005de0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
+00005df0: 6f74 655f 6e65 7463 6466 2c20 2272 222c  ote_netcdf, "r",
+00005e00: 2070 686f 6e79 5f64 696d 733d 2273 6f72   phony_dims="sor
+00005e10: 7422 2920 6173 2064 733a 0a20 2020 2020  t") as ds:.     
+00005e20: 2020 2076 6172 203d 2064 732e 7661 7269     var = ds.vari
+00005e30: 6162 6c65 730a 2020 2020 2020 2020 6368  ables.        ch
+00005e40: 6563 6b5f 696e 7661 6c69 645f 6e65 7463  eck_invalid_netc
+00005e50: 6466 345f 6d69 7865 6428 7661 722c 2033  df4_mixed(var, 3
+00005e60: 290a 0a20 2020 2077 6974 6820 6835 6e65  )..    with h5ne
+00005e70: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+00005e80: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00005e90: 7463 6466 2c20 2272 222c 2070 686f 6e79  tcdf, "r", phony
+00005ea0: 5f64 696d 733d 2261 6363 6573 7322 2920  _dims="access") 
+00005eb0: 6173 2064 733a 0a20 2020 2020 2020 2076  as ds:.        v
+00005ec0: 6172 203d 2064 732e 7661 7269 6162 6c65  ar = ds.variable
+00005ed0: 730a 2020 2020 2020 2020 6368 6563 6b5f  s.        check_
+00005ee0: 696e 7661 6c69 645f 6e65 7463 6466 345f  invalid_netcdf4_
+00005ef0: 6d69 7865 6428 7661 722c 2030 290a 0a20  mixed(var, 0).. 
+00005f00: 2020 2069 6620 6e6f 7420 746d 705f 6c6f     if not tmp_lo
+00005f10: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00005f20: 7463 6466 2e73 7461 7274 7377 6974 6828  tcdf.startswith(
+00005f30: 7265 6d6f 7465 5f68 3529 3a0a 2020 2020  remote_h5):.    
+00005f40: 2020 2020 2320 6e65 7463 6466 3420 7061      # netcdf4 pa
+00005f50: 636b 6167 6520 646f 6573 206e 6f74 2077  ckage does not w
+00005f60: 6f72 6b20 7769 7468 2072 656d 6f74 6520  ork with remote 
+00005f70: 4844 4635 2066 696c 6573 0a20 2020 2020  HDF5 files.     
+00005f80: 2020 2077 6974 6820 6e65 7443 4446 342e     with netCDF4.
+00005f90: 4461 7461 7365 7428 746d 705f 6c6f 6361  Dataset(tmp_loca
+00005fa0: 6c5f 6f72 5f72 656d 6f74 655f 6e65 7463  l_or_remote_netc
+00005fb0: 6466 2c20 2272 2229 2061 7320 6473 3a0a  df, "r") as ds:.
+00005fc0: 2020 2020 2020 2020 2020 2020 7661 7220              var 
+00005fd0: 3d20 6473 2e76 6172 6961 626c 6573 0a20  = ds.variables. 
+00005fe0: 2020 2020 2020 2020 2020 2063 6865 636b             check
+00005ff0: 5f69 6e76 616c 6964 5f6e 6574 6364 6634  _invalid_netcdf4
+00006000: 5f6d 6978 6564 2876 6172 2c20 3329 0a0a  _mixed(var, 3)..
+00006010: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
+00006020: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
+00006030: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
+00006040: 662c 2022 7222 2920 6173 2064 733a 0a20  f, "r") as ds:. 
+00006050: 2020 2020 2020 2077 6974 6820 7261 6973         with rais
+00006060: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00006070: 2020 2020 2020 2020 2020 2020 6473 2e76              ds.v
+00006080: 6172 6961 626c 6573 5b22 666f 6f31 225d  ariables["foo1"]
+00006090: 2e64 696d 656e 7369 6f6e 730a 0a0a 6465  .dimensions...de
+000060a0: 6620 7465 7374 5f69 6e76 616c 6964 5f6e  f test_invalid_n
+000060b0: 6574 6364 665f 6d61 6c66 6f72 6d65 645f  etcdf_malformed_
+000060c0: 6469 6d65 6e73 696f 6e5f 7363 616c 6573  dimension_scales
+000060d0: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+000060e0: 6d6f 7465 5f6e 6574 6364 6629 3a0a 2020  mote_netcdf):.  
+000060f0: 2020 6835 203d 2067 6574 5f68 6466 355f    h5 = get_hdf5_
+00006100: 6d6f 6475 6c65 2874 6d70 5f6c 6f63 616c  module(tmp_local
+00006110: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
+00006120: 6629 0a20 2020 2077 6974 6820 6835 2e46  f).    with h5.F
+00006130: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
+00006140: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
+00006150: 2277 2229 2061 7320 663a 0a20 2020 2020  "w") as f:.     
+00006160: 2020 2066 6f6f 5f64 6174 6120 3d20 6e70     foo_data = np
+00006170: 2e61 7261 6e67 6528 3132 3529 2e72 6573  .arange(125).res
+00006180: 6861 7065 2835 2c20 352c 2035 290a 2020  hape(5, 5, 5).  
+00006190: 2020 2020 2020 662e 6372 6561 7465 5f64        f.create_d
+000061a0: 6174 6173 6574 2822 666f 6f31 222c 2064  ataset("foo1", d
+000061b0: 6174 613d 666f 6f5f 6461 7461 290a 2020  ata=foo_data).  
+000061c0: 2020 2020 2020 662e 6372 6561 7465 5f64        f.create_d
+000061d0: 6174 6173 6574 2822 7822 2c20 6461 7461  ataset("x", data
+000061e0: 3d6e 702e 6172 616e 6765 2835 2929 0a20  =np.arange(5)). 
+000061f0: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
+00006200: 6461 7461 7365 7428 2279 222c 2064 6174  dataset("y", dat
+00006210: 613d 6e70 2e61 7261 6e67 6528 3529 290a  a=np.arange(5)).
+00006220: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
+00006230: 5f64 6174 6173 6574 2822 7a22 2c20 6461  _dataset("z", da
+00006240: 7461 3d6e 702e 6172 616e 6765 2835 2929  ta=np.arange(5))
+00006250: 0a0a 2020 2020 2020 2020 665b 2278 225d  ..        f["x"]
+00006260: 2e6d 616b 655f 7363 616c 6528 290a 2020  .make_scale().  
+00006270: 2020 2020 2020 665b 2279 225d 2e6d 616b        f["y"].mak
+00006280: 655f 7363 616c 6528 290a 2020 2020 2020  e_scale().      
+00006290: 2020 665b 227a 225d 2e6d 616b 655f 7363    f["z"].make_sc
+000062a0: 616c 6528 290a 2020 2020 2020 2020 665b  ale().        f[
+000062b0: 2266 6f6f 3122 5d2e 6469 6d73 5b30 5d2e  "foo1"].dims[0].
+000062c0: 6174 7461 6368 5f73 6361 6c65 2866 5b22  attach_scale(f["
+000062d0: 7822 5d29 0a0a 2020 2020 7769 7468 2072  x"])..    with r
+000062e0: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
+000062f0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+00006300: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
+00006310: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+00006320: 655f 6e65 7463 6466 2c20 2272 2229 2061  e_netcdf, "r") a
+00006330: 7320 6473 3a0a 2020 2020 2020 2020 2020  s ds:.          
+00006340: 2020 6173 7365 7274 2064 730a 2020 2020    assert ds.    
+00006350: 2020 2020 2020 2020 7072 696e 7428 6473          print(ds
+00006360: 290a 0a20 2020 2077 6974 6820 7261 6973  )..    with rais
+00006370: 6573 2856 616c 7565 4572 726f 7229 3a0a  es(ValueError):.
+00006380: 2020 2020 2020 2020 7769 7468 2068 356e          with h5n
+00006390: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+000063a0: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+000063b0: 6574 6364 662c 2022 7222 2c20 7068 6f6e  etcdf, "r", phon
+000063c0: 795f 6469 6d73 3d22 736f 7274 2229 2061  y_dims="sort") a
+000063d0: 7320 6473 3a0a 2020 2020 2020 2020 2020  s ds:.          
+000063e0: 2020 6173 7365 7274 2064 730a 2020 2020    assert ds.    
+000063f0: 2020 2020 2020 2020 7072 696e 7428 6473          print(ds
+00006400: 290a 0a0a 6465 6620 7465 7374 5f68 6965  )...def test_hie
+00006410: 7261 7263 6869 6361 6c5f 6163 6365 7373  rarchical_access
+00006420: 5f61 7574 6f5f 6372 6561 7465 2874 6d70  _auto_create(tmp
+00006430: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
+00006440: 5f6e 6574 6364 6629 3a0a 2020 2020 6473  _netcdf):.    ds
+00006450: 203d 2068 356e 6574 6364 662e 4669 6c65   = h5netcdf.File
+00006460: 2874 6d70 5f6c 6f63 616c 5f6f 725f 7265  (tmp_local_or_re
+00006470: 6d6f 7465 5f6e 6574 6364 662c 2022 7722  mote_netcdf, "w"
+00006480: 290a 2020 2020 6473 2e63 7265 6174 655f  ).    ds.create_
+00006490: 7661 7269 6162 6c65 2822 2f66 6f6f 2f62  variable("/foo/b
+000064a0: 6172 222c 2064 6174 613d 3129 0a20 2020  ar", data=1).   
+000064b0: 2067 203d 2064 732e 6372 6561 7465 5f67   g = ds.create_g
+000064c0: 726f 7570 2822 666f 6f2f 6261 7a22 290a  roup("foo/baz").
+000064d0: 2020 2020 672e 6372 6561 7465 5f76 6172      g.create_var
+000064e0: 6961 626c 6528 222f 666f 6f2f 6865 6c6c  iable("/foo/hell
+000064f0: 6f22 2c20 6461 7461 3d32 290a 2020 2020  o", data=2).    
+00006500: 6173 7365 7274 2073 6574 2864 7329 203d  assert set(ds) =
+00006510: 3d20 7365 7428 5b22 666f 6f22 5d29 0a20  = set(["foo"]). 
+00006520: 2020 2061 7373 6572 7420 7365 7428 6473     assert set(ds
+00006530: 5b22 666f 6f22 5d29 203d 3d20 7365 7428  ["foo"]) == set(
+00006540: 5b22 6261 7222 2c20 2262 617a 222c 2022  ["bar", "baz", "
+00006550: 6865 6c6c 6f22 5d29 0a20 2020 2064 732e  hello"]).    ds.
+00006560: 636c 6f73 6528 290a 0a20 2020 2064 7320  close()..    ds 
+00006570: 3d20 6835 6e65 7463 6466 2e46 696c 6528  = h5netcdf.File(
+00006580: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
+00006590: 6f74 655f 6e65 7463 6466 2c20 2272 2229  ote_netcdf, "r")
+000065a0: 0a20 2020 2061 7373 6572 7420 7365 7428  .    assert set(
+000065b0: 6473 2920 3d3d 2073 6574 285b 2266 6f6f  ds) == set(["foo
+000065c0: 225d 290a 2020 2020 6173 7365 7274 2073  "]).    assert s
+000065d0: 6574 2864 735b 2266 6f6f 225d 2920 3d3d  et(ds["foo"]) ==
+000065e0: 2073 6574 285b 2262 6172 222c 2022 6261   set(["bar", "ba
+000065f0: 7a22 2c20 2268 656c 6c6f 225d 290a 2020  z", "hello"]).  
+00006600: 2020 6473 2e63 6c6f 7365 2829 0a0a 0a64    ds.close()...d
+00006610: 6566 2074 6573 745f 4e65 7463 6466 3444  ef test_Netcdf4D
+00006620: 696d 6964 2874 6d70 5f6c 6f63 616c 5f6e  imid(tmp_local_n
+00006630: 6574 6364 6629 3a0a 2020 2020 2320 7265  etcdf):.    # re
+00006640: 6772 6573 7369 6f6e 2074 6573 7420 666f  gression test fo
+00006650: 7220 6874 7470 733a 2f2f 6769 7468 7562  r https://github
+00006660: 2e63 6f6d 2f68 356e 6574 6364 662f 6835  .com/h5netcdf/h5
+00006670: 6e65 7463 6466 2f69 7373 7565 732f 3533  netcdf/issues/53
+00006680: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
+00006690: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
+000066a0: 6c5f 6e65 7463 6466 2c20 2277 2229 2061  l_netcdf, "w") a
+000066b0: 7320 663a 0a20 2020 2020 2020 2066 2e64  s f:.        f.d
+000066c0: 696d 656e 7369 6f6e 735b 2278 225d 203d  imensions["x"] =
+000066d0: 2031 0a20 2020 2020 2020 2067 203d 2066   1.        g = f
+000066e0: 2e63 7265 6174 655f 6772 6f75 7028 2266  .create_group("f
+000066f0: 6f6f 2229 0a20 2020 2020 2020 2067 2e64  oo").        g.d
+00006700: 696d 656e 7369 6f6e 735b 2278 225d 203d  imensions["x"] =
+00006710: 2032 0a20 2020 2020 2020 2067 2e64 696d   2.        g.dim
+00006720: 656e 7369 6f6e 735b 2279 225d 203d 2033  ensions["y"] = 3
+00006730: 0a0a 2020 2020 7769 7468 2068 3570 792e  ..    with h5py.
+00006740: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
+00006750: 6574 6364 662c 2022 7222 2920 6173 2066  etcdf, "r") as f
+00006760: 3a0a 2020 2020 2020 2020 2320 616c 6c20  :.        # all 
+00006770: 6469 6d65 6e73 696f 6e20 4944 7320 7368  dimension IDs sh
+00006780: 6f75 6c64 2062 6520 7072 6573 656e 7420  ould be present 
+00006790: 6578 6163 746c 7920 6f6e 6365 0a20 2020  exactly once.   
+000067a0: 2020 2020 2064 696d 5f69 6473 203d 207b       dim_ids = {
+000067b0: 665b 6e61 6d65 5d2e 6174 7472 735b 225f  f[name].attrs["_
+000067c0: 4e65 7463 6466 3444 696d 6964 225d 2066  Netcdf4Dimid"] f
+000067d0: 6f72 206e 616d 6520 696e 205b 2278 222c  or name in ["x",
+000067e0: 2022 666f 6f2f 7822 2c20 2266 6f6f 2f79   "foo/x", "foo/y
+000067f0: 225d 7d0a 2020 2020 2020 2020 6173 7365  "]}.        asse
+00006800: 7274 2064 696d 5f69 6473 203d 3d20 7b30  rt dim_ids == {0
+00006810: 2c20 312c 2032 7d0a 0a0a 6465 6620 7465  , 1, 2}...def te
+00006820: 7374 5f72 6561 6469 6e67 5f73 7472 5f61  st_reading_str_a
+00006830: 7272 6179 5f66 726f 6d5f 6e65 7443 4446  rray_from_netCDF
+00006840: 3428 746d 705f 6c6f 6361 6c5f 6e65 7463  4(tmp_local_netc
+00006850: 6466 2c20 6465 636f 6465 5f76 6c65 6e5f  df, decode_vlen_
+00006860: 7374 7269 6e67 7329 3a0a 2020 2020 2320  strings):.    # 
+00006870: 5468 6973 2074 6573 7473 2072 6561 6469  This tests readi
+00006880: 6e67 2073 7472 696e 6720 7661 7269 6162  ng string variab
+00006890: 6c65 7320 6372 6561 7465 6420 6279 206e  les created by n
+000068a0: 6574 4344 4634 0a20 2020 2077 6974 6820  etCDF4.    with 
+000068b0: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
+000068c0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+000068d0: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
+000068e0: 2020 2020 2020 6473 2e63 7265 6174 6544        ds.createD
+000068f0: 696d 656e 7369 6f6e 2822 666f 6f31 222c  imension("foo1",
+00006900: 205f 7374 7269 6e67 5f61 7272 6179 2e73   _string_array.s
+00006910: 6861 7065 5b30 5d29 0a20 2020 2020 2020  hape[0]).       
+00006920: 2064 732e 6372 6561 7465 4469 6d65 6e73   ds.createDimens
+00006930: 696f 6e28 2266 6f6f 3222 2c20 5f73 7472  ion("foo2", _str
+00006940: 696e 675f 6172 7261 792e 7368 6170 655b  ing_array.shape[
+00006950: 315d 290a 2020 2020 2020 2020 6473 2e63  1]).        ds.c
+00006960: 7265 6174 6556 6172 6961 626c 6528 2262  reateVariable("b
+00006970: 6172 222c 2073 7472 2c20 2822 666f 6f31  ar", str, ("foo1
+00006980: 222c 2022 666f 6f32 2229 290a 2020 2020  ", "foo2")).    
+00006990: 2020 2020 6473 2e76 6172 6961 626c 6573      ds.variables
+000069a0: 5b22 6261 7222 5d5b 3a5d 203d 205f 7374  ["bar"][:] = _st
+000069b0: 7269 6e67 5f61 7272 6179 0a0a 2020 2020  ring_array..    
+000069c0: 6473 203d 2068 356e 6574 6364 662e 4669  ds = h5netcdf.Fi
+000069d0: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+000069e0: 6364 662c 2022 7222 2c20 2a2a 6465 636f  cdf, "r", **deco
+000069f0: 6465 5f76 6c65 6e5f 7374 7269 6e67 7329  de_vlen_strings)
+00006a00: 0a0a 2020 2020 7620 3d20 6473 2e76 6172  ..    v = ds.var
+00006a10: 6961 626c 6573 5b22 6261 7222 5d0a 2020  iables["bar"].  
+00006a20: 2020 6966 2067 6574 6174 7472 2864 732c    if getattr(ds,
+00006a30: 2022 6465 636f 6465 5f76 6c65 6e5f 7374   "decode_vlen_st
+00006a40: 7269 6e67 7322 2c20 5472 7565 293a 0a20  rings", True):. 
+00006a50: 2020 2020 2020 2061 7373 6572 7420 6172         assert ar
+00006a60: 7261 795f 6571 7561 6c28 762c 205f 7374  ray_equal(v, _st
+00006a70: 7269 6e67 5f61 7272 6179 290a 2020 2020  ring_array).    
+00006a80: 656c 7365 3a0a 2020 2020 2020 2020 6173  else:.        as
+00006a90: 7365 7274 2061 7272 6179 5f65 7175 616c  sert array_equal
+00006aa0: 2876 2c20 6e70 2e63 6861 722e 656e 636f  (v, np.char.enco
+00006ab0: 6465 285f 7374 7269 6e67 5f61 7272 6179  de(_string_array
+00006ac0: 2929 0a0a 2020 2020 6473 2e63 6c6f 7365  ))..    ds.close
+00006ad0: 2829 0a0a 0a64 6566 2074 6573 745f 6e63  ()...def test_nc
+00006ae0: 5f70 726f 7065 7274 6965 735f 6e65 7728  _properties_new(
+00006af0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
+00006b00: 6f74 655f 6e65 7463 6466 293a 0a20 2020  ote_netcdf):.   
+00006b10: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+00006b20: 696c 6528 746d 705f 6c6f 6361 6c5f 6f72  ile(tmp_local_or
+00006b30: 5f72 656d 6f74 655f 6e65 7463 6466 2c20  _remote_netcdf, 
+00006b40: 2277 2229 3a0a 2020 2020 2020 2020 7061  "w"):.        pa
+00006b50: 7373 0a20 2020 2068 3520 3d20 6765 745f  ss.    h5 = get_
+00006b60: 6864 6635 5f6d 6f64 756c 6528 746d 705f  hdf5_module(tmp_
+00006b70: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
+00006b80: 6e65 7463 6466 290a 2020 2020 7769 7468  netcdf).    with
+00006b90: 2068 352e 4669 6c65 2874 6d70 5f6c 6f63   h5.File(tmp_loc
+00006ba0: 616c 5f6f 725f 7265 6d6f 7465 5f6e 6574  al_or_remote_net
+00006bb0: 6364 662c 2022 7222 2920 6173 2066 3a0a  cdf, "r") as f:.
+00006bc0: 2020 2020 2020 2020 6173 7365 7274 2062          assert b
+00006bd0: 2268 356e 6574 6364 6622 2069 6e20 662e  "h5netcdf" in f.
+00006be0: 6174 7472 735b 225f 4e43 5072 6f70 6572  attrs["_NCProper
+00006bf0: 7469 6573 225d 0a0a 0a64 6566 2074 6573  ties"]...def tes
+00006c00: 745f 6661 696c 6564 5f72 6561 645f 6f70  t_failed_read_op
+00006c10: 656e 5f61 6e64 5f63 6c65 616e 5f64 656c  en_and_clean_del
+00006c20: 6574 6528 746d 7064 6972 293a 0a20 2020  ete(tmpdir):.   
+00006c30: 2023 2041 2066 696c 6520 7468 6174 2064   # A file that d
+00006c40: 6f65 7320 6e6f 7420 6578 6973 7420 6275  oes not exist bu
+00006c50: 7420 6973 206f 7065 6e65 6420 666f 720a  t is opened for.
+00006c60: 2020 2020 2320 7265 6164 696e 6720 7368      # reading sh
+00006c70: 6f75 6c64 206f 6e6c 7920 7261 6973 6520  ould only raise 
+00006c80: 616e 2049 4f45 7272 6f72 2061 6e64 0a20  an IOError and. 
+00006c90: 2020 2023 206e 6f20 4174 7472 6962 7574     # no Attribut
+00006ca0: 6545 7272 6f72 2061 7420 6761 7262 6167  eError at garbag
+00006cb0: 6520 636f 6c6c 6563 7469 6f6e 2e0a 2020  e collection..  
+00006cc0: 2020 7061 7468 203d 2073 7472 2874 6d70    path = str(tmp
+00006cd0: 6469 722e 6a6f 696e 2822 7468 6973 5f66  dir.join("this_f
+00006ce0: 696c 655f 646f 6573 5f6e 6f74 5f65 7869  ile_does_not_exi
+00006cf0: 7374 2e6e 6322 2929 0a20 2020 2074 7279  st.nc")).    try
+00006d00: 3a0a 2020 2020 2020 2020 7769 7468 2068  :.        with h
+00006d10: 356e 6574 6364 662e 4669 6c65 2870 6174  5netcdf.File(pat
+00006d20: 682c 2022 7222 2920 6173 2064 733a 0a20  h, "r") as ds:. 
+00006d30: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00006d40: 7420 6473 0a20 2020 2065 7863 6570 7420  t ds.    except 
+00006d50: 4f53 4572 726f 723a 0a20 2020 2020 2020  OSError:.       
+00006d60: 2070 6173 730a 0a20 2020 2023 204c 6f6f   pass..    # Loo
+00006d70: 6b20 6174 2067 6172 6261 6765 2063 6f6c  k at garbage col
+00006d80: 6c65 6374 696f 6e3a 0a20 2020 2023 2041  lection:.    # A
+00006d90: 2073 696d 706c 6520 6763 2e63 6f6c 6c65   simple gc.colle
+00006da0: 6374 2829 2064 6f65 7320 6e6f 7420 7261  ct() does not ra
+00006db0: 6973 6520 616e 2065 7863 6570 7469 6f6e  ise an exception
+00006dc0: 2e0a 2020 2020 2320 4d75 7374 2073 6565  ..    # Must see
+00006dd0: 6b20 7468 6520 4669 6c65 206f 626a 6563  k the File objec
+00006de0: 7420 616e 6420 696d 6974 6174 6520 6974  t and imitate it
+00006df0: 7320 6465 6c20 636f 6d6d 616e 640a 2020  s del command.  
+00006e00: 2020 2320 6279 2066 6f72 6369 6e67 2069    # by forcing i
+00006e10: 7420 746f 2063 6c6f 7365 2e0a 2020 2020  t to close..    
+00006e20: 6f62 6a5f 6c69 7374 203d 2067 632e 6765  obj_list = gc.ge
+00006e30: 745f 6f62 6a65 6374 7328 290a 2020 2020  t_objects().    
+00006e40: 666f 7220 6f62 6a20 696e 206f 626a 5f6c  for obj in obj_l
+00006e50: 6973 743a 0a20 2020 2020 2020 2074 7279  ist:.        try
+00006e60: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
+00006e70: 5f68 356e 6574 6364 665f 4669 6c65 203d  _h5netcdf_File =
+00006e80: 2069 7369 6e73 7461 6e63 6528 6f62 6a2c   isinstance(obj,
+00006e90: 2068 356e 6574 6364 662e 4669 6c65 290a   h5netcdf.File).
+00006ea0: 2020 2020 2020 2020 6578 6365 7074 2041          except A
+00006eb0: 7474 7269 6275 7465 4572 726f 723a 0a20  ttributeError:. 
+00006ec0: 2020 2020 2020 2020 2020 2069 735f 6835             is_h5
+00006ed0: 6e65 7463 6466 5f46 696c 6520 3d20 4661  netcdf_File = Fa
+00006ee0: 6c73 650a 2020 2020 2020 2020 6966 2069  lse.        if i
+00006ef0: 735f 6835 6e65 7463 6466 5f46 696c 653a  s_h5netcdf_File:
+00006f00: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
+00006f10: 2e63 6c6f 7365 2829 0a0a 0a64 6566 2074  .close()...def t
+00006f20: 6573 745f 6372 6561 7465 5f76 6172 6961  est_create_varia
+00006f30: 626c 655f 6d61 7463 6869 6e67 5f73 6176  ble_matching_sav
+00006f40: 6564 5f64 696d 656e 7369 6f6e 2874 6d70  ed_dimension(tmp
+00006f50: 5f6c 6f63 616c 5f6f 725f 7265 6d6f 7465  _local_or_remote
+00006f60: 5f6e 6574 6364 6629 3a0a 2020 2020 6835  _netcdf):.    h5
+00006f70: 203d 2067 6574 5f68 6466 355f 6d6f 6475   = get_hdf5_modu
+00006f80: 6c65 2874 6d70 5f6c 6f63 616c 5f6f 725f  le(tmp_local_or_
+00006f90: 7265 6d6f 7465 5f6e 6574 6364 6629 0a0a  remote_netcdf)..
+00006fa0: 2020 2020 2320 6966 2068 3520 6973 206e      # if h5 is n
+00006fb0: 6f74 2068 3570 793a 0a20 2020 2023 2020  ot h5py:.    #  
+00006fc0: 2020 2070 7974 6573 742e 7866 6169 6c28     pytest.xfail(
+00006fd0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00006fe0: 636f 6d2f 6835 6e65 7463 6466 2f68 356e  com/h5netcdf/h5n
+00006ff0: 6574 6364 662f 6973 7375 6573 2f34 3822  etcdf/issues/48"
+00007000: 290a 0a20 2020 2077 6974 6820 6835 6e65  )..    with h5ne
+00007010: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+00007020: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00007030: 7463 6466 2c20 2277 2229 2061 7320 663a  tcdf, "w") as f:
+00007040: 0a20 2020 2020 2020 2066 2e64 696d 656e  .        f.dimen
+00007050: 7369 6f6e 735b 2278 225d 203d 2032 0a20  sions["x"] = 2. 
+00007060: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
+00007070: 7661 7269 6162 6c65 2822 7922 2c20 6461  variable("y", da
+00007080: 7461 3d5b 312c 2032 5d2c 2064 696d 656e  ta=[1, 2], dimen
+00007090: 7369 6f6e 733d 2822 7822 2c29 290a 0a20  sions=("x",)).. 
+000070a0: 2020 2077 6974 6820 6835 2e46 696c 6528     with h5.File(
+000070b0: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
+000070c0: 6f74 655f 6e65 7463 6466 2c20 2272 2229  ote_netcdf, "r")
+000070d0: 2061 7320 663a 0a20 2020 2020 2020 2064   as f:.        d
+000070e0: 696d 6c65 6e20 3d20 6622 7b66 5b27 7927  imlen = f"{f['y'
+000070f0: 5d2e 6469 6d73 5b30 5d2e 7661 6c75 6573  ].dims[0].values
+00007100: 2829 5b30 5d2e 7369 7a65 3a31 307d 220a  ()[0].size:10}".
+00007110: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+00007120: 5b22 7922 5d2e 6469 6d73 5b30 5d2e 6b65  ["y"].dims[0].ke
+00007130: 7973 2829 203d 3d20 5b4e 4f54 5f41 5f56  ys() == [NOT_A_V
+00007140: 4152 4941 424c 452e 6465 636f 6465 2822  ARIABLE.decode("
+00007150: 6173 6369 6922 2920 2b20 6469 6d6c 656e  ascii") + dimlen
+00007160: 5d0a 0a20 2020 2077 6974 6820 6835 6e65  ]..    with h5ne
+00007170: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+00007180: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00007190: 7463 6466 2c20 2261 2229 2061 7320 663a  tcdf, "a") as f:
+000071a0: 0a20 2020 2020 2020 2066 2e63 7265 6174  .        f.creat
+000071b0: 655f 7661 7269 6162 6c65 2822 7822 2c20  e_variable("x", 
+000071c0: 6461 7461 3d5b 302c 2031 5d2c 2064 696d  data=[0, 1], dim
+000071d0: 656e 7369 6f6e 733d 2822 7822 2c29 290a  ensions=("x",)).
+000071e0: 0a20 2020 2077 6974 6820 6835 2e46 696c  .    with h5.Fil
+000071f0: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
+00007200: 656d 6f74 655f 6e65 7463 6466 2c20 2272  emote_netcdf, "r
+00007210: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00007220: 2061 7373 6572 7420 665b 2279 225d 2e64   assert f["y"].d
+00007230: 696d 735b 305d 2e6b 6579 7328 2920 3d3d  ims[0].keys() ==
+00007240: 205b 2278 225d 0a0a 0a64 6566 2074 6573   ["x"]...def tes
+00007250: 745f 696e 7661 6c69 645f 6e65 7463 6466  t_invalid_netcdf
+00007260: 5f65 7272 6f72 2874 6d70 5f6c 6f63 616c  _error(tmp_local
+00007270: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
+00007280: 6629 3a0a 2020 2020 6966 2074 6d70 5f6c  f):.    if tmp_l
+00007290: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+000072a0: 6574 6364 662e 7374 6172 7473 7769 7468  etcdf.startswith
+000072b0: 2872 656d 6f74 655f 6835 293a 0a20 2020  (remote_h5):.   
+000072c0: 2020 2020 2070 7974 6573 742e 736b 6970       pytest.skip
+000072d0: 2822 5265 6d6f 7465 2048 4446 3520 646f  ("Remote HDF5 do
+000072e0: 6573 206e 6f74 2079 6574 2073 7570 706f  es not yet suppo
+000072f0: 7274 204c 5a46 2063 6f6d 7072 6573 7369  rt LZF compressi
+00007300: 6f6e 2229 0a20 2020 2077 6974 6820 6835  on").    with h5
+00007310: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+00007320: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
+00007330: 6e65 7463 6466 2c20 2277 222c 2069 6e76  netcdf, "w", inv
+00007340: 616c 6964 5f6e 6574 6364 663d 4661 6c73  alid_netcdf=Fals
+00007350: 6529 2061 7320 663a 0a20 2020 2020 2020  e) as f:.       
+00007360: 2023 2076 616c 6964 0a20 2020 2020 2020   # valid.       
+00007370: 2066 2e63 7265 6174 655f 7661 7269 6162   f.create_variab
+00007380: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00007390: 226c 7a66 5f63 6f6d 7072 6573 7365 6422  "lzf_compressed"
+000073a0: 2c20 6461 7461 3d5b 315d 2c20 6469 6d65  , data=[1], dime
+000073b0: 6e73 696f 6e73 3d28 2278 2229 2c20 636f  nsions=("x"), co
+000073c0: 6d70 7265 7373 696f 6e3d 226c 7a66 220a  mpression="lzf".
+000073d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000073e0: 2020 2320 696e 7661 6c69 640a 2020 2020    # invalid.    
+000073f0: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
+00007400: 7261 6973 6573 2868 356e 6574 6364 662e  raises(h5netcdf.
+00007410: 436f 6d70 6174 6962 696c 6974 7945 7272  CompatibilityErr
+00007420: 6f72 293a 0a20 2020 2020 2020 2020 2020  or):.           
+00007430: 2066 2e63 7265 6174 655f 7661 7269 6162   f.create_variab
+00007440: 6c65 2822 636f 6d70 6c65 7822 2c20 6461  le("complex", da
+00007450: 7461 3d31 6a29 0a20 2020 2020 2020 2077  ta=1j).        w
+00007460: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00007470: 7328 6835 6e65 7463 6466 2e43 6f6d 7061  s(h5netcdf.Compa
+00007480: 7469 6269 6c69 7479 4572 726f 7229 3a0a  tibilityError):.
+00007490: 2020 2020 2020 2020 2020 2020 662e 6174              f.at
+000074a0: 7472 735b 2263 6f6d 706c 6578 5f61 7474  trs["complex_att
+000074b0: 7222 5d20 3d20 316a 0a20 2020 2020 2020  r"] = 1j.       
+000074c0: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
+000074d0: 7365 7328 6835 6e65 7463 6466 2e43 6f6d  ses(h5netcdf.Com
+000074e0: 7061 7469 6269 6c69 7479 4572 726f 7229  patibilityError)
+000074f0: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
+00007500: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+00007510: 2273 6361 6c65 6f66 6673 6574 222c 2064  "scaleoffset", d
+00007520: 6174 613d 5b31 5d2c 2064 696d 656e 7369  ata=[1], dimensi
+00007530: 6f6e 733d 2822 7822 2c29 2c20 7363 616c  ons=("x",), scal
+00007540: 656f 6666 7365 743d 3029 0a0a 0a64 6566  eoffset=0)...def
+00007550: 2074 6573 745f 696e 7661 6c69 645f 6e65   test_invalid_ne
+00007560: 7463 6466 5f6f 6b61 7928 746d 705f 6c6f  tcdf_okay(tmp_lo
+00007570: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00007580: 7463 6466 293a 0a20 2020 2069 6620 746d  tcdf):.    if tm
+00007590: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+000075a0: 655f 6e65 7463 6466 2e73 7461 7274 7377  e_netcdf.startsw
+000075b0: 6974 6828 7265 6d6f 7465 5f68 3529 3a0a  ith(remote_h5):.
+000075c0: 2020 2020 2020 2020 7079 7465 7374 2e73          pytest.s
+000075d0: 6b69 7028 2268 3570 7964 2064 6f65 7320  kip("h5pyd does 
+000075e0: 6e6f 7420 7375 7070 6f72 7420 4e75 6d50  not support NumP
+000075f0: 7920 636f 6d70 6c65 7820 6474 7970 6520  y complex dtype 
+00007600: 7965 7422 290a 2020 2020 7769 7468 2070  yet").    with p
+00007610: 7974 6573 742e 7761 726e 7328 5573 6572  ytest.warns(User
+00007620: 5761 726e 696e 672c 206d 6174 6368 3d22  Warning, match="
+00007630: 696e 7661 6c69 6420 6e65 7463 6466 2066  invalid netcdf f
+00007640: 6561 7475 7265 7322 293a 0a20 2020 2020  eatures"):.     
+00007650: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
+00007660: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+00007670: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+00007680: 2c20 2277 222c 2069 6e76 616c 6964 5f6e  , "w", invalid_n
+00007690: 6574 6364 663d 5472 7565 2920 6173 2066  etcdf=True) as f
+000076a0: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
+000076b0: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+000076c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000076d0: 2022 6c7a 665f 636f 6d70 7265 7373 6564   "lzf_compressed
+000076e0: 222c 2064 6174 613d 5b31 5d2c 2064 696d  ", data=[1], dim
+000076f0: 656e 7369 6f6e 733d 2822 7822 292c 2063  ensions=("x"), c
+00007700: 6f6d 7072 6573 7369 6f6e 3d22 6c7a 6622  ompression="lzf"
+00007710: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+00007720: 2020 2020 2020 2020 2020 2066 2e63 7265             f.cre
+00007730: 6174 655f 7661 7269 6162 6c65 2822 636f  ate_variable("co
+00007740: 6d70 6c65 7822 2c20 6461 7461 3d31 6a29  mplex", data=1j)
+00007750: 0a20 2020 2020 2020 2020 2020 2066 2e61  .            f.a
+00007760: 7474 7273 5b22 636f 6d70 6c65 785f 6174  ttrs["complex_at
+00007770: 7472 225d 203d 2031 6a0a 2020 2020 2020  tr"] = 1j.      
+00007780: 2020 2020 2020 662e 6372 6561 7465 5f76        f.create_v
+00007790: 6172 6961 626c 6528 2273 6361 6c65 6f66  ariable("scaleof
+000077a0: 6673 6574 222c 2064 6174 613d 5b31 5d2c  fset", data=[1],
+000077b0: 2064 696d 656e 7369 6f6e 733d 2822 7822   dimensions=("x"
+000077c0: 2c29 2c20 7363 616c 656f 6666 7365 743d  ,), scaleoffset=
+000077d0: 3029 0a20 2020 2077 6974 6820 6835 6e65  0).    with h5ne
+000077e0: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+000077f0: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00007800: 7463 6466 2c20 2272 2229 2061 7320 663a  tcdf, "r") as f:
+00007810: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
+00007820: 696e 672e 6173 7365 7274 5f65 7175 616c  ing.assert_equal
+00007830: 2866 5b22 6c7a 665f 636f 6d70 7265 7373  (f["lzf_compress
+00007840: 6564 225d 5b3a 5d2c 205b 315d 290a 2020  ed"][:], [1]).  
+00007850: 2020 2020 2020 6173 7365 7274 2066 5b22        assert f["
+00007860: 636f 6d70 6c65 7822 5d5b 2e2e 2e5d 203d  complex"][...] =
+00007870: 3d20 316a 0a20 2020 2020 2020 2061 7373  = 1j.        ass
+00007880: 6572 7420 662e 6174 7472 735b 2263 6f6d  ert f.attrs["com
+00007890: 706c 6578 5f61 7474 7222 5d20 3d3d 2031  plex_attr"] == 1
+000078a0: 6a0a 2020 2020 2020 2020 6e70 2e74 6573  j.        np.tes
+000078b0: 7469 6e67 2e61 7373 6572 745f 6571 7561  ting.assert_equa
+000078c0: 6c28 665b 2273 6361 6c65 6f66 6673 6574  l(f["scaleoffset
+000078d0: 225d 5b3a 5d2c 205b 315d 290a 2020 2020  "][:], [1]).    
+000078e0: 6835 203d 2067 6574 5f68 6466 355f 6d6f  h5 = get_hdf5_mo
+000078f0: 6475 6c65 2874 6d70 5f6c 6f63 616c 5f6f  dule(tmp_local_o
+00007900: 725f 7265 6d6f 7465 5f6e 6574 6364 6629  r_remote_netcdf)
+00007910: 0a20 2020 2077 6974 6820 6835 2e46 696c  .    with h5.Fil
+00007920: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
+00007930: 656d 6f74 655f 6e65 7463 6466 2c20 2272  emote_netcdf, "r
+00007940: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00007950: 2061 7373 6572 7420 225f 4e43 5072 6f70   assert "_NCProp
+00007960: 6572 7469 6573 2220 6e6f 7420 696e 2066  erties" not in f
+00007970: 2e61 7474 7273 0a0a 0a64 6566 2074 6573  .attrs...def tes
+00007980: 745f 696e 7661 6c69 645f 6e65 7463 6466  t_invalid_netcdf
+00007990: 5f6f 7665 7277 7269 7465 5f76 616c 6964  _overwrite_valid
+000079a0: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+000079b0: 6629 3a0a 2020 2020 2320 6874 7470 733a  f):.    # https:
+000079c0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
+000079d0: 6574 6364 662f 6835 6e65 7463 6466 2f69  etcdf/h5netcdf/i
+000079e0: 7373 7565 732f 3136 350a 2020 2020 7769  ssues/165.    wi
+000079f0: 7468 206e 6574 4344 4634 2e44 6174 6173  th netCDF4.Datas
+00007a00: 6574 2874 6d70 5f6c 6f63 616c 5f6e 6574  et(tmp_local_net
+00007a10: 6364 662c 206d 6f64 653d 2277 2229 3a0a  cdf, mode="w"):.
+00007a20: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00007a30: 2077 6974 6820 7079 7465 7374 2e77 6172   with pytest.war
+00007a40: 6e73 2855 7365 7257 6172 6e69 6e67 293a  ns(UserWarning):
+00007a50: 0a20 2020 2020 2020 2077 6974 6820 6835  .        with h5
+00007a60: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+00007a70: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2261  local_netcdf, "a
+00007a80: 222c 2069 6e76 616c 6964 5f6e 6574 6364  ", invalid_netcd
+00007a90: 663d 5472 7565 2920 6173 2066 3a0a 2020  f=True) as f:.  
+00007aa0: 2020 2020 2020 2020 2020 662e 6372 6561            f.crea
+00007ab0: 7465 5f76 6172 6961 626c 6528 0a20 2020  te_variable(.   
+00007ac0: 2020 2020 2020 2020 2020 2020 2022 6c7a               "lz
+00007ad0: 665f 636f 6d70 7265 7373 6564 222c 2064  f_compressed", d
+00007ae0: 6174 613d 5b31 5d2c 2064 696d 656e 7369  ata=[1], dimensi
+00007af0: 6f6e 733d 2822 7822 292c 2063 6f6d 7072  ons=("x"), compr
+00007b00: 6573 7369 6f6e 3d22 6c7a 6622 0a20 2020  ession="lzf".   
+00007b10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00007b20: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
+00007b30: 7661 7269 6162 6c65 2822 636f 6d70 6c65  variable("comple
+00007b40: 7822 2c20 6461 7461 3d31 6a29 0a20 2020  x", data=1j).   
+00007b50: 2020 2020 2020 2020 2066 2e61 7474 7273           f.attrs
+00007b60: 5b22 636f 6d70 6c65 785f 6174 7472 225d  ["complex_attr"]
+00007b70: 203d 2031 6a0a 2020 2020 2020 2020 2020   = 1j.          
+00007b80: 2020 662e 6372 6561 7465 5f76 6172 6961    f.create_varia
+00007b90: 626c 6528 2273 6361 6c65 6f66 6673 6574  ble("scaleoffset
+00007ba0: 222c 2064 6174 613d 5b31 5d2c 2064 696d  ", data=[1], dim
+00007bb0: 656e 7369 6f6e 733d 2822 7822 2c29 2c20  ensions=("x",), 
+00007bc0: 7363 616c 656f 6666 7365 743d 3029 0a20  scaleoffset=0). 
+00007bd0: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
+00007be0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+00007bf0: 6e65 7463 6466 2c20 2272 2229 2061 7320  netcdf, "r") as 
+00007c00: 663a 0a20 2020 2020 2020 206e 702e 7465  f:.        np.te
+00007c10: 7374 696e 672e 6173 7365 7274 5f65 7175  sting.assert_equ
+00007c20: 616c 2866 5b22 6c7a 665f 636f 6d70 7265  al(f["lzf_compre
+00007c30: 7373 6564 225d 5b3a 5d2c 205b 315d 290a  ssed"][:], [1]).
+00007c40: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+00007c50: 5b22 636f 6d70 6c65 7822 5d5b 2e2e 2e5d  ["complex"][...]
+00007c60: 203d 3d20 316a 0a20 2020 2020 2020 2061   == 1j.        a
+00007c70: 7373 6572 7420 662e 6174 7472 735b 2263  ssert f.attrs["c
+00007c80: 6f6d 706c 6578 5f61 7474 7222 5d20 3d3d  omplex_attr"] ==
+00007c90: 2031 6a0a 2020 2020 2020 2020 6e70 2e74   1j.        np.t
+00007ca0: 6573 7469 6e67 2e61 7373 6572 745f 6571  esting.assert_eq
+00007cb0: 7561 6c28 665b 2273 6361 6c65 6f66 6673  ual(f["scaleoffs
+00007cc0: 6574 225d 5b3a 5d2c 205b 315d 290a 2020  et"][:], [1]).  
+00007cd0: 2020 6835 203d 2067 6574 5f68 6466 355f    h5 = get_hdf5_
+00007ce0: 6d6f 6475 6c65 2874 6d70 5f6c 6f63 616c  module(tmp_local
+00007cf0: 5f6e 6574 6364 6629 0a20 2020 2077 6974  _netcdf).    wit
+00007d00: 6820 6835 2e46 696c 6528 746d 705f 6c6f  h h5.File(tmp_lo
+00007d10: 6361 6c5f 6e65 7463 6466 2c20 2272 2229  cal_netcdf, "r")
+00007d20: 2061 7320 663a 0a20 2020 2020 2020 2061   as f:.        a
+00007d30: 7373 6572 7420 225f 4e43 5072 6f70 6572  ssert "_NCProper
+00007d40: 7469 6573 2220 6e6f 7420 696e 2066 2e61  ties" not in f.a
+00007d50: 7474 7273 0a0a 0a64 6566 2074 6573 745f  ttrs...def test_
+00007d60: 7265 6f70 656e 5f66 696c 655f 6469 6666  reopen_file_diff
+00007d70: 6572 656e 745f 6469 6d65 6e73 696f 6e5f  erent_dimension_
+00007d80: 7369 7a65 7328 746d 705f 6c6f 6361 6c5f  sizes(tmp_local_
+00007d90: 6e65 7463 6466 293a 0a20 2020 2023 2072  netcdf):.    # r
+00007da0: 6567 7265 7373 696f 6e20 7465 7374 2066  egression test f
+00007db0: 6f72 2068 7474 7073 3a2f 2f67 6974 6875  or https://githu
+00007dc0: 622e 636f 6d2f 6835 6e65 7463 6466 2f68  b.com/h5netcdf/h
+00007dd0: 356e 6574 6364 662f 6973 7375 6573 2f35  5netcdf/issues/5
+00007de0: 350a 2020 2020 7769 7468 2068 356e 6574  5.    with h5net
+00007df0: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
+00007e00: 616c 5f6e 6574 6364 662c 2022 7722 2920  al_netcdf, "w") 
+00007e10: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
+00007e20: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+00007e30: 222f 6f6e 652f 666f 6f22 2c20 6461 7461  "/one/foo", data
+00007e40: 3d5b 315d 2c20 6469 6d65 6e73 696f 6e73  =[1], dimensions
+00007e50: 3d28 2278 222c 2929 0a20 2020 2077 6974  =("x",)).    wit
+00007e60: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+00007e70: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+00007e80: 2c20 2261 2229 2061 7320 663a 0a20 2020  , "a") as f:.   
+00007e90: 2020 2020 2066 2e63 7265 6174 655f 7661       f.create_va
+00007ea0: 7269 6162 6c65 2822 2f74 776f 2f66 6f6f  riable("/two/foo
+00007eb0: 222c 2064 6174 613d 5b31 2c20 325d 2c20  ", data=[1, 2], 
+00007ec0: 6469 6d65 6e73 696f 6e73 3d28 2278 222c  dimensions=("x",
+00007ed0: 2929 0a20 2020 2077 6974 6820 6e65 7443  )).    with netC
+00007ee0: 4446 342e 4461 7461 7365 7428 746d 705f  DF4.Dataset(tmp_
+00007ef0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
+00007f00: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+00007f10: 2061 7373 6572 7420 662e 6772 6f75 7073   assert f.groups
+00007f20: 5b22 6f6e 6522 5d2e 7661 7269 6162 6c65  ["one"].variable
+00007f30: 735b 2266 6f6f 225d 5b2e 2e2e 5d2e 7368  s["foo"][...].sh
+00007f40: 6170 6520 3d3d 2028 312c 290a 0a0a 6465  ape == (1,)...de
+00007f50: 6620 7465 7374 5f69 6e76 616c 6964 5f74  f test_invalid_t
+00007f60: 6865 6e5f 7661 6c69 645f 6e6f 5f6e 6370  hen_valid_no_ncp
+00007f70: 726f 7065 7274 6965 7328 746d 705f 6c6f  roperties(tmp_lo
+00007f80: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+00007f90: 7463 6466 293a 0a20 2020 2077 6974 6820  tcdf):.    with 
+00007fa0: 7079 7465 7374 2e77 6172 6e73 2855 7365  pytest.warns(Use
+00007fb0: 7257 6172 6e69 6e67 2c20 6d61 7463 683d  rWarning, match=
+00007fc0: 2269 6e76 616c 6964 206e 6574 6364 6620  "invalid netcdf 
+00007fd0: 6665 6174 7572 6573 2229 3a0a 2020 2020  features"):.    
+00007fe0: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
+00007ff0: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
+00008000: 5f6f 725f 7265 6d6f 7465 5f6e 6574 6364  _or_remote_netcd
+00008010: 662c 2022 7722 2c20 696e 7661 6c69 645f  f, "w", invalid_
+00008020: 6e65 7463 6466 3d54 7275 6529 3a0a 2020  netcdf=True):.  
+00008030: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00008040: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
+00008050: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+00008060: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+00008070: 2c20 2261 2229 3a0a 2020 2020 2020 2020  , "a"):.        
+00008080: 7061 7373 0a20 2020 2068 3520 3d20 6765  pass.    h5 = ge
+00008090: 745f 6864 6635 5f6d 6f64 756c 6528 746d  t_hdf5_module(tm
+000080a0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+000080b0: 655f 6e65 7463 6466 290a 2020 2020 7769  e_netcdf).    wi
+000080c0: 7468 2068 352e 4669 6c65 2874 6d70 5f6c  th h5.File(tmp_l
+000080d0: 6f63 616c 5f6f 725f 7265 6d6f 7465 5f6e  ocal_or_remote_n
+000080e0: 6574 6364 662c 2022 7222 2920 6173 2066  etcdf, "r") as f
+000080f0: 3a0a 2020 2020 2020 2020 2320 7374 696c  :.        # stil
+00008100: 6c20 6e6f 7420 6120 7661 6c69 6420 6e65  l not a valid ne
+00008110: 7463 6466 2066 696c 650a 2020 2020 2020  tcdf file.      
+00008120: 2020 6173 7365 7274 2022 5f4e 4350 726f    assert "_NCPro
+00008130: 7065 7274 6965 7322 206e 6f74 2069 6e20  perties" not in 
+00008140: 662e 6174 7472 730a 0a0a 6465 6620 7465  f.attrs...def te
+00008150: 7374 5f63 7265 6174 696e 675f 616e 645f  st_creating_and_
+00008160: 7265 7369 7a69 6e67 5f75 6e6c 696d 6974  resizing_unlimit
+00008170: 6564 5f64 696d 656e 7369 6f6e 7328 746d  ed_dimensions(tm
+00008180: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+00008190: 655f 6e65 7463 6466 293a 0a20 2020 2077  e_netcdf):.    w
+000081a0: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
+000081b0: 6528 746d 705f 6c6f 6361 6c5f 6f72 5f72  e(tmp_local_or_r
+000081c0: 656d 6f74 655f 6e65 7463 6466 2c20 2277  emote_netcdf, "w
+000081d0: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+000081e0: 2066 2e64 696d 656e 7369 6f6e 735b 2278   f.dimensions["x
+000081f0: 225d 203d 204e 6f6e 650a 2020 2020 2020  "] = None.      
+00008200: 2020 662e 6469 6d65 6e73 696f 6e73 5b22    f.dimensions["
+00008210: 7922 5d20 3d20 3135 0a20 2020 2020 2020  y"] = 15.       
+00008220: 2066 2e64 696d 656e 7369 6f6e 735b 227a   f.dimensions["z
+00008230: 225d 203d 204e 6f6e 650a 2020 2020 2020  "] = None.      
+00008240: 2020 662e 7265 7369 7a65 5f64 696d 656e    f.resize_dimen
+00008250: 7369 6f6e 2822 7a22 2c20 3230 290a 0a20  sion("z", 20).. 
+00008260: 2020 2020 2020 2077 6974 6820 7079 7465         with pyte
+00008270: 7374 2e72 6169 7365 7328 5661 6c75 6545  st.raises(ValueE
+00008280: 7272 6f72 2920 6173 2065 3a0a 2020 2020  rror) as e:.    
+00008290: 2020 2020 2020 2020 662e 7265 7369 7a65          f.resize
+000082a0: 5f64 696d 656e 7369 6f6e 2822 7922 2c20  _dimension("y", 
+000082b0: 3230 290a 2020 2020 2020 2020 6173 7365  20).        asse
+000082c0: 7274 2065 2e76 616c 7565 2e61 7267 735b  rt e.value.args[
+000082d0: 305d 203d 3d20 280a 2020 2020 2020 2020  0] == (.        
+000082e0: 2020 2020 2244 696d 656e 7369 6f6e 2027      "Dimension '
+000082f0: 7927 2069 7320 6e6f 7420 756e 6c69 6d69  y' is not unlimi
+00008300: 7465 6420 616e 6420 7468 7573 2063 616e  ted and thus can
+00008310: 6e6f 7420 6265 2072 6573 697a 6564 2e22  not be resized."
+00008320: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00008330: 6835 203d 2067 6574 5f68 6466 355f 6d6f  h5 = get_hdf5_mo
+00008340: 6475 6c65 2874 6d70 5f6c 6f63 616c 5f6f  dule(tmp_local_o
+00008350: 725f 7265 6d6f 7465 5f6e 6574 6364 6629  r_remote_netcdf)
+00008360: 0a20 2020 2023 2041 7373 6572 7420 736f  .    # Assert so
+00008370: 6d65 2062 6568 6176 696f 7220 6f62 7365  me behavior obse
+00008380: 7276 6564 2062 7920 7573 696e 6720 7468  rved by using th
+00008390: 6520 4320 6e65 7443 4446 2062 696e 6469  e C netCDF bindi
+000083a0: 6e67 732e 0a20 2020 2077 6974 6820 6835  ngs..    with h5
+000083b0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+000083c0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+000083d0: 2c20 2272 2229 2061 7320 663a 0a20 2020  , "r") as f:.   
+000083e0: 2020 2020 2061 7373 6572 7420 665b 2278       assert f["x
+000083f0: 225d 2e73 6861 7065 203d 3d20 2830 2c29  "].shape == (0,)
+00008400: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00008410: 665b 2278 225d 2e6d 6178 7368 6170 6520  f["x"].maxshape 
+00008420: 3d3d 2028 4e6f 6e65 2c29 0a20 2020 2020  == (None,).     
+00008430: 2020 2061 7373 6572 7420 665b 2279 225d     assert f["y"]
+00008440: 2e73 6861 7065 203d 3d20 2831 352c 290a  .shape == (15,).
+00008450: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+00008460: 5b22 7922 5d2e 6d61 7873 6861 7065 203d  ["y"].maxshape =
+00008470: 3d20 2831 352c 290a 2020 2020 2020 2020  = (15,).        
+00008480: 6173 7365 7274 2066 5b22 7a22 5d2e 7368  assert f["z"].sh
+00008490: 6170 6520 3d3d 2028 3230 2c29 0a20 2020  ape == (20,).   
+000084a0: 2020 2020 2061 7373 6572 7420 665b 227a       assert f["z
+000084b0: 225d 2e6d 6178 7368 6170 6520 3d3d 2028  "].maxshape == (
+000084c0: 4e6f 6e65 2c29 0a0a 0a64 6566 2074 6573  None,)...def tes
+000084d0: 745f 6372 6561 7469 6e67 5f76 6172 6961  t_creating_varia
+000084e0: 626c 6573 5f77 6974 685f 756e 6c69 6d69  bles_with_unlimi
+000084f0: 7465 645f 6469 6d65 6e73 696f 6e73 2874  ted_dimensions(t
+00008500: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
+00008510: 7465 5f6e 6574 6364 6629 3a0a 2020 2020  te_netcdf):.    
+00008520: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+00008530: 6c65 2874 6d70 5f6c 6f63 616c 5f6f 725f  le(tmp_local_or_
+00008540: 7265 6d6f 7465 5f6e 6574 6364 662c 2022  remote_netcdf, "
+00008550: 7722 2920 6173 2066 3a0a 2020 2020 2020  w") as f:.      
+00008560: 2020 662e 6469 6d65 6e73 696f 6e73 5b22    f.dimensions["
+00008570: 7822 5d20 3d20 4e6f 6e65 0a20 2020 2020  x"] = None.     
+00008580: 2020 2066 2e64 696d 656e 7369 6f6e 735b     f.dimensions[
+00008590: 2279 225d 203d 2032 0a0a 2020 2020 2020  "y"] = 2..      
+000085a0: 2020 2320 4372 6561 7469 6e67 2061 2076    # Creating a v
+000085b0: 6172 6961 626c 6520 7769 7468 6f75 7420  ariable without 
+000085c0: 6461 7461 2077 696c 6c20 696e 6974 6961  data will initia
+000085d0: 6c69 7a65 2061 6e20 6172 7261 7920 7769  lize an array wi
+000085e0: 7468 207a 6572 6f0a 2020 2020 2020 2020  th zero.        
+000085f0: 2320 6c65 6e67 7468 2e0a 2020 2020 2020  # length..      
+00008600: 2020 662e 6372 6561 7465 5f76 6172 6961    f.create_varia
+00008610: 626c 6528 2264 756d 6d79 222c 2064 696d  ble("dummy", dim
+00008620: 656e 7369 6f6e 733d 2822 7822 2c20 2279  ensions=("x", "y
+00008630: 2229 2c20 6474 7970 653d 6e70 2e69 6e74  "), dtype=np.int
+00008640: 3634 290a 2020 2020 2020 2020 6173 7365  64).        asse
+00008650: 7274 2066 2e76 6172 6961 626c 6573 5b22  rt f.variables["
+00008660: 6475 6d6d 7922 5d2e 7368 6170 6520 3d3d  dummy"].shape ==
+00008670: 2028 302c 2032 290a 2020 2020 2020 2020   (0, 2).        
+00008680: 6173 7365 7274 2066 2e76 6172 6961 626c  assert f.variabl
+00008690: 6573 5b22 6475 6d6d 7922 5d2e 5f68 3564  es["dummy"]._h5d
+000086a0: 732e 6d61 7873 6861 7065 203d 3d20 284e  s.maxshape == (N
+000086b0: 6f6e 652c 2032 290a 0a20 2020 2020 2020  one, 2)..       
+000086c0: 2023 2054 7279 696e 6720 746f 2063 7265   # Trying to cre
+000086d0: 6174 6520 6120 7661 7269 6162 6c65 2077  ate a variable w
+000086e0: 6869 6c65 2074 6865 2063 7572 7265 6e74  hile the current
+000086f0: 2073 697a 6520 6f66 2074 6865 2064 696d   size of the dim
+00008700: 656e 7369 6f6e 0a20 2020 2020 2020 2023  ension.        #
+00008710: 2069 7320 7374 696c 6c20 7a65 726f 2077   is still zero w
+00008720: 696c 6c20 6661 696c 2e0a 2020 2020 2020  ill fail..      
+00008730: 2020 7769 7468 2070 7974 6573 742e 7261    with pytest.ra
+00008740: 6973 6573 2856 616c 7565 4572 726f 7229  ises(ValueError)
+00008750: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00008760: 2020 2066 2e63 7265 6174 655f 7661 7269     f.create_vari
+00008770: 6162 6c65 280a 2020 2020 2020 2020 2020  able(.          
+00008780: 2020 2020 2020 2264 756d 6d79 3222 2c20        "dummy2", 
+00008790: 6461 7461 3d6e 702e 6172 7261 7928 5b5b  data=np.array([[
+000087a0: 312c 2032 5d2c 205b 332c 2034 5d5d 292c  1, 2], [3, 4]]),
+000087b0: 2064 696d 656e 7369 6f6e 733d 2822 7822   dimensions=("x"
+000087c0: 2c20 2279 2229 0a20 2020 2020 2020 2020  , "y").         
+000087d0: 2020 2029 0a20 2020 2020 2020 2061 7373     ).        ass
+000087e0: 6572 7420 652e 7661 6c75 652e 6172 6773  ert e.value.args
+000087f0: 5b30 5d20 3d3d 2022 5368 6170 6520 7475  [0] == "Shape tu
+00008800: 706c 6520 6973 2069 6e63 6f6d 7061 7469  ple is incompati
+00008810: 626c 6520 7769 7468 2064 6174 6122 0a0a  ble with data"..
+00008820: 2020 2020 2020 2020 2320 4372 6561 7469          # Creati
+00008830: 6e67 2061 2063 6f6f 7264 696e 6174 6520  ng a coordinate 
+00008840: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+00008850: 2066 2e63 7265 6174 655f 7661 7269 6162   f.create_variab
+00008860: 6c65 2822 7822 2c20 6469 6d65 6e73 696f  le("x", dimensio
+00008870: 6e73 3d28 2278 222c 292c 2064 7479 7065  ns=("x",), dtype
+00008880: 3d6e 702e 696e 7436 3429 0a0a 2020 2020  =np.int64)..    
+00008890: 2020 2020 2320 5265 7369 7a65 2064 6174      # Resize dat
+000088a0: 612e 0a20 2020 2020 2020 2061 7373 6572  a..        asser
+000088b0: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
+000088c0: 756d 6d79 225d 2e73 6861 7065 203d 3d20  ummy"].shape == 
+000088d0: 2830 2c20 3229 0a20 2020 2020 2020 2066  (0, 2).        f
+000088e0: 2e72 6573 697a 655f 6469 6d65 6e73 696f  .resize_dimensio
+000088f0: 6e28 2278 222c 2033 290a 2020 2020 2020  n("x", 3).      
+00008900: 2020 2320 5468 6973 2077 696c 6c20 616c    # This will al
+00008910: 736f 2066 6f72 6365 2061 2072 6573 697a  so force a resiz
+00008920: 6520 6f66 2074 6865 2065 7869 7374 696e  e of the existin
+00008930: 6720 7661 7269 6162 6c65 7320 616e 6420  g variables and 
+00008940: 6974 2077 696c 6c0a 2020 2020 2020 2020  it will.        
+00008950: 2320 6265 2070 6164 6465 6420 7769 7468  # be padded with
+00008960: 207a 6572 6f73 2e0a 2020 2020 2020 2020   zeros..        
+00008970: 6173 7365 7274 2066 2e64 696d 656e 7369  assert f.dimensi
+00008980: 6f6e 735b 2278 225d 2e73 697a 6520 3d3d  ons["x"].size ==
+00008990: 2033 0a20 2020 2020 2020 206e 702e 7465   3.        np.te
+000089a0: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
+000089b0: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
+000089c0: 735b 2264 756d 6d79 225d 2c20 6e70 2e7a  s["dummy"], np.z
+000089d0: 6572 6f73 2828 332c 2032 2929 290a 0a20  eros((3, 2))).. 
+000089e0: 2020 2020 2020 2023 2043 7265 6174 696e         # Creatin
+000089f0: 6720 616e 6f74 6865 7220 7661 7269 6162  g another variab
+00008a00: 6c65 2077 6974 6820 6e6f 2064 6174 6120  le with no data 
+00008a10: 7769 6c6c 206e 6f77 2061 6c73 6f20 7461  will now also ta
+00008a20: 6b65 2074 6865 2073 6861 7065 0a20 2020  ke the shape.   
+00008a30: 2020 2020 2023 206f 6620 7468 6520 6375       # of the cu
+00008a40: 7272 656e 7420 6469 6d65 6e73 696f 6e73  rrent dimensions
+00008a50: 2e0a 2020 2020 2020 2020 662e 6372 6561  ..        f.crea
+00008a60: 7465 5f76 6172 6961 626c 6528 2264 756d  te_variable("dum
+00008a70: 6d79 3322 2c20 6469 6d65 6e73 696f 6e73  my3", dimensions
+00008a80: 3d28 2278 222c 2022 7922 292c 2064 7479  =("x", "y"), dty
+00008a90: 7065 3d6e 702e 696e 7436 3429 0a20 2020  pe=np.int64).   
+00008aa0: 2020 2020 2061 7373 6572 7420 662e 7661       assert f.va
+00008ab0: 7269 6162 6c65 735b 2264 756d 6d79 3322  riables["dummy3"
+00008ac0: 5d2e 7368 6170 6520 3d3d 2028 332c 2032  ].shape == (3, 2
+00008ad0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00008ae0: 2066 2e76 6172 6961 626c 6573 5b22 6475   f.variables["du
+00008af0: 6d6d 7933 225d 2e5f 6835 6473 2e6d 6178  mmy3"]._h5ds.max
+00008b00: 7368 6170 6520 3d3d 2028 4e6f 6e65 2c20  shape == (None, 
+00008b10: 3229 0a20 2020 2020 2020 206e 702e 7465  2).        np.te
+00008b20: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
+00008b30: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
+00008b40: 735b 2264 756d 6d79 3322 5d2c 206e 702e  s["dummy3"], np.
+00008b50: 7a65 726f 7328 2833 2c20 3229 2929 0a0a  zeros((3, 2)))..
+00008b60: 2020 2020 2020 2020 2320 5772 6974 696e          # Writin
+00008b70: 6720 746f 2061 2076 6172 6961 626c 6520  g to a variable 
+00008b80: 7769 7468 2061 6e20 756e 6c69 6d69 7465  with an unlimite
+00008b90: 6420 6469 6d65 6e73 696f 6e20 7261 6973  d dimension rais
+00008ba0: 6573 0a20 2020 2020 2020 2069 6620 746d  es.        if tm
+00008bb0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+00008bc0: 655f 6e65 7463 6466 2e73 7461 7274 7377  e_netcdf.startsw
+00008bd0: 6974 6828 7265 6d6f 7465 5f68 3529 3a0a  ith(remote_h5):.
+00008be0: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00008bf0: 2064 6f6e 2774 2065 7870 6563 7420 616e   don't expect an
+00008c00: 7920 6572 726f 7273 2e20 5468 6973 2069  y errors. This i
+00008c10: 7320 6566 6665 6374 6976 656c 7920 6120  s effectively a 
+00008c20: 766f 6964 2063 6f6e 7465 7874 206d 616e  void context man
+00008c30: 6167 6572 0a20 2020 2020 2020 2020 2020  ager.           
+00008c40: 2065 7870 6563 7465 645f 6572 726f 7273   expected_errors
+00008c50: 203d 206d 656d 6f72 7976 6965 7728 6222   = memoryview(b"
+00008c60: 2229 0a20 2020 2020 2020 2065 6c73 653a  ").        else:
+00008c70: 0a20 2020 2020 2020 2020 2020 2065 7870  .            exp
+00008c80: 6563 7465 645f 6572 726f 7273 203d 2070  ected_errors = p
+00008c90: 7974 6573 742e 7261 6973 6573 2854 7970  ytest.raises(Typ
+00008ca0: 6545 7272 6f72 290a 2020 2020 2020 2020  eError).        
+00008cb0: 7769 7468 2065 7870 6563 7465 645f 6572  with expected_er
+00008cc0: 726f 7273 2061 7320 653a 0a20 2020 2020  rors as e:.     
+00008cd0: 2020 2020 2020 2066 2e76 6172 6961 626c         f.variabl
+00008ce0: 6573 5b22 6475 6d6d 7933 225d 5b3a 5d20  es["dummy3"][:] 
+00008cf0: 3d20 6e70 2e6f 6e65 7328 2835 2c20 3229  = np.ones((5, 2)
+00008d00: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00008d10: 2074 6d70 5f6c 6f63 616c 5f6f 725f 7265   tmp_local_or_re
+00008d20: 6d6f 7465 5f6e 6574 6364 662e 7374 6172  mote_netcdf.star
+00008d30: 7473 7769 7468 2872 656d 6f74 655f 6835  tswith(remote_h5
+00008d40: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
+00008d50: 7373 6572 7420 652e 7661 6c75 652e 6172  ssert e.value.ar
+00008d60: 6773 5b30 5d20 3d3d 2022 4361 6e27 7420  gs[0] == "Can't 
+00008d70: 6272 6f61 6463 6173 7420 2835 2c20 3229  broadcast (5, 2)
+00008d80: 202d 3e20 2833 2c20 3229 220a 2020 2020   -> (3, 2)".    
+00008d90: 2020 2020 6173 7365 7274 2066 2e76 6172      assert f.var
+00008da0: 6961 626c 6573 5b22 6475 6d6d 7933 225d  iables["dummy3"]
+00008db0: 2e73 6861 7065 203d 3d20 2833 2c20 3229  .shape == (3, 2)
+00008dc0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00008dd0: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
+00008de0: 6d79 3322 5d2e 5f68 3564 732e 6d61 7873  my3"]._h5ds.maxs
+00008df0: 6861 7065 203d 3d20 284e 6f6e 652c 2032  hape == (None, 2
+00008e00: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00008e10: 2066 5b22 7822 5d2e 7368 6170 6520 3d3d   f["x"].shape ==
+00008e20: 2028 332c 290a 2020 2020 2020 2020 6173   (3,).        as
+00008e30: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
+00008e40: 735b 2278 225d 2e73 697a 6520 3d3d 2033  s["x"].size == 3
+00008e50: 0a20 2020 2020 2020 2069 6620 746d 705f  .        if tmp_
+00008e60: 6c6f 6361 6c5f 6f72 5f72 656d 6f74 655f  local_or_remote_
+00008e70: 6e65 7463 6466 2e73 7461 7274 7377 6974  netcdf.startswit
+00008e80: 6828 7265 6d6f 7465 5f68 3529 3a0a 2020  h(remote_h5):.  
+00008e90: 2020 2020 2020 2020 2020 2320 6835 7079            # h5py
+00008ea0: 6420 7772 6974 6573 2074 6865 2064 6174  d writes the dat
+00008eb0: 612c 2062 7574 2064 6f65 7320 6e6f 7420  a, but does not 
+00008ec0: 6578 7061 6e64 2074 6865 2064 696d 656e  expand the dimen
+00008ed0: 7369 6f6e 730a 2020 2020 2020 2020 2020  sions.          
+00008ee0: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
+00008ef0: 6572 745f 616c 6c63 6c6f 7365 2866 2e76  ert_allclose(f.v
+00008f00: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
+00008f10: 225d 2c20 6e70 2e6f 6e65 7328 2833 2c20  "], np.ones((3, 
+00008f20: 3229 2929 0a20 2020 2020 2020 2065 6c73  2))).        els
+00008f30: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00008f40: 206f 7269 6769 6e61 6c20 6461 7461 2069   original data i
+00008f50: 7320 6b65 7074 2066 6f72 2068 3570 790a  s kept for h5py.
+00008f60: 2020 2020 2020 2020 2020 2020 6e70 2e74              np.t
+00008f70: 6573 7469 6e67 2e61 7373 6572 745f 616c  esting.assert_al
+00008f80: 6c63 6c6f 7365 2866 2e76 6172 6961 626c  lclose(f.variabl
+00008f90: 6573 5b22 6475 6d6d 7933 225d 2c20 6e70  es["dummy3"], np
+00008fa0: 2e7a 6572 6f73 2828 332c 2032 2929 290a  .zeros((3, 2))).
+00008fb0: 0a20 2020 2023 2043 6c6f 7365 2061 6e64  .    # Close and
+00008fc0: 2072 6561 6420 6167 6169 6e20 746f 2061   read again to a
+00008fd0: 6c73 6f20 7465 7374 2063 6f72 7265 6374  lso test correct
+00008fe0: 2070 6172 7369 6e67 206f 6620 756e 6c69   parsing of unli
+00008ff0: 6d69 7465 640a 2020 2020 2320 6469 6d65  mited.    # dime
+00009000: 6e73 696f 6e73 2e0a 2020 2020 7769 7468  nsions..    with
+00009010: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
+00009020: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
+00009030: 7465 5f6e 6574 6364 662c 2022 7222 2920  te_netcdf, "r") 
+00009040: 6173 2066 3a0a 2020 2020 2020 2020 6173  as f:.        as
+00009050: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
+00009060: 735b 2278 225d 2e69 7375 6e6c 696d 6974  s["x"].isunlimit
+00009070: 6564 2829 0a20 2020 2020 2020 2061 7373  ed().        ass
+00009080: 6572 7420 662e 6469 6d65 6e73 696f 6e73  ert f.dimensions
+00009090: 5b22 7822 5d2e 7369 7a65 203d 3d20 330a  ["x"].size == 3.
+000090a0: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+000090b0: 2e5f 6835 6669 6c65 5b22 7822 5d2e 6d61  ._h5file["x"].ma
+000090c0: 7873 6861 7065 203d 3d20 284e 6f6e 652c  xshape == (None,
+000090d0: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+000090e0: 2066 2e5f 6835 6669 6c65 5b22 7822 5d2e   f._h5file["x"].
+000090f0: 7368 6170 6520 3d3d 2028 332c 290a 0a20  shape == (3,).. 
+00009100: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
+00009110: 6469 6d65 6e73 696f 6e73 5b22 7922 5d2e  dimensions["y"].
+00009120: 7369 7a65 203d 3d20 320a 2020 2020 2020  size == 2.      
+00009130: 2020 6173 7365 7274 2066 2e5f 6835 6669    assert f._h5fi
+00009140: 6c65 5b22 7922 5d2e 6d61 7873 6861 7065  le["y"].maxshape
+00009150: 203d 3d20 2832 2c29 0a20 2020 2020 2020   == (2,).       
+00009160: 2061 7373 6572 7420 662e 5f68 3566 696c   assert f._h5fil
+00009170: 655b 2279 225d 2e73 6861 7065 203d 3d20  e["y"].shape == 
+00009180: 2832 2c29 0a0a 0a64 6566 2074 6573 745f  (2,)...def test_
+00009190: 7772 6974 696e 675f 746f 5f61 6e5f 756e  writing_to_an_un
+000091a0: 6c69 6d69 7465 645f 6469 6d65 6e73 696f  limited_dimensio
+000091b0: 6e28 746d 705f 6c6f 6361 6c5f 6f72 5f72  n(tmp_local_or_r
+000091c0: 656d 6f74 655f 6e65 7463 6466 293a 0a20  emote_netcdf):. 
+000091d0: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
+000091e0: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+000091f0: 6f72 5f72 656d 6f74 655f 6e65 7463 6466  or_remote_netcdf
+00009200: 2c20 2277 2229 2061 7320 663a 0a20 2020  , "w") as f:.   
+00009210: 2020 2020 2023 2054 776f 2064 696d 656e       # Two dimen
+00009220: 7369 6f6e 732c 206f 6e6c 7920 6f6e 6520  sions, only one 
+00009230: 6973 2075 6e6c 696d 6974 6564 2e0a 2020  is unlimited..  
+00009240: 2020 2020 2020 662e 6469 6d65 6e73 696f        f.dimensio
+00009250: 6e73 5b22 7822 5d20 3d20 4e6f 6e65 0a20  ns["x"] = None. 
+00009260: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
+00009270: 6f6e 735b 2279 225d 203d 2033 0a20 2020  ons["y"] = 3.   
+00009280: 2020 2020 2066 2e64 696d 656e 7369 6f6e       f.dimension
+00009290: 735b 227a 225d 203d 204e 6f6e 650a 0a20  s["z"] = None.. 
+000092a0: 2020 2020 2020 2023 2043 616e 6e6f 7420         # Cannot 
+000092b0: 6372 6561 7465 2069 7420 7769 7468 6f75  create it withou
+000092c0: 7420 6669 7273 7420 7265 7369 7a69 6e67  t first resizing
+000092d0: 2069 742e 0a20 2020 2020 2020 2077 6974   it..        wit
+000092e0: 6820 7079 7465 7374 2e72 6169 7365 7328  h pytest.raises(
+000092f0: 5661 6c75 6545 7272 6f72 2920 6173 2065  ValueError) as e
+00009300: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
+00009310: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+00009320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009330: 2022 6475 6d6d 7931 222c 2064 6174 613d   "dummy1", data=
+00009340: 6e70 2e61 7272 6179 285b 5b31 2c20 322c  np.array([[1, 2,
+00009350: 2033 5d5d 292c 2064 696d 656e 7369 6f6e   3]]), dimension
+00009360: 733d 2822 7822 2c20 2279 2229 0a20 2020  s=("x", "y").   
+00009370: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00009380: 2020 2020 2020 2061 7373 6572 7420 652e         assert e.
+00009390: 7661 6c75 652e 6172 6773 5b30 5d20 3d3d  value.args[0] ==
+000093a0: 2022 5368 6170 6520 7475 706c 6520 6973   "Shape tuple is
+000093b0: 2069 6e63 6f6d 7061 7469 626c 6520 7769   incompatible wi
+000093c0: 7468 2064 6174 6122 0a0a 2020 2020 2020  th data"..      
+000093d0: 2020 2320 5769 7468 6f75 7420 6461 7461    # Without data
+000093e0: 2e0a 2020 2020 2020 2020 662e 6372 6561  ..        f.crea
+000093f0: 7465 5f76 6172 6961 626c 6528 2264 756d  te_variable("dum
+00009400: 6d79 3122 2c20 6469 6d65 6e73 696f 6e73  my1", dimensions
+00009410: 3d28 2278 222c 2022 7922 292c 2064 7479  =("x", "y"), dty
+00009420: 7065 3d6e 702e 696e 7436 3429 0a20 2020  pe=np.int64).   
+00009430: 2020 2020 2066 2e63 7265 6174 655f 7661       f.create_va
+00009440: 7269 6162 6c65 2822 6475 6d6d 7932 222c  riable("dummy2",
+00009450: 2064 696d 656e 7369 6f6e 733d 2822 7822   dimensions=("x"
+00009460: 2c20 2279 2229 2c20 6474 7970 653d 6e70  , "y"), dtype=np
+00009470: 2e69 6e74 3634 290a 2020 2020 2020 2020  .int64).        
+00009480: 662e 6372 6561 7465 5f76 6172 6961 626c  f.create_variabl
+00009490: 6528 2264 756d 6d79 3322 2c20 6469 6d65  e("dummy3", dime
+000094a0: 6e73 696f 6e73 3d28 2278 222c 2022 7922  nsions=("x", "y"
+000094b0: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
+000094c0: 3429 0a20 2020 2020 2020 2066 2e63 7265  4).        f.cre
+000094d0: 6174 655f 7661 7269 6162 6c65 2822 6475  ate_variable("du
+000094e0: 6d6d 7958 222c 2064 696d 656e 7369 6f6e  mmyX", dimension
+000094f0: 733d 2822 7822 2c20 2279 222c 2022 7a22  s=("x", "y", "z"
+00009500: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
+00009510: 3429 0a20 2020 2020 2020 2067 203d 2066  4).        g = f
+00009520: 2e63 7265 6174 655f 6772 6f75 7028 2274  .create_group("t
+00009530: 6573 7422 290a 2020 2020 2020 2020 672e  est").        g.
+00009540: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+00009550: 2264 756d 6d79 3422 2c20 6469 6d65 6e73  "dummy4", dimens
+00009560: 696f 6e73 3d28 2279 222c 2022 7822 2c20  ions=("y", "x", 
+00009570: 2278 2229 2c20 6474 7970 653d 6e70 2e69  "x"), dtype=np.i
+00009580: 6e74 3634 290a 2020 2020 2020 2020 672e  nt64).        g.
+00009590: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
+000095a0: 2264 756d 6d79 3522 2c20 6469 6d65 6e73  "dummy5", dimens
+000095b0: 696f 6e73 3d28 2279 222c 2022 7922 292c  ions=("y", "y"),
+000095c0: 2064 7479 7065 3d6e 702e 696e 7436 3429   dtype=np.int64)
+000095d0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000095e0: 2066 2e76 6172 6961 626c 6573 5b22 6475   f.variables["du
+000095f0: 6d6d 7931 225d 2e73 6861 7065 203d 3d20  mmy1"].shape == 
+00009600: 2830 2c20 3329 0a20 2020 2020 2020 2061  (0, 3).        a
+00009610: 7373 6572 7420 662e 7661 7269 6162 6c65  ssert f.variable
+00009620: 735b 2264 756d 6d79 3222 5d2e 7368 6170  s["dummy2"].shap
+00009630: 6520 3d3d 2028 302c 2033 290a 2020 2020  e == (0, 3).    
+00009640: 2020 2020 6173 7365 7274 2066 2e76 6172      assert f.var
+00009650: 6961 626c 6573 5b22 6475 6d6d 7933 225d  iables["dummy3"]
+00009660: 2e73 6861 7065 203d 3d20 2830 2c20 3329  .shape == (0, 3)
+00009670: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00009680: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
+00009690: 6d79 5822 5d2e 7368 6170 6520 3d3d 2028  myX"].shape == (
+000096a0: 302c 2033 2c20 3029 0a20 2020 2020 2020  0, 3, 0).       
+000096b0: 2061 7373 6572 7420 672e 7661 7269 6162   assert g.variab
+000096c0: 6c65 735b 2264 756d 6d79 3422 5d2e 7368  les["dummy4"].sh
+000096d0: 6170 6520 3d3d 2028 332c 2030 2c20 3029  ape == (3, 0, 0)
+000096e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000096f0: 672e 7661 7269 6162 6c65 735b 2264 756d  g.variables["dum
+00009700: 6d79 3522 5d2e 7368 6170 6520 3d3d 2028  my5"].shape == (
+00009710: 332c 2033 290a 0a20 2020 2020 2020 2023  3, 3)..        #
+00009720: 2072 6573 697a 6520 6469 6d65 6e73 696f   resize dimensio
+00009730: 6e73 2061 6e64 2061 6c6c 2063 6f6e 6e65  ns and all conne
+00009740: 6374 6564 2076 6172 6961 626c 6573 0a20  cted variables. 
+00009750: 2020 2020 2020 2066 2e72 6573 697a 655f         f.resize_
+00009760: 6469 6d65 6e73 696f 6e28 2278 222c 2032  dimension("x", 2
+00009770: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00009780: 2066 2e76 6172 6961 626c 6573 5b22 6475   f.variables["du
+00009790: 6d6d 7931 225d 2e73 6861 7065 203d 3d20  mmy1"].shape == 
+000097a0: 2832 2c20 3329 0a20 2020 2020 2020 2061  (2, 3).        a
+000097b0: 7373 6572 7420 662e 7661 7269 6162 6c65  ssert f.variable
+000097c0: 735b 2264 756d 6d79 3222 5d2e 7368 6170  s["dummy2"].shap
+000097d0: 6520 3d3d 2028 322c 2033 290a 2020 2020  e == (2, 3).    
+000097e0: 2020 2020 6173 7365 7274 2066 2e76 6172      assert f.var
+000097f0: 6961 626c 6573 5b22 6475 6d6d 7933 225d  iables["dummy3"]
+00009800: 2e73 6861 7065 203d 3d20 2832 2c20 3329  .shape == (2, 3)
+00009810: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00009820: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
+00009830: 6d79 5822 5d2e 7368 6170 6520 3d3d 2028  myX"].shape == (
+00009840: 322c 2033 2c20 3029 0a20 2020 2020 2020  2, 3, 0).       
+00009850: 2061 7373 6572 7420 672e 7661 7269 6162   assert g.variab
+00009860: 6c65 735b 2264 756d 6d79 3422 5d2e 7368  les["dummy4"].sh
+00009870: 6170 6520 3d3d 2028 332c 2032 2c20 3229  ape == (3, 2, 2)
+00009880: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00009890: 672e 7661 7269 6162 6c65 735b 2264 756d  g.variables["dum
+000098a0: 6d79 3522 5d2e 7368 6170 6520 3d3d 2028  my5"].shape == (
+000098b0: 332c 2033 290a 0a20 2020 2020 2020 2023  3, 3)..        #
+000098c0: 2062 726f 6164 6361 7374 2077 7269 7469   broadcast writi
+000098d0: 6e67 0a20 2020 2020 2020 2069 6620 746d  ng.        if tm
+000098e0: 705f 6c6f 6361 6c5f 6f72 5f72 656d 6f74  p_local_or_remot
+000098f0: 655f 6e65 7463 6466 2e73 7461 7274 7377  e_netcdf.startsw
+00009900: 6974 6828 7265 6d6f 7465 5f68 3529 3a0a  ith(remote_h5):.
+00009910: 2020 2020 2020 2020 2020 2020 6578 7065              expe
+00009920: 6374 6564 5f65 7272 6f72 7320 3d20 7079  cted_errors = py
+00009930: 7465 7374 2e72 6169 7365 7328 4f53 4572  test.raises(OSEr
+00009940: 726f 7229 0a20 2020 2020 2020 2065 6c73  ror).        els
+00009950: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00009960: 2057 6520 646f 6e27 7420 6578 7065 6374   We don't expect
+00009970: 2061 6e79 2065 7272 6f72 732e 2054 6869   any errors. Thi
+00009980: 7320 6973 2065 6666 6563 7469 7665 6c79  s is effectively
+00009990: 2061 2076 6f69 6420 636f 6e74 6578 7420   a void context 
+000099a0: 6d61 6e61 6765 720a 2020 2020 2020 2020  manager.        
+000099b0: 2020 2020 6578 7065 6374 6564 5f65 7272      expected_err
+000099c0: 6f72 7320 3d20 6d65 6d6f 7279 7669 6577  ors = memoryview
+000099d0: 2862 2222 290a 2020 2020 2020 2020 7769  (b"").        wi
+000099e0: 7468 2065 7870 6563 7465 645f 6572 726f  th expected_erro
+000099f0: 7273 2061 7320 653a 0a20 2020 2020 2020  rs as e:.       
+00009a00: 2020 2020 2066 2e76 6172 6961 626c 6573       f.variables
+00009a10: 5b22 6475 6d6d 7933 225d 5b2e 2e2e 5d20  ["dummy3"][...] 
+00009a20: 3d20 5b5b 312c 2032 2c20 335d 5d0a 2020  = [[1, 2, 3]].  
+00009a30: 2020 2020 2020 2020 2020 6e70 2e74 6573            np.tes
+00009a40: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
+00009a50: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
+00009a60: 5b22 6475 6d6d 7933 225d 2c20 5b5b 312c  ["dummy3"], [[1,
+00009a70: 2032 2c20 335d 2c20 5b31 2c20 322c 2033   2, 3], [1, 2, 3
+00009a80: 5d5d 290a 2020 2020 2020 2020 6966 2074  ]]).        if t
+00009a90: 6d70 5f6c 6f63 616c 5f6f 725f 7265 6d6f  mp_local_or_remo
+00009aa0: 7465 5f6e 6574 6364 662e 7374 6172 7473  te_netcdf.starts
+00009ab0: 7769 7468 2872 656d 6f74 655f 6835 293a  with(remote_h5):
+00009ac0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00009ad0: 6572 7420 2247 6f74 2061 7379 6e63 696f  ert "Got asyncio
+00009ae0: 2e49 6e63 6f6d 706c 6574 6552 6561 6445  .IncompleteReadE
+00009af0: 7272 6f72 2220 696e 2065 2e76 616c 7565  rror" in e.value
+00009b00: 2e61 7267 735b 305d 0a0a 0a64 6566 2074  .args[0]...def t
+00009b10: 6573 745f 635f 6170 695f 6361 6e5f 7265  est_c_api_can_re
+00009b20: 6164 5f75 6e6c 696d 6974 6564 5f64 696d  ad_unlimited_dim
+00009b30: 656e 7369 6f6e 7328 746d 705f 6c6f 6361  ensions(tmp_loca
+00009b40: 6c5f 6e65 7463 6466 293a 0a20 2020 2077  l_netcdf):.    w
+00009b50: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
+00009b60: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
+00009b70: 6466 2c20 2277 2229 2061 7320 663a 0a20  df, "w") as f:. 
+00009b80: 2020 2020 2020 2023 2054 6872 6565 2064         # Three d
+00009b90: 696d 656e 7369 6f6e 732c 206f 6e6c 7920  imensions, only 
+00009ba0: 6f6e 6520 6973 206c 696d 6974 6564 2e0a  one is limited..
+00009bb0: 2020 2020 2020 2020 662e 6469 6d65 6e73          f.dimens
+00009bc0: 696f 6e73 5b22 7822 5d20 3d20 4e6f 6e65  ions["x"] = None
+00009bd0: 0a20 2020 2020 2020 2066 2e64 696d 656e  .        f.dimen
+00009be0: 7369 6f6e 735b 2279 225d 203d 2033 0a20  sions["y"] = 3. 
+00009bf0: 2020 2020 2020 2066 2e64 696d 656e 7369         f.dimensi
+00009c00: 6f6e 735b 227a 225d 203d 204e 6f6e 650a  ons["z"] = None.
+00009c10: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
+00009c20: 5f76 6172 6961 626c 6528 2264 756d 6d79  _variable("dummy
+00009c30: 3122 2c20 6469 6d65 6e73 696f 6e73 3d28  1", dimensions=(
+00009c40: 2278 222c 2022 7922 292c 2064 7479 7065  "x", "y"), dtype
+00009c50: 3d6e 702e 696e 7436 3429 0a20 2020 2020  =np.int64).     
+00009c60: 2020 2066 2e63 7265 6174 655f 7661 7269     f.create_vari
+00009c70: 6162 6c65 2822 6475 6d6d 7932 222c 2064  able("dummy2", d
+00009c80: 696d 656e 7369 6f6e 733d 2822 7922 2c20  imensions=("y", 
+00009c90: 2278 222c 2022 7822 292c 2064 7479 7065  "x", "x"), dtype
+00009ca0: 3d6e 702e 696e 7436 3429 0a20 2020 2020  =np.int64).     
+00009cb0: 2020 2067 203d 2066 2e63 7265 6174 655f     g = f.create_
+00009cc0: 6772 6f75 7028 2274 6573 7422 290a 2020  group("test").  
+00009cd0: 2020 2020 2020 672e 6372 6561 7465 5f76        g.create_v
+00009ce0: 6172 6961 626c 6528 2264 756d 6d79 3322  ariable("dummy3"
+00009cf0: 2c20 6469 6d65 6e73 696f 6e73 3d28 2279  , dimensions=("y
+00009d00: 222c 2022 7922 292c 2064 7479 7065 3d6e  ", "y"), dtype=n
+00009d10: 702e 696e 7436 3429 0a20 2020 2020 2020  p.int64).       
+00009d20: 2067 2e63 7265 6174 655f 7661 7269 6162   g.create_variab
+00009d30: 6c65 2822 6475 6d6d 7934 222c 2064 696d  le("dummy4", dim
+00009d40: 656e 7369 6f6e 733d 2822 7a22 2c20 227a  ensions=("z", "z
+00009d50: 2229 2c20 6474 7970 653d 6e70 2e69 6e74  "), dtype=np.int
+00009d60: 3634 290a 2020 2020 2020 2020 662e 7265  64).        f.re
+00009d70: 7369 7a65 5f64 696d 656e 7369 6f6e 2822  size_dimension("
+00009d80: 7822 2c20 3229 0a0a 2020 2020 7769 7468  x", 2)..    with
+00009d90: 206e 6574 4344 4634 2e44 6174 6173 6574   netCDF4.Dataset
+00009da0: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+00009db0: 662c 2022 7222 2920 6173 2066 3a0a 2020  f, "r") as f:.  
+00009dc0: 2020 2020 2020 6173 7365 7274 2066 2e64        assert f.d
+00009dd0: 696d 656e 7369 6f6e 735b 2278 225d 2e73  imensions["x"].s
+00009de0: 697a 6520 3d3d 2032 0a20 2020 2020 2020  ize == 2.       
+00009df0: 2061 7373 6572 7420 662e 6469 6d65 6e73   assert f.dimens
+00009e00: 696f 6e73 5b22 7822 5d2e 6973 756e 6c69  ions["x"].isunli
+00009e10: 6d69 7465 6428 2920 6973 2054 7275 650a  mited() is True.
+00009e20: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+00009e30: 2e64 696d 656e 7369 6f6e 735b 2279 225d  .dimensions["y"]
+00009e40: 2e73 697a 6520 3d3d 2033 0a20 2020 2020  .size == 3.     
+00009e50: 2020 2061 7373 6572 7420 662e 6469 6d65     assert f.dime
+00009e60: 6e73 696f 6e73 5b22 7922 5d2e 6973 756e  nsions["y"].isun
+00009e70: 6c69 6d69 7465 6428 2920 6973 2046 616c  limited() is Fal
+00009e80: 7365 0a20 2020 2020 2020 2061 7373 6572  se.        asser
+00009e90: 7420 662e 6469 6d65 6e73 696f 6e73 5b22  t f.dimensions["
+00009ea0: 7a22 5d2e 7369 7a65 203d 3d20 300a 2020  z"].size == 0.  
+00009eb0: 2020 2020 2020 6173 7365 7274 2066 2e64        assert f.d
+00009ec0: 696d 656e 7369 6f6e 735b 227a 225d 2e69  imensions["z"].i
+00009ed0: 7375 6e6c 696d 6974 6564 2829 2069 7320  sunlimited() is 
+00009ee0: 5472 7565 0a0a 2020 2020 2020 2020 6173  True..        as
+00009ef0: 7365 7274 2066 2e76 6172 6961 626c 6573  sert f.variables
+00009f00: 5b22 6475 6d6d 7931 225d 2e73 6861 7065  ["dummy1"].shape
+00009f10: 203d 3d20 2832 2c20 3329 0a20 2020 2020   == (2, 3).     
+00009f20: 2020 2061 7373 6572 7420 662e 7661 7269     assert f.vari
+00009f30: 6162 6c65 735b 2264 756d 6d79 3222 5d2e  ables["dummy2"].
+00009f40: 7368 6170 6520 3d3d 2028 332c 2032 2c20  shape == (3, 2, 
+00009f50: 3229 0a20 2020 2020 2020 2067 203d 2066  2).        g = f
+00009f60: 2e67 726f 7570 735b 2274 6573 7422 5d0a  .groups["test"].
+00009f70: 2020 2020 2020 2020 6173 7365 7274 2067          assert g
+00009f80: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
+00009f90: 7933 225d 2e73 6861 7065 203d 3d20 2833  y3"].shape == (3
+00009fa0: 2c20 3329 0a20 2020 2020 2020 2061 7373  , 3).        ass
+00009fb0: 6572 7420 672e 7661 7269 6162 6c65 735b  ert g.variables[
+00009fc0: 2264 756d 6d79 3422 5d2e 7368 6170 6520  "dummy4"].shape 
+00009fd0: 3d3d 2028 302c 2030 290a 0a0a 6465 6620  == (0, 0)...def 
+00009fe0: 7465 7374 5f72 6561 6469 6e67 5f75 6e6c  test_reading_unl
+00009ff0: 696d 6974 6564 5f64 696d 656e 7369 6f6e  imited_dimension
+0000a000: 735f 6372 6561 7465 645f 7769 7468 5f63  s_created_with_c
+0000a010: 5f61 7069 2874 6d70 5f6c 6f63 616c 5f6e  _api(tmp_local_n
+0000a020: 6574 6364 6629 3a0a 2020 2020 7769 7468  etcdf):.    with
+0000a030: 206e 6574 4344 4634 2e44 6174 6173 6574   netCDF4.Dataset
+0000a040: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000a050: 662c 2022 7722 2920 6173 2066 3a0a 2020  f, "w") as f:.  
+0000a060: 2020 2020 2020 662e 6372 6561 7465 4469        f.createDi
+0000a070: 6d65 6e73 696f 6e28 2278 222c 204e 6f6e  mension("x", Non
+0000a080: 6529 0a20 2020 2020 2020 2066 2e63 7265  e).        f.cre
+0000a090: 6174 6544 696d 656e 7369 6f6e 2822 7922  ateDimension("y"
+0000a0a0: 2c20 3329 0a20 2020 2020 2020 2066 2e63  , 3).        f.c
+0000a0b0: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
+0000a0c0: 7a22 2c20 4e6f 6e65 290a 0a20 2020 2020  z", None)..     
+0000a0d0: 2020 2064 756d 6d79 3120 3d20 662e 6372     dummy1 = f.cr
+0000a0e0: 6561 7465 5661 7269 6162 6c65 2822 6475  eateVariable("du
+0000a0f0: 6d6d 7931 222c 2066 6c6f 6174 2c20 2822  mmy1", float, ("
+0000a100: 7822 2c20 2279 2229 290a 2020 2020 2020  x", "y")).      
+0000a110: 2020 662e 6372 6561 7465 5661 7269 6162    f.createVariab
+0000a120: 6c65 2822 6475 6d6d 7932 222c 2066 6c6f  le("dummy2", flo
+0000a130: 6174 2c20 2822 7922 2c20 2278 222c 2022  at, ("y", "x", "
+0000a140: 7822 2929 0a20 2020 2020 2020 2067 203d  x")).        g =
+0000a150: 2066 2e63 7265 6174 6547 726f 7570 2822   f.createGroup("
+0000a160: 7465 7374 2229 0a20 2020 2020 2020 2067  test").        g
+0000a170: 2e63 7265 6174 6556 6172 6961 626c 6528  .createVariable(
+0000a180: 2264 756d 6d79 3322 2c20 666c 6f61 742c  "dummy3", float,
+0000a190: 2028 2279 222c 2022 7922 2929 0a20 2020   ("y", "y")).   
+0000a1a0: 2020 2020 2067 2e63 7265 6174 6556 6172       g.createVar
+0000a1b0: 6961 626c 6528 2264 756d 6d79 3422 2c20  iable("dummy4", 
+0000a1c0: 666c 6f61 742c 2028 227a 222c 2022 7a22  float, ("z", "z"
+0000a1d0: 2929 0a0a 2020 2020 2020 2020 2320 4173  ))..        # As
+0000a1e0: 7369 676e 2073 6f6d 6574 6869 6e67 2074  sign something t
+0000a1f0: 6f20 7472 6967 6765 7220 6120 7265 7369  o trigger a resi
+0000a200: 7a65 2e0a 2020 2020 2020 2020 6475 6d6d  ze..        dumm
+0000a210: 7931 5b3a 5d20 3d20 5b5b 312c 2032 2c20  y1[:] = [[1, 2, 
+0000a220: 335d 2c20 5b34 2c20 352c 2036 5d5d 0a0a  3], [4, 5, 6]]..
+0000a230: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+0000a240: 2061 6e6f 7468 6572 2076 6172 6961 626c   another variabl
+0000a250: 6520 7769 7468 2073 616d 6520 6469 6d65  e with same dime
+0000a260: 6e73 696f 6e73 0a20 2020 2020 2020 2066  nsions.        f
+0000a270: 2e63 7265 6174 6556 6172 6961 626c 6528  .createVariable(
+0000a280: 2264 756d 6d79 3522 2c20 666c 6f61 742c  "dummy5", float,
+0000a290: 2028 2278 222c 2022 7922 2929 0a0a 2020   ("x", "y"))..  
+0000a2a0: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+0000a2b0: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
+0000a2c0: 6574 6364 662c 2022 7222 2920 6173 2066  etcdf, "r") as f
+0000a2d0: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+0000a2e0: 2066 2e64 696d 656e 7369 6f6e 735b 2278   f.dimensions["x
+0000a2f0: 225d 2e69 7375 6e6c 696d 6974 6564 2829  "].isunlimited()
+0000a300: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000a310: 662e 6469 6d65 6e73 696f 6e73 5b22 7922  f.dimensions["y"
+0000a320: 5d2e 7369 7a65 203d 3d20 330a 2020 2020  ].size == 3.    
+0000a330: 2020 2020 6173 7365 7274 2066 2e64 696d      assert f.dim
+0000a340: 656e 7369 6f6e 735b 227a 225d 2e69 7375  ensions["z"].isu
+0000a350: 6e6c 696d 6974 6564 2829 0a0a 2020 2020  nlimited()..    
+0000a360: 2020 2020 2320 5468 6973 2069 7320 7061      # This is pa
+0000a370: 7273 6564 2063 6f72 7265 6374 6c79 2064  rsed correctly d
+0000a380: 7565 2074 6f20 6835 6e65 7463 6466 2773  ue to h5netcdf's
+0000a390: 2069 6e69 7420 7472 6963 6b65 7279 2e0a   init trickery..
+0000a3a0: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+0000a3b0: 2e64 696d 656e 7369 6f6e 735b 2278 225d  .dimensions["x"]
+0000a3c0: 2e73 697a 6520 3d3d 2032 0a20 2020 2020  .size == 2.     
+0000a3d0: 2020 2061 7373 6572 7420 662e 6469 6d65     assert f.dime
+0000a3e0: 6e73 696f 6e73 5b22 7922 5d2e 7369 7a65  nsions["y"].size
+0000a3f0: 203d 3d20 330a 2020 2020 2020 2020 6173   == 3.        as
+0000a400: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
+0000a410: 735b 227a 225d 2e73 697a 6520 3d3d 2030  s["z"].size == 0
+0000a420: 0a0a 2020 2020 2020 2020 2320 4275 7420  ..        # But 
+0000a430: 7468 6520 6163 7475 616c 2064 6174 612d  the actual data-
+0000a440: 7365 7420 616e 6420 6172 7261 7973 2061  set and arrays a
+0000a450: 7265 206e 6f74 2063 6f72 7265 6374 2e0a  re not correct..
+0000a460: 2020 2020 2020 2020 2320 6173 7365 7274          # assert
+0000a470: 2066 5b22 6475 6d6d 7931 225d 2e73 6861   f["dummy1"].sha
+0000a480: 7065 203d 3d20 2832 2c20 3329 0a20 2020  pe == (2, 3).   
+0000a490: 2020 2020 2023 2058 5858 3a20 5468 6973       # XXX: This
+0000a4a0: 2061 7272 6179 2068 6173 2073 6f6d 6520   array has some 
+0000a4b0: 6461 7461 2077 6974 6820 6469 6d65 6e73  data with dimens
+0000a4c0: 696f 6e20 7820 2d20 6e65 7463 6466 2064  ion x - netcdf d
+0000a4d0: 6f65 7320 6e6f 740a 2020 2020 2020 2020  oes not.        
+0000a4e0: 2320 6170 7065 6172 2074 6f20 6b65 6570  # appear to keep
+0000a4f0: 2064 696d 656e 7369 6f6e 7320 636f 6e73   dimensions cons
+0000a500: 6973 7465 6e74 2e0a 2020 2020 2020 2020  istent..        
+0000a510: 2320 5769 7468 2068 7474 7073 3a2f 2f67  # With https://g
+0000a520: 6974 6875 622e 636f 6d2f 6835 6e65 7463  ithub.com/h5netc
+0000a530: 6466 2f68 356e 6574 6364 662f 7075 6c6c  df/h5netcdf/pull
+0000a540: 2f31 3033 2068 356e 6574 6364 6620 7769  /103 h5netcdf wi
+0000a550: 6c6c 0a20 2020 2020 2020 2023 2072 6574  ll.        # ret
+0000a560: 7572 6e20 6120 7061 6464 6564 2061 7272  urn a padded arr
+0000a570: 6179 0a20 2020 2020 2020 2061 7373 6572  ay.        asser
+0000a580: 7420 665b 2264 756d 6d79 3222 5d2e 7368  t f["dummy2"].sh
+0000a590: 6170 6520 3d3d 2028 332c 2032 2c20 3229  ape == (3, 2, 2)
+0000a5a0: 0a20 2020 2020 2020 2066 2e67 726f 7570  .        f.group
+0000a5b0: 735b 2274 6573 7422 5d5b 2264 756d 6d79  s["test"]["dummy
+0000a5c0: 3322 5d2e 7368 6170 6520 3d3d 2028 332c  3"].shape == (3,
+0000a5d0: 2033 290a 2020 2020 2020 2020 662e 6772   3).        f.gr
+0000a5e0: 6f75 7073 5b22 7465 7374 225d 5b22 6475  oups["test"]["du
+0000a5f0: 6d6d 7934 225d 2e73 6861 7065 203d 3d20  mmy4"].shape == 
+0000a600: 2830 2c20 3029 0a20 2020 2020 2020 2061  (0, 0).        a
+0000a610: 7373 6572 7420 665b 2264 756d 6d79 3522  ssert f["dummy5"
+0000a620: 5d2e 7368 6170 6520 3d3d 2028 322c 2033  ].shape == (2, 3
+0000a630: 290a 0a0a 6465 6620 7465 7374 5f72 6561  )...def test_rea
+0000a640: 6469 6e67 5f75 6e75 7365 645f 756e 6c69  ding_unused_unli
+0000a650: 6d69 7465 645f 6469 6d65 6e73 696f 6e28  mited_dimension(
+0000a660: 746d 705f 6c6f 6361 6c5f 6f72 5f72 656d  tmp_local_or_rem
+0000a670: 6f74 655f 6e65 7463 6466 293a 0a20 2020  ote_netcdf):.   
+0000a680: 2022 2222 5465 7374 2072 6561 6469 6e67   """Test reading
+0000a690: 2061 2066 696c 6520 7769 7468 2075 6e75   a file with unu
+0000a6a0: 7365 6420 6469 6d65 6e73 696f 6e20 6f66  sed dimension of
+0000a6b0: 2075 6e6c 696d 6974 6564 2073 697a 6522   unlimited size"
+0000a6c0: 2222 0a20 2020 2077 6974 6820 6835 6e65  "".    with h5ne
+0000a6d0: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+0000a6e0: 6361 6c5f 6f72 5f72 656d 6f74 655f 6e65  cal_or_remote_ne
+0000a6f0: 7463 6466 2c20 2277 2229 2061 7320 663a  tcdf, "w") as f:
+0000a700: 0a20 2020 2020 2020 2066 2e64 696d 656e  .        f.dimen
+0000a710: 7369 6f6e 7320 3d20 7b22 7822 3a20 4e6f  sions = {"x": No
+0000a720: 6e65 7d0a 2020 2020 2020 2020 662e 7265  ne}.        f.re
+0000a730: 7369 7a65 5f64 696d 656e 7369 6f6e 2822  size_dimension("
+0000a740: 7822 2c20 3529 0a20 2020 2020 2020 2061  x", 5).        a
+0000a750: 7373 6572 7420 662e 6469 6d65 6e73 696f  ssert f.dimensio
+0000a760: 6e73 5b22 7822 5d2e 6973 756e 6c69 6d69  ns["x"].isunlimi
+0000a770: 7465 6428 290a 2020 2020 2020 2020 6173  ted().        as
+0000a780: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
+0000a790: 735b 2278 225d 2e73 697a 6520 3d3d 2035  s["x"].size == 5
+0000a7a0: 0a0a 0a64 6566 2074 6573 745f 7265 6164  ...def test_read
+0000a7b0: 696e 675f 7370 6563 6961 6c5f 6461 7461  ing_special_data
+0000a7c0: 7479 7065 5f63 7265 6174 6564 5f77 6974  type_created_wit
+0000a7d0: 685f 635f 6170 6928 746d 705f 6c6f 6361  h_c_api(tmp_loca
+0000a7e0: 6c5f 6e65 7463 6466 293a 0a20 2020 2022  l_netcdf):.    "
+0000a7f0: 2222 5465 7374 2072 6561 6469 6e67 2061  ""Test reading a
+0000a800: 2066 696c 6520 7769 7468 2075 6e73 7570   file with unsup
+0000a810: 706f 7274 6564 2044 6174 6174 7970 6522  ported Datatype"
+0000a820: 2222 0a20 2020 2077 6974 6820 6e65 7443  "".    with netC
+0000a830: 4446 342e 4461 7461 7365 7428 746d 705f  DF4.Dataset(tmp_
+0000a840: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2277  local_netcdf, "w
+0000a850: 2229 2061 7320 663a 0a20 2020 2020 2020  ") as f:.       
+0000a860: 2063 6f6d 706c 6578 3132 3820 3d20 6e70   complex128 = np
+0000a870: 2e64 7479 7065 285b 2822 7265 616c 222c  .dtype([("real",
+0000a880: 206e 702e 666c 6f61 7436 3429 2c20 2822   np.float64), ("
+0000a890: 696d 6167 222c 206e 702e 666c 6f61 7436  imag", np.float6
+0000a8a0: 3429 5d29 0a20 2020 2020 2020 2066 2e63  4)]).        f.c
+0000a8b0: 7265 6174 6543 6f6d 706f 756e 6454 7970  reateCompoundTyp
+0000a8c0: 6528 636f 6d70 6c65 7831 3238 2c20 2263  e(complex128, "c
+0000a8d0: 6f6d 706c 6578 3132 3822 290a 2020 2020  omplex128").    
+0000a8e0: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+0000a8f0: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+0000a900: 6364 662c 2022 7222 2920 6173 2066 3a0a  cdf, "r") as f:.
+0000a910: 2020 2020 2020 2020 7061 7373 0a0a 0a64          pass...d
+0000a920: 6566 2074 6573 745f 6e63 345f 6e6f 6e5f  ef test_nc4_non_
+0000a930: 636f 6f72 6428 746d 705f 6c6f 6361 6c5f  coord(tmp_local_
+0000a940: 6e65 7463 6466 293a 0a20 2020 2023 2048  netcdf):.    # H
+0000a950: 6572 6520 7765 2067 656e 6572 6174 6520  ere we generate 
+0000a960: 6120 6665 7720 7661 7269 6162 6c65 7320  a few variables 
+0000a970: 616e 6420 636f 6f72 6469 6e61 7465 730a  and coordinates.
+0000a980: 2020 2020 2320 5468 6520 6465 6661 756c      # The defaul
+0000a990: 7420 7368 6f75 6c64 2062 6520 746f 2074  t should be to t
+0000a9a0: 7261 636b 2074 6865 206f 7264 6572 206f  rack the order o
+0000a9b0: 6620 6372 6561 7469 6f6e 0a20 2020 2023  f creation.    #
+0000a9c0: 2054 6875 732c 206f 6e20 7265 6f70 656e   Thus, on reopen
+0000a9d0: 696e 6720 7468 6520 6669 6c65 2c20 7468  ing the file, th
+0000a9e0: 6520 6f72 6465 7220 696e 2077 6869 6368  e order in which
+0000a9f0: 0a20 2020 2023 2074 6865 2076 6172 6961  .    # the varia
+0000aa00: 626c 6573 2061 7265 206c 6973 7465 6420  bles are listed 
+0000aa10: 7368 6f75 6c64 2062 6520 6d61 696e 7461  should be mainta
+0000aa20: 696e 6564 0a20 2020 2023 2079 2020 202d  ined.    # y   -
+0000aa30: 2d20 2020 7265 6665 7273 2074 6f20 7468  -   refers to th
+0000aa40: 6520 636f 6f72 6469 6e61 7465 2079 0a20  e coordinate y. 
+0000aa50: 2020 2023 205f 6e63 345f 6e6f 6e5f 636f     # _nc4_non_co
+0000aa60: 6f72 645f 7920 202d 2d20 2072 6566 6572  ord_y  --  refer
+0000aa70: 7320 746f 2074 6865 2064 6174 6120 790a  s to the data y.
+0000aa80: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
+0000aa90: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
+0000aaa0: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
+0000aab0: 2066 3a0a 2020 2020 2020 2020 662e 6469   f:.        f.di
+0000aac0: 6d65 6e73 696f 6e73 203d 207b 2278 223a  mensions = {"x":
+0000aad0: 204e 6f6e 652c 2022 7922 3a20 327d 0a20   None, "y": 2}. 
+0000aae0: 2020 2020 2020 2066 2e63 7265 6174 655f         f.create_
+0000aaf0: 7661 7269 6162 6c65 2822 7465 7374 222c  variable("test",
+0000ab00: 2064 696d 656e 7369 6f6e 733d 2822 7822   dimensions=("x"
+0000ab10: 2c29 2c20 6474 7970 653d 6e70 2e69 6e74  ,), dtype=np.int
+0000ab20: 3634 290a 2020 2020 2020 2020 662e 6372  64).        f.cr
+0000ab30: 6561 7465 5f76 6172 6961 626c 6528 2279  eate_variable("y
+0000ab40: 222c 2064 696d 656e 7369 6f6e 733d 2822  ", dimensions=("
+0000ab50: 7822 2c29 2c20 6474 7970 653d 6e70 2e69  x",), dtype=np.i
+0000ab60: 6e74 3634 290a 0a20 2020 2077 6974 6820  nt64)..    with 
+0000ab70: 6835 6e65 7463 6466 2e46 696c 6528 746d  h5netcdf.File(tm
+0000ab80: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
+0000ab90: 2272 2229 2061 7320 663a 0a20 2020 2020  "r") as f:.     
+0000aba0: 2020 2061 7373 6572 7420 6c69 7374 2866     assert list(f
+0000abb0: 2e64 696d 656e 7369 6f6e 7329 203d 3d20  .dimensions) == 
+0000abc0: 5b22 7822 2c20 2279 225d 0a20 2020 2020  ["x", "y"].     
+0000abd0: 2020 2061 7373 6572 7420 662e 6469 6d65     assert f.dime
+0000abe0: 6e73 696f 6e73 5b22 7822 5d2e 7369 7a65  nsions["x"].size
+0000abf0: 203d 3d20 300a 2020 2020 2020 2020 6173   == 0.        as
 0000ac00: 7365 7274 2066 2e64 696d 656e 7369 6f6e  sert f.dimension
-0000ac10: 735b 2279 225d 2e73 697a 6520 3d3d 2032  s["y"].size == 2
-0000ac20: 0a20 2020 2020 2020 2069 6620 7665 7273  .        if vers
-0000ac30: 696f 6e2e 7061 7273 6528 6835 7079 2e5f  ion.parse(h5py._
-0000ac40: 5f76 6572 7369 6f6e 5f5f 2920 3e3d 2076  _version__) >= v
-0000ac50: 6572 7369 6f6e 2e70 6172 7365 2822 332e  ersion.parse("3.
-0000ac60: 372e 3022 293a 0a20 2020 2020 2020 2020  7.0"):.         
-0000ac70: 2020 2061 7373 6572 7420 6c69 7374 2866     assert list(f
-0000ac80: 2e76 6172 6961 626c 6573 2920 3d3d 205b  .variables) == [
-0000ac90: 2279 222c 2022 7465 7374 225d 0a20 2020  "y", "test"].   
-0000aca0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000acb0: 6c69 7374 2866 2e5f 6835 6772 6f75 702e  list(f._h5group.
-0000acc0: 6b65 7973 2829 2920 3d3d 205b 2278 222c  keys()) == ["x",
-0000acd0: 2022 7922 2c20 225f 6e63 345f 6e6f 6e5f   "y", "_nc4_non_
-0000ace0: 636f 6f72 645f 7922 2c20 2274 6573 7422  coord_y", "test"
-0000acf0: 5d0a 0a0a 6465 6620 7465 7374 5f6f 7665  ]...def test_ove
-0000ad00: 7277 7269 7465 5f65 7869 7374 696e 675f  rwrite_existing_
-0000ad10: 6669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  file(tmp_local_n
-0000ad20: 6574 6364 6629 3a0a 2020 2020 2320 6372  etcdf):.    # cr
-0000ad30: 6561 7465 2066 696c 6520 7769 7468 205f  eate file with _
-0000ad40: 4e43 5072 6f70 6572 7469 6573 2061 7474  NCProperties att
-0000ad50: 7269 6275 7465 0a20 2020 2077 6974 6820  ribute.    with 
-0000ad60: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
-0000ad70: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000ad80: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
-0000ad90: 2020 2020 2020 6473 2e63 7265 6174 6544        ds.createD
-0000ada0: 696d 656e 7369 6f6e 2822 7822 2c20 3130  imension("x", 10
-0000adb0: 290a 0a20 2020 2023 2063 6865 636b 2061  )..    # check a
-0000adc0: 7474 7269 6275 7465 0a20 2020 2077 6974  ttribute.    wit
-0000add0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-0000ade0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000adf0: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
-0000ae00: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-0000ae10: 6174 7472 732e 5f68 3561 7474 7273 2e67  attrs._h5attrs.g
-0000ae20: 6574 2822 5f4e 4350 726f 7065 7274 6965  et("_NCPropertie
-0000ae30: 7322 2c20 4661 6c73 6529 0a0a 2020 2020  s", False)..    
-0000ae40: 2320 6f76 6572 7772 6974 6520 6669 6c65  # overwrite file
-0000ae50: 2077 6974 6820 6c65 6761 6379 6170 690a   with legacyapi.
-0000ae60: 2020 2020 7769 7468 206c 6567 6163 7961      with legacya
-0000ae70: 7069 2e44 6174 6173 6574 2874 6d70 5f6c  pi.Dataset(tmp_l
-0000ae80: 6f63 616c 5f6e 6574 6364 662c 2022 7722  ocal_netcdf, "w"
-0000ae90: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-0000aea0: 2064 732e 6372 6561 7465 4469 6d65 6e73   ds.createDimens
-0000aeb0: 696f 6e28 2278 222c 2031 3029 0a0a 2020  ion("x", 10)..  
-0000aec0: 2020 2320 6368 6563 6b20 6174 7472 6962    # check attrib
-0000aed0: 7574 650a 2020 2020 7769 7468 2068 356e  ute.    with h5n
-0000aee0: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
-0000aef0: 6f63 616c 5f6e 6574 6364 662c 2022 7222  ocal_netcdf, "r"
-0000af00: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-0000af10: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
-0000af20: 2e5f 6835 6174 7472 732e 6765 7428 225f  ._h5attrs.get("_
-0000af30: 4e43 5072 6f70 6572 7469 6573 222c 2046  NCProperties", F
-0000af40: 616c 7365 290a 0a20 2020 2023 206f 7665  alse)..    # ove
-0000af50: 7277 7269 7465 2066 696c 6520 7769 7468  rwrite file with
-0000af60: 206e 6577 2061 7069 0a20 2020 2077 6974   new api.    wit
-0000af70: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-0000af80: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000af90: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
-0000afa0: 2020 2020 2020 6473 2e64 696d 656e 7369        ds.dimensi
-0000afb0: 6f6e 735b 2278 225d 203d 2031 300a 0a20  ons["x"] = 10.. 
-0000afc0: 2020 2023 2063 6865 636b 2061 7474 7269     # check attri
-0000afd0: 6275 7465 0a20 2020 2077 6974 6820 6835  bute.    with h5
-0000afe0: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
-0000aff0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
-0000b000: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
-0000b010: 2020 6173 7365 7274 2064 732e 6174 7472    assert ds.attr
-0000b020: 732e 5f68 3561 7474 7273 2e67 6574 2822  s._h5attrs.get("
-0000b030: 5f4e 4350 726f 7065 7274 6965 7322 2c20  _NCProperties", 
-0000b040: 4661 6c73 6529 0a0a 0a64 6566 2074 6573  False)...def tes
-0000b050: 745f 7363 616c 6573 5f6f 6e5f 6170 7065  t_scales_on_appe
-0000b060: 6e64 2874 6d70 5f6c 6f63 616c 5f6e 6574  nd(tmp_local_net
-0000b070: 6364 6629 3a0a 2020 2020 2320 6372 6561  cdf):.    # crea
-0000b080: 7465 2066 696c 6520 7769 7468 205f 4e43  te file with _NC
-0000b090: 5072 6f70 6572 7469 6573 2061 7474 7269  Properties attri
-0000b0a0: 6275 7465 0a20 2020 2077 6974 6820 6e65  bute.    with ne
-0000b0b0: 7443 4446 342e 4461 7461 7365 7428 746d  tCDF4.Dataset(tm
-0000b0c0: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-0000b0d0: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
-0000b0e0: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-0000b0f0: 656e 7369 6f6e 2822 7822 2c20 3130 290a  ension("x", 10).
-0000b100: 0a20 2020 2023 2061 7070 656e 6420 6669  .    # append fi
-0000b110: 6c65 2077 6974 6820 6e65 7443 4446 340a  le with netCDF4.
-0000b120: 2020 2020 7769 7468 206e 6574 4344 4634      with netCDF4
-0000b130: 2e44 6174 6173 6574 2874 6d70 5f6c 6f63  .Dataset(tmp_loc
-0000b140: 616c 5f6e 6574 6364 662c 2022 722b 2229  al_netcdf, "r+")
-0000b150: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-0000b160: 6473 2e63 7265 6174 6556 6172 6961 626c  ds.createVariabl
-0000b170: 6528 2274 6573 7422 2c20 2269 3422 2c20  e("test", "i4", 
-0000b180: 2822 7822 2c29 290a 0a20 2020 2023 2063  ("x",))..    # c
-0000b190: 6865 636b 2073 6361 6c65 730a 2020 2020  heck scales.    
-0000b1a0: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
-0000b1b0: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
-0000b1c0: 6364 662c 2022 7222 2920 6173 2064 733a  cdf, "r") as ds:
-0000b1d0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000b1e0: 6473 2e76 6172 6961 626c 6573 5b22 7465  ds.variables["te
-0000b1f0: 7374 225d 2e61 7474 7273 2e5f 6835 6174  st"].attrs._h5at
-0000b200: 7472 732e 6765 7428 2244 494d 454e 5349  trs.get("DIMENSI
-0000b210: 4f4e 5f4c 4953 5422 2c20 4661 6c73 6529  ON_LIST", False)
-0000b220: 0a0a 2020 2020 2320 6170 7065 6e64 2066  ..    # append f
-0000b230: 696c 6520 7769 7468 206c 6567 6163 7961  ile with legacya
-0000b240: 7069 0a20 2020 2077 6974 6820 6c65 6761  pi.    with lega
-0000b250: 6379 6170 692e 4461 7461 7365 7428 746d  cyapi.Dataset(tm
-0000b260: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-0000b270: 2272 2b22 2920 6173 2064 733a 0a20 2020  "r+") as ds:.   
-0000b280: 2020 2020 2064 732e 6372 6561 7465 5661       ds.createVa
-0000b290: 7269 6162 6c65 2822 7465 7374 3122 2c20  riable("test1", 
-0000b2a0: 2269 3422 2c20 2822 7822 2c29 290a 0a20  "i4", ("x",)).. 
-0000b2b0: 2020 2023 2063 6865 636b 2073 6361 6c65     # check scale
-0000b2c0: 730a 2020 2020 7769 7468 2068 356e 6574  s.    with h5net
-0000b2d0: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
-0000b2e0: 616c 5f6e 6574 6364 662c 2022 7222 2920  al_netcdf, "r") 
-0000b2f0: 6173 2064 733a 0a20 2020 2020 2020 2061  as ds:.        a
-0000b300: 7373 6572 7420 6473 2e76 6172 6961 626c  ssert ds.variabl
-0000b310: 6573 5b22 7465 7374 3122 5d2e 6174 7472  es["test1"].attr
-0000b320: 732e 5f68 3561 7474 7273 2e67 6574 2822  s._h5attrs.get("
-0000b330: 4449 4d45 4e53 494f 4e5f 4c49 5354 222c  DIMENSION_LIST",
-0000b340: 2046 616c 7365 290a 0a0a 6465 6620 6372   False)...def cr
-0000b350: 6561 7465 5f61 7474 6163 685f 7363 616c  eate_attach_scal
-0000b360: 6573 2866 696c 656e 616d 652c 2061 7070  es(filename, app
-0000b370: 656e 645f 6d6f 6475 6c65 293a 0a20 2020  end_module):.   
-0000b380: 2023 2063 7265 6174 6520 6669 6c65 2077   # create file w
-0000b390: 6974 6820 6e65 7443 4446 340a 2020 2020  ith netCDF4.    
-0000b3a0: 7769 7468 206e 6574 4344 4634 2e44 6174  with netCDF4.Dat
-0000b3b0: 6173 6574 2866 696c 656e 616d 652c 2022  aset(filename, "
-0000b3c0: 7722 2920 6173 2064 733a 0a20 2020 2020  w") as ds:.     
-0000b3d0: 2020 2064 732e 6372 6561 7465 4469 6d65     ds.createDime
-0000b3e0: 6e73 696f 6e28 2278 222c 2030 290a 2020  nsion("x", 0).  
-0000b3f0: 2020 2020 2020 6473 2e63 7265 6174 6544        ds.createD
-0000b400: 696d 656e 7369 6f6e 2822 7922 2c20 3129  imension("y", 1)
-0000b410: 0a20 2020 2020 2020 2064 732e 6372 6561  .        ds.crea
-0000b420: 7465 5661 7269 6162 6c65 2822 7465 7374  teVariable("test
-0000b430: 222c 2022 6934 222c 2028 2278 222c 2929  ", "i4", ("x",))
-0000b440: 0a20 2020 2020 2020 2064 732e 7661 7269  .        ds.vari
-0000b450: 6162 6c65 735b 2274 6573 7422 5d20 3d20  ables["test"] = 
-0000b460: 6e70 2e6f 6e65 7328 2831 302c 2929 0a0a  np.ones((10,))..
-0000b470: 2020 2020 2320 6170 7065 6e64 2066 696c      # append fil
-0000b480: 6520 7769 7468 206e 6574 4344 4634 0a20  e with netCDF4. 
-0000b490: 2020 2077 6974 6820 6170 7065 6e64 5f6d     with append_m
-0000b4a0: 6f64 756c 652e 4461 7461 7365 7428 6669  odule.Dataset(fi
-0000b4b0: 6c65 6e61 6d65 2c20 2261 2229 2061 7320  lename, "a") as 
-0000b4c0: 6473 3a0a 2020 2020 2020 2020 6473 2e63  ds:.        ds.c
-0000b4d0: 7265 6174 6556 6172 6961 626c 6528 2274  reateVariable("t
-0000b4e0: 6573 7431 222c 2022 6934 222c 2028 2278  est1", "i4", ("x
-0000b4f0: 222c 2929 0a20 2020 2020 2020 2064 732e  ",)).        ds.
-0000b500: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
-0000b510: 7922 2c20 2269 3422 2c20 2822 7822 2c20  y", "i4", ("x", 
-0000b520: 2279 2229 290a 0a20 2020 2023 2063 6865  "y"))..    # che
-0000b530: 636b 2073 6361 6c65 730a 2020 2020 7769  ck scales.    wi
-0000b540: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-0000b550: 2866 696c 656e 616d 652c 2022 7222 2920  (filename, "r") 
-0000b560: 6173 2064 733a 0a20 2020 2020 2020 2072  as ds:.        r
-0000b570: 6566 7320 3d20 6473 2e5f 6835 6772 6f75  efs = ds._h5grou
-0000b580: 705b 2278 225d 2e61 7474 7273 2e67 6574  p["x"].attrs.get
-0000b590: 2822 5245 4645 5245 4e43 455f 4c49 5354  ("REFERENCE_LIST
-0000b5a0: 222c 2046 616c 7365 290a 2020 2020 2020  ", False).      
-0000b5b0: 2020 6173 7365 7274 206c 656e 2872 6566    assert len(ref
-0000b5c0: 7329 203d 3d20 330a 2020 2020 2020 2020  s) == 3.        
-0000b5d0: 666f 7220 2872 6566 2c20 6469 6d29 2c20  for (ref, dim), 
-0000b5e0: 6e61 6d65 2069 6e20 7a69 7028 7265 6673  name in zip(refs
-0000b5f0: 2c20 5b22 2f74 6573 7422 2c20 222f 7465  , ["/test", "/te
-0000b600: 7374 3122 2c20 222f 5f6e 6334 5f6e 6f6e  st1", "/_nc4_non
-0000b610: 5f63 6f6f 7264 5f79 225d 293a 0a20 2020  _coord_y"]):.   
-0000b620: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000b630: 6469 6d20 3d3d 2030 0a20 2020 2020 2020  dim == 0.       
-0000b640: 2020 2020 2061 7373 6572 7420 6473 2e5f       assert ds._
-0000b650: 726f 6f74 2e5f 6835 6669 6c65 5b72 6566  root._h5file[ref
-0000b660: 5d2e 6e61 6d65 203d 3d20 6e61 6d65 0a0a  ].name == name..
-0000b670: 0a64 6566 2074 6573 745f 6372 6561 7465  .def test_create
-0000b680: 5f61 7474 6163 685f 7363 616c 6573 5f6e  _attach_scales_n
-0000b690: 6574 6364 6634 2874 6d70 5f6c 6f63 616c  etcdf4(tmp_local
-0000b6a0: 5f6e 6574 6364 6629 3a0a 2020 2020 6372  _netcdf):.    cr
-0000b6b0: 6561 7465 5f61 7474 6163 685f 7363 616c  eate_attach_scal
-0000b6c0: 6573 2874 6d70 5f6c 6f63 616c 5f6e 6574  es(tmp_local_net
-0000b6d0: 6364 662c 206e 6574 4344 4634 290a 0a0a  cdf, netCDF4)...
-0000b6e0: 6465 6620 7465 7374 5f63 7265 6174 655f  def test_create_
-0000b6f0: 6174 7461 6368 5f73 6361 6c65 735f 6c65  attach_scales_le
-0000b700: 6761 6379 6170 6928 746d 705f 6c6f 6361  gacyapi(tmp_loca
-0000b710: 6c5f 6e65 7463 6466 293a 0a20 2020 2063  l_netcdf):.    c
-0000b720: 7265 6174 655f 6174 7461 6368 5f73 6361  reate_attach_sca
-0000b730: 6c65 7328 746d 705f 6c6f 6361 6c5f 6e65  les(tmp_local_ne
-0000b740: 7463 6466 2c20 6c65 6761 6379 6170 6929  tcdf, legacyapi)
-0000b750: 0a0a 0a64 6566 2074 6573 745f 6465 7461  ...def test_deta
-0000b760: 6368 5f73 6361 6c65 2874 6d70 5f6c 6f63  ch_scale(tmp_loc
-0000b770: 616c 5f6e 6574 6364 6629 3a0a 2020 2020  al_netcdf):.    
-0000b780: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
-0000b790: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
-0000b7a0: 6364 662c 2022 7722 2920 6173 2064 733a  cdf, "w") as ds:
-0000b7b0: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
-0000b7c0: 6e73 696f 6e73 5b22 7822 5d20 3d20 320a  nsions["x"] = 2.
-0000b7d0: 2020 2020 2020 2020 6473 2e64 696d 656e          ds.dimen
-0000b7e0: 7369 6f6e 735b 2279 225d 203d 2032 0a0a  sions["y"] = 2..
-0000b7f0: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
-0000b800: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
-0000b810: 5f6e 6574 6364 662c 2022 6122 2920 6173  _netcdf, "a") as
-0000b820: 2064 733a 0a20 2020 2020 2020 2064 732e   ds:.        ds.
-0000b830: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
-0000b840: 2274 6573 7422 2c20 6469 6d65 6e73 696f  "test", dimensio
-0000b850: 6e73 3d28 2278 222c 292c 2064 7479 7065  ns=("x",), dtype
-0000b860: 3d6e 702e 696e 7436 3429 0a0a 2020 2020  =np.int64)..    
-0000b870: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
-0000b880: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
-0000b890: 6364 662c 2022 7222 2920 6173 2064 733a  cdf, "r") as ds:
-0000b8a0: 0a20 2020 2020 2020 2072 6566 7320 3d20  .        refs = 
-0000b8b0: 6473 2e5f 6835 6772 6f75 705b 2278 225d  ds._h5group["x"]
-0000b8c0: 2e61 7474 7273 2e67 6574 2822 5245 4645  .attrs.get("REFE
-0000b8d0: 5245 4e43 455f 4c49 5354 222c 2046 616c  RENCE_LIST", Fal
-0000b8e0: 7365 290a 2020 2020 2020 2020 6173 7365  se).        asse
-0000b8f0: 7274 206c 656e 2872 6566 7329 203d 3d20  rt len(refs) == 
-0000b900: 310a 2020 2020 2020 2020 666f 7220 2872  1.        for (r
-0000b910: 6566 2c20 6469 6d29 2c20 6e61 6d65 2069  ef, dim), name i
-0000b920: 6e20 7a69 7028 7265 6673 2c20 5b22 2f74  n zip(refs, ["/t
-0000b930: 6573 7422 5d29 3a0a 2020 2020 2020 2020  est"]):.        
-0000b940: 2020 2020 6173 7365 7274 2064 696d 203d      assert dim =
-0000b950: 3d20 300a 2020 2020 2020 2020 2020 2020  = 0.            
-0000b960: 6173 7365 7274 2064 732e 5f72 6f6f 742e  assert ds._root.
-0000b970: 5f68 3566 696c 655b 7265 665d 2e6e 616d  _h5file[ref].nam
-0000b980: 6520 3d3d 206e 616d 650a 0a20 2020 2077  e == name..    w
-0000b990: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-0000b9a0: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-0000b9b0: 6466 2c20 2261 2229 2061 7320 6473 3a0a  df, "a") as ds:.
-0000b9c0: 2020 2020 2020 2020 6473 2e64 696d 656e          ds.dimen
-0000b9d0: 7369 6f6e 735b 2278 225d 2e5f 6465 7461  sions["x"]._deta
-0000b9e0: 6368 5f73 6361 6c65 2829 0a0a 2020 2020  ch_scale()..    
-0000b9f0: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
-0000ba00: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
-0000ba10: 6364 662c 2022 7222 2920 6173 2064 733a  cdf, "r") as ds:
-0000ba20: 0a20 2020 2020 2020 2072 6566 7320 3d20  .        refs = 
-0000ba30: 6473 2e5f 6835 6772 6f75 705b 2278 225d  ds._h5group["x"]
-0000ba40: 2e61 7474 7273 2e67 6574 2822 5245 4645  .attrs.get("REFE
-0000ba50: 5245 4e43 455f 4c49 5354 222c 2046 616c  RENCE_LIST", Fal
-0000ba60: 7365 290a 2020 2020 2020 2020 6173 7365  se).        asse
-0000ba70: 7274 206e 6f74 2072 6566 730a 0a0a 6465  rt not refs...de
-0000ba80: 6620 7465 7374 5f69 735f 7363 616c 6528  f test_is_scale(
-0000ba90: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000baa0: 293a 0a20 2020 2077 6974 6820 6c65 6761  ):.    with lega
-0000bab0: 6379 6170 692e 4461 7461 7365 7428 746d  cyapi.Dataset(tm
-0000bac0: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-0000bad0: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
-0000bae0: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-0000baf0: 656e 7369 6f6e 2822 7822 2c20 3130 290a  ension("x", 10).
-0000bb00: 2020 2020 7769 7468 206c 6567 6163 7961      with legacya
-0000bb10: 7069 2e44 6174 6173 6574 2874 6d70 5f6c  pi.Dataset(tmp_l
-0000bb20: 6f63 616c 5f6e 6574 6364 662c 2022 7222  ocal_netcdf, "r"
-0000bb30: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-0000bb40: 2061 7373 6572 7420 6473 2e64 696d 656e   assert ds.dimen
-0000bb50: 7369 6f6e 735b 2278 225d 2e5f 6973 7363  sions["x"]._issc
-0000bb60: 616c 650a 0a0a 6465 6620 7465 7374 5f67  ale...def test_g
-0000bb70: 6574 5f64 696d 5f73 6361 6c65 5f72 6566  et_dim_scale_ref
-0000bb80: 7328 746d 705f 6c6f 6361 6c5f 6e65 7463  s(tmp_local_netc
-0000bb90: 6466 293a 0a20 2020 2077 6974 6820 6c65  df):.    with le
-0000bba0: 6761 6379 6170 692e 4461 7461 7365 7428  gacyapi.Dataset(
-0000bbb0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000bbc0: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
-0000bbd0: 2020 2020 2020 6473 2e63 7265 6174 6544        ds.createD
-0000bbe0: 696d 656e 7369 6f6e 2822 7822 2c20 3130  imension("x", 10
-0000bbf0: 290a 2020 2020 2020 2020 6473 2e63 7265  ).        ds.cre
-0000bc00: 6174 6556 6172 6961 626c 6528 2274 6573  ateVariable("tes
-0000bc10: 7430 222c 2022 6938 222c 2028 2278 222c  t0", "i8", ("x",
-0000bc20: 2929 0a20 2020 2020 2020 2064 732e 6372  )).        ds.cr
-0000bc30: 6561 7465 5661 7269 6162 6c65 2822 7465  eateVariable("te
-0000bc40: 7374 3122 2c20 2269 3822 2c20 2822 7822  st1", "i8", ("x"
-0000bc50: 2c29 290a 2020 2020 7769 7468 206c 6567  ,)).    with leg
-0000bc60: 6163 7961 7069 2e44 6174 6173 6574 2874  acyapi.Dataset(t
-0000bc70: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-0000bc80: 2022 7222 2920 6173 2064 733a 0a20 2020   "r") as ds:.   
-0000bc90: 2020 2020 2072 6566 7320 3d20 6473 2e64       refs = ds.d
-0000bca0: 696d 656e 7369 6f6e 735b 2278 225d 2e5f  imensions["x"]._
-0000bcb0: 7363 616c 655f 7265 6673 0a20 2020 2020  scale_refs.     
-0000bcc0: 2020 2061 7373 6572 7420 6473 2e5f 6835     assert ds._h5
-0000bcd0: 6669 6c65 5b72 6566 735b 305d 5b30 5d5d  file[refs[0][0]]
-0000bce0: 203d 3d20 6473 5b22 7465 7374 3022 5d2e   == ds["test0"].
-0000bcf0: 5f68 3564 730a 2020 2020 2020 2020 6173  _h5ds.        as
-0000bd00: 7365 7274 2064 732e 5f68 3566 696c 655b  sert ds._h5file[
-0000bd10: 7265 6673 5b31 5d5b 305d 5d20 3d3d 2064  refs[1][0]] == d
-0000bd20: 735b 2274 6573 7431 225d 2e5f 6835 6473  s["test1"]._h5ds
-0000bd30: 0a0a 0a64 6566 2063 7265 6174 655f 6e65  ...def create_ne
-0000bd40: 7463 6466 5f64 696d 656e 7369 6f6e 7328  tcdf_dimensions(
-0000bd50: 6473 2c20 6964 7829 3a0a 2020 2020 2320  ds, idx):.    # 
-0000bd60: 6469 6d65 6e73 696f 6e20 616e 6420 7661  dimension and va
-0000bd70: 7269 6162 6c65 2073 6574 7570 2069 7320  riable setup is 
-0000bd80: 6164 6170 7465 6420 6672 6f6d 2074 6865  adapted from the
-0000bd90: 2062 6c6f 6770 6f73 7420 6174 0a20 2020   blogpost at.   
-0000bda0: 2023 2068 7474 7073 3a2f 2f77 7777 2e75   # https://www.u
-0000bdb0: 6e69 6461 7461 2e75 6361 722e 6564 752f  nidata.ucar.edu/
-0000bdc0: 626c 6f67 732f 6465 7665 6c6f 7065 722f  blogs/developer/
-0000bdd0: 656e 2f65 6e74 7279 2f6e 6574 6364 6634  en/entry/netcdf4
-0000bde0: 5f73 6861 7265 645f 6469 6d65 6e73 696f  _shared_dimensio
-0000bdf0: 6e73 0a20 2020 2067 203d 2064 732e 6372  ns.    g = ds.cr
-0000be00: 6561 7465 4772 6f75 7028 2264 696d 7465  eateGroup("dimte
-0000be10: 7374 2220 2b20 7374 7228 6964 7829 290a  st" + str(idx)).
-0000be20: 2020 2020 672e 6372 6561 7465 4469 6d65      g.createDime
-0000be30: 6e73 696f 6e28 2274 696d 6522 2c20 3029  nsion("time", 0)
-0000be40: 2020 2320 7469 6d65 0a20 2020 2067 2e63    # time.    g.c
-0000be50: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
-0000be60: 6e76 6563 222c 2035 202b 2069 6478 2920  nvec", 5 + idx) 
-0000be70: 2023 206e 7665 630a 2020 2020 672e 6372   # nvec.    g.cr
-0000be80: 6561 7465 4469 6d65 6e73 696f 6e28 2273  eateDimension("s
-0000be90: 616d 706c 6522 2c20 3220 2b20 6964 7829  ample", 2 + idx)
-0000bea0: 2020 2320 7361 6d70 6c65 0a20 2020 2067    # sample.    g
-0000beb0: 2e63 7265 6174 6544 696d 656e 7369 6f6e  .createDimension
-0000bec0: 2822 7368 6970 222c 2033 202b 2069 6478  ("ship", 3 + idx
-0000bed0: 2920 2023 2073 6869 700a 2020 2020 672e  )  # ship.    g.
-0000bee0: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
-0000bef0: 2273 6869 705f 7374 726c 656e 222c 2031  "ship_strlen", 1
-0000bf00: 3029 2020 2320 7368 6970 5f73 7472 6c65  0)  # ship_strle
-0000bf10: 6e0a 2020 2020 672e 6372 6561 7465 4469  n.    g.createDi
-0000bf20: 6d65 6e73 696f 6e28 2263 6f6c 6c69 6465  mension("collide
-0000bf30: 222c 2037 202b 2069 6478 2920 2023 2063  ", 7 + idx)  # c
-0000bf40: 6f6c 6c69 6465 0a0a 2020 2020 7469 6d65  ollide..    time
-0000bf50: 203d 2067 2e63 7265 6174 6556 6172 6961   = g.createVaria
-0000bf60: 626c 6528 2274 696d 6522 2c20 2266 3822  ble("time", "f8"
-0000bf70: 2c20 2822 7469 6d65 222c 2929 0a20 2020  , ("time",)).   
-0000bf80: 2064 6174 6120 3d20 672e 6372 6561 7465   data = g.create
-0000bf90: 5661 7269 6162 6c65 2822 6461 7461 222c  Variable("data",
-0000bfa0: 2022 6938 222c 2028 2273 6869 7022 2c20   "i8", ("ship", 
-0000bfb0: 2273 616d 706c 6522 2c20 2274 696d 6522  "sample", "time"
-0000bfc0: 2c20 226e 7665 6322 2929 0a20 2020 2063  , "nvec")).    c
-0000bfd0: 6f6c 6c69 6465 203d 2067 2e63 7265 6174  ollide = g.creat
-0000bfe0: 6556 6172 6961 626c 6528 2263 6f6c 6c69  eVariable("colli
-0000bff0: 6465 222c 2022 6938 222c 2028 226e 7665  de", "i8", ("nve
-0000c000: 6322 2c29 290a 2020 2020 6e6f 6e5f 636f  c",)).    non_co
-0000c010: 6c6c 6964 6520 3d20 672e 6372 6561 7465  llide = g.create
-0000c020: 5661 7269 6162 6c65 2822 6e6f 6e5f 636f  Variable("non_co
-0000c030: 6c6c 6964 6522 2c20 2269 3822 2c20 2822  llide", "i8", ("
-0000c040: 6e76 6563 222c 2929 0a20 2020 2073 6869  nvec",)).    shi
-0000c050: 7020 3d20 672e 6372 6561 7465 5661 7269  p = g.createVari
-0000c060: 6162 6c65 2822 7368 6970 222c 2022 5331  able("ship", "S1
-0000c070: 222c 2028 2273 6869 7022 2c20 2273 6869  ", ("ship", "shi
-0000c080: 705f 7374 726c 656e 2229 290a 2020 2020  p_strlen")).    
-0000c090: 7361 6d70 6c65 203d 2067 2e63 7265 6174  sample = g.creat
-0000c0a0: 6556 6172 6961 626c 6528 2273 616d 706c  eVariable("sampl
-0000c0b0: 6522 2c20 2269 3822 2c20 2822 7469 6d65  e", "i8", ("time
-0000c0c0: 222c 2022 7361 6d70 6c65 2229 290a 0a20  ", "sample")).. 
-0000c0d0: 2020 2074 696d 655b 3a5d 203d 206e 702e     time[:] = np.
-0000c0e0: 6172 616e 6765 2831 3020 2b20 6964 7829  arange(10 + idx)
-0000c0f0: 0a20 2020 2064 6174 615b 3a5d 203d 206e  .    data[:] = n
-0000c100: 702e 6f6e 6573 2828 3320 2b20 6964 782c  p.ones((3 + idx,
-0000c110: 2032 202b 2069 6478 2c20 3130 202b 2069   2 + idx, 10 + i
-0000c120: 6478 2c20 3520 2b20 6964 7829 2920 2a20  dx, 5 + idx)) * 
-0000c130: 3132 2e30 0a20 2020 2063 6f6c 6c69 6465  12.0.    collide
-0000c140: 5b2e 2e2e 5d20 3d20 6e70 2e61 7261 6e67  [...] = np.arang
-0000c150: 6528 3520 2b20 6964 7829 0a20 2020 206e  e(5 + idx).    n
-0000c160: 6f6e 5f63 6f6c 6c69 6465 5b2e 2e2e 5d20  on_collide[...] 
-0000c170: 3d20 6e70 2e61 7261 6e67 6528 3520 2b20  = np.arange(5 + 
-0000c180: 6964 7829 202b 2031 300a 2020 2020 7361  idx) + 10.    sa
-0000c190: 6d70 6c65 5b30 203a 2032 202b 2069 6478  mple[0 : 2 + idx
-0000c1a0: 2c20 3a20 3220 2b20 6964 785d 203d 206e  , : 2 + idx] = n
-0000c1b0: 702e 6f6e 6573 2828 3220 2b20 6964 782c  p.ones((2 + idx,
-0000c1c0: 2032 202b 2069 6478 2929 0a20 2020 2069   2 + idx)).    i
-0000c1d0: 6620 7665 7273 696f 6e2e 7061 7273 6528  f version.parse(
-0000c1e0: 6835 7079 2e5f 5f76 6572 7369 6f6e 5f5f  h5py.__version__
-0000c1f0: 2920 3e3d 2076 6572 7369 6f6e 2e70 6172  ) >= version.par
-0000c200: 7365 2822 332e 302e 3022 293a 0a20 2020  se("3.0.0"):.   
-0000c210: 2020 2020 2073 6869 705b 305d 203d 206c       ship[0] = l
-0000c220: 6973 7428 2253 6b69 6666 2020 2020 2022  ist("Skiff     "
-0000c230: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000c240: 2020 2020 7368 6970 5b30 5d20 3d20 7374      ship[0] = st
-0000c250: 7269 6e67 5f74 6f5f 6368 6172 286e 702e  ring_to_char(np.
-0000c260: 6172 7261 7928 2253 6b69 6666 2020 2020  array("Skiff    
-0000c270: 2022 2c20 6474 7970 653d 227c 5331 2229   ", dtype="|S1")
-0000c280: 290a 0a0a 6465 6620 6372 6561 7465 5f68  )...def create_h
-0000c290: 356e 6574 6364 665f 6469 6d65 6e73 696f  5netcdf_dimensio
-0000c2a0: 6e73 2864 732c 2069 6478 293a 0a20 2020  ns(ds, idx):.   
-0000c2b0: 2023 2064 696d 656e 7369 6f6e 2061 6e64   # dimension and
-0000c2c0: 2076 6172 6961 626c 6520 7365 7475 7020   variable setup 
-0000c2d0: 6973 2061 6461 7074 6564 2066 726f 6d20  is adapted from 
-0000c2e0: 7468 6520 626c 6f67 706f 7374 2061 740a  the blogpost at.
-0000c2f0: 2020 2020 2320 6874 7470 733a 2f2f 7777      # https://ww
-0000c300: 772e 756e 6964 6174 612e 7563 6172 2e65  w.unidata.ucar.e
-0000c310: 6475 2f62 6c6f 6773 2f64 6576 656c 6f70  du/blogs/develop
-0000c320: 6572 2f65 6e2f 656e 7472 792f 6e65 7463  er/en/entry/netc
-0000c330: 6466 345f 7368 6172 6564 5f64 696d 656e  df4_shared_dimen
-0000c340: 7369 6f6e 730a 2020 2020 6720 3d20 6473  sions.    g = ds
-0000c350: 2e63 7265 6174 655f 6772 6f75 7028 2264  .create_group("d
-0000c360: 696d 7465 7374 2220 2b20 7374 7228 6964  imtest" + str(id
-0000c370: 7829 290a 2020 2020 672e 6469 6d65 6e73  x)).    g.dimens
-0000c380: 696f 6e73 5b22 7469 6d65 225d 203d 2030  ions["time"] = 0
-0000c390: 2020 2320 7469 6d65 0a20 2020 2067 2e64    # time.    g.d
-0000c3a0: 696d 656e 7369 6f6e 735b 226e 7665 6322  imensions["nvec"
-0000c3b0: 5d20 3d20 3520 2b20 6964 7820 2023 206e  ] = 5 + idx  # n
-0000c3c0: 7665 630a 2020 2020 672e 6469 6d65 6e73  vec.    g.dimens
-0000c3d0: 696f 6e73 5b22 7361 6d70 6c65 225d 203d  ions["sample"] =
-0000c3e0: 2032 202b 2069 6478 2020 2320 7361 6d70   2 + idx  # samp
-0000c3f0: 6c65 0a20 2020 2067 2e64 696d 656e 7369  le.    g.dimensi
-0000c400: 6f6e 735b 2273 6869 7022 5d20 3d20 3320  ons["ship"] = 3 
-0000c410: 2b20 6964 7820 2023 2073 6869 700a 2020  + idx  # ship.  
-0000c420: 2020 672e 6469 6d65 6e73 696f 6e73 5b22    g.dimensions["
-0000c430: 7368 6970 5f73 7472 6c65 6e22 5d20 3d20  ship_strlen"] = 
-0000c440: 3130 2020 2320 7368 6970 5f73 7472 6c65  10  # ship_strle
-0000c450: 6e0a 2020 2020 672e 6469 6d65 6e73 696f  n.    g.dimensio
-0000c460: 6e73 5b22 636f 6c6c 6964 6522 5d20 3d20  ns["collide"] = 
-0000c470: 3720 2b20 6964 7820 2023 2063 6f6c 6c69  7 + idx  # colli
-0000c480: 6465 0a0a 2020 2020 672e 6372 6561 7465  de..    g.create
-0000c490: 5f76 6172 6961 626c 6528 2274 696d 6522  _variable("time"
-0000c4a0: 2c20 6469 6d65 6e73 696f 6e73 3d28 2274  , dimensions=("t
-0000c4b0: 696d 6522 2c29 2c20 6474 7970 653d 6e70  ime",), dtype=np
-0000c4c0: 2e66 6c6f 6174 3634 290a 2020 2020 672e  .float64).    g.
-0000c4d0: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
-0000c4e0: 0a20 2020 2020 2020 2022 6461 7461 222c  .        "data",
-0000c4f0: 2064 696d 656e 7369 6f6e 733d 2822 7368   dimensions=("sh
-0000c500: 6970 222c 2022 7361 6d70 6c65 222c 2022  ip", "sample", "
-0000c510: 7469 6d65 222c 2022 6e76 6563 2229 2c20  time", "nvec"), 
-0000c520: 6474 7970 653d 6e70 2e69 6e74 3634 0a20  dtype=np.int64. 
-0000c530: 2020 2029 0a20 2020 2067 2e63 7265 6174     ).    g.creat
-0000c540: 655f 7661 7269 6162 6c65 2822 636f 6c6c  e_variable("coll
-0000c550: 6964 6522 2c20 6469 6d65 6e73 696f 6e73  ide", dimensions
-0000c560: 3d28 226e 7665 6322 2c29 2c20 6474 7970  =("nvec",), dtyp
-0000c570: 653d 6e70 2e69 6e74 3634 290a 2020 2020  e=np.int64).    
-0000c580: 672e 6372 6561 7465 5f76 6172 6961 626c  g.create_variabl
-0000c590: 6528 226e 6f6e 5f63 6f6c 6c69 6465 222c  e("non_collide",
-0000c5a0: 2064 696d 656e 7369 6f6e 733d 2822 6e76   dimensions=("nv
-0000c5b0: 6563 222c 292c 2064 7479 7065 3d6e 702e  ec",), dtype=np.
-0000c5c0: 696e 7436 3429 0a20 2020 2067 2e63 7265  int64).    g.cre
-0000c5d0: 6174 655f 7661 7269 6162 6c65 2822 7361  ate_variable("sa
-0000c5e0: 6d70 6c65 222c 2064 696d 656e 7369 6f6e  mple", dimension
-0000c5f0: 733d 2822 7469 6d65 222c 2022 7361 6d70  s=("time", "samp
-0000c600: 6c65 2229 2c20 6474 7970 653d 6e70 2e69  le"), dtype=np.i
-0000c610: 6e74 3634 290a 2020 2020 672e 6372 6561  nt64).    g.crea
-0000c620: 7465 5f76 6172 6961 626c 6528 2273 6869  te_variable("shi
-0000c630: 7022 2c20 6469 6d65 6e73 696f 6e73 3d28  p", dimensions=(
-0000c640: 2273 6869 7022 2c20 2273 6869 705f 7374  "ship", "ship_st
-0000c650: 726c 656e 2229 2c20 6474 7970 653d 2253  rlen"), dtype="S
-0000c660: 3122 290a 0a20 2020 2067 2e72 6573 697a  1")..    g.resiz
-0000c670: 655f 6469 6d65 6e73 696f 6e28 2274 696d  e_dimension("tim
-0000c680: 6522 2c20 3130 202b 2069 6478 290a 2020  e", 10 + idx).  
-0000c690: 2020 672e 7661 7269 6162 6c65 735b 2274    g.variables["t
-0000c6a0: 696d 6522 5d5b 3a5d 203d 206e 702e 6172  ime"][:] = np.ar
-0000c6b0: 616e 6765 2831 3020 2b20 6964 7829 0a20  ange(10 + idx). 
-0000c6c0: 2020 2067 2e76 6172 6961 626c 6573 5b22     g.variables["
-0000c6d0: 6461 7461 225d 5b3a 5d20 3d20 6e70 2e6f  data"][:] = np.o
-0000c6e0: 6e65 7328 2833 202b 2069 6478 2c20 3220  nes((3 + idx, 2 
-0000c6f0: 2b20 6964 782c 2031 3020 2b20 6964 782c  + idx, 10 + idx,
-0000c700: 2035 202b 2069 6478 2929 202a 2031 322e   5 + idx)) * 12.
-0000c710: 300a 2020 2020 672e 7661 7269 6162 6c65  0.    g.variable
-0000c720: 735b 2263 6f6c 6c69 6465 225d 5b2e 2e2e  s["collide"][...
-0000c730: 5d20 3d20 6e70 2e61 7261 6e67 6528 3520  ] = np.arange(5 
-0000c740: 2b20 6964 7829 0a20 2020 2067 2e76 6172  + idx).    g.var
-0000c750: 6961 626c 6573 5b22 6e6f 6e5f 636f 6c6c  iables["non_coll
-0000c760: 6964 6522 5d5b 2e2e 2e5d 203d 206e 702e  ide"][...] = np.
-0000c770: 6172 616e 6765 2835 202b 2069 6478 2920  arange(5 + idx) 
-0000c780: 2b20 3130 0a20 2020 2067 2e76 6172 6961  + 10.    g.varia
-0000c790: 626c 6573 5b22 7361 6d70 6c65 225d 5b30  bles["sample"][0
-0000c7a0: 203a 2032 202b 2069 6478 2c20 3a20 3220   : 2 + idx, : 2 
-0000c7b0: 2b20 6964 785d 203d 206e 702e 6f6e 6573  + idx] = np.ones
-0000c7c0: 2828 3220 2b20 6964 782c 2032 202b 2069  ((2 + idx, 2 + i
-0000c7d0: 6478 2929 0a20 2020 2069 6620 7665 7273  dx)).    if vers
-0000c7e0: 696f 6e2e 7061 7273 6528 6835 7079 2e5f  ion.parse(h5py._
-0000c7f0: 5f76 6572 7369 6f6e 5f5f 2920 3e3d 2076  _version__) >= v
-0000c800: 6572 7369 6f6e 2e70 6172 7365 2822 332e  ersion.parse("3.
-0000c810: 302e 3022 293a 0a20 2020 2020 2020 2067  0.0"):.        g
-0000c820: 2e76 6172 6961 626c 6573 5b22 7368 6970  .variables["ship
-0000c830: 225d 5b30 5d20 3d20 6c69 7374 2822 536b  "][0] = list("Sk
-0000c840: 6966 6620 2020 2020 2229 0a20 2020 2065  iff     ").    e
-0000c850: 6c73 653a 0a20 2020 2020 2020 2067 2e76  lse:.        g.v
-0000c860: 6172 6961 626c 6573 5b22 7368 6970 225d  ariables["ship"]
-0000c870: 5b30 5d20 3d20 7374 7269 6e67 5f74 6f5f  [0] = string_to_
-0000c880: 6368 6172 286e 702e 6172 7261 7928 2253  char(np.array("S
-0000c890: 6b69 6666 2020 2020 2022 2c20 6474 7970  kiff     ", dtyp
-0000c8a0: 653d 227c 5331 2229 290a 0a0a 6465 6620  e="|S1"))...def 
-0000c8b0: 6368 6563 6b5f 6e65 7463 6466 5f64 696d  check_netcdf_dim
-0000c8c0: 656e 7369 6f6e 7328 746d 705f 6e65 7463  ensions(tmp_netc
-0000c8d0: 6466 2c20 7772 6974 655f 6d6f 6475 6c65  df, write_module
-0000c8e0: 2c20 7265 6164 5f6d 6f64 756c 6529 3a0a  , read_module):.
-0000c8f0: 2020 2020 6966 2072 6561 645f 6d6f 6475      if read_modu
-0000c900: 6c65 2069 6e20 5b6c 6567 6163 7961 7069  le in [legacyapi
-0000c910: 2c20 6e65 7443 4446 345d 3a0a 2020 2020  , netCDF4]:.    
-0000c920: 2020 2020 6f70 656e 6572 203d 2072 6561      opener = rea
-0000c930: 645f 6d6f 6475 6c65 2e44 6174 6173 6574  d_module.Dataset
-0000c940: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000c950: 2020 206f 7065 6e65 7220 3d20 6835 6e65     opener = h5ne
-0000c960: 7463 6466 2e46 696c 650a 2020 2020 7769  tcdf.File.    wi
-0000c970: 7468 206f 7065 6e65 7228 746d 705f 6e65  th opener(tmp_ne
-0000c980: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
-0000c990: 3a0a 2020 2020 2020 2020 666f 7220 692c  :.        for i,
-0000c9a0: 2067 7270 2069 6e20 656e 756d 6572 6174   grp in enumerat
-0000c9b0: 6528 5b22 6469 6d74 6573 7430 222c 2022  e(["dimtest0", "
-0000c9c0: 6469 6d74 6573 7431 225d 293a 0a20 2020  dimtest1"]):.   
-0000c9d0: 2020 2020 2020 2020 2067 203d 2064 732e           g = ds.
-0000c9e0: 6772 6f75 7073 5b67 7270 5d0a 2020 2020  groups[grp].    
-0000c9f0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-0000ca00: 6574 2867 2e64 696d 656e 7369 6f6e 7329  et(g.dimensions)
-0000ca10: 203d 3d20 7b0a 2020 2020 2020 2020 2020   == {.          
-0000ca20: 2020 2020 2020 2263 6f6c 6c69 6465 222c        "collide",
-0000ca30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ca40: 2022 7368 6970 5f73 7472 6c65 6e22 2c0a   "ship_strlen",.
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2274 696d 6522 2c0a 2020 2020 2020 2020  "time",.        
-0000ca70: 2020 2020 2020 2020 226e 7665 6322 2c0a          "nvec",.
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2273 6869 7022 2c0a 2020 2020 2020 2020  "ship",.        
-0000caa0: 2020 2020 2020 2020 2273 616d 706c 6522          "sample"
-0000cab0: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
-0000cac0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-0000cad0: 6561 645f 6d6f 6475 6c65 2069 6e20 5b6c  ead_module in [l
-0000cae0: 6567 6163 7961 7069 2c20 6835 6e65 7463  egacyapi, h5netc
-0000caf0: 6466 5d3a 0a20 2020 2020 2020 2020 2020  df]:.           
-0000cb00: 2020 2020 2061 7373 6572 7420 672e 6469       assert g.di
-0000cb10: 6d65 6e73 696f 6e73 5b22 7469 6d65 225d  mensions["time"]
-0000cb20: 2e69 7375 6e6c 696d 6974 6564 2829 0a20  .isunlimited(). 
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000cb40: 7373 6572 7420 672e 6469 6d65 6e73 696f  ssert g.dimensio
-0000cb50: 6e73 5b22 7469 6d65 225d 2e73 697a 6520  ns["time"].size 
-0000cb60: 3d3d 2031 3020 2b20 690a 2020 2020 2020  == 10 + i.      
-0000cb70: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000cb80: 206e 6f74 2067 2e64 696d 656e 7369 6f6e   not g.dimension
-0000cb90: 735b 226e 7665 6322 5d2e 6973 756e 6c69  s["nvec"].isunli
-0000cba0: 6d69 7465 6428 290a 2020 2020 2020 2020  mited().        
-0000cbb0: 2020 2020 2020 2020 6173 7365 7274 2067          assert g
-0000cbc0: 2e64 696d 656e 7369 6f6e 735b 226e 7665  .dimensions["nve
-0000cbd0: 6322 5d2e 7369 7a65 203d 3d20 3520 2b20  c"].size == 5 + 
-0000cbe0: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-0000cbf0: 2020 6173 7365 7274 206e 6f74 2067 2e64    assert not g.d
-0000cc00: 696d 656e 7369 6f6e 735b 2273 616d 706c  imensions["sampl
-0000cc10: 6522 5d2e 6973 756e 6c69 6d69 7465 6428  e"].isunlimited(
-0000cc20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000cc30: 2020 6173 7365 7274 2067 2e64 696d 656e    assert g.dimen
-0000cc40: 7369 6f6e 735b 2273 616d 706c 6522 5d2e  sions["sample"].
-0000cc50: 7369 7a65 203d 3d20 3220 2b20 690a 2020  size == 2 + i.  
-0000cc60: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000cc70: 7365 7274 206e 6f74 2067 2e64 696d 656e  sert not g.dimen
-0000cc80: 7369 6f6e 735b 2263 6f6c 6c69 6465 225d  sions["collide"]
-0000cc90: 2e69 7375 6e6c 696d 6974 6564 2829 0a20  .isunlimited(). 
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000ccb0: 7373 6572 7420 672e 6469 6d65 6e73 696f  ssert g.dimensio
-0000ccc0: 6e73 5b22 636f 6c6c 6964 6522 5d2e 7369  ns["collide"].si
-0000ccd0: 7a65 203d 3d20 3720 2b20 690a 2020 2020  ze == 7 + i.    
-0000cce0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000ccf0: 7274 206e 6f74 2067 2e64 696d 656e 7369  rt not g.dimensi
-0000cd00: 6f6e 735b 2273 6869 7022 5d2e 6973 756e  ons["ship"].isun
-0000cd10: 6c69 6d69 7465 6428 290a 2020 2020 2020  limited().      
-0000cd20: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000cd30: 2067 2e64 696d 656e 7369 6f6e 735b 2273   g.dimensions["s
-0000cd40: 6869 7022 5d2e 7369 7a65 203d 3d20 3320  hip"].size == 3 
-0000cd50: 2b20 690a 2020 2020 2020 2020 2020 2020  + i.            
-0000cd60: 2020 2020 6173 7365 7274 206e 6f74 2067      assert not g
-0000cd70: 2e64 696d 656e 7369 6f6e 735b 2273 6869  .dimensions["shi
-0000cd80: 705f 7374 726c 656e 225d 2e69 7375 6e6c  p_strlen"].isunl
-0000cd90: 696d 6974 6564 2829 0a20 2020 2020 2020  imited().       
-0000cda0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000cdb0: 672e 6469 6d65 6e73 696f 6e73 5b22 7368  g.dimensions["sh
-0000cdc0: 6970 5f73 7472 6c65 6e22 5d2e 7369 7a65  ip_strlen"].size
-0000cdd0: 203d 3d20 3130 0a20 2020 2020 2020 2020   == 10.         
-0000cde0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000cdf0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000ce00: 672e 6469 6d65 6e73 696f 6e73 5b22 7469  g.dimensions["ti
-0000ce10: 6d65 225d 2e69 7375 6e6c 696d 6974 6564  me"].isunlimited
-0000ce20: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-0000ce30: 2020 2061 7373 6572 7420 672e 6469 6d65     assert g.dime
-0000ce40: 6e73 696f 6e73 5b22 7469 6d65 225d 2e73  nsions["time"].s
-0000ce50: 697a 6520 3d3d 2031 3020 2b20 690a 2020  ize == 10 + i.  
-0000ce60: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000ce70: 7365 7274 206e 6f74 2067 2e64 696d 656e  sert not g.dimen
-0000ce80: 7369 6f6e 735b 226e 7665 6322 5d2e 6973  sions["nvec"].is
-0000ce90: 756e 6c69 6d69 7465 6428 290a 2020 2020  unlimited().    
-0000cea0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000ceb0: 7274 2067 2e64 696d 656e 7369 6f6e 735b  rt g.dimensions[
-0000cec0: 226e 7665 6322 5d2e 7369 7a65 203d 3d20  "nvec"].size == 
-0000ced0: 3520 2b20 690a 2020 2020 2020 2020 2020  5 + i.          
-0000cee0: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
-0000cef0: 2067 2e64 696d 656e 7369 6f6e 735b 2273   g.dimensions["s
-0000cf00: 616d 706c 6522 5d2e 6973 756e 6c69 6d69  ample"].isunlimi
-0000cf10: 7465 6428 290a 2020 2020 2020 2020 2020  ted().          
-0000cf20: 2020 2020 2020 6173 7365 7274 2067 2e64        assert g.d
-0000cf30: 696d 656e 7369 6f6e 735b 2273 616d 706c  imensions["sampl
-0000cf40: 6522 5d2e 7369 7a65 203d 3d20 3220 2b20  e"].size == 2 + 
-0000cf50: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-0000cf60: 2020 6173 7365 7274 206e 6f74 2067 2e64    assert not g.d
-0000cf70: 696d 656e 7369 6f6e 735b 2273 6869 7022  imensions["ship"
-0000cf80: 5d2e 6973 756e 6c69 6d69 7465 6428 290a  ].isunlimited().
-0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfa0: 6173 7365 7274 2067 2e64 696d 656e 7369  assert g.dimensi
-0000cfb0: 6f6e 735b 2273 6869 7022 5d2e 7369 7a65  ons["ship"].size
-0000cfc0: 203d 3d20 3320 2b20 690a 2020 2020 2020   == 3 + i.      
-0000cfd0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-0000cfe0: 206e 6f74 2067 2e64 696d 656e 7369 6f6e   not g.dimension
-0000cff0: 735b 2273 6869 705f 7374 726c 656e 225d  s["ship_strlen"]
-0000d000: 2e69 7375 6e6c 696d 6974 6564 2829 0a20  .isunlimited(). 
-0000d010: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000d020: 7373 6572 7420 672e 6469 6d65 6e73 696f  ssert g.dimensio
-0000d030: 6e73 5b22 7368 6970 5f73 7472 6c65 6e22  ns["ship_strlen"
-0000d040: 5d2e 7369 7a65 203d 3d20 3130 0a20 2020  ].size == 10.   
-0000d050: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-0000d060: 6572 7420 6e6f 7420 672e 6469 6d65 6e73  ert not g.dimens
-0000d070: 696f 6e73 5b22 636f 6c6c 6964 6522 5d2e  ions["collide"].
-0000d080: 6973 756e 6c69 6d69 7465 6428 290a 2020  isunlimited().  
-0000d090: 2020 2020 2020 2020 2020 2020 2020 6173                as
-0000d0a0: 7365 7274 2067 2e64 696d 656e 7369 6f6e  sert g.dimension
-0000d0b0: 735b 2263 6f6c 6c69 6465 225d 2e73 697a  s["collide"].siz
-0000d0c0: 6520 3d3d 2037 202b 2069 0a0a 2020 2020  e == 7 + i..    
-0000d0d0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-0000d0e0: 6574 2867 2e76 6172 6961 626c 6573 2920  et(g.variables) 
-0000d0f0: 3d3d 207b 0a20 2020 2020 2020 2020 2020  == {.           
-0000d100: 2020 2020 2022 6461 7461 222c 0a20 2020       "data",.   
-0000d110: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-0000d120: 6c6c 6964 6522 2c0a 2020 2020 2020 2020  llide",.        
-0000d130: 2020 2020 2020 2020 226e 6f6e 5f63 6f6c          "non_col
-0000d140: 6c69 6465 222c 0a20 2020 2020 2020 2020  lide",.         
-0000d150: 2020 2020 2020 2022 7469 6d65 222c 0a20         "time",. 
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d170: 7361 6d70 6c65 222c 0a20 2020 2020 2020  sample",.       
-0000d180: 2020 2020 2020 2020 2022 7368 6970 222c           "ship",
-0000d190: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-0000d1a0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000d1b0: 7420 672e 7661 7269 6162 6c65 735b 2274  t g.variables["t
-0000d1c0: 696d 6522 5d2e 7368 6170 6520 3d3d 2028  ime"].shape == (
-0000d1d0: 3130 202b 2069 2c29 0a20 2020 2020 2020  10 + i,).       
-0000d1e0: 2020 2020 2061 7373 6572 7420 672e 7661       assert g.va
-0000d1f0: 7269 6162 6c65 735b 2264 6174 6122 5d2e  riables["data"].
-0000d200: 7368 6170 6520 3d3d 2028 3320 2b20 692c  shape == (3 + i,
-0000d210: 2032 202b 2069 2c20 3130 202b 2069 2c20   2 + i, 10 + i, 
-0000d220: 3520 2b20 6929 0a20 2020 2020 2020 2020  5 + i).         
-0000d230: 2020 2061 7373 6572 7420 672e 7661 7269     assert g.vari
-0000d240: 6162 6c65 735b 2263 6f6c 6c69 6465 225d  ables["collide"]
-0000d250: 2e73 6861 7065 203d 3d20 2835 202b 2069  .shape == (5 + i
-0000d260: 2c29 0a20 2020 2020 2020 2020 2020 2061  ,).            a
-0000d270: 7373 6572 7420 672e 7661 7269 6162 6c65  ssert g.variable
-0000d280: 735b 226e 6f6e 5f63 6f6c 6c69 6465 225d  s["non_collide"]
-0000d290: 2e73 6861 7065 203d 3d20 2835 202b 2069  .shape == (5 + i
-0000d2a0: 2c29 0a20 2020 2020 2020 2020 2020 2061  ,).            a
-0000d2b0: 7373 6572 7420 672e 7661 7269 6162 6c65  ssert g.variable
-0000d2c0: 735b 2273 616d 706c 6522 5d2e 7368 6170  s["sample"].shap
-0000d2d0: 6520 3d3d 2028 3130 202b 2069 2c20 3220  e == (10 + i, 2 
-0000d2e0: 2b20 6929 0a20 2020 2020 2020 2020 2020  + i).           
-0000d2f0: 2061 7373 6572 7420 672e 7661 7269 6162   assert g.variab
-0000d300: 6c65 735b 2273 6869 7022 5d2e 7368 6170  les["ship"].shap
-0000d310: 6520 3d3d 2028 3320 2b20 692c 2031 3029  e == (3 + i, 10)
-0000d320: 0a0a 0a64 6566 2077 7269 7465 5f64 696d  ...def write_dim
-0000d330: 656e 7369 6f6e 7328 746d 705f 6e65 7463  ensions(tmp_netc
-0000d340: 6466 2c20 7772 6974 655f 6d6f 6475 6c65  df, write_module
-0000d350: 293a 0a20 2020 2069 6620 7772 6974 655f  ):.    if write_
-0000d360: 6d6f 6475 6c65 2069 6e20 5b6c 6567 6163  module in [legac
-0000d370: 7961 7069 2c20 6e65 7443 4446 345d 3a0a  yapi, netCDF4]:.
-0000d380: 2020 2020 2020 2020 7769 7468 2077 7269          with wri
-0000d390: 7465 5f6d 6f64 756c 652e 4461 7461 7365  te_module.Datase
-0000d3a0: 7428 746d 705f 6e65 7463 6466 2c20 2277  t(tmp_netcdf, "w
-0000d3b0: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
-0000d3c0: 2020 2020 2020 6372 6561 7465 5f6e 6574        create_net
-0000d3d0: 6364 665f 6469 6d65 6e73 696f 6e73 2864  cdf_dimensions(d
-0000d3e0: 732c 2030 290a 2020 2020 2020 2020 2020  s, 0).          
-0000d3f0: 2020 6372 6561 7465 5f6e 6574 6364 665f    create_netcdf_
-0000d400: 6469 6d65 6e73 696f 6e73 2864 732c 2031  dimensions(ds, 1
-0000d410: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000d420: 2020 2020 7769 7468 2077 7269 7465 5f6d      with write_m
-0000d430: 6f64 756c 652e 4669 6c65 2874 6d70 5f6e  odule.File(tmp_n
-0000d440: 6574 6364 662c 2022 7722 2920 6173 2064  etcdf, "w") as d
-0000d450: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-0000d460: 7265 6174 655f 6835 6e65 7463 6466 5f64  reate_h5netcdf_d
-0000d470: 696d 656e 7369 6f6e 7328 6473 2c20 3029  imensions(ds, 0)
-0000d480: 0a20 2020 2020 2020 2020 2020 2063 7265  .            cre
-0000d490: 6174 655f 6835 6e65 7463 6466 5f64 696d  ate_h5netcdf_dim
-0000d4a0: 656e 7369 6f6e 7328 6473 2c20 3129 0a0a  ensions(ds, 1)..
-0000d4b0: 0a40 7079 7465 7374 2e66 6978 7475 7265  .@pytest.fixture
-0000d4c0: 280a 2020 2020 7061 7261 6d73 3d5b 0a20  (.    params=[. 
-0000d4d0: 2020 2020 2020 205b 6e65 7443 4446 342c         [netCDF4,
-0000d4e0: 206e 6574 4344 4634 5d2c 0a20 2020 2020   netCDF4],.     
-0000d4f0: 2020 205b 6c65 6761 6379 6170 692c 206c     [legacyapi, l
-0000d500: 6567 6163 7961 7069 5d2c 0a20 2020 2020  egacyapi],.     
-0000d510: 2020 205b 6835 6e65 7463 6466 2c20 6835     [h5netcdf, h5
-0000d520: 6e65 7463 6466 5d2c 0a20 2020 2020 2020  netcdf],.       
-0000d530: 205b 6c65 6761 6379 6170 692c 206e 6574   [legacyapi, net
-0000d540: 4344 4634 5d2c 0a20 2020 2020 2020 205b  CDF4],.        [
-0000d550: 6e65 7443 4446 342c 206c 6567 6163 7961  netCDF4, legacya
-0000d560: 7069 5d2c 0a20 2020 2020 2020 205b 6835  pi],.        [h5
-0000d570: 6e65 7463 6466 2c20 6e65 7443 4446 345d  netcdf, netCDF4]
-0000d580: 2c0a 2020 2020 2020 2020 5b6e 6574 4344  ,.        [netCD
-0000d590: 4634 2c20 6835 6e65 7463 6466 5d2c 0a20  F4, h5netcdf],. 
-0000d5a0: 2020 2020 2020 205b 6c65 6761 6379 6170         [legacyap
-0000d5b0: 692c 2068 356e 6574 6364 665d 2c0a 2020  i, h5netcdf],.  
-0000d5c0: 2020 2020 2020 5b68 356e 6574 6364 662c        [h5netcdf,
-0000d5d0: 206c 6567 6163 7961 7069 5d2c 0a20 2020   legacyapi],.   
-0000d5e0: 205d 0a29 0a64 6566 2072 6561 645f 7772   ].).def read_wr
-0000d5f0: 6974 655f 6d61 7472 6978 2872 6571 7565  ite_matrix(reque
-0000d600: 7374 293a 0a20 2020 2070 7269 6e74 2822  st):.    print("
-0000d610: 7772 6974 6520 6d6f 6475 6c65 3a22 2c20  write module:", 
-0000d620: 7265 7175 6573 742e 7061 7261 6d5b 305d  request.param[0]
-0000d630: 2e5f 5f6e 616d 655f 5f29 0a20 2020 2070  .__name__).    p
-0000d640: 7269 6e74 2822 7265 6164 5f6d 6f64 756c  rint("read_modul
-0000d650: 653a 222c 2072 6571 7565 7374 2e70 6172  e:", request.par
-0000d660: 616d 5b31 5d2e 5f5f 6e61 6d65 5f5f 290a  am[1].__name__).
-0000d670: 2020 2020 7265 7475 726e 2072 6571 7565      return reque
-0000d680: 7374 2e70 6172 616d 0a0a 0a64 6566 2074  st.param...def t
-0000d690: 6573 745f 6469 6d65 6e73 696f 6e73 2874  est_dimensions(t
-0000d6a0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-0000d6b0: 2072 6561 645f 7772 6974 655f 6d61 7472   read_write_matr
-0000d6c0: 6978 293a 0a20 2020 2077 7269 7465 5f64  ix):.    write_d
-0000d6d0: 696d 656e 7369 6f6e 7328 746d 705f 6c6f  imensions(tmp_lo
-0000d6e0: 6361 6c5f 6e65 7463 6466 2c20 7265 6164  cal_netcdf, read
-0000d6f0: 5f77 7269 7465 5f6d 6174 7269 785b 305d  _write_matrix[0]
-0000d700: 290a 2020 2020 6368 6563 6b5f 6e65 7463  ).    check_netc
-0000d710: 6466 5f64 696d 656e 7369 6f6e 7328 0a20  df_dimensions(. 
-0000d720: 2020 2020 2020 2074 6d70 5f6c 6f63 616c         tmp_local
-0000d730: 5f6e 6574 6364 662c 2072 6561 645f 7772  _netcdf, read_wr
-0000d740: 6974 655f 6d61 7472 6978 5b30 5d2c 2072  ite_matrix[0], r
-0000d750: 6561 645f 7772 6974 655f 6d61 7472 6978  ead_write_matrix
-0000d760: 5b31 5d0a 2020 2020 290a 0a0a 6465 6620  [1].    )...def 
-0000d770: 7465 7374 5f6e 6f5f 6369 7263 756c 6172  test_no_circular
-0000d780: 5f72 6566 6572 656e 6365 7328 746d 705f  _references(tmp_
-0000d790: 6c6f 6361 6c5f 6e65 7463 6466 293a 0a20  local_netcdf):. 
-0000d7a0: 2020 2023 2068 7474 7073 3a2f 2f67 6974     # https://git
-0000d7b0: 6875 622e 636f 6d2f 6835 7079 2f68 3570  hub.com/h5py/h5p
-0000d7c0: 792f 6973 7375 6573 2f32 3031 390a 2020  y/issues/2019.  
-0000d7d0: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
-0000d7e0: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
-0000d7f0: 6574 6364 662c 2022 7722 2920 6173 2064  etcdf, "w") as d
-0000d800: 733a 0a20 2020 2020 2020 2064 732e 6469  s:.        ds.di
-0000d810: 6d65 6e73 696f 6e73 5b22 7822 5d20 3d20  mensions["x"] = 
-0000d820: 320a 2020 2020 2020 2020 6473 2e64 696d  2.        ds.dim
-0000d830: 656e 7369 6f6e 735b 2279 225d 203d 2032  ensions["y"] = 2
-0000d840: 0a0a 2020 2020 6763 2e63 6f6c 6c65 6374  ..    gc.collect
-0000d850: 2829 0a20 2020 2077 6974 6820 6835 6e65  ().    with h5ne
-0000d860: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
-0000d870: 6361 6c5f 6e65 7463 6466 2c20 2272 2229  cal_netcdf, "r")
-0000d880: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-0000d890: 7265 6673 203d 2067 632e 6765 745f 7265  refs = gc.get_re
-0000d8a0: 6665 7272 6572 7328 6473 290a 2020 2020  ferrers(ds).    
-0000d8b0: 2020 2020 666f 7220 7265 6620 696e 2072      for ref in r
-0000d8c0: 6566 733a 0a20 2020 2020 2020 2020 2020  efs:.           
-0000d8d0: 2070 7269 6e74 2872 6566 290a 2020 2020   print(ref).    
-0000d8e0: 2020 2020 6173 7365 7274 206c 656e 2872      assert len(r
-0000d8f0: 6566 7329 203d 3d20 310a 0a0a 6465 6620  efs) == 1...def 
-0000d900: 7465 7374 5f65 7870 616e 6465 645f 7661  test_expanded_va
-0000d910: 7269 6162 6c65 735f 6e65 7463 6466 3428  riables_netcdf4(
-0000d920: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000d930: 2c20 6e65 7463 6466 5f77 7269 7465 5f6d  , netcdf_write_m
-0000d940: 6f64 756c 6529 3a0a 2020 2020 2320 7061  odule):.    # pa
-0000d950: 7274 6961 6c6c 7920 7265 696d 706c 656d  rtially reimplem
-0000d960: 656e 7465 6420 6475 6520 746f 2070 6572  ented due to per
-0000d970: 666f 726d 616e 6365 2072 6561 736f 6e20  formance reason 
-0000d980: 696e 2065 6467 6520 6361 7365 730a 2020  in edge cases.  
-0000d990: 2020 2320 6874 7470 733a 2f2f 6769 7468    # https://gith
-0000d9a0: 7562 2e63 6f6d 2f68 356e 6574 6364 662f  ub.com/h5netcdf/
-0000d9b0: 6835 6e65 7463 6466 2f69 7373 7565 732f  h5netcdf/issues/
-0000d9c0: 3138 320a 0a20 2020 2077 6974 6820 6e65  182..    with ne
-0000d9d0: 7463 6466 5f77 7269 7465 5f6d 6f64 756c  tcdf_write_modul
-0000d9e0: 652e 4461 7461 7365 7428 746d 705f 6c6f  e.Dataset(tmp_lo
-0000d9f0: 6361 6c5f 6e65 7463 6466 2c20 2277 2229  cal_netcdf, "w")
-0000da00: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-0000da10: 6620 3d20 6473 2e63 7265 6174 6547 726f  f = ds.createGro
-0000da20: 7570 2822 7465 7374 2229 0a20 2020 2020  up("test").     
-0000da30: 2020 2066 2e63 7265 6174 6544 696d 656e     f.createDimen
-0000da40: 7369 6f6e 2822 7822 2c20 4e6f 6e65 290a  sion("x", None).
-0000da50: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
-0000da60: 4469 6d65 6e73 696f 6e28 2279 222c 2033  Dimension("y", 3
-0000da70: 290a 0a20 2020 2020 2020 2064 756d 6d79  )..        dummy
-0000da80: 3120 3d20 662e 6372 6561 7465 5661 7269  1 = f.createVari
-0000da90: 6162 6c65 2822 6475 6d6d 7931 222c 2066  able("dummy1", f
-0000daa0: 6c6f 6174 2c20 2822 7822 2c20 2279 2229  loat, ("x", "y")
-0000dab0: 290a 2020 2020 2020 2020 6475 6d6d 7932  ).        dummy2
-0000dac0: 203d 2066 2e63 7265 6174 6556 6172 6961   = f.createVaria
-0000dad0: 626c 6528 2264 756d 6d79 3222 2c20 666c  ble("dummy2", fl
-0000dae0: 6f61 742c 2028 2278 222c 2022 7922 2929  oat, ("x", "y"))
-0000daf0: 0a20 2020 2020 2020 2064 756d 6d79 3320  .        dummy3 
-0000db00: 3d20 662e 6372 6561 7465 5661 7269 6162  = f.createVariab
-0000db10: 6c65 2822 6475 6d6d 7933 222c 2066 6c6f  le("dummy3", flo
-0000db20: 6174 2c20 2822 7822 2c20 2279 2229 290a  at, ("x", "y")).
-0000db30: 2020 2020 2020 2020 6475 6d6d 7934 203d          dummy4 =
-0000db40: 2066 2e63 7265 6174 6556 6172 6961 626c   f.createVariabl
-0000db50: 6528 2264 756d 6d79 3422 2c20 666c 6f61  e("dummy4", floa
-0000db60: 742c 2028 2278 222c 2022 7922 2929 0a0a  t, ("x", "y"))..
-0000db70: 2020 2020 2020 2020 6475 6d6d 7931 5b3a          dummy1[:
-0000db80: 5d20 3d20 5b5b 312c 2032 2c20 335d 2c20  ] = [[1, 2, 3], 
-0000db90: 5b34 2c20 352c 2036 5d2c 205b 372c 2038  [4, 5, 6], [7, 8
-0000dba0: 2c20 395d 5d0a 2020 2020 2020 2020 6475  , 9]].        du
-0000dbb0: 6d6d 7932 5b31 2c20 3a5d 203d 205b 342c  mmy2[1, :] = [4,
-0000dbc0: 2035 2c20 365d 0a20 2020 2020 2020 2064   5, 6].        d
-0000dbd0: 756d 6d79 335b 303a 322c 203a 5d20 3d20  ummy3[0:2, :] = 
-0000dbe0: 5b5b 312c 2032 2c20 335d 2c20 5b34 2c20  [[1, 2, 3], [4, 
-0000dbf0: 352c 2036 5d5d 0a0a 2020 2020 2020 2020  5, 6]]..        
-0000dc00: 2320 646f 6e27 7420 6d61 736b 2c20 7369  # don't mask, si
-0000dc10: 6e63 6520 6835 6e65 7463 6466 2064 6f65  nce h5netcdf doe
-0000dc20: 736e 2774 2064 6f20 6d61 736b 696e 670a  sn't do masking.
-0000dc30: 2020 2020 2020 2020 6966 206e 6574 6364          if netcd
-0000dc40: 665f 7772 6974 655f 6d6f 6475 6c65 203d  f_write_module =
-0000dc50: 3d20 6e65 7443 4446 343a 0a20 2020 2020  = netCDF4:.     
-0000dc60: 2020 2020 2020 2064 732e 7365 745f 6175         ds.set_au
-0000dc70: 746f 5f6d 6173 6b28 4661 6c73 6529 0a0a  to_mask(False)..
-0000dc80: 2020 2020 2020 2020 7265 7331 203d 2064          res1 = d
-0000dc90: 756d 6d79 315b 3a5d 0a20 2020 2020 2020  ummy1[:].       
-0000dca0: 2072 6573 3220 3d20 6475 6d6d 7932 5b3a   res2 = dummy2[:
-0000dcb0: 5d0a 2020 2020 2020 2020 7265 7333 203d  ].        res3 =
-0000dcc0: 2064 756d 6d79 335b 3a5d 0a20 2020 2020   dummy3[:].     
-0000dcd0: 2020 2072 6573 3420 3d20 6475 6d6d 7934     res4 = dummy4
-0000dce0: 5b3a 5d0a 0a20 2020 2077 6974 6820 6e65  [:]..    with ne
-0000dcf0: 7443 4446 342e 4461 7461 7365 7428 746d  tCDF4.Dataset(tm
-0000dd00: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-0000dd10: 2272 2229 2061 7320 6473 3a0a 2020 2020  "r") as ds:.    
-0000dd20: 2020 2020 2320 646f 6e27 7420 6d61 736b      # don't mask
-0000dd30: 2c20 7369 6e63 6520 6835 6e65 7463 6466  , since h5netcdf
-0000dd40: 2064 6f65 736e 2774 2064 6f20 6d61 736b   doesn't do mask
-0000dd50: 696e 670a 2020 2020 2020 2020 6966 206e  ing.        if n
-0000dd60: 6574 6364 665f 7772 6974 655f 6d6f 6475  etcdf_write_modu
-0000dd70: 6c65 203d 3d20 6e65 7443 4446 343a 0a20  le == netCDF4:. 
-0000dd80: 2020 2020 2020 2020 2020 2064 732e 7365             ds.se
-0000dd90: 745f 6175 746f 5f6d 6173 6b28 4661 6c73  t_auto_mask(Fals
-0000dda0: 6529 0a0a 2020 2020 2020 2020 6620 3d20  e)..        f = 
-0000ddb0: 6473 5b22 7465 7374 225d 0a0a 2020 2020  ds["test"]..    
-0000ddc0: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
-0000ddd0: 7373 6572 745f 616c 6c63 6c6f 7365 2866  ssert_allclose(f
-0000dde0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000ddf0: 7931 225d 5b3a 5d2c 2072 6573 3129 0a20  y1"][:], res1). 
-0000de00: 2020 2020 2020 206e 702e 7465 7374 696e         np.testin
-0000de10: 672e 6173 7365 7274 5f61 6c6c 636c 6f73  g.assert_allclos
-0000de20: 6528 662e 7661 7269 6162 6c65 735b 2264  e(f.variables["d
-0000de30: 756d 6d79 3122 5d5b 312c 203a 5d2c 205b  ummy1"][1, :], [
-0000de40: 342e 302c 2035 2e30 2c20 362e 305d 290a  4.0, 5.0, 6.0]).
-0000de50: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
-0000de60: 6e67 2e61 7373 6572 745f 616c 6c63 6c6f  ng.assert_allclo
-0000de70: 7365 2866 2e76 6172 6961 626c 6573 5b22  se(f.variables["
-0000de80: 6475 6d6d 7931 225d 5b31 3a32 2c20 3a5d  dummy1"][1:2, :]
-0000de90: 2c20 5b5b 342e 302c 2035 2e30 2c20 362e  , [[4.0, 5.0, 6.
-0000dea0: 305d 5d29 0a20 2020 2020 2020 2061 7373  0]]).        ass
-0000deb0: 6572 7420 662e 7661 7269 6162 6c65 735b  ert f.variables[
-0000dec0: 2264 756d 6d79 3122 5d2e 7368 6170 6520  "dummy1"].shape 
-0000ded0: 3d3d 2028 332c 2033 290a 2020 2020 2020  == (3, 3).      
-0000dee0: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
-0000def0: 6572 745f 616c 6c63 6c6f 7365 2866 2e76  ert_allclose(f.v
-0000df00: 6172 6961 626c 6573 5b22 6475 6d6d 7932  ariables["dummy2
-0000df10: 225d 5b3a 5d2c 2072 6573 3229 0a20 2020  "][:], res2).   
-0000df20: 2020 2020 206e 702e 7465 7374 696e 672e       np.testing.
-0000df30: 6173 7365 7274 5f61 6c6c 636c 6f73 6528  assert_allclose(
-0000df40: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-0000df50: 6d79 3222 5d5b 312c 203a 5d2c 205b 342e  my2"][1, :], [4.
-0000df60: 302c 2035 2e30 2c20 362e 305d 290a 2020  0, 5.0, 6.0]).  
-0000df70: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
-0000df80: 2e61 7373 6572 745f 616c 6c63 6c6f 7365  .assert_allclose
-0000df90: 2866 2e76 6172 6961 626c 6573 5b22 6475  (f.variables["du
-0000dfa0: 6d6d 7932 225d 5b31 3a32 2c20 3a5d 2c20  mmy2"][1:2, :], 
-0000dfb0: 5b5b 342e 302c 2035 2e30 2c20 362e 305d  [[4.0, 5.0, 6.0]
-0000dfc0: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0000dfd0: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
-0000dfe0: 756d 6d79 3222 5d2e 7368 6170 6520 3d3d  ummy2"].shape ==
-0000dff0: 2028 332c 2033 290a 2020 2020 2020 2020   (3, 3).        
-0000e000: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
-0000e010: 745f 616c 6c63 6c6f 7365 2866 2e76 6172  t_allclose(f.var
-0000e020: 6961 626c 6573 5b22 6475 6d6d 7933 225d  iables["dummy3"]
-0000e030: 5b3a 5d2c 2072 6573 3329 0a20 2020 2020  [:], res3).     
-0000e040: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
-0000e050: 7365 7274 5f61 6c6c 636c 6f73 6528 662e  sert_allclose(f.
-0000e060: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
-0000e070: 3322 5d5b 312c 203a 5d2c 205b 342e 302c  3"][1, :], [4.0,
-0000e080: 2035 2e30 2c20 362e 305d 290a 2020 2020   5.0, 6.0]).    
-0000e090: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
-0000e0a0: 7373 6572 745f 616c 6c63 6c6f 7365 2866  ssert_allclose(f
-0000e0b0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000e0c0: 7933 225d 5b31 3a32 2c20 3a5d 2c20 5b5b  y3"][1:2, :], [[
-0000e0d0: 342e 302c 2035 2e30 2c20 362e 305d 5d29  4.0, 5.0, 6.0]])
-0000e0e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000e0f0: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-0000e100: 6d79 3322 5d2e 7368 6170 6520 3d3d 2028  my3"].shape == (
-0000e110: 332c 2033 290a 2020 2020 2020 2020 6e70  3, 3).        np
-0000e120: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
-0000e130: 616c 6c63 6c6f 7365 2866 2e76 6172 6961  allclose(f.varia
-0000e140: 626c 6573 5b22 6475 6d6d 7934 225d 5b3a  bles["dummy4"][:
-0000e150: 5d2c 2072 6573 3429 0a20 2020 2020 2020  ], res4).       
+0000ac10: 735b 2278 225d 2e69 7375 6e6c 696d 6974  s["x"].isunlimit
+0000ac20: 6564 2829 0a20 2020 2020 2020 2061 7373  ed().        ass
+0000ac30: 6572 7420 662e 6469 6d65 6e73 696f 6e73  ert f.dimensions
+0000ac40: 5b22 7922 5d2e 7369 7a65 203d 3d20 320a  ["y"].size == 2.
+0000ac50: 2020 2020 2020 2020 6966 2076 6572 7369          if versi
+0000ac60: 6f6e 2e70 6172 7365 2868 3570 792e 5f5f  on.parse(h5py.__
+0000ac70: 7665 7273 696f 6e5f 5f29 203e 3d20 7665  version__) >= ve
+0000ac80: 7273 696f 6e2e 7061 7273 6528 2233 2e37  rsion.parse("3.7
+0000ac90: 2e30 2229 3a0a 2020 2020 2020 2020 2020  .0"):.          
+0000aca0: 2020 6173 7365 7274 206c 6973 7428 662e    assert list(f.
+0000acb0: 7661 7269 6162 6c65 7329 203d 3d20 5b22  variables) == ["
+0000acc0: 7465 7374 222c 2022 7922 5d0a 2020 2020  test", "y"].    
+0000acd0: 2020 2020 2020 2020 6173 7365 7274 206c          assert l
+0000ace0: 6973 7428 662e 5f68 3567 726f 7570 2e6b  ist(f._h5group.k
+0000acf0: 6579 7328 2929 203d 3d20 5b22 7822 2c20  eys()) == ["x", 
+0000ad00: 2279 222c 2022 7465 7374 222c 2022 5f6e  "y", "test", "_n
+0000ad10: 6334 5f6e 6f6e 5f63 6f6f 7264 5f79 225d  c4_non_coord_y"]
+0000ad20: 0a0a 2020 2020 7769 7468 2068 356e 6574  ..    with h5net
+0000ad30: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
+0000ad40: 616c 5f6e 6574 6364 662c 2022 7722 2920  al_netcdf, "w") 
+0000ad50: 6173 2066 3a0a 2020 2020 2020 2020 662e  as f:.        f.
+0000ad60: 6469 6d65 6e73 696f 6e73 203d 207b 2278  dimensions = {"x
+0000ad70: 223a 204e 6f6e 652c 2022 7922 3a20 327d  ": None, "y": 2}
+0000ad80: 0a20 2020 2020 2020 2066 2e63 7265 6174  .        f.creat
+0000ad90: 655f 7661 7269 6162 6c65 2822 7922 2c20  e_variable("y", 
+0000ada0: 6469 6d65 6e73 696f 6e73 3d28 2278 222c  dimensions=("x",
+0000adb0: 292c 2064 7479 7065 3d6e 702e 696e 7436  ), dtype=np.int6
+0000adc0: 3429 0a20 2020 2020 2020 2066 2e63 7265  4).        f.cre
+0000add0: 6174 655f 7661 7269 6162 6c65 2822 7465  ate_variable("te
+0000ade0: 7374 222c 2064 696d 656e 7369 6f6e 733d  st", dimensions=
+0000adf0: 2822 7822 2c29 2c20 6474 7970 653d 6e70  ("x",), dtype=np
+0000ae00: 2e69 6e74 3634 290a 0a20 2020 2077 6974  .int64)..    wit
+0000ae10: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+0000ae20: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000ae30: 2c20 2272 2229 2061 7320 663a 0a20 2020  , "r") as f:.   
+0000ae40: 2020 2020 2061 7373 6572 7420 6c69 7374       assert list
+0000ae50: 2866 2e64 696d 656e 7369 6f6e 7329 203d  (f.dimensions) =
+0000ae60: 3d20 5b22 7822 2c20 2279 225d 0a20 2020  = ["x", "y"].   
+0000ae70: 2020 2020 2061 7373 6572 7420 662e 6469       assert f.di
+0000ae80: 6d65 6e73 696f 6e73 5b22 7822 5d2e 7369  mensions["x"].si
+0000ae90: 7a65 203d 3d20 300a 2020 2020 2020 2020  ze == 0.        
+0000aea0: 6173 7365 7274 2066 2e64 696d 656e 7369  assert f.dimensi
+0000aeb0: 6f6e 735b 2278 225d 2e69 7375 6e6c 696d  ons["x"].isunlim
+0000aec0: 6974 6564 2829 0a20 2020 2020 2020 2061  ited().        a
+0000aed0: 7373 6572 7420 662e 6469 6d65 6e73 696f  ssert f.dimensio
+0000aee0: 6e73 5b22 7922 5d2e 7369 7a65 203d 3d20  ns["y"].size == 
+0000aef0: 320a 2020 2020 2020 2020 6966 2076 6572  2.        if ver
+0000af00: 7369 6f6e 2e70 6172 7365 2868 3570 792e  sion.parse(h5py.
+0000af10: 5f5f 7665 7273 696f 6e5f 5f29 203e 3d20  __version__) >= 
+0000af20: 7665 7273 696f 6e2e 7061 7273 6528 2233  version.parse("3
+0000af30: 2e37 2e30 2229 3a0a 2020 2020 2020 2020  .7.0"):.        
+0000af40: 2020 2020 6173 7365 7274 206c 6973 7428      assert list(
+0000af50: 662e 7661 7269 6162 6c65 7329 203d 3d20  f.variables) == 
+0000af60: 5b22 7922 2c20 2274 6573 7422 5d0a 2020  ["y", "test"].  
+0000af70: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000af80: 206c 6973 7428 662e 5f68 3567 726f 7570   list(f._h5group
+0000af90: 2e6b 6579 7328 2929 203d 3d20 5b22 7822  .keys()) == ["x"
+0000afa0: 2c20 2279 222c 2022 5f6e 6334 5f6e 6f6e  , "y", "_nc4_non
+0000afb0: 5f63 6f6f 7264 5f79 222c 2022 7465 7374  _coord_y", "test
+0000afc0: 225d 0a0a 0a64 6566 2074 6573 745f 6f76  "]...def test_ov
+0000afd0: 6572 7772 6974 655f 6578 6973 7469 6e67  erwrite_existing
+0000afe0: 5f66 696c 6528 746d 705f 6c6f 6361 6c5f  _file(tmp_local_
+0000aff0: 6e65 7463 6466 293a 0a20 2020 2023 2063  netcdf):.    # c
+0000b000: 7265 6174 6520 6669 6c65 2077 6974 6820  reate file with 
+0000b010: 5f4e 4350 726f 7065 7274 6965 7320 6174  _NCProperties at
+0000b020: 7472 6962 7574 650a 2020 2020 7769 7468  tribute.    with
+0000b030: 206e 6574 4344 4634 2e44 6174 6173 6574   netCDF4.Dataset
+0000b040: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000b050: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
+0000b060: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+0000b070: 4469 6d65 6e73 696f 6e28 2278 222c 2031  Dimension("x", 1
+0000b080: 3029 0a0a 2020 2020 2320 6368 6563 6b20  0)..    # check 
+0000b090: 6174 7472 6962 7574 650a 2020 2020 7769  attribute.    wi
+0000b0a0: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
+0000b0b0: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000b0c0: 662c 2022 7222 2920 6173 2064 733a 0a20  f, "r") as ds:. 
+0000b0d0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+0000b0e0: 2e61 7474 7273 2e5f 6835 6174 7472 732e  .attrs._h5attrs.
+0000b0f0: 6765 7428 225f 4e43 5072 6f70 6572 7469  get("_NCProperti
+0000b100: 6573 222c 2046 616c 7365 290a 0a20 2020  es", False)..   
+0000b110: 2023 206f 7665 7277 7269 7465 2066 696c   # overwrite fil
+0000b120: 6520 7769 7468 206c 6567 6163 7961 7069  e with legacyapi
+0000b130: 0a20 2020 2077 6974 6820 6c65 6761 6379  .    with legacy
+0000b140: 6170 692e 4461 7461 7365 7428 746d 705f  api.Dataset(tmp_
+0000b150: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2277  local_netcdf, "w
+0000b160: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
+0000b170: 2020 6473 2e63 7265 6174 6544 696d 656e    ds.createDimen
+0000b180: 7369 6f6e 2822 7822 2c20 3130 290a 0a20  sion("x", 10).. 
+0000b190: 2020 2023 2063 6865 636b 2061 7474 7269     # check attri
+0000b1a0: 6275 7465 0a20 2020 2077 6974 6820 6835  bute.    with h5
+0000b1b0: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+0000b1c0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
+0000b1d0: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
+0000b1e0: 2020 6173 7365 7274 2064 732e 6174 7472    assert ds.attr
+0000b1f0: 732e 5f68 3561 7474 7273 2e67 6574 2822  s._h5attrs.get("
+0000b200: 5f4e 4350 726f 7065 7274 6965 7322 2c20  _NCProperties", 
+0000b210: 4661 6c73 6529 0a0a 2020 2020 2320 6f76  False)..    # ov
+0000b220: 6572 7772 6974 6520 6669 6c65 2077 6974  erwrite file wit
+0000b230: 6820 6e65 7720 6170 690a 2020 2020 7769  h new api.    wi
+0000b240: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
+0000b250: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000b260: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
+0000b270: 2020 2020 2020 2064 732e 6469 6d65 6e73         ds.dimens
+0000b280: 696f 6e73 5b22 7822 5d20 3d20 3130 0a0a  ions["x"] = 10..
+0000b290: 2020 2020 2320 6368 6563 6b20 6174 7472      # check attr
+0000b2a0: 6962 7574 650a 2020 2020 7769 7468 2068  ibute.    with h
+0000b2b0: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
+0000b2c0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
+0000b2d0: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
+0000b2e0: 2020 2061 7373 6572 7420 6473 2e61 7474     assert ds.att
+0000b2f0: 7273 2e5f 6835 6174 7472 732e 6765 7428  rs._h5attrs.get(
+0000b300: 225f 4e43 5072 6f70 6572 7469 6573 222c  "_NCProperties",
+0000b310: 2046 616c 7365 290a 0a0a 6465 6620 7465   False)...def te
+0000b320: 7374 5f73 6361 6c65 735f 6f6e 5f61 7070  st_scales_on_app
+0000b330: 656e 6428 746d 705f 6c6f 6361 6c5f 6e65  end(tmp_local_ne
+0000b340: 7463 6466 293a 0a20 2020 2023 2063 7265  tcdf):.    # cre
+0000b350: 6174 6520 6669 6c65 2077 6974 6820 5f4e  ate file with _N
+0000b360: 4350 726f 7065 7274 6965 7320 6174 7472  CProperties attr
+0000b370: 6962 7574 650a 2020 2020 7769 7468 206e  ibute.    with n
+0000b380: 6574 4344 4634 2e44 6174 6173 6574 2874  etCDF4.Dataset(t
+0000b390: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+0000b3a0: 2022 7722 2920 6173 2064 733a 0a20 2020   "w") as ds:.   
+0000b3b0: 2020 2020 2064 732e 6372 6561 7465 4469       ds.createDi
+0000b3c0: 6d65 6e73 696f 6e28 2278 222c 2031 3029  mension("x", 10)
+0000b3d0: 0a0a 2020 2020 2320 6170 7065 6e64 2066  ..    # append f
+0000b3e0: 696c 6520 7769 7468 206e 6574 4344 4634  ile with netCDF4
+0000b3f0: 0a20 2020 2077 6974 6820 6e65 7443 4446  .    with netCDF
+0000b400: 342e 4461 7461 7365 7428 746d 705f 6c6f  4.Dataset(tmp_lo
+0000b410: 6361 6c5f 6e65 7463 6466 2c20 2272 2b22  cal_netcdf, "r+"
+0000b420: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
+0000b430: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
+0000b440: 6c65 2822 7465 7374 222c 2022 6934 222c  le("test", "i4",
+0000b450: 2028 2278 222c 2929 0a0a 2020 2020 2320   ("x",))..    # 
+0000b460: 6368 6563 6b20 7363 616c 6573 0a20 2020  check scales.   
+0000b470: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+0000b480: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
+0000b490: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
+0000b4a0: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+0000b4b0: 2064 732e 7661 7269 6162 6c65 735b 2274   ds.variables["t
+0000b4c0: 6573 7422 5d2e 6174 7472 732e 5f68 3561  est"].attrs._h5a
+0000b4d0: 7474 7273 2e67 6574 2822 4449 4d45 4e53  ttrs.get("DIMENS
+0000b4e0: 494f 4e5f 4c49 5354 222c 2046 616c 7365  ION_LIST", False
+0000b4f0: 290a 0a20 2020 2023 2061 7070 656e 6420  )..    # append 
+0000b500: 6669 6c65 2077 6974 6820 6c65 6761 6379  file with legacy
+0000b510: 6170 690a 2020 2020 7769 7468 206c 6567  api.    with leg
+0000b520: 6163 7961 7069 2e44 6174 6173 6574 2874  acyapi.Dataset(t
+0000b530: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+0000b540: 2022 722b 2229 2061 7320 6473 3a0a 2020   "r+") as ds:.  
+0000b550: 2020 2020 2020 6473 2e63 7265 6174 6556        ds.createV
+0000b560: 6172 6961 626c 6528 2274 6573 7431 222c  ariable("test1",
+0000b570: 2022 6934 222c 2028 2278 222c 2929 0a0a   "i4", ("x",))..
+0000b580: 2020 2020 2320 6368 6563 6b20 7363 616c      # check scal
+0000b590: 6573 0a20 2020 2077 6974 6820 6835 6e65  es.    with h5ne
+0000b5a0: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+0000b5b0: 6361 6c5f 6e65 7463 6466 2c20 2272 2229  cal_netcdf, "r")
+0000b5c0: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
+0000b5d0: 6173 7365 7274 2064 732e 7661 7269 6162  assert ds.variab
+0000b5e0: 6c65 735b 2274 6573 7431 225d 2e61 7474  les["test1"].att
+0000b5f0: 7273 2e5f 6835 6174 7472 732e 6765 7428  rs._h5attrs.get(
+0000b600: 2244 494d 454e 5349 4f4e 5f4c 4953 5422  "DIMENSION_LIST"
+0000b610: 2c20 4661 6c73 6529 0a0a 0a64 6566 2063  , False)...def c
+0000b620: 7265 6174 655f 6174 7461 6368 5f73 6361  reate_attach_sca
+0000b630: 6c65 7328 6669 6c65 6e61 6d65 2c20 6170  les(filename, ap
+0000b640: 7065 6e64 5f6d 6f64 756c 6529 3a0a 2020  pend_module):.  
+0000b650: 2020 2320 6372 6561 7465 2066 696c 6520    # create file 
+0000b660: 7769 7468 206e 6574 4344 4634 0a20 2020  with netCDF4.   
+0000b670: 2077 6974 6820 6e65 7443 4446 342e 4461   with netCDF4.Da
+0000b680: 7461 7365 7428 6669 6c65 6e61 6d65 2c20  taset(filename, 
+0000b690: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
+0000b6a0: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
+0000b6b0: 656e 7369 6f6e 2822 7822 2c20 3029 0a20  ension("x", 0). 
+0000b6c0: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+0000b6d0: 4469 6d65 6e73 696f 6e28 2279 222c 2031  Dimension("y", 1
+0000b6e0: 290a 2020 2020 2020 2020 6473 2e63 7265  ).        ds.cre
+0000b6f0: 6174 6556 6172 6961 626c 6528 2274 6573  ateVariable("tes
+0000b700: 7422 2c20 2269 3422 2c20 2822 7822 2c29  t", "i4", ("x",)
+0000b710: 290a 2020 2020 2020 2020 6473 2e76 6172  ).        ds.var
+0000b720: 6961 626c 6573 5b22 7465 7374 225d 203d  iables["test"] =
+0000b730: 206e 702e 6f6e 6573 2828 3130 2c29 290a   np.ones((10,)).
+0000b740: 0a20 2020 2023 2061 7070 656e 6420 6669  .    # append fi
+0000b750: 6c65 2077 6974 6820 6e65 7443 4446 340a  le with netCDF4.
+0000b760: 2020 2020 7769 7468 2061 7070 656e 645f      with append_
+0000b770: 6d6f 6475 6c65 2e44 6174 6173 6574 2866  module.Dataset(f
+0000b780: 696c 656e 616d 652c 2022 6122 2920 6173  ilename, "a") as
+0000b790: 2064 733a 0a20 2020 2020 2020 2064 732e   ds:.        ds.
+0000b7a0: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
+0000b7b0: 7465 7374 3122 2c20 2269 3422 2c20 2822  test1", "i4", ("
+0000b7c0: 7822 2c29 290a 2020 2020 2020 2020 6473  x",)).        ds
+0000b7d0: 2e63 7265 6174 6556 6172 6961 626c 6528  .createVariable(
+0000b7e0: 2279 222c 2022 6934 222c 2028 2278 222c  "y", "i4", ("x",
+0000b7f0: 2022 7922 2929 0a0a 2020 2020 2320 6368   "y"))..    # ch
+0000b800: 6563 6b20 7363 616c 6573 0a20 2020 2077  eck scales.    w
+0000b810: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
+0000b820: 6528 6669 6c65 6e61 6d65 2c20 2272 2229  e(filename, "r")
+0000b830: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
+0000b840: 7265 6673 203d 2064 732e 5f68 3567 726f  refs = ds._h5gro
+0000b850: 7570 5b22 7822 5d2e 6174 7472 732e 6765  up["x"].attrs.ge
+0000b860: 7428 2252 4546 4552 454e 4345 5f4c 4953  t("REFERENCE_LIS
+0000b870: 5422 2c20 4661 6c73 6529 0a20 2020 2020  T", False).     
+0000b880: 2020 2061 7373 6572 7420 6c65 6e28 7265     assert len(re
+0000b890: 6673 2920 3d3d 2033 0a20 2020 2020 2020  fs) == 3.       
+0000b8a0: 2066 6f72 2028 7265 662c 2064 696d 292c   for (ref, dim),
+0000b8b0: 206e 616d 6520 696e 207a 6970 2872 6566   name in zip(ref
+0000b8c0: 732c 205b 222f 7465 7374 222c 2022 2f74  s, ["/test", "/t
+0000b8d0: 6573 7431 222c 2022 2f5f 6e63 345f 6e6f  est1", "/_nc4_no
+0000b8e0: 6e5f 636f 6f72 645f 7922 5d29 3a0a 2020  n_coord_y"]):.  
+0000b8f0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000b900: 2064 696d 203d 3d20 300a 2020 2020 2020   dim == 0.      
+0000b910: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+0000b920: 5f72 6f6f 742e 5f68 3566 696c 655b 7265  _root._h5file[re
+0000b930: 665d 2e6e 616d 6520 3d3d 206e 616d 650a  f].name == name.
+0000b940: 0a0a 6465 6620 7465 7374 5f63 7265 6174  ..def test_creat
+0000b950: 655f 6174 7461 6368 5f73 6361 6c65 735f  e_attach_scales_
+0000b960: 6e65 7463 6466 3428 746d 705f 6c6f 6361  netcdf4(tmp_loca
+0000b970: 6c5f 6e65 7463 6466 293a 0a20 2020 2063  l_netcdf):.    c
+0000b980: 7265 6174 655f 6174 7461 6368 5f73 6361  reate_attach_sca
+0000b990: 6c65 7328 746d 705f 6c6f 6361 6c5f 6e65  les(tmp_local_ne
+0000b9a0: 7463 6466 2c20 6e65 7443 4446 3429 0a0a  tcdf, netCDF4)..
+0000b9b0: 0a64 6566 2074 6573 745f 6372 6561 7465  .def test_create
+0000b9c0: 5f61 7474 6163 685f 7363 616c 6573 5f6c  _attach_scales_l
+0000b9d0: 6567 6163 7961 7069 2874 6d70 5f6c 6f63  egacyapi(tmp_loc
+0000b9e0: 616c 5f6e 6574 6364 6629 3a0a 2020 2020  al_netcdf):.    
+0000b9f0: 6372 6561 7465 5f61 7474 6163 685f 7363  create_attach_sc
+0000ba00: 616c 6573 2874 6d70 5f6c 6f63 616c 5f6e  ales(tmp_local_n
+0000ba10: 6574 6364 662c 206c 6567 6163 7961 7069  etcdf, legacyapi
+0000ba20: 290a 0a0a 6465 6620 7465 7374 5f64 6574  )...def test_det
+0000ba30: 6163 685f 7363 616c 6528 746d 705f 6c6f  ach_scale(tmp_lo
+0000ba40: 6361 6c5f 6e65 7463 6466 293a 0a20 2020  cal_netcdf):.   
+0000ba50: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+0000ba60: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
+0000ba70: 7463 6466 2c20 2277 2229 2061 7320 6473  tcdf, "w") as ds
+0000ba80: 3a0a 2020 2020 2020 2020 6473 2e64 696d  :.        ds.dim
+0000ba90: 656e 7369 6f6e 735b 2278 225d 203d 2032  ensions["x"] = 2
+0000baa0: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
+0000bab0: 6e73 696f 6e73 5b22 7922 5d20 3d20 320a  nsions["y"] = 2.
+0000bac0: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
+0000bad0: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
+0000bae0: 6c5f 6e65 7463 6466 2c20 2261 2229 2061  l_netcdf, "a") a
+0000baf0: 7320 6473 3a0a 2020 2020 2020 2020 6473  s ds:.        ds
+0000bb00: 2e63 7265 6174 655f 7661 7269 6162 6c65  .create_variable
+0000bb10: 2822 7465 7374 222c 2064 696d 656e 7369  ("test", dimensi
+0000bb20: 6f6e 733d 2822 7822 2c29 2c20 6474 7970  ons=("x",), dtyp
+0000bb30: 653d 6e70 2e69 6e74 3634 290a 0a20 2020  e=np.int64)..   
+0000bb40: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+0000bb50: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
+0000bb60: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
+0000bb70: 3a0a 2020 2020 2020 2020 7265 6673 203d  :.        refs =
+0000bb80: 2064 732e 5f68 3567 726f 7570 5b22 7822   ds._h5group["x"
+0000bb90: 5d2e 6174 7472 732e 6765 7428 2252 4546  ].attrs.get("REF
+0000bba0: 4552 454e 4345 5f4c 4953 5422 2c20 4661  ERENCE_LIST", Fa
+0000bbb0: 6c73 6529 0a20 2020 2020 2020 2061 7373  lse).        ass
+0000bbc0: 6572 7420 6c65 6e28 7265 6673 2920 3d3d  ert len(refs) ==
+0000bbd0: 2031 0a20 2020 2020 2020 2066 6f72 2028   1.        for (
+0000bbe0: 7265 662c 2064 696d 292c 206e 616d 6520  ref, dim), name 
+0000bbf0: 696e 207a 6970 2872 6566 732c 205b 222f  in zip(refs, ["/
+0000bc00: 7465 7374 225d 293a 0a20 2020 2020 2020  test"]):.       
+0000bc10: 2020 2020 2061 7373 6572 7420 6469 6d20       assert dim 
+0000bc20: 3d3d 2030 0a20 2020 2020 2020 2020 2020  == 0.           
+0000bc30: 2061 7373 6572 7420 6473 2e5f 726f 6f74   assert ds._root
+0000bc40: 2e5f 6835 6669 6c65 5b72 6566 5d2e 6e61  ._h5file[ref].na
+0000bc50: 6d65 203d 3d20 6e61 6d65 0a0a 2020 2020  me == name..    
+0000bc60: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+0000bc70: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+0000bc80: 6364 662c 2022 6122 2920 6173 2064 733a  cdf, "a") as ds:
+0000bc90: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
+0000bca0: 6e73 696f 6e73 5b22 7822 5d2e 5f64 6574  nsions["x"]._det
+0000bcb0: 6163 685f 7363 616c 6528 290a 0a20 2020  ach_scale()..   
+0000bcc0: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+0000bcd0: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
+0000bce0: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
+0000bcf0: 3a0a 2020 2020 2020 2020 7265 6673 203d  :.        refs =
+0000bd00: 2064 732e 5f68 3567 726f 7570 5b22 7822   ds._h5group["x"
+0000bd10: 5d2e 6174 7472 732e 6765 7428 2252 4546  ].attrs.get("REF
+0000bd20: 4552 454e 4345 5f4c 4953 5422 2c20 4661  ERENCE_LIST", Fa
+0000bd30: 6c73 6529 0a20 2020 2020 2020 2061 7373  lse).        ass
+0000bd40: 6572 7420 6e6f 7420 7265 6673 0a0a 0a64  ert not refs...d
+0000bd50: 6566 2074 6573 745f 6973 5f73 6361 6c65  ef test_is_scale
+0000bd60: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000bd70: 6629 3a0a 2020 2020 7769 7468 206c 6567  f):.    with leg
+0000bd80: 6163 7961 7069 2e44 6174 6173 6574 2874  acyapi.Dataset(t
+0000bd90: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+0000bda0: 2022 7722 2920 6173 2064 733a 0a20 2020   "w") as ds:.   
+0000bdb0: 2020 2020 2064 732e 6372 6561 7465 4469       ds.createDi
+0000bdc0: 6d65 6e73 696f 6e28 2278 222c 2031 3029  mension("x", 10)
+0000bdd0: 0a20 2020 2077 6974 6820 6c65 6761 6379  .    with legacy
+0000bde0: 6170 692e 4461 7461 7365 7428 746d 705f  api.Dataset(tmp_
+0000bdf0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
+0000be00: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
+0000be10: 2020 6173 7365 7274 2064 732e 6469 6d65    assert ds.dime
+0000be20: 6e73 696f 6e73 5b22 7822 5d2e 5f69 7373  nsions["x"]._iss
+0000be30: 6361 6c65 0a0a 0a64 6566 2074 6573 745f  cale...def test_
+0000be40: 6765 745f 6469 6d5f 7363 616c 655f 7265  get_dim_scale_re
+0000be50: 6673 2874 6d70 5f6c 6f63 616c 5f6e 6574  fs(tmp_local_net
+0000be60: 6364 6629 3a0a 2020 2020 7769 7468 206c  cdf):.    with l
+0000be70: 6567 6163 7961 7069 2e44 6174 6173 6574  egacyapi.Dataset
+0000be80: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000be90: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
+0000bea0: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+0000beb0: 4469 6d65 6e73 696f 6e28 2278 222c 2031  Dimension("x", 1
+0000bec0: 3029 0a20 2020 2020 2020 2064 732e 6372  0).        ds.cr
+0000bed0: 6561 7465 5661 7269 6162 6c65 2822 7465  eateVariable("te
+0000bee0: 7374 3022 2c20 2269 3822 2c20 2822 7822  st0", "i8", ("x"
+0000bef0: 2c29 290a 2020 2020 2020 2020 6473 2e63  ,)).        ds.c
+0000bf00: 7265 6174 6556 6172 6961 626c 6528 2274  reateVariable("t
+0000bf10: 6573 7431 222c 2022 6938 222c 2028 2278  est1", "i8", ("x
+0000bf20: 222c 2929 0a20 2020 2077 6974 6820 6c65  ",)).    with le
+0000bf30: 6761 6379 6170 692e 4461 7461 7365 7428  gacyapi.Dataset(
+0000bf40: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000bf50: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+0000bf60: 2020 2020 2020 7265 6673 203d 2064 732e        refs = ds.
+0000bf70: 6469 6d65 6e73 696f 6e73 5b22 7822 5d2e  dimensions["x"].
+0000bf80: 5f73 6361 6c65 5f72 6566 730a 2020 2020  _scale_refs.    
+0000bf90: 2020 2020 6173 7365 7274 2064 732e 5f68      assert ds._h
+0000bfa0: 3566 696c 655b 7265 6673 5b30 5d5b 305d  5file[refs[0][0]
+0000bfb0: 5d20 3d3d 2064 735b 2274 6573 7430 225d  ] == ds["test0"]
+0000bfc0: 2e5f 6835 6473 0a20 2020 2020 2020 2061  ._h5ds.        a
+0000bfd0: 7373 6572 7420 6473 2e5f 6835 6669 6c65  ssert ds._h5file
+0000bfe0: 5b72 6566 735b 315d 5b30 5d5d 203d 3d20  [refs[1][0]] == 
+0000bff0: 6473 5b22 7465 7374 3122 5d2e 5f68 3564  ds["test1"]._h5d
+0000c000: 730a 0a0a 6465 6620 6372 6561 7465 5f6e  s...def create_n
+0000c010: 6574 6364 665f 6469 6d65 6e73 696f 6e73  etcdf_dimensions
+0000c020: 2864 732c 2069 6478 293a 0a20 2020 2023  (ds, idx):.    #
+0000c030: 2064 696d 656e 7369 6f6e 2061 6e64 2076   dimension and v
+0000c040: 6172 6961 626c 6520 7365 7475 7020 6973  ariable setup is
+0000c050: 2061 6461 7074 6564 2066 726f 6d20 7468   adapted from th
+0000c060: 6520 626c 6f67 706f 7374 2061 740a 2020  e blogpost at.  
+0000c070: 2020 2320 6874 7470 733a 2f2f 7777 772e    # https://www.
+0000c080: 756e 6964 6174 612e 7563 6172 2e65 6475  unidata.ucar.edu
+0000c090: 2f62 6c6f 6773 2f64 6576 656c 6f70 6572  /blogs/developer
+0000c0a0: 2f65 6e2f 656e 7472 792f 6e65 7463 6466  /en/entry/netcdf
+0000c0b0: 345f 7368 6172 6564 5f64 696d 656e 7369  4_shared_dimensi
+0000c0c0: 6f6e 730a 2020 2020 6720 3d20 6473 2e63  ons.    g = ds.c
+0000c0d0: 7265 6174 6547 726f 7570 2822 6469 6d74  reateGroup("dimt
+0000c0e0: 6573 7422 202b 2073 7472 2869 6478 2929  est" + str(idx))
+0000c0f0: 0a20 2020 2067 2e63 7265 6174 6544 696d  .    g.createDim
+0000c100: 656e 7369 6f6e 2822 7469 6d65 222c 2030  ension("time", 0
+0000c110: 2920 2023 2074 696d 650a 2020 2020 672e  )  # time.    g.
+0000c120: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+0000c130: 226e 7665 6322 2c20 3520 2b20 6964 7829  "nvec", 5 + idx)
+0000c140: 2020 2320 6e76 6563 0a20 2020 2067 2e63    # nvec.    g.c
+0000c150: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
+0000c160: 7361 6d70 6c65 222c 2032 202b 2069 6478  sample", 2 + idx
+0000c170: 2920 2023 2073 616d 706c 650a 2020 2020  )  # sample.    
+0000c180: 672e 6372 6561 7465 4469 6d65 6e73 696f  g.createDimensio
+0000c190: 6e28 2273 6869 7022 2c20 3320 2b20 6964  n("ship", 3 + id
+0000c1a0: 7829 2020 2320 7368 6970 0a20 2020 2067  x)  # ship.    g
+0000c1b0: 2e63 7265 6174 6544 696d 656e 7369 6f6e  .createDimension
+0000c1c0: 2822 7368 6970 5f73 7472 6c65 6e22 2c20  ("ship_strlen", 
+0000c1d0: 3130 2920 2023 2073 6869 705f 7374 726c  10)  # ship_strl
+0000c1e0: 656e 0a20 2020 2067 2e63 7265 6174 6544  en.    g.createD
+0000c1f0: 696d 656e 7369 6f6e 2822 636f 6c6c 6964  imension("collid
+0000c200: 6522 2c20 3720 2b20 6964 7829 2020 2320  e", 7 + idx)  # 
+0000c210: 636f 6c6c 6964 650a 0a20 2020 2074 696d  collide..    tim
+0000c220: 6520 3d20 672e 6372 6561 7465 5661 7269  e = g.createVari
+0000c230: 6162 6c65 2822 7469 6d65 222c 2022 6638  able("time", "f8
+0000c240: 222c 2028 2274 696d 6522 2c29 290a 2020  ", ("time",)).  
+0000c250: 2020 6461 7461 203d 2067 2e63 7265 6174    data = g.creat
+0000c260: 6556 6172 6961 626c 6528 2264 6174 6122  eVariable("data"
+0000c270: 2c20 2269 3822 2c20 2822 7368 6970 222c  , "i8", ("ship",
+0000c280: 2022 7361 6d70 6c65 222c 2022 7469 6d65   "sample", "time
+0000c290: 222c 2022 6e76 6563 2229 290a 2020 2020  ", "nvec")).    
+0000c2a0: 636f 6c6c 6964 6520 3d20 672e 6372 6561  collide = g.crea
+0000c2b0: 7465 5661 7269 6162 6c65 2822 636f 6c6c  teVariable("coll
+0000c2c0: 6964 6522 2c20 2269 3822 2c20 2822 6e76  ide", "i8", ("nv
+0000c2d0: 6563 222c 2929 0a20 2020 206e 6f6e 5f63  ec",)).    non_c
+0000c2e0: 6f6c 6c69 6465 203d 2067 2e63 7265 6174  ollide = g.creat
+0000c2f0: 6556 6172 6961 626c 6528 226e 6f6e 5f63  eVariable("non_c
+0000c300: 6f6c 6c69 6465 222c 2022 6938 222c 2028  ollide", "i8", (
+0000c310: 226e 7665 6322 2c29 290a 2020 2020 7368  "nvec",)).    sh
+0000c320: 6970 203d 2067 2e63 7265 6174 6556 6172  ip = g.createVar
+0000c330: 6961 626c 6528 2273 6869 7022 2c20 2253  iable("ship", "S
+0000c340: 3122 2c20 2822 7368 6970 222c 2022 7368  1", ("ship", "sh
+0000c350: 6970 5f73 7472 6c65 6e22 2929 0a20 2020  ip_strlen")).   
+0000c360: 2073 616d 706c 6520 3d20 672e 6372 6561   sample = g.crea
+0000c370: 7465 5661 7269 6162 6c65 2822 7361 6d70  teVariable("samp
+0000c380: 6c65 222c 2022 6938 222c 2028 2274 696d  le", "i8", ("tim
+0000c390: 6522 2c20 2273 616d 706c 6522 2929 0a0a  e", "sample"))..
+0000c3a0: 2020 2020 7469 6d65 5b3a 5d20 3d20 6e70      time[:] = np
+0000c3b0: 2e61 7261 6e67 6528 3130 202b 2069 6478  .arange(10 + idx
+0000c3c0: 290a 2020 2020 6461 7461 5b3a 5d20 3d20  ).    data[:] = 
+0000c3d0: 6e70 2e6f 6e65 7328 2833 202b 2069 6478  np.ones((3 + idx
+0000c3e0: 2c20 3220 2b20 6964 782c 2031 3020 2b20  , 2 + idx, 10 + 
+0000c3f0: 6964 782c 2035 202b 2069 6478 2929 202a  idx, 5 + idx)) *
+0000c400: 2031 322e 300a 2020 2020 636f 6c6c 6964   12.0.    collid
+0000c410: 655b 2e2e 2e5d 203d 206e 702e 6172 616e  e[...] = np.aran
+0000c420: 6765 2835 202b 2069 6478 290a 2020 2020  ge(5 + idx).    
+0000c430: 6e6f 6e5f 636f 6c6c 6964 655b 2e2e 2e5d  non_collide[...]
+0000c440: 203d 206e 702e 6172 616e 6765 2835 202b   = np.arange(5 +
+0000c450: 2069 6478 2920 2b20 3130 0a20 2020 2073   idx) + 10.    s
+0000c460: 616d 706c 655b 3020 3a20 3220 2b20 6964  ample[0 : 2 + id
+0000c470: 782c 203a 2032 202b 2069 6478 5d20 3d20  x, : 2 + idx] = 
+0000c480: 6e70 2e6f 6e65 7328 2832 202b 2069 6478  np.ones((2 + idx
+0000c490: 2c20 3220 2b20 6964 7829 290a 2020 2020  , 2 + idx)).    
+0000c4a0: 7368 6970 5b30 5d20 3d20 6c69 7374 2822  ship[0] = list("
+0000c4b0: 536b 6966 6620 2020 2020 2229 0a0a 0a64  Skiff     ")...d
+0000c4c0: 6566 2063 7265 6174 655f 6835 6e65 7463  ef create_h5netc
+0000c4d0: 6466 5f64 696d 656e 7369 6f6e 7328 6473  df_dimensions(ds
+0000c4e0: 2c20 6964 7829 3a0a 2020 2020 2320 6469  , idx):.    # di
+0000c4f0: 6d65 6e73 696f 6e20 616e 6420 7661 7269  mension and vari
+0000c500: 6162 6c65 2073 6574 7570 2069 7320 6164  able setup is ad
+0000c510: 6170 7465 6420 6672 6f6d 2074 6865 2062  apted from the b
+0000c520: 6c6f 6770 6f73 7420 6174 0a20 2020 2023  logpost at.    #
+0000c530: 2068 7474 7073 3a2f 2f77 7777 2e75 6e69   https://www.uni
+0000c540: 6461 7461 2e75 6361 722e 6564 752f 626c  data.ucar.edu/bl
+0000c550: 6f67 732f 6465 7665 6c6f 7065 722f 656e  ogs/developer/en
+0000c560: 2f65 6e74 7279 2f6e 6574 6364 6634 5f73  /entry/netcdf4_s
+0000c570: 6861 7265 645f 6469 6d65 6e73 696f 6e73  hared_dimensions
+0000c580: 0a20 2020 2067 203d 2064 732e 6372 6561  .    g = ds.crea
+0000c590: 7465 5f67 726f 7570 2822 6469 6d74 6573  te_group("dimtes
+0000c5a0: 7422 202b 2073 7472 2869 6478 2929 0a20  t" + str(idx)). 
+0000c5b0: 2020 2067 2e64 696d 656e 7369 6f6e 735b     g.dimensions[
+0000c5c0: 2274 696d 6522 5d20 3d20 3020 2023 2074  "time"] = 0  # t
+0000c5d0: 696d 650a 2020 2020 672e 6469 6d65 6e73  ime.    g.dimens
+0000c5e0: 696f 6e73 5b22 6e76 6563 225d 203d 2035  ions["nvec"] = 5
+0000c5f0: 202b 2069 6478 2020 2320 6e76 6563 0a20   + idx  # nvec. 
+0000c600: 2020 2067 2e64 696d 656e 7369 6f6e 735b     g.dimensions[
+0000c610: 2273 616d 706c 6522 5d20 3d20 3220 2b20  "sample"] = 2 + 
+0000c620: 6964 7820 2023 2073 616d 706c 650a 2020  idx  # sample.  
+0000c630: 2020 672e 6469 6d65 6e73 696f 6e73 5b22    g.dimensions["
+0000c640: 7368 6970 225d 203d 2033 202b 2069 6478  ship"] = 3 + idx
+0000c650: 2020 2320 7368 6970 0a20 2020 2067 2e64    # ship.    g.d
+0000c660: 696d 656e 7369 6f6e 735b 2273 6869 705f  imensions["ship_
+0000c670: 7374 726c 656e 225d 203d 2031 3020 2023  strlen"] = 10  #
+0000c680: 2073 6869 705f 7374 726c 656e 0a20 2020   ship_strlen.   
+0000c690: 2067 2e64 696d 656e 7369 6f6e 735b 2263   g.dimensions["c
+0000c6a0: 6f6c 6c69 6465 225d 203d 2037 202b 2069  ollide"] = 7 + i
+0000c6b0: 6478 2020 2320 636f 6c6c 6964 650a 0a20  dx  # collide.. 
+0000c6c0: 2020 2067 2e63 7265 6174 655f 7661 7269     g.create_vari
+0000c6d0: 6162 6c65 2822 7469 6d65 222c 2064 696d  able("time", dim
+0000c6e0: 656e 7369 6f6e 733d 2822 7469 6d65 222c  ensions=("time",
+0000c6f0: 292c 2064 7479 7065 3d6e 702e 666c 6f61  ), dtype=np.floa
+0000c700: 7436 3429 0a20 2020 2067 2e63 7265 6174  t64).    g.creat
+0000c710: 655f 7661 7269 6162 6c65 280a 2020 2020  e_variable(.    
+0000c720: 2020 2020 2264 6174 6122 2c20 6469 6d65      "data", dime
+0000c730: 6e73 696f 6e73 3d28 2273 6869 7022 2c20  nsions=("ship", 
+0000c740: 2273 616d 706c 6522 2c20 2274 696d 6522  "sample", "time"
+0000c750: 2c20 226e 7665 6322 292c 2064 7479 7065  , "nvec"), dtype
+0000c760: 3d6e 702e 696e 7436 340a 2020 2020 290a  =np.int64.    ).
+0000c770: 2020 2020 672e 6372 6561 7465 5f76 6172      g.create_var
+0000c780: 6961 626c 6528 2263 6f6c 6c69 6465 222c  iable("collide",
+0000c790: 2064 696d 656e 7369 6f6e 733d 2822 6e76   dimensions=("nv
+0000c7a0: 6563 222c 292c 2064 7479 7065 3d6e 702e  ec",), dtype=np.
+0000c7b0: 696e 7436 3429 0a20 2020 2067 2e63 7265  int64).    g.cre
+0000c7c0: 6174 655f 7661 7269 6162 6c65 2822 6e6f  ate_variable("no
+0000c7d0: 6e5f 636f 6c6c 6964 6522 2c20 6469 6d65  n_collide", dime
+0000c7e0: 6e73 696f 6e73 3d28 226e 7665 6322 2c29  nsions=("nvec",)
+0000c7f0: 2c20 6474 7970 653d 6e70 2e69 6e74 3634  , dtype=np.int64
+0000c800: 290a 2020 2020 672e 6372 6561 7465 5f76  ).    g.create_v
+0000c810: 6172 6961 626c 6528 2273 616d 706c 6522  ariable("sample"
+0000c820: 2c20 6469 6d65 6e73 696f 6e73 3d28 2274  , dimensions=("t
+0000c830: 696d 6522 2c20 2273 616d 706c 6522 292c  ime", "sample"),
+0000c840: 2064 7479 7065 3d6e 702e 696e 7436 3429   dtype=np.int64)
+0000c850: 0a20 2020 2067 2e63 7265 6174 655f 7661  .    g.create_va
+0000c860: 7269 6162 6c65 2822 7368 6970 222c 2064  riable("ship", d
+0000c870: 696d 656e 7369 6f6e 733d 2822 7368 6970  imensions=("ship
+0000c880: 222c 2022 7368 6970 5f73 7472 6c65 6e22  ", "ship_strlen"
+0000c890: 292c 2064 7479 7065 3d22 5331 2229 0a0a  ), dtype="S1")..
+0000c8a0: 2020 2020 672e 7265 7369 7a65 5f64 696d      g.resize_dim
+0000c8b0: 656e 7369 6f6e 2822 7469 6d65 222c 2031  ension("time", 1
+0000c8c0: 3020 2b20 6964 7829 0a20 2020 2067 2e76  0 + idx).    g.v
+0000c8d0: 6172 6961 626c 6573 5b22 7469 6d65 225d  ariables["time"]
+0000c8e0: 5b3a 5d20 3d20 6e70 2e61 7261 6e67 6528  [:] = np.arange(
+0000c8f0: 3130 202b 2069 6478 290a 2020 2020 672e  10 + idx).    g.
+0000c900: 7661 7269 6162 6c65 735b 2264 6174 6122  variables["data"
+0000c910: 5d5b 3a5d 203d 206e 702e 6f6e 6573 2828  ][:] = np.ones((
+0000c920: 3320 2b20 6964 782c 2032 202b 2069 6478  3 + idx, 2 + idx
+0000c930: 2c20 3130 202b 2069 6478 2c20 3520 2b20  , 10 + idx, 5 + 
+0000c940: 6964 7829 2920 2a20 3132 2e30 0a20 2020  idx)) * 12.0.   
+0000c950: 2067 2e76 6172 6961 626c 6573 5b22 636f   g.variables["co
+0000c960: 6c6c 6964 6522 5d5b 2e2e 2e5d 203d 206e  llide"][...] = n
+0000c970: 702e 6172 616e 6765 2835 202b 2069 6478  p.arange(5 + idx
+0000c980: 290a 2020 2020 672e 7661 7269 6162 6c65  ).    g.variable
+0000c990: 735b 226e 6f6e 5f63 6f6c 6c69 6465 225d  s["non_collide"]
+0000c9a0: 5b2e 2e2e 5d20 3d20 6e70 2e61 7261 6e67  [...] = np.arang
+0000c9b0: 6528 3520 2b20 6964 7829 202b 2031 300a  e(5 + idx) + 10.
+0000c9c0: 2020 2020 672e 7661 7269 6162 6c65 735b      g.variables[
+0000c9d0: 2273 616d 706c 6522 5d5b 3020 3a20 3220  "sample"][0 : 2 
+0000c9e0: 2b20 6964 782c 203a 2032 202b 2069 6478  + idx, : 2 + idx
+0000c9f0: 5d20 3d20 6e70 2e6f 6e65 7328 2832 202b  ] = np.ones((2 +
+0000ca00: 2069 6478 2c20 3220 2b20 6964 7829 290a   idx, 2 + idx)).
+0000ca10: 2020 2020 672e 7661 7269 6162 6c65 735b      g.variables[
+0000ca20: 2273 6869 7022 5d5b 305d 203d 206c 6973  "ship"][0] = lis
+0000ca30: 7428 2253 6b69 6666 2020 2020 2022 290a  t("Skiff     ").
+0000ca40: 0a0a 6465 6620 6368 6563 6b5f 6e65 7463  ..def check_netc
+0000ca50: 6466 5f64 696d 656e 7369 6f6e 7328 746d  df_dimensions(tm
+0000ca60: 705f 6e65 7463 6466 2c20 7772 6974 655f  p_netcdf, write_
+0000ca70: 6d6f 6475 6c65 2c20 7265 6164 5f6d 6f64  module, read_mod
+0000ca80: 756c 6529 3a0a 2020 2020 6966 2072 6561  ule):.    if rea
+0000ca90: 645f 6d6f 6475 6c65 2069 6e20 5b6c 6567  d_module in [leg
+0000caa0: 6163 7961 7069 2c20 6e65 7443 4446 345d  acyapi, netCDF4]
+0000cab0: 3a0a 2020 2020 2020 2020 6f70 656e 6572  :.        opener
+0000cac0: 203d 2072 6561 645f 6d6f 6475 6c65 2e44   = read_module.D
+0000cad0: 6174 6173 6574 0a20 2020 2065 6c73 653a  ataset.    else:
+0000cae0: 0a20 2020 2020 2020 206f 7065 6e65 7220  .        opener 
+0000caf0: 3d20 6835 6e65 7463 6466 2e46 696c 650a  = h5netcdf.File.
+0000cb00: 2020 2020 7769 7468 206f 7065 6e65 7228      with opener(
+0000cb10: 746d 705f 6e65 7463 6466 2c20 2272 2229  tmp_netcdf, "r")
+0000cb20: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
+0000cb30: 666f 7220 692c 2067 7270 2069 6e20 656e  for i, grp in en
+0000cb40: 756d 6572 6174 6528 5b22 6469 6d74 6573  umerate(["dimtes
+0000cb50: 7430 222c 2022 6469 6d74 6573 7431 225d  t0", "dimtest1"]
+0000cb60: 293a 0a20 2020 2020 2020 2020 2020 2067  ):.            g
+0000cb70: 203d 2064 732e 6772 6f75 7073 5b67 7270   = ds.groups[grp
+0000cb80: 5d0a 2020 2020 2020 2020 2020 2020 6173  ].            as
+0000cb90: 7365 7274 2073 6574 2867 2e64 696d 656e  sert set(g.dimen
+0000cba0: 7369 6f6e 7329 203d 3d20 7b0a 2020 2020  sions) == {.    
+0000cbb0: 2020 2020 2020 2020 2020 2020 2263 6f6c              "col
+0000cbc0: 6c69 6465 222c 0a20 2020 2020 2020 2020  lide",.         
+0000cbd0: 2020 2020 2020 2022 7368 6970 5f73 7472         "ship_str
+0000cbe0: 6c65 6e22 2c0a 2020 2020 2020 2020 2020  len",.          
+0000cbf0: 2020 2020 2020 2274 696d 6522 2c0a 2020        "time",.  
+0000cc00: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0000cc10: 7665 6322 2c0a 2020 2020 2020 2020 2020  vec",.          
+0000cc20: 2020 2020 2020 2273 6869 7022 2c0a 2020        "ship",.  
+0000cc30: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+0000cc40: 616d 706c 6522 2c0a 2020 2020 2020 2020  ample",.        
+0000cc50: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+0000cc60: 2020 6966 2072 6561 645f 6d6f 6475 6c65    if read_module
+0000cc70: 2069 6e20 5b6c 6567 6163 7961 7069 2c20   in [legacyapi, 
+0000cc80: 6835 6e65 7463 6466 5d3a 0a20 2020 2020  h5netcdf]:.     
+0000cc90: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000cca0: 7420 672e 6469 6d65 6e73 696f 6e73 5b22  t g.dimensions["
+0000ccb0: 7469 6d65 225d 2e69 7375 6e6c 696d 6974  time"].isunlimit
+0000ccc0: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
+0000ccd0: 2020 2020 2061 7373 6572 7420 672e 6469       assert g.di
+0000cce0: 6d65 6e73 696f 6e73 5b22 7469 6d65 225d  mensions["time"]
+0000ccf0: 2e73 697a 6520 3d3d 2031 3020 2b20 690a  .size == 10 + i.
+0000cd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd10: 6173 7365 7274 206e 6f74 2067 2e64 696d  assert not g.dim
+0000cd20: 656e 7369 6f6e 735b 226e 7665 6322 5d2e  ensions["nvec"].
+0000cd30: 6973 756e 6c69 6d69 7465 6428 290a 2020  isunlimited().  
+0000cd40: 2020 2020 2020 2020 2020 2020 2020 6173                as
+0000cd50: 7365 7274 2067 2e64 696d 656e 7369 6f6e  sert g.dimension
+0000cd60: 735b 226e 7665 6322 5d2e 7369 7a65 203d  s["nvec"].size =
+0000cd70: 3d20 3520 2b20 690a 2020 2020 2020 2020  = 5 + i.        
+0000cd80: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+0000cd90: 6f74 2067 2e64 696d 656e 7369 6f6e 735b  ot g.dimensions[
+0000cda0: 2273 616d 706c 6522 5d2e 6973 756e 6c69  "sample"].isunli
+0000cdb0: 6d69 7465 6428 290a 2020 2020 2020 2020  mited().        
+0000cdc0: 2020 2020 2020 2020 6173 7365 7274 2067          assert g
+0000cdd0: 2e64 696d 656e 7369 6f6e 735b 2273 616d  .dimensions["sam
+0000cde0: 706c 6522 5d2e 7369 7a65 203d 3d20 3220  ple"].size == 2 
+0000cdf0: 2b20 690a 2020 2020 2020 2020 2020 2020  + i.            
+0000ce00: 2020 2020 6173 7365 7274 206e 6f74 2067      assert not g
+0000ce10: 2e64 696d 656e 7369 6f6e 735b 2263 6f6c  .dimensions["col
+0000ce20: 6c69 6465 225d 2e69 7375 6e6c 696d 6974  lide"].isunlimit
+0000ce30: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
+0000ce40: 2020 2020 2061 7373 6572 7420 672e 6469       assert g.di
+0000ce50: 6d65 6e73 696f 6e73 5b22 636f 6c6c 6964  mensions["collid
+0000ce60: 6522 5d2e 7369 7a65 203d 3d20 3720 2b20  e"].size == 7 + 
+0000ce70: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
+0000ce80: 2020 6173 7365 7274 206e 6f74 2067 2e64    assert not g.d
+0000ce90: 696d 656e 7369 6f6e 735b 2273 6869 7022  imensions["ship"
+0000cea0: 5d2e 6973 756e 6c69 6d69 7465 6428 290a  ].isunlimited().
+0000ceb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cec0: 6173 7365 7274 2067 2e64 696d 656e 7369  assert g.dimensi
+0000ced0: 6f6e 735b 2273 6869 7022 5d2e 7369 7a65  ons["ship"].size
+0000cee0: 203d 3d20 3320 2b20 690a 2020 2020 2020   == 3 + i.      
+0000cef0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000cf00: 206e 6f74 2067 2e64 696d 656e 7369 6f6e   not g.dimension
+0000cf10: 735b 2273 6869 705f 7374 726c 656e 225d  s["ship_strlen"]
+0000cf20: 2e69 7375 6e6c 696d 6974 6564 2829 0a20  .isunlimited(). 
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000cf40: 7373 6572 7420 672e 6469 6d65 6e73 696f  ssert g.dimensio
+0000cf50: 6e73 5b22 7368 6970 5f73 7472 6c65 6e22  ns["ship_strlen"
+0000cf60: 5d2e 7369 7a65 203d 3d20 3130 0a20 2020  ].size == 10.   
+0000cf70: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000cf90: 7373 6572 7420 672e 6469 6d65 6e73 696f  ssert g.dimensio
+0000cfa0: 6e73 5b22 7469 6d65 225d 2e69 7375 6e6c  ns["time"].isunl
+0000cfb0: 696d 6974 6564 2829 0a20 2020 2020 2020  imited().       
+0000cfc0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000cfd0: 672e 6469 6d65 6e73 696f 6e73 5b22 7469  g.dimensions["ti
+0000cfe0: 6d65 225d 2e73 697a 6520 3d3d 2031 3020  me"].size == 10 
+0000cff0: 2b20 690a 2020 2020 2020 2020 2020 2020  + i.            
+0000d000: 2020 2020 6173 7365 7274 206e 6f74 2067      assert not g
+0000d010: 2e64 696d 656e 7369 6f6e 735b 226e 7665  .dimensions["nve
+0000d020: 6322 5d2e 6973 756e 6c69 6d69 7465 6428  c"].isunlimited(
+0000d030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d040: 2020 6173 7365 7274 2067 2e64 696d 656e    assert g.dimen
+0000d050: 7369 6f6e 735b 226e 7665 6322 5d2e 7369  sions["nvec"].si
+0000d060: 7a65 203d 3d20 3520 2b20 690a 2020 2020  ze == 5 + i.    
+0000d070: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000d080: 7274 206e 6f74 2067 2e64 696d 656e 7369  rt not g.dimensi
+0000d090: 6f6e 735b 2273 616d 706c 6522 5d2e 6973  ons["sample"].is
+0000d0a0: 756e 6c69 6d69 7465 6428 290a 2020 2020  unlimited().    
+0000d0b0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+0000d0c0: 7274 2067 2e64 696d 656e 7369 6f6e 735b  rt g.dimensions[
+0000d0d0: 2273 616d 706c 6522 5d2e 7369 7a65 203d  "sample"].size =
+0000d0e0: 3d20 3220 2b20 690a 2020 2020 2020 2020  = 2 + i.        
+0000d0f0: 2020 2020 2020 2020 6173 7365 7274 206e          assert n
+0000d100: 6f74 2067 2e64 696d 656e 7369 6f6e 735b  ot g.dimensions[
+0000d110: 2273 6869 7022 5d2e 6973 756e 6c69 6d69  "ship"].isunlimi
+0000d120: 7465 6428 290a 2020 2020 2020 2020 2020  ted().          
+0000d130: 2020 2020 2020 6173 7365 7274 2067 2e64        assert g.d
+0000d140: 696d 656e 7369 6f6e 735b 2273 6869 7022  imensions["ship"
+0000d150: 5d2e 7369 7a65 203d 3d20 3320 2b20 690a  ].size == 3 + i.
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 6173 7365 7274 206e 6f74 2067 2e64 696d  assert not g.dim
+0000d180: 656e 7369 6f6e 735b 2273 6869 705f 7374  ensions["ship_st
+0000d190: 726c 656e 225d 2e69 7375 6e6c 696d 6974  rlen"].isunlimit
+0000d1a0: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
+0000d1b0: 2020 2020 2061 7373 6572 7420 672e 6469       assert g.di
+0000d1c0: 6d65 6e73 696f 6e73 5b22 7368 6970 5f73  mensions["ship_s
+0000d1d0: 7472 6c65 6e22 5d2e 7369 7a65 203d 3d20  trlen"].size == 
+0000d1e0: 3130 0a20 2020 2020 2020 2020 2020 2020  10.             
+0000d1f0: 2020 2061 7373 6572 7420 6e6f 7420 672e     assert not g.
+0000d200: 6469 6d65 6e73 696f 6e73 5b22 636f 6c6c  dimensions["coll
+0000d210: 6964 6522 5d2e 6973 756e 6c69 6d69 7465  ide"].isunlimite
+0000d220: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+0000d230: 2020 2020 6173 7365 7274 2067 2e64 696d      assert g.dim
+0000d240: 656e 7369 6f6e 735b 2263 6f6c 6c69 6465  ensions["collide
+0000d250: 225d 2e73 697a 6520 3d3d 2037 202b 2069  "].size == 7 + i
+0000d260: 0a0a 2020 2020 2020 2020 2020 2020 6173  ..            as
+0000d270: 7365 7274 2073 6574 2867 2e76 6172 6961  sert set(g.varia
+0000d280: 626c 6573 2920 3d3d 207b 0a20 2020 2020  bles) == {.     
+0000d290: 2020 2020 2020 2020 2020 2022 6461 7461             "data
+0000d2a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000d2b0: 2020 2022 636f 6c6c 6964 6522 2c0a 2020     "collide",.  
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0000d2d0: 6f6e 5f63 6f6c 6c69 6465 222c 0a20 2020  on_collide",.   
+0000d2e0: 2020 2020 2020 2020 2020 2020 2022 7469               "ti
+0000d2f0: 6d65 222c 0a20 2020 2020 2020 2020 2020  me",.           
+0000d300: 2020 2020 2022 7361 6d70 6c65 222c 0a20       "sample",. 
+0000d310: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000d320: 7368 6970 222c 0a20 2020 2020 2020 2020  ship",.         
+0000d330: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+0000d340: 2061 7373 6572 7420 672e 7661 7269 6162   assert g.variab
+0000d350: 6c65 735b 2274 696d 6522 5d2e 7368 6170  les["time"].shap
+0000d360: 6520 3d3d 2028 3130 202b 2069 2c29 0a20  e == (10 + i,). 
+0000d370: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000d380: 7420 672e 7661 7269 6162 6c65 735b 2264  t g.variables["d
+0000d390: 6174 6122 5d2e 7368 6170 6520 3d3d 2028  ata"].shape == (
+0000d3a0: 3320 2b20 692c 2032 202b 2069 2c20 3130  3 + i, 2 + i, 10
+0000d3b0: 202b 2069 2c20 3520 2b20 6929 0a20 2020   + i, 5 + i).   
+0000d3c0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
+0000d3d0: 672e 7661 7269 6162 6c65 735b 2263 6f6c  g.variables["col
+0000d3e0: 6c69 6465 225d 2e73 6861 7065 203d 3d20  lide"].shape == 
+0000d3f0: 2835 202b 2069 2c29 0a20 2020 2020 2020  (5 + i,).       
+0000d400: 2020 2020 2061 7373 6572 7420 672e 7661       assert g.va
+0000d410: 7269 6162 6c65 735b 226e 6f6e 5f63 6f6c  riables["non_col
+0000d420: 6c69 6465 225d 2e73 6861 7065 203d 3d20  lide"].shape == 
+0000d430: 2835 202b 2069 2c29 0a20 2020 2020 2020  (5 + i,).       
+0000d440: 2020 2020 2061 7373 6572 7420 672e 7661       assert g.va
+0000d450: 7269 6162 6c65 735b 2273 616d 706c 6522  riables["sample"
+0000d460: 5d2e 7368 6170 6520 3d3d 2028 3130 202b  ].shape == (10 +
+0000d470: 2069 2c20 3220 2b20 6929 0a20 2020 2020   i, 2 + i).     
+0000d480: 2020 2020 2020 2061 7373 6572 7420 672e         assert g.
+0000d490: 7661 7269 6162 6c65 735b 2273 6869 7022  variables["ship"
+0000d4a0: 5d2e 7368 6170 6520 3d3d 2028 3320 2b20  ].shape == (3 + 
+0000d4b0: 692c 2031 3029 0a0a 0a64 6566 2077 7269  i, 10)...def wri
+0000d4c0: 7465 5f64 696d 656e 7369 6f6e 7328 746d  te_dimensions(tm
+0000d4d0: 705f 6e65 7463 6466 2c20 7772 6974 655f  p_netcdf, write_
+0000d4e0: 6d6f 6475 6c65 293a 0a20 2020 2069 6620  module):.    if 
+0000d4f0: 7772 6974 655f 6d6f 6475 6c65 2069 6e20  write_module in 
+0000d500: 5b6c 6567 6163 7961 7069 2c20 6e65 7443  [legacyapi, netC
+0000d510: 4446 345d 3a0a 2020 2020 2020 2020 7769  DF4]:.        wi
+0000d520: 7468 2077 7269 7465 5f6d 6f64 756c 652e  th write_module.
+0000d530: 4461 7461 7365 7428 746d 705f 6e65 7463  Dataset(tmp_netc
+0000d540: 6466 2c20 2277 2229 2061 7320 6473 3a0a  df, "w") as ds:.
+0000d550: 2020 2020 2020 2020 2020 2020 6372 6561              crea
+0000d560: 7465 5f6e 6574 6364 665f 6469 6d65 6e73  te_netcdf_dimens
+0000d570: 696f 6e73 2864 732c 2030 290a 2020 2020  ions(ds, 0).    
+0000d580: 2020 2020 2020 2020 6372 6561 7465 5f6e          create_n
+0000d590: 6574 6364 665f 6469 6d65 6e73 696f 6e73  etcdf_dimensions
+0000d5a0: 2864 732c 2031 290a 2020 2020 656c 7365  (ds, 1).    else
+0000d5b0: 3a0a 2020 2020 2020 2020 7769 7468 2077  :.        with w
+0000d5c0: 7269 7465 5f6d 6f64 756c 652e 4669 6c65  rite_module.File
+0000d5d0: 2874 6d70 5f6e 6574 6364 662c 2022 7722  (tmp_netcdf, "w"
+0000d5e0: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
+0000d5f0: 2020 2020 2063 7265 6174 655f 6835 6e65       create_h5ne
+0000d600: 7463 6466 5f64 696d 656e 7369 6f6e 7328  tcdf_dimensions(
+0000d610: 6473 2c20 3029 0a20 2020 2020 2020 2020  ds, 0).         
+0000d620: 2020 2063 7265 6174 655f 6835 6e65 7463     create_h5netc
+0000d630: 6466 5f64 696d 656e 7369 6f6e 7328 6473  df_dimensions(ds
+0000d640: 2c20 3129 0a0a 0a40 7079 7465 7374 2e66  , 1)...@pytest.f
+0000d650: 6978 7475 7265 280a 2020 2020 7061 7261  ixture(.    para
+0000d660: 6d73 3d5b 0a20 2020 2020 2020 205b 6e65  ms=[.        [ne
+0000d670: 7443 4446 342c 206e 6574 4344 4634 5d2c  tCDF4, netCDF4],
+0000d680: 0a20 2020 2020 2020 205b 6c65 6761 6379  .        [legacy
+0000d690: 6170 692c 206c 6567 6163 7961 7069 5d2c  api, legacyapi],
+0000d6a0: 0a20 2020 2020 2020 205b 6835 6e65 7463  .        [h5netc
+0000d6b0: 6466 2c20 6835 6e65 7463 6466 5d2c 0a20  df, h5netcdf],. 
+0000d6c0: 2020 2020 2020 205b 6c65 6761 6379 6170         [legacyap
+0000d6d0: 692c 206e 6574 4344 4634 5d2c 0a20 2020  i, netCDF4],.   
+0000d6e0: 2020 2020 205b 6e65 7443 4446 342c 206c       [netCDF4, l
+0000d6f0: 6567 6163 7961 7069 5d2c 0a20 2020 2020  egacyapi],.     
+0000d700: 2020 205b 6835 6e65 7463 6466 2c20 6e65     [h5netcdf, ne
+0000d710: 7443 4446 345d 2c0a 2020 2020 2020 2020  tCDF4],.        
+0000d720: 5b6e 6574 4344 4634 2c20 6835 6e65 7463  [netCDF4, h5netc
+0000d730: 6466 5d2c 0a20 2020 2020 2020 205b 6c65  df],.        [le
+0000d740: 6761 6379 6170 692c 2068 356e 6574 6364  gacyapi, h5netcd
+0000d750: 665d 2c0a 2020 2020 2020 2020 5b68 356e  f],.        [h5n
+0000d760: 6574 6364 662c 206c 6567 6163 7961 7069  etcdf, legacyapi
+0000d770: 5d2c 0a20 2020 205d 0a29 0a64 6566 2072  ],.    ].).def r
+0000d780: 6561 645f 7772 6974 655f 6d61 7472 6978  ead_write_matrix
+0000d790: 2872 6571 7565 7374 293a 0a20 2020 2070  (request):.    p
+0000d7a0: 7269 6e74 2822 7772 6974 6520 6d6f 6475  rint("write modu
+0000d7b0: 6c65 3a22 2c20 7265 7175 6573 742e 7061  le:", request.pa
+0000d7c0: 7261 6d5b 305d 2e5f 5f6e 616d 655f 5f29  ram[0].__name__)
+0000d7d0: 0a20 2020 2070 7269 6e74 2822 7265 6164  .    print("read
+0000d7e0: 5f6d 6f64 756c 653a 222c 2072 6571 7565  _module:", reque
+0000d7f0: 7374 2e70 6172 616d 5b31 5d2e 5f5f 6e61  st.param[1].__na
+0000d800: 6d65 5f5f 290a 2020 2020 7265 7475 726e  me__).    return
+0000d810: 2072 6571 7565 7374 2e70 6172 616d 0a0a   request.param..
+0000d820: 0a64 6566 2074 6573 745f 6469 6d65 6e73  .def test_dimens
+0000d830: 696f 6e73 2874 6d70 5f6c 6f63 616c 5f6e  ions(tmp_local_n
+0000d840: 6574 6364 662c 2072 6561 645f 7772 6974  etcdf, read_writ
+0000d850: 655f 6d61 7472 6978 293a 0a20 2020 2077  e_matrix):.    w
+0000d860: 7269 7465 5f64 696d 656e 7369 6f6e 7328  rite_dimensions(
+0000d870: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000d880: 2c20 7265 6164 5f77 7269 7465 5f6d 6174  , read_write_mat
+0000d890: 7269 785b 305d 290a 2020 2020 6368 6563  rix[0]).    chec
+0000d8a0: 6b5f 6e65 7463 6466 5f64 696d 656e 7369  k_netcdf_dimensi
+0000d8b0: 6f6e 7328 0a20 2020 2020 2020 2074 6d70  ons(.        tmp
+0000d8c0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2072  _local_netcdf, r
+0000d8d0: 6561 645f 7772 6974 655f 6d61 7472 6978  ead_write_matrix
+0000d8e0: 5b30 5d2c 2072 6561 645f 7772 6974 655f  [0], read_write_
+0000d8f0: 6d61 7472 6978 5b31 5d0a 2020 2020 290a  matrix[1].    ).
+0000d900: 0a0a 6465 6620 7465 7374 5f6e 6f5f 6369  ..def test_no_ci
+0000d910: 7263 756c 6172 5f72 6566 6572 656e 6365  rcular_reference
+0000d920: 7328 746d 705f 6c6f 6361 6c5f 6e65 7463  s(tmp_local_netc
+0000d930: 6466 293a 0a20 2020 2023 2068 7474 7073  df):.    # https
+0000d940: 3a2f 2f67 6974 6875 622e 636f 6d2f 6835  ://github.com/h5
+0000d950: 7079 2f68 3570 792f 6973 7375 6573 2f32  py/h5py/issues/2
+0000d960: 3031 390a 2020 2020 7769 7468 2068 356e  019.    with h5n
+0000d970: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+0000d980: 6f63 616c 5f6e 6574 6364 662c 2022 7722  ocal_netcdf, "w"
+0000d990: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
+0000d9a0: 2064 732e 6469 6d65 6e73 696f 6e73 5b22   ds.dimensions["
+0000d9b0: 7822 5d20 3d20 320a 2020 2020 2020 2020  x"] = 2.        
+0000d9c0: 6473 2e64 696d 656e 7369 6f6e 735b 2279  ds.dimensions["y
+0000d9d0: 225d 203d 2032 0a0a 2020 2020 6763 2e63  "] = 2..    gc.c
+0000d9e0: 6f6c 6c65 6374 2829 0a20 2020 2077 6974  ollect().    wit
+0000d9f0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+0000da00: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000da10: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+0000da20: 2020 2020 2020 7265 6673 203d 2067 632e        refs = gc.
+0000da30: 6765 745f 7265 6665 7272 6572 7328 6473  get_referrers(ds
+0000da40: 290a 2020 2020 2020 2020 666f 7220 7265  ).        for re
+0000da50: 6620 696e 2072 6566 733a 0a20 2020 2020  f in refs:.     
+0000da60: 2020 2020 2020 2070 7269 6e74 2872 6566         print(ref
+0000da70: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+0000da80: 206c 656e 2872 6566 7329 203d 3d20 310a   len(refs) == 1.
+0000da90: 0a0a 6465 6620 7465 7374 5f65 7870 616e  ..def test_expan
+0000daa0: 6465 645f 7661 7269 6162 6c65 735f 6e65  ded_variables_ne
+0000dab0: 7463 6466 3428 746d 705f 6c6f 6361 6c5f  tcdf4(tmp_local_
+0000dac0: 6e65 7463 6466 2c20 6e65 7463 6466 5f77  netcdf, netcdf_w
+0000dad0: 7269 7465 5f6d 6f64 756c 6529 3a0a 2020  rite_module):.  
+0000dae0: 2020 2320 7061 7274 6961 6c6c 7920 7265    # partially re
+0000daf0: 696d 706c 656d 656e 7465 6420 6475 6520  implemented due 
+0000db00: 746f 2070 6572 666f 726d 616e 6365 2072  to performance r
+0000db10: 6561 736f 6e20 696e 2065 6467 6520 6361  eason in edge ca
+0000db20: 7365 730a 2020 2020 2320 6874 7470 733a  ses.    # https:
+0000db30: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
+0000db40: 6574 6364 662f 6835 6e65 7463 6466 2f69  etcdf/h5netcdf/i
+0000db50: 7373 7565 732f 3138 320a 0a20 2020 2077  ssues/182..    w
+0000db60: 6974 6820 6e65 7463 6466 5f77 7269 7465  ith netcdf_write
+0000db70: 5f6d 6f64 756c 652e 4461 7461 7365 7428  _module.Dataset(
+0000db80: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000db90: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
+0000dba0: 2020 2020 2020 6620 3d20 6473 2e63 7265        f = ds.cre
+0000dbb0: 6174 6547 726f 7570 2822 7465 7374 2229  ateGroup("test")
+0000dbc0: 0a20 2020 2020 2020 2066 2e63 7265 6174  .        f.creat
+0000dbd0: 6544 696d 656e 7369 6f6e 2822 7822 2c20  eDimension("x", 
+0000dbe0: 4e6f 6e65 290a 2020 2020 2020 2020 662e  None).        f.
+0000dbf0: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+0000dc00: 2279 222c 2033 290a 0a20 2020 2020 2020  "y", 3)..       
+0000dc10: 2064 756d 6d79 3120 3d20 662e 6372 6561   dummy1 = f.crea
+0000dc20: 7465 5661 7269 6162 6c65 2822 6475 6d6d  teVariable("dumm
+0000dc30: 7931 222c 2066 6c6f 6174 2c20 2822 7822  y1", float, ("x"
+0000dc40: 2c20 2279 2229 290a 2020 2020 2020 2020  , "y")).        
+0000dc50: 6475 6d6d 7932 203d 2066 2e63 7265 6174  dummy2 = f.creat
+0000dc60: 6556 6172 6961 626c 6528 2264 756d 6d79  eVariable("dummy
+0000dc70: 3222 2c20 666c 6f61 742c 2028 2278 222c  2", float, ("x",
+0000dc80: 2022 7922 2929 0a20 2020 2020 2020 2064   "y")).        d
+0000dc90: 756d 6d79 3320 3d20 662e 6372 6561 7465  ummy3 = f.create
+0000dca0: 5661 7269 6162 6c65 2822 6475 6d6d 7933  Variable("dummy3
+0000dcb0: 222c 2066 6c6f 6174 2c20 2822 7822 2c20  ", float, ("x", 
+0000dcc0: 2279 2229 290a 2020 2020 2020 2020 6475  "y")).        du
+0000dcd0: 6d6d 7934 203d 2066 2e63 7265 6174 6556  mmy4 = f.createV
+0000dce0: 6172 6961 626c 6528 2264 756d 6d79 3422  ariable("dummy4"
+0000dcf0: 2c20 666c 6f61 742c 2028 2278 222c 2022  , float, ("x", "
+0000dd00: 7922 2929 0a0a 2020 2020 2020 2020 6475  y"))..        du
+0000dd10: 6d6d 7931 5b3a 5d20 3d20 5b5b 312c 2032  mmy1[:] = [[1, 2
+0000dd20: 2c20 335d 2c20 5b34 2c20 352c 2036 5d2c  , 3], [4, 5, 6],
+0000dd30: 205b 372c 2038 2c20 395d 5d0a 2020 2020   [7, 8, 9]].    
+0000dd40: 2020 2020 6475 6d6d 7932 5b31 2c20 3a5d      dummy2[1, :]
+0000dd50: 203d 205b 342c 2035 2c20 365d 0a20 2020   = [4, 5, 6].   
+0000dd60: 2020 2020 2064 756d 6d79 335b 303a 322c       dummy3[0:2,
+0000dd70: 203a 5d20 3d20 5b5b 312c 2032 2c20 335d   :] = [[1, 2, 3]
+0000dd80: 2c20 5b34 2c20 352c 2036 5d5d 0a0a 2020  , [4, 5, 6]]..  
+0000dd90: 2020 2020 2020 2320 646f 6e27 7420 6d61        # don't ma
+0000dda0: 736b 2c20 7369 6e63 6520 6835 6e65 7463  sk, since h5netc
+0000ddb0: 6466 2064 6f65 736e 2774 2064 6f20 6d61  df doesn't do ma
+0000ddc0: 736b 696e 670a 2020 2020 2020 2020 6966  sking.        if
+0000ddd0: 206e 6574 6364 665f 7772 6974 655f 6d6f   netcdf_write_mo
+0000dde0: 6475 6c65 203d 3d20 6e65 7443 4446 343a  dule == netCDF4:
+0000ddf0: 0a20 2020 2020 2020 2020 2020 2064 732e  .            ds.
+0000de00: 7365 745f 6175 746f 5f6d 6173 6b28 4661  set_auto_mask(Fa
+0000de10: 6c73 6529 0a0a 2020 2020 2020 2020 7265  lse)..        re
+0000de20: 7331 203d 2064 756d 6d79 315b 3a5d 0a20  s1 = dummy1[:]. 
+0000de30: 2020 2020 2020 2072 6573 3220 3d20 6475         res2 = du
+0000de40: 6d6d 7932 5b3a 5d0a 2020 2020 2020 2020  mmy2[:].        
+0000de50: 7265 7333 203d 2064 756d 6d79 335b 3a5d  res3 = dummy3[:]
+0000de60: 0a20 2020 2020 2020 2072 6573 3420 3d20  .        res4 = 
+0000de70: 6475 6d6d 7934 5b3a 5d0a 0a20 2020 2077  dummy4[:]..    w
+0000de80: 6974 6820 6e65 7443 4446 342e 4461 7461  ith netCDF4.Data
+0000de90: 7365 7428 746d 705f 6c6f 6361 6c5f 6e65  set(tmp_local_ne
+0000dea0: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
+0000deb0: 3a0a 2020 2020 2020 2020 2320 646f 6e27  :.        # don'
+0000dec0: 7420 6d61 736b 2c20 7369 6e63 6520 6835  t mask, since h5
+0000ded0: 6e65 7463 6466 2064 6f65 736e 2774 2064  netcdf doesn't d
+0000dee0: 6f20 6d61 736b 696e 670a 2020 2020 2020  o masking.      
+0000def0: 2020 6966 206e 6574 6364 665f 7772 6974    if netcdf_writ
+0000df00: 655f 6d6f 6475 6c65 203d 3d20 6e65 7443  e_module == netC
+0000df10: 4446 343a 0a20 2020 2020 2020 2020 2020  DF4:.           
+0000df20: 2064 732e 7365 745f 6175 746f 5f6d 6173   ds.set_auto_mas
+0000df30: 6b28 4661 6c73 6529 0a0a 2020 2020 2020  k(False)..      
+0000df40: 2020 6620 3d20 6473 5b22 7465 7374 225d    f = ds["test"]
+0000df50: 0a0a 2020 2020 2020 2020 6e70 2e74 6573  ..        np.tes
+0000df60: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
+0000df70: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
+0000df80: 5b22 6475 6d6d 7931 225d 5b3a 5d2c 2072  ["dummy1"][:], r
+0000df90: 6573 3129 0a20 2020 2020 2020 206e 702e  es1).        np.
+0000dfa0: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
+0000dfb0: 6c6c 636c 6f73 6528 662e 7661 7269 6162  llclose(f.variab
+0000dfc0: 6c65 735b 2264 756d 6d79 3122 5d5b 312c  les["dummy1"][1,
+0000dfd0: 203a 5d2c 205b 342e 302c 2035 2e30 2c20   :], [4.0, 5.0, 
+0000dfe0: 362e 305d 290a 2020 2020 2020 2020 6e70  6.0]).        np
+0000dff0: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
+0000e000: 616c 6c63 6c6f 7365 2866 2e76 6172 6961  allclose(f.varia
+0000e010: 626c 6573 5b22 6475 6d6d 7931 225d 5b31  bles["dummy1"][1
+0000e020: 3a32 2c20 3a5d 2c20 5b5b 342e 302c 2035  :2, :], [[4.0, 5
+0000e030: 2e30 2c20 362e 305d 5d29 0a20 2020 2020  .0, 6.0]]).     
+0000e040: 2020 2061 7373 6572 7420 662e 7661 7269     assert f.vari
+0000e050: 6162 6c65 735b 2264 756d 6d79 3122 5d2e  ables["dummy1"].
+0000e060: 7368 6170 6520 3d3d 2028 332c 2033 290a  shape == (3, 3).
+0000e070: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
+0000e080: 6e67 2e61 7373 6572 745f 616c 6c63 6c6f  ng.assert_allclo
+0000e090: 7365 2866 2e76 6172 6961 626c 6573 5b22  se(f.variables["
+0000e0a0: 6475 6d6d 7932 225d 5b3a 5d2c 2072 6573  dummy2"][:], res
+0000e0b0: 3229 0a20 2020 2020 2020 206e 702e 7465  2).        np.te
+0000e0c0: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
+0000e0d0: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
+0000e0e0: 735b 2264 756d 6d79 3222 5d5b 312c 203a  s["dummy2"][1, :
+0000e0f0: 5d2c 205b 342e 302c 2035 2e30 2c20 362e  ], [4.0, 5.0, 6.
+0000e100: 305d 290a 2020 2020 2020 2020 6e70 2e74  0]).        np.t
+0000e110: 6573 7469 6e67 2e61 7373 6572 745f 616c  esting.assert_al
+0000e120: 6c63 6c6f 7365 2866 2e76 6172 6961 626c  lclose(f.variabl
+0000e130: 6573 5b22 6475 6d6d 7932 225d 5b31 3a32  es["dummy2"][1:2
+0000e140: 2c20 3a5d 2c20 5b5b 342e 302c 2035 2e30  , :], [[4.0, 5.0
+0000e150: 2c20 362e 305d 5d29 0a20 2020 2020 2020  , 6.0]]).       
 0000e160: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
-0000e170: 6c65 735b 2264 756d 6d79 3422 5d2e 7368  les["dummy4"].sh
-0000e180: 6170 6520 3d3d 2028 332c 2033 290a 0a20  ape == (3, 3).. 
-0000e190: 2020 2077 6974 6820 6c65 6761 6379 6170     with legacyap
-0000e1a0: 692e 4461 7461 7365 7428 746d 705f 6c6f  i.Dataset(tmp_lo
-0000e1b0: 6361 6c5f 6e65 7463 6466 2c20 2272 2229  cal_netcdf, "r")
-0000e1c0: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-0000e1d0: 6620 3d20 6473 5b22 7465 7374 225d 0a20  f = ds["test"]. 
-0000e1e0: 2020 2020 2020 206e 702e 7465 7374 696e         np.testin
-0000e1f0: 672e 6173 7365 7274 5f61 6c6c 636c 6f73  g.assert_allclos
-0000e200: 6528 662e 7661 7269 6162 6c65 735b 2264  e(f.variables["d
-0000e210: 756d 6d79 3122 5d5b 3a5d 2c20 7265 7331  ummy1"][:], res1
+0000e170: 6c65 735b 2264 756d 6d79 3222 5d2e 7368  les["dummy2"].sh
+0000e180: 6170 6520 3d3d 2028 332c 2033 290a 2020  ape == (3, 3).  
+0000e190: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
+0000e1a0: 2e61 7373 6572 745f 616c 6c63 6c6f 7365  .assert_allclose
+0000e1b0: 2866 2e76 6172 6961 626c 6573 5b22 6475  (f.variables["du
+0000e1c0: 6d6d 7933 225d 5b3a 5d2c 2072 6573 3329  mmy3"][:], res3)
+0000e1d0: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
+0000e1e0: 696e 672e 6173 7365 7274 5f61 6c6c 636c  ing.assert_allcl
+0000e1f0: 6f73 6528 662e 7661 7269 6162 6c65 735b  ose(f.variables[
+0000e200: 2264 756d 6d79 3322 5d5b 312c 203a 5d2c  "dummy3"][1, :],
+0000e210: 205b 342e 302c 2035 2e30 2c20 362e 305d   [4.0, 5.0, 6.0]
 0000e220: 290a 2020 2020 2020 2020 6e70 2e74 6573  ).        np.tes
 0000e230: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
 0000e240: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
-0000e250: 5b22 6475 6d6d 7931 225d 5b31 2c20 3a5d  ["dummy1"][1, :]
-0000e260: 2c20 5b34 2e30 2c20 352e 302c 2036 2e30  , [4.0, 5.0, 6.0
-0000e270: 5d29 0a20 2020 2020 2020 206e 702e 7465  ]).        np.te
-0000e280: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
-0000e290: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
-0000e2a0: 735b 2264 756d 6d79 3122 5d5b 313a 322c  s["dummy1"][1:2,
-0000e2b0: 203a 5d2c 205b 5b34 2e30 2c20 352e 302c   :], [[4.0, 5.0,
-0000e2c0: 2036 2e30 5d5d 290a 2020 2020 2020 2020   6.0]]).        
-0000e2d0: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
-0000e2e0: 745f 616c 6c63 6c6f 7365 2866 2e76 6172  t_allclose(f.var
-0000e2f0: 6961 626c 6573 5b22 6475 6d6d 7931 225d  iables["dummy1"]
-0000e300: 2e5f 6835 6473 5b31 2c20 3a5d 2c20 5b34  ._h5ds[1, :], [4
-0000e310: 2e30 2c20 352e 302c 2036 2e30 5d29 0a20  .0, 5.0, 6.0]). 
-0000e320: 2020 2020 2020 206e 702e 7465 7374 696e         np.testin
-0000e330: 672e 6173 7365 7274 5f61 6c6c 636c 6f73  g.assert_allclos
-0000e340: 6528 0a20 2020 2020 2020 2020 2020 2066  e(.            f
-0000e350: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000e360: 7931 225d 2e5f 6835 6473 5b31 3a32 2c20  y1"]._h5ds[1:2, 
-0000e370: 3a5d 2c20 5b5b 342e 302c 2035 2e30 2c20  :], [[4.0, 5.0, 
-0000e380: 362e 305d 5d0a 2020 2020 2020 2020 290a  6.0]].        ).
-0000e390: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
-0000e3a0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000e3b0: 7931 225d 2e73 6861 7065 203d 3d20 2833  y1"].shape == (3
-0000e3c0: 2c20 3329 0a20 2020 2020 2020 2061 7373  , 3).        ass
-0000e3d0: 6572 7420 662e 7661 7269 6162 6c65 735b  ert f.variables[
-0000e3e0: 2264 756d 6d79 3122 5d2e 5f68 3564 732e  "dummy1"]._h5ds.
-0000e3f0: 7368 6170 6520 3d3d 2028 332c 2033 290a  shape == (3, 3).
-0000e400: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
-0000e410: 6e67 2e61 7373 6572 745f 616c 6c63 6c6f  ng.assert_allclo
-0000e420: 7365 2866 2e76 6172 6961 626c 6573 5b22  se(f.variables["
-0000e430: 6475 6d6d 7932 225d 5b3a 5d2c 2072 6573  dummy2"][:], res
-0000e440: 3229 0a20 2020 2020 2020 206e 702e 7465  2).        np.te
-0000e450: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
-0000e460: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
-0000e470: 735b 2264 756d 6d79 3222 5d5b 312c 203a  s["dummy2"][1, :
-0000e480: 5d2c 205b 342e 302c 2035 2e30 2c20 362e  ], [4.0, 5.0, 6.
-0000e490: 305d 290a 2020 2020 2020 2020 6e70 2e74  0]).        np.t
-0000e4a0: 6573 7469 6e67 2e61 7373 6572 745f 616c  esting.assert_al
-0000e4b0: 6c63 6c6f 7365 2866 2e76 6172 6961 626c  lclose(f.variabl
-0000e4c0: 6573 5b22 6475 6d6d 7932 225d 5b31 3a32  es["dummy2"][1:2
-0000e4d0: 2c20 3a5d 2c20 5b5b 342e 302c 2035 2e30  , :], [[4.0, 5.0
-0000e4e0: 2c20 362e 305d 5d29 0a20 2020 2020 2020  , 6.0]]).       
-0000e4f0: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
-0000e500: 6c65 735b 2264 756d 6d79 3222 5d2e 7368  les["dummy2"].sh
-0000e510: 6170 6520 3d3d 2028 332c 2033 290a 2020  ape == (3, 3).  
-0000e520: 2020 2020 2020 6173 7365 7274 2066 2e76        assert f.v
-0000e530: 6172 6961 626c 6573 5b22 6475 6d6d 7932  ariables["dummy2
-0000e540: 225d 2e5f 6835 6473 2e73 6861 7065 203d  "]._h5ds.shape =
-0000e550: 3d20 2832 2c20 3329 0a20 2020 2020 2020  = (2, 3).       
-0000e560: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-0000e570: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
-0000e580: 7269 6162 6c65 735b 2264 756d 6d79 3322  riables["dummy3"
-0000e590: 5d5b 3a5d 2c20 7265 7333 290a 2020 2020  ][:], res3).    
-0000e5a0: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
-0000e5b0: 7373 6572 745f 616c 6c63 6c6f 7365 2866  ssert_allclose(f
-0000e5c0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000e5d0: 7933 225d 5b31 2c20 3a5d 2c20 5b34 2e30  y3"][1, :], [4.0
-0000e5e0: 2c20 352e 302c 2036 2e30 5d29 0a20 2020  , 5.0, 6.0]).   
-0000e5f0: 2020 2020 206e 702e 7465 7374 696e 672e       np.testing.
-0000e600: 6173 7365 7274 5f61 6c6c 636c 6f73 6528  assert_allclose(
-0000e610: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-0000e620: 6d79 3322 5d5b 313a 322c 203a 5d2c 205b  my3"][1:2, :], [
-0000e630: 5b34 2e30 2c20 352e 302c 2036 2e30 5d5d  [4.0, 5.0, 6.0]]
-0000e640: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
-0000e650: 2066 2e76 6172 6961 626c 6573 5b22 6475   f.variables["du
-0000e660: 6d6d 7933 225d 2e73 6861 7065 203d 3d20  mmy3"].shape == 
-0000e670: 2833 2c20 3329 0a20 2020 2020 2020 2061  (3, 3).        a
-0000e680: 7373 6572 7420 662e 7661 7269 6162 6c65  ssert f.variable
-0000e690: 735b 2264 756d 6d79 3322 5d2e 5f68 3564  s["dummy3"]._h5d
-0000e6a0: 732e 7368 6170 6520 3d3d 2028 322c 2033  s.shape == (2, 3
-0000e6b0: 290a 2020 2020 2020 2020 6e70 2e74 6573  ).        np.tes
-0000e6c0: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
-0000e6d0: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
-0000e6e0: 5b22 6475 6d6d 7934 225d 5b3a 5d2c 2072  ["dummy4"][:], r
-0000e6f0: 6573 3429 0a20 2020 2020 2020 2061 7373  es4).        ass
-0000e700: 6572 7420 662e 7661 7269 6162 6c65 735b  ert f.variables[
-0000e710: 2264 756d 6d79 3422 5d2e 7368 6170 6520  "dummy4"].shape 
-0000e720: 3d3d 2028 332c 2033 290a 2020 2020 2020  == (3, 3).      
-0000e730: 2020 6173 7365 7274 2066 2e76 6172 6961    assert f.varia
-0000e740: 626c 6573 5b22 6475 6d6d 7934 225d 2e5f  bles["dummy4"]._
-0000e750: 6835 6473 2e73 6861 7065 203d 3d20 2830  h5ds.shape == (0
-0000e760: 2c20 3329 0a0a 2020 2020 7769 7468 2068  , 3)..    with h
-0000e770: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-0000e780: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-0000e790: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
-0000e7a0: 2020 2066 203d 2064 735b 2274 6573 7422     f = ds["test"
-0000e7b0: 5d0a 2020 2020 2020 2020 6e70 2e74 6573  ].        np.tes
-0000e7c0: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
-0000e7d0: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
-0000e7e0: 5b22 6475 6d6d 7931 225d 5b3a 5d2c 2072  ["dummy1"][:], r
-0000e7f0: 6573 3129 0a20 2020 2020 2020 206e 702e  es1).        np.
-0000e800: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
-0000e810: 6c6c 636c 6f73 6528 662e 7661 7269 6162  llclose(f.variab
-0000e820: 6c65 735b 2264 756d 6d79 3122 5d5b 3a2c  les["dummy1"][:,
-0000e830: 203a 5d2c 2072 6573 3129 0a20 2020 2020   :], res1).     
-0000e840: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
-0000e850: 7365 7274 5f61 6c6c 636c 6f73 6528 662e  sert_allclose(f.
-0000e860: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
-0000e870: 3122 5d5b 312c 203a 5d2c 205b 342e 302c  1"][1, :], [4.0,
-0000e880: 2035 2e30 2c20 362e 305d 290a 2020 2020   5.0, 6.0]).    
-0000e890: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
-0000e8a0: 7373 6572 745f 616c 6c63 6c6f 7365 2866  ssert_allclose(f
-0000e8b0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
-0000e8c0: 7931 225d 5b31 3a32 2c20 3a5d 2c20 5b5b  y1"][1:2, :], [[
-0000e8d0: 342e 302c 2035 2e30 2c20 362e 305d 5d29  4.0, 5.0, 6.0]])
-0000e8e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-0000e8f0: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-0000e900: 6d79 3122 5d2e 7368 6170 6520 3d3d 2028  my1"].shape == (
-0000e910: 332c 2033 290a 2020 2020 2020 2020 6173  3, 3).        as
-0000e920: 7365 7274 2066 2e76 6172 6961 626c 6573  sert f.variables
-0000e930: 5b22 6475 6d6d 7931 225d 2e5f 6835 6473  ["dummy1"]._h5ds
-0000e940: 2e73 6861 7065 203d 3d20 2833 2c20 3329  .shape == (3, 3)
-0000e950: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
-0000e960: 696e 672e 6173 7365 7274 5f61 6c6c 636c  ing.assert_allcl
-0000e970: 6f73 6528 662e 7661 7269 6162 6c65 735b  ose(f.variables[
-0000e980: 2264 756d 6d79 3222 5d5b 3a5d 2c20 7265  "dummy2"][:], re
-0000e990: 7332 290a 2020 2020 2020 2020 6e70 2e74  s2).        np.t
-0000e9a0: 6573 7469 6e67 2e61 7373 6572 745f 616c  esting.assert_al
-0000e9b0: 6c63 6c6f 7365 2866 2e76 6172 6961 626c  lclose(f.variabl
-0000e9c0: 6573 5b22 6475 6d6d 7932 225d 5b31 2c20  es["dummy2"][1, 
-0000e9d0: 3a5d 2c20 5b34 2e30 2c20 352e 302c 2036  :], [4.0, 5.0, 6
-0000e9e0: 2e30 5d29 0a20 2020 2020 2020 206e 702e  .0]).        np.
-0000e9f0: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
-0000ea00: 6c6c 636c 6f73 6528 662e 7661 7269 6162  llclose(f.variab
-0000ea10: 6c65 735b 2264 756d 6d79 3222 5d5b 313a  les["dummy2"][1:
-0000ea20: 322c 203a 5d2c 205b 5b34 2e30 2c20 352e  2, :], [[4.0, 5.
-0000ea30: 302c 2036 2e30 5d5d 290a 2020 2020 2020  0, 6.0]]).      
-0000ea40: 2020 6173 7365 7274 2066 2e76 6172 6961    assert f.varia
-0000ea50: 626c 6573 5b22 6475 6d6d 7932 225d 2e73  bles["dummy2"].s
-0000ea60: 6861 7065 203d 3d20 2833 2c20 3329 0a20  hape == (3, 3). 
-0000ea70: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
-0000ea80: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
-0000ea90: 3222 5d2e 5f68 3564 732e 7368 6170 6520  2"]._h5ds.shape 
-0000eaa0: 3d3d 2028 322c 2033 290a 2020 2020 2020  == (2, 3).      
-0000eab0: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
-0000eac0: 6572 745f 616c 6c63 6c6f 7365 2866 2e76  ert_allclose(f.v
-0000ead0: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
-0000eae0: 225d 5b3a 5d2c 2072 6573 3329 0a20 2020  "][:], res3).   
-0000eaf0: 2020 2020 206e 702e 7465 7374 696e 672e       np.testing.
-0000eb00: 6173 7365 7274 5f61 6c6c 636c 6f73 6528  assert_allclose(
-0000eb10: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
-0000eb20: 6d79 3322 5d5b 312c 203a 5d2c 205b 342e  my3"][1, :], [4.
-0000eb30: 302c 2035 2e30 2c20 362e 305d 290a 2020  0, 5.0, 6.0]).  
-0000eb40: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
-0000eb50: 2e61 7373 6572 745f 616c 6c63 6c6f 7365  .assert_allclose
-0000eb60: 2866 2e76 6172 6961 626c 6573 5b22 6475  (f.variables["du
-0000eb70: 6d6d 7933 225d 5b31 3a32 2c20 3a5d 2c20  mmy3"][1:2, :], 
-0000eb80: 5b5b 342e 302c 2035 2e30 2c20 362e 305d  [[4.0, 5.0, 6.0]
-0000eb90: 5d29 0a20 2020 2020 2020 2061 7373 6572  ]).        asser
-0000eba0: 7420 662e 7661 7269 6162 6c65 735b 2264  t f.variables["d
-0000ebb0: 756d 6d79 3322 5d2e 7368 6170 6520 3d3d  ummy3"].shape ==
-0000ebc0: 2028 332c 2033 290a 2020 2020 2020 2020   (3, 3).        
-0000ebd0: 6173 7365 7274 2066 2e76 6172 6961 626c  assert f.variabl
-0000ebe0: 6573 5b22 6475 6d6d 7933 225d 2e5f 6835  es["dummy3"]._h5
-0000ebf0: 6473 2e73 6861 7065 203d 3d20 2832 2c20  ds.shape == (2, 
-0000ec00: 3329 0a20 2020 2020 2020 206e 702e 7465  3).        np.te
-0000ec10: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
-0000ec20: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
-0000ec30: 735b 2264 756d 6d79 3422 5d5b 3a5d 2c20  s["dummy4"][:], 
-0000ec40: 7265 7334 290a 2020 2020 2020 2020 6173  res4).        as
-0000ec50: 7365 7274 2066 2e76 6172 6961 626c 6573  sert f.variables
-0000ec60: 5b22 6475 6d6d 7934 225d 2e73 6861 7065  ["dummy4"].shape
-0000ec70: 203d 3d20 2833 2c20 3329 0a20 2020 2020   == (3, 3).     
-0000ec80: 2020 2061 7373 6572 7420 662e 7661 7269     assert f.vari
-0000ec90: 6162 6c65 735b 2264 756d 6d79 3422 5d2e  ables["dummy4"].
-0000eca0: 5f68 3564 732e 7368 6170 6520 3d3d 2028  _h5ds.shape == (
-0000ecb0: 302c 2033 290a 0a0a 2320 6874 7470 733a  0, 3)...# https:
-0000ecc0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
-0000ecd0: 6574 6364 662f 6835 6e65 7463 6466 2f69  etcdf/h5netcdf/i
-0000ece0: 7373 7565 732f 3133 360a 4070 7974 6573  ssues/136.@pytes
-0000ecf0: 742e 6d61 726b 2e73 6b69 7028 7265 6173  t.mark.skip(reas
-0000ed00: 6f6e 3d22 6835 7079 2062 7567 2077 6974  on="h5py bug wit
-0000ed10: 6820 7472 6163 6b5f 6f72 6465 7220 7072  h track_order pr
-0000ed20: 6576 656e 7473 2065 6469 7469 6e67 2077  events editing w
-0000ed30: 6974 6820 6e65 7443 4446 3422 290a 6465  ith netCDF4").de
-0000ed40: 6620 7465 7374 5f63 7265 6174 696f 6e5f  f test_creation_
-0000ed50: 7769 7468 5f68 356e 6574 6364 665f 6564  with_h5netcdf_ed
-0000ed60: 6974 5f77 6974 685f 6e65 7463 6466 3428  it_with_netcdf4(
-0000ed70: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000ed80: 293a 0a20 2020 2023 2049 6e20 7665 7273  ):.    # In vers
-0000ed90: 696f 6e20 302e 3132 2e30 2c20 7468 6520  ion 0.12.0, the 
-0000eda0: 7772 6f6e 6720 6669 6c65 2063 7265 6174  wrong file creat
-0000edb0: 696f 6e20 6174 7472 6962 7574 6573 2077  ion attributes w
-0000edc0: 6572 6520 7573 6564 0a20 2020 2023 206d  ere used.    # m
-0000edd0: 616b 696e 6720 6e65 7463 6466 3420 756e  aking netcdf4 un
-0000ede0: 6162 6c65 2074 6f20 6f70 656e 2066 696c  able to open fil
-0000edf0: 6573 2063 7265 6174 6564 2062 7920 6835  es created by h5
-0000ee00: 6e65 7463 6466 0a20 2020 2023 2068 7474  netcdf.    # htt
-0000ee10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-0000ee20: 6835 6e65 7463 6466 2f68 356e 6574 6364  h5netcdf/h5netcd
-0000ee30: 662f 6973 7375 6573 2f31 3238 0a20 2020  f/issues/128.   
-0000ee40: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
-0000ee50: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
-0000ee60: 7463 6466 2c20 2277 2229 2061 7320 7468  tcdf, "w") as th
-0000ee70: 655f 6669 6c65 3a0a 2020 2020 2020 2020  e_file:.        
-0000ee80: 7468 655f 6669 6c65 2e64 696d 656e 7369  the_file.dimensi
-0000ee90: 6f6e 7320 3d20 7b22 7822 3a20 357d 0a20  ons = {"x": 5}. 
-0000eea0: 2020 2020 2020 2076 6172 6961 626c 6520         variable 
-0000eeb0: 3d20 7468 655f 6669 6c65 2e63 7265 6174  = the_file.creat
-0000eec0: 655f 7661 7269 6162 6c65 2822 6865 6c6c  e_variable("hell
-0000eed0: 6f22 2c20 2822 7822 2c29 2c20 666c 6f61  o", ("x",), floa
-0000eee0: 7429 0a20 2020 2020 2020 2076 6172 6961  t).        varia
-0000eef0: 626c 655b 2e2e 2e5d 203d 2035 0a0a 2020  ble[...] = 5..  
-0000ef00: 2020 7769 7468 206e 6574 4344 4634 2e44    with netCDF4.D
-0000ef10: 6174 6173 6574 2874 6d70 5f6c 6f63 616c  ataset(tmp_local
-0000ef20: 5f6e 6574 6364 662c 206d 6f64 653d 2261  _netcdf, mode="a
-0000ef30: 2229 2061 7320 7468 655f 6669 6c65 3a0a  ") as the_file:.
-0000ef40: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
-0000ef50: 203d 2074 6865 5f66 696c 655b 2268 656c   = the_file["hel
-0000ef60: 6c6f 225d 0a20 2020 2020 2020 206e 702e  lo"].        np.
-0000ef70: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
-0000ef80: 7272 6179 5f65 7175 616c 2876 6172 6961  rray_equal(varia
-0000ef90: 626c 655b 2e2e 2e5d 2e64 6174 612c 2035  ble[...].data, 5
-0000efa0: 290a 2020 2020 2020 2020 2320 4564 6974  ).        # Edit
-0000efb0: 2061 6e20 6578 6973 7469 6e67 2076 6172   an existing var
-0000efc0: 6961 626c 650a 2020 2020 2020 2020 7661  iable.        va
-0000efd0: 7269 6162 6c65 5b3a 335d 203d 2032 0a0a  riable[:3] = 2..
-0000efe0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-0000eff0: 2061 206e 6577 2076 6172 6961 626c 650a   a new variable.
-0000f000: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
-0000f010: 203d 2074 6865 5f66 696c 652e 6372 6561   = the_file.crea
-0000f020: 7465 5661 7269 6162 6c65 2822 676f 6f64  teVariable("good
-0000f030: 6279 6522 2c20 666c 6f61 742c 2028 2278  bye", float, ("x
-0000f040: 222c 2929 0a20 2020 2020 2020 2076 6172  ",)).        var
-0000f050: 6961 626c 655b 2e2e 2e5d 203d 2031 300a  iable[...] = 10.
-0000f060: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-0000f070: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-0000f080: 6c5f 6e65 7463 6466 2c20 2261 2229 2061  l_netcdf, "a") a
-0000f090: 7320 7468 655f 6669 6c65 3a0a 2020 2020  s the_file:.    
-0000f0a0: 2020 2020 2320 456e 7375 7265 2065 6469      # Ensure edi
-0000f0b0: 7465 6420 7661 7269 6162 6c65 2069 7320  ted variable is 
-0000f0c0: 636f 6e73 6973 7465 6e74 2077 6974 6820  consistent with 
-0000f0d0: 7468 6520 6578 7065 6374 6564 2064 6174  the expected dat
-0000f0e0: 610a 2020 2020 2020 2020 7661 7269 6162  a.        variab
-0000f0f0: 6c65 203d 2074 6865 5f66 696c 655b 2268  le = the_file["h
-0000f100: 656c 6c6f 225d 0a20 2020 2020 2020 206e  ello"].        n
-0000f110: 702e 7465 7374 696e 672e 6173 7365 7274  p.testing.assert
-0000f120: 5f61 7272 6179 5f65 7175 616c 2876 6172  _array_equal(var
-0000f130: 6961 626c 655b 2e2e 2e5d 2e64 6174 612c  iable[...].data,
-0000f140: 205b 322c 2032 2c20 322c 2035 2c20 355d   [2, 2, 2, 5, 5]
-0000f150: 290a 0a20 2020 2020 2020 2023 2045 6e73  )..        # Ens
-0000f160: 7572 6520 6e65 7720 7661 7269 6162 6c65  ure new variable
-0000f170: 2069 7320 6163 6365 7373 6962 6c65 0a20   is accessible. 
-0000f180: 2020 2020 2020 2076 6172 6961 626c 6520         variable 
-0000f190: 3d20 7468 655f 6669 6c65 5b22 676f 6f64  = the_file["good
-0000f1a0: 6279 6522 5d0a 2020 2020 2020 2020 6e70  bye"].        np
-0000f1b0: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
-0000f1c0: 6172 7261 795f 6571 7561 6c28 7661 7269  array_equal(vari
-0000f1d0: 6162 6c65 5b2e 2e2e 5d2e 6461 7461 2c20  able[...].data, 
-0000f1e0: 3130 290a 0a0a 6465 6620 7465 7374 5f74  10)...def test_t
-0000f1f0: 7261 636b 5f6f 7264 6572 5f73 7065 6369  rack_order_speci
-0000f200: 6669 6361 7469 6f6e 2874 6d70 5f6c 6f63  fication(tmp_loc
-0000f210: 616c 5f6e 6574 6364 6629 3a0a 2020 2020  al_netcdf):.    
-0000f220: 2320 5768 696c 6520 6e65 7463 6466 342d  # While netcdf4-
-0000f230: 6320 6861 7320 6869 7374 6f72 6963 616c  c has historical
-0000f240: 6c79 206f 6e6c 7920 616c 6c6f 7765 6420  ly only allowed 
-0000f250: 7472 6163 6b5f 6f72 6465 7220 746f 2062  track_order to b
-0000f260: 6520 5472 7565 0a20 2020 2023 2054 6865  e True.    # The
-0000f270: 7265 2064 6f65 736e 2774 2073 6565 6d20  re doesn't seem 
-0000f280: 746f 2062 6520 6120 676f 6f64 2072 6561  to be a good rea
-0000f290: 736f 6e20 666f 7220 7468 6973 0a20 2020  son for this.   
-0000f2a0: 2023 2068 7474 7073 3a2f 2f67 6974 6875   # https://githu
-0000f2b0: 622e 636f 6d2f 556e 6964 6174 612f 6e65  b.com/Unidata/ne
-0000f2c0: 7463 6466 2d63 2f69 7373 7565 732f 3230  tcdf-c/issues/20
-0000f2d0: 3534 2068 6973 746f 7269 6361 6c6c 792c  54 historically,
-0000f2e0: 2068 356e 6574 6364 660a 2020 2020 2320   h5netcdf.    # 
-0000f2f0: 6861 7320 6e6f 7420 7370 6563 6966 6965  has not specifie
-0000f300: 6420 7468 6973 2070 6172 616d 6574 6572  d this parameter
-0000f310: 2028 6c65 6176 696e 6720 6974 2069 6d70   (leaving it imp
-0000f320: 6c69 6369 7465 6c79 2061 7320 4661 6c73  licitely as Fals
-0000f330: 6529 0a20 2020 2023 2057 6520 7761 6e74  e).    # We want
-0000f340: 2074 6f20 6d61 6b65 2073 7572 6520 7765   to make sure we
-0000f350: 2061 6c6c 6f77 2062 6f74 6820 6865 7265   allow both here
-0000f360: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-0000f370: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-0000f380: 6c5f 6e65 7463 6466 2c20 2277 222c 2074  l_netcdf, "w", t
-0000f390: 7261 636b 5f6f 7264 6572 3d46 616c 7365  rack_order=False
-0000f3a0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-0000f3b0: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
-0000f3c0: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
-0000f3d0: 6c5f 6e65 7463 6466 2c20 2277 222c 2074  l_netcdf, "w", t
-0000f3e0: 7261 636b 5f6f 7264 6572 3d54 7275 6529  rack_order=True)
-0000f3f0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0000f400: 0a23 2054 6869 7320 7368 6f75 6c64 2061  .# This should a
-0000f410: 6c77 6179 7320 776f 726b 2077 6974 6820  lways work with 
-0000f420: 7468 6520 6465 6661 756c 7420 6669 6c65  the default file
-0000f430: 206f 7065 6e69 6e67 2073 6574 7469 6e67   opening setting
-0000f440: 730a 2320 6874 7470 733a 2f2f 6769 7468  s.# https://gith
-0000f450: 7562 2e63 6f6d 2f68 356e 6574 6364 662f  ub.com/h5netcdf/
-0000f460: 6835 6e65 7463 6466 2f69 7373 7565 732f  h5netcdf/issues/
-0000f470: 3133 3623 6973 7375 6563 6f6d 6d65 6e74  136#issuecomment
-0000f480: 2d31 3031 3734 3537 3036 370a 6465 6620  -1017457067.def 
-0000f490: 7465 7374 5f6d 6f72 655f 7468 616e 5f37  test_more_than_7
-0000f4a0: 5f61 7474 725f 6372 6561 7469 6f6e 2874  _attr_creation(t
-0000f4b0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 6629  mp_local_netcdf)
-0000f4c0: 3a0a 2020 2020 7769 7468 2068 356e 6574  :.    with h5net
-0000f4d0: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
-0000f4e0: 616c 5f6e 6574 6364 662c 2022 7722 2920  al_netcdf, "w") 
-0000f4f0: 6173 2068 3566 696c 653a 0a20 2020 2020  as h5file:.     
-0000f500: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000f510: 6528 3130 3029 3a0a 2020 2020 2020 2020  e(100):.        
-0000f520: 2020 2020 6835 6669 6c65 2e61 7474 7273      h5file.attrs
-0000f530: 5b66 226b 6579 7b69 7d22 5d20 3d20 690a  [f"key{i}"] = i.
-0000f540: 2020 2020 2020 2020 2020 2020 6835 6669              h5fi
-0000f550: 6c65 2e61 7474 7273 5b66 226b 6579 7b69  le.attrs[f"key{i
-0000f560: 7d22 5d20 3d20 300a 0a0a 2320 4164 6420  }"] = 0...# Add 
-0000f570: 6120 7465 7374 2074 6861 7420 6973 2073  a test that is s
-0000f580: 7570 706f 7365 6420 746f 2066 6169 6c20  upposed to fail 
-0000f590: 696e 2072 656c 6174 696f 6e20 746f 2069  in relation to i
-0000f5a0: 7373 7565 2023 3133 360a 2320 5765 2063  ssue #136.# We c
-0000f5b0: 686f 6f73 6520 746f 206d 6f6e 6974 6f72  hoose to monitor
-0000f5c0: 2077 6865 6e20 6835 7079 2077 696c 6c20   when h5py will 
-0000f5d0: 6861 7665 2066 6978 6564 2074 6865 6972  have fixed their
-0000f5e0: 2069 7373 7565 2069 6e20 6f75 7220 7465   issue in our te
-0000f5f0: 7374 2073 7569 7465 0a23 2074 6f20 656e  st suite.# to en
-0000f600: 6861 6e63 6520 6d61 696e 7461 696e 6162  hance maintainab
-0000f610: 696c 6974 790a 2320 6874 7470 733a 2f2f  ility.# https://
-0000f620: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
-0000f630: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
-0000f640: 7565 732f 3133 3623 6973 7375 6563 6f6d  ues/136#issuecom
-0000f650: 6d65 6e74 2d31 3031 3734 3537 3036 370a  ment-1017457067.
-0000f660: 4070 7974 6573 742e 6d61 726b 2e70 6172  @pytest.mark.par
-0000f670: 616d 6574 7269 7a65 2822 7472 6163 6b5f  ametrize("track_
-0000f680: 6f72 6465 7222 2c20 5b46 616c 7365 2c20  order", [False, 
-0000f690: 5472 7565 5d29 0a64 6566 2074 6573 745f  True]).def test_
-0000f6a0: 6d6f 7265 5f74 6861 6e5f 375f 6174 7472  more_than_7_attr
-0000f6b0: 5f63 7265 6174 696f 6e5f 7472 6163 6b5f  _creation_track_
-0000f6c0: 6f72 6465 7228 746d 705f 6c6f 6361 6c5f  order(tmp_local_
-0000f6d0: 6e65 7463 6466 2c20 7472 6163 6b5f 6f72  netcdf, track_or
-0000f6e0: 6465 7229 3a0a 2020 2020 6835 7079 5f76  der):.    h5py_v
-0000f6f0: 6572 7369 6f6e 203d 2076 6572 7369 6f6e  ersion = version
-0000f700: 2e70 6172 7365 2868 3570 792e 5f5f 7665  .parse(h5py.__ve
-0000f710: 7273 696f 6e5f 5f29 0a20 2020 2069 6620  rsion__).    if 
-0000f720: 7472 6163 6b5f 6f72 6465 7220 616e 6420  track_order and 
-0000f730: 6835 7079 5f76 6572 7369 6f6e 203c 2076  h5py_version < v
-0000f740: 6572 7369 6f6e 2e70 6172 7365 2822 332e  ersion.parse("3.
-0000f750: 372e 3022 293a 0a20 2020 2020 2020 2065  7.0"):.        e
-0000f760: 7870 6563 7465 645f 6572 726f 7273 203d  xpected_errors =
-0000f770: 2070 7974 6573 742e 7261 6973 6573 284b   pytest.raises(K
-0000f780: 6579 4572 726f 7229 0a20 2020 2065 6c73  eyError).    els
-0000f790: 653a 0a20 2020 2020 2020 2023 2057 6520  e:.        # We 
-0000f7a0: 646f 6e27 7420 6578 7065 6374 2061 6e79  don't expect any
-0000f7b0: 2065 7272 6f72 732e 2054 6869 7320 6973   errors. This is
-0000f7c0: 2065 6666 6563 7469 7665 6c79 2061 2076   effectively a v
-0000f7d0: 6f69 6420 636f 6e74 6578 7420 6d61 6e61  oid context mana
-0000f7e0: 6765 720a 2020 2020 2020 2020 6578 7065  ger.        expe
-0000f7f0: 6374 6564 5f65 7272 6f72 7320 3d20 6d65  cted_errors = me
-0000f800: 6d6f 7279 7669 6577 2862 2222 290a 0a20  moryview(b"").. 
-0000f810: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-0000f820: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-0000f830: 6e65 7463 6466 2c20 2277 222c 2074 7261  netcdf, "w", tra
-0000f840: 636b 5f6f 7264 6572 3d74 7261 636b 5f6f  ck_order=track_o
-0000f850: 7264 6572 2920 6173 2068 3566 696c 653a  rder) as h5file:
-0000f860: 0a20 2020 2020 2020 2077 6974 6820 6578  .        with ex
-0000f870: 7065 6374 6564 5f65 7272 6f72 733a 0a20  pected_errors:. 
-0000f880: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-0000f890: 2069 6e20 7261 6e67 6528 3130 3029 3a0a   in range(100):.
-0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8b0: 6835 6669 6c65 2e61 7474 7273 5b66 226b  h5file.attrs[f"k
-0000f8c0: 6579 7b69 7d22 5d20 3d20 690a 2020 2020  ey{i}"] = i.    
-0000f8d0: 2020 2020 2020 2020 2020 2020 6835 6669              h5fi
-0000f8e0: 6c65 2e61 7474 7273 5b66 226b 6579 7b69  le.attrs[f"key{i
-0000f8f0: 7d22 5d20 3d20 300a 0a0a 6465 6620 7465  }"] = 0...def te
-0000f900: 7374 5f67 726f 7570 5f6e 616d 6573 2874  st_group_names(t
-0000f910: 6d70 5f6c 6f63 616c 5f6e 6574 6364 6629  mp_local_netcdf)
-0000f920: 3a0a 2020 2020 2320 6874 7470 733a 2f2f  :.    # https://
-0000f930: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
-0000f940: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
-0000f950: 7565 732f 3638 0a20 2020 2077 6974 6820  ues/68.    with 
-0000f960: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
-0000f970: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000f980: 2c20 6d6f 6465 3d22 7722 2920 6173 2064  , mode="w") as d
-0000f990: 733a 0a20 2020 2020 2020 2066 6f72 2069  s:.        for i
-0000f9a0: 2069 6e20 7261 6e67 6528 3130 293a 0a20   in range(10):. 
-0000f9b0: 2020 2020 2020 2020 2020 2064 7320 3d20             ds = 
-0000f9c0: 6473 2e63 7265 6174 6547 726f 7570 2866  ds.createGroup(f
-0000f9d0: 2267 726f 7570 7b69 3a30 3264 7d22 290a  "group{i:02d}").
-0000f9e0: 0a20 2020 2077 6974 6820 6e65 7443 4446  .    with netCDF
-0000f9f0: 342e 4461 7461 7365 7428 746d 705f 6c6f  4.Dataset(tmp_lo
-0000fa00: 6361 6c5f 6e65 7463 6466 2c20 2272 2229  cal_netcdf, "r")
-0000fa10: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-0000fa20: 6173 7365 7274 2064 732e 6e61 6d65 203d  assert ds.name =
-0000fa30: 3d20 222f 220a 2020 2020 2020 2020 6e61  = "/".        na
-0000fa40: 6d65 203d 2022 220a 2020 2020 2020 2020  me = "".        
-0000fa50: 666f 7220 6920 696e 2072 616e 6765 2831  for i in range(1
-0000fa60: 3029 3a0a 2020 2020 2020 2020 2020 2020  0):.            
-0000fa70: 6e61 6d65 203d 2022 2f22 2e6a 6f69 6e28  name = "/".join(
-0000fa80: 5b6e 616d 652c 2066 2267 726f 7570 7b69  [name, f"group{i
-0000fa90: 3a30 3264 7d22 5d29 0a20 2020 2020 2020  :02d}"]).       
-0000faa0: 2020 2020 2061 7373 6572 7420 6473 5b6e       assert ds[n
-0000fab0: 616d 655d 2e6e 616d 6520 3d3d 206e 616d  ame].name == nam
-0000fac0: 652e 7370 6c69 7428 222f 2229 5b2d 315d  e.split("/")[-1]
-0000fad0: 0a0a 2020 2020 7769 7468 206c 6567 6163  ..    with legac
-0000fae0: 7961 7069 2e44 6174 6173 6574 2874 6d70  yapi.Dataset(tmp
-0000faf0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-0000fb00: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
-0000fb10: 2020 2061 7373 6572 7420 6473 2e6e 616d     assert ds.nam
-0000fb20: 6520 3d3d 2022 2f22 0a20 2020 2020 2020  e == "/".       
-0000fb30: 206e 616d 6520 3d20 2222 0a20 2020 2020   name = "".     
-0000fb40: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-0000fb50: 6528 3130 293a 0a20 2020 2020 2020 2020  e(10):.         
-0000fb60: 2020 206e 616d 6520 3d20 222f 222e 6a6f     name = "/".jo
-0000fb70: 696e 285b 6e61 6d65 2c20 6622 6772 6f75  in([name, f"grou
-0000fb80: 707b 693a 3032 647d 225d 290a 2020 2020  p{i:02d}"]).    
-0000fb90: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-0000fba0: 735b 6e61 6d65 5d2e 6e61 6d65 203d 3d20  s[name].name == 
-0000fbb0: 6e61 6d65 2e73 706c 6974 2822 2f22 295b  name.split("/")[
-0000fbc0: 2d31 5d0a 0a20 2020 2077 6974 6820 6835  -1]..    with h5
-0000fbd0: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
-0000fbe0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
-0000fbf0: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
-0000fc00: 2020 6173 7365 7274 2064 732e 6e61 6d65    assert ds.name
-0000fc10: 203d 3d20 222f 220a 2020 2020 2020 2020   == "/".        
-0000fc20: 6e61 6d65 203d 2022 220a 2020 2020 2020  name = "".      
-0000fc30: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0000fc40: 2831 3029 3a0a 2020 2020 2020 2020 2020  (10):.          
-0000fc50: 2020 6e61 6d65 203d 2022 2f22 2e6a 6f69    name = "/".joi
-0000fc60: 6e28 5b6e 616d 652c 2066 2267 726f 7570  n([name, f"group
-0000fc70: 7b69 3a30 3264 7d22 5d29 0a20 2020 2020  {i:02d}"]).     
-0000fc80: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-0000fc90: 5b6e 616d 655d 2e6e 616d 6520 3d3d 206e  [name].name == n
-0000fca0: 616d 650a 0a0a 6465 6620 7465 7374 5f6c  ame...def test_l
-0000fcb0: 6567 6163 7961 7069 5f65 6e64 6961 6e65  egacyapi_endiane
-0000fcc0: 7373 2874 6d70 5f6c 6f63 616c 5f6e 6574  ss(tmp_local_net
-0000fcd0: 6364 6629 3a0a 2020 2020 2320 6874 7470  cdf):.    # http
-0000fce0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-0000fcf0: 356e 6574 6364 662f 6835 6e65 7463 6466  5netcdf/h5netcdf
-0000fd00: 2f69 7373 7565 732f 3135 0a20 2020 2062  /issues/15.    b
-0000fd10: 6967 203d 206c 6567 6163 7961 7069 2e5f  ig = legacyapi._
-0000fd20: 6368 6563 6b5f 7265 7475 726e 5f64 7479  check_return_dty
-0000fd30: 7065 5f65 6e64 6961 6e65 7373 2822 6269  pe_endianess("bi
-0000fd40: 6722 290a 2020 2020 6c69 7474 6c65 203d  g").    little =
-0000fd50: 206c 6567 6163 7961 7069 2e5f 6368 6563   legacyapi._chec
-0000fd60: 6b5f 7265 7475 726e 5f64 7479 7065 5f65  k_return_dtype_e
-0000fd70: 6e64 6961 6e65 7373 2822 6c69 7474 6c65  ndianess("little
-0000fd80: 2229 0a20 2020 206e 6174 6976 6520 3d20  ").    native = 
-0000fd90: 6c65 6761 6379 6170 692e 5f63 6865 636b  legacyapi._check
-0000fda0: 5f72 6574 7572 6e5f 6474 7970 655f 656e  _return_dtype_en
-0000fdb0: 6469 616e 6573 7328 226e 6174 6976 6522  dianess("native"
-0000fdc0: 290a 0a20 2020 2077 6974 6820 6c65 6761  )..    with lega
-0000fdd0: 6379 6170 692e 4461 7461 7365 7428 746d  cyapi.Dataset(tm
-0000fde0: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-0000fdf0: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
-0000fe00: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-0000fe10: 656e 7369 6f6e 2822 7822 2c20 3429 0a20  ension("x", 4). 
-0000fe20: 2020 2020 2020 2023 2074 6573 7420 6372         # test cr
-0000fe30: 6561 7469 6e67 2076 6172 6961 626c 6520  eating variable 
-0000fe40: 7573 696e 6720 656e 6469 616e 206b 6579  using endian key
-0000fe50: 776f 7264 2061 7267 756d 656e 740a 2020  word argument.  
-0000fe60: 2020 2020 2020 7620 3d20 6473 2e63 7265        v = ds.cre
-0000fe70: 6174 6556 6172 6961 626c 6528 2262 6967  ateVariable("big
-0000fe80: 222c 2069 6e74 2c20 2822 7822 292c 2065  ", int, ("x"), e
-0000fe90: 6e64 6961 6e3d 2262 6967 2229 0a20 2020  ndian="big").   
-0000fea0: 2020 2020 2076 5b2e 2e2e 5d20 3d20 3635       v[...] = 65
-0000feb0: 3533 330a 2020 2020 2020 2020 7620 3d20  533.        v = 
-0000fec0: 6473 2e63 7265 6174 6556 6172 6961 626c  ds.createVariabl
-0000fed0: 6528 226c 6974 746c 6522 2c20 696e 742c  e("little", int,
-0000fee0: 2028 2278 2229 2c20 656e 6469 616e 3d22   ("x"), endian="
-0000fef0: 6c69 7474 6c65 2229 0a20 2020 2020 2020  little").       
-0000ff00: 2076 5b2e 2e2e 5d20 3d20 3635 3533 330a   v[...] = 65533.
-0000ff10: 2020 2020 2020 2020 7620 3d20 6473 2e63          v = ds.c
-0000ff20: 7265 6174 6556 6172 6961 626c 6528 226e  reateVariable("n
-0000ff30: 6174 6976 6522 2c20 696e 742c 2028 2278  ative", int, ("x
-0000ff40: 2229 2c20 656e 6469 616e 3d22 6e61 7469  "), endian="nati
-0000ff50: 7665 2229 0a20 2020 2020 2020 2076 5b2e  ve").        v[.
-0000ff60: 2e2e 5d20 3d20 3635 3533 350a 0a20 2020  ..] = 65535..   
-0000ff70: 2077 6974 6820 6835 7079 2e46 696c 6528   with h5py.File(
-0000ff80: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-0000ff90: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
-0000ffa0: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
-0000ffb0: 2262 6967 225d 2e64 7479 7065 2e62 7974  "big"].dtype.byt
-0000ffc0: 656f 7264 6572 203d 3d20 6269 670a 2020  eorder == big.  
-0000ffd0: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
-0000ffe0: 226c 6974 746c 6522 5d2e 6474 7970 652e  "little"].dtype.
-0000fff0: 6279 7465 6f72 6465 7220 3d3d 206c 6974  byteorder == lit
-00010000: 746c 650a 2020 2020 2020 2020 6173 7365  tle.        asse
-00010010: 7274 2064 735b 226e 6174 6976 6522 5d2e  rt ds["native"].
-00010020: 6474 7970 652e 6279 7465 6f72 6465 7220  dtype.byteorder 
-00010030: 3d3d 206e 6174 6976 650a 0a20 2020 2077  == native..    w
-00010040: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-00010050: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-00010060: 6466 2c20 2272 2229 2061 7320 6473 3a0a  df, "r") as ds:.
-00010070: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00010080: 735b 2262 6967 225d 2e64 7479 7065 2e62  s["big"].dtype.b
-00010090: 7974 656f 7264 6572 203d 3d20 6269 670a  yteorder == big.
-000100a0: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-000100b0: 735b 226c 6974 746c 6522 5d2e 6474 7970  s["little"].dtyp
-000100c0: 652e 6279 7465 6f72 6465 7220 3d3d 206c  e.byteorder == l
-000100d0: 6974 746c 650a 2020 2020 2020 2020 6173  ittle.        as
-000100e0: 7365 7274 2064 735b 226e 6174 6976 6522  sert ds["native"
-000100f0: 5d2e 6474 7970 652e 6279 7465 6f72 6465  ].dtype.byteorde
-00010100: 7220 3d3d 206e 6174 6976 650a 0a20 2020  r == native..   
-00010110: 2077 6974 6820 6c65 6761 6379 6170 692e   with legacyapi.
-00010120: 4461 7461 7365 7428 746d 705f 6c6f 6361  Dataset(tmp_loca
-00010130: 6c5f 6e65 7463 6466 2c20 2272 2229 2061  l_netcdf, "r") a
-00010140: 7320 6473 3a0a 2020 2020 2020 2020 6173  s ds:.        as
-00010150: 7365 7274 2064 735b 2262 6967 225d 2e64  sert ds["big"].d
-00010160: 7479 7065 2e62 7974 656f 7264 6572 203d  type.byteorder =
-00010170: 3d20 6269 670a 2020 2020 2020 2020 6173  = big.        as
-00010180: 7365 7274 2064 735b 226c 6974 746c 6522  sert ds["little"
-00010190: 5d2e 6474 7970 652e 6279 7465 6f72 6465  ].dtype.byteorde
-000101a0: 7220 3d3d 206c 6974 746c 650a 2020 2020  r == little.    
-000101b0: 2020 2020 6173 7365 7274 2064 735b 226e      assert ds["n
-000101c0: 6174 6976 6522 5d2e 6474 7970 652e 6279  ative"].dtype.by
-000101d0: 7465 6f72 6465 7220 3d3d 206e 6174 6976  teorder == nativ
-000101e0: 650a 0a20 2020 2077 6974 6820 6e65 7443  e..    with netC
-000101f0: 4446 342e 4461 7461 7365 7428 746d 705f  DF4.Dataset(tmp_
-00010200: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2272  local_netcdf, "r
-00010210: 2229 2061 7320 6473 3a0a 2020 2020 2020  ") as ds:.      
-00010220: 2020 6173 7365 7274 2064 735b 2262 6967    assert ds["big
-00010230: 225d 2e64 7479 7065 2e62 7974 656f 7264  "].dtype.byteord
-00010240: 6572 203d 3d20 6269 670a 2020 2020 2020  er == big.      
-00010250: 2020 6173 7365 7274 2064 735b 226c 6974    assert ds["lit
-00010260: 746c 6522 5d2e 6474 7970 652e 6279 7465  tle"].dtype.byte
-00010270: 6f72 6465 7220 3d3d 206c 6974 746c 650a  order == little.
-00010280: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00010290: 735b 226e 6174 6976 6522 5d2e 6474 7970  s["native"].dtyp
-000102a0: 652e 6279 7465 6f72 6465 7220 3d3d 206e  e.byteorder == n
-000102b0: 6174 6976 650a 0a0a 6465 6620 7465 7374  ative...def test
-000102c0: 5f62 6f6f 6c5f 736c 6963 696e 675f 6c65  _bool_slicing_le
-000102d0: 6e67 7468 5f6f 6e65 5f64 696d 2874 6d70  ngth_one_dim(tmp
-000102e0: 5f6c 6f63 616c 5f6e 6574 6364 6629 3a0a  _local_netcdf):.
-000102f0: 2020 2020 2320 7365 6520 6874 7470 733a      # see https:
-00010300: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
-00010310: 6574 6364 662f 6835 6e65 7463 6466 2f69  etcdf/h5netcdf/i
-00010320: 7373 7565 732f 3233 0a20 2020 2077 6974  ssues/23.    wit
-00010330: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00010340: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00010350: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
-00010360: 2020 2020 2020 6473 2e64 696d 656e 7369        ds.dimensi
-00010370: 6f6e 7320 3d20 7b22 7822 3a20 312c 2022  ons = {"x": 1, "
-00010380: 7922 3a20 327d 0a20 2020 2020 2020 2076  y": 2}.        v
-00010390: 203d 2064 732e 6372 6561 7465 5f76 6172   = ds.create_var
-000103a0: 6961 626c 6528 2268 656c 6c6f 222c 2028  iable("hello", (
-000103b0: 2278 222c 2022 7922 292c 2022 666c 6f61  "x", "y"), "floa
-000103c0: 7422 290a 2020 2020 2020 2020 765b 3a5d  t").        v[:]
-000103d0: 203d 206e 702e 6f6e 6573 2828 312c 2032   = np.ones((1, 2
-000103e0: 2929 0a0a 2020 2020 626f 6f6c 5f73 6c69  ))..    bool_sli
-000103f0: 6365 203d 206e 702e 6172 7261 7928 5b31  ce = np.array([1
-00010400: 5d2c 2064 7479 7065 3d62 6f6f 6c29 0a0a  ], dtype=bool)..
-00010410: 2020 2020 2320 776f 726b 7320 666f 7220      # works for 
-00010420: 6c65 6761 6379 2041 5049 0a20 2020 2077  legacy API.    w
-00010430: 6974 6820 6c65 6761 6379 6170 692e 4461  ith legacyapi.Da
-00010440: 7461 7365 7428 746d 705f 6c6f 6361 6c5f  taset(tmp_local_
-00010450: 6e65 7463 6466 2c20 2261 2229 2061 7320  netcdf, "a") as 
-00010460: 6473 3a0a 2020 2020 2020 2020 6461 7461  ds:.        data
-00010470: 203d 2064 735b 2268 656c 6c6f 225d 5b62   = ds["hello"][b
-00010480: 6f6f 6c5f 736c 6963 652c 203a 5d0a 2020  ool_slice, :].  
-00010490: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
-000104a0: 2e61 7373 6572 745f 6571 7561 6c28 6461  .assert_equal(da
-000104b0: 7461 2c20 6e70 2e6f 6e65 7328 2831 2c20  ta, np.ones((1, 
-000104c0: 3229 2929 0a20 2020 2020 2020 2064 735b  2))).        ds[
-000104d0: 2268 656c 6c6f 225d 5b62 6f6f 6c5f 736c  "hello"][bool_sl
-000104e0: 6963 652c 203a 5d20 3d20 6e70 2e7a 6572  ice, :] = np.zer
-000104f0: 6f73 2828 312c 2032 2929 0a20 2020 2020  os((1, 2)).     
-00010500: 2020 2064 6174 6120 3d20 6473 5b22 6865     data = ds["he
-00010510: 6c6c 6f22 5d5b 626f 6f6c 5f73 6c69 6365  llo"][bool_slice
-00010520: 2c20 3a5d 0a20 2020 2020 2020 206e 702e  , :].        np.
-00010530: 7465 7374 696e 672e 6173 7365 7274 5f65  testing.assert_e
-00010540: 7175 616c 2864 6174 612c 206e 702e 7a65  qual(data, np.ze
-00010550: 726f 7328 2831 2c20 3229 2929 0a0a 2020  ros((1, 2)))..  
-00010560: 2020 2320 7368 6f75 6c64 2072 6169 7365    # should raise
-00010570: 2066 6f72 2068 3570 7920 3e3d 2033 2e30   for h5py >= 3.0
-00010580: 2e30 2061 6e64 2068 3570 7920 3c20 332e  .0 and h5py < 3.
-00010590: 372e 300a 2020 2020 2320 6874 7470 733a  7.0.    # https:
-000105a0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 3570  //github.com/h5p
-000105b0: 792f 6835 7079 2f70 756c 6c2f 3230 3739  y/h5py/pull/2079
-000105c0: 0a20 2020 2023 2068 7474 7073 3a2f 2f67  .    # https://g
-000105d0: 6974 6875 622e 636f 6d2f 6835 6e65 7463  ithub.com/h5netc
-000105e0: 6466 2f68 356e 6574 6364 662f 7075 6c6c  df/h5netcdf/pull
-000105f0: 2f31 3235 2f0a 2020 2020 7769 7468 2068  /125/.    with h
-00010600: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-00010610: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-00010620: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
-00010630: 2020 2068 3570 795f 7665 7273 696f 6e20     h5py_version 
-00010640: 3d20 7665 7273 696f 6e2e 7061 7273 6528  = version.parse(
-00010650: 6835 7079 2e5f 5f76 6572 7369 6f6e 5f5f  h5py.__version__
-00010660: 290a 2020 2020 2020 2020 6966 2076 6572  ).        if ver
-00010670: 7369 6f6e 2e70 6172 7365 2822 332e 302e  sion.parse("3.0.
-00010680: 3022 2920 3c3d 2068 3570 795f 7665 7273  0") <= h5py_vers
-00010690: 696f 6e20 3c20 7665 7273 696f 6e2e 7061  ion < version.pa
-000106a0: 7273 6528 2233 2e37 2e30 2229 3a0a 2020  rse("3.7.0"):.  
-000106b0: 2020 2020 2020 2020 2020 6572 726f 7220            error 
-000106c0: 3d20 2249 6e64 6578 696e 6720 6172 7261  = "Indexing arra
-000106d0: 7973 206d 7573 7420 6861 7665 2069 6e74  ys must have int
-000106e0: 6567 6572 2064 7479 7065 7322 0a20 2020  eger dtypes".   
-000106f0: 2020 2020 2020 2020 2077 6974 6820 7079           with py
-00010700: 7465 7374 2e72 6169 7365 7328 5479 7065  test.raises(Type
-00010710: 4572 726f 7229 2061 7320 653a 0a20 2020  Error) as e:.   
-00010720: 2020 2020 2020 2020 2020 2020 2064 735b               ds[
-00010730: 2268 656c 6c6f 225d 5b62 6f6f 6c5f 736c  "hello"][bool_sl
-00010740: 6963 652c 203a 5d0a 2020 2020 2020 2020  ice, :].        
-00010750: 2020 2020 6173 7365 7274 2065 7272 6f72      assert error
-00010760: 203d 3d20 7374 7228 652e 7661 6c75 6529   == str(e.value)
-00010770: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00010780: 2020 2020 2020 2020 2020 2064 735b 2268             ds["h
-00010790: 656c 6c6f 225d 5b62 6f6f 6c5f 736c 6963  ello"][bool_slic
-000107a0: 652c 203a 5d0a 0a0a 6465 6620 7465 7374  e, :]...def test
-000107b0: 5f66 616e 6379 5f69 6e64 6578 696e 6728  _fancy_indexing(
-000107c0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-000107d0: 293a 0a20 2020 2023 2072 6567 7265 7373  ):.    # regress
-000107e0: 696f 6e20 7465 7374 2066 6f72 2068 7474  ion test for htt
-000107f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00010800: 7079 6461 7461 2f78 6172 7261 792f 6973  pydata/xarray/is
-00010810: 7375 6573 2f37 3135 340a 2020 2020 7769  sues/7154.    wi
-00010820: 7468 2068 356e 6574 6364 662e 6c65 6761  th h5netcdf.lega
-00010830: 6379 6170 692e 4461 7461 7365 7428 746d  cyapi.Dataset(tm
-00010840: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-00010850: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
-00010860: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-00010870: 656e 7369 6f6e 2822 7822 2c20 4e6f 6e65  ension("x", None
-00010880: 290a 2020 2020 2020 2020 6473 2e63 7265  ).        ds.cre
-00010890: 6174 6544 696d 656e 7369 6f6e 2822 7922  ateDimension("y"
-000108a0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
-000108b0: 6473 2e63 7265 6174 6556 6172 6961 626c  ds.createVariabl
-000108c0: 6528 2268 656c 6c6f 222c 2069 6e74 2c20  e("hello", int, 
-000108d0: 2822 7822 2c20 2279 2229 2c20 6669 6c6c  ("x", "y"), fill
-000108e0: 5f76 616c 7565 3d30 290a 2020 2020 2020  _value=0).      
-000108f0: 2020 6473 5b22 6865 6c6c 6f22 5d5b 3a35    ds["hello"][:5
-00010900: 2c20 3a31 305d 203d 206e 702e 6172 616e  , :10] = np.aran
-00010910: 6765 2835 202a 2031 302c 2064 7479 7065  ge(5 * 10, dtype
-00010920: 3d22 696e 7422 292e 7265 7368 6170 6528  ="int").reshape(
-00010930: 2835 2c20 3130 2929 0a20 2020 2020 2020  (5, 10)).       
-00010940: 2064 732e 6372 6561 7465 5661 7269 6162   ds.createVariab
-00010950: 6c65 2822 6865 6c6c 6f32 222c 2069 6e74  le("hello2", int
-00010960: 2c20 2822 7822 2c20 2279 2229 290a 2020  , ("x", "y")).  
-00010970: 2020 2020 2020 6473 5b22 6865 6c6c 6f32        ds["hello2
-00010980: 225d 5b3a 3130 2c20 3a32 305d 203d 206e  "][:10, :20] = n
-00010990: 702e 6172 616e 6765 2831 3020 2a20 3230  p.arange(10 * 20
-000109a0: 2c20 6474 7970 653d 2269 6e74 2229 2e72  , dtype="int").r
-000109b0: 6573 6861 7065 2828 3130 2c20 3230 2929  eshape((10, 20))
-000109c0: 0a0a 2020 2020 7769 7468 206c 6567 6163  ..    with legac
-000109d0: 7961 7069 2e44 6174 6173 6574 2874 6d70  yapi.Dataset(tmp
-000109e0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-000109f0: 6122 2920 6173 2064 733a 0a20 2020 2020  a") as ds:.     
-00010a00: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
-00010a10: 7365 7274 5f61 7272 6179 5f65 7175 616c  sert_array_equal
-00010a20: 2864 735b 2268 656c 6c6f 225d 5b31 2c20  (ds["hello"][1, 
-00010a30: 5b37 2c20 382c 2039 5d5d 2c20 5b31 372c  [7, 8, 9]], [17,
-00010a40: 2031 382c 2031 395d 290a 2020 2020 2020   18, 19]).      
-00010a50: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
-00010a60: 6572 745f 6172 7261 795f 6571 7561 6c28  ert_array_equal(
-00010a70: 6473 5b22 6865 6c6c 6f22 5d5b 312c 205b  ds["hello"][1, [
-00010a80: 392c 2031 302c 2031 315d 5d2c 205b 3139  9, 10, 11]], [19
-00010a90: 2c20 302c 2030 5d29 0a20 2020 2020 2020  , 0, 0]).       
-00010aa0: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-00010ab0: 7274 5f61 7272 6179 5f65 7175 616c 2864  rt_array_equal(d
-00010ac0: 735b 2268 656c 6c6f 225d 5b31 2c20 736c  s["hello"][1, sl
-00010ad0: 6963 6528 392c 2031 3229 5d2c 205b 3139  ice(9, 12)], [19
-00010ae0: 2c20 302c 2030 5d29 0a20 2020 2020 2020  , 0, 0]).       
-00010af0: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
-00010b00: 7274 5f61 7272 6179 5f65 7175 616c 2864  rt_array_equal(d
-00010b10: 735b 2268 656c 6c6f 225d 5b5b 322c 2033  s["hello"][[2, 3
-00010b20: 2c20 345d 2c20 315d 2c20 5b32 312c 2033  , 4], 1], [21, 3
-00010b30: 312c 2034 315d 290a 2020 2020 2020 2020  1, 41]).        
-00010b40: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
-00010b50: 745f 6172 7261 795f 6571 7561 6c28 6473  t_array_equal(ds
-00010b60: 5b22 6865 6c6c 6f22 5d5b 5b34 2c20 352c  ["hello"][[4, 5,
-00010b70: 2036 5d2c 2031 5d2c 205b 3431 2c20 302c   6], 1], [41, 0,
-00010b80: 2030 5d29 0a20 2020 2020 2020 206e 702e   0]).        np.
-00010b90: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
-00010ba0: 7272 6179 5f65 7175 616c 2864 735b 2268  rray_equal(ds["h
-00010bb0: 656c 6c6f 225d 5b73 6c69 6365 2834 2c20  ello"][slice(4, 
-00010bc0: 3729 2c20 315d 2c20 5b34 312c 2030 2c20  7), 1], [41, 0, 
-00010bd0: 305d 290a 0a0a 6465 6620 7465 7374 5f68  0])...def test_h
-00010be0: 3570 795f 6368 756e 6b69 6e67 2874 6d70  5py_chunking(tmp
-00010bf0: 5f6c 6f63 616c 5f6e 6574 6364 6629 3a0a  _local_netcdf):.
-00010c00: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
-00010c10: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
-00010c20: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
-00010c30: 2064 733a 0a20 2020 2020 2020 2064 732e   ds:.        ds.
-00010c40: 6469 6d65 6e73 696f 6e73 203d 207b 2278  dimensions = {"x
-00010c50: 223a 2031 302c 2022 7922 3a20 3130 2c20  ": 10, "y": 10, 
-00010c60: 227a 223a 2031 302c 2022 7422 3a20 4e6f  "z": 10, "t": No
-00010c70: 6e65 7d0a 0a20 2020 2020 2020 2076 203d  ne}..        v =
-00010c80: 2064 732e 6372 6561 7465 5f76 6172 6961   ds.create_varia
-00010c90: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00010ca0: 2022 6865 6c6c 6f22 2c20 2822 7822 2c20   "hello", ("x", 
-00010cb0: 2279 222c 2022 7a22 2c20 2274 2229 2c20  "y", "z", "t"), 
-00010cc0: 2266 6c6f 6174 222c 2063 6875 6e6b 696e  "float", chunkin
-00010cd0: 675f 6865 7572 6973 7469 633d 2268 3570  g_heuristic="h5p
-00010ce0: 7922 0a20 2020 2020 2020 2029 0a20 2020  y".        ).   
-00010cf0: 2020 2020 2063 6875 6e6b 735f 6835 7079       chunks_h5py
-00010d00: 203d 2076 2e63 6875 6e6b 730a 0a20 2020   = v.chunks..   
-00010d10: 2020 2020 2064 732e 7265 7369 7a65 5f64       ds.resize_d
-00010d20: 696d 656e 7369 6f6e 2822 7422 2c20 3429  imension("t", 4)
-00010d30: 0a20 2020 2020 2020 2076 203d 2064 732e  .        v = ds.
-00010d40: 6372 6561 7465 5f76 6172 6961 626c 6528  create_variable(
-00010d50: 0a20 2020 2020 2020 2020 2020 2022 6865  .            "he
-00010d60: 6c6c 6f33 222c 2028 2278 222c 2022 7922  llo3", ("x", "y"
-00010d70: 2c20 227a 222c 2022 7422 292c 2022 666c  , "z", "t"), "fl
-00010d80: 6f61 7422 2c20 6368 756e 6b69 6e67 5f68  oat", chunking_h
-00010d90: 6575 7269 7374 6963 3d22 6835 7079 220a  euristic="h5py".
-00010da0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010db0: 2020 6368 756e 6b73 5f72 6573 697a 6564    chunks_resized
-00010dc0: 203d 2076 2e63 6875 6e6b 730a 0a20 2020   = v.chunks..   
-00010dd0: 2023 2063 6173 6573 2061 626f 7665 2073   # cases above s
-00010de0: 686f 756c 6420 6265 2065 7175 6976 616c  hould be equival
-00010df0: 656e 7420 746f 2061 2066 6978 6564 2064  ent to a fixed d
-00010e00: 696d 656e 7369 6f6e 2077 6974 6820 6170  imension with ap
-00010e10: 7072 6f70 7269 6174 6520 7369 7a65 0a20  propriate size. 
-00010e20: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-00010e30: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-00010e40: 6e65 7463 6466 2c20 2277 2229 2061 7320  netcdf, "w") as 
-00010e50: 6473 3a0a 2020 2020 2020 2020 6473 2e64  ds:.        ds.d
-00010e60: 696d 656e 7369 6f6e 7320 3d20 7b22 7822  imensions = {"x"
-00010e70: 3a20 3130 2c20 2279 223a 2031 302c 2022  : 10, "y": 10, "
-00010e80: 7a22 3a20 3130 2c20 2274 223a 2031 3032  z": 10, "t": 102
-00010e90: 347d 0a0a 2020 2020 2020 2020 7620 3d20  4}..        v = 
-00010ea0: 6473 2e63 7265 6174 655f 7661 7269 6162  ds.create_variab
-00010eb0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00010ec0: 2268 656c 6c6f 222c 0a20 2020 2020 2020  "hello",.       
-00010ed0: 2020 2020 2028 2278 222c 2022 7922 2c20       ("x", "y", 
-00010ee0: 227a 222c 2022 7422 292c 0a20 2020 2020  "z", "t"),.     
-00010ef0: 2020 2020 2020 2022 666c 6f61 7422 2c0a         "float",.
-00010f00: 2020 2020 2020 2020 2020 2020 6368 756e              chun
-00010f10: 6b73 3d54 7275 652c 0a20 2020 2020 2020  ks=True,.       
-00010f20: 2020 2020 2063 6875 6e6b 696e 675f 6865       chunking_he
-00010f30: 7572 6973 7469 633d 2268 3570 7922 2c0a  uristic="h5py",.
-00010f40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00010f50: 2020 6368 756e 6b73 5f74 7275 6520 3d20    chunks_true = 
-00010f60: 762e 6368 756e 6b73 0a0a 2020 2020 7769  v.chunks..    wi
-00010f70: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-00010f80: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
-00010f90: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
-00010fa0: 2020 2020 2020 2064 732e 6469 6d65 6e73         ds.dimens
-00010fb0: 696f 6e73 203d 207b 2278 223a 2031 302c  ions = {"x": 10,
-00010fc0: 2022 7922 3a20 3130 2c20 227a 223a 2031   "y": 10, "z": 1
-00010fd0: 302c 2022 7422 3a20 347d 0a0a 2020 2020  0, "t": 4}..    
-00010fe0: 2020 2020 7620 3d20 6473 2e63 7265 6174      v = ds.creat
-00010ff0: 655f 7661 7269 6162 6c65 280a 2020 2020  e_variable(.    
-00011000: 2020 2020 2020 2020 2268 656c 6c6f 222c          "hello",
-00011010: 0a20 2020 2020 2020 2020 2020 2028 2278  .            ("x
-00011020: 222c 2022 7922 2c20 227a 222c 2022 7422  ", "y", "z", "t"
-00011030: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
-00011040: 666c 6f61 7422 2c0a 2020 2020 2020 2020  float",.        
-00011050: 2020 2020 6368 756e 6b73 3d54 7275 652c      chunks=True,
-00011060: 0a20 2020 2020 2020 2020 2020 2063 6875  .            chu
-00011070: 6e6b 696e 675f 6865 7572 6973 7469 633d  nking_heuristic=
-00011080: 2268 3570 7922 2c0a 2020 2020 2020 2020  "h5py",.        
-00011090: 290a 2020 2020 2020 2020 6368 756e 6b73  ).        chunks
-000110a0: 5f74 7275 655f 7265 7369 7a65 6420 3d20  _true_resized = 
-000110b0: 762e 6368 756e 6b73 0a0a 2020 2020 6173  v.chunks..    as
-000110c0: 7365 7274 2063 6875 6e6b 735f 6835 7079  sert chunks_h5py
-000110d0: 203d 3d20 6368 756e 6b73 5f74 7275 650a   == chunks_true.
-000110e0: 2020 2020 6173 7365 7274 2063 6875 6e6b      assert chunk
-000110f0: 735f 7265 7369 7a65 6420 3d3d 2063 6875  s_resized == chu
-00011100: 6e6b 735f 7472 7565 5f72 6573 697a 6564  nks_true_resized
-00011110: 0a0a 0a64 6566 2074 6573 745f 6835 6e65  ...def test_h5ne
-00011120: 7463 6466 5f63 6875 6e6b 696e 6728 746d  tcdf_chunking(tm
-00011130: 705f 6c6f 6361 6c5f 6e65 7463 6466 293a  p_local_netcdf):
-00011140: 0a20 2020 2023 2070 726f 6475 6365 7320  .    # produces 
-00011150: 6d75 6368 2073 6d61 6c6c 6572 2063 6875  much smaller chu
-00011160: 6e6b 7320 666f 7220 756e 7369 7a65 6420  nks for unsized 
-00011170: 6469 6d65 6e73 696f 6e73 0a20 2020 2077  dimensions.    w
-00011180: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-00011190: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-000111a0: 6466 2c20 2277 2229 2061 7320 6473 3a0a  df, "w") as ds:.
-000111b0: 2020 2020 2020 2020 6473 2e64 696d 656e          ds.dimen
-000111c0: 7369 6f6e 7320 3d20 7b22 7822 3a20 3130  sions = {"x": 10
-000111d0: 2c20 2279 223a 2031 302c 2022 7a22 3a20  , "y": 10, "z": 
-000111e0: 3130 2c20 2274 223a 204e 6f6e 657d 0a20  10, "t": None}. 
-000111f0: 2020 2020 2020 2076 203d 2064 732e 6372         v = ds.cr
-00011200: 6561 7465 5f76 6172 6961 626c 6528 0a20  eate_variable(. 
-00011210: 2020 2020 2020 2020 2020 2022 6865 6c6c             "hell
-00011220: 6f22 2c20 2822 7822 2c20 2279 222c 2022  o", ("x", "y", "
-00011230: 7a22 2c20 2274 2229 2c20 2266 6c6f 6174  z", "t"), "float
-00011240: 222c 2063 6875 6e6b 696e 675f 6865 7572  ", chunking_heur
-00011250: 6973 7469 633d 2268 356e 6574 6364 6622  istic="h5netcdf"
-00011260: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00011270: 2020 2063 6875 6e6b 735f 6835 6e65 7463     chunks_h5netc
-00011280: 6466 203d 2076 2e63 6875 6e6b 730a 0a20  df = v.chunks.. 
-00011290: 2020 2061 7373 6572 7420 6368 756e 6b73     assert chunks
-000112a0: 5f68 356e 6574 6364 6620 3d3d 2028 3130  _h5netcdf == (10
-000112b0: 2c20 3130 2c20 3130 2c20 3129 0a0a 2020  , 10, 10, 1)..  
-000112c0: 2020 2320 7368 6f75 6c64 2070 726f 6475    # should produ
-000112d0: 6365 2063 6875 6e6b 7320 3e20 3120 666f  ce chunks > 1 fo
-000112e0: 7220 736d 616c 6c20 6669 7865 6420 6469  r small fixed di
-000112f0: 6d73 0a20 2020 2077 6974 6820 6835 6e65  ms.    with h5ne
-00011300: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
-00011310: 6361 6c5f 6e65 7463 6466 2c20 2277 2229  cal_netcdf, "w")
-00011320: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
-00011330: 6473 2e64 696d 656e 7369 6f6e 7320 3d20  ds.dimensions = 
-00011340: 7b22 7822 3a20 3130 2c20 2274 223a 204e  {"x": 10, "t": N
-00011350: 6f6e 657d 0a20 2020 2020 2020 2076 203d  one}.        v =
-00011360: 2064 732e 6372 6561 7465 5f76 6172 6961   ds.create_varia
-00011370: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
-00011380: 2022 6865 6c6c 6f22 2c20 2822 7822 2c20   "hello", ("x", 
-00011390: 2274 2229 2c20 2266 6c6f 6174 222c 2063  "t"), "float", c
-000113a0: 6875 6e6b 696e 675f 6865 7572 6973 7469  hunking_heuristi
-000113b0: 633d 2268 356e 6574 6364 6622 0a20 2020  c="h5netcdf".   
-000113c0: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-000113d0: 6875 6e6b 735f 6835 6e65 7463 6466 203d  hunks_h5netcdf =
-000113e0: 2076 2e63 6875 6e6b 730a 0a20 2020 2061   v.chunks..    a
-000113f0: 7373 6572 7420 6368 756e 6b73 5f68 356e  ssert chunks_h5n
-00011400: 6574 6364 6620 3d3d 2028 3130 2c20 3132  etcdf == (10, 12
-00011410: 3829 0a0a 2020 2020 2320 7265 7369 7a65  8)..    # resize
-00011420: 6420 756e 6c69 6d69 7465 6420 6469 6d65  d unlimited dime
-00011430: 6e73 696f 6e73 2073 686f 756c 6420 6265  nsions should be
-00011440: 2074 7265 6174 6564 206c 696b 6520 6669   treated like fi
-00011450: 7865 6420 6469 6d73 0a20 2020 2077 6974  xed dims.    wit
-00011460: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00011470: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00011480: 2c20 2277 2229 2061 7320 6473 3a0a 2020  , "w") as ds:.  
-00011490: 2020 2020 2020 6473 2e64 696d 656e 7369        ds.dimensi
-000114a0: 6f6e 7320 3d20 7b22 7822 3a20 3130 2c20  ons = {"x": 10, 
-000114b0: 2279 223a 2031 302c 2022 7a22 3a20 3130  "y": 10, "z": 10
-000114c0: 2c20 2274 223a 204e 6f6e 657d 0a20 2020  , "t": None}.   
-000114d0: 2020 2020 2064 732e 7265 7369 7a65 5f64       ds.resize_d
-000114e0: 696d 656e 7369 6f6e 2822 7422 2c20 3130  imension("t", 10
-000114f0: 290a 2020 2020 2020 2020 7620 3d20 6473  ).        v = ds
-00011500: 2e63 7265 6174 655f 7661 7269 6162 6c65  .create_variable
-00011510: 280a 2020 2020 2020 2020 2020 2020 2268  (.            "h
-00011520: 656c 6c6f 222c 2028 2278 222c 2022 7922  ello", ("x", "y"
-00011530: 2c20 227a 222c 2022 7422 292c 2022 666c  , "z", "t"), "fl
-00011540: 6f61 7422 2c20 6368 756e 6b69 6e67 5f68  oat", chunking_h
-00011550: 6575 7269 7374 6963 3d22 6835 6e65 7463  euristic="h5netc
-00011560: 6466 220a 2020 2020 2020 2020 290a 2020  df".        ).  
-00011570: 2020 2020 2020 6368 756e 6b73 5f68 356e        chunks_h5n
-00011580: 6574 6364 6620 3d20 762e 6368 756e 6b73  etcdf = v.chunks
-00011590: 0a0a 2020 2020 6173 7365 7274 2063 6875  ..    assert chu
-000115a0: 6e6b 735f 6835 6e65 7463 6466 203d 3d20  nks_h5netcdf == 
-000115b0: 2835 2c20 352c 2035 2c20 3130 290a 0a0a  (5, 5, 5, 10)...
-000115c0: 6465 6620 7465 7374 5f63 7265 6174 655f  def test_create_
-000115d0: 696e 7661 6c69 645f 6e65 7463 6466 5f63  invalid_netcdf_c
-000115e0: 6174 6368 5f65 7272 6f72 2874 6d70 5f6c  atch_error(tmp_l
-000115f0: 6f63 616c 5f6e 6574 6364 6629 3a0a 2020  ocal_netcdf):.  
-00011600: 2020 2320 7365 6520 6874 7470 733a 2f2f    # see https://
-00011610: 6769 7468 7562 2e63 6f6d 2f68 356e 6574  github.com/h5net
-00011620: 6364 662f 6835 6e65 7463 6466 2f69 7373  cdf/h5netcdf/iss
-00011630: 7565 732f 3133 380a 2020 2020 7769 7468  ues/138.    with
-00011640: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
-00011650: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-00011660: 2022 7722 2920 6173 2066 3a0a 2020 2020   "w") as f:.    
-00011670: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00011680: 2020 2020 2066 2e63 7265 6174 655f 7661       f.create_va
-00011690: 7269 6162 6c65 2822 7465 7374 222c 2028  riable("test", (
-000116a0: 2278 222c 2022 7922 292c 2064 6174 613d  "x", "y"), data=
-000116b0: 6e70 2e6f 6e65 7328 2831 302c 2031 3029  np.ones((10, 10)
-000116c0: 2c20 6474 7970 653d 2262 6f6f 6c22 2929  , dtype="bool"))
-000116d0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-000116e0: 436f 6d70 6174 6962 696c 6974 7945 7272  CompatibilityErr
-000116f0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00011700: 7061 7373 0a20 2020 2020 2020 2061 7373  pass.        ass
-00011710: 6572 7420 7265 7072 2866 2e64 696d 656e  ert repr(f.dimen
-00011720: 7369 6f6e 7329 203d 3d20 223c 6835 6e65  sions) == "<h5ne
-00011730: 7463 6466 2e44 696d 656e 7369 6f6e 733a  tcdf.Dimensions:
-00011740: 203e 220a 0a0a 6465 6620 7465 7374 5f64   >"...def test_d
-00011750: 696d 656e 7369 6f6e 735f 696e 5f70 6172  imensions_in_par
-00011760: 656e 745f 6772 6f75 7073 2874 6d70 6469  ent_groups(tmpdi
-00011770: 7229 3a0a 2020 2020 7769 7468 206e 6574  r):.    with net
-00011780: 4344 4634 2e44 6174 6173 6574 2874 6d70  CDF4.Dataset(tmp
-00011790: 6469 722e 6a6f 696e 2822 7465 7374 5f6e  dir.join("test_n
-000117a0: 6574 6364 662e 6e63 2229 2c20 6d6f 6465  etcdf.nc"), mode
-000117b0: 3d22 7722 2920 6173 2064 733a 0a20 2020  ="w") as ds:.   
-000117c0: 2020 2020 2064 7330 203d 2064 730a 2020       ds0 = ds.  
-000117d0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-000117e0: 616e 6765 2831 3029 3a0a 2020 2020 2020  ange(10):.      
-000117f0: 2020 2020 2020 6473 203d 2064 732e 6372        ds = ds.cr
-00011800: 6561 7465 4772 6f75 7028 6622 6772 6f75  eateGroup(f"grou
-00011810: 707b 693a 3032 647d 2229 0a20 2020 2020  p{i:02d}").     
-00011820: 2020 2064 7330 2e63 7265 6174 6544 696d     ds0.createDim
-00011830: 656e 7369 6f6e 2822 7822 2c20 3130 290a  ension("x", 10).
-00011840: 2020 2020 2020 2020 6473 302e 6372 6561          ds0.crea
-00011850: 7465 4469 6d65 6e73 696f 6e28 2279 222c  teDimension("y",
-00011860: 2032 3029 0a20 2020 2020 2020 2064 7330   20).        ds0
-00011870: 5b22 6772 6f75 7030 3022 5d2e 6372 6561  ["group00"].crea
-00011880: 7465 5661 7269 6162 6c65 2822 7465 7374  teVariable("test
-00011890: 222c 2066 6c6f 6174 2c20 2822 7822 2c20  ", float, ("x", 
-000118a0: 2279 2229 290a 2020 2020 2020 2020 7661  "y")).        va
-000118b0: 7220 3d20 6473 305b 2267 726f 7570 3030  r = ds0["group00
-000118c0: 225d 2e63 7265 6174 6556 6172 6961 626c  "].createVariabl
-000118d0: 6528 2278 222c 2066 6c6f 6174 2c20 2822  e("x", float, ("
-000118e0: 7822 2c20 2279 2229 290a 2020 2020 2020  x", "y")).      
-000118f0: 2020 7661 725b 3a5d 203d 206e 702e 6f6e    var[:] = np.on
-00011900: 6573 2828 3130 2c20 3230 2929 0a0a 2020  es((10, 20))..  
-00011910: 2020 7769 7468 206c 6567 6163 7961 7069    with legacyapi
-00011920: 2e44 6174 6173 6574 2874 6d70 6469 722e  .Dataset(tmpdir.
-00011930: 6a6f 696e 2822 7465 7374 5f6c 6567 6163  join("test_legac
-00011940: 792e 6e63 2229 2c20 6d6f 6465 3d22 7722  y.nc"), mode="w"
-00011950: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
-00011960: 2064 7330 203d 2064 730a 2020 2020 2020   ds0 = ds.      
-00011970: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00011980: 2831 3029 3a0a 2020 2020 2020 2020 2020  (10):.          
-00011990: 2020 6473 203d 2064 732e 6372 6561 7465    ds = ds.create
-000119a0: 4772 6f75 7028 6622 6772 6f75 707b 693a  Group(f"group{i:
-000119b0: 3032 647d 2229 0a20 2020 2020 2020 2064  02d}").        d
-000119c0: 7330 2e63 7265 6174 6544 696d 656e 7369  s0.createDimensi
-000119d0: 6f6e 2822 7822 2c20 3130 290a 2020 2020  on("x", 10).    
-000119e0: 2020 2020 6473 302e 6372 6561 7465 4469      ds0.createDi
-000119f0: 6d65 6e73 696f 6e28 2279 222c 2032 3029  mension("y", 20)
-00011a00: 0a20 2020 2020 2020 2064 7330 5b22 6772  .        ds0["gr
-00011a10: 6f75 7030 3022 5d2e 6372 6561 7465 5661  oup00"].createVa
-00011a20: 7269 6162 6c65 2822 7465 7374 222c 2066  riable("test", f
-00011a30: 6c6f 6174 2c20 2822 7822 2c20 2279 2229  loat, ("x", "y")
-00011a40: 290a 2020 2020 2020 2020 7661 7220 3d20  ).        var = 
+0000e250: 5b22 6475 6d6d 7933 225d 5b31 3a32 2c20  ["dummy3"][1:2, 
+0000e260: 3a5d 2c20 5b5b 342e 302c 2035 2e30 2c20  :], [[4.0, 5.0, 
+0000e270: 362e 305d 5d29 0a20 2020 2020 2020 2061  6.0]]).        a
+0000e280: 7373 6572 7420 662e 7661 7269 6162 6c65  ssert f.variable
+0000e290: 735b 2264 756d 6d79 3322 5d2e 7368 6170  s["dummy3"].shap
+0000e2a0: 6520 3d3d 2028 332c 2033 290a 2020 2020  e == (3, 3).    
+0000e2b0: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
+0000e2c0: 7373 6572 745f 616c 6c63 6c6f 7365 2866  ssert_allclose(f
+0000e2d0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
+0000e2e0: 7934 225d 5b3a 5d2c 2072 6573 3429 0a20  y4"][:], res4). 
+0000e2f0: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
+0000e300: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
+0000e310: 3422 5d2e 7368 6170 6520 3d3d 2028 332c  4"].shape == (3,
+0000e320: 2033 290a 0a20 2020 2077 6974 6820 6c65   3)..    with le
+0000e330: 6761 6379 6170 692e 4461 7461 7365 7428  gacyapi.Dataset(
+0000e340: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000e350: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+0000e360: 2020 2020 2020 6620 3d20 6473 5b22 7465        f = ds["te
+0000e370: 7374 225d 0a20 2020 2020 2020 206e 702e  st"].        np.
+0000e380: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
+0000e390: 6c6c 636c 6f73 6528 662e 7661 7269 6162  llclose(f.variab
+0000e3a0: 6c65 735b 2264 756d 6d79 3122 5d5b 3a5d  les["dummy1"][:]
+0000e3b0: 2c20 7265 7331 290a 2020 2020 2020 2020  , res1).        
+0000e3c0: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+0000e3d0: 745f 616c 6c63 6c6f 7365 2866 2e76 6172  t_allclose(f.var
+0000e3e0: 6961 626c 6573 5b22 6475 6d6d 7931 225d  iables["dummy1"]
+0000e3f0: 5b31 2c20 3a5d 2c20 5b34 2e30 2c20 352e  [1, :], [4.0, 5.
+0000e400: 302c 2036 2e30 5d29 0a20 2020 2020 2020  0, 6.0]).       
+0000e410: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
+0000e420: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
+0000e430: 7269 6162 6c65 735b 2264 756d 6d79 3122  riables["dummy1"
+0000e440: 5d5b 313a 322c 203a 5d2c 205b 5b34 2e30  ][1:2, :], [[4.0
+0000e450: 2c20 352e 302c 2036 2e30 5d5d 290a 2020  , 5.0, 6.0]]).  
+0000e460: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
+0000e470: 2e61 7373 6572 745f 616c 6c63 6c6f 7365  .assert_allclose
+0000e480: 2866 2e76 6172 6961 626c 6573 5b22 6475  (f.variables["du
+0000e490: 6d6d 7931 225d 2e5f 6835 6473 5b31 2c20  mmy1"]._h5ds[1, 
+0000e4a0: 3a5d 2c20 5b34 2e30 2c20 352e 302c 2036  :], [4.0, 5.0, 6
+0000e4b0: 2e30 5d29 0a20 2020 2020 2020 206e 702e  .0]).        np.
+0000e4c0: 7465 7374 696e 672e 6173 7365 7274 5f61  testing.assert_a
+0000e4d0: 6c6c 636c 6f73 6528 0a20 2020 2020 2020  llclose(.       
+0000e4e0: 2020 2020 2066 2e76 6172 6961 626c 6573       f.variables
+0000e4f0: 5b22 6475 6d6d 7931 225d 2e5f 6835 6473  ["dummy1"]._h5ds
+0000e500: 5b31 3a32 2c20 3a5d 2c20 5b5b 342e 302c  [1:2, :], [[4.0,
+0000e510: 2035 2e30 2c20 362e 305d 5d0a 2020 2020   5.0, 6.0]].    
+0000e520: 2020 2020 290a 2020 2020 2020 2020 6173      ).        as
+0000e530: 7365 7274 2066 2e76 6172 6961 626c 6573  sert f.variables
+0000e540: 5b22 6475 6d6d 7931 225d 2e73 6861 7065  ["dummy1"].shape
+0000e550: 203d 3d20 2833 2c20 3329 0a20 2020 2020   == (3, 3).     
+0000e560: 2020 2061 7373 6572 7420 662e 7661 7269     assert f.vari
+0000e570: 6162 6c65 735b 2264 756d 6d79 3122 5d2e  ables["dummy1"].
+0000e580: 5f68 3564 732e 7368 6170 6520 3d3d 2028  _h5ds.shape == (
+0000e590: 332c 2033 290a 2020 2020 2020 2020 6e70  3, 3).        np
+0000e5a0: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
+0000e5b0: 616c 6c63 6c6f 7365 2866 2e76 6172 6961  allclose(f.varia
+0000e5c0: 626c 6573 5b22 6475 6d6d 7932 225d 5b3a  bles["dummy2"][:
+0000e5d0: 5d2c 2072 6573 3229 0a20 2020 2020 2020  ], res2).       
+0000e5e0: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
+0000e5f0: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
+0000e600: 7269 6162 6c65 735b 2264 756d 6d79 3222  riables["dummy2"
+0000e610: 5d5b 312c 203a 5d2c 205b 342e 302c 2035  ][1, :], [4.0, 5
+0000e620: 2e30 2c20 362e 305d 290a 2020 2020 2020  .0, 6.0]).      
+0000e630: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
+0000e640: 6572 745f 616c 6c63 6c6f 7365 2866 2e76  ert_allclose(f.v
+0000e650: 6172 6961 626c 6573 5b22 6475 6d6d 7932  ariables["dummy2
+0000e660: 225d 5b31 3a32 2c20 3a5d 2c20 5b5b 342e  "][1:2, :], [[4.
+0000e670: 302c 2035 2e30 2c20 362e 305d 5d29 0a20  0, 5.0, 6.0]]). 
+0000e680: 2020 2020 2020 2061 7373 6572 7420 662e         assert f.
+0000e690: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
+0000e6a0: 3222 5d2e 7368 6170 6520 3d3d 2028 332c  2"].shape == (3,
+0000e6b0: 2033 290a 2020 2020 2020 2020 6173 7365   3).        asse
+0000e6c0: 7274 2066 2e76 6172 6961 626c 6573 5b22  rt f.variables["
+0000e6d0: 6475 6d6d 7932 225d 2e5f 6835 6473 2e73  dummy2"]._h5ds.s
+0000e6e0: 6861 7065 203d 3d20 2832 2c20 3329 0a20  hape == (2, 3). 
+0000e6f0: 2020 2020 2020 206e 702e 7465 7374 696e         np.testin
+0000e700: 672e 6173 7365 7274 5f61 6c6c 636c 6f73  g.assert_allclos
+0000e710: 6528 662e 7661 7269 6162 6c65 735b 2264  e(f.variables["d
+0000e720: 756d 6d79 3322 5d5b 3a5d 2c20 7265 7333  ummy3"][:], res3
+0000e730: 290a 2020 2020 2020 2020 6e70 2e74 6573  ).        np.tes
+0000e740: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
+0000e750: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
+0000e760: 5b22 6475 6d6d 7933 225d 5b31 2c20 3a5d  ["dummy3"][1, :]
+0000e770: 2c20 5b34 2e30 2c20 352e 302c 2036 2e30  , [4.0, 5.0, 6.0
+0000e780: 5d29 0a20 2020 2020 2020 206e 702e 7465  ]).        np.te
+0000e790: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
+0000e7a0: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
+0000e7b0: 735b 2264 756d 6d79 3322 5d5b 313a 322c  s["dummy3"][1:2,
+0000e7c0: 203a 5d2c 205b 5b34 2e30 2c20 352e 302c   :], [[4.0, 5.0,
+0000e7d0: 2036 2e30 5d5d 290a 2020 2020 2020 2020   6.0]]).        
+0000e7e0: 6173 7365 7274 2066 2e76 6172 6961 626c  assert f.variabl
+0000e7f0: 6573 5b22 6475 6d6d 7933 225d 2e73 6861  es["dummy3"].sha
+0000e800: 7065 203d 3d20 2833 2c20 3329 0a20 2020  pe == (3, 3).   
+0000e810: 2020 2020 2061 7373 6572 7420 662e 7661       assert f.va
+0000e820: 7269 6162 6c65 735b 2264 756d 6d79 3322  riables["dummy3"
+0000e830: 5d2e 5f68 3564 732e 7368 6170 6520 3d3d  ]._h5ds.shape ==
+0000e840: 2028 322c 2033 290a 2020 2020 2020 2020   (2, 3).        
+0000e850: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+0000e860: 745f 616c 6c63 6c6f 7365 2866 2e76 6172  t_allclose(f.var
+0000e870: 6961 626c 6573 5b22 6475 6d6d 7934 225d  iables["dummy4"]
+0000e880: 5b3a 5d2c 2072 6573 3429 0a20 2020 2020  [:], res4).     
+0000e890: 2020 2061 7373 6572 7420 662e 7661 7269     assert f.vari
+0000e8a0: 6162 6c65 735b 2264 756d 6d79 3422 5d2e  ables["dummy4"].
+0000e8b0: 7368 6170 6520 3d3d 2028 332c 2033 290a  shape == (3, 3).
+0000e8c0: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+0000e8d0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
+0000e8e0: 7934 225d 2e5f 6835 6473 2e73 6861 7065  y4"]._h5ds.shape
+0000e8f0: 203d 3d20 2830 2c20 3329 0a0a 2020 2020   == (0, 3)..    
+0000e900: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+0000e910: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+0000e920: 6364 662c 2022 7222 2920 6173 2064 733a  cdf, "r") as ds:
+0000e930: 0a20 2020 2020 2020 2066 203d 2064 735b  .        f = ds[
+0000e940: 2274 6573 7422 5d0a 2020 2020 2020 2020  "test"].        
+0000e950: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+0000e960: 745f 616c 6c63 6c6f 7365 2866 2e76 6172  t_allclose(f.var
+0000e970: 6961 626c 6573 5b22 6475 6d6d 7931 225d  iables["dummy1"]
+0000e980: 5b3a 5d2c 2072 6573 3129 0a20 2020 2020  [:], res1).     
+0000e990: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
+0000e9a0: 7365 7274 5f61 6c6c 636c 6f73 6528 662e  sert_allclose(f.
+0000e9b0: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
+0000e9c0: 3122 5d5b 3a2c 203a 5d2c 2072 6573 3129  1"][:, :], res1)
+0000e9d0: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
+0000e9e0: 696e 672e 6173 7365 7274 5f61 6c6c 636c  ing.assert_allcl
+0000e9f0: 6f73 6528 662e 7661 7269 6162 6c65 735b  ose(f.variables[
+0000ea00: 2264 756d 6d79 3122 5d5b 312c 203a 5d2c  "dummy1"][1, :],
+0000ea10: 205b 342e 302c 2035 2e30 2c20 362e 305d   [4.0, 5.0, 6.0]
+0000ea20: 290a 2020 2020 2020 2020 6e70 2e74 6573  ).        np.tes
+0000ea30: 7469 6e67 2e61 7373 6572 745f 616c 6c63  ting.assert_allc
+0000ea40: 6c6f 7365 2866 2e76 6172 6961 626c 6573  lose(f.variables
+0000ea50: 5b22 6475 6d6d 7931 225d 5b31 3a32 2c20  ["dummy1"][1:2, 
+0000ea60: 3a5d 2c20 5b5b 342e 302c 2035 2e30 2c20  :], [[4.0, 5.0, 
+0000ea70: 362e 305d 5d29 0a20 2020 2020 2020 2061  6.0]]).        a
+0000ea80: 7373 6572 7420 662e 7661 7269 6162 6c65  ssert f.variable
+0000ea90: 735b 2264 756d 6d79 3122 5d2e 7368 6170  s["dummy1"].shap
+0000eaa0: 6520 3d3d 2028 332c 2033 290a 2020 2020  e == (3, 3).    
+0000eab0: 2020 2020 6173 7365 7274 2066 2e76 6172      assert f.var
+0000eac0: 6961 626c 6573 5b22 6475 6d6d 7931 225d  iables["dummy1"]
+0000ead0: 2e5f 6835 6473 2e73 6861 7065 203d 3d20  ._h5ds.shape == 
+0000eae0: 2833 2c20 3329 0a20 2020 2020 2020 206e  (3, 3).        n
+0000eaf0: 702e 7465 7374 696e 672e 6173 7365 7274  p.testing.assert
+0000eb00: 5f61 6c6c 636c 6f73 6528 662e 7661 7269  _allclose(f.vari
+0000eb10: 6162 6c65 735b 2264 756d 6d79 3222 5d5b  ables["dummy2"][
+0000eb20: 3a5d 2c20 7265 7332 290a 2020 2020 2020  :], res2).      
+0000eb30: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
+0000eb40: 6572 745f 616c 6c63 6c6f 7365 2866 2e76  ert_allclose(f.v
+0000eb50: 6172 6961 626c 6573 5b22 6475 6d6d 7932  ariables["dummy2
+0000eb60: 225d 5b31 2c20 3a5d 2c20 5b34 2e30 2c20  "][1, :], [4.0, 
+0000eb70: 352e 302c 2036 2e30 5d29 0a20 2020 2020  5.0, 6.0]).     
+0000eb80: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
+0000eb90: 7365 7274 5f61 6c6c 636c 6f73 6528 662e  sert_allclose(f.
+0000eba0: 7661 7269 6162 6c65 735b 2264 756d 6d79  variables["dummy
+0000ebb0: 3222 5d5b 313a 322c 203a 5d2c 205b 5b34  2"][1:2, :], [[4
+0000ebc0: 2e30 2c20 352e 302c 2036 2e30 5d5d 290a  .0, 5.0, 6.0]]).
+0000ebd0: 2020 2020 2020 2020 6173 7365 7274 2066          assert f
+0000ebe0: 2e76 6172 6961 626c 6573 5b22 6475 6d6d  .variables["dumm
+0000ebf0: 7932 225d 2e73 6861 7065 203d 3d20 2833  y2"].shape == (3
+0000ec00: 2c20 3329 0a20 2020 2020 2020 2061 7373  , 3).        ass
+0000ec10: 6572 7420 662e 7661 7269 6162 6c65 735b  ert f.variables[
+0000ec20: 2264 756d 6d79 3222 5d2e 5f68 3564 732e  "dummy2"]._h5ds.
+0000ec30: 7368 6170 6520 3d3d 2028 322c 2033 290a  shape == (2, 3).
+0000ec40: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
+0000ec50: 6e67 2e61 7373 6572 745f 616c 6c63 6c6f  ng.assert_allclo
+0000ec60: 7365 2866 2e76 6172 6961 626c 6573 5b22  se(f.variables["
+0000ec70: 6475 6d6d 7933 225d 5b3a 5d2c 2072 6573  dummy3"][:], res
+0000ec80: 3329 0a20 2020 2020 2020 206e 702e 7465  3).        np.te
+0000ec90: 7374 696e 672e 6173 7365 7274 5f61 6c6c  sting.assert_all
+0000eca0: 636c 6f73 6528 662e 7661 7269 6162 6c65  close(f.variable
+0000ecb0: 735b 2264 756d 6d79 3322 5d5b 312c 203a  s["dummy3"][1, :
+0000ecc0: 5d2c 205b 342e 302c 2035 2e30 2c20 362e  ], [4.0, 5.0, 6.
+0000ecd0: 305d 290a 2020 2020 2020 2020 6e70 2e74  0]).        np.t
+0000ece0: 6573 7469 6e67 2e61 7373 6572 745f 616c  esting.assert_al
+0000ecf0: 6c63 6c6f 7365 2866 2e76 6172 6961 626c  lclose(f.variabl
+0000ed00: 6573 5b22 6475 6d6d 7933 225d 5b31 3a32  es["dummy3"][1:2
+0000ed10: 2c20 3a5d 2c20 5b5b 342e 302c 2035 2e30  , :], [[4.0, 5.0
+0000ed20: 2c20 362e 305d 5d29 0a20 2020 2020 2020  , 6.0]]).       
+0000ed30: 2061 7373 6572 7420 662e 7661 7269 6162   assert f.variab
+0000ed40: 6c65 735b 2264 756d 6d79 3322 5d2e 7368  les["dummy3"].sh
+0000ed50: 6170 6520 3d3d 2028 332c 2033 290a 2020  ape == (3, 3).  
+0000ed60: 2020 2020 2020 6173 7365 7274 2066 2e76        assert f.v
+0000ed70: 6172 6961 626c 6573 5b22 6475 6d6d 7933  ariables["dummy3
+0000ed80: 225d 2e5f 6835 6473 2e73 6861 7065 203d  "]._h5ds.shape =
+0000ed90: 3d20 2832 2c20 3329 0a20 2020 2020 2020  = (2, 3).       
+0000eda0: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
+0000edb0: 7274 5f61 6c6c 636c 6f73 6528 662e 7661  rt_allclose(f.va
+0000edc0: 7269 6162 6c65 735b 2264 756d 6d79 3422  riables["dummy4"
+0000edd0: 5d5b 3a5d 2c20 7265 7334 290a 2020 2020  ][:], res4).    
+0000ede0: 2020 2020 6173 7365 7274 2066 2e76 6172      assert f.var
+0000edf0: 6961 626c 6573 5b22 6475 6d6d 7934 225d  iables["dummy4"]
+0000ee00: 2e73 6861 7065 203d 3d20 2833 2c20 3329  .shape == (3, 3)
+0000ee10: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000ee20: 662e 7661 7269 6162 6c65 735b 2264 756d  f.variables["dum
+0000ee30: 6d79 3422 5d2e 5f68 3564 732e 7368 6170  my4"]._h5ds.shap
+0000ee40: 6520 3d3d 2028 302c 2033 290a 0a0a 2320  e == (0, 3)...# 
+0000ee50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000ee60: 6f6d 2f68 356e 6574 6364 662f 6835 6e65  om/h5netcdf/h5ne
+0000ee70: 7463 6466 2f69 7373 7565 732f 3133 360a  tcdf/issues/136.
+0000ee80: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
+0000ee90: 7069 6628 0a20 2020 2076 6572 7369 6f6e  pif(.    version
+0000eea0: 2e70 6172 7365 2868 3570 792e 5f5f 7665  .parse(h5py.__ve
+0000eeb0: 7273 696f 6e5f 5f29 203c 2076 6572 7369  rsion__) < versi
+0000eec0: 6f6e 2e70 6172 7365 2822 332e 372e 3022  on.parse("3.7.0"
+0000eed0: 292c 0a20 2020 2072 6561 736f 6e3d 2268  ),.    reason="h
+0000eee0: 3570 793c 332e 372e 3020 6275 6720 7769  5py<3.7.0 bug wi
+0000eef0: 7468 2074 7261 636b 5f6f 7264 6572 2070  th track_order p
+0000ef00: 7265 7665 6e74 7320 6564 6974 696e 6720  revents editing 
+0000ef10: 7769 7468 206e 6574 4344 4634 222c 0a29  with netCDF4",.)
+0000ef20: 0a64 6566 2074 6573 745f 6372 6561 7469  .def test_creati
+0000ef30: 6f6e 5f77 6974 685f 6835 6e65 7463 6466  on_with_h5netcdf
+0000ef40: 5f65 6469 745f 7769 7468 5f6e 6574 6364  _edit_with_netcd
+0000ef50: 6634 2874 6d70 5f6c 6f63 616c 5f6e 6574  f4(tmp_local_net
+0000ef60: 6364 6629 3a0a 2020 2020 2320 496e 2076  cdf):.    # In v
+0000ef70: 6572 7369 6f6e 2030 2e31 322e 302c 2074  ersion 0.12.0, t
+0000ef80: 6865 2077 726f 6e67 2066 696c 6520 6372  he wrong file cr
+0000ef90: 6561 7469 6f6e 2061 7474 7269 6275 7465  eation attribute
+0000efa0: 7320 7765 7265 2075 7365 640a 2020 2020  s were used.    
+0000efb0: 2320 6d61 6b69 6e67 206e 6574 6364 6634  # making netcdf4
+0000efc0: 2075 6e61 626c 6520 746f 206f 7065 6e20   unable to open 
+0000efd0: 6669 6c65 7320 6372 6561 7465 6420 6279  files created by
+0000efe0: 2068 356e 6574 6364 660a 2020 2020 2320   h5netcdf.    # 
+0000eff0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+0000f000: 6f6d 2f68 356e 6574 6364 662f 6835 6e65  om/h5netcdf/h5ne
+0000f010: 7463 6466 2f69 7373 7565 732f 3132 380a  tcdf/issues/128.
+0000f020: 2020 2020 7769 7468 2068 356e 6574 6364      with h5netcd
+0000f030: 662e 4669 6c65 2874 6d70 5f6c 6f63 616c  f.File(tmp_local
+0000f040: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
+0000f050: 2074 6865 5f66 696c 653a 0a20 2020 2020   the_file:.     
+0000f060: 2020 2074 6865 5f66 696c 652e 6469 6d65     the_file.dime
+0000f070: 6e73 696f 6e73 203d 207b 2278 223a 2035  nsions = {"x": 5
+0000f080: 7d0a 2020 2020 2020 2020 7661 7269 6162  }.        variab
+0000f090: 6c65 203d 2074 6865 5f66 696c 652e 6372  le = the_file.cr
+0000f0a0: 6561 7465 5f76 6172 6961 626c 6528 2268  eate_variable("h
+0000f0b0: 656c 6c6f 222c 2028 2278 222c 292c 2066  ello", ("x",), f
+0000f0c0: 6c6f 6174 290a 2020 2020 2020 2020 7661  loat).        va
+0000f0d0: 7269 6162 6c65 5b2e 2e2e 5d20 3d20 350a  riable[...] = 5.
+0000f0e0: 0a20 2020 2077 6974 6820 6e65 7443 4446  .    with netCDF
+0000f0f0: 342e 4461 7461 7365 7428 746d 705f 6c6f  4.Dataset(tmp_lo
+0000f100: 6361 6c5f 6e65 7463 6466 2c20 6d6f 6465  cal_netcdf, mode
+0000f110: 3d22 6122 2920 6173 2074 6865 5f66 696c  ="a") as the_fil
+0000f120: 653a 0a20 2020 2020 2020 2076 6172 6961  e:.        varia
+0000f130: 626c 6520 3d20 7468 655f 6669 6c65 5b22  ble = the_file["
+0000f140: 6865 6c6c 6f22 5d0a 2020 2020 2020 2020  hello"].        
+0000f150: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+0000f160: 745f 6172 7261 795f 6571 7561 6c28 7661  t_array_equal(va
+0000f170: 7269 6162 6c65 5b2e 2e2e 5d2e 6461 7461  riable[...].data
+0000f180: 2c20 3529 0a20 2020 2020 2020 2023 2045  , 5).        # E
+0000f190: 6469 7420 616e 2065 7869 7374 696e 6720  dit an existing 
+0000f1a0: 7661 7269 6162 6c65 0a20 2020 2020 2020  variable.       
+0000f1b0: 2076 6172 6961 626c 655b 3a33 5d20 3d20   variable[:3] = 
+0000f1c0: 320a 0a20 2020 2020 2020 2023 2043 7265  2..        # Cre
+0000f1d0: 6174 6520 6120 6e65 7720 7661 7269 6162  ate a new variab
+0000f1e0: 6c65 0a20 2020 2020 2020 2076 6172 6961  le.        varia
+0000f1f0: 626c 6520 3d20 7468 655f 6669 6c65 2e63  ble = the_file.c
+0000f200: 7265 6174 6556 6172 6961 626c 6528 2267  reateVariable("g
+0000f210: 6f6f 6462 7965 222c 2066 6c6f 6174 2c20  oodbye", float, 
+0000f220: 2822 7822 2c29 290a 2020 2020 2020 2020  ("x",)).        
+0000f230: 7661 7269 6162 6c65 5b2e 2e2e 5d20 3d20  variable[...] = 
+0000f240: 3130 0a0a 2020 2020 7769 7468 2068 356e  10..    with h5n
+0000f250: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+0000f260: 6f63 616c 5f6e 6574 6364 662c 2022 6122  ocal_netcdf, "a"
+0000f270: 2920 6173 2074 6865 5f66 696c 653a 0a20  ) as the_file:. 
+0000f280: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
+0000f290: 6564 6974 6564 2076 6172 6961 626c 6520  edited variable 
+0000f2a0: 6973 2063 6f6e 7369 7374 656e 7420 7769  is consistent wi
+0000f2b0: 7468 2074 6865 2065 7870 6563 7465 6420  th the expected 
+0000f2c0: 6461 7461 0a20 2020 2020 2020 2076 6172  data.        var
+0000f2d0: 6961 626c 6520 3d20 7468 655f 6669 6c65  iable = the_file
+0000f2e0: 5b22 6865 6c6c 6f22 5d0a 2020 2020 2020  ["hello"].      
+0000f2f0: 2020 6e70 2e74 6573 7469 6e67 2e61 7373    np.testing.ass
+0000f300: 6572 745f 6172 7261 795f 6571 7561 6c28  ert_array_equal(
+0000f310: 7661 7269 6162 6c65 5b2e 2e2e 5d2e 6461  variable[...].da
+0000f320: 7461 2c20 5b32 2c20 322c 2032 2c20 352c  ta, [2, 2, 2, 5,
+0000f330: 2035 5d29 0a0a 2020 2020 2020 2020 2320   5])..        # 
+0000f340: 456e 7375 7265 206e 6577 2076 6172 6961  Ensure new varia
+0000f350: 626c 6520 6973 2061 6363 6573 7369 626c  ble is accessibl
+0000f360: 650a 2020 2020 2020 2020 7661 7269 6162  e.        variab
+0000f370: 6c65 203d 2074 6865 5f66 696c 655b 2267  le = the_file["g
+0000f380: 6f6f 6462 7965 225d 0a20 2020 2020 2020  oodbye"].       
+0000f390: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
+0000f3a0: 7274 5f61 7272 6179 5f65 7175 616c 2876  rt_array_equal(v
+0000f3b0: 6172 6961 626c 655b 2e2e 2e5d 2e64 6174  ariable[...].dat
+0000f3c0: 612c 2031 3029 0a0a 0a64 6566 2074 6573  a, 10)...def tes
+0000f3d0: 745f 7472 6163 6b5f 6f72 6465 725f 7370  t_track_order_sp
+0000f3e0: 6563 6966 6963 6174 696f 6e28 746d 705f  ecification(tmp_
+0000f3f0: 6c6f 6361 6c5f 6e65 7463 6466 293a 0a20  local_netcdf):. 
+0000f400: 2020 2023 2057 6869 6c65 206e 6574 6364     # While netcd
+0000f410: 6634 2d63 2068 6173 2068 6973 746f 7269  f4-c has histori
+0000f420: 6361 6c6c 7920 6f6e 6c79 2061 6c6c 6f77  cally only allow
+0000f430: 6564 2074 7261 636b 5f6f 7264 6572 2074  ed track_order t
+0000f440: 6f20 6265 2054 7275 650a 2020 2020 2320  o be True.    # 
+0000f450: 5468 6572 6520 646f 6573 6e27 7420 7365  There doesn't se
+0000f460: 656d 2074 6f20 6265 2061 2067 6f6f 6420  em to be a good 
+0000f470: 7265 6173 6f6e 2066 6f72 2074 6869 730a  reason for this.
+0000f480: 2020 2020 2320 6874 7470 733a 2f2f 6769      # https://gi
+0000f490: 7468 7562 2e63 6f6d 2f55 6e69 6461 7461  thub.com/Unidata
+0000f4a0: 2f6e 6574 6364 662d 632f 6973 7375 6573  /netcdf-c/issues
+0000f4b0: 2f32 3035 3420 6869 7374 6f72 6963 616c  /2054 historical
+0000f4c0: 6c79 2c20 6835 6e65 7463 6466 0a20 2020  ly, h5netcdf.   
+0000f4d0: 2023 2068 6173 206e 6f74 2073 7065 6369   # has not speci
+0000f4e0: 6669 6564 2074 6869 7320 7061 7261 6d65  fied this parame
+0000f4f0: 7465 7220 286c 6561 7669 6e67 2069 7420  ter (leaving it 
+0000f500: 696d 706c 6963 6974 656c 7920 6173 2046  implicitely as F
+0000f510: 616c 7365 290a 2020 2020 2320 5765 2077  alse).    # We w
+0000f520: 616e 7420 746f 206d 616b 6520 7375 7265  ant to make sure
+0000f530: 2077 6520 616c 6c6f 7720 626f 7468 2068   we allow both h
+0000f540: 6572 650a 2020 2020 7769 7468 2068 356e  ere.    with h5n
+0000f550: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+0000f560: 6f63 616c 5f6e 6574 6364 662c 2022 7722  ocal_netcdf, "w"
+0000f570: 2c20 7472 6163 6b5f 6f72 6465 723d 4661  , track_order=Fa
+0000f580: 6c73 6529 3a0a 2020 2020 2020 2020 7061  lse):.        pa
+0000f590: 7373 0a0a 2020 2020 7769 7468 2068 356e  ss..    with h5n
+0000f5a0: 6574 6364 662e 4669 6c65 2874 6d70 5f6c  etcdf.File(tmp_l
+0000f5b0: 6f63 616c 5f6e 6574 6364 662c 2022 7722  ocal_netcdf, "w"
+0000f5c0: 2c20 7472 6163 6b5f 6f72 6465 723d 5472  , track_order=Tr
+0000f5d0: 7565 293a 0a20 2020 2020 2020 2070 6173  ue):.        pas
+0000f5e0: 730a 0a0a 2320 5468 6973 2073 686f 756c  s...# This shoul
+0000f5f0: 6420 616c 7761 7973 2077 6f72 6b20 7769  d always work wi
+0000f600: 7468 2074 6865 2064 6566 6175 6c74 2066  th the default f
+0000f610: 696c 6520 6f70 656e 696e 6720 7365 7474  ile opening sett
+0000f620: 696e 6773 0a23 2068 7474 7073 3a2f 2f67  ings.# https://g
+0000f630: 6974 6875 622e 636f 6d2f 6835 6e65 7463  ithub.com/h5netc
+0000f640: 6466 2f68 356e 6574 6364 662f 6973 7375  df/h5netcdf/issu
+0000f650: 6573 2f31 3336 2369 7373 7565 636f 6d6d  es/136#issuecomm
+0000f660: 656e 742d 3130 3137 3435 3730 3637 0a64  ent-1017457067.d
+0000f670: 6566 2074 6573 745f 6d6f 7265 5f74 6861  ef test_more_tha
+0000f680: 6e5f 375f 6174 7472 5f63 7265 6174 696f  n_7_attr_creatio
+0000f690: 6e28 746d 705f 6c6f 6361 6c5f 6e65 7463  n(tmp_local_netc
+0000f6a0: 6466 293a 0a20 2020 2077 6974 6820 6835  df):.    with h5
+0000f6b0: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+0000f6c0: 6c6f 6361 6c5f 6e65 7463 6466 2c20 2277  local_netcdf, "w
+0000f6d0: 2229 2061 7320 6835 6669 6c65 3a0a 2020  ") as h5file:.  
+0000f6e0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000f6f0: 616e 6765 2831 3030 293a 0a20 2020 2020  ange(100):.     
+0000f700: 2020 2020 2020 2068 3566 696c 652e 6174         h5file.at
+0000f710: 7472 735b 6622 6b65 797b 697d 225d 203d  trs[f"key{i}"] =
+0000f720: 2069 0a20 2020 2020 2020 2020 2020 2068   i.            h
+0000f730: 3566 696c 652e 6174 7472 735b 6622 6b65  5file.attrs[f"ke
+0000f740: 797b 697d 225d 203d 2030 0a0a 0a23 2041  y{i}"] = 0...# A
+0000f750: 6464 2061 2074 6573 7420 7468 6174 2069  dd a test that i
+0000f760: 7320 7375 7070 6f73 6564 2074 6f20 6661  s supposed to fa
+0000f770: 696c 2069 6e20 7265 6c61 7469 6f6e 2074  il in relation t
+0000f780: 6f20 6973 7375 6520 2331 3336 0a23 2057  o issue #136.# W
+0000f790: 6520 6368 6f6f 7365 2074 6f20 6d6f 6e69  e choose to moni
+0000f7a0: 746f 7220 7768 656e 2068 3570 7920 7769  tor when h5py wi
+0000f7b0: 6c6c 2068 6176 6520 6669 7865 6420 7468  ll have fixed th
+0000f7c0: 6569 7220 6973 7375 6520 696e 206f 7572  eir issue in our
+0000f7d0: 2074 6573 7420 7375 6974 650a 2320 746f   test suite.# to
+0000f7e0: 2065 6e68 616e 6365 206d 6169 6e74 6169   enhance maintai
+0000f7f0: 6e61 6269 6c69 7479 0a23 2068 7474 7073  nability.# https
+0000f800: 3a2f 2f67 6974 6875 622e 636f 6d2f 6835  ://github.com/h5
+0000f810: 6e65 7463 6466 2f68 356e 6574 6364 662f  netcdf/h5netcdf/
+0000f820: 6973 7375 6573 2f31 3336 2369 7373 7565  issues/136#issue
+0000f830: 636f 6d6d 656e 742d 3130 3137 3435 3730  comment-10174570
+0000f840: 3637 0a40 7079 7465 7374 2e6d 6172 6b2e  67.@pytest.mark.
+0000f850: 7061 7261 6d65 7472 697a 6528 2274 7261  parametrize("tra
+0000f860: 636b 5f6f 7264 6572 222c 205b 4661 6c73  ck_order", [Fals
+0000f870: 652c 2054 7275 655d 290a 6465 6620 7465  e, True]).def te
+0000f880: 7374 5f6d 6f72 655f 7468 616e 5f37 5f61  st_more_than_7_a
+0000f890: 7474 725f 6372 6561 7469 6f6e 5f74 7261  ttr_creation_tra
+0000f8a0: 636b 5f6f 7264 6572 2874 6d70 5f6c 6f63  ck_order(tmp_loc
+0000f8b0: 616c 5f6e 6574 6364 662c 2074 7261 636b  al_netcdf, track
+0000f8c0: 5f6f 7264 6572 293a 0a20 2020 2068 3570  _order):.    h5p
+0000f8d0: 795f 7665 7273 696f 6e20 3d20 7665 7273  y_version = vers
+0000f8e0: 696f 6e2e 7061 7273 6528 6835 7079 2e5f  ion.parse(h5py._
+0000f8f0: 5f76 6572 7369 6f6e 5f5f 290a 2020 2020  _version__).    
+0000f900: 6966 2074 7261 636b 5f6f 7264 6572 2061  if track_order a
+0000f910: 6e64 2068 3570 795f 7665 7273 696f 6e20  nd h5py_version 
+0000f920: 3c20 7665 7273 696f 6e2e 7061 7273 6528  < version.parse(
+0000f930: 2233 2e37 2e30 2229 3a0a 2020 2020 2020  "3.7.0"):.      
+0000f940: 2020 6578 7065 6374 6564 5f65 7272 6f72    expected_error
+0000f950: 7320 3d20 7079 7465 7374 2e72 6169 7365  s = pytest.raise
+0000f960: 7328 4b65 7945 7272 6f72 290a 2020 2020  s(KeyError).    
+0000f970: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+0000f980: 5765 2064 6f6e 2774 2065 7870 6563 7420  We don't expect 
+0000f990: 616e 7920 6572 726f 7273 2e20 5468 6973  any errors. This
+0000f9a0: 2069 7320 6566 6665 6374 6976 656c 7920   is effectively 
+0000f9b0: 6120 766f 6964 2063 6f6e 7465 7874 206d  a void context m
+0000f9c0: 616e 6167 6572 0a20 2020 2020 2020 2065  anager.        e
+0000f9d0: 7870 6563 7465 645f 6572 726f 7273 203d  xpected_errors =
+0000f9e0: 206d 656d 6f72 7976 6965 7728 6222 2229   memoryview(b"")
+0000f9f0: 0a0a 2020 2020 7769 7468 2068 356e 6574  ..    with h5net
+0000fa00: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
+0000fa10: 616c 5f6e 6574 6364 662c 2022 7722 2c20  al_netcdf, "w", 
+0000fa20: 7472 6163 6b5f 6f72 6465 723d 7472 6163  track_order=trac
+0000fa30: 6b5f 6f72 6465 7229 2061 7320 6835 6669  k_order) as h5fi
+0000fa40: 6c65 3a0a 2020 2020 2020 2020 7769 7468  le:.        with
+0000fa50: 2065 7870 6563 7465 645f 6572 726f 7273   expected_errors
+0000fa60: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0000fa70: 7220 6920 696e 2072 616e 6765 2831 3030  r i in range(100
+0000fa80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000fa90: 2020 2068 3566 696c 652e 6174 7472 735b     h5file.attrs[
+0000faa0: 6622 6b65 797b 697d 225d 203d 2069 0a20  f"key{i}"] = i. 
+0000fab0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+0000fac0: 3566 696c 652e 6174 7472 735b 6622 6b65  5file.attrs[f"ke
+0000fad0: 797b 697d 225d 203d 2030 0a0a 0a64 6566  y{i}"] = 0...def
+0000fae0: 2074 6573 745f 6772 6f75 705f 6e61 6d65   test_group_name
+0000faf0: 7328 746d 705f 6c6f 6361 6c5f 6e65 7463  s(tmp_local_netc
+0000fb00: 6466 293a 0a20 2020 2023 2068 7474 7073  df):.    # https
+0000fb10: 3a2f 2f67 6974 6875 622e 636f 6d2f 6835  ://github.com/h5
+0000fb20: 6e65 7463 6466 2f68 356e 6574 6364 662f  netcdf/h5netcdf/
+0000fb30: 6973 7375 6573 2f36 380a 2020 2020 7769  issues/68.    wi
+0000fb40: 7468 206e 6574 4344 4634 2e44 6174 6173  th netCDF4.Datas
+0000fb50: 6574 2874 6d70 5f6c 6f63 616c 5f6e 6574  et(tmp_local_net
+0000fb60: 6364 662c 206d 6f64 653d 2277 2229 2061  cdf, mode="w") a
+0000fb70: 7320 6473 3a0a 2020 2020 2020 2020 666f  s ds:.        fo
+0000fb80: 7220 6920 696e 2072 616e 6765 2831 3029  r i in range(10)
+0000fb90: 3a0a 2020 2020 2020 2020 2020 2020 6473  :.            ds
+0000fba0: 203d 2064 732e 6372 6561 7465 4772 6f75   = ds.createGrou
+0000fbb0: 7028 6622 6772 6f75 707b 693a 3032 647d  p(f"group{i:02d}
+0000fbc0: 2229 0a0a 2020 2020 7769 7468 206e 6574  ")..    with net
+0000fbd0: 4344 4634 2e44 6174 6173 6574 2874 6d70  CDF4.Dataset(tmp
+0000fbe0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
+0000fbf0: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
+0000fc00: 2020 2061 7373 6572 7420 6473 2e6e 616d     assert ds.nam
+0000fc10: 6520 3d3d 2022 2f22 0a20 2020 2020 2020  e == "/".       
+0000fc20: 206e 616d 6520 3d20 2222 0a20 2020 2020   name = "".     
+0000fc30: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0000fc40: 6528 3130 293a 0a20 2020 2020 2020 2020  e(10):.         
+0000fc50: 2020 206e 616d 6520 3d20 222f 222e 6a6f     name = "/".jo
+0000fc60: 696e 285b 6e61 6d65 2c20 6622 6772 6f75  in([name, f"grou
+0000fc70: 707b 693a 3032 647d 225d 290a 2020 2020  p{i:02d}"]).    
+0000fc80: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+0000fc90: 735b 6e61 6d65 5d2e 6e61 6d65 203d 3d20  s[name].name == 
+0000fca0: 6e61 6d65 2e73 706c 6974 2822 2f22 295b  name.split("/")[
+0000fcb0: 2d31 5d0a 0a20 2020 2077 6974 6820 6c65  -1]..    with le
+0000fcc0: 6761 6379 6170 692e 4461 7461 7365 7428  gacyapi.Dataset(
+0000fcd0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+0000fce0: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+0000fcf0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+0000fd00: 6e61 6d65 203d 3d20 222f 220a 2020 2020  name == "/".    
+0000fd10: 2020 2020 6e61 6d65 203d 2022 220a 2020      name = "".  
+0000fd20: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000fd30: 616e 6765 2831 3029 3a0a 2020 2020 2020  ange(10):.      
+0000fd40: 2020 2020 2020 6e61 6d65 203d 2022 2f22        name = "/"
+0000fd50: 2e6a 6f69 6e28 5b6e 616d 652c 2066 2267  .join([name, f"g
+0000fd60: 726f 7570 7b69 3a30 3264 7d22 5d29 0a20  roup{i:02d}"]). 
+0000fd70: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000fd80: 7420 6473 5b6e 616d 655d 2e6e 616d 6520  t ds[name].name 
+0000fd90: 3d3d 206e 616d 652e 7370 6c69 7428 222f  == name.split("/
+0000fda0: 2229 5b2d 315d 0a0a 2020 2020 7769 7468  ")[-1]..    with
+0000fdb0: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
+0000fdc0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+0000fdd0: 2022 7222 2920 6173 2064 733a 0a20 2020   "r") as ds:.   
+0000fde0: 2020 2020 2061 7373 6572 7420 6473 2e6e       assert ds.n
+0000fdf0: 616d 6520 3d3d 2022 2f22 0a20 2020 2020  ame == "/".     
+0000fe00: 2020 206e 616d 6520 3d20 2222 0a20 2020     name = "".   
+0000fe10: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+0000fe20: 6e67 6528 3130 293a 0a20 2020 2020 2020  nge(10):.       
+0000fe30: 2020 2020 206e 616d 6520 3d20 222f 222e       name = "/".
+0000fe40: 6a6f 696e 285b 6e61 6d65 2c20 6622 6772  join([name, f"gr
+0000fe50: 6f75 707b 693a 3032 647d 225d 290a 2020  oup{i:02d}"]).  
+0000fe60: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+0000fe70: 2064 735b 6e61 6d65 5d2e 6e61 6d65 203d   ds[name].name =
+0000fe80: 3d20 6e61 6d65 0a0a 0a64 6566 2074 6573  = name...def tes
+0000fe90: 745f 6c65 6761 6379 6170 695f 656e 6469  t_legacyapi_endi
+0000fea0: 616e 6573 7328 746d 705f 6c6f 6361 6c5f  aness(tmp_local_
+0000feb0: 6e65 7463 6466 293a 0a20 2020 2023 2068  netcdf):.    # h
+0000fec0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000fed0: 6d2f 6835 6e65 7463 6466 2f68 356e 6574  m/h5netcdf/h5net
+0000fee0: 6364 662f 6973 7375 6573 2f31 350a 2020  cdf/issues/15.  
+0000fef0: 2020 6269 6720 3d20 6c65 6761 6379 6170    big = legacyap
+0000ff00: 692e 5f63 6865 636b 5f72 6574 7572 6e5f  i._check_return_
+0000ff10: 6474 7970 655f 656e 6469 616e 6573 7328  dtype_endianess(
+0000ff20: 2262 6967 2229 0a20 2020 206c 6974 746c  "big").    littl
+0000ff30: 6520 3d20 6c65 6761 6379 6170 692e 5f63  e = legacyapi._c
+0000ff40: 6865 636b 5f72 6574 7572 6e5f 6474 7970  heck_return_dtyp
+0000ff50: 655f 656e 6469 616e 6573 7328 226c 6974  e_endianess("lit
+0000ff60: 746c 6522 290a 2020 2020 6e61 7469 7665  tle").    native
+0000ff70: 203d 206c 6567 6163 7961 7069 2e5f 6368   = legacyapi._ch
+0000ff80: 6563 6b5f 7265 7475 726e 5f64 7479 7065  eck_return_dtype
+0000ff90: 5f65 6e64 6961 6e65 7373 2822 6e61 7469  _endianess("nati
+0000ffa0: 7665 2229 0a0a 2020 2020 7769 7468 206c  ve")..    with l
+0000ffb0: 6567 6163 7961 7069 2e44 6174 6173 6574  egacyapi.Dataset
+0000ffc0: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+0000ffd0: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
+0000ffe0: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+0000fff0: 4469 6d65 6e73 696f 6e28 2278 222c 2034  Dimension("x", 4
+00010000: 290a 2020 2020 2020 2020 2320 7465 7374  ).        # test
+00010010: 2063 7265 6174 696e 6720 7661 7269 6162   creating variab
+00010020: 6c65 2075 7369 6e67 2065 6e64 6961 6e20  le using endian 
+00010030: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00010040: 0a20 2020 2020 2020 2076 203d 2064 732e  .        v = ds.
+00010050: 6372 6561 7465 5661 7269 6162 6c65 2822  createVariable("
+00010060: 6269 6722 2c20 696e 742c 2028 2278 2229  big", int, ("x")
+00010070: 2c20 656e 6469 616e 3d22 6269 6722 290a  , endian="big").
+00010080: 2020 2020 2020 2020 765b 2e2e 2e5d 203d          v[...] =
+00010090: 2036 3535 3333 0a20 2020 2020 2020 2076   65533.        v
+000100a0: 203d 2064 732e 6372 6561 7465 5661 7269   = ds.createVari
+000100b0: 6162 6c65 2822 6c69 7474 6c65 222c 2069  able("little", i
+000100c0: 6e74 2c20 2822 7822 292c 2065 6e64 6961  nt, ("x"), endia
+000100d0: 6e3d 226c 6974 746c 6522 290a 2020 2020  n="little").    
+000100e0: 2020 2020 765b 2e2e 2e5d 203d 2036 3535      v[...] = 655
+000100f0: 3333 0a20 2020 2020 2020 2076 203d 2064  33.        v = d
+00010100: 732e 6372 6561 7465 5661 7269 6162 6c65  s.createVariable
+00010110: 2822 6e61 7469 7665 222c 2069 6e74 2c20  ("native", int, 
+00010120: 2822 7822 292c 2065 6e64 6961 6e3d 226e  ("x"), endian="n
+00010130: 6174 6976 6522 290a 2020 2020 2020 2020  ative").        
+00010140: 765b 2e2e 2e5d 203d 2036 3535 3335 0a0a  v[...] = 65535..
+00010150: 2020 2020 7769 7468 2068 3570 792e 4669      with h5py.Fi
+00010160: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+00010170: 6364 662c 2022 7222 2920 6173 2064 733a  cdf, "r") as ds:
+00010180: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00010190: 6473 5b22 6269 6722 5d2e 6474 7970 652e  ds["big"].dtype.
+000101a0: 6279 7465 6f72 6465 7220 3d3d 2062 6967  byteorder == big
+000101b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000101c0: 6473 5b22 6c69 7474 6c65 225d 2e64 7479  ds["little"].dty
+000101d0: 7065 2e62 7974 656f 7264 6572 203d 3d20  pe.byteorder == 
+000101e0: 6c69 7474 6c65 0a20 2020 2020 2020 2061  little.        a
+000101f0: 7373 6572 7420 6473 5b22 6e61 7469 7665  ssert ds["native
+00010200: 225d 2e64 7479 7065 2e62 7974 656f 7264  "].dtype.byteord
+00010210: 6572 203d 3d20 6e61 7469 7665 0a0a 2020  er == native..  
+00010220: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+00010230: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
+00010240: 6574 6364 662c 2022 7222 2920 6173 2064  etcdf, "r") as d
+00010250: 733a 0a20 2020 2020 2020 2061 7373 6572  s:.        asser
+00010260: 7420 6473 5b22 6269 6722 5d2e 6474 7970  t ds["big"].dtyp
+00010270: 652e 6279 7465 6f72 6465 7220 3d3d 2062  e.byteorder == b
+00010280: 6967 0a20 2020 2020 2020 2061 7373 6572  ig.        asser
+00010290: 7420 6473 5b22 6c69 7474 6c65 225d 2e64  t ds["little"].d
+000102a0: 7479 7065 2e62 7974 656f 7264 6572 203d  type.byteorder =
+000102b0: 3d20 6c69 7474 6c65 0a20 2020 2020 2020  = little.       
+000102c0: 2061 7373 6572 7420 6473 5b22 6e61 7469   assert ds["nati
+000102d0: 7665 225d 2e64 7479 7065 2e62 7974 656f  ve"].dtype.byteo
+000102e0: 7264 6572 203d 3d20 6e61 7469 7665 0a0a  rder == native..
+000102f0: 2020 2020 7769 7468 206c 6567 6163 7961      with legacya
+00010300: 7069 2e44 6174 6173 6574 2874 6d70 5f6c  pi.Dataset(tmp_l
+00010310: 6f63 616c 5f6e 6574 6364 662c 2022 7222  ocal_netcdf, "r"
+00010320: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
+00010330: 2061 7373 6572 7420 6473 5b22 6269 6722   assert ds["big"
+00010340: 5d2e 6474 7970 652e 6279 7465 6f72 6465  ].dtype.byteorde
+00010350: 7220 3d3d 2062 6967 0a20 2020 2020 2020  r == big.       
+00010360: 2061 7373 6572 7420 6473 5b22 6c69 7474   assert ds["litt
+00010370: 6c65 225d 2e64 7479 7065 2e62 7974 656f  le"].dtype.byteo
+00010380: 7264 6572 203d 3d20 6c69 7474 6c65 0a20  rder == little. 
+00010390: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+000103a0: 5b22 6e61 7469 7665 225d 2e64 7479 7065  ["native"].dtype
+000103b0: 2e62 7974 656f 7264 6572 203d 3d20 6e61  .byteorder == na
+000103c0: 7469 7665 0a0a 2020 2020 7769 7468 206e  tive..    with n
+000103d0: 6574 4344 4634 2e44 6174 6173 6574 2874  etCDF4.Dataset(t
+000103e0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+000103f0: 2022 7222 2920 6173 2064 733a 0a20 2020   "r") as ds:.   
+00010400: 2020 2020 2061 7373 6572 7420 6473 5b22       assert ds["
+00010410: 6269 6722 5d2e 6474 7970 652e 6279 7465  big"].dtype.byte
+00010420: 6f72 6465 7220 3d3d 2062 6967 0a20 2020  order == big.   
+00010430: 2020 2020 2061 7373 6572 7420 6473 5b22       assert ds["
+00010440: 6c69 7474 6c65 225d 2e64 7479 7065 2e62  little"].dtype.b
+00010450: 7974 656f 7264 6572 203d 3d20 6c69 7474  yteorder == litt
+00010460: 6c65 0a20 2020 2020 2020 2061 7373 6572  le.        asser
+00010470: 7420 6473 5b22 6e61 7469 7665 225d 2e64  t ds["native"].d
+00010480: 7479 7065 2e62 7974 656f 7264 6572 203d  type.byteorder =
+00010490: 3d20 6e61 7469 7665 0a0a 0a64 6566 2074  = native...def t
+000104a0: 6573 745f 626f 6f6c 5f73 6c69 6369 6e67  est_bool_slicing
+000104b0: 5f6c 656e 6774 685f 6f6e 655f 6469 6d28  _length_one_dim(
+000104c0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+000104d0: 293a 0a20 2020 2023 2073 6565 2068 7474  ):.    # see htt
+000104e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000104f0: 6835 6e65 7463 6466 2f68 356e 6574 6364  h5netcdf/h5netcd
+00010500: 662f 6973 7375 6573 2f32 330a 2020 2020  f/issues/23.    
+00010510: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+00010520: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+00010530: 6364 662c 2022 7722 2920 6173 2064 733a  cdf, "w") as ds:
+00010540: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
+00010550: 6e73 696f 6e73 203d 207b 2278 223a 2031  nsions = {"x": 1
+00010560: 2c20 2279 223a 2032 7d0a 2020 2020 2020  , "y": 2}.      
+00010570: 2020 7620 3d20 6473 2e63 7265 6174 655f    v = ds.create_
+00010580: 7661 7269 6162 6c65 2822 6865 6c6c 6f22  variable("hello"
+00010590: 2c20 2822 7822 2c20 2279 2229 2c20 2266  , ("x", "y"), "f
+000105a0: 6c6f 6174 2229 0a20 2020 2020 2020 2076  loat").        v
+000105b0: 5b3a 5d20 3d20 6e70 2e6f 6e65 7328 2831  [:] = np.ones((1
+000105c0: 2c20 3229 290a 0a20 2020 2062 6f6f 6c5f  , 2))..    bool_
+000105d0: 736c 6963 6520 3d20 6e70 2e61 7272 6179  slice = np.array
+000105e0: 285b 315d 2c20 6474 7970 653d 626f 6f6c  ([1], dtype=bool
+000105f0: 290a 0a20 2020 2023 2077 6f72 6b73 2066  )..    # works f
+00010600: 6f72 206c 6567 6163 7920 4150 490a 2020  or legacy API.  
+00010610: 2020 7769 7468 206c 6567 6163 7961 7069    with legacyapi
+00010620: 2e44 6174 6173 6574 2874 6d70 5f6c 6f63  .Dataset(tmp_loc
+00010630: 616c 5f6e 6574 6364 662c 2022 6122 2920  al_netcdf, "a") 
+00010640: 6173 2064 733a 0a20 2020 2020 2020 2064  as ds:.        d
+00010650: 6174 6120 3d20 6473 5b22 6865 6c6c 6f22  ata = ds["hello"
+00010660: 5d5b 626f 6f6c 5f73 6c69 6365 2c20 3a5d  ][bool_slice, :]
+00010670: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
+00010680: 696e 672e 6173 7365 7274 5f65 7175 616c  ing.assert_equal
+00010690: 2864 6174 612c 206e 702e 6f6e 6573 2828  (data, np.ones((
+000106a0: 312c 2032 2929 290a 2020 2020 2020 2020  1, 2))).        
+000106b0: 6473 5b22 6865 6c6c 6f22 5d5b 626f 6f6c  ds["hello"][bool
+000106c0: 5f73 6c69 6365 2c20 3a5d 203d 206e 702e  _slice, :] = np.
+000106d0: 7a65 726f 7328 2831 2c20 3229 290a 2020  zeros((1, 2)).  
+000106e0: 2020 2020 2020 6461 7461 203d 2064 735b        data = ds[
+000106f0: 2268 656c 6c6f 225d 5b62 6f6f 6c5f 736c  "hello"][bool_sl
+00010700: 6963 652c 203a 5d0a 2020 2020 2020 2020  ice, :].        
+00010710: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+00010720: 745f 6571 7561 6c28 6461 7461 2c20 6e70  t_equal(data, np
+00010730: 2e7a 6572 6f73 2828 312c 2032 2929 290a  .zeros((1, 2))).
+00010740: 0a20 2020 2023 2073 686f 756c 6420 7261  .    # should ra
+00010750: 6973 6520 666f 7220 6835 7079 203e 3d20  ise for h5py >= 
+00010760: 332e 302e 3020 616e 6420 6835 7079 203c  3.0.0 and h5py <
+00010770: 2033 2e37 2e30 0a20 2020 2023 2068 7474   3.7.0.    # htt
+00010780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00010790: 6835 7079 2f68 3570 792f 7075 6c6c 2f32  h5py/h5py/pull/2
+000107a0: 3037 390a 2020 2020 2320 6874 7470 733a  079.    # https:
+000107b0: 2f2f 6769 7468 7562 2e63 6f6d 2f68 356e  //github.com/h5n
+000107c0: 6574 6364 662f 6835 6e65 7463 6466 2f70  etcdf/h5netcdf/p
+000107d0: 756c 6c2f 3132 352f 0a20 2020 2077 6974  ull/125/.    wit
+000107e0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+000107f0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+00010800: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
+00010810: 2020 2020 2020 6835 7079 5f76 6572 7369        h5py_versi
+00010820: 6f6e 203d 2076 6572 7369 6f6e 2e70 6172  on = version.par
+00010830: 7365 2868 3570 792e 5f5f 7665 7273 696f  se(h5py.__versio
+00010840: 6e5f 5f29 0a20 2020 2020 2020 2069 6620  n__).        if 
+00010850: 7665 7273 696f 6e2e 7061 7273 6528 2233  version.parse("3
+00010860: 2e30 2e30 2229 203c 3d20 6835 7079 5f76  .0.0") <= h5py_v
+00010870: 6572 7369 6f6e 203c 2076 6572 7369 6f6e  ersion < version
+00010880: 2e70 6172 7365 2822 332e 372e 3022 293a  .parse("3.7.0"):
+00010890: 0a20 2020 2020 2020 2020 2020 2065 7272  .            err
+000108a0: 6f72 203d 2022 496e 6465 7869 6e67 2061  or = "Indexing a
+000108b0: 7272 6179 7320 6d75 7374 2068 6176 6520  rrays must have 
+000108c0: 696e 7465 6765 7220 6474 7970 6573 220a  integer dtypes".
+000108d0: 2020 2020 2020 2020 2020 2020 7769 7468              with
+000108e0: 2070 7974 6573 742e 7261 6973 6573 2854   pytest.raises(T
+000108f0: 7970 6545 7272 6f72 2920 6173 2065 3a0a  ypeError) as e:.
+00010900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010910: 6473 5b22 6865 6c6c 6f22 5d5b 626f 6f6c  ds["hello"][bool
+00010920: 5f73 6c69 6365 2c20 3a5d 0a20 2020 2020  _slice, :].     
+00010930: 2020 2020 2020 2061 7373 6572 7420 6572         assert er
+00010940: 726f 7220 3d3d 2073 7472 2865 2e76 616c  ror == str(e.val
+00010950: 7565 290a 2020 2020 2020 2020 656c 7365  ue).        else
+00010960: 3a0a 2020 2020 2020 2020 2020 2020 6473  :.            ds
+00010970: 5b22 6865 6c6c 6f22 5d5b 626f 6f6c 5f73  ["hello"][bool_s
+00010980: 6c69 6365 2c20 3a5d 0a0a 0a64 6566 2074  lice, :]...def t
+00010990: 6573 745f 6661 6e63 795f 696e 6465 7869  est_fancy_indexi
+000109a0: 6e67 2874 6d70 5f6c 6f63 616c 5f6e 6574  ng(tmp_local_net
+000109b0: 6364 6629 3a0a 2020 2020 2320 7265 6772  cdf):.    # regr
+000109c0: 6573 7369 6f6e 2074 6573 7420 666f 7220  ession test for 
+000109d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000109e0: 6f6d 2f70 7964 6174 612f 7861 7272 6179  om/pydata/xarray
+000109f0: 2f69 7373 7565 732f 3731 3534 0a20 2020  /issues/7154.   
+00010a00: 2077 6974 6820 6835 6e65 7463 6466 2e6c   with h5netcdf.l
+00010a10: 6567 6163 7961 7069 2e44 6174 6173 6574  egacyapi.Dataset
+00010a20: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+00010a30: 662c 2022 7722 2920 6173 2064 733a 0a20  f, "w") as ds:. 
+00010a40: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
+00010a50: 4469 6d65 6e73 696f 6e28 2278 222c 204e  Dimension("x", N
+00010a60: 6f6e 6529 0a20 2020 2020 2020 2064 732e  one).        ds.
+00010a70: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+00010a80: 2279 222c 204e 6f6e 6529 0a20 2020 2020  "y", None).     
+00010a90: 2020 2064 732e 6372 6561 7465 5661 7269     ds.createVari
+00010aa0: 6162 6c65 2822 6865 6c6c 6f22 2c20 696e  able("hello", in
+00010ab0: 742c 2028 2278 222c 2022 7922 292c 2066  t, ("x", "y"), f
+00010ac0: 696c 6c5f 7661 6c75 653d 3029 0a20 2020  ill_value=0).   
+00010ad0: 2020 2020 2064 735b 2268 656c 6c6f 225d       ds["hello"]
+00010ae0: 5b3a 352c 203a 3130 5d20 3d20 6e70 2e61  [:5, :10] = np.a
+00010af0: 7261 6e67 6528 3520 2a20 3130 2c20 6474  range(5 * 10, dt
+00010b00: 7970 653d 2269 6e74 2229 2e72 6573 6861  ype="int").resha
+00010b10: 7065 2828 352c 2031 3029 290a 2020 2020  pe((5, 10)).    
+00010b20: 2020 2020 6473 2e63 7265 6174 6556 6172      ds.createVar
+00010b30: 6961 626c 6528 2268 656c 6c6f 3222 2c20  iable("hello2", 
+00010b40: 696e 742c 2028 2278 222c 2022 7922 2929  int, ("x", "y"))
+00010b50: 0a20 2020 2020 2020 2064 735b 2268 656c  .        ds["hel
+00010b60: 6c6f 3222 5d5b 3a31 302c 203a 3230 5d20  lo2"][:10, :20] 
+00010b70: 3d20 6e70 2e61 7261 6e67 6528 3130 202a  = np.arange(10 *
+00010b80: 2032 302c 2064 7479 7065 3d22 696e 7422   20, dtype="int"
+00010b90: 292e 7265 7368 6170 6528 2831 302c 2032  ).reshape((10, 2
+00010ba0: 3029 290a 0a20 2020 2077 6974 6820 6c65  0))..    with le
+00010bb0: 6761 6379 6170 692e 4461 7461 7365 7428  gacyapi.Dataset(
+00010bc0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+00010bd0: 2c20 2261 2229 2061 7320 6473 3a0a 2020  , "a") as ds:.  
+00010be0: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
+00010bf0: 2e61 7373 6572 745f 6172 7261 795f 6571  .assert_array_eq
+00010c00: 7561 6c28 6473 5b22 6865 6c6c 6f22 5d5b  ual(ds["hello"][
+00010c10: 312c 205b 372c 2038 2c20 395d 5d2c 205b  1, [7, 8, 9]], [
+00010c20: 3137 2c20 3138 2c20 3139 5d29 0a20 2020  17, 18, 19]).   
+00010c30: 2020 2020 206e 702e 7465 7374 696e 672e       np.testing.
+00010c40: 6173 7365 7274 5f61 7272 6179 5f65 7175  assert_array_equ
+00010c50: 616c 2864 735b 2268 656c 6c6f 225d 5b31  al(ds["hello"][1
+00010c60: 2c20 5b39 2c20 3130 2c20 3131 5d5d 2c20  , [9, 10, 11]], 
+00010c70: 5b31 392c 2030 2c20 305d 290a 2020 2020  [19, 0, 0]).    
+00010c80: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
+00010c90: 7373 6572 745f 6172 7261 795f 6571 7561  ssert_array_equa
+00010ca0: 6c28 6473 5b22 6865 6c6c 6f22 5d5b 312c  l(ds["hello"][1,
+00010cb0: 2073 6c69 6365 2839 2c20 3132 295d 2c20   slice(9, 12)], 
+00010cc0: 5b31 392c 2030 2c20 305d 290a 2020 2020  [19, 0, 0]).    
+00010cd0: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
+00010ce0: 7373 6572 745f 6172 7261 795f 6571 7561  ssert_array_equa
+00010cf0: 6c28 6473 5b22 6865 6c6c 6f22 5d5b 5b32  l(ds["hello"][[2
+00010d00: 2c20 332c 2034 5d2c 2031 5d2c 205b 3231  , 3, 4], 1], [21
+00010d10: 2c20 3331 2c20 3431 5d29 0a20 2020 2020  , 31, 41]).     
+00010d20: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
+00010d30: 7365 7274 5f61 7272 6179 5f65 7175 616c  sert_array_equal
+00010d40: 2864 735b 2268 656c 6c6f 225d 5b5b 342c  (ds["hello"][[4,
+00010d50: 2035 2c20 365d 2c20 315d 2c20 5b34 312c   5, 6], 1], [41,
+00010d60: 2030 2c20 305d 290a 2020 2020 2020 2020   0, 0]).        
+00010d70: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
+00010d80: 745f 6172 7261 795f 6571 7561 6c28 6473  t_array_equal(ds
+00010d90: 5b22 6865 6c6c 6f22 5d5b 736c 6963 6528  ["hello"][slice(
+00010da0: 342c 2037 292c 2031 5d2c 205b 3431 2c20  4, 7), 1], [41, 
+00010db0: 302c 2030 5d29 0a0a 0a64 6566 2074 6573  0, 0])...def tes
+00010dc0: 745f 6835 7079 5f63 6875 6e6b 696e 6728  t_h5py_chunking(
+00010dd0: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
+00010de0: 293a 0a20 2020 2077 6974 6820 6835 6e65  ):.    with h5ne
+00010df0: 7463 6466 2e46 696c 6528 746d 705f 6c6f  tcdf.File(tmp_lo
+00010e00: 6361 6c5f 6e65 7463 6466 2c20 2277 2229  cal_netcdf, "w")
+00010e10: 2061 7320 6473 3a0a 2020 2020 2020 2020   as ds:.        
+00010e20: 6473 2e64 696d 656e 7369 6f6e 7320 3d20  ds.dimensions = 
+00010e30: 7b22 7822 3a20 3130 2c20 2279 223a 2031  {"x": 10, "y": 1
+00010e40: 302c 2022 7a22 3a20 3130 2c20 2274 223a  0, "z": 10, "t":
+00010e50: 204e 6f6e 657d 0a0a 2020 2020 2020 2020   None}..        
+00010e60: 7620 3d20 6473 2e63 7265 6174 655f 7661  v = ds.create_va
+00010e70: 7269 6162 6c65 280a 2020 2020 2020 2020  riable(.        
+00010e80: 2020 2020 2268 656c 6c6f 222c 2028 2278      "hello", ("x
+00010e90: 222c 2022 7922 2c20 227a 222c 2022 7422  ", "y", "z", "t"
+00010ea0: 292c 2022 666c 6f61 7422 2c20 6368 756e  ), "float", chun
+00010eb0: 6b69 6e67 5f68 6575 7269 7374 6963 3d22  king_heuristic="
+00010ec0: 6835 7079 220a 2020 2020 2020 2020 290a  h5py".        ).
+00010ed0: 2020 2020 2020 2020 6368 756e 6b73 5f68          chunks_h
+00010ee0: 3570 7920 3d20 762e 6368 756e 6b73 0a0a  5py = v.chunks..
+00010ef0: 2020 2020 2020 2020 6473 2e72 6573 697a          ds.resiz
+00010f00: 655f 6469 6d65 6e73 696f 6e28 2274 222c  e_dimension("t",
+00010f10: 2034 290a 2020 2020 2020 2020 7620 3d20   4).        v = 
+00010f20: 6473 2e63 7265 6174 655f 7661 7269 6162  ds.create_variab
+00010f30: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
+00010f40: 2268 656c 6c6f 3322 2c20 2822 7822 2c20  "hello3", ("x", 
+00010f50: 2279 222c 2022 7a22 2c20 2274 2229 2c20  "y", "z", "t"), 
+00010f60: 2266 6c6f 6174 222c 2063 6875 6e6b 696e  "float", chunkin
+00010f70: 675f 6865 7572 6973 7469 633d 2268 3570  g_heuristic="h5p
+00010f80: 7922 0a20 2020 2020 2020 2029 0a20 2020  y".        ).   
+00010f90: 2020 2020 2063 6875 6e6b 735f 7265 7369       chunks_resi
+00010fa0: 7a65 6420 3d20 762e 6368 756e 6b73 0a0a  zed = v.chunks..
+00010fb0: 2020 2020 2320 6361 7365 7320 6162 6f76      # cases abov
+00010fc0: 6520 7368 6f75 6c64 2062 6520 6571 7569  e should be equi
+00010fd0: 7661 6c65 6e74 2074 6f20 6120 6669 7865  valent to a fixe
+00010fe0: 6420 6469 6d65 6e73 696f 6e20 7769 7468  d dimension with
+00010ff0: 2061 7070 726f 7072 6961 7465 2073 697a   appropriate siz
+00011000: 650a 2020 2020 7769 7468 2068 356e 6574  e.    with h5net
+00011010: 6364 662e 4669 6c65 2874 6d70 5f6c 6f63  cdf.File(tmp_loc
+00011020: 616c 5f6e 6574 6364 662c 2022 7722 2920  al_netcdf, "w") 
+00011030: 6173 2064 733a 0a20 2020 2020 2020 2064  as ds:.        d
+00011040: 732e 6469 6d65 6e73 696f 6e73 203d 207b  s.dimensions = {
+00011050: 2278 223a 2031 302c 2022 7922 3a20 3130  "x": 10, "y": 10
+00011060: 2c20 227a 223a 2031 302c 2022 7422 3a20  , "z": 10, "t": 
+00011070: 3130 3234 7d0a 0a20 2020 2020 2020 2076  1024}..        v
+00011080: 203d 2064 732e 6372 6561 7465 5f76 6172   = ds.create_var
+00011090: 6961 626c 6528 0a20 2020 2020 2020 2020  iable(.         
+000110a0: 2020 2022 6865 6c6c 6f22 2c0a 2020 2020     "hello",.    
+000110b0: 2020 2020 2020 2020 2822 7822 2c20 2279          ("x", "y
+000110c0: 222c 2022 7a22 2c20 2274 2229 2c0a 2020  ", "z", "t"),.  
+000110d0: 2020 2020 2020 2020 2020 2266 6c6f 6174            "float
+000110e0: 222c 0a20 2020 2020 2020 2020 2020 2063  ",.            c
+000110f0: 6875 6e6b 733d 5472 7565 2c0a 2020 2020  hunks=True,.    
+00011100: 2020 2020 2020 2020 6368 756e 6b69 6e67          chunking
+00011110: 5f68 6575 7269 7374 6963 3d22 6835 7079  _heuristic="h5py
+00011120: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+00011130: 2020 2020 2063 6875 6e6b 735f 7472 7565       chunks_true
+00011140: 203d 2076 2e63 6875 6e6b 730a 0a20 2020   = v.chunks..   
+00011150: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+00011160: 696c 6528 746d 705f 6c6f 6361 6c5f 6e65  ile(tmp_local_ne
+00011170: 7463 6466 2c20 2277 2229 2061 7320 6473  tcdf, "w") as ds
+00011180: 3a0a 2020 2020 2020 2020 6473 2e64 696d  :.        ds.dim
+00011190: 656e 7369 6f6e 7320 3d20 7b22 7822 3a20  ensions = {"x": 
+000111a0: 3130 2c20 2279 223a 2031 302c 2022 7a22  10, "y": 10, "z"
+000111b0: 3a20 3130 2c20 2274 223a 2034 7d0a 0a20  : 10, "t": 4}.. 
+000111c0: 2020 2020 2020 2076 203d 2064 732e 6372         v = ds.cr
+000111d0: 6561 7465 5f76 6172 6961 626c 6528 0a20  eate_variable(. 
+000111e0: 2020 2020 2020 2020 2020 2022 6865 6c6c             "hell
+000111f0: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
+00011200: 2822 7822 2c20 2279 222c 2022 7a22 2c20  ("x", "y", "z", 
+00011210: 2274 2229 2c0a 2020 2020 2020 2020 2020  "t"),.          
+00011220: 2020 2266 6c6f 6174 222c 0a20 2020 2020    "float",.     
+00011230: 2020 2020 2020 2063 6875 6e6b 733d 5472         chunks=Tr
+00011240: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00011250: 6368 756e 6b69 6e67 5f68 6575 7269 7374  chunking_heurist
+00011260: 6963 3d22 6835 7079 222c 0a20 2020 2020  ic="h5py",.     
+00011270: 2020 2029 0a20 2020 2020 2020 2063 6875     ).        chu
+00011280: 6e6b 735f 7472 7565 5f72 6573 697a 6564  nks_true_resized
+00011290: 203d 2076 2e63 6875 6e6b 730a 0a20 2020   = v.chunks..   
+000112a0: 2061 7373 6572 7420 6368 756e 6b73 5f68   assert chunks_h
+000112b0: 3570 7920 3d3d 2063 6875 6e6b 735f 7472  5py == chunks_tr
+000112c0: 7565 0a20 2020 2061 7373 6572 7420 6368  ue.    assert ch
+000112d0: 756e 6b73 5f72 6573 697a 6564 203d 3d20  unks_resized == 
+000112e0: 6368 756e 6b73 5f74 7275 655f 7265 7369  chunks_true_resi
+000112f0: 7a65 640a 0a0a 6465 6620 7465 7374 5f68  zed...def test_h
+00011300: 356e 6574 6364 665f 6368 756e 6b69 6e67  5netcdf_chunking
+00011310: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
+00011320: 6629 3a0a 2020 2020 2320 7072 6f64 7563  f):.    # produc
+00011330: 6573 206d 7563 6820 736d 616c 6c65 7220  es much smaller 
+00011340: 6368 756e 6b73 2066 6f72 2075 6e73 697a  chunks for unsiz
+00011350: 6564 2064 696d 656e 7369 6f6e 730a 2020  ed dimensions.  
+00011360: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+00011370: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
+00011380: 6574 6364 662c 2022 7722 2920 6173 2064  etcdf, "w") as d
+00011390: 733a 0a20 2020 2020 2020 2064 732e 6469  s:.        ds.di
+000113a0: 6d65 6e73 696f 6e73 203d 207b 2278 223a  mensions = {"x":
+000113b0: 2031 302c 2022 7922 3a20 3130 2c20 227a   10, "y": 10, "z
+000113c0: 223a 2031 302c 2022 7422 3a20 4e6f 6e65  ": 10, "t": None
+000113d0: 7d0a 2020 2020 2020 2020 7620 3d20 6473  }.        v = ds
+000113e0: 2e63 7265 6174 655f 7661 7269 6162 6c65  .create_variable
+000113f0: 280a 2020 2020 2020 2020 2020 2020 2268  (.            "h
+00011400: 656c 6c6f 222c 2028 2278 222c 2022 7922  ello", ("x", "y"
+00011410: 2c20 227a 222c 2022 7422 292c 2022 666c  , "z", "t"), "fl
+00011420: 6f61 7422 2c20 6368 756e 6b69 6e67 5f68  oat", chunking_h
+00011430: 6575 7269 7374 6963 3d22 6835 6e65 7463  euristic="h5netc
+00011440: 6466 220a 2020 2020 2020 2020 290a 2020  df".        ).  
+00011450: 2020 2020 2020 6368 756e 6b73 5f68 356e        chunks_h5n
+00011460: 6574 6364 6620 3d20 762e 6368 756e 6b73  etcdf = v.chunks
+00011470: 0a0a 2020 2020 6173 7365 7274 2063 6875  ..    assert chu
+00011480: 6e6b 735f 6835 6e65 7463 6466 203d 3d20  nks_h5netcdf == 
+00011490: 2831 302c 2031 302c 2031 302c 2031 290a  (10, 10, 10, 1).
+000114a0: 0a20 2020 2023 2073 686f 756c 6420 7072  .    # should pr
+000114b0: 6f64 7563 6520 6368 756e 6b73 203e 2031  oduce chunks > 1
+000114c0: 2066 6f72 2073 6d61 6c6c 2066 6978 6564   for small fixed
+000114d0: 2064 696d 730a 2020 2020 7769 7468 2068   dims.    with h
+000114e0: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
+000114f0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
+00011500: 7722 2920 6173 2064 733a 0a20 2020 2020  w") as ds:.     
+00011510: 2020 2064 732e 6469 6d65 6e73 696f 6e73     ds.dimensions
+00011520: 203d 207b 2278 223a 2031 302c 2022 7422   = {"x": 10, "t"
+00011530: 3a20 4e6f 6e65 7d0a 2020 2020 2020 2020  : None}.        
+00011540: 7620 3d20 6473 2e63 7265 6174 655f 7661  v = ds.create_va
+00011550: 7269 6162 6c65 280a 2020 2020 2020 2020  riable(.        
+00011560: 2020 2020 2268 656c 6c6f 222c 2028 2278      "hello", ("x
+00011570: 222c 2022 7422 292c 2022 666c 6f61 7422  ", "t"), "float"
+00011580: 2c20 6368 756e 6b69 6e67 5f68 6575 7269  , chunking_heuri
+00011590: 7374 6963 3d22 6835 6e65 7463 6466 220a  stic="h5netcdf".
+000115a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000115b0: 2020 6368 756e 6b73 5f68 356e 6574 6364    chunks_h5netcd
+000115c0: 6620 3d20 762e 6368 756e 6b73 0a0a 2020  f = v.chunks..  
+000115d0: 2020 6173 7365 7274 2063 6875 6e6b 735f    assert chunks_
+000115e0: 6835 6e65 7463 6466 203d 3d20 2831 302c  h5netcdf == (10,
+000115f0: 2031 3238 290a 0a20 2020 2023 2072 6573   128)..    # res
+00011600: 697a 6564 2075 6e6c 696d 6974 6564 2064  ized unlimited d
+00011610: 696d 656e 7369 6f6e 7320 7368 6f75 6c64  imensions should
+00011620: 2062 6520 7472 6561 7465 6420 6c69 6b65   be treated like
+00011630: 2066 6978 6564 2064 696d 730a 2020 2020   fixed dims.    
+00011640: 7769 7468 2068 356e 6574 6364 662e 4669  with h5netcdf.Fi
+00011650: 6c65 2874 6d70 5f6c 6f63 616c 5f6e 6574  le(tmp_local_net
+00011660: 6364 662c 2022 7722 2920 6173 2064 733a  cdf, "w") as ds:
+00011670: 0a20 2020 2020 2020 2064 732e 6469 6d65  .        ds.dime
+00011680: 6e73 696f 6e73 203d 207b 2278 223a 2031  nsions = {"x": 1
+00011690: 302c 2022 7922 3a20 3130 2c20 227a 223a  0, "y": 10, "z":
+000116a0: 2031 302c 2022 7422 3a20 4e6f 6e65 7d0a   10, "t": None}.
+000116b0: 2020 2020 2020 2020 6473 2e72 6573 697a          ds.resiz
+000116c0: 655f 6469 6d65 6e73 696f 6e28 2274 222c  e_dimension("t",
+000116d0: 2031 3029 0a20 2020 2020 2020 2076 203d   10).        v =
+000116e0: 2064 732e 6372 6561 7465 5f76 6172 6961   ds.create_varia
+000116f0: 626c 6528 0a20 2020 2020 2020 2020 2020  ble(.           
+00011700: 2022 6865 6c6c 6f22 2c20 2822 7822 2c20   "hello", ("x", 
+00011710: 2279 222c 2022 7a22 2c20 2274 2229 2c20  "y", "z", "t"), 
+00011720: 2266 6c6f 6174 222c 2063 6875 6e6b 696e  "float", chunkin
+00011730: 675f 6865 7572 6973 7469 633d 2268 356e  g_heuristic="h5n
+00011740: 6574 6364 6622 0a20 2020 2020 2020 2029  etcdf".        )
+00011750: 0a20 2020 2020 2020 2063 6875 6e6b 735f  .        chunks_
+00011760: 6835 6e65 7463 6466 203d 2076 2e63 6875  h5netcdf = v.chu
+00011770: 6e6b 730a 0a20 2020 2061 7373 6572 7420  nks..    assert 
+00011780: 6368 756e 6b73 5f68 356e 6574 6364 6620  chunks_h5netcdf 
+00011790: 3d3d 2028 352c 2035 2c20 352c 2031 3029  == (5, 5, 5, 10)
+000117a0: 0a0a 0a64 6566 2074 6573 745f 6372 6561  ...def test_crea
+000117b0: 7465 5f69 6e76 616c 6964 5f6e 6574 6364  te_invalid_netcd
+000117c0: 665f 6361 7463 685f 6572 726f 7228 746d  f_catch_error(tm
+000117d0: 705f 6c6f 6361 6c5f 6e65 7463 6466 293a  p_local_netcdf):
+000117e0: 0a20 2020 2023 2073 6565 2068 7474 7073  .    # see https
+000117f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6835  ://github.com/h5
+00011800: 6e65 7463 6466 2f68 356e 6574 6364 662f  netcdf/h5netcdf/
+00011810: 6973 7375 6573 2f31 3338 0a20 2020 2077  issues/138.    w
+00011820: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
+00011830: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
+00011840: 6466 2c20 2277 2229 2061 7320 663a 0a20  df, "w") as f:. 
+00011850: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00011860: 2020 2020 2020 2020 662e 6372 6561 7465          f.create
+00011870: 5f76 6172 6961 626c 6528 2274 6573 7422  _variable("test"
+00011880: 2c20 2822 7822 2c20 2279 2229 2c20 6461  , ("x", "y"), da
+00011890: 7461 3d6e 702e 6f6e 6573 2828 3130 2c20  ta=np.ones((10, 
+000118a0: 3130 292c 2064 7479 7065 3d22 626f 6f6c  10), dtype="bool
+000118b0: 2229 290a 2020 2020 2020 2020 6578 6365  ")).        exce
+000118c0: 7074 2043 6f6d 7061 7469 6269 6c69 7479  pt Compatibility
+000118d0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+000118e0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
+000118f0: 6173 7365 7274 2072 6570 7228 662e 6469  assert repr(f.di
+00011900: 6d65 6e73 696f 6e73 2920 3d3d 2022 3c68  mensions) == "<h
+00011910: 356e 6574 6364 662e 4469 6d65 6e73 696f  5netcdf.Dimensio
+00011920: 6e73 3a20 3e22 0a0a 0a64 6566 2074 6573  ns: >"...def tes
+00011930: 745f 6469 6d65 6e73 696f 6e73 5f69 6e5f  t_dimensions_in_
+00011940: 7061 7265 6e74 5f67 726f 7570 7328 746d  parent_groups(tm
+00011950: 7064 6972 293a 0a20 2020 2077 6974 6820  pdir):.    with 
+00011960: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
+00011970: 746d 7064 6972 2e6a 6f69 6e28 2274 6573  tmpdir.join("tes
+00011980: 745f 6e65 7463 6466 2e6e 6322 292c 206d  t_netcdf.nc"), m
+00011990: 6f64 653d 2277 2229 2061 7320 6473 3a0a  ode="w") as ds:.
+000119a0: 2020 2020 2020 2020 6473 3020 3d20 6473          ds0 = ds
+000119b0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
+000119c0: 6e20 7261 6e67 6528 3130 293a 0a20 2020  n range(10):.   
+000119d0: 2020 2020 2020 2020 2064 7320 3d20 6473           ds = ds
+000119e0: 2e63 7265 6174 6547 726f 7570 2866 2267  .createGroup(f"g
+000119f0: 726f 7570 7b69 3a30 3264 7d22 290a 2020  roup{i:02d}").  
+00011a00: 2020 2020 2020 6473 302e 6372 6561 7465        ds0.create
+00011a10: 4469 6d65 6e73 696f 6e28 2278 222c 2031  Dimension("x", 1
+00011a20: 3029 0a20 2020 2020 2020 2064 7330 2e63  0).        ds0.c
+00011a30: 7265 6174 6544 696d 656e 7369 6f6e 2822  reateDimension("
+00011a40: 7922 2c20 3230 290a 2020 2020 2020 2020  y", 20).        
 00011a50: 6473 305b 2267 726f 7570 3030 225d 2e63  ds0["group00"].c
-00011a60: 7265 6174 6556 6172 6961 626c 6528 2278  reateVariable("x
-00011a70: 222c 2066 6c6f 6174 2c20 2822 7822 2c20  ", float, ("x", 
-00011a80: 2279 2229 290a 2020 2020 2020 2020 7661  "y")).        va
-00011a90: 725b 3a5d 203d 206e 702e 6f6e 6573 2828  r[:] = np.ones((
-00011aa0: 3130 2c20 3230 2929 0a0a 2020 2020 7769  10, 20))..    wi
-00011ab0: 7468 2068 356e 6574 6364 662e 4669 6c65  th h5netcdf.File
-00011ac0: 2874 6d70 6469 722e 6a6f 696e 2822 7465  (tmpdir.join("te
-00011ad0: 7374 5f6e 6574 6364 662e 6e63 2229 2c20  st_netcdf.nc"), 
-00011ae0: 6d6f 6465 3d22 7222 2920 6173 2064 7330  mode="r") as ds0
-00011af0: 3a0a 2020 2020 2020 2020 7769 7468 2068  :.        with h
-00011b00: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-00011b10: 6469 722e 6a6f 696e 2822 7465 7374 5f6c  dir.join("test_l
-00011b20: 6567 6163 792e 6e63 2229 2c20 6d6f 6465  egacy.nc"), mode
-00011b30: 3d22 7222 2920 6173 2064 7331 3a0a 2020  ="r") as ds1:.  
-00011b40: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00011b50: 2072 6570 7228 6473 302e 6469 6d65 6e73   repr(ds0.dimens
-00011b60: 696f 6e73 5b22 7822 5d29 203d 3d20 7265  ions["x"]) == re
-00011b70: 7072 2864 7331 2e64 696d 656e 7369 6f6e  pr(ds1.dimension
-00011b80: 735b 2278 225d 290a 2020 2020 2020 2020  s["x"]).        
-00011b90: 2020 2020 6173 7365 7274 2072 6570 7228      assert repr(
-00011ba0: 6473 302e 6469 6d65 6e73 696f 6e73 5b22  ds0.dimensions["
-00011bb0: 7922 5d29 203d 3d20 7265 7072 2864 7331  y"]) == repr(ds1
-00011bc0: 2e64 696d 656e 7369 6f6e 735b 2279 225d  .dimensions["y"]
-00011bd0: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-00011be0: 7365 7274 2072 6570 7228 6473 305b 2267  sert repr(ds0["g
-00011bf0: 726f 7570 3030 225d 2920 3d3d 2072 6570  roup00"]) == rep
-00011c00: 7228 6473 315b 2267 726f 7570 3030 225d  r(ds1["group00"]
-00011c10: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-00011c20: 7365 7274 2072 6570 7228 6473 305b 2267  sert repr(ds0["g
-00011c30: 726f 7570 3030 225d 5b22 7465 7374 225d  roup00"]["test"]
-00011c40: 2920 3d3d 2072 6570 7228 6473 315b 2267  ) == repr(ds1["g
-00011c50: 726f 7570 3030 225d 5b22 7465 7374 225d  roup00"]["test"]
-00011c60: 290a 2020 2020 2020 2020 2020 2020 6173  ).            as
-00011c70: 7365 7274 2072 6570 7228 6473 305b 2267  sert repr(ds0["g
-00011c80: 726f 7570 3030 225d 5b22 7822 5d29 203d  roup00"]["x"]) =
-00011c90: 3d20 7265 7072 2864 7331 5b22 6772 6f75  = repr(ds1["grou
-00011ca0: 7030 3022 5d5b 2278 225d 290a 0a0a 6465  p00"]["x"])...de
-00011cb0: 6620 7465 7374 5f61 7272 6179 5f61 7474  f test_array_att
-00011cc0: 7269 6275 7465 7328 746d 705f 6c6f 6361  ributes(tmp_loca
-00011cd0: 6c5f 6e65 7463 6466 293a 0a20 2020 2077  l_netcdf):.    w
-00011ce0: 6974 6820 6835 6e65 7463 6466 2e46 696c  ith h5netcdf.Fil
-00011cf0: 6528 746d 705f 6c6f 6361 6c5f 6e65 7463  e(tmp_local_netc
-00011d00: 6466 2c20 2277 2229 2061 7320 6473 3a0a  df, "w") as ds:.
-00011d10: 2020 2020 2020 2020 6474 203d 2068 3570          dt = h5p
-00011d20: 792e 7374 7269 6e67 5f64 7479 7065 2822  y.string_dtype("
-00011d30: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
-00011d40: 756e 6963 6f64 6520 3d20 2275 6e69 636f  unicode = "unico
-00011d50: 64c3 a922 0a20 2020 2020 2020 2064 732e  d..".        ds.
-00011d60: 6174 7472 735b 2275 6e69 636f 6465 225d  attrs["unicode"]
-00011d70: 203d 2075 6e69 636f 6465 0a20 2020 2020   = unicode.     
-00011d80: 2020 2064 732e 6174 7472 735b 2275 6e69     ds.attrs["uni
-00011d90: 636f 6465 5f30 6469 6d22 5d20 3d20 6e70  code_0dim"] = np
-00011da0: 2e61 7272 6179 2875 6e69 636f 6465 2c20  .array(unicode, 
-00011db0: 6474 7970 653d 6474 290a 2020 2020 2020  dtype=dt).      
-00011dc0: 2020 6473 2e61 7474 7273 5b22 756e 6963    ds.attrs["unic
-00011dd0: 6f64 655f 3164 696d 225d 203d 206e 702e  ode_1dim"] = np.
-00011de0: 6172 7261 7928 5b75 6e69 636f 6465 5d2c  array([unicode],
-00011df0: 2064 7479 7065 3d64 7429 0a20 2020 2020   dtype=dt).     
-00011e00: 2020 2064 732e 6174 7472 735b 2275 6e69     ds.attrs["uni
-00011e10: 636f 6465 5f61 7272 6172 7922 5d20 3d20  code_arrary"] = 
-00011e20: 6e70 2e61 7272 6179 285b 756e 6963 6f64  np.array([unicod
-00011e30: 652c 2022 666f 6f62 c3a1 7222 5d2c 2064  e, "foob..r"], d
-00011e40: 7479 7065 3d64 7429 0a20 2020 2020 2020  type=dt).       
-00011e50: 2064 732e 6174 7472 735b 2275 6e69 636f   ds.attrs["unico
-00011e60: 6465 5f6c 6973 7422 5d20 3d20 5b75 6e69  de_list"] = [uni
-00011e70: 636f 6465 5d0a 0a20 2020 2020 2020 2064  code]..        d
-00011e80: 7420 3d20 6835 7079 2e73 7472 696e 675f  t = h5py.string_
-00011e90: 6474 7970 6528 2261 7363 6969 2229 0a20  dtype("ascii"). 
-00011ea0: 2020 2020 2020 2023 2069 6620 6474 7970         # if dtyp
-00011eb0: 6520 6973 2061 7363 6969 2069 7427 7320  e is ascii it's 
-00011ec0: 6972 7265 6c65 7661 6e74 2069 6620 7468  irrelevant if th
-00011ed0: 6520 6461 7461 2069 7320 7072 6f76 6964  e data is provid
-00011ee0: 6564 2061 7320 6279 7465 7320 6f72 2073  ed as bytes or s
-00011ef0: 7472 696e 670a 2020 2020 2020 2020 6173  tring.        as
-00011f00: 6369 6920 3d20 2261 7363 6969 220a 2020  cii = "ascii".  
-00011f10: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
-00011f20: 6173 6369 6922 5d20 3d20 6173 6369 690a  ascii"] = ascii.
-00011f30: 2020 2020 2020 2020 6473 2e61 7474 7273          ds.attrs
-00011f40: 5b22 6173 6369 695f 3064 696d 225d 203d  ["ascii_0dim"] =
-00011f50: 206e 702e 6172 7261 7928 6173 6369 692c   np.array(ascii,
-00011f60: 2064 7479 7065 3d64 7429 0a20 2020 2020   dtype=dt).     
-00011f70: 2020 2064 732e 6174 7472 735b 2261 7363     ds.attrs["asc
-00011f80: 6969 5f31 6469 6d22 5d20 3d20 6e70 2e61  ii_1dim"] = np.a
-00011f90: 7272 6179 285b 6173 6369 695d 2c20 6474  rray([ascii], dt
-00011fa0: 7970 653d 6474 290a 2020 2020 2020 2020  ype=dt).        
-00011fb0: 6473 2e61 7474 7273 5b22 6173 6369 695f  ds.attrs["ascii_
-00011fc0: 6172 7261 7922 5d20 3d20 6e70 2e61 7272  array"] = np.arr
-00011fd0: 6179 285b 6173 6369 692c 2022 666f 6f62  ay([ascii, "foob
-00011fe0: 6172 225d 2c20 6474 7970 653d 6474 290a  ar"], dtype=dt).
-00011ff0: 2020 2020 2020 2020 6473 2e61 7474 7273          ds.attrs
-00012000: 5b22 6173 6369 695f 6c69 7374 225d 203d  ["ascii_list"] =
-00012010: 205b 6173 6369 695d 0a0a 2020 2020 2020   [ascii]..      
-00012020: 2020 6173 6369 6920 3d20 6222 6173 6369    ascii = b"asci
-00012030: 6922 0a20 2020 2020 2020 2064 732e 6174  i".        ds.at
-00012040: 7472 735b 2262 7974 6573 225d 203d 2061  trs["bytes"] = a
-00012050: 7363 6969 0a20 2020 2020 2020 2064 732e  scii.        ds.
-00012060: 6174 7472 735b 2262 7974 6573 5f30 6469  attrs["bytes_0di
-00012070: 6d22 5d20 3d20 6e70 2e61 7272 6179 2861  m"] = np.array(a
-00012080: 7363 6969 2c20 6474 7970 653d 6474 290a  scii, dtype=dt).
-00012090: 2020 2020 2020 2020 6473 2e61 7474 7273          ds.attrs
-000120a0: 5b22 6279 7465 735f 3164 696d 225d 203d  ["bytes_1dim"] =
-000120b0: 206e 702e 6172 7261 7928 5b61 7363 6969   np.array([ascii
-000120c0: 5d2c 2064 7479 7065 3d64 7429 0a20 2020  ], dtype=dt).   
-000120d0: 2020 2020 2064 732e 6174 7472 735b 2262       ds.attrs["b
-000120e0: 7974 6573 5f61 7272 6179 225d 203d 206e  ytes_array"] = n
-000120f0: 702e 6172 7261 7928 5b61 7363 6969 2c20  p.array([ascii, 
-00012100: 6222 666f 6f62 6172 225d 2c20 6474 7970  b"foobar"], dtyp
-00012110: 653d 6474 290a 2020 2020 2020 2020 6473  e=dt).        ds
-00012120: 2e61 7474 7273 5b22 6279 7465 735f 6c69  .attrs["bytes_li
-00012130: 7374 225d 203d 205b 6173 6369 695d 0a0a  st"] = [ascii]..
-00012140: 2020 2020 2020 2020 6474 203d 2068 3570          dt = h5p
-00012150: 792e 7374 7269 6e67 5f64 7479 7065 2822  y.string_dtype("
-00012160: 7574 662d 3822 2c20 3130 290a 2020 2020  utf-8", 10).    
-00012170: 2020 2020 2320 756e 6963 6f64 6520 6e65      # unicode ne
-00012180: 6564 7320 746f 2062 6520 656e 636f 6465  eds to be encode
-00012190: 6420 7072 6f70 6572 6c79 2066 6f72 2066  d properly for f
-000121a0: 6978 6564 2073 697a 6520 7374 7269 6e67  ixed size string
-000121b0: 2074 7970 650a 2020 2020 2020 2020 6473   type.        ds
-000121c0: 2e61 7474 7273 5b22 756e 6963 6f64 655f  .attrs["unicode_
-000121d0: 6669 7865 6422 5d20 3d20 6e70 2e61 7272  fixed"] = np.arr
-000121e0: 6179 2875 6e69 636f 6465 2e65 6e63 6f64  ay(unicode.encod
-000121f0: 6528 2275 7466 2d38 2229 2c20 6474 7970  e("utf-8"), dtyp
-00012200: 653d 6474 290a 2020 2020 2020 2020 6473  e=dt).        ds
-00012210: 2e61 7474 7273 5b22 756e 6963 6f64 655f  .attrs["unicode_
-00012220: 6669 7865 645f 3064 696d 225d 203d 206e  fixed_0dim"] = n
-00012230: 702e 6172 7261 7928 756e 6963 6f64 652e  p.array(unicode.
-00012240: 656e 636f 6465 2822 7574 662d 3822 292c  encode("utf-8"),
-00012250: 2064 7479 7065 3d64 7429 0a20 2020 2020   dtype=dt).     
-00012260: 2020 2064 732e 6174 7472 735b 2275 6e69     ds.attrs["uni
-00012270: 636f 6465 5f66 6978 6564 5f31 6469 6d22  code_fixed_1dim"
-00012280: 5d20 3d20 6e70 2e61 7272 6179 285b 756e  ] = np.array([un
-00012290: 6963 6f64 652e 656e 636f 6465 2822 7574  icode.encode("ut
-000122a0: 662d 3822 295d 2c20 6474 7970 653d 6474  f-8")], dtype=dt
-000122b0: 290a 2020 2020 2020 2020 6473 2e61 7474  ).        ds.att
-000122c0: 7273 5b22 756e 6963 6f64 655f 6669 7865  rs["unicode_fixe
-000122d0: 645f 6172 7261 7279 225d 203d 206e 702e  d_arrary"] = np.
-000122e0: 6172 7261 7928 0a20 2020 2020 2020 2020  array(.         
-000122f0: 2020 205b 756e 6963 6f64 652e 656e 636f     [unicode.enco
-00012300: 6465 2822 7574 662d 3822 292c 2022 666f  de("utf-8"), "fo
-00012310: 6f62 c3a1 7222 2e65 6e63 6f64 6528 2275  ob..r".encode("u
-00012320: 7466 2d38 2229 5d2c 2064 7479 7065 3d64  tf-8")], dtype=d
-00012330: 740a 2020 2020 2020 2020 290a 0a20 2020  t.        )..   
-00012340: 2020 2020 2064 7420 3d20 6835 7079 2e73       dt = h5py.s
-00012350: 7472 696e 675f 6474 7970 6528 2261 7363  tring_dtype("asc
-00012360: 6969 222c 2031 3029 0a20 2020 2020 2020  ii", 10).       
-00012370: 2061 7363 6969 203d 2022 6173 6369 6922   ascii = "ascii"
-00012380: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
-00012390: 735b 2261 7363 6969 5f66 6978 6564 225d  s["ascii_fixed"]
-000123a0: 203d 206e 702e 6172 7261 7928 6173 6369   = np.array(asci
-000123b0: 692c 2064 7479 7065 3d64 7429 0a20 2020  i, dtype=dt).   
-000123c0: 2020 2020 2064 732e 6174 7472 735b 2261       ds.attrs["a
-000123d0: 7363 6969 5f66 6978 6564 5f30 6469 6d22  scii_fixed_0dim"
-000123e0: 5d20 3d20 6e70 2e61 7272 6179 2861 7363  ] = np.array(asc
-000123f0: 6969 2c20 6474 7970 653d 6474 290a 2020  ii, dtype=dt).  
-00012400: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
-00012410: 6173 6369 695f 6669 7865 645f 3164 696d  ascii_fixed_1dim
-00012420: 225d 203d 206e 702e 6172 7261 7928 5b61  "] = np.array([a
-00012430: 7363 6969 5d2c 2064 7479 7065 3d64 7429  scii], dtype=dt)
-00012440: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
-00012450: 735b 2261 7363 6969 5f66 6978 6564 5f61  s["ascii_fixed_a
-00012460: 7272 6179 225d 203d 206e 702e 6172 7261  rray"] = np.arra
-00012470: 7928 5b61 7363 6969 2c20 2266 6f6f 6261  y([ascii, "fooba
-00012480: 7222 5d2c 2064 7479 7065 3d64 7429 0a0a  r"], dtype=dt)..
-00012490: 2020 2020 2020 2020 6173 6369 6920 3d20          ascii = 
-000124a0: 6222 6173 6369 6922 0a20 2020 2020 2020  b"ascii".       
-000124b0: 2064 732e 6174 7472 735b 2262 7974 6573   ds.attrs["bytes
-000124c0: 5f66 6978 6564 225d 203d 206e 702e 6172  _fixed"] = np.ar
-000124d0: 7261 7928 6173 6369 692c 2064 7479 7065  ray(ascii, dtype
-000124e0: 3d64 7429 0a20 2020 2020 2020 2064 732e  =dt).        ds.
-000124f0: 6174 7472 735b 2262 7974 6573 5f66 6978  attrs["bytes_fix
-00012500: 6564 5f30 6469 6d22 5d20 3d20 6e70 2e61  ed_0dim"] = np.a
-00012510: 7272 6179 2861 7363 6969 2c20 6474 7970  rray(ascii, dtyp
-00012520: 653d 6474 290a 2020 2020 2020 2020 6473  e=dt).        ds
-00012530: 2e61 7474 7273 5b22 6279 7465 735f 6669  .attrs["bytes_fi
-00012540: 7865 645f 3164 696d 225d 203d 206e 702e  xed_1dim"] = np.
-00012550: 6172 7261 7928 5b61 7363 6969 5d2c 2064  array([ascii], d
-00012560: 7479 7065 3d64 7429 0a20 2020 2020 2020  type=dt).       
-00012570: 2064 732e 6174 7472 735b 2262 7974 6573   ds.attrs["bytes
-00012580: 5f66 6978 6564 5f61 7272 6179 225d 203d  _fixed_array"] =
-00012590: 206e 702e 6172 7261 7928 5b61 7363 6969   np.array([ascii
-000125a0: 2c20 6222 666f 6f62 6172 225d 2c20 6474  , b"foobar"], dt
-000125b0: 7970 653d 6474 290a 0a20 2020 2020 2020  ype=dt)..       
-000125c0: 2064 732e 6174 7472 735b 2269 6e74 225d   ds.attrs["int"]
-000125d0: 203d 2031 0a20 2020 2020 2020 2064 732e   = 1.        ds.
-000125e0: 6174 7472 735b 2269 6e74 6c69 7374 225d  attrs["intlist"]
-000125f0: 203d 205b 315d 0a20 2020 2020 2020 2064   = [1].        d
-00012600: 732e 6174 7472 735b 2269 6e74 5f61 7272  s.attrs["int_arr
-00012610: 6179 225d 203d 206e 702e 6172 616e 6765  ay"] = np.arange
-00012620: 2831 3029 0a20 2020 2020 2020 2064 732e  (10).        ds.
-00012630: 6174 7472 735b 2265 6d70 7479 5f6c 6973  attrs["empty_lis
-00012640: 7422 5d20 3d20 5b5d 0a20 2020 2020 2020  t"] = [].       
-00012650: 2064 732e 6174 7472 735b 2265 6d70 7479   ds.attrs["empty
-00012660: 5f61 7272 6179 225d 203d 206e 702e 6172  _array"] = np.ar
-00012670: 7261 7928 5b5d 290a 0a20 2020 2077 6974  ray([])..    wit
-00012680: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
-00012690: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-000126a0: 2c20 6d6f 6465 3d22 7222 2920 6173 2064  , mode="r") as d
-000126b0: 733a 0a20 2020 2020 2020 2061 7373 6572  s:.        asser
-000126c0: 7420 6473 2e61 7474 7273 5b22 756e 6963  t ds.attrs["unic
-000126d0: 6f64 6522 5d20 3d3d 2075 6e69 636f 6465  ode"] == unicode
-000126e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000126f0: 6473 2e61 7474 7273 5b22 756e 6963 6f64  ds.attrs["unicod
-00012700: 655f 3064 696d 225d 203d 3d20 756e 6963  e_0dim"] == unic
-00012710: 6f64 650a 2020 2020 2020 2020 6173 7365  ode.        asse
-00012720: 7274 2064 732e 6174 7472 735b 2275 6e69  rt ds.attrs["uni
-00012730: 636f 6465 5f31 6469 6d22 5d20 3d3d 2075  code_1dim"] == u
-00012740: 6e69 636f 6465 0a20 2020 2020 2020 2061  nicode.        a
-00012750: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
-00012760: 756e 6963 6f64 655f 6172 7261 7279 225d  unicode_arrary"]
-00012770: 203d 3d20 5b75 6e69 636f 6465 2c20 2266   == [unicode, "f
-00012780: 6f6f 62c3 a172 225d 0a20 2020 2020 2020  oob..r"].       
-00012790: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
-000127a0: 5b22 756e 6963 6f64 655f 6c69 7374 225d  ["unicode_list"]
-000127b0: 203d 3d20 756e 6963 6f64 650a 0a20 2020   == unicode..   
-000127c0: 2020 2020 2023 2062 7974 6573 2061 6e64       # bytes and
-000127d0: 2073 7472 696e 6773 2061 7265 2072 6563   strings are rec
-000127e0: 6569 7665 6420 6173 2073 7472 696e 6773  eived as strings
-000127f0: 2066 6f72 2068 3570 7933 0a20 2020 2020   for h5py3.     
-00012800: 2020 2069 6620 7665 7273 696f 6e2e 7061     if version.pa
-00012810: 7273 6528 6835 7079 2e5f 5f76 6572 7369  rse(h5py.__versi
-00012820: 6f6e 5f5f 2920 3e3d 2076 6572 7369 6f6e  on__) >= version
-00012830: 2e70 6172 7365 2822 332e 302e 3022 293a  .parse("3.0.0"):
-00012840: 0a20 2020 2020 2020 2020 2020 2061 7363  .            asc
-00012850: 6969 203d 2022 6173 6369 6922 0a20 2020  ii = "ascii".   
-00012860: 2020 2020 2020 2020 2066 6f6f 6261 7220           foobar 
-00012870: 3d20 2266 6f6f 6261 7222 0a20 2020 2020  = "foobar".     
-00012880: 2020 2023 2061 6e64 2062 7974 6573 2066     # and bytes f
-00012890: 6f72 2068 3570 7932 0a20 2020 2020 2020  or h5py2.       
-000128a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000128b0: 2020 2061 7363 6969 203d 2062 2261 7363     ascii = b"asc
-000128c0: 6969 220a 2020 2020 2020 2020 2020 2020  ii".            
-000128d0: 666f 6f62 6172 203d 2062 2266 6f6f 6261  foobar = b"fooba
-000128e0: 7222 0a20 2020 2020 2020 2061 7373 6572  r".        asser
-000128f0: 7420 6473 2e61 7474 7273 5b22 6173 6369  t ds.attrs["asci
-00012900: 6922 5d20 3d3d 2022 6173 6369 6922 0a20  i"] == "ascii". 
-00012910: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-00012920: 2e61 7474 7273 5b22 6173 6369 695f 3064  .attrs["ascii_0d
-00012930: 696d 225d 203d 3d20 6173 6369 690a 2020  im"] == ascii.  
-00012940: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-00012950: 6174 7472 735b 2261 7363 6969 5f31 6469  attrs["ascii_1di
-00012960: 6d22 5d20 3d3d 2061 7363 6969 0a20 2020  m"] == ascii.   
-00012970: 2020 2020 2061 7373 6572 7420 6473 2e61       assert ds.a
-00012980: 7474 7273 5b22 6173 6369 695f 6172 7261  ttrs["ascii_arra
-00012990: 7922 5d20 3d3d 205b 6173 6369 692c 2066  y"] == [ascii, f
-000129a0: 6f6f 6261 725d 0a20 2020 2020 2020 2023  oobar].        #
-000129b0: 206c 6973 7420 6973 2064 6563 6f64 6564   list is decoded
-000129c0: 2066 6f72 2068 3570 7932 0a20 2020 2020   for h5py2.     
-000129d0: 2020 2061 7373 6572 7420 6473 2e61 7474     assert ds.att
-000129e0: 7273 5b22 6173 6369 695f 6c69 7374 225d  rs["ascii_list"]
-000129f0: 203d 3d20 2261 7363 6969 220a 0a20 2020   == "ascii"..   
-00012a00: 2020 2020 2061 7373 6572 7420 6473 2e61       assert ds.a
-00012a10: 7474 7273 5b22 6279 7465 7322 5d20 3d3d  ttrs["bytes"] ==
-00012a20: 2061 7363 6969 0a20 2020 2020 2020 2061   ascii.        a
-00012a30: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
-00012a40: 6279 7465 735f 3064 696d 225d 203d 3d20  bytes_0dim"] == 
-00012a50: 6173 6369 690a 2020 2020 2020 2020 6173  ascii.        as
-00012a60: 7365 7274 2064 732e 6174 7472 735b 2262  sert ds.attrs["b
-00012a70: 7974 6573 5f31 6469 6d22 5d20 3d3d 2061  ytes_1dim"] == a
-00012a80: 7363 6969 0a20 2020 2020 2020 2061 7373  scii.        ass
-00012a90: 6572 7420 6473 2e61 7474 7273 5b22 6279  ert ds.attrs["by
-00012aa0: 7465 735f 6172 7261 7922 5d20 3d3d 205b  tes_array"] == [
-00012ab0: 6173 6369 692c 2066 6f6f 6261 725d 0a20  ascii, foobar]. 
-00012ac0: 2020 2020 2020 2023 206c 6973 7420 6973         # list is
-00012ad0: 2064 6563 6f64 6564 2066 6f72 2068 3570   decoded for h5p
-00012ae0: 7932 0a20 2020 2020 2020 2061 7373 6572  y2.        asser
-00012af0: 7420 6473 2e61 7474 7273 5b22 6279 7465  t ds.attrs["byte
-00012b00: 735f 6c69 7374 225d 203d 3d20 2261 7363  s_list"] == "asc
-00012b10: 6969 220a 0a20 2020 2020 2020 2061 7373  ii"..        ass
-00012b20: 6572 7420 6473 2e61 7474 7273 5b22 756e  ert ds.attrs["un
-00012b30: 6963 6f64 655f 6669 7865 6422 5d20 3d3d  icode_fixed"] ==
-00012b40: 2075 6e69 636f 6465 0a20 2020 2020 2020   unicode.       
-00012b50: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
-00012b60: 5b22 756e 6963 6f64 655f 6669 7865 645f  ["unicode_fixed_
-00012b70: 3064 696d 225d 203d 3d20 756e 6963 6f64  0dim"] == unicod
-00012b80: 650a 2020 2020 2020 2020 6173 7365 7274  e.        assert
-00012b90: 2064 732e 6174 7472 735b 2275 6e69 636f   ds.attrs["unico
-00012ba0: 6465 5f66 6978 6564 5f31 6469 6d22 5d20  de_fixed_1dim"] 
-00012bb0: 3d3d 2075 6e69 636f 6465 0a20 2020 2020  == unicode.     
-00012bc0: 2020 2061 7373 6572 7420 6473 2e61 7474     assert ds.att
-00012bd0: 7273 5b22 756e 6963 6f64 655f 6669 7865  rs["unicode_fixe
-00012be0: 645f 6172 7261 7279 225d 203d 3d20 5b75  d_arrary"] == [u
-00012bf0: 6e69 636f 6465 2c20 2266 6f6f 62c3 a172  nicode, "foob..r
-00012c00: 225d 0a0a 2020 2020 2020 2020 6173 6369  "]..        asci
-00012c10: 6920 3d20 2261 7363 6969 220a 2020 2020  i = "ascii".    
-00012c20: 2020 2020 6173 7365 7274 2064 732e 6174      assert ds.at
-00012c30: 7472 735b 2261 7363 6969 5f66 6978 6564  trs["ascii_fixed
-00012c40: 225d 203d 3d20 6173 6369 690a 2020 2020  "] == ascii.    
-00012c50: 2020 2020 6173 7365 7274 2064 732e 6174      assert ds.at
-00012c60: 7472 735b 2261 7363 6969 5f66 6978 6564  trs["ascii_fixed
-00012c70: 5f30 6469 6d22 5d20 3d3d 2061 7363 6969  _0dim"] == ascii
-00012c80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00012c90: 6473 2e61 7474 7273 5b22 6173 6369 695f  ds.attrs["ascii_
-00012ca0: 6669 7865 645f 3164 696d 225d 203d 3d20  fixed_1dim"] == 
-00012cb0: 6173 6369 690a 2020 2020 2020 2020 6173  ascii.        as
-00012cc0: 7365 7274 2064 732e 6174 7472 735b 2261  sert ds.attrs["a
-00012cd0: 7363 6969 5f66 6978 6564 5f61 7272 6179  scii_fixed_array
-00012ce0: 225d 203d 3d20 5b61 7363 6969 2c20 2266  "] == [ascii, "f
-00012cf0: 6f6f 6261 7222 5d0a 0a20 2020 2020 2020  oobar"]..       
-00012d00: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
-00012d10: 5b22 6279 7465 735f 6669 7865 6422 5d20  ["bytes_fixed"] 
-00012d20: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
-00012d30: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
-00012d40: 5b22 6279 7465 735f 6669 7865 645f 3064  ["bytes_fixed_0d
-00012d50: 696d 225d 203d 3d20 6173 6369 690a 2020  im"] == ascii.  
-00012d60: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-00012d70: 6174 7472 735b 2262 7974 6573 5f66 6978  attrs["bytes_fix
-00012d80: 6564 5f31 6469 6d22 5d20 3d3d 2061 7363  ed_1dim"] == asc
-00012d90: 6969 0a20 2020 2020 2020 2061 7373 6572  ii.        asser
-00012da0: 7420 6473 2e61 7474 7273 5b22 6279 7465  t ds.attrs["byte
-00012db0: 735f 6669 7865 645f 6172 7261 7922 5d20  s_fixed_array"] 
-00012dc0: 3d3d 205b 6173 6369 692c 2022 666f 6f62  == [ascii, "foob
-00012dd0: 6172 225d 0a0a 2020 2020 2020 2020 6173  ar"]..        as
-00012de0: 7365 7274 2064 732e 6174 7472 735b 2269  sert ds.attrs["i
-00012df0: 6e74 225d 203d 3d20 310a 2020 2020 2020  nt"] == 1.      
-00012e00: 2020 6173 7365 7274 2064 732e 6174 7472    assert ds.attr
-00012e10: 735b 2269 6e74 6c69 7374 225d 203d 3d20  s["intlist"] == 
-00012e20: 310a 2020 2020 2020 2020 6e70 2e74 6573  1.        np.tes
-00012e30: 7469 6e67 2e61 7373 6572 745f 6571 7561  ting.assert_equa
-00012e40: 6c28 6473 2e61 7474 7273 5b22 696e 745f  l(ds.attrs["int_
-00012e50: 6172 7261 7922 5d2c 206e 702e 6172 616e  array"], np.aran
-00012e60: 6765 2831 3029 290a 2020 2020 2020 2020  ge(10)).        
-00012e70: 6e70 2e74 6573 7469 6e67 2e61 7373 6572  np.testing.asser
-00012e80: 745f 6571 7561 6c28 6473 2e61 7474 7273  t_equal(ds.attrs
-00012e90: 5b22 656d 7074 795f 6c69 7374 225d 2c20  ["empty_list"], 
-00012ea0: 6e70 2e61 7272 6179 285b 5d29 290a 2020  np.array([])).  
-00012eb0: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
-00012ec0: 2e61 7373 6572 745f 6571 7561 6c28 6473  .assert_equal(ds
-00012ed0: 2e61 7474 7273 5b22 656d 7074 795f 6172  .attrs["empty_ar
-00012ee0: 7261 7922 5d2c 206e 702e 6172 7261 7928  ray"], np.array(
-00012ef0: 5b5d 2929 0a0a 2020 2020 7769 7468 206c  []))..    with l
-00012f00: 6567 6163 7961 7069 2e44 6174 6173 6574  egacyapi.Dataset
-00012f10: 2874 6d70 5f6c 6f63 616c 5f6e 6574 6364  (tmp_local_netcd
-00012f20: 662c 206d 6f64 653d 2272 2229 2061 7320  f, mode="r") as 
-00012f30: 6473 3a0a 2020 2020 2020 2020 6173 7365  ds:.        asse
-00012f40: 7274 2064 732e 756e 6963 6f64 6520 3d3d  rt ds.unicode ==
-00012f50: 2075 6e69 636f 6465 0a20 2020 2020 2020   unicode.       
-00012f60: 2061 7373 6572 7420 6473 2e75 6e69 636f   assert ds.unico
-00012f70: 6465 5f30 6469 6d20 3d3d 2075 6e69 636f  de_0dim == unico
-00012f80: 6465 0a20 2020 2020 2020 2061 7373 6572  de.        asser
-00012f90: 7420 6473 2e75 6e69 636f 6465 5f31 6469  t ds.unicode_1di
-00012fa0: 6d20 3d3d 2075 6e69 636f 6465 0a20 2020  m == unicode.   
-00012fb0: 2020 2020 2061 7373 6572 7420 6473 2e75       assert ds.u
-00012fc0: 6e69 636f 6465 5f61 7272 6172 7920 3d3d  nicode_arrary ==
-00012fd0: 205b 756e 6963 6f64 652c 2022 666f 6f62   [unicode, "foob
-00012fe0: c3a1 7222 5d0a 2020 2020 2020 2020 6173  ..r"].        as
-00012ff0: 7365 7274 2064 732e 756e 6963 6f64 655f  sert ds.unicode_
-00013000: 6c69 7374 203d 3d20 756e 6963 6f64 650a  list == unicode.
-00013010: 0a20 2020 2020 2020 2023 2062 7974 6573  .        # bytes
-00013020: 2061 6e64 2073 7472 696e 6773 2061 7265   and strings are
-00013030: 2072 6563 6569 7665 6420 6173 2073 7472   received as str
-00013040: 696e 6773 2066 6f72 2068 3570 7933 0a20  ings for h5py3. 
-00013050: 2020 2020 2020 2069 6620 7665 7273 696f         if versio
-00013060: 6e2e 7061 7273 6528 6835 7079 2e5f 5f76  n.parse(h5py.__v
-00013070: 6572 7369 6f6e 5f5f 2920 3e3d 2076 6572  ersion__) >= ver
-00013080: 7369 6f6e 2e70 6172 7365 2822 332e 302e  sion.parse("3.0.
-00013090: 3022 293a 0a20 2020 2020 2020 2020 2020  0"):.           
-000130a0: 2061 7363 6969 203d 2022 6173 6369 6922   ascii = "ascii"
-000130b0: 0a20 2020 2020 2020 2020 2020 2066 6f6f  .            foo
-000130c0: 6261 7220 3d20 2266 6f6f 6261 7222 0a20  bar = "foobar". 
-000130d0: 2020 2020 2020 2023 2061 6e64 2062 7974         # and byt
-000130e0: 6573 2066 6f72 2068 3570 7932 0a20 2020  es for h5py2.   
-000130f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00013100: 2020 2020 2020 2061 7363 6969 203d 2062         ascii = b
-00013110: 2261 7363 6969 220a 2020 2020 2020 2020  "ascii".        
-00013120: 2020 2020 666f 6f62 6172 203d 2062 2266      foobar = b"f
-00013130: 6f6f 6261 7222 0a20 2020 2020 2020 2061  oobar".        a
-00013140: 7373 6572 7420 6473 2e61 7363 6969 203d  ssert ds.ascii =
-00013150: 3d20 2261 7363 6969 220a 2020 2020 2020  = "ascii".      
-00013160: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
-00013170: 695f 3064 696d 203d 3d20 6173 6369 690a  i_0dim == ascii.
-00013180: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00013190: 732e 6173 6369 695f 3164 696d 203d 3d20  s.ascii_1dim == 
-000131a0: 6173 6369 690a 2020 2020 2020 2020 6173  ascii.        as
-000131b0: 7365 7274 2064 732e 6173 6369 695f 6172  sert ds.ascii_ar
-000131c0: 7261 7920 3d3d 205b 6173 6369 692c 2066  ray == [ascii, f
-000131d0: 6f6f 6261 725d 0a20 2020 2020 2020 2023  oobar].        #
-000131e0: 206c 6973 7420 6973 2064 6563 6f64 6564   list is decoded
-000131f0: 2066 6f72 2068 3570 7932 0a20 2020 2020   for h5py2.     
-00013200: 2020 2061 7373 6572 7420 6473 2e61 7363     assert ds.asc
-00013210: 6969 5f6c 6973 7420 3d3d 2022 6173 6369  ii_list == "asci
-00013220: 6922 0a0a 2020 2020 2020 2020 6173 7365  i"..        asse
-00013230: 7274 2064 732e 6279 7465 7320 3d3d 2061  rt ds.bytes == a
-00013240: 7363 6969 0a20 2020 2020 2020 2061 7373  scii.        ass
-00013250: 6572 7420 6473 2e62 7974 6573 5f30 6469  ert ds.bytes_0di
-00013260: 6d20 3d3d 2061 7363 6969 0a20 2020 2020  m == ascii.     
-00013270: 2020 2061 7373 6572 7420 6473 2e62 7974     assert ds.byt
-00013280: 6573 5f31 6469 6d20 3d3d 2061 7363 6969  es_1dim == ascii
-00013290: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000132a0: 6473 2e62 7974 6573 5f61 7272 6179 203d  ds.bytes_array =
-000132b0: 3d20 5b61 7363 6969 2c20 666f 6f62 6172  = [ascii, foobar
-000132c0: 5d0a 2020 2020 2020 2020 2320 6c69 7374  ].        # list
-000132d0: 2069 7320 6465 636f 6465 6420 666f 7220   is decoded for 
-000132e0: 6835 7079 320a 2020 2020 2020 2020 6173  h5py2.        as
-000132f0: 7365 7274 2064 732e 6279 7465 735f 6c69  sert ds.bytes_li
-00013300: 7374 203d 3d20 2261 7363 6969 220a 0a20  st == "ascii".. 
-00013310: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-00013320: 2e75 6e69 636f 6465 5f66 6978 6564 203d  .unicode_fixed =
-00013330: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-00013340: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-00013350: 6f64 655f 6669 7865 645f 3064 696d 203d  ode_fixed_0dim =
-00013360: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-00013370: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-00013380: 6f64 655f 6669 7865 645f 3164 696d 203d  ode_fixed_1dim =
-00013390: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-000133a0: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-000133b0: 6f64 655f 6669 7865 645f 6172 7261 7279  ode_fixed_arrary
-000133c0: 203d 3d20 5b75 6e69 636f 6465 2c20 2266   == [unicode, "f
-000133d0: 6f6f 62c3 a172 225d 0a0a 2020 2020 2020  oob..r"]..      
-000133e0: 2020 6173 6369 6920 3d20 2261 7363 6969    ascii = "ascii
-000133f0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00013400: 2064 732e 6173 6369 695f 6669 7865 6420   ds.ascii_fixed 
-00013410: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
-00013420: 2061 7373 6572 7420 6473 2e61 7363 6969   assert ds.ascii
-00013430: 5f66 6978 6564 5f30 6469 6d20 3d3d 2061  _fixed_0dim == a
-00013440: 7363 6969 0a20 2020 2020 2020 2061 7373  scii.        ass
-00013450: 6572 7420 6473 2e61 7363 6969 5f66 6978  ert ds.ascii_fix
-00013460: 6564 5f31 6469 6d20 3d3d 2061 7363 6969  ed_1dim == ascii
-00013470: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00013480: 6473 2e61 7363 6969 5f66 6978 6564 5f61  ds.ascii_fixed_a
-00013490: 7272 6179 203d 3d20 5b61 7363 6969 2c20  rray == [ascii, 
-000134a0: 2266 6f6f 6261 7222 5d0a 0a20 2020 2020  "foobar"]..     
-000134b0: 2020 2061 7373 6572 7420 6473 2e62 7974     assert ds.byt
-000134c0: 6573 5f66 6978 6564 203d 3d20 6173 6369  es_fixed == asci
-000134d0: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
-000134e0: 2064 732e 6279 7465 735f 6669 7865 645f   ds.bytes_fixed_
-000134f0: 3064 696d 203d 3d20 6173 6369 690a 2020  0dim == ascii.  
-00013500: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-00013510: 6279 7465 735f 6669 7865 645f 3164 696d  bytes_fixed_1dim
-00013520: 203d 3d20 6173 6369 690a 2020 2020 2020   == ascii.      
-00013530: 2020 6173 7365 7274 2064 732e 6279 7465    assert ds.byte
-00013540: 735f 6669 7865 645f 6172 7261 7920 3d3d  s_fixed_array ==
-00013550: 205b 6173 6369 692c 2022 666f 6f62 6172   [ascii, "foobar
-00013560: 225d 0a0a 2020 2020 2020 2020 6173 7365  "]..        asse
-00013570: 7274 2064 732e 696e 7420 3d3d 2031 0a20  rt ds.int == 1. 
-00013580: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-00013590: 2e69 6e74 6c69 7374 203d 3d20 310a 2020  .intlist == 1.  
-000135a0: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
-000135b0: 2e61 7373 6572 745f 6571 7561 6c28 6473  .assert_equal(ds
-000135c0: 2e69 6e74 5f61 7272 6179 2c20 6e70 2e61  .int_array, np.a
-000135d0: 7261 6e67 6528 3130 2929 0a20 2020 2020  range(10)).     
-000135e0: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
-000135f0: 7365 7274 5f65 7175 616c 2864 732e 6174  sert_equal(ds.at
-00013600: 7472 735b 2265 6d70 7479 5f6c 6973 7422  trs["empty_list"
-00013610: 5d2c 206e 702e 6172 7261 7928 5b5d 2929  ], np.array([]))
-00013620: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
-00013630: 696e 672e 6173 7365 7274 5f65 7175 616c  ing.assert_equal
-00013640: 2864 732e 6174 7472 735b 2265 6d70 7479  (ds.attrs["empty
-00013650: 5f61 7272 6179 225d 2c20 6e70 2e61 7272  _array"], np.arr
-00013660: 6179 285b 5d29 290a 0a20 2020 2077 6974  ay([]))..    wit
-00013670: 6820 6e65 7443 4446 342e 4461 7461 7365  h netCDF4.Datase
-00013680: 7428 746d 705f 6c6f 6361 6c5f 6e65 7463  t(tmp_local_netc
-00013690: 6466 2c20 6d6f 6465 3d22 7222 2920 6173  df, mode="r") as
-000136a0: 2064 733a 0a20 2020 2020 2020 2061 7373   ds:.        ass
-000136b0: 6572 7420 6473 2e75 6e69 636f 6465 203d  ert ds.unicode =
-000136c0: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-000136d0: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-000136e0: 6f64 655f 3064 696d 203d 3d20 756e 6963  ode_0dim == unic
-000136f0: 6f64 650a 2020 2020 2020 2020 6173 7365  ode.        asse
-00013700: 7274 2064 732e 756e 6963 6f64 655f 3164  rt ds.unicode_1d
-00013710: 696d 203d 3d20 756e 6963 6f64 650a 2020  im == unicode.  
-00013720: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-00013730: 756e 6963 6f64 655f 6172 7261 7279 203d  unicode_arrary =
-00013740: 3d20 5b75 6e69 636f 6465 2c20 2266 6f6f  = [unicode, "foo
-00013750: 62c3 a172 225d 0a20 2020 2020 2020 2061  b..r"].        a
-00013760: 7373 6572 7420 6473 2e75 6e69 636f 6465  ssert ds.unicode
-00013770: 5f6c 6973 7420 3d3d 2075 6e69 636f 6465  _list == unicode
-00013780: 0a0a 2020 2020 2020 2020 6173 6369 6920  ..        ascii 
-00013790: 3d20 2261 7363 6969 220a 2020 2020 2020  = "ascii".      
-000137a0: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
-000137b0: 6920 3d3d 2061 7363 6969 0a20 2020 2020  i == ascii.     
-000137c0: 2020 2061 7373 6572 7420 6473 2e61 7363     assert ds.asc
-000137d0: 6969 5f30 6469 6d20 3d3d 2061 7363 6969  ii_0dim == ascii
-000137e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000137f0: 6473 2e61 7363 6969 5f31 6469 6d20 3d3d  ds.ascii_1dim ==
-00013800: 2061 7363 6969 0a20 2020 2020 2020 2061   ascii.        a
-00013810: 7373 6572 7420 6473 2e61 7363 6969 5f61  ssert ds.ascii_a
-00013820: 7272 6179 203d 3d20 5b61 7363 6969 2c20  rray == [ascii, 
-00013830: 2266 6f6f 6261 7222 5d0a 2020 2020 2020  "foobar"].      
-00013840: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
-00013850: 695f 6c69 7374 203d 3d20 6173 6369 690a  i_list == ascii.
-00013860: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00013870: 6473 2e62 7974 6573 203d 3d20 6173 6369  ds.bytes == asci
-00013880: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
-00013890: 2064 732e 6279 7465 735f 3064 696d 203d   ds.bytes_0dim =
-000138a0: 3d20 6173 6369 690a 2020 2020 2020 2020  = ascii.        
-000138b0: 6173 7365 7274 2064 732e 6279 7465 735f  assert ds.bytes_
-000138c0: 3164 696d 203d 3d20 6173 6369 690a 2020  1dim == ascii.  
-000138d0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
-000138e0: 6279 7465 735f 6172 7261 7920 3d3d 205b  bytes_array == [
-000138f0: 6173 6369 692c 2022 666f 6f62 6172 225d  ascii, "foobar"]
-00013900: 0a20 2020 2020 2020 2023 2077 7269 7469  .        # writi
-00013910: 6e67 2f72 6561 6469 6e67 206c 6973 7473  ng/reading lists
-00013920: 2069 7320 6272 6f6b 656e 2077 6974 6820   is broken with 
-00013930: 6835 7079 322f 6e65 7443 4446 340a 2020  h5py2/netCDF4.  
-00013940: 2020 2020 2020 6966 2076 6572 7369 6f6e        if version
-00013950: 2e70 6172 7365 2868 3570 792e 5f5f 7665  .parse(h5py.__ve
-00013960: 7273 696f 6e5f 5f29 203e 3d20 7665 7273  rsion__) >= vers
-00013970: 696f 6e2e 7061 7273 6528 2233 2e30 2e30  ion.parse("3.0.0
-00013980: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00013990: 6173 7365 7274 2064 732e 6279 7465 735f  assert ds.bytes_
-000139a0: 6c69 7374 203d 3d20 6173 6369 690a 0a20  list == ascii.. 
-000139b0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-000139c0: 2e75 6e69 636f 6465 5f66 6978 6564 203d  .unicode_fixed =
-000139d0: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-000139e0: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-000139f0: 6f64 655f 6669 7865 645f 3064 696d 203d  ode_fixed_0dim =
-00013a00: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-00013a10: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-00013a20: 6f64 655f 6669 7865 645f 3164 696d 203d  ode_fixed_1dim =
-00013a30: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
-00013a40: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
-00013a50: 6f64 655f 6669 7865 645f 6172 7261 7279  ode_fixed_arrary
-00013a60: 203d 3d20 5b75 6e69 636f 6465 2c20 2266   == [unicode, "f
-00013a70: 6f6f 62c3 a172 225d 0a0a 2020 2020 2020  oob..r"]..      
-00013a80: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
-00013a90: 695f 6669 7865 6420 3d3d 2061 7363 6969  i_fixed == ascii
-00013aa0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00013ab0: 6473 2e61 7363 6969 5f66 6978 6564 5f30  ds.ascii_fixed_0
-00013ac0: 6469 6d20 3d3d 2061 7363 6969 0a20 2020  dim == ascii.   
-00013ad0: 2020 2020 2061 7373 6572 7420 6473 2e61       assert ds.a
-00013ae0: 7363 6969 5f66 6978 6564 5f31 6469 6d20  scii_fixed_1dim 
-00013af0: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
-00013b00: 2061 7373 6572 7420 6473 2e61 7363 6969   assert ds.ascii
-00013b10: 5f66 6978 6564 5f61 7272 6179 203d 3d20  _fixed_array == 
-00013b20: 5b61 7363 6969 2c20 2266 6f6f 6261 7222  [ascii, "foobar"
-00013b30: 5d0a 0a20 2020 2020 2020 2061 7373 6572  ]..        asser
-00013b40: 7420 6473 2e62 7974 6573 5f66 6978 6564  t ds.bytes_fixed
-00013b50: 203d 3d20 6173 6369 690a 2020 2020 2020   == ascii.      
-00013b60: 2020 6173 7365 7274 2064 732e 6279 7465    assert ds.byte
-00013b70: 735f 6669 7865 645f 3064 696d 203d 3d20  s_fixed_0dim == 
-00013b80: 6173 6369 690a 2020 2020 2020 2020 6173  ascii.        as
-00013b90: 7365 7274 2064 732e 6279 7465 735f 6669  sert ds.bytes_fi
-00013ba0: 7865 645f 3164 696d 203d 3d20 6173 6369  xed_1dim == asci
-00013bb0: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
-00013bc0: 2064 732e 6279 7465 735f 6669 7865 645f   ds.bytes_fixed_
-00013bd0: 6172 7261 7920 3d3d 205b 6173 6369 692c  array == [ascii,
-00013be0: 2022 666f 6f62 6172 225d 0a0a 2020 2020   "foobar"]..    
-00013bf0: 2020 2020 6173 7365 7274 2064 732e 696e      assert ds.in
-00013c00: 7420 3d3d 2031 0a20 2020 2020 2020 2061  t == 1.        a
-00013c10: 7373 6572 7420 6473 2e69 6e74 6c69 7374  ssert ds.intlist
-00013c20: 203d 3d20 310a 2020 2020 2020 2020 6e70   == 1.        np
-00013c30: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
-00013c40: 6571 7561 6c28 6473 2e69 6e74 5f61 7272  equal(ds.int_arr
-00013c50: 6179 2c20 6e70 2e61 7261 6e67 6528 3130  ay, np.arange(10
-00013c60: 2929 0a20 2020 2020 2020 206e 702e 7465  )).        np.te
-00013c70: 7374 696e 672e 6173 7365 7274 5f65 7175  sting.assert_equ
-00013c80: 616c 2864 732e 656d 7074 795f 6c69 7374  al(ds.empty_list
-00013c90: 2c20 6e70 2e61 7272 6179 285b 5d29 290a  , np.array([])).
-00013ca0: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
-00013cb0: 6e67 2e61 7373 6572 745f 6571 7561 6c28  ng.assert_equal(
-00013cc0: 6473 2e65 6d70 7479 5f61 7272 6179 2c20  ds.empty_array, 
-00013cd0: 6e70 2e61 7272 6179 285b 5d29 290a 0a0a  np.array([]))...
-00013ce0: 4070 7974 6573 742e 6d61 726b 2e73 6b69  @pytest.mark.ski
-00013cf0: 7069 6628 0a20 2020 2076 6572 7369 6f6e  pif(.    version
-00013d00: 2e70 6172 7365 2868 3570 792e 5f5f 7665  .parse(h5py.__ve
-00013d10: 7273 696f 6e5f 5f29 203c 2076 6572 7369  rsion__) < versi
-00013d20: 6f6e 2e70 6172 7365 2822 332e 372e 3022  on.parse("3.7.0"
-00013d30: 292c 0a20 2020 2072 6561 736f 6e3d 2264  ),.    reason="d
-00013d40: 6f65 7320 6e6f 7420 776f 726b 2077 6974  oes not work wit
-00013d50: 6820 6835 7079 203c 2033 2e37 2e30 222c  h h5py < 3.7.0",
-00013d60: 0a29 0a64 6566 2074 6573 745f 766c 656e  .).def test_vlen
-00013d70: 5f73 7472 696e 675f 6461 7461 7365 745f  _string_dataset_
-00013d80: 6669 6c6c 7661 6c75 6528 746d 705f 6c6f  fillvalue(tmp_lo
-00013d90: 6361 6c5f 6e65 7463 6466 2c20 6465 636f  cal_netcdf, deco
-00013da0: 6465 5f76 6c65 6e5f 7374 7269 6e67 7329  de_vlen_strings)
-00013db0: 3a0a 2020 2020 2320 6368 6563 6b20 5f46  :.    # check _F
-00013dc0: 696c 6c56 616c 7565 2066 6f72 2056 4c45  illValue for VLE
-00013dd0: 4e20 7374 7269 6e67 2064 6174 6173 6574  N string dataset
-00013de0: 730a 2020 2020 2320 6f6e 6c79 2077 6f72  s.    # only wor
-00013df0: 6b73 2066 6f72 2068 3570 7920 3e3d 2033  ks for h5py >= 3
-00013e00: 2e37 2e30 0a0a 2020 2020 2320 6669 7273  .7.0..    # firs
-00013e10: 7420 7769 7468 206e 6577 2041 5049 0a20  t with new API. 
-00013e20: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
-00013e30: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
-00013e40: 6e65 7463 6466 2c20 2277 2229 2061 7320  netcdf, "w") as 
-00013e50: 6473 3a0a 2020 2020 2020 2020 6473 2e64  ds:.        ds.d
-00013e60: 696d 656e 7369 6f6e 7320 3d20 7b22 7374  imensions = {"st
-00013e70: 7269 6e67 223a 2031 307d 0a20 2020 2020  ring": 10}.     
-00013e80: 2020 2064 7430 203d 2068 3570 792e 7374     dt0 = h5py.st
-00013e90: 7269 6e67 5f64 7479 7065 2829 0a20 2020  ring_dtype().   
-00013ea0: 2020 2020 2066 696c 6c5f 7661 6c75 6530       fill_value0
-00013eb0: 203d 2022 62c3 a172 220a 2020 2020 2020   = "b..r".      
-00013ec0: 2020 6473 2e63 7265 6174 655f 7661 7269    ds.create_vari
-00013ed0: 6162 6c65 2822 7830 222c 2028 2273 7472  able("x0", ("str
-00013ee0: 696e 6722 2c29 2c20 6474 7970 653d 6474  ing",), dtype=dt
-00013ef0: 302c 2066 696c 6c76 616c 7565 3d66 696c  0, fillvalue=fil
-00013f00: 6c5f 7661 6c75 6530 290a 2020 2020 2020  l_value0).      
-00013f10: 2020 6474 3120 3d20 6835 7079 2e73 7472    dt1 = h5py.str
-00013f20: 696e 675f 6474 7970 6528 2261 7363 6969  ing_dtype("ascii
-00013f30: 2229 0a20 2020 2020 2020 2066 696c 6c5f  ").        fill_
-00013f40: 7661 6c75 6531 203d 2022 6261 7222 0a20  value1 = "bar". 
-00013f50: 2020 2020 2020 2064 732e 6372 6561 7465         ds.create
-00013f60: 5f76 6172 6961 626c 6528 2278 3122 2c20  _variable("x1", 
-00013f70: 2822 7374 7269 6e67 222c 292c 2064 7479  ("string",), dty
-00013f80: 7065 3d64 7431 2c20 6669 6c6c 7661 6c75  pe=dt1, fillvalu
-00013f90: 653d 6669 6c6c 5f76 616c 7565 3129 0a0a  e=fill_value1)..
-00013fa0: 2020 2020 2320 6368 6563 6b2c 2069 6620      # check, if 
-00013fb0: 6e65 7720 4150 4920 6361 6e20 7265 6164  new API can read
-00013fc0: 2074 6865 6d0a 2020 2020 7769 7468 2068   them.    with h
-00013fd0: 356e 6574 6364 662e 4669 6c65 2874 6d70  5netcdf.File(tmp
-00013fe0: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
-00013ff0: 7222 2c20 2a2a 6465 636f 6465 5f76 6c65  r", **decode_vle
-00014000: 6e5f 7374 7269 6e67 7329 2061 7320 6473  n_strings) as ds
-00014010: 3a0a 2020 2020 2020 2020 6465 636f 6465  :.        decode
-00014020: 5f76 6c65 6e20 3d20 6465 636f 6465 5f76  _vlen = decode_v
-00014030: 6c65 6e5f 7374 7269 6e67 735b 2264 6563  len_strings["dec
-00014040: 6f64 655f 766c 656e 5f73 7472 696e 6773  ode_vlen_strings
-00014050: 225d 0a20 2020 2020 2020 2066 7661 6c75  "].        fvalu
-00014060: 6530 203d 2066 696c 6c5f 7661 6c75 6530  e0 = fill_value0
-00014070: 2069 6620 6465 636f 6465 5f76 6c65 6e20   if decode_vlen 
-00014080: 656c 7365 2066 696c 6c5f 7661 6c75 6530  else fill_value0
-00014090: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-000140a0: 0a20 2020 2020 2020 2066 7661 6c75 6531  .        fvalue1
-000140b0: 203d 2066 696c 6c5f 7661 6c75 6531 2069   = fill_value1 i
-000140c0: 6620 6465 636f 6465 5f76 6c65 6e20 656c  f decode_vlen el
-000140d0: 7365 2066 696c 6c5f 7661 6c75 6531 2e65  se fill_value1.e
-000140e0: 6e63 6f64 6528 2275 7466 2d38 2229 0a20  ncode("utf-8"). 
-000140f0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
-00014100: 5b22 7830 225d 5b30 5d20 3d3d 2066 7661  ["x0"][0] == fva
-00014110: 6c75 6530 0a20 2020 2020 2020 2061 7373  lue0.        ass
-00014120: 6572 7420 6473 5b22 7830 225d 2e61 7474  ert ds["x0"].att
-00014130: 7273 5b22 5f46 696c 6c56 616c 7565 225d  rs["_FillValue"]
-00014140: 203d 3d20 6669 6c6c 5f76 616c 7565 300a   == fill_value0.
-00014150: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00014160: 735b 2278 3122 5d5b 305d 203d 3d20 6676  s["x1"][0] == fv
-00014170: 616c 7565 310a 2020 2020 2020 2020 6173  alue1.        as
-00014180: 7365 7274 2064 735b 2278 3122 5d2e 6174  sert ds["x1"].at
-00014190: 7472 735b 225f 4669 6c6c 5661 6c75 6522  trs["_FillValue"
-000141a0: 5d20 3d3d 2066 696c 6c5f 7661 6c75 6531  ] == fill_value1
-000141b0: 0a0a 2020 2020 2320 6368 6563 6b20 6966  ..    # check if
-000141c0: 206c 6567 6163 7961 7069 2063 616e 2072   legacyapi can r
-000141d0: 6561 6420 7468 656d 0a20 2020 2077 6974  ead them.    wit
-000141e0: 6820 6c65 6761 6379 6170 692e 4461 7461  h legacyapi.Data
-000141f0: 7365 7428 746d 705f 6c6f 6361 6c5f 6e65  set(tmp_local_ne
-00014200: 7463 6466 2c20 2272 2229 2061 7320 6473  tcdf, "r") as ds
-00014210: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
-00014220: 2064 735b 2278 3022 5d5b 305d 203d 3d20   ds["x0"][0] == 
-00014230: 6669 6c6c 5f76 616c 7565 300a 2020 2020  fill_value0.    
-00014240: 2020 2020 6173 7365 7274 2064 735b 2278      assert ds["x
-00014250: 3022 5d2e 5f46 696c 6c56 616c 7565 203d  0"]._FillValue =
-00014260: 3d20 6669 6c6c 5f76 616c 7565 300a 2020  = fill_value0.  
-00014270: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
-00014280: 2278 3122 5d5b 305d 203d 3d20 6669 6c6c  "x1"][0] == fill
-00014290: 5f76 616c 7565 310a 2020 2020 2020 2020  _value1.        
-000142a0: 6173 7365 7274 2064 735b 2278 3122 5d2e  assert ds["x1"].
-000142b0: 5f46 696c 6c56 616c 7565 203d 3d20 6669  _FillValue == fi
-000142c0: 6c6c 5f76 616c 7565 310a 0a20 2020 2023  ll_value1..    #
-000142d0: 2063 6865 636b 2069 6620 6e65 7443 4446   check if netCDF
-000142e0: 342d 7079 7468 6f6e 2063 616e 2072 6561  4-python can rea
-000142f0: 6420 7468 656d 0a20 2020 2077 6974 6820  d them.    with 
-00014300: 6e65 7443 4446 342e 4461 7461 7365 7428  netCDF4.Dataset(
-00014310: 746d 705f 6c6f 6361 6c5f 6e65 7463 6466  tmp_local_netcdf
-00014320: 2c20 2272 2229 2061 7320 6473 3a0a 2020  , "r") as ds:.  
-00014330: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
-00014340: 2278 3022 5d5b 305d 203d 3d20 6669 6c6c  "x0"][0] == fill
-00014350: 5f76 616c 7565 300a 2020 2020 2020 2020  _value0.        
-00014360: 6173 7365 7274 2064 735b 2278 3022 5d2e  assert ds["x0"].
-00014370: 5f46 696c 6c56 616c 7565 203d 3d20 6669  _FillValue == fi
-00014380: 6c6c 5f76 616c 7565 300a 2020 2020 2020  ll_value0.      
-00014390: 2020 6173 7365 7274 2064 735b 2278 3122    assert ds["x1"
-000143a0: 5d5b 305d 203d 3d20 6669 6c6c 5f76 616c  ][0] == fill_val
-000143b0: 7565 310a 2020 2020 2020 2020 6173 7365  ue1.        asse
-000143c0: 7274 2064 735b 2278 3122 5d2e 5f46 696c  rt ds["x1"]._Fil
-000143d0: 6c56 616c 7565 203d 3d20 6669 6c6c 5f76  lValue == fill_v
-000143e0: 616c 7565 310a 0a20 2020 2023 2073 6563  alue1..    # sec
-000143f0: 6f6e 6420 7769 7468 206c 6567 6163 7961  ond with legacya
-00014400: 7069 0a20 2020 2077 6974 6820 6c65 6761  pi.    with lega
-00014410: 6379 6170 692e 4461 7461 7365 7428 746d  cyapi.Dataset(tm
-00014420: 705f 6c6f 6361 6c5f 6e65 7463 6466 2c20  p_local_netcdf, 
-00014430: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
-00014440: 2020 2020 6473 2e63 7265 6174 6544 696d      ds.createDim
-00014450: 656e 7369 6f6e 2822 7374 7269 6e67 222c  ension("string",
-00014460: 2031 3029 0a20 2020 2020 2020 2066 696c   10).        fil
-00014470: 6c5f 7661 6c75 6530 203d 2022 62c3 a172  l_value0 = "b..r
-00014480: 220a 2020 2020 2020 2020 6473 2e63 7265  ".        ds.cre
-00014490: 6174 6556 6172 6961 626c 6528 2278 3022  ateVariable("x0"
-000144a0: 2c20 7374 722c 2028 2273 7472 696e 6722  , str, ("string"
-000144b0: 2c29 2c20 6669 6c6c 5f76 616c 7565 3d66  ,), fill_value=f
-000144c0: 696c 6c5f 7661 6c75 6530 290a 2020 2020  ill_value0).    
-000144d0: 2020 2020 6669 6c6c 5f76 616c 7565 3120      fill_value1 
-000144e0: 3d20 2262 6172 220a 2020 2020 2020 2020  = "bar".        
-000144f0: 6473 2e63 7265 6174 6556 6172 6961 626c  ds.createVariabl
-00014500: 6528 2278 3122 2c20 7374 722c 2028 2273  e("x1", str, ("s
-00014510: 7472 696e 6722 2c29 2c20 6669 6c6c 5f76  tring",), fill_v
-00014520: 616c 7565 3d66 696c 6c5f 7661 6c75 6531  alue=fill_value1
-00014530: 290a 0a20 2020 2023 2063 6865 636b 2069  )..    # check i
-00014540: 6620 6e65 7720 4150 4920 6361 6e20 7265  f new API can re
-00014550: 6164 2074 6865 6d0a 2020 2020 7769 7468  ad them.    with
-00014560: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
-00014570: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
-00014580: 2022 7222 2c20 2a2a 6465 636f 6465 5f76   "r", **decode_v
-00014590: 6c65 6e5f 7374 7269 6e67 7329 2061 7320  len_strings) as 
-000145a0: 6473 3a0a 2020 2020 2020 2020 6465 636f  ds:.        deco
-000145b0: 6465 5f76 6c65 6e20 3d20 6465 636f 6465  de_vlen = decode
-000145c0: 5f76 6c65 6e5f 7374 7269 6e67 735b 2264  _vlen_strings["d
-000145d0: 6563 6f64 655f 766c 656e 5f73 7472 696e  ecode_vlen_strin
-000145e0: 6773 225d 0a20 2020 2020 2020 2066 7661  gs"].        fva
-000145f0: 6c75 6530 203d 2066 696c 6c5f 7661 6c75  lue0 = fill_valu
-00014600: 6530 2069 6620 6465 636f 6465 5f76 6c65  e0 if decode_vle
-00014610: 6e20 656c 7365 2066 696c 6c5f 7661 6c75  n else fill_valu
-00014620: 6530 2e65 6e63 6f64 6528 2275 7466 2d38  e0.encode("utf-8
-00014630: 2229 0a20 2020 2020 2020 2066 7661 6c75  ").        fvalu
-00014640: 6531 203d 2066 696c 6c5f 7661 6c75 6531  e1 = fill_value1
-00014650: 2069 6620 6465 636f 6465 5f76 6c65 6e20   if decode_vlen 
-00014660: 656c 7365 2066 696c 6c5f 7661 6c75 6531  else fill_value1
-00014670: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-00014680: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00014690: 6473 5b22 7830 225d 5b30 5d20 3d3d 2066  ds["x0"][0] == f
-000146a0: 7661 6c75 6530 0a20 2020 2020 2020 2061  value0.        a
-000146b0: 7373 6572 7420 6473 5b22 7830 225d 2e61  ssert ds["x0"].a
-000146c0: 7474 7273 5b22 5f46 696c 6c56 616c 7565  ttrs["_FillValue
-000146d0: 225d 203d 3d20 6669 6c6c 5f76 616c 7565  "] == fill_value
-000146e0: 300a 2020 2020 2020 2020 6173 7365 7274  0.        assert
-000146f0: 2064 735b 2278 3122 5d5b 305d 203d 3d20   ds["x1"][0] == 
-00014700: 6676 616c 7565 310a 2020 2020 2020 2020  fvalue1.        
-00014710: 6173 7365 7274 2064 735b 2278 3122 5d2e  assert ds["x1"].
-00014720: 6174 7472 735b 225f 4669 6c6c 5661 6c75  attrs["_FillValu
-00014730: 6522 5d20 3d3d 2066 696c 6c5f 7661 6c75  e"] == fill_valu
-00014740: 6531 0a0a 2020 2020 2320 6368 6563 6b20  e1..    # check 
-00014750: 6966 206c 6567 6163 7961 7069 2063 616e  if legacyapi can
-00014760: 2072 6561 6420 7468 656d 0a20 2020 2077   read them.    w
-00014770: 6974 6820 6c65 6761 6379 6170 692e 4461  ith legacyapi.Da
-00014780: 7461 7365 7428 746d 705f 6c6f 6361 6c5f  taset(tmp_local_
-00014790: 6e65 7463 6466 2c20 2272 2229 2061 7320  netcdf, "r") as 
-000147a0: 6473 3a0a 2020 2020 2020 2020 6173 7365  ds:.        asse
-000147b0: 7274 2064 735b 2278 3022 5d5b 305d 203d  rt ds["x0"][0] =
-000147c0: 3d20 6669 6c6c 5f76 616c 7565 300a 2020  = fill_value0.  
-000147d0: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
-000147e0: 2278 3022 5d2e 5f46 696c 6c56 616c 7565  "x0"]._FillValue
-000147f0: 203d 3d20 6669 6c6c 5f76 616c 7565 300a   == fill_value0.
-00014800: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-00014810: 735b 2278 3122 5d5b 305d 203d 3d20 6669  s["x1"][0] == fi
-00014820: 6c6c 5f76 616c 7565 310a 2020 2020 2020  ll_value1.      
-00014830: 2020 6173 7365 7274 2064 735b 2278 3122    assert ds["x1"
-00014840: 5d2e 5f46 696c 6c56 616c 7565 203d 3d20  ]._FillValue == 
-00014850: 6669 6c6c 5f76 616c 7565 310a 0a20 2020  fill_value1..   
-00014860: 2023 2063 6865 636b 2069 6620 6e65 7443   # check if netC
-00014870: 4446 342d 7079 7468 6f6e 2063 616e 2072  DF4-python can r
-00014880: 6561 6420 7468 656d 0a20 2020 2077 6974  ead them.    wit
-00014890: 6820 6e65 7443 4446 342e 4461 7461 7365  h netCDF4.Datase
-000148a0: 7428 746d 705f 6c6f 6361 6c5f 6e65 7463  t(tmp_local_netc
-000148b0: 6466 2c20 2272 2229 2061 7320 6473 3a0a  df, "r") as ds:.
-000148c0: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-000148d0: 735b 2278 3022 5d5b 305d 203d 3d20 6669  s["x0"][0] == fi
-000148e0: 6c6c 5f76 616c 7565 300a 2020 2020 2020  ll_value0.      
-000148f0: 2020 6173 7365 7274 2064 735b 2278 3022    assert ds["x0"
-00014900: 5d2e 5f46 696c 6c56 616c 7565 203d 3d20  ]._FillValue == 
-00014910: 6669 6c6c 5f76 616c 7565 300a 2020 2020  fill_value0.    
-00014920: 2020 2020 6173 7365 7274 2064 735b 2278      assert ds["x
-00014930: 3122 5d5b 305d 203d 3d20 6669 6c6c 5f76  1"][0] == fill_v
-00014940: 616c 7565 310a 2020 2020 2020 2020 6173  alue1.        as
-00014950: 7365 7274 2064 735b 2278 3122 5d2e 5f46  sert ds["x1"]._F
-00014960: 696c 6c56 616c 7565 203d 3d20 6669 6c6c  illValue == fill
-00014970: 5f76 616c 7565 310a                      _value1.
+00011a60: 7265 6174 6556 6172 6961 626c 6528 2274  reateVariable("t
+00011a70: 6573 7422 2c20 666c 6f61 742c 2028 2278  est", float, ("x
+00011a80: 222c 2022 7922 2929 0a20 2020 2020 2020  ", "y")).       
+00011a90: 2076 6172 203d 2064 7330 5b22 6772 6f75   var = ds0["grou
+00011aa0: 7030 3022 5d2e 6372 6561 7465 5661 7269  p00"].createVari
+00011ab0: 6162 6c65 2822 7822 2c20 666c 6f61 742c  able("x", float,
+00011ac0: 2028 2278 222c 2022 7922 2929 0a20 2020   ("x", "y")).   
+00011ad0: 2020 2020 2076 6172 5b3a 5d20 3d20 6e70       var[:] = np
+00011ae0: 2e6f 6e65 7328 2831 302c 2032 3029 290a  .ones((10, 20)).
+00011af0: 0a20 2020 2077 6974 6820 6c65 6761 6379  .    with legacy
+00011b00: 6170 692e 4461 7461 7365 7428 746d 7064  api.Dataset(tmpd
+00011b10: 6972 2e6a 6f69 6e28 2274 6573 745f 6c65  ir.join("test_le
+00011b20: 6761 6379 2e6e 6322 292c 206d 6f64 653d  gacy.nc"), mode=
+00011b30: 2277 2229 2061 7320 6473 3a0a 2020 2020  "w") as ds:.    
+00011b40: 2020 2020 6473 3020 3d20 6473 0a20 2020      ds0 = ds.   
+00011b50: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00011b60: 6e67 6528 3130 293a 0a20 2020 2020 2020  nge(10):.       
+00011b70: 2020 2020 2064 7320 3d20 6473 2e63 7265       ds = ds.cre
+00011b80: 6174 6547 726f 7570 2866 2267 726f 7570  ateGroup(f"group
+00011b90: 7b69 3a30 3264 7d22 290a 2020 2020 2020  {i:02d}").      
+00011ba0: 2020 6473 302e 6372 6561 7465 4469 6d65    ds0.createDime
+00011bb0: 6e73 696f 6e28 2278 222c 2031 3029 0a20  nsion("x", 10). 
+00011bc0: 2020 2020 2020 2064 7330 2e63 7265 6174         ds0.creat
+00011bd0: 6544 696d 656e 7369 6f6e 2822 7922 2c20  eDimension("y", 
+00011be0: 3230 290a 2020 2020 2020 2020 6473 305b  20).        ds0[
+00011bf0: 2267 726f 7570 3030 225d 2e63 7265 6174  "group00"].creat
+00011c00: 6556 6172 6961 626c 6528 2274 6573 7422  eVariable("test"
+00011c10: 2c20 666c 6f61 742c 2028 2278 222c 2022  , float, ("x", "
+00011c20: 7922 2929 0a20 2020 2020 2020 2076 6172  y")).        var
+00011c30: 203d 2064 7330 5b22 6772 6f75 7030 3022   = ds0["group00"
+00011c40: 5d2e 6372 6561 7465 5661 7269 6162 6c65  ].createVariable
+00011c50: 2822 7822 2c20 666c 6f61 742c 2028 2278  ("x", float, ("x
+00011c60: 222c 2022 7922 2929 0a20 2020 2020 2020  ", "y")).       
+00011c70: 2076 6172 5b3a 5d20 3d20 6e70 2e6f 6e65   var[:] = np.one
+00011c80: 7328 2831 302c 2032 3029 290a 0a20 2020  s((10, 20))..   
+00011c90: 2077 6974 6820 6835 6e65 7463 6466 2e46   with h5netcdf.F
+00011ca0: 696c 6528 746d 7064 6972 2e6a 6f69 6e28  ile(tmpdir.join(
+00011cb0: 2274 6573 745f 6e65 7463 6466 2e6e 6322  "test_netcdf.nc"
+00011cc0: 292c 206d 6f64 653d 2272 2229 2061 7320  ), mode="r") as 
+00011cd0: 6473 303a 0a20 2020 2020 2020 2077 6974  ds0:.        wit
+00011ce0: 6820 6835 6e65 7463 6466 2e46 696c 6528  h h5netcdf.File(
+00011cf0: 746d 7064 6972 2e6a 6f69 6e28 2274 6573  tmpdir.join("tes
+00011d00: 745f 6c65 6761 6379 2e6e 6322 292c 206d  t_legacy.nc"), m
+00011d10: 6f64 653d 2272 2229 2061 7320 6473 313a  ode="r") as ds1:
+00011d20: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+00011d30: 6572 7420 7265 7072 2864 7330 2e64 696d  ert repr(ds0.dim
+00011d40: 656e 7369 6f6e 735b 2278 225d 2920 3d3d  ensions["x"]) ==
+00011d50: 2072 6570 7228 6473 312e 6469 6d65 6e73   repr(ds1.dimens
+00011d60: 696f 6e73 5b22 7822 5d29 0a20 2020 2020  ions["x"]).     
+00011d70: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+00011d80: 7072 2864 7330 2e64 696d 656e 7369 6f6e  pr(ds0.dimension
+00011d90: 735b 2279 225d 2920 3d3d 2072 6570 7228  s["y"]) == repr(
+00011da0: 6473 312e 6469 6d65 6e73 696f 6e73 5b22  ds1.dimensions["
+00011db0: 7922 5d29 0a20 2020 2020 2020 2020 2020  y"]).           
+00011dc0: 2061 7373 6572 7420 7265 7072 2864 7330   assert repr(ds0
+00011dd0: 5b22 6772 6f75 7030 3022 5d29 203d 3d20  ["group00"]) == 
+00011de0: 7265 7072 2864 7331 5b22 6772 6f75 7030  repr(ds1["group0
+00011df0: 3022 5d29 0a20 2020 2020 2020 2020 2020  0"]).           
+00011e00: 2061 7373 6572 7420 7265 7072 2864 7330   assert repr(ds0
+00011e10: 5b22 6772 6f75 7030 3022 5d5b 2274 6573  ["group00"]["tes
+00011e20: 7422 5d29 203d 3d20 7265 7072 2864 7331  t"]) == repr(ds1
+00011e30: 5b22 6772 6f75 7030 3022 5d5b 2274 6573  ["group00"]["tes
+00011e40: 7422 5d29 0a20 2020 2020 2020 2020 2020  t"]).           
+00011e50: 2061 7373 6572 7420 7265 7072 2864 7330   assert repr(ds0
+00011e60: 5b22 6772 6f75 7030 3022 5d5b 2278 225d  ["group00"]["x"]
+00011e70: 2920 3d3d 2072 6570 7228 6473 315b 2267  ) == repr(ds1["g
+00011e80: 726f 7570 3030 225d 5b22 7822 5d29 0a0a  roup00"]["x"])..
+00011e90: 0a64 6566 2074 6573 745f 6172 7261 795f  .def test_array_
+00011ea0: 6174 7472 6962 7574 6573 2874 6d70 5f6c  attributes(tmp_l
+00011eb0: 6f63 616c 5f6e 6574 6364 6629 3a0a 2020  ocal_netcdf):.  
+00011ec0: 2020 7769 7468 2068 356e 6574 6364 662e    with h5netcdf.
+00011ed0: 4669 6c65 2874 6d70 5f6c 6f63 616c 5f6e  File(tmp_local_n
+00011ee0: 6574 6364 662c 2022 7722 2920 6173 2064  etcdf, "w") as d
+00011ef0: 733a 0a20 2020 2020 2020 2064 7420 3d20  s:.        dt = 
+00011f00: 6835 7079 2e73 7472 696e 675f 6474 7970  h5py.string_dtyp
+00011f10: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00011f20: 2020 2075 6e69 636f 6465 203d 2022 756e     unicode = "un
+00011f30: 6963 6f64 c3a9 220a 2020 2020 2020 2020  icod..".        
+00011f40: 6473 2e61 7474 7273 5b22 756e 6963 6f64  ds.attrs["unicod
+00011f50: 6522 5d20 3d20 756e 6963 6f64 650a 2020  e"] = unicode.  
+00011f60: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
+00011f70: 756e 6963 6f64 655f 3064 696d 225d 203d  unicode_0dim"] =
+00011f80: 206e 702e 6172 7261 7928 756e 6963 6f64   np.array(unicod
+00011f90: 652c 2064 7479 7065 3d64 7429 0a20 2020  e, dtype=dt).   
+00011fa0: 2020 2020 2064 732e 6174 7472 735b 2275       ds.attrs["u
+00011fb0: 6e69 636f 6465 5f31 6469 6d22 5d20 3d20  nicode_1dim"] = 
+00011fc0: 6e70 2e61 7272 6179 285b 756e 6963 6f64  np.array([unicod
+00011fd0: 655d 2c20 6474 7970 653d 6474 290a 2020  e], dtype=dt).  
+00011fe0: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
+00011ff0: 756e 6963 6f64 655f 6172 7261 7279 225d  unicode_arrary"]
+00012000: 203d 206e 702e 6172 7261 7928 5b75 6e69   = np.array([uni
+00012010: 636f 6465 2c20 2266 6f6f 62c3 a172 225d  code, "foob..r"]
+00012020: 2c20 6474 7970 653d 6474 290a 2020 2020  , dtype=dt).    
+00012030: 2020 2020 6473 2e61 7474 7273 5b22 756e      ds.attrs["un
+00012040: 6963 6f64 655f 6c69 7374 225d 203d 205b  icode_list"] = [
+00012050: 756e 6963 6f64 655d 0a0a 2020 2020 2020  unicode]..      
+00012060: 2020 6474 203d 2068 3570 792e 7374 7269    dt = h5py.stri
+00012070: 6e67 5f64 7479 7065 2822 6173 6369 6922  ng_dtype("ascii"
+00012080: 290a 2020 2020 2020 2020 2320 6966 2064  ).        # if d
+00012090: 7479 7065 2069 7320 6173 6369 6920 6974  type is ascii it
+000120a0: 2773 2069 7272 656c 6576 616e 7420 6966  's irrelevant if
+000120b0: 2074 6865 2064 6174 6120 6973 2070 726f   the data is pro
+000120c0: 7669 6465 6420 6173 2062 7974 6573 206f  vided as bytes o
+000120d0: 7220 7374 7269 6e67 0a20 2020 2020 2020  r string.       
+000120e0: 2061 7363 6969 203d 2022 6173 6369 6922   ascii = "ascii"
+000120f0: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
+00012100: 735b 2261 7363 6969 225d 203d 2061 7363  s["ascii"] = asc
+00012110: 6969 0a20 2020 2020 2020 2064 732e 6174  ii.        ds.at
+00012120: 7472 735b 2261 7363 6969 5f30 6469 6d22  trs["ascii_0dim"
+00012130: 5d20 3d20 6e70 2e61 7272 6179 2861 7363  ] = np.array(asc
+00012140: 6969 2c20 6474 7970 653d 6474 290a 2020  ii, dtype=dt).  
+00012150: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
+00012160: 6173 6369 695f 3164 696d 225d 203d 206e  ascii_1dim"] = n
+00012170: 702e 6172 7261 7928 5b61 7363 6969 5d2c  p.array([ascii],
+00012180: 2064 7479 7065 3d64 7429 0a20 2020 2020   dtype=dt).     
+00012190: 2020 2064 732e 6174 7472 735b 2261 7363     ds.attrs["asc
+000121a0: 6969 5f61 7272 6179 225d 203d 206e 702e  ii_array"] = np.
+000121b0: 6172 7261 7928 5b61 7363 6969 2c20 2266  array([ascii, "f
+000121c0: 6f6f 6261 7222 5d2c 2064 7479 7065 3d64  oobar"], dtype=d
+000121d0: 7429 0a20 2020 2020 2020 2064 732e 6174  t).        ds.at
+000121e0: 7472 735b 2261 7363 6969 5f6c 6973 7422  trs["ascii_list"
+000121f0: 5d20 3d20 5b61 7363 6969 5d0a 0a20 2020  ] = [ascii]..   
+00012200: 2020 2020 2061 7363 6969 203d 2062 2261       ascii = b"a
+00012210: 7363 6969 220a 2020 2020 2020 2020 6473  scii".        ds
+00012220: 2e61 7474 7273 5b22 6279 7465 7322 5d20  .attrs["bytes"] 
+00012230: 3d20 6173 6369 690a 2020 2020 2020 2020  = ascii.        
+00012240: 6473 2e61 7474 7273 5b22 6279 7465 735f  ds.attrs["bytes_
+00012250: 3064 696d 225d 203d 206e 702e 6172 7261  0dim"] = np.arra
+00012260: 7928 6173 6369 692c 2064 7479 7065 3d64  y(ascii, dtype=d
+00012270: 7429 0a20 2020 2020 2020 2064 732e 6174  t).        ds.at
+00012280: 7472 735b 2262 7974 6573 5f31 6469 6d22  trs["bytes_1dim"
+00012290: 5d20 3d20 6e70 2e61 7272 6179 285b 6173  ] = np.array([as
+000122a0: 6369 695d 2c20 6474 7970 653d 6474 290a  cii], dtype=dt).
+000122b0: 2020 2020 2020 2020 6473 2e61 7474 7273          ds.attrs
+000122c0: 5b22 6279 7465 735f 6172 7261 7922 5d20  ["bytes_array"] 
+000122d0: 3d20 6e70 2e61 7272 6179 285b 6173 6369  = np.array([asci
+000122e0: 692c 2062 2266 6f6f 6261 7222 5d2c 2064  i, b"foobar"], d
+000122f0: 7479 7065 3d64 7429 0a20 2020 2020 2020  type=dt).       
+00012300: 2064 732e 6174 7472 735b 2262 7974 6573   ds.attrs["bytes
+00012310: 5f6c 6973 7422 5d20 3d20 5b61 7363 6969  _list"] = [ascii
+00012320: 5d0a 0a20 2020 2020 2020 2064 7420 3d20  ]..        dt = 
+00012330: 6835 7079 2e73 7472 696e 675f 6474 7970  h5py.string_dtyp
+00012340: 6528 2275 7466 2d38 222c 2031 3029 0a20  e("utf-8", 10). 
+00012350: 2020 2020 2020 2023 2075 6e69 636f 6465         # unicode
+00012360: 206e 6565 6473 2074 6f20 6265 2065 6e63   needs to be enc
+00012370: 6f64 6564 2070 726f 7065 726c 7920 666f  oded properly fo
+00012380: 7220 6669 7865 6420 7369 7a65 2073 7472  r fixed size str
+00012390: 696e 6720 7479 7065 0a20 2020 2020 2020  ing type.       
+000123a0: 2064 732e 6174 7472 735b 2275 6e69 636f   ds.attrs["unico
+000123b0: 6465 5f66 6978 6564 225d 203d 206e 702e  de_fixed"] = np.
+000123c0: 6172 7261 7928 756e 6963 6f64 652e 656e  array(unicode.en
+000123d0: 636f 6465 2822 7574 662d 3822 292c 2064  code("utf-8"), d
+000123e0: 7479 7065 3d64 7429 0a20 2020 2020 2020  type=dt).       
+000123f0: 2064 732e 6174 7472 735b 2275 6e69 636f   ds.attrs["unico
+00012400: 6465 5f66 6978 6564 5f30 6469 6d22 5d20  de_fixed_0dim"] 
+00012410: 3d20 6e70 2e61 7272 6179 2875 6e69 636f  = np.array(unico
+00012420: 6465 2e65 6e63 6f64 6528 2275 7466 2d38  de.encode("utf-8
+00012430: 2229 2c20 6474 7970 653d 6474 290a 2020  "), dtype=dt).  
+00012440: 2020 2020 2020 6473 2e61 7474 7273 5b22        ds.attrs["
+00012450: 756e 6963 6f64 655f 6669 7865 645f 3164  unicode_fixed_1d
+00012460: 696d 225d 203d 206e 702e 6172 7261 7928  im"] = np.array(
+00012470: 5b75 6e69 636f 6465 2e65 6e63 6f64 6528  [unicode.encode(
+00012480: 2275 7466 2d38 2229 5d2c 2064 7479 7065  "utf-8")], dtype
+00012490: 3d64 7429 0a20 2020 2020 2020 2064 732e  =dt).        ds.
+000124a0: 6174 7472 735b 2275 6e69 636f 6465 5f66  attrs["unicode_f
+000124b0: 6978 6564 5f61 7272 6172 7922 5d20 3d20  ixed_arrary"] = 
+000124c0: 6e70 2e61 7272 6179 280a 2020 2020 2020  np.array(.      
+000124d0: 2020 2020 2020 5b75 6e69 636f 6465 2e65        [unicode.e
+000124e0: 6e63 6f64 6528 2275 7466 2d38 2229 2c20  ncode("utf-8"), 
+000124f0: 2266 6f6f 62c3 a172 222e 656e 636f 6465  "foob..r".encode
+00012500: 2829 5d2c 2064 7479 7065 3d64 740a 2020  ()], dtype=dt.  
+00012510: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00012520: 2064 7420 3d20 6835 7079 2e73 7472 696e   dt = h5py.strin
+00012530: 675f 6474 7970 6528 2261 7363 6969 222c  g_dtype("ascii",
+00012540: 2031 3029 0a20 2020 2020 2020 2061 7363   10).        asc
+00012550: 6969 203d 2022 6173 6369 6922 0a20 2020  ii = "ascii".   
+00012560: 2020 2020 2064 732e 6174 7472 735b 2261       ds.attrs["a
+00012570: 7363 6969 5f66 6978 6564 225d 203d 206e  scii_fixed"] = n
+00012580: 702e 6172 7261 7928 6173 6369 692c 2064  p.array(ascii, d
+00012590: 7479 7065 3d64 7429 0a20 2020 2020 2020  type=dt).       
+000125a0: 2064 732e 6174 7472 735b 2261 7363 6969   ds.attrs["ascii
+000125b0: 5f66 6978 6564 5f30 6469 6d22 5d20 3d20  _fixed_0dim"] = 
+000125c0: 6e70 2e61 7272 6179 2861 7363 6969 2c20  np.array(ascii, 
+000125d0: 6474 7970 653d 6474 290a 2020 2020 2020  dtype=dt).      
+000125e0: 2020 6473 2e61 7474 7273 5b22 6173 6369    ds.attrs["asci
+000125f0: 695f 6669 7865 645f 3164 696d 225d 203d  i_fixed_1dim"] =
+00012600: 206e 702e 6172 7261 7928 5b61 7363 6969   np.array([ascii
+00012610: 5d2c 2064 7479 7065 3d64 7429 0a20 2020  ], dtype=dt).   
+00012620: 2020 2020 2064 732e 6174 7472 735b 2261       ds.attrs["a
+00012630: 7363 6969 5f66 6978 6564 5f61 7272 6179  scii_fixed_array
+00012640: 225d 203d 206e 702e 6172 7261 7928 5b61  "] = np.array([a
+00012650: 7363 6969 2c20 2266 6f6f 6261 7222 5d2c  scii, "foobar"],
+00012660: 2064 7479 7065 3d64 7429 0a0a 2020 2020   dtype=dt)..    
+00012670: 2020 2020 6173 6369 6920 3d20 6222 6173      ascii = b"as
+00012680: 6369 6922 0a20 2020 2020 2020 2064 732e  cii".        ds.
+00012690: 6174 7472 735b 2262 7974 6573 5f66 6978  attrs["bytes_fix
+000126a0: 6564 225d 203d 206e 702e 6172 7261 7928  ed"] = np.array(
+000126b0: 6173 6369 692c 2064 7479 7065 3d64 7429  ascii, dtype=dt)
+000126c0: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
+000126d0: 735b 2262 7974 6573 5f66 6978 6564 5f30  s["bytes_fixed_0
+000126e0: 6469 6d22 5d20 3d20 6e70 2e61 7272 6179  dim"] = np.array
+000126f0: 2861 7363 6969 2c20 6474 7970 653d 6474  (ascii, dtype=dt
+00012700: 290a 2020 2020 2020 2020 6473 2e61 7474  ).        ds.att
+00012710: 7273 5b22 6279 7465 735f 6669 7865 645f  rs["bytes_fixed_
+00012720: 3164 696d 225d 203d 206e 702e 6172 7261  1dim"] = np.arra
+00012730: 7928 5b61 7363 6969 5d2c 2064 7479 7065  y([ascii], dtype
+00012740: 3d64 7429 0a20 2020 2020 2020 2064 732e  =dt).        ds.
+00012750: 6174 7472 735b 2262 7974 6573 5f66 6978  attrs["bytes_fix
+00012760: 6564 5f61 7272 6179 225d 203d 206e 702e  ed_array"] = np.
+00012770: 6172 7261 7928 5b61 7363 6969 2c20 6222  array([ascii, b"
+00012780: 666f 6f62 6172 225d 2c20 6474 7970 653d  foobar"], dtype=
+00012790: 6474 290a 0a20 2020 2020 2020 2064 732e  dt)..        ds.
+000127a0: 6174 7472 735b 2269 6e74 225d 203d 2031  attrs["int"] = 1
+000127b0: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
+000127c0: 735b 2269 6e74 6c69 7374 225d 203d 205b  s["intlist"] = [
+000127d0: 315d 0a20 2020 2020 2020 2064 732e 6174  1].        ds.at
+000127e0: 7472 735b 2269 6e74 5f61 7272 6179 225d  trs["int_array"]
+000127f0: 203d 206e 702e 6172 616e 6765 2831 3029   = np.arange(10)
+00012800: 0a20 2020 2020 2020 2064 732e 6174 7472  .        ds.attr
+00012810: 735b 2265 6d70 7479 5f6c 6973 7422 5d20  s["empty_list"] 
+00012820: 3d20 5b5d 0a20 2020 2020 2020 2064 732e  = [].        ds.
+00012830: 6174 7472 735b 2265 6d70 7479 5f61 7272  attrs["empty_arr
+00012840: 6179 225d 203d 206e 702e 6172 7261 7928  ay"] = np.array(
+00012850: 5b5d 290a 0a20 2020 2077 6974 6820 6835  [])..    with h5
+00012860: 6e65 7463 6466 2e46 696c 6528 746d 705f  netcdf.File(tmp_
+00012870: 6c6f 6361 6c5f 6e65 7463 6466 2c20 6d6f  local_netcdf, mo
+00012880: 6465 3d22 7222 2920 6173 2064 733a 0a20  de="r") as ds:. 
+00012890: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+000128a0: 2e61 7474 7273 5b22 756e 6963 6f64 6522  .attrs["unicode"
+000128b0: 5d20 3d3d 2075 6e69 636f 6465 0a20 2020  ] == unicode.   
+000128c0: 2020 2020 2061 7373 6572 7420 6473 2e61       assert ds.a
+000128d0: 7474 7273 5b22 756e 6963 6f64 655f 3064  ttrs["unicode_0d
+000128e0: 696d 225d 203d 3d20 756e 6963 6f64 650a  im"] == unicode.
+000128f0: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+00012900: 732e 6174 7472 735b 2275 6e69 636f 6465  s.attrs["unicode
+00012910: 5f31 6469 6d22 5d20 3d3d 2075 6e69 636f  _1dim"] == unico
+00012920: 6465 0a20 2020 2020 2020 2061 7373 6572  de.        asser
+00012930: 7420 6473 2e61 7474 7273 5b22 756e 6963  t ds.attrs["unic
+00012940: 6f64 655f 6172 7261 7279 225d 203d 3d20  ode_arrary"] == 
+00012950: 5b75 6e69 636f 6465 2c20 2266 6f6f 62c3  [unicode, "foob.
+00012960: a172 225d 0a20 2020 2020 2020 2061 7373  .r"].        ass
+00012970: 6572 7420 6473 2e61 7474 7273 5b22 756e  ert ds.attrs["un
+00012980: 6963 6f64 655f 6c69 7374 225d 203d 3d20  icode_list"] == 
+00012990: 756e 6963 6f64 650a 0a20 2020 2020 2020  unicode..       
+000129a0: 2023 2062 7974 6573 2061 6e64 2073 7472   # bytes and str
+000129b0: 696e 6773 2061 7265 2072 6563 6569 7665  ings are receive
+000129c0: 6420 6173 2073 7472 696e 6773 2066 6f72  d as strings for
+000129d0: 2068 3570 7933 0a20 2020 2020 2020 2061   h5py3.        a
+000129e0: 7363 6969 203d 2022 6173 6369 6922 0a20  scii = "ascii". 
+000129f0: 2020 2020 2020 2066 6f6f 6261 7220 3d20         foobar = 
+00012a00: 2266 6f6f 6261 7222 0a20 2020 2020 2020  "foobar".       
+00012a10: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
+00012a20: 5b22 6173 6369 6922 5d20 3d3d 2022 6173  ["ascii"] == "as
+00012a30: 6369 6922 0a20 2020 2020 2020 2061 7373  cii".        ass
+00012a40: 6572 7420 6473 2e61 7474 7273 5b22 6173  ert ds.attrs["as
+00012a50: 6369 695f 3064 696d 225d 203d 3d20 6173  cii_0dim"] == as
+00012a60: 6369 690a 2020 2020 2020 2020 6173 7365  cii.        asse
+00012a70: 7274 2064 732e 6174 7472 735b 2261 7363  rt ds.attrs["asc
+00012a80: 6969 5f31 6469 6d22 5d20 3d3d 2061 7363  ii_1dim"] == asc
+00012a90: 6969 0a20 2020 2020 2020 2061 7373 6572  ii.        asser
+00012aa0: 7420 6473 2e61 7474 7273 5b22 6173 6369  t ds.attrs["asci
+00012ab0: 695f 6172 7261 7922 5d20 3d3d 205b 6173  i_array"] == [as
+00012ac0: 6369 692c 2066 6f6f 6261 725d 0a20 2020  cii, foobar].   
+00012ad0: 2020 2020 2061 7373 6572 7420 6473 2e61       assert ds.a
+00012ae0: 7474 7273 5b22 6173 6369 695f 6c69 7374  ttrs["ascii_list
+00012af0: 225d 203d 3d20 2261 7363 6969 220a 0a20  "] == "ascii".. 
+00012b00: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00012b10: 2e61 7474 7273 5b22 6279 7465 7322 5d20  .attrs["bytes"] 
+00012b20: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
+00012b30: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
+00012b40: 5b22 6279 7465 735f 3064 696d 225d 203d  ["bytes_0dim"] =
+00012b50: 3d20 6173 6369 690a 2020 2020 2020 2020  = ascii.        
+00012b60: 6173 7365 7274 2064 732e 6174 7472 735b  assert ds.attrs[
+00012b70: 2262 7974 6573 5f31 6469 6d22 5d20 3d3d  "bytes_1dim"] ==
+00012b80: 2061 7363 6969 0a20 2020 2020 2020 2061   ascii.        a
+00012b90: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
+00012ba0: 6279 7465 735f 6172 7261 7922 5d20 3d3d  bytes_array"] ==
+00012bb0: 205b 6173 6369 692c 2066 6f6f 6261 725d   [ascii, foobar]
+00012bc0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00012bd0: 6473 2e61 7474 7273 5b22 6279 7465 735f  ds.attrs["bytes_
+00012be0: 6c69 7374 225d 203d 3d20 2261 7363 6969  list"] == "ascii
+00012bf0: 220a 0a20 2020 2020 2020 2061 7373 6572  "..        asser
+00012c00: 7420 6473 2e61 7474 7273 5b22 756e 6963  t ds.attrs["unic
+00012c10: 6f64 655f 6669 7865 6422 5d20 3d3d 2075  ode_fixed"] == u
+00012c20: 6e69 636f 6465 0a20 2020 2020 2020 2061  nicode.        a
+00012c30: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
+00012c40: 756e 6963 6f64 655f 6669 7865 645f 3064  unicode_fixed_0d
+00012c50: 696d 225d 203d 3d20 756e 6963 6f64 650a  im"] == unicode.
+00012c60: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+00012c70: 732e 6174 7472 735b 2275 6e69 636f 6465  s.attrs["unicode
+00012c80: 5f66 6978 6564 5f31 6469 6d22 5d20 3d3d  _fixed_1dim"] ==
+00012c90: 2075 6e69 636f 6465 0a20 2020 2020 2020   unicode.       
+00012ca0: 2061 7373 6572 7420 6473 2e61 7474 7273   assert ds.attrs
+00012cb0: 5b22 756e 6963 6f64 655f 6669 7865 645f  ["unicode_fixed_
+00012cc0: 6172 7261 7279 225d 203d 3d20 5b75 6e69  arrary"] == [uni
+00012cd0: 636f 6465 2c20 2266 6f6f 62c3 a172 225d  code, "foob..r"]
+00012ce0: 0a0a 2020 2020 2020 2020 6173 6369 6920  ..        ascii 
+00012cf0: 3d20 2261 7363 6969 220a 2020 2020 2020  = "ascii".      
+00012d00: 2020 6173 7365 7274 2064 732e 6174 7472    assert ds.attr
+00012d10: 735b 2261 7363 6969 5f66 6978 6564 225d  s["ascii_fixed"]
+00012d20: 203d 3d20 6173 6369 690a 2020 2020 2020   == ascii.      
+00012d30: 2020 6173 7365 7274 2064 732e 6174 7472    assert ds.attr
+00012d40: 735b 2261 7363 6969 5f66 6978 6564 5f30  s["ascii_fixed_0
+00012d50: 6469 6d22 5d20 3d3d 2061 7363 6969 0a20  dim"] == ascii. 
+00012d60: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00012d70: 2e61 7474 7273 5b22 6173 6369 695f 6669  .attrs["ascii_fi
+00012d80: 7865 645f 3164 696d 225d 203d 3d20 6173  xed_1dim"] == as
+00012d90: 6369 690a 2020 2020 2020 2020 6173 7365  cii.        asse
+00012da0: 7274 2064 732e 6174 7472 735b 2261 7363  rt ds.attrs["asc
+00012db0: 6969 5f66 6978 6564 5f61 7272 6179 225d  ii_fixed_array"]
+00012dc0: 203d 3d20 5b61 7363 6969 2c20 2266 6f6f   == [ascii, "foo
+00012dd0: 6261 7222 5d0a 0a20 2020 2020 2020 2061  bar"]..        a
+00012de0: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
+00012df0: 6279 7465 735f 6669 7865 6422 5d20 3d3d  bytes_fixed"] ==
+00012e00: 2061 7363 6969 0a20 2020 2020 2020 2061   ascii.        a
+00012e10: 7373 6572 7420 6473 2e61 7474 7273 5b22  ssert ds.attrs["
+00012e20: 6279 7465 735f 6669 7865 645f 3064 696d  bytes_fixed_0dim
+00012e30: 225d 203d 3d20 6173 6369 690a 2020 2020  "] == ascii.    
+00012e40: 2020 2020 6173 7365 7274 2064 732e 6174      assert ds.at
+00012e50: 7472 735b 2262 7974 6573 5f66 6978 6564  trs["bytes_fixed
+00012e60: 5f31 6469 6d22 5d20 3d3d 2061 7363 6969  _1dim"] == ascii
+00012e70: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00012e80: 6473 2e61 7474 7273 5b22 6279 7465 735f  ds.attrs["bytes_
+00012e90: 6669 7865 645f 6172 7261 7922 5d20 3d3d  fixed_array"] ==
+00012ea0: 205b 6173 6369 692c 2022 666f 6f62 6172   [ascii, "foobar
+00012eb0: 225d 0a0a 2020 2020 2020 2020 6173 7365  "]..        asse
+00012ec0: 7274 2064 732e 6174 7472 735b 2269 6e74  rt ds.attrs["int
+00012ed0: 225d 203d 3d20 310a 2020 2020 2020 2020  "] == 1.        
+00012ee0: 6173 7365 7274 2064 732e 6174 7472 735b  assert ds.attrs[
+00012ef0: 2269 6e74 6c69 7374 225d 203d 3d20 310a  "intlist"] == 1.
+00012f00: 2020 2020 2020 2020 6e70 2e74 6573 7469          np.testi
+00012f10: 6e67 2e61 7373 6572 745f 6571 7561 6c28  ng.assert_equal(
+00012f20: 6473 2e61 7474 7273 5b22 696e 745f 6172  ds.attrs["int_ar
+00012f30: 7261 7922 5d2c 206e 702e 6172 616e 6765  ray"], np.arange
+00012f40: 2831 3029 290a 2020 2020 2020 2020 6e70  (10)).        np
+00012f50: 2e74 6573 7469 6e67 2e61 7373 6572 745f  .testing.assert_
+00012f60: 6571 7561 6c28 6473 2e61 7474 7273 5b22  equal(ds.attrs["
+00012f70: 656d 7074 795f 6c69 7374 225d 2c20 6e70  empty_list"], np
+00012f80: 2e61 7272 6179 285b 5d29 290a 2020 2020  .array([])).    
+00012f90: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
+00012fa0: 7373 6572 745f 6571 7561 6c28 6473 2e61  ssert_equal(ds.a
+00012fb0: 7474 7273 5b22 656d 7074 795f 6172 7261  ttrs["empty_arra
+00012fc0: 7922 5d2c 206e 702e 6172 7261 7928 5b5d  y"], np.array([]
+00012fd0: 2929 0a0a 2020 2020 7769 7468 206c 6567  ))..    with leg
+00012fe0: 6163 7961 7069 2e44 6174 6173 6574 2874  acyapi.Dataset(t
+00012ff0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+00013000: 206d 6f64 653d 2272 2229 2061 7320 6473   mode="r") as ds
+00013010: 3a0a 2020 2020 2020 2020 6173 7365 7274  :.        assert
+00013020: 2064 732e 756e 6963 6f64 6520 3d3d 2075   ds.unicode == u
+00013030: 6e69 636f 6465 0a20 2020 2020 2020 2061  nicode.        a
+00013040: 7373 6572 7420 6473 2e75 6e69 636f 6465  ssert ds.unicode
+00013050: 5f30 6469 6d20 3d3d 2075 6e69 636f 6465  _0dim == unicode
+00013060: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00013070: 6473 2e75 6e69 636f 6465 5f31 6469 6d20  ds.unicode_1dim 
+00013080: 3d3d 2075 6e69 636f 6465 0a20 2020 2020  == unicode.     
+00013090: 2020 2061 7373 6572 7420 6473 2e75 6e69     assert ds.uni
+000130a0: 636f 6465 5f61 7272 6172 7920 3d3d 205b  code_arrary == [
+000130b0: 756e 6963 6f64 652c 2022 666f 6f62 c3a1  unicode, "foob..
+000130c0: 7222 5d0a 2020 2020 2020 2020 6173 7365  r"].        asse
+000130d0: 7274 2064 732e 756e 6963 6f64 655f 6c69  rt ds.unicode_li
+000130e0: 7374 203d 3d20 756e 6963 6f64 650a 0a20  st == unicode.. 
+000130f0: 2020 2020 2020 2023 2062 7974 6573 2061         # bytes a
+00013100: 6e64 2073 7472 696e 6773 2061 7265 2072  nd strings are r
+00013110: 6563 6569 7665 6420 6173 2073 7472 696e  eceived as strin
+00013120: 6773 2066 6f72 2068 3570 7933 0a20 2020  gs for h5py3.   
+00013130: 2020 2020 2061 7363 6969 203d 2022 6173       ascii = "as
+00013140: 6369 6922 0a20 2020 2020 2020 2066 6f6f  cii".        foo
+00013150: 6261 7220 3d20 2266 6f6f 6261 7222 0a20  bar = "foobar". 
+00013160: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013170: 2e61 7363 6969 203d 3d20 2261 7363 6969  .ascii == "ascii
+00013180: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00013190: 2064 732e 6173 6369 695f 3064 696d 203d   ds.ascii_0dim =
+000131a0: 3d20 6173 6369 690a 2020 2020 2020 2020  = ascii.        
+000131b0: 6173 7365 7274 2064 732e 6173 6369 695f  assert ds.ascii_
+000131c0: 3164 696d 203d 3d20 6173 6369 690a 2020  1dim == ascii.  
+000131d0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+000131e0: 6173 6369 695f 6172 7261 7920 3d3d 205b  ascii_array == [
+000131f0: 6173 6369 692c 2066 6f6f 6261 725d 0a20  ascii, foobar]. 
+00013200: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013210: 2e61 7363 6969 5f6c 6973 7420 3d3d 2022  .ascii_list == "
+00013220: 6173 6369 6922 0a0a 2020 2020 2020 2020  ascii"..        
+00013230: 6173 7365 7274 2064 732e 6279 7465 7320  assert ds.bytes 
+00013240: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
+00013250: 2061 7373 6572 7420 6473 2e62 7974 6573   assert ds.bytes
+00013260: 5f30 6469 6d20 3d3d 2061 7363 6969 0a20  _0dim == ascii. 
+00013270: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013280: 2e62 7974 6573 5f31 6469 6d20 3d3d 2061  .bytes_1dim == a
+00013290: 7363 6969 0a20 2020 2020 2020 2061 7373  scii.        ass
+000132a0: 6572 7420 6473 2e62 7974 6573 5f61 7272  ert ds.bytes_arr
+000132b0: 6179 203d 3d20 5b61 7363 6969 2c20 666f  ay == [ascii, fo
+000132c0: 6f62 6172 5d0a 2020 2020 2020 2020 6173  obar].        as
+000132d0: 7365 7274 2064 732e 6279 7465 735f 6c69  sert ds.bytes_li
+000132e0: 7374 203d 3d20 2261 7363 6969 220a 0a20  st == "ascii".. 
+000132f0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013300: 2e75 6e69 636f 6465 5f66 6978 6564 203d  .unicode_fixed =
+00013310: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
+00013320: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
+00013330: 6f64 655f 6669 7865 645f 3064 696d 203d  ode_fixed_0dim =
+00013340: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
+00013350: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
+00013360: 6f64 655f 6669 7865 645f 3164 696d 203d  ode_fixed_1dim =
+00013370: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
+00013380: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
+00013390: 6f64 655f 6669 7865 645f 6172 7261 7279  ode_fixed_arrary
+000133a0: 203d 3d20 5b75 6e69 636f 6465 2c20 2266   == [unicode, "f
+000133b0: 6f6f 62c3 a172 225d 0a0a 2020 2020 2020  oob..r"]..      
+000133c0: 2020 6173 6369 6920 3d20 2261 7363 6969    ascii = "ascii
+000133d0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+000133e0: 2064 732e 6173 6369 695f 6669 7865 6420   ds.ascii_fixed 
+000133f0: 3d3d 2061 7363 6969 0a20 2020 2020 2020  == ascii.       
+00013400: 2061 7373 6572 7420 6473 2e61 7363 6969   assert ds.ascii
+00013410: 5f66 6978 6564 5f30 6469 6d20 3d3d 2061  _fixed_0dim == a
+00013420: 7363 6969 0a20 2020 2020 2020 2061 7373  scii.        ass
+00013430: 6572 7420 6473 2e61 7363 6969 5f66 6978  ert ds.ascii_fix
+00013440: 6564 5f31 6469 6d20 3d3d 2061 7363 6969  ed_1dim == ascii
+00013450: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00013460: 6473 2e61 7363 6969 5f66 6978 6564 5f61  ds.ascii_fixed_a
+00013470: 7272 6179 203d 3d20 5b61 7363 6969 2c20  rray == [ascii, 
+00013480: 2266 6f6f 6261 7222 5d0a 0a20 2020 2020  "foobar"]..     
+00013490: 2020 2061 7373 6572 7420 6473 2e62 7974     assert ds.byt
+000134a0: 6573 5f66 6978 6564 203d 3d20 6173 6369  es_fixed == asci
+000134b0: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
+000134c0: 2064 732e 6279 7465 735f 6669 7865 645f   ds.bytes_fixed_
+000134d0: 3064 696d 203d 3d20 6173 6369 690a 2020  0dim == ascii.  
+000134e0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+000134f0: 6279 7465 735f 6669 7865 645f 3164 696d  bytes_fixed_1dim
+00013500: 203d 3d20 6173 6369 690a 2020 2020 2020   == ascii.      
+00013510: 2020 6173 7365 7274 2064 732e 6279 7465    assert ds.byte
+00013520: 735f 6669 7865 645f 6172 7261 7920 3d3d  s_fixed_array ==
+00013530: 205b 6173 6369 692c 2022 666f 6f62 6172   [ascii, "foobar
+00013540: 225d 0a0a 2020 2020 2020 2020 6173 7365  "]..        asse
+00013550: 7274 2064 732e 696e 7420 3d3d 2031 0a20  rt ds.int == 1. 
+00013560: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013570: 2e69 6e74 6c69 7374 203d 3d20 310a 2020  .intlist == 1.  
+00013580: 2020 2020 2020 6e70 2e74 6573 7469 6e67        np.testing
+00013590: 2e61 7373 6572 745f 6571 7561 6c28 6473  .assert_equal(ds
+000135a0: 2e69 6e74 5f61 7272 6179 2c20 6e70 2e61  .int_array, np.a
+000135b0: 7261 6e67 6528 3130 2929 0a20 2020 2020  range(10)).     
+000135c0: 2020 206e 702e 7465 7374 696e 672e 6173     np.testing.as
+000135d0: 7365 7274 5f65 7175 616c 2864 732e 6174  sert_equal(ds.at
+000135e0: 7472 735b 2265 6d70 7479 5f6c 6973 7422  trs["empty_list"
+000135f0: 5d2c 206e 702e 6172 7261 7928 5b5d 2929  ], np.array([]))
+00013600: 0a20 2020 2020 2020 206e 702e 7465 7374  .        np.test
+00013610: 696e 672e 6173 7365 7274 5f65 7175 616c  ing.assert_equal
+00013620: 2864 732e 6174 7472 735b 2265 6d70 7479  (ds.attrs["empty
+00013630: 5f61 7272 6179 225d 2c20 6e70 2e61 7272  _array"], np.arr
+00013640: 6179 285b 5d29 290a 0a20 2020 2077 6974  ay([]))..    wit
+00013650: 6820 6e65 7443 4446 342e 4461 7461 7365  h netCDF4.Datase
+00013660: 7428 746d 705f 6c6f 6361 6c5f 6e65 7463  t(tmp_local_netc
+00013670: 6466 2c20 6d6f 6465 3d22 7222 2920 6173  df, mode="r") as
+00013680: 2064 733a 0a20 2020 2020 2020 2061 7373   ds:.        ass
+00013690: 6572 7420 6473 2e75 6e69 636f 6465 203d  ert ds.unicode =
+000136a0: 3d20 756e 6963 6f64 650a 2020 2020 2020  = unicode.      
+000136b0: 2020 6173 7365 7274 2064 732e 756e 6963    assert ds.unic
+000136c0: 6f64 655f 3064 696d 203d 3d20 756e 6963  ode_0dim == unic
+000136d0: 6f64 650a 2020 2020 2020 2020 6173 7365  ode.        asse
+000136e0: 7274 2064 732e 756e 6963 6f64 655f 3164  rt ds.unicode_1d
+000136f0: 696d 203d 3d20 756e 6963 6f64 650a 2020  im == unicode.  
+00013700: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+00013710: 756e 6963 6f64 655f 6172 7261 7279 203d  unicode_arrary =
+00013720: 3d20 5b75 6e69 636f 6465 2c20 2266 6f6f  = [unicode, "foo
+00013730: 62c3 a172 225d 0a20 2020 2020 2020 2061  b..r"].        a
+00013740: 7373 6572 7420 6473 2e75 6e69 636f 6465  ssert ds.unicode
+00013750: 5f6c 6973 7420 3d3d 2075 6e69 636f 6465  _list == unicode
+00013760: 0a0a 2020 2020 2020 2020 6173 6369 6920  ..        ascii 
+00013770: 3d20 2261 7363 6969 220a 2020 2020 2020  = "ascii".      
+00013780: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
+00013790: 6920 3d3d 2061 7363 6969 0a20 2020 2020  i == ascii.     
+000137a0: 2020 2061 7373 6572 7420 6473 2e61 7363     assert ds.asc
+000137b0: 6969 5f30 6469 6d20 3d3d 2061 7363 6969  ii_0dim == ascii
+000137c0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000137d0: 6473 2e61 7363 6969 5f31 6469 6d20 3d3d  ds.ascii_1dim ==
+000137e0: 2061 7363 6969 0a20 2020 2020 2020 2061   ascii.        a
+000137f0: 7373 6572 7420 6473 2e61 7363 6969 5f61  ssert ds.ascii_a
+00013800: 7272 6179 203d 3d20 5b61 7363 6969 2c20  rray == [ascii, 
+00013810: 2266 6f6f 6261 7222 5d0a 2020 2020 2020  "foobar"].      
+00013820: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
+00013830: 695f 6c69 7374 203d 3d20 6173 6369 690a  i_list == ascii.
+00013840: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00013850: 6473 2e62 7974 6573 203d 3d20 6173 6369  ds.bytes == asci
+00013860: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
+00013870: 2064 732e 6279 7465 735f 3064 696d 203d   ds.bytes_0dim =
+00013880: 3d20 6173 6369 690a 2020 2020 2020 2020  = ascii.        
+00013890: 6173 7365 7274 2064 732e 6279 7465 735f  assert ds.bytes_
+000138a0: 3164 696d 203d 3d20 6173 6369 690a 2020  1dim == ascii.  
+000138b0: 2020 2020 2020 6173 7365 7274 2064 732e        assert ds.
+000138c0: 6279 7465 735f 6172 7261 7920 3d3d 205b  bytes_array == [
+000138d0: 6173 6369 692c 2022 666f 6f62 6172 225d  ascii, "foobar"]
+000138e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000138f0: 6473 2e62 7974 6573 5f6c 6973 7420 3d3d  ds.bytes_list ==
+00013900: 2061 7363 6969 0a0a 2020 2020 2020 2020   ascii..        
+00013910: 6173 7365 7274 2064 732e 756e 6963 6f64  assert ds.unicod
+00013920: 655f 6669 7865 6420 3d3d 2075 6e69 636f  e_fixed == unico
+00013930: 6465 0a20 2020 2020 2020 2061 7373 6572  de.        asser
+00013940: 7420 6473 2e75 6e69 636f 6465 5f66 6978  t ds.unicode_fix
+00013950: 6564 5f30 6469 6d20 3d3d 2075 6e69 636f  ed_0dim == unico
+00013960: 6465 0a20 2020 2020 2020 2061 7373 6572  de.        asser
+00013970: 7420 6473 2e75 6e69 636f 6465 5f66 6978  t ds.unicode_fix
+00013980: 6564 5f31 6469 6d20 3d3d 2075 6e69 636f  ed_1dim == unico
+00013990: 6465 0a20 2020 2020 2020 2061 7373 6572  de.        asser
+000139a0: 7420 6473 2e75 6e69 636f 6465 5f66 6978  t ds.unicode_fix
+000139b0: 6564 5f61 7272 6172 7920 3d3d 205b 756e  ed_arrary == [un
+000139c0: 6963 6f64 652c 2022 666f 6f62 c3a1 7222  icode, "foob..r"
+000139d0: 5d0a 0a20 2020 2020 2020 2061 7373 6572  ]..        asser
+000139e0: 7420 6473 2e61 7363 6969 5f66 6978 6564  t ds.ascii_fixed
+000139f0: 203d 3d20 6173 6369 690a 2020 2020 2020   == ascii.      
+00013a00: 2020 6173 7365 7274 2064 732e 6173 6369    assert ds.asci
+00013a10: 695f 6669 7865 645f 3064 696d 203d 3d20  i_fixed_0dim == 
+00013a20: 6173 6369 690a 2020 2020 2020 2020 6173  ascii.        as
+00013a30: 7365 7274 2064 732e 6173 6369 695f 6669  sert ds.ascii_fi
+00013a40: 7865 645f 3164 696d 203d 3d20 6173 6369  xed_1dim == asci
+00013a50: 690a 2020 2020 2020 2020 6173 7365 7274  i.        assert
+00013a60: 2064 732e 6173 6369 695f 6669 7865 645f   ds.ascii_fixed_
+00013a70: 6172 7261 7920 3d3d 205b 6173 6369 692c  array == [ascii,
+00013a80: 2022 666f 6f62 6172 225d 0a0a 2020 2020   "foobar"]..    
+00013a90: 2020 2020 6173 7365 7274 2064 732e 6279      assert ds.by
+00013aa0: 7465 735f 6669 7865 6420 3d3d 2061 7363  tes_fixed == asc
+00013ab0: 6969 0a20 2020 2020 2020 2061 7373 6572  ii.        asser
+00013ac0: 7420 6473 2e62 7974 6573 5f66 6978 6564  t ds.bytes_fixed
+00013ad0: 5f30 6469 6d20 3d3d 2061 7363 6969 0a20  _0dim == ascii. 
+00013ae0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+00013af0: 2e62 7974 6573 5f66 6978 6564 5f31 6469  .bytes_fixed_1di
+00013b00: 6d20 3d3d 2061 7363 6969 0a20 2020 2020  m == ascii.     
+00013b10: 2020 2061 7373 6572 7420 6473 2e62 7974     assert ds.byt
+00013b20: 6573 5f66 6978 6564 5f61 7272 6179 203d  es_fixed_array =
+00013b30: 3d20 5b61 7363 6969 2c20 2266 6f6f 6261  = [ascii, "fooba
+00013b40: 7222 5d0a 0a20 2020 2020 2020 2061 7373  r"]..        ass
+00013b50: 6572 7420 6473 2e69 6e74 203d 3d20 310a  ert ds.int == 1.
+00013b60: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+00013b70: 732e 696e 746c 6973 7420 3d3d 2031 0a20  s.intlist == 1. 
+00013b80: 2020 2020 2020 206e 702e 7465 7374 696e         np.testin
+00013b90: 672e 6173 7365 7274 5f65 7175 616c 2864  g.assert_equal(d
+00013ba0: 732e 696e 745f 6172 7261 792c 206e 702e  s.int_array, np.
+00013bb0: 6172 616e 6765 2831 3029 290a 2020 2020  arange(10)).    
+00013bc0: 2020 2020 6e70 2e74 6573 7469 6e67 2e61      np.testing.a
+00013bd0: 7373 6572 745f 6571 7561 6c28 6473 2e65  ssert_equal(ds.e
+00013be0: 6d70 7479 5f6c 6973 742c 206e 702e 6172  mpty_list, np.ar
+00013bf0: 7261 7928 5b5d 2929 0a20 2020 2020 2020  ray([])).       
+00013c00: 206e 702e 7465 7374 696e 672e 6173 7365   np.testing.asse
+00013c10: 7274 5f65 7175 616c 2864 732e 656d 7074  rt_equal(ds.empt
+00013c20: 795f 6172 7261 792c 206e 702e 6172 7261  y_array, np.arra
+00013c30: 7928 5b5d 2929 0a0a 0a40 7079 7465 7374  y([]))...@pytest
+00013c40: 2e6d 6172 6b2e 736b 6970 6966 280a 2020  .mark.skipif(.  
+00013c50: 2020 7665 7273 696f 6e2e 7061 7273 6528    version.parse(
+00013c60: 6835 7079 2e5f 5f76 6572 7369 6f6e 5f5f  h5py.__version__
+00013c70: 2920 3c20 7665 7273 696f 6e2e 7061 7273  ) < version.pars
+00013c80: 6528 2233 2e37 2e30 2229 2c0a 2020 2020  e("3.7.0"),.    
+00013c90: 7265 6173 6f6e 3d22 646f 6573 206e 6f74  reason="does not
+00013ca0: 2077 6f72 6b20 7769 7468 2068 3570 7920   work with h5py 
+00013cb0: 3c20 332e 372e 3022 2c0a 290a 6465 6620  < 3.7.0",.).def 
+00013cc0: 7465 7374 5f76 6c65 6e5f 7374 7269 6e67  test_vlen_string
+00013cd0: 5f64 6174 6173 6574 5f66 696c 6c76 616c  _dataset_fillval
+00013ce0: 7565 2874 6d70 5f6c 6f63 616c 5f6e 6574  ue(tmp_local_net
+00013cf0: 6364 662c 2064 6563 6f64 655f 766c 656e  cdf, decode_vlen
+00013d00: 5f73 7472 696e 6773 293a 0a20 2020 2023  _strings):.    #
+00013d10: 2063 6865 636b 205f 4669 6c6c 5661 6c75   check _FillValu
+00013d20: 6520 666f 7220 564c 454e 2073 7472 696e  e for VLEN strin
+00013d30: 6720 6461 7461 7365 7473 0a20 2020 2023  g datasets.    #
+00013d40: 206f 6e6c 7920 776f 726b 7320 666f 7220   only works for 
+00013d50: 6835 7079 203e 3d20 332e 372e 300a 0a20  h5py >= 3.7.0.. 
+00013d60: 2020 2023 2066 6972 7374 2077 6974 6820     # first with 
+00013d70: 6e65 7720 4150 490a 2020 2020 7769 7468  new API.    with
+00013d80: 2068 356e 6574 6364 662e 4669 6c65 2874   h5netcdf.File(t
+00013d90: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+00013da0: 2022 7722 2920 6173 2064 733a 0a20 2020   "w") as ds:.   
+00013db0: 2020 2020 2064 732e 6469 6d65 6e73 696f       ds.dimensio
+00013dc0: 6e73 203d 207b 2273 7472 696e 6722 3a20  ns = {"string": 
+00013dd0: 3130 7d0a 2020 2020 2020 2020 6474 3020  10}.        dt0 
+00013de0: 3d20 6835 7079 2e73 7472 696e 675f 6474  = h5py.string_dt
+00013df0: 7970 6528 290a 2020 2020 2020 2020 6669  ype().        fi
+00013e00: 6c6c 5f76 616c 7565 3020 3d20 2262 c3a1  ll_value0 = "b..
+00013e10: 7222 0a20 2020 2020 2020 2064 732e 6372  r".        ds.cr
+00013e20: 6561 7465 5f76 6172 6961 626c 6528 2278  eate_variable("x
+00013e30: 3022 2c20 2822 7374 7269 6e67 222c 292c  0", ("string",),
+00013e40: 2064 7479 7065 3d64 7430 2c20 6669 6c6c   dtype=dt0, fill
+00013e50: 7661 6c75 653d 6669 6c6c 5f76 616c 7565  value=fill_value
+00013e60: 3029 0a20 2020 2020 2020 2064 7431 203d  0).        dt1 =
+00013e70: 2068 3570 792e 7374 7269 6e67 5f64 7479   h5py.string_dty
+00013e80: 7065 2822 6173 6369 6922 290a 2020 2020  pe("ascii").    
+00013e90: 2020 2020 6669 6c6c 5f76 616c 7565 3120      fill_value1 
+00013ea0: 3d20 2262 6172 220a 2020 2020 2020 2020  = "bar".        
+00013eb0: 6473 2e63 7265 6174 655f 7661 7269 6162  ds.create_variab
+00013ec0: 6c65 2822 7831 222c 2028 2273 7472 696e  le("x1", ("strin
+00013ed0: 6722 2c29 2c20 6474 7970 653d 6474 312c  g",), dtype=dt1,
+00013ee0: 2066 696c 6c76 616c 7565 3d66 696c 6c5f   fillvalue=fill_
+00013ef0: 7661 6c75 6531 290a 0a20 2020 2023 2063  value1)..    # c
+00013f00: 6865 636b 2c20 6966 206e 6577 2041 5049  heck, if new API
+00013f10: 2063 616e 2072 6561 6420 7468 656d 0a20   can read them. 
+00013f20: 2020 2077 6974 6820 6835 6e65 7463 6466     with h5netcdf
+00013f30: 2e46 696c 6528 746d 705f 6c6f 6361 6c5f  .File(tmp_local_
+00013f40: 6e65 7463 6466 2c20 2272 222c 202a 2a64  netcdf, "r", **d
+00013f50: 6563 6f64 655f 766c 656e 5f73 7472 696e  ecode_vlen_strin
+00013f60: 6773 2920 6173 2064 733a 0a20 2020 2020  gs) as ds:.     
+00013f70: 2020 2064 6563 6f64 655f 766c 656e 203d     decode_vlen =
+00013f80: 2064 6563 6f64 655f 766c 656e 5f73 7472   decode_vlen_str
+00013f90: 696e 6773 5b22 6465 636f 6465 5f76 6c65  ings["decode_vle
+00013fa0: 6e5f 7374 7269 6e67 7322 5d0a 2020 2020  n_strings"].    
+00013fb0: 2020 2020 6676 616c 7565 3020 3d20 6669      fvalue0 = fi
+00013fc0: 6c6c 5f76 616c 7565 3020 6966 2064 6563  ll_value0 if dec
+00013fd0: 6f64 655f 766c 656e 2065 6c73 6520 6669  ode_vlen else fi
+00013fe0: 6c6c 5f76 616c 7565 302e 656e 636f 6465  ll_value0.encode
+00013ff0: 2822 7574 662d 3822 290a 2020 2020 2020  ("utf-8").      
+00014000: 2020 6676 616c 7565 3120 3d20 6669 6c6c    fvalue1 = fill
+00014010: 5f76 616c 7565 3120 6966 2064 6563 6f64  _value1 if decod
+00014020: 655f 766c 656e 2065 6c73 6520 6669 6c6c  e_vlen else fill
+00014030: 5f76 616c 7565 312e 656e 636f 6465 2822  _value1.encode("
+00014040: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
+00014050: 6173 7365 7274 2064 735b 2278 3022 5d5b  assert ds["x0"][
+00014060: 305d 203d 3d20 6676 616c 7565 300a 2020  0] == fvalue0.  
+00014070: 2020 2020 2020 6173 7365 7274 2064 735b        assert ds[
+00014080: 2278 3022 5d2e 6174 7472 735b 225f 4669  "x0"].attrs["_Fi
+00014090: 6c6c 5661 6c75 6522 5d20 3d3d 2066 696c  llValue"] == fil
+000140a0: 6c5f 7661 6c75 6530 0a20 2020 2020 2020  l_value0.       
+000140b0: 2061 7373 6572 7420 6473 5b22 7831 225d   assert ds["x1"]
+000140c0: 5b30 5d20 3d3d 2066 7661 6c75 6531 0a20  [0] == fvalue1. 
+000140d0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+000140e0: 5b22 7831 225d 2e61 7474 7273 5b22 5f46  ["x1"].attrs["_F
+000140f0: 696c 6c56 616c 7565 225d 203d 3d20 6669  illValue"] == fi
+00014100: 6c6c 5f76 616c 7565 310a 0a20 2020 2023  ll_value1..    #
+00014110: 2063 6865 636b 2069 6620 6c65 6761 6379   check if legacy
+00014120: 6170 6920 6361 6e20 7265 6164 2074 6865  api can read the
+00014130: 6d0a 2020 2020 7769 7468 206c 6567 6163  m.    with legac
+00014140: 7961 7069 2e44 6174 6173 6574 2874 6d70  yapi.Dataset(tmp
+00014150: 5f6c 6f63 616c 5f6e 6574 6364 662c 2022  _local_netcdf, "
+00014160: 7222 2920 6173 2064 733a 0a20 2020 2020  r") as ds:.     
+00014170: 2020 2061 7373 6572 7420 6473 5b22 7830     assert ds["x0
+00014180: 225d 5b30 5d20 3d3d 2066 696c 6c5f 7661  "][0] == fill_va
+00014190: 6c75 6530 0a20 2020 2020 2020 2061 7373  lue0.        ass
+000141a0: 6572 7420 6473 5b22 7830 225d 2e5f 4669  ert ds["x0"]._Fi
+000141b0: 6c6c 5661 6c75 6520 3d3d 2066 696c 6c5f  llValue == fill_
+000141c0: 7661 6c75 6530 0a20 2020 2020 2020 2061  value0.        a
+000141d0: 7373 6572 7420 6473 5b22 7831 225d 5b30  ssert ds["x1"][0
+000141e0: 5d20 3d3d 2066 696c 6c5f 7661 6c75 6531  ] == fill_value1
+000141f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00014200: 6473 5b22 7831 225d 2e5f 4669 6c6c 5661  ds["x1"]._FillVa
+00014210: 6c75 6520 3d3d 2066 696c 6c5f 7661 6c75  lue == fill_valu
+00014220: 6531 0a0a 2020 2020 2320 6368 6563 6b20  e1..    # check 
+00014230: 6966 206e 6574 4344 4634 2d70 7974 686f  if netCDF4-pytho
+00014240: 6e20 6361 6e20 7265 6164 2074 6865 6d0a  n can read them.
+00014250: 2020 2020 7769 7468 206e 6574 4344 4634      with netCDF4
+00014260: 2e44 6174 6173 6574 2874 6d70 5f6c 6f63  .Dataset(tmp_loc
+00014270: 616c 5f6e 6574 6364 662c 2022 7222 2920  al_netcdf, "r") 
+00014280: 6173 2064 733a 0a20 2020 2020 2020 2061  as ds:.        a
+00014290: 7373 6572 7420 6473 5b22 7830 225d 5b30  ssert ds["x0"][0
+000142a0: 5d20 3d3d 2066 696c 6c5f 7661 6c75 6530  ] == fill_value0
+000142b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000142c0: 6473 5b22 7830 225d 2e5f 4669 6c6c 5661  ds["x0"]._FillVa
+000142d0: 6c75 6520 3d3d 2066 696c 6c5f 7661 6c75  lue == fill_valu
+000142e0: 6530 0a20 2020 2020 2020 2061 7373 6572  e0.        asser
+000142f0: 7420 6473 5b22 7831 225d 5b30 5d20 3d3d  t ds["x1"][0] ==
+00014300: 2066 696c 6c5f 7661 6c75 6531 0a20 2020   fill_value1.   
+00014310: 2020 2020 2061 7373 6572 7420 6473 5b22       assert ds["
+00014320: 7831 225d 2e5f 4669 6c6c 5661 6c75 6520  x1"]._FillValue 
+00014330: 3d3d 2066 696c 6c5f 7661 6c75 6531 0a0a  == fill_value1..
+00014340: 2020 2020 2320 7365 636f 6e64 2077 6974      # second wit
+00014350: 6820 6c65 6761 6379 6170 690a 2020 2020  h legacyapi.    
+00014360: 7769 7468 206c 6567 6163 7961 7069 2e44  with legacyapi.D
+00014370: 6174 6173 6574 2874 6d70 5f6c 6f63 616c  ataset(tmp_local
+00014380: 5f6e 6574 6364 662c 2022 7722 2920 6173  _netcdf, "w") as
+00014390: 2064 733a 0a20 2020 2020 2020 2064 732e   ds:.        ds.
+000143a0: 6372 6561 7465 4469 6d65 6e73 696f 6e28  createDimension(
+000143b0: 2273 7472 696e 6722 2c20 3130 290a 2020  "string", 10).  
+000143c0: 2020 2020 2020 6669 6c6c 5f76 616c 7565        fill_value
+000143d0: 3020 3d20 2262 c3a1 7222 0a20 2020 2020  0 = "b..r".     
+000143e0: 2020 2064 732e 6372 6561 7465 5661 7269     ds.createVari
+000143f0: 6162 6c65 2822 7830 222c 2073 7472 2c20  able("x0", str, 
+00014400: 2822 7374 7269 6e67 222c 292c 2066 696c  ("string",), fil
+00014410: 6c5f 7661 6c75 653d 6669 6c6c 5f76 616c  l_value=fill_val
+00014420: 7565 3029 0a20 2020 2020 2020 2066 696c  ue0).        fil
+00014430: 6c5f 7661 6c75 6531 203d 2022 6261 7222  l_value1 = "bar"
+00014440: 0a20 2020 2020 2020 2064 732e 6372 6561  .        ds.crea
+00014450: 7465 5661 7269 6162 6c65 2822 7831 222c  teVariable("x1",
+00014460: 2073 7472 2c20 2822 7374 7269 6e67 222c   str, ("string",
+00014470: 292c 2066 696c 6c5f 7661 6c75 653d 6669  ), fill_value=fi
+00014480: 6c6c 5f76 616c 7565 3129 0a0a 2020 2020  ll_value1)..    
+00014490: 2320 6368 6563 6b20 6966 206e 6577 2041  # check if new A
+000144a0: 5049 2063 616e 2072 6561 6420 7468 656d  PI can read them
+000144b0: 0a20 2020 2077 6974 6820 6835 6e65 7463  .    with h5netc
+000144c0: 6466 2e46 696c 6528 746d 705f 6c6f 6361  df.File(tmp_loca
+000144d0: 6c5f 6e65 7463 6466 2c20 2272 222c 202a  l_netcdf, "r", *
+000144e0: 2a64 6563 6f64 655f 766c 656e 5f73 7472  *decode_vlen_str
+000144f0: 696e 6773 2920 6173 2064 733a 0a20 2020  ings) as ds:.   
+00014500: 2020 2020 2064 6563 6f64 655f 766c 656e       decode_vlen
+00014510: 203d 2064 6563 6f64 655f 766c 656e 5f73   = decode_vlen_s
+00014520: 7472 696e 6773 5b22 6465 636f 6465 5f76  trings["decode_v
+00014530: 6c65 6e5f 7374 7269 6e67 7322 5d0a 2020  len_strings"].  
+00014540: 2020 2020 2020 6676 616c 7565 3020 3d20        fvalue0 = 
+00014550: 6669 6c6c 5f76 616c 7565 3020 6966 2064  fill_value0 if d
+00014560: 6563 6f64 655f 766c 656e 2065 6c73 6520  ecode_vlen else 
+00014570: 6669 6c6c 5f76 616c 7565 302e 656e 636f  fill_value0.enco
+00014580: 6465 2822 7574 662d 3822 290a 2020 2020  de("utf-8").    
+00014590: 2020 2020 6676 616c 7565 3120 3d20 6669      fvalue1 = fi
+000145a0: 6c6c 5f76 616c 7565 3120 6966 2064 6563  ll_value1 if dec
+000145b0: 6f64 655f 766c 656e 2065 6c73 6520 6669  ode_vlen else fi
+000145c0: 6c6c 5f76 616c 7565 312e 656e 636f 6465  ll_value1.encode
+000145d0: 2822 7574 662d 3822 290a 2020 2020 2020  ("utf-8").      
+000145e0: 2020 6173 7365 7274 2064 735b 2278 3022    assert ds["x0"
+000145f0: 5d5b 305d 203d 3d20 6676 616c 7565 300a  ][0] == fvalue0.
+00014600: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
+00014610: 735b 2278 3022 5d2e 6174 7472 735b 225f  s["x0"].attrs["_
+00014620: 4669 6c6c 5661 6c75 6522 5d20 3d3d 2066  FillValue"] == f
+00014630: 696c 6c5f 7661 6c75 6530 0a20 2020 2020  ill_value0.     
+00014640: 2020 2061 7373 6572 7420 6473 5b22 7831     assert ds["x1
+00014650: 225d 5b30 5d20 3d3d 2066 7661 6c75 6531  "][0] == fvalue1
+00014660: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00014670: 6473 5b22 7831 225d 2e61 7474 7273 5b22  ds["x1"].attrs["
+00014680: 5f46 696c 6c56 616c 7565 225d 203d 3d20  _FillValue"] == 
+00014690: 6669 6c6c 5f76 616c 7565 310a 0a20 2020  fill_value1..   
+000146a0: 2023 2063 6865 636b 2069 6620 6c65 6761   # check if lega
+000146b0: 6379 6170 6920 6361 6e20 7265 6164 2074  cyapi can read t
+000146c0: 6865 6d0a 2020 2020 7769 7468 206c 6567  hem.    with leg
+000146d0: 6163 7961 7069 2e44 6174 6173 6574 2874  acyapi.Dataset(t
+000146e0: 6d70 5f6c 6f63 616c 5f6e 6574 6364 662c  mp_local_netcdf,
+000146f0: 2022 7222 2920 6173 2064 733a 0a20 2020   "r") as ds:.   
+00014700: 2020 2020 2061 7373 6572 7420 6473 5b22       assert ds["
+00014710: 7830 225d 5b30 5d20 3d3d 2066 696c 6c5f  x0"][0] == fill_
+00014720: 7661 6c75 6530 0a20 2020 2020 2020 2061  value0.        a
+00014730: 7373 6572 7420 6473 5b22 7830 225d 2e5f  ssert ds["x0"]._
+00014740: 4669 6c6c 5661 6c75 6520 3d3d 2066 696c  FillValue == fil
+00014750: 6c5f 7661 6c75 6530 0a20 2020 2020 2020  l_value0.       
+00014760: 2061 7373 6572 7420 6473 5b22 7831 225d   assert ds["x1"]
+00014770: 5b30 5d20 3d3d 2066 696c 6c5f 7661 6c75  [0] == fill_valu
+00014780: 6531 0a20 2020 2020 2020 2061 7373 6572  e1.        asser
+00014790: 7420 6473 5b22 7831 225d 2e5f 4669 6c6c  t ds["x1"]._Fill
+000147a0: 5661 6c75 6520 3d3d 2066 696c 6c5f 7661  Value == fill_va
+000147b0: 6c75 6531 0a0a 2020 2020 2320 6368 6563  lue1..    # chec
+000147c0: 6b20 6966 206e 6574 4344 4634 2d70 7974  k if netCDF4-pyt
+000147d0: 686f 6e20 6361 6e20 7265 6164 2074 6865  hon can read the
+000147e0: 6d0a 2020 2020 7769 7468 206e 6574 4344  m.    with netCD
+000147f0: 4634 2e44 6174 6173 6574 2874 6d70 5f6c  F4.Dataset(tmp_l
+00014800: 6f63 616c 5f6e 6574 6364 662c 2022 7222  ocal_netcdf, "r"
+00014810: 2920 6173 2064 733a 0a20 2020 2020 2020  ) as ds:.       
+00014820: 2061 7373 6572 7420 6473 5b22 7830 225d   assert ds["x0"]
+00014830: 5b30 5d20 3d3d 2066 696c 6c5f 7661 6c75  [0] == fill_valu
+00014840: 6530 0a20 2020 2020 2020 2061 7373 6572  e0.        asser
+00014850: 7420 6473 5b22 7830 225d 2e5f 4669 6c6c  t ds["x0"]._Fill
+00014860: 5661 6c75 6520 3d3d 2066 696c 6c5f 7661  Value == fill_va
+00014870: 6c75 6530 0a20 2020 2020 2020 2061 7373  lue0.        ass
+00014880: 6572 7420 6473 5b22 7831 225d 5b30 5d20  ert ds["x1"][0] 
+00014890: 3d3d 2066 696c 6c5f 7661 6c75 6531 0a20  == fill_value1. 
+000148a0: 2020 2020 2020 2061 7373 6572 7420 6473         assert ds
+000148b0: 5b22 7831 225d 2e5f 4669 6c6c 5661 6c75  ["x1"]._FillValu
+000148c0: 6520 3d3d 2066 696c 6c5f 7661 6c75 6531  e == fill_value1
+000148d0: 0a                                       .
```

### Comparing `h5netcdf-1.1.0/h5netcdf/utils.py` & `h5netcdf-1.2.0/h5netcdf/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     def __len__(self):
         return len(self._mapping)
 
     def __contains__(self, key):
         return key in self._mapping
 
     def __repr__(self):
-        return "%s(%r)" % (type(self).__name__, self._mapping)
+        return f"{type(self).__name__}({self._mapping!r})"
```

### Comparing `h5netcdf-1.1.0/h5netcdf.egg-info/PKG-INFO` & `h5netcdf-1.2.0/h5netcdf.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 Metadata-Version: 2.1
 Name: h5netcdf
-Version: 1.1.0
+Version: 1.2.0
 Summary: netCDF4 via h5py
-Home-page: https://h5netcdf.org
-Author: h5netcdf developers
-Author-email: devteam@h5netcdf.org
-License: BSD
-Classifier: Development Status :: 4 - Beta
+Author-email: Stephan Hoyer <shoyer@gmail.com>, Kai Mühlbauer <kmuehlbauer@wradlib.org>
+Maintainer-email: h5netcdf developers <devteam@h5netcdf.org>
+License: Copyright (c) 2015, h5netcdf developers
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its contributors
+           may be used to endorse or promote products derived from this software
+           without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: homepage, https://h5netcdf.org
+Project-URL: documentation, https://h5netcdf.org
+Project-URL: repository, https://github.com/h5netcdf/h5netcdf
+Project-URL: changelog, https://github.com/h5netcdf/h5netcdf/blob/main/CHANGELOG.rst
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS.txt
 
 h5netcdf
 ========
 
 .. image:: https://github.com/h5netcdf/h5netcdf/workflows/CI/badge.svg
@@ -63,25 +93,30 @@
 .. _xarray: https://github.com/pydata/xarray/
 
 Install
 -------
 
 Ensure you have a recent version of h5py installed (I recommend using `conda`_ or
 the community effort `conda-forge`_).
-At least version 2.1 is required (for dimension scales); versions 2.3 and newer
-have been verified to work, though some tests only pass on h5py 2.6. Then::
+At least version 3.0 is required. Then::
 
     $ pip install h5netcdf
 
 Or if you are already using conda::
 
     $ conda install h5netcdf
 
+Note:
+
+From version 1.2. h5netcdf tries to align with a `nep29`_-like support policy with regard
+to it's upstream dependencies.
+
 .. _conda: https://conda.io/
 .. _conda-forge: https://conda-forge.org/
+.. _nep29: https://numpy.org/neps/nep-0029-deprecation_policy.html
 
 Usage
 -----
 
 h5netcdf has two APIs, a new API and a legacy API. Both interfaces currently
 reproduce most of the features of the netCDF interface, with the notable
 exception of support for operations that rename or delete existing objects.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `h5netcdf-1.1.0/h5netcdf.egg-info/SOURCES.txt` & `h5netcdf-1.2.0/h5netcdf.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+.pre-commit-config.yaml
 AUTHORS.txt
 CHANGELOG.rst
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 doc/Makefile
 doc/api.rst
 doc/changelog.rst
 doc/conf.py
 doc/devguide.rst
 doc/feature.rst
 doc/index.rst
```

### Comparing `h5netcdf-1.1.0/licenses/H5PY_LICENSE.txt` & `h5netcdf-1.2.0/licenses/H5PY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `h5netcdf-1.1.0/licenses/PSF_LICENSE.txt` & `h5netcdf-1.2.0/licenses/PSF_LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -247,8 +247,8 @@
 
 STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO
 THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
 FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE
 FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
-OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
```

