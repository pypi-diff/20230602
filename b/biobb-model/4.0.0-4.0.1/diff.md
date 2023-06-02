# Comparing `tmp/biobb_model-4.0.0.tar.gz` & `tmp/biobb_model-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_model-4.0.0.tar", last modified: Wed Apr  5 08:47:55 2023, max compression
+gzip compressed data, was "dist/biobb_model-4.0.1.tar", last modified: Fri Jun  2 09:59:37 2023, max compression
```

## Comparing `biobb_model-4.0.0.tar` & `biobb_model-4.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-05 08:47:55.000000 biobb_model-4.0.0/
--rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:05.000000 biobb_model-4.0.0/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)     6169 2023-04-05 08:47:55.000000 biobb_model-4.0.0/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     5124 2023-04-05 06:22:23.000000 biobb_model-4.0.0/README.md
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model/
--rwxr-xr-x   0 pau        (501) staff       (20)       63 2023-04-05 06:15:40.000000 biobb_model-4.0.0/biobb_model/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model/model/
--rwxr-xr-x   0 pau        (501) staff       (20)      157 2022-11-02 12:01:31.000000 biobb_model-4.0.0/biobb_model/model/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5196 2023-04-05 06:36:46.000000 biobb_model-4.0.0/biobb_model/model/checking_log.py
--rw-r--r--   0 pau        (501) staff       (20)      716 2023-04-05 06:37:11.000000 biobb_model-4.0.0/biobb_model/model/common.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5605 2023-03-23 12:01:36.000000 biobb_model-4.0.0/biobb_model/model/fix_altlocs.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5142 2023-03-27 10:29:40.000000 biobb_model-4.0.0/biobb_model/model/fix_amides.py
--rwxr-xr-x   0 pau        (501) staff       (20)     7211 2023-03-27 09:39:08.000000 biobb_model-4.0.0/biobb_model/model/fix_backbone.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5263 2023-03-27 10:32:27.000000 biobb_model-4.0.0/biobb_model/model/fix_chirality.py
--rw-r--r--   0 pau        (501) staff       (20)     6145 2023-03-27 10:33:54.000000 biobb_model-4.0.0/biobb_model/model/fix_pdb.py
--rw-r--r--   0 pau        (501) staff       (20)    46058 2023-04-05 08:36:34.000000 biobb_model-4.0.0/biobb_model/model/fix_pdb_utils.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6148 2023-03-27 10:33:01.000000 biobb_model-4.0.0/biobb_model/model/fix_side_chain.py
--rwxr-xr-x   0 pau        (501) staff       (20)     5117 2023-03-27 10:28:39.000000 biobb_model-4.0.0/biobb_model/model/fix_ssbonds.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6529 2023-04-04 17:32:15.000000 biobb_model-4.0.0/biobb_model/model/mutate.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model/test/
--rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:05.000000 biobb_model-4.0.0/biobb_model/test/__init__.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     6169 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)      678 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)      454 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)       63 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)       12 2023-04-05 08:47:55.000000 biobb_model-4.0.0/biobb_model.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)       38 2023-04-05 08:47:55.000000 biobb_model-4.0.0/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2032 2023-04-05 06:15:38.000000 biobb_model-4.0.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-02 09:59:37.000000 biobb_model-4.0.1/
+-rwxr-xr-x   0 pau        (501) staff       (20)    11358 2021-06-11 09:52:05.000000 biobb_model-4.0.1/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)     6244 2023-06-02 09:59:37.000000 biobb_model-4.0.1/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     5251 2023-06-02 09:55:46.000000 biobb_model-4.0.1/README.md
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model/
+-rwxr-xr-x   0 pau        (501) staff       (20)       63 2023-06-02 09:53:45.000000 biobb_model-4.0.1/biobb_model/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model/model/
+-rwxr-xr-x   0 pau        (501) staff       (20)      157 2022-11-02 12:01:31.000000 biobb_model-4.0.1/biobb_model/model/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5196 2023-04-05 06:36:46.000000 biobb_model-4.0.1/biobb_model/model/checking_log.py
+-rw-r--r--   0 pau        (501) staff       (20)      716 2023-04-05 06:37:11.000000 biobb_model-4.0.1/biobb_model/model/common.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5605 2023-03-23 12:01:36.000000 biobb_model-4.0.1/biobb_model/model/fix_altlocs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5142 2023-03-27 10:29:40.000000 biobb_model-4.0.1/biobb_model/model/fix_amides.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     7211 2023-03-27 09:39:08.000000 biobb_model-4.0.1/biobb_model/model/fix_backbone.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5263 2023-03-27 10:32:27.000000 biobb_model-4.0.1/biobb_model/model/fix_chirality.py
+-rw-r--r--   0 pau        (501) staff       (20)     6145 2023-03-27 10:33:54.000000 biobb_model-4.0.1/biobb_model/model/fix_pdb.py
+-rw-r--r--   0 pau        (501) staff       (20)    46058 2023-04-05 08:36:34.000000 biobb_model-4.0.1/biobb_model/model/fix_pdb_utils.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6148 2023-03-27 10:33:01.000000 biobb_model-4.0.1/biobb_model/model/fix_side_chain.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     5117 2023-03-27 10:28:39.000000 biobb_model-4.0.1/biobb_model/model/fix_ssbonds.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6529 2023-04-04 17:32:15.000000 biobb_model-4.0.1/biobb_model/model/mutate.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model/test/
+-rwxr-xr-x   0 pau        (501) staff       (20)        0 2021-06-11 09:52:05.000000 biobb_model-4.0.1/biobb_model/test/__init__.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     6244 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)      678 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)      454 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)       63 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)       12 2023-06-02 09:59:37.000000 biobb_model-4.0.1/biobb_model.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)       38 2023-06-02 09:59:37.000000 biobb_model-4.0.1/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     1981 2023-06-02 09:54:44.000000 biobb_model-4.0.1/setup.py
```

### Comparing `biobb_model-4.0.0/LICENSE` & `biobb_model-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/PKG-INFO` & `biobb_model-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: biobb_model
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.
 Home-page: https://github.com/bioexcel/biobb_model
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_model.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -54,51 +54,51 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.0.0"
+        pip install "biobb_model>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.0.0"
+        conda install -c bioconda "biobb_model>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
```

### Comparing `biobb_model-4.0.0/README.md` & `biobb_model-4.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -29,51 +30,51 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.0.0"
+        pip install "biobb_model>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.0.0"
+        conda install -c bioconda "biobb_model>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
```

### Comparing `biobb_model-4.0.0/biobb_model/model/checking_log.py` & `biobb_model-4.0.1/biobb_model/model/checking_log.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/common.py` & `biobb_model-4.0.1/biobb_model/model/common.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_altlocs.py` & `biobb_model-4.0.1/biobb_model/model/fix_altlocs.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_amides.py` & `biobb_model-4.0.1/biobb_model/model/fix_amides.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_backbone.py` & `biobb_model-4.0.1/biobb_model/model/fix_backbone.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_chirality.py` & `biobb_model-4.0.1/biobb_model/model/fix_chirality.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_pdb.py` & `biobb_model-4.0.1/biobb_model/model/fix_pdb.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_pdb_utils.py` & `biobb_model-4.0.1/biobb_model/model/fix_pdb_utils.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_side_chain.py` & `biobb_model-4.0.1/biobb_model/model/fix_side_chain.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/fix_ssbonds.py` & `biobb_model-4.0.1/biobb_model/model/fix_ssbonds.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model/model/mutate.py` & `biobb_model-4.0.1/biobb_model/model/mutate.py`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/biobb_model.egg-info/PKG-INFO` & `biobb_model-4.0.1/biobb_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: biobb-model
-Version: 4.0.0
+Version: 4.0.1
 Summary: Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.
 Home-page: https://github.com/bioexcel/biobb_model
 Author: Biobb developers
 Author-email: pau.andrio@bsc.es
 License: UNKNOWN
 Project-URL: Documentation, http://biobb_model.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_model?label=Version)](https://GitHub.com/bioexcel/biobb_model/tags/)
 [![](https://img.shields.io/pypi/v/biobb-model.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-model/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_model?label=Conda)](https://anaconda.org/bioconda/biobb_model)
+[![](https://img.shields.io/conda/dn/bioconda/biobb_model?label=Conda%20downloads)](https://anaconda.org/bioconda/biobb_model)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_model?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_model:4.0.1--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_model)
 [![](https://img.shields.io/pypi/pyversions/biobb-model.svg?label=Python%20Versions)](https://pypi.org/project/biobb-model/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_model)
 
 [![](https://readthedocs.org/projects/biobb-model/badge/?version=latest&label=Docs)](https://biobb-model.readthedocs.io/en/latest/?badge=latest)
@@ -54,51 +54,51 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_model.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA, DOCKER or SINGULARITY.
 
 * Installation:
 
 
-        pip install "biobb_model>=4.0.0"
+        pip install "biobb_model>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_model>=4.0.0"
+        conda install -c bioconda "biobb_model>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-model.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-model.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_model:4.0.0--pyhdfd78af_0 <command>
+        docker run quay.io/biocontainers/biobb_model:4.0.1--pyhdfd78af_0 <command>
 
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
```

### Comparing `biobb_model-4.0.0/biobb_model.egg-info/SOURCES.txt` & `biobb_model-4.0.1/biobb_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_model-4.0.0/setup.py` & `biobb_model-4.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_model",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="pau.andrio@bsc.es",
     description="Biobb_model is the Biobb module collection to check and model 3d structures, create mutations or reconstruct missing atoms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility",
     url="https://github.com/bioexcel/biobb_model",
     project_urls={
         "Documentation": "http://biobb_model.readthedocs.io/en/latest/",
         "Bioexcel": "https://bioexcel.eu/"
     },
     packages=setuptools.find_packages(exclude=['docs', 'test']),
     install_requires=[
         'biobb_common==4.0.0',
-        'biobb_structure_checking==3.12.1',
+        'biobb_structure_checking>=3.13.0',
         'xmltodict'
     ],
-    python_requires='>=3.7,<=3.10',
+    python_requires='>=3.7,<3.10',
     entry_points={
         "console_scripts": [
             "checking_log = biobb_model.model.checking_log:main",
             "fix_chirality = biobb_model.model.fix_chirality:main",
             "fix_amides = biobb_model.model.fix_amides:main",
             "fix_altlocs = biobb_model.model.fix_altlocs:main",
             "fix_ssbonds = biobb_model.model.fix_ssbonds:main",
@@ -38,14 +38,13 @@
         ]
     },
     classifiers=(
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Operating System :: Unix"
     ),
 )
```

