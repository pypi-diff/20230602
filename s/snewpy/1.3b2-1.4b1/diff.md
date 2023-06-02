# Comparing `tmp/snewpy-1.3b2.tar.gz` & `tmp/snewpy-1.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snewpy-1.3b2.tar", last modified: Tue Oct 18 16:25:31 2022, max compression
+gzip compressed data, was "snewpy-1.4b1.tar", last modified: Fri Jun  2 16:36:29 2023, max compression
```

## Comparing `snewpy-1.3b2.tar` & `snewpy-1.4b1.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:25:31.907538 snewpy-1.3b2/
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2022-10-18 16:25:31.907538 snewpy-1.3b2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:25:31.907538 snewpy-1.3b2/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:25:31.907538 snewpy-1.3b2/python/snewpy/
--rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5734 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/_git.py
--rw-r--r--   0 runner    (1001) docker     (121)     6930 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/_model_downloader.py
--rw-r--r--   0 runner    (1001) docker     (121)    85298 2022-10-18 16:25:05.163276 snewpy-1.3b2/python/snewpy/_model_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    45394 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/flavor_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/from_snowglobes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:25:31.907538 snewpy-1.3b2/python/snewpy/models/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13307 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    32514 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/ccsn.py
--rw-r--r--   0 runner    (1001) docker     (121)    30335 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/loaders.py
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/model_files.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/presn.py
--rw-r--r--   0 runner    (1001) docker     (121)     6598 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/models/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/neutrino.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/run_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (121)    23656 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (121)    12194 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/snowglobes_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 16:25:31.907538 snewpy-1.3b2/python/snewpy/test/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3470 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/simplerate_integrationtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/snewpy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_00_init.py
--rw-r--r--   0 runner    (1001) docker     (121)    12230 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_01_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)    12991 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_02_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_03_neutrino.py
--rw-r--r--   0 runner    (1001) docker     (121)    25185 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_04_xforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/test/test_05_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-10-18 16:24:54.899176 snewpy-1.3b2/python/snewpy/to_snowglobes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-10-18 16:24:54.899176 snewpy-1.3b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:36:29.846803 snewpy-1.4b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-06-02 16:36:29.846803 snewpy-1.4b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:36:29.842803 snewpy-1.4b1/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:36:29.846803 snewpy-1.4b1/python/snewpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5671 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/_model_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89954 2023-06-02 16:35:53.014526 snewpy-1.4b1/python/snewpy/_model_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45394 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/flavor_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/from_snowglobes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:36:29.846803 snewpy-1.4b1/python/snewpy/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18095 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33528 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/ccsn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27793 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/model_files.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/models/presn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-02 16:35:41.118435 snewpy-1.4b1/python/snewpy/run_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23637 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/snowglobes_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:36:29.846803 snewpy-1.4b1/python/snewpy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/simplerate_integrationtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/snewpy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_00_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13032 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_01_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_02_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_03_neutrino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25185 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_04_xforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/test/test_05_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-02 16:35:41.122435 snewpy-1.4b1/python/snewpy/to_snowglobes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-02 16:35:41.122435 snewpy-1.4b1/setup.py
```

### Comparing `snewpy-1.3b2/PKG-INFO` & `snewpy-1.4b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: snewpy
-Version: 1.3b2
+Version: 1.4b1
 Summary: A Python package for working with supernova neutrinos
 Home-page: https://github.com/SNEWS2/snewpy
 Author: SNEWS Collaboration
 Author-email: snews2.0@lists.bnl.gov
 License: BSD
 Provides: snewpy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # SNEWPY: Supernova Neutrino Early Warning Models for Python
 
@@ -42,24 +42,14 @@
 
 **Your contributions to SNEWPY are welcome!** For minor changes, simply submit a pull request. If you plan larger changes, it’s probably a good idea to open an issue first to coordinate our work.
 
 To contribute, first clone the repository (`git clone https://github.com/SNEWS2/snewpy.git`), then make changes and install your modified version locally using `pip install .` from the base directory of the repository.
 Once you’re happy with your changes, please submit a pull request.
 Unit tests will run automatically for every pull request or you can run them locally using `python -m unittest python/snewpy/test/test_*.py`.
 
-### Dependencies 
-
-Some functionality of SNEWPY requires that [SNOwGLoBES](https://github.com/SNOwGLoBES/snowglobes) is downloaded.
-In your project directory, run the following commands to get SNOwGLoBES and set it up for use with SNEWPY:
-```bash
-	git clone https://github.com/SNOwGLoBES/snowglobes.git
-	cd snowglobes
-	export SNOWGLOBES=${PWD}
-```
-
 ## Usage and Documentation
 Example scripts which show how SNEWPY can be used are available in the
 `python/snewpy/scripts/` subfolder as well as notebooks in `doc/nb/`.
 Most downloadable models also include a Jupyter notebook with simple usage examples.
 
 A paper describing SNEWPY and the underlying physics is available at [arXiv:2109.08188](https://arxiv.org/abs/2109.08188).
```

### Comparing `snewpy-1.3b2/python/snewpy/__init__.py` & `snewpy-1.4b1/python/snewpy/__init__.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/_git.py` & `snewpy-1.4b1/python/snewpy/_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 #
 """Some code for interacting with git.
 """
 
 import re
-from os.path import abspath, exists, isdir, isfile, join
+from os.path import abspath, isdir, isfile, join
 from setuptools import Command
-from distutils.log import INFO, WARN, ERROR
+from distutils.log import INFO
 
 
 def get_version():
     """Get the value of ``__version__`` without having to import the module.
 
     Returns
     -------
@@ -171,11 +171,10 @@
     def initialize_options(self):
         self.tag = None
 
     def finalize_options(self):
         pass
 
     def run(self):
-        meta = self.distribution.metadata
         update_version(tag=self.tag)
         ver = get_version()
         self.announce("Version is now {}.".format(ver), level=INFO)
```

### Comparing `snewpy-1.3b2/python/snewpy/_model_downloader.py` & `snewpy-1.4b1/python/snewpy/_model_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 available for the models supported by SNEWPY. These data files can either
 be local (in the SNEWPY source tree) or uploaded to a model repository on
 Zenodo. The YAML file supports regular expressions to allow matching of all
 possible model files.
 """
 
 import hashlib
-import re
 import os
 import requests
 import yaml
 
-from contextlib import contextmanager, AbstractContextManager
 from dataclasses import dataclass
 from importlib.resources import open_text
 from pathlib import Path
 from tqdm.auto import tqdm
 from typing import Optional
 
 from snewpy import model_path
@@ -98,18 +96,14 @@
             self.check()
         except FileNotFoundError as e:
             logger.info(f'Downloading file {self.path}')
             _download(self.remote, self.path)
             self.check()
         return self.path
 
-    def open(self, flags='r'):
-        """ Load and open the local file, return the file object"""
-        return open(self.load(), flags)
-
 
 def from_zenodo(zenodo_id:str, model:str, filename:str, path:str=model_path):
     """Access files on Zenodo.
 
     Parameters
     ----------
     zenodo_id : Zenodo record for model files.
@@ -158,30 +152,30 @@
     localpath = Path(path)/str(model)
     localpath.mkdir(exist_ok=True, parents=True)
 
     return FileHandle(path = localpath/filename,
                       remote = github_url)
 
 
-def get_model_data(model:str, filename:str, path:str=model_path):
+def get_model_data(model: str, filename: str, path: str = model_path) -> Path:
     """Access model data. Configuration for each model is in a YAML file
     distributed with SNEWPY.
 
     Parameters
     ----------
     model : Name of the model class for this model file.
     filename : Name of simulation datafile, or a relative path from the model sub-directory
     path : Local installation path (defaults to astropy cache).
 
     Returns
     -------
-    file : FileHandle object.
+    Path of downloaded file.
     """
     if os.path.isabs(filename):
-        return FileHandle(path=Path(filename))
+        return Path(filename)
 
     params = { 'model':model, 'filename':filename, 'path':path }
 
     # Parse YAML file with model repository configurations.
     with open_text('snewpy.models', 'model_files.yml') as f:
         config = yaml.safe_load(f)
         models = config['models']
@@ -189,16 +183,17 @@
         if model in models.keys():
             # Get data from GitHub or Zenodo.
             modconf = models[model]
             repo = modconf['repository']
 
             if repo == 'github':
                 params['release_version'] = modconf['release_version']
-                return from_github(**params)
+                fh = from_github(**params)
             elif repo == 'zenodo':
                 params['zenodo_id'] = modconf['zenodo_id']
-                return from_zenodo(**params)
+                fh = from_zenodo(**params)
             else:
                 raise ValueError(f'Repository {repo} not recognized')
+            return fh.load()
         else:
             raise KeyError(f'No configuration for {model}')
```

### Comparing `snewpy-1.3b2/python/snewpy/_model_urls.py` & `snewpy-1.4b1/python/snewpy/_model_urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,767 +1,812 @@
 model_urls = {
     "Bollig_2016": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/Bollig_2016.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s11.2c_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s11.2c_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s11.2c_LS220_nux",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s27.0c_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s27.0c_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Bollig_2016/s27.0c_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/Bollig_2016.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s11.2c_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s11.2c_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s11.2c_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s27.0c_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s27.0c_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Bollig_2016/s27.0c_LS220_nux",
     ],
     "Fornax_2019": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/Fornax_2019.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/grid.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_10M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_12M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_13M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_14M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_15M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_16M_r250.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_19M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_25M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_60M.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2019/lum_spec_9M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/Fornax_2019.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/grid.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_10M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_12M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_13M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_14M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_15M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_16M_r250.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_19M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_25M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_60M.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2019/lum_spec_9M.h5",
     ],
     "Fornax_2021": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/Fornax_2021.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_12M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_13M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_14M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_15M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_16M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_17M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_18M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_19M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_20M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_21M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_22M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_23M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_25M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_26.99M_r10000_dat.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Fornax_2021/lum_spec_26M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/Fornax_2021.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_12M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_13M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_14M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_15M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_16M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_17M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_18M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_19M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_20M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_21M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_22M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_23M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_25M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_26.99M_r10000_dat.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Fornax_2021/lum_spec_26M_r10000_dat.h5",
     ],
     "Kuroda_2020": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Kuroda_2020/Kuroda_2020.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Kuroda_2020/LnuR00B00.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Kuroda_2020/LnuR10B12.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Kuroda_2020/LnuR10B13.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Kuroda_2020/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Kuroda_2020/Kuroda_2020.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Kuroda_2020/LnuR00B00.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Kuroda_2020/LnuR10B12.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Kuroda_2020/LnuR10B13.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Kuroda_2020/README.md",
     ],
     "Nakazato_2013": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/Nakazato_2013.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-LS220-BH-z0.004-s30.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-BH-z0.004-s30.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s30.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s30.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s13.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s20.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s30.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s50.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Nakazato_2013/nakazato-togashi-BH-z0.004-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/Nakazato_2013.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-LS220-BH-z0.004-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-BH-z0.004-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev100ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev200ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.004-t_rev300ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev100ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev200ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s13.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s20.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s30.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-shen-z0.02-t_rev300ms-s50.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Nakazato_2013/nakazato-togashi-BH-z0.004-s30.0.fits",
     ],
     "OConnor_2013": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/HShen_datafiles.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/HShen_timeseries.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/HShen_timeseries_spectra.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/LS220_datafiles.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/LS220_timeseries.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/LS220_timeseries_spectra.tar.gz",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/OConnor_2013.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2013/read.py",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/HShen_datafiles.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/HShen_timeseries.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/HShen_timeseries_spectra.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/LS220_datafiles.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/LS220_timeseries.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/LS220_timeseries_spectra.tar.gz",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/OConnor_2013.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2013/read.py",
     ],
     "OConnor_2015": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2015/M1_neutrinos.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2015/OConnor_2015.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/OConnor_2015/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2015/M1_neutrinos.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2015/OConnor_2015.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/OConnor_2015/README.md",
     ],
     "PISN": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/PISN_150Msun_EOS=Helm_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/PISN_150Msun_EOS=SFHo_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/PISN_250Msun_EOS=Helm_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/PISN_250Msun_EOS=SFHo_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/PISN/read.py",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/PISN_150Msun_EOS=Helm_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/PISN_150Msun_EOS=SFHo_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/PISN_250Msun_EOS=Helm_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/PISN_250Msun_EOS=SFHo_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/PISN/read.py",
     ],
     "Sukhbold_2015": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/Sukhbold_2015.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/sukhbold-LS220-s27.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/sukhbold-LS220-z9.6.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/sukhbold-SFHo-s27.0.fits",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Sukhbold_2015/sukhbold-SFHo-z9.6.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/Sukhbold_2015.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/sukhbold-LS220-s27.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/sukhbold-LS220-z9.6.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/sukhbold-SFHo-s27.0.fits",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Sukhbold_2015/sukhbold-SFHo-z9.6.fits",
     ],
     "Tamborra_2014": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/Tamborra_2014.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nux",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/Tamborra_2014.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s11.2c_3D_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s11.2c_3D_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s11.2c_3D_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s20.0c_3D_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir2_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir3_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir3_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Tamborra_2014/s27.0c_3D_dir3_LS220_nux",
     ],
     "Type_Ia": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Type_Ia/DDT_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Type_Ia/GCD_NeutrinoFlux.tar.bz2",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Type_Ia/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Type_Ia/DDT_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Type_Ia/GCD_NeutrinoFlux.tar.bz2",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Type_Ia/README.md",
     ],
     "Walk_2018": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2018/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2018/Walk_2018.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/Walk_2018.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir2_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir3_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir3_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_fastrot_dir3_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir2_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir3_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir3_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_nonrot_dir3_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir2_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir3_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir3_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2018/s15.0c_3D_slowrot_dir3_LS220_nux",
     ],
     "Walk_2019": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2019/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2019/Walk_2019.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nue",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nuebar",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/Walk_2019.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir2_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir3_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir3_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s40.0c_3DBH_dir3_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir1_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir1_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir1_LS220_nux",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir2_LS220_nue",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir2_LS220_nuebar",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Walk_2019/s75.0c_3DBH_dir2_LS220_nux",
     ],
     "Warren_2020": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/Warren_2020.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m100.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m120.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m30.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m31.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m32.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m33.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m35.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m40.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m45.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m50.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m55.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m60.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m70.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m80.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m100.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m120.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m30.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m31.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m32.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m33.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m35.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m40.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m45.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m50.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m55.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m60.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m70.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m80.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m100.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.75.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m120.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.1.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.2.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.3.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.4.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.6.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.7.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.8.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.9.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m30.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m31.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m32.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m33.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m35.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m40.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m45.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m50.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m55.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m60.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m70.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m80.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.0.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.25.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.5.h5",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/Warren_2020.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m10.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m100.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m11.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m12.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m120.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m13.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m14.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m15.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m16.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m17.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m18.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m19.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m20.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m21.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m22.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m23.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m24.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m25.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m26.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m27.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m28.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m29.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m30.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m31.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m32.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m33.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m35.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m40.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m45.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m50.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m55.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m60.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m70.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m80.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.23/stir_multimessenger_a1.23_m9.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m10.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m100.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m11.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m12.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m120.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m13.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m14.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m15.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m16.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m17.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m18.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m19.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m20.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m21.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m22.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m23.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m24.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m25.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m26.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m27.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m28.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m29.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m30.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m31.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m32.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m33.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m35.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m40.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m45.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m50.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m55.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m60.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m70.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m80.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.25/stir_multimessenger_a1.25_m9.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m10.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m100.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m11.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m12.75.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m120.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m13.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m14.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m15.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m16.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m17.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m18.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m19.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m20.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m21.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m22.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m23.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m24.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m25.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m26.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m27.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m28.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.1.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.2.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.3.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.4.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.6.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.7.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.8.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m29.9.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m30.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m31.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m32.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m33.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m35.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m40.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m45.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m50.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m55.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m60.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m70.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m80.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.0.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.25.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.5.h5",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Warren_2020/stir_a1.27/stir_multimessenger_a1.27_m9.75.h5",
     ],
     "Zha_2021": [
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/README.md",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/Zha_2021.ipynb",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s16.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s17.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s18.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s19.89.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s19.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s20.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s21.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s22.39.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s22.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s23.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s24.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s25.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s26.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s30.dat",
-        "https://github.com/SNEWS2/snewpy/raw/v1.3b2/models/Zha_2021/s33.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/README.md",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/Zha_2021.ipynb",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s16.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s17.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s18.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s19.89.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s19.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s20.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s21.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s22.39.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s22.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s23.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s24.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s25.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s26.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s30.dat",
+        "https://github.com/SNEWS2/snewpy/raw/v1.4b1/models/Zha_2021/s33.dat",
     ],
     "presn-models": [
     ],
 }
```

### Comparing `snewpy-1.3b2/python/snewpy/flavor_transformation.py` & `snewpy-1.4b1/python/snewpy/flavor_transformation.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/from_snowglobes.py` & `snewpy-1.4b1/python/snewpy/from_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/models/ccsn.py` & `snewpy-1.4b1/python/snewpy/models/ccsn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 # -*- coding: utf-8 -*-
 """
 The submodule ``snewpy.models.ccsn`` contains models of core-collapse supernovae
 derived from the :class:`SupernovaModel` base class.
 
-You can :ref:`download neutrino fluxes for each of these models <sec-download_models>`
-using ``snewpy.get_models("<model_name>")``.
+Since SNEWPY v1.3, the prefered method is to initialise a model based on its physics parameters.
+Initialisation from a file name is deprecated.
+
+Use the ``param`` class property to view all physics parameters and their possible values:
+
+>>> from snewpy.models.ccsn import Nakazato_2013
+>>> Nakazato_2013.param
+{'progenitor_mass': <Quantity [13., 20., 30., 50.] solMass>,
+ 'revival_time': <Quantity [  0., 100., 200., 300.] ms>,
+ 'metallicity': [0.02, 0.004],
+ 'eos': ['LS220', 'shen', 'togashi']}
+
+For some models, not all combinations of parameters are valid. Use the ``get_param_combinations()``
+class method to get a list of all valid combinations and filter it:
+
+>>> list(params for params in Nakazato_2013.get_param_combinations() if params['eos'] != 'shen')
+[{'progenitor_mass': <Quantity 30. solMass>, 'revival_time': <Quantity 0. ms>,
+  'metallicity': 0.004, 'eos': 'LS220'},
+ {'progenitor_mass': <Quantity 30. solMass>, 'revival_time': <Quantity 0. ms>,
+  'metallicity': 0.004, 'eos': 'togashi'}]
 
 .. _Garching Supernova Archive: https://wwwmpa.mpa-garching.mpg.de/ccsnarchive/
 """
 import logging
 import os
 import re
 import tarfile
 
 import numpy as np
 from astropy import units as u
 from astropy.table import Table
 
 from snewpy.models import loaders
-from .base import PinchedModel
-from .util import check_valid_params, get_param_combinations
+from .base import PinchedModel, _RegistryModel
 
 from warnings import warn
 from functools import wraps
 
 
 def _warn_deprecated_filename_argument(func):
     """Decorator for model.__new__ methods, causing them to issue a deprecation warning
@@ -32,29 +49,31 @@
     """
     @wraps(func)  # Ensures docstrings are preserved
     def decorator(cls, *args, **kwargs):
         filename = args[0] if len(args) > 0 else None  # Assumes filename is first pos. arg if provided
         if filename is not None:
             msg = ''.join(['Initializing this model with a filename is deprecated. ',
                            f'Instead, use keyword arguments {list(cls.param.keys())}. ',
-                           f'See `{cls.__name__}.param`, `{cls.__name__}.param_combinations` for more info.'])
+                           f'See `{cls.__name__}.param`, `{cls.__name__}.get_param_combinations()` for more info.'])
             warn(FutureWarning(msg), stacklevel=2)
         return func(cls, *args, **kwargs)
     return decorator
 
 
-class _RegistryModel():
-    """TODO: empty base class for now?"""
-    pass
-
 class Analytic3Species(PinchedModel):
     """An analytical model calculating spectra given total luminosity,
     average energy, and rms or pinch, for each species.
     """
 
+    param = "There are no input files available for this class. Use `doc/scripts/Analytic.py` in the SNEWPY GitHub repo to create a custom input file."
+
+    def get_param_combinations(cls):
+        print(cls.param)
+        return []
+
     def __init__(self, filename):
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to file with model data.
         """
@@ -70,28 +89,27 @@
     """
 
     param = {'progenitor_mass': [13, 20, 30, 50] * u.Msun,
              'revival_time': [0, 100, 200, 300] * u.ms,
              'metallicity': [0.02, 0.004],
              'eos': ['LS220', 'shen', 'togashi']}
 
-    _isvalid_combo = lambda p: (p['revival_time'] == 0 * u.ms and p['progenitor_mass'] == 30 * u.Msun and
-                                p['metallicity'] == 0.004) or \
-                               (p['revival_time'] != 0 * u.ms and p['eos'] == 'shen' and
-                                not (p['progenitor_mass'] == 30 * u.Msun and p['metallicity'] == 0.004))
-    param_combinations = get_param_combinations(param, _isvalid_combo)
+    _param_validator = lambda p: (p['revival_time'] == 0 * u.ms and p['progenitor_mass'] == 30 * u.Msun
+                                  and p['metallicity'] == 0.004) or \
+                                 (p['revival_time'] != 0 * u.ms and p['eos'] == 'shen'
+                                  and not (p['progenitor_mass'] == 30 * u.Msun and p['metallicity'] == 0.004))
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, *, progenitor_mass=None, revival_time=None, metallicity=None, eos=None):
         """Model initialization.
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to FITS file with model data. This argument will be deprecated.
+            Absolute or relative path to FITS file with model data. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
         revival_time: astropy.units.Quantity
             Time of shock revival in model in units ms. Valid values are {revival_time}.
@@ -105,18 +123,18 @@
         ------
         ValueError
             If a combination of parameters is invalid when loading from parameters
 
         Examples
         --------
         >>> from snewpy.models.ccsn import Nakazato_2013; import astropy.units as u
-        >>> Nakazato_2013(progenitor_mass=13*u.Msun, metallicity=0.004, revival_time=0*u.s, eos='togashi')
+        >>> Nakazato_2013(progenitor_mass=30*u.Msun, metallicity=0.004, revival_time=0*u.s, eos='togashi')
         Nakazato_2013 Model: nakazato-togashi-BH-z0.004-s30.0.fits
         Progenitor mass  : 30.0 solMass
-        EOS              : Togashi
+        EOS              : togashi
         Metallicity      : 0.004
         Revival time     : 0.0 ms
         """
         # Attempt to load model from parameters
         if filename is not None:
             metadata = {'Progenitor mass': float(filename.split('-')[-1].strip('s%.fits')) * u.Msun}
             if 't_rev' in filename:
@@ -132,15 +150,15 @@
                     'Metallicity': float(filename.split('-')[-2].strip('z%')),
                     'Revival time': 0 * u.ms
                 })
             return loaders.Nakazato_2013(os.path.abspath(filename), metadata)
 
         # Load from model parameters
         user_params = dict(zip(cls.param.keys(), (progenitor_mass, revival_time, metallicity, eos)))
-        check_valid_params(cls, **user_params)
+        cls.check_valid_params(cls, **user_params)
 
         # Store model metadata.
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': eos,
             'Metallicity': metallicity,
             'Revival time': revival_time
@@ -163,24 +181,22 @@
 
 class Sukhbold_2015(_RegistryModel):
     """Model based on simulations from Sukhbold et al., ApJ 821:38,2016. Models were shared privately by email.
     """
     param = {'progenitor_mass': [27., 9.6] * u.Msun,
              'eos': ['LS220', 'SFHo']}
 
-    param_combinations = get_param_combinations(param)
-
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, *, progenitor_mass=None, eos=None):
         """Model Initialization
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to FITS file with model data. This argument will be deprecated.
+            Absolute or relative path to FITS file with model data. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
         eos: str
             Equation of state. Valid values are {eos}.
@@ -196,15 +212,15 @@
             metadata = {
                 'Progenitor mass': float(filename.split('-')[-1].strip('z%.fits')) * u.Msun,
                 'EOS': filename.split('-')[-2]
             }
             return loaders.Sukhbold_2015(os.path.abspath(filename), metadata)
 
         user_params = dict(zip(cls.param.keys(), (progenitor_mass, eos)))
-        check_valid_params(cls, **user_params)
+        cls.check_valid_params(cls, **user_params)
 
         if progenitor_mass.value == 9.6:
             filename = f'sukhbold-{eos}-z{progenitor_mass.value:3.1f}.fits'
         else:
             filename = f'sukhbold-{eos}-s{progenitor_mass.value:3.1f}.fits'
 
         metadata = {
@@ -218,25 +234,28 @@
 
 
 class Tamborra_2014(_RegistryModel):
     """Model based on 3D simulations from `Tamborra et al., PRD 90:045032, 2014 <https://arxiv.org/abs/1406.0006>`_.
     Data files are from the `Garching Supernova Archive`_.
     """
 
-    param = {'progenitor_mass': [20., 27.] * u.Msun}
-    param_combinations = get_param_combinations(param)
-
+    param = {'progenitor_mass': [11.2, 20., 27.] * u.Msun,
+             'direction': [1,2,3]}
+    _param_validator = lambda p: (p['progenitor_mass'] == 11.2 * u.Msun and p['direction'] in (1,)) or \
+        (p['progenitor_mass'] == 20. * u.Msun and p['direction'] in (1,)) or \
+        (p['progenitor_mass'] == 27. * u.Msun and p['direction'] in (1,2,3))
+    
     @_warn_deprecated_filename_argument
-    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None):
+    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None, direction=None):
         if filename is not None:
             # Metadata creation is implemented in snewpy.models.base._GarchingArchiveModel
             return loaders.Tamborra_2014(os.path.abspath(filename))
 
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
-        filename = f's{progenitor_mass.value:3.1f}c_3D_dir1'
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass, direction=direction)
+        filename = f's{progenitor_mass.value:3.1f}c_3D_dir{direction}'
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': 'LS220'
         }
 
         # Metadata is handled by __init__ in _GarchingArchiveModel
@@ -244,26 +263,25 @@
 
     # Populate Docstring with param values
     __new__.__doc__ = loaders.Tamborra_2014.__init__.__doc__.format(**param)
 
 
 class Bollig_2016(_RegistryModel):
     """Model based on simulations from `Bollig et al. (2016) <https://arxiv.org/abs/1508.00785>`_.
-    Models were taken, with permission, from the Garching Supernova Archive.
+    Models were taken, with permission, from the `Garching Supernova Archive`_.
     """
 
     param = {'progenitor_mass': [11.2, 27.] * u.Msun}
-    param_combinations = get_param_combinations(param)
 
     def __new__(cls, filename=None,  eos='LS220', *, progenitor_mass=None):
         if filename is not None:
             # Metadata creation is implemented in snewpy.models.base._GarchingArchiveModel
             return loaders.Bollig_2016(os.path.abspath(filename))
 
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass)
         filename = f's{progenitor_mass.value:3.1f}c'
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': 'LS220'
         }
 
@@ -275,25 +293,24 @@
 
 class Walk_2018(_RegistryModel):
     """Model based on SASI-dominated simulations from `Walk et al.,
     PRD 98:123001, 2018 <https://arxiv.org/abs/1807.02366>`_. Data files are from
     the `Garching Supernova Archive`_.
     """
 
-    param = {'progenitor_mass': 15. * u.Msun}
-    param_combinations = get_param_combinations(param)
+    param = {'progenitor_mass': 15. * u.Msun, 'rotation': ['fast','slow','non'], 'direction': [1,2,3]}
 
     @_warn_deprecated_filename_argument
-    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None):
+    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None, rotation=None, direction=None):
         if filename is not None:
             # Metadata creation is implemented in snewpy.models.base._GarchingArchiveModel
             return loaders.Walk_2018(os.path.abspath(filename))
 
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
-        filename = f's{progenitor_mass.value:3.1f}c_3D_nonrot_dir1'
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass, rotation=rotation, direction=direction)
+        filename = f's{progenitor_mass.value:3.1f}c_3D_{rotation}rot_dir{direction}'
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': 'LS220'
         }
 
         return loaders.Walk_2018(filename=filename, metadata=metadata)
@@ -304,61 +321,61 @@
 
 class Walk_2019(_RegistryModel):
     """Model based on SASI-dominated simulations from `Walk et al.,
     PRD 101:123013, 2019 <https://arxiv.org/abs/1910.12971>`_. Data files are
     from the `Garching Supernova Archive`_.
     """
 
-    param = {'progenitor_mass': 40 * u.Msun}
-    param_combinations = get_param_combinations(param)
-
+    param = {'progenitor_mass': [40., 75.] * u.Msun,
+             'direction': [1,2,3]}
+    _param_validator = lambda p: (p['progenitor_mass'] == 75. * u.Msun and p['direction'] in (1,2)) or \
+        (p['progenitor_mass'] == 40. * u.Msun and p['direction'] in (1,2,3))
+    
     @_warn_deprecated_filename_argument
-    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None):
+    def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None, direction=None):
         if filename is not None:
             # Metadata creation is implemented in snewpy.models.base._GarchingArchiveModel
             return loaders.Walk_2019(os.path.abspath(filename))
 
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
-        filename = f's{progenitor_mass.value:3.1f}c_3DBH_dir1'
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass, direction=direction)
+        filename = f's{progenitor_mass.value:3.1f}c_3DBH_dir{direction}'
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': 'LS220'
         }
 
         return loaders.Walk_2019(filename=filename, metadata=metadata)
 
     # Populate Docstring with param values (Docstring is inherited from base._GarchingArchiveModel.__init__)
     __new__.__doc__ = loaders.Walk_2019.__init__.__doc__.format(**param)
 
 
-class OConnor_2013(PinchedModel):
+class OConnor_2013(_RegistryModel):
     """Model based on the black hole formation simulation in `O'Connor & Ott (2013) <https://arxiv.org/abs/1207.1100>`_.
     """
 
     param = {'progenitor_mass': (list(range(12, 34)) +
                                  list(range(35, 61, 5)) +
                                  [70, 80, 100, 120]) * u.Msun,
              'eos': ['HShen', 'LS220']}
-    param_combinations = get_param_combinations(param)
 
     _param_abbrv = {'progenitor_mass': '[12..33, 35..5..60, 70, 80, 100, 120] solMass',
                     'eos': ['HShen', 'LS220']}
 
     @_warn_deprecated_filename_argument
     def __new__(cls, base=None, mass=None, eos='LS220', *, progenitor_mass=None):
         """Model Initialization.
 
         Parameters
         ----------
         base : str
-            Absolute or relative path folder with model data. This argument will be deprecated.
-            TODO: (For v2.0) Change base to filename, move compressed model files to OCOnnor_2013 model folder
+            Absolute or relative path folder with model data. This argument is deprecated.
         mass: int
-            Mass of model progenitor in units Msun. This argument will be deprecated.
+            Mass of model progenitor in units Msun. This argument is deprecated.
         eos: str
             Equation of state. Valid values are {eos}.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
@@ -367,17 +384,18 @@
         ------
         FileNotFoundError
             If a file for the chosen model parameters cannot be found
         ValueError
             If a combination of parameters is invalid when loading from parameters
 
         """
+        # TODO: (For v2.0) Change `base` to filename, move compressed model files to OConnor_2013 model folder
         if mass is not None:
-            warn(f'Argument `mass` of type int will be deprecated. To initialize this model, use keyword arguments '
-                 f'{list(cls.param.keys())}. See {cls.__name__}.param, {cls.__name__}.param_combinations for more info',
+            warn(f'Argument `mass` of type int is deprecated. To initialize this model, use keyword arguments '
+                 f'{list(cls.param.keys())}. See {cls.__name__}.param, {cls.__name__}.get_param_combinations() for more info',
                  category=DeprecationWarning, stacklevel=2)
         else:
             mass = 15  # Default Value, this is handled this way for backwards compatibility -- TODO (For V2.0) Remove
 
         if base is not None:
             # If base is provided, do not attempt to load from param.
             if mass * u.Msun not in cls.param['progenitor_mass']:
@@ -386,45 +404,44 @@
             metadata = {'Progenitor mass': progenitor_mass if progenitor_mass is not None else mass * u.Msun,
                         'EOS': eos}
 
             filename = os.path.join(base, f"{eos}_timeseries.tar.gz")
             return loaders.OConnor_2013(os.path.abspath(filename), metadata)
 
         # Load from Parameters
-        check_valid_params(cls, progenitor_mass=progenitor_mass, eos=eos)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass, eos=eos)
         filename = f'{eos}_timeseries.tar.gz'
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': eos,
         }
 
         return loaders.OConnor_2013(filename=filename, metadata=metadata)
 
     # Populate Docstring with param values
-    # __new__.__doc__ = __new__.__doc__.format(**_param_abbrv)
+    __new__.__doc__ = __new__.__doc__.format(**_param_abbrv)
 
 
 class OConnor_2015(_RegistryModel):
     """Model based on the black hole formation simulation in `O'Connor (2015) <https://arxiv.org/abs/1411.7058>`_.
     """
 
     param = {'progenitor_mass': 40 * u.Msun}
-    param_combinations = get_param_combinations(param)
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, eos='LS220', *, progenitor_mass=None):
         """Model Initialization.
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to tar.gz file with model data. This argument will be deprecated.
+            Absolute or relative path to tar.gz file with model data. This argument is deprecated.
         eos: str
-            Equation of state. Valid value is 'LS220'. This argument will be deprecated.
+            Equation of state. Valid value is 'LS220'. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
 
         Raises
@@ -439,43 +456,42 @@
             'EOS': 'LS220',
         }
 
         if filename is not None:
             return loaders.OConnor_2015(os.path.abspath(filename), metadata)
 
         # Load from Parameters
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass)
         # Filename is currently the same regardless of parameters
         filename = 'M1_neutrinos.dat'
 
         return loaders.OConnor_2015(filename, metadata)
 
     # Populate Docstring with param values
     __new__.__doc__ = __new__.__doc__.format(**param)
 
 
 class Zha_2021(_RegistryModel):
     """Model based on the hadron-quark phse transition models from `Zha et al. 2021 <https://arxiv.org/abs/2103.02268>`_.
     """
 
     param = {'progenitor_mass': (list(range(16, 27)) + [19.89, 22.39, 30, 33]) * u.Msun}
-    param_combinations = get_param_combinations(param)
 
     _param_abbrv = {'progenitor_mass': '[16..26, 19.89, 22.39, 30, 33] solMass'}
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, eos='ST0S_B145', *, progenitor_mass=None):
         """Model Initialization.
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to file with model data. This argument will be deprecated.
+            Absolute or relative path to file with model data. This argument is deprecated.
         eos : str
-            Equation of state. Valid value is 'ST0S_B145'. This argument will be deprecated.
+            Equation of state. Valid value is 'ST0S_B145'. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
 
         Raises
@@ -487,15 +503,15 @@
         """
         if filename is not None:
             metadata = {'Progenitor mass': float(os.path.splitext(os.path.basename(filename))[0][1:]) * u.Msun,
                         'EOS': 'STOS_B145'}
             return loaders.Zha_2021(os.path.abspath(filename), metadata)
 
         # Load from Parameters
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass)
 
         metadata = {
             'Progenitor mass': progenitor_mass,
             'EOS': 'STOS_B145',
         }
 
         filename = f's{progenitor_mass.value:g}.dat'
@@ -515,29 +531,28 @@
     param = {'progenitor_mass': np.concatenate((np.linspace(9.0, 12.75, 16),
                                                 np.linspace(13, 30., 171),
                                                 np.linspace(31., 33., 3),
                                                 np.linspace(35, 55, 5),
                                                 np.linspace(60, 80, 3),
                                                 np.linspace(100, 120, 2))) * u.Msun,
              'turbmixing_param': [1.23, 1.25, 1.27]}
-    param_combinations = get_param_combinations(param)
 
     _param_abbrv = {'progenitor_mass': '[9..0.25..13, 13..0.1..30, 31..35, 35..5..60, 70..10..90, 100, 120] solMass',
                     'turbmixing_param': [1.23, 1.25, 1.27]}
 
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, eos='SFHo', *, progenitor_mass=None, turbmixing_param=None):
         """
         Parameters
         ----------
         filename : str
-            Absolute or relative path to file with model data. This argument will be deprecated.
+            Absolute or relative path to file with model data. This argument is deprecated.
         eos : str
-            Equation of state. Valid value is 'SFHo'. This argument will be deprecated.
+            Equation of state. Valid value is 'SFHo'. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
         turbmixing_param: float
             Turbulent mixing parameter alpha_lambda. Valid Values are {turbmixing_param}
@@ -555,15 +570,15 @@
                         'Turb. mixing param.': float(turbmixing_param[1:]),
                         'EOS': 'SFHo'}
 
             return loaders.Warren_2020(os.path.abspath(filename), metadata)
 
         # Load from Parameters
         user_params = dict(zip(cls.param.keys(), (progenitor_mass, turbmixing_param)))
-        check_valid_params(cls, **user_params)
+        cls.check_valid_params(cls, **user_params)
 
         if progenitor_mass.value.is_integer() and progenitor_mass.value <= 30.:
             fname = os.path.join(f'stir_a{turbmixing_param:3.2f}',
                                  f'stir_multimessenger_a{turbmixing_param:3.2f}_m{progenitor_mass.value:.1f}.h5')
         else:
             fname = os.path.join(f'stir_a{turbmixing_param:3.2f}',
                                  f'stir_multimessenger_a{turbmixing_param:3.2f}_m{progenitor_mass.value:g}.h5')
@@ -582,30 +597,29 @@
 
 
 class Kuroda_2020(_RegistryModel):
     """Model based on simulations from `Kuroda et al. (2020) <https://arxiv.org/abs/2009.07733>`_."""
 
     param = {'rotational_velocity': [0, 1] * u.rad / u.s,
              'magnetic_field_exponent': [0, 12, 13]}
-    _isvalid_combo = lambda p: (p['rotational_velocity'].value == 1 and p['magnetic_field_exponent'] in (12, 13)) or \
+    _param_validator = lambda p: (p['rotational_velocity'].value == 1 and p['magnetic_field_exponent'] in (12, 13)) or \
                                (p['rotational_velocity'].value == 0 and p['magnetic_field_exponent'] == 0)
-    param_combinations = get_param_combinations(param, _isvalid_combo)
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, eos='LS220', mass=20*u.Msun, *, rotational_velocity=None,
                 magnetic_field_exponent=None):
         """
         Parameters
         ----------
         filename : str
-            Absolute or relative path to file with model data. This argument will be deprecated.
+            Absolute or relative path to file with model data. This argument is deprecated.
         eos : str
-            Equation of state. Valid value is 'LS220'. This argument will be deprecated.
+            Equation of state. Valid value is 'LS220'. This argument is deprecated.
         mass: astropy.units.Quantity
-            Mass of model progenitor in units Msun. Valid value is 20 * u.Msun. This argument will be deprecated.
+            Mass of model progenitor in units Msun. Valid value is 20 * u.Msun. This argument is deprecated.
 
         Other Parameters
         ----------------
         rotational_velocity: astropy.units.Quantity
             Rotational velocity of progenitor. Valid values are {rotational_velocity}
         magnetic_field_exponent: int
             Exponent of magnetic field (See Eq. 46). Valid Values are {magnetic_field_exponent}
@@ -625,16 +639,16 @@
                 'Rotational Velocity': int(rotational_velocity[0]),
                 'B_0 Exponent': int(magnetic_field_exponent),
                 'EOS': 'LS220'
             }
             return loaders.Kuroda_2020(os.path.abspath(filename), metadata)
 
         # Load from Parameters
-        check_valid_params(cls, rotational_velocity=rotational_velocity,
-                           magnetic_field_exponent=magnetic_field_exponent)
+        cls.check_valid_params(cls, rotational_velocity=rotational_velocity,
+                               magnetic_field_exponent=magnetic_field_exponent)
         filename = f'LnuR{int(rotational_velocity.value):1d}0B{int(magnetic_field_exponent):02d}.dat'
 
         metadata = {
             'Progenitor mass': 20 * u.Msun,
             'Rotational Velocity': rotational_velocity,
             'B_0 Exponent': magnetic_field_exponent,
             'EOS': 'LS220',
@@ -646,24 +660,23 @@
 
 
 class Fornax_2019(_RegistryModel):
     """Model based on 3D simulations from D. Vartanyan, A. Burrows, D. Radice, M.  A. Skinner and J. Dolence, MNRAS 482(1):351, 2019. 
        Data available at https://www.astro.princeton.edu/~burrows/nu-emissions.3d/
     """
     param = {'progenitor_mass': [9, 10, 12, 13, 14, 15, 16, 19, 25, 60] * u.Msun}
-    param_combinations = get_param_combinations(param)
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, cache_flux=False, *, progenitor_mass=None, ):
         """Model Initialization.
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to file with model data. This argument will be deprecated.
+            Absolute or relative path to file with model data. This argument is deprecated.
         cache_flux : bool
             If true, pre-compute the flux on a fixed angular grid and store the values in a FITS file.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
@@ -672,15 +685,15 @@
             progenitor_mass = os.path.splitext(os.path.basename(filename))[0].split('_')[2]
             metadata = {'Progenitor mass': int(progenitor_mass[:-1]) * u.Msun}
             return loaders.Fornax_2019(os.path.abspath(filename), metadata, cache_flux=cache_flux)
 
         # Load from Parameters
         metadata = {'Progenitor mass': progenitor_mass}
 
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass)
         if progenitor_mass.value == 16:
             filename = f'lum_spec_{int(progenitor_mass.value):d}M_r250.h5'
         else:
             filename = f'lum_spec_{int(progenitor_mass.value):d}M.h5'
 
         return loaders.Fornax_2019(filename, metadata, cache_flux=cache_flux)
 
@@ -689,39 +702,38 @@
 
 
 class Fornax_2021(_RegistryModel):
     """Model based on 3D simulations from D. Vartanyan, A. Burrows, D. Radice, M.  A. Skinner and J. Dolence, MNRAS 482(1):351, 2019. 
        Data available at https://www.astro.princeton.edu/~burrows/nu-emissions.3d/
         """
     param = {'progenitor_mass': (list(range(12, 24)) + [25, 26, 26.99]) * u.Msun}
-    param_combinations = get_param_combinations(param)
 
     _param_abbrv = {'progenitor_mass': '[12..26, 26.99] solMass'}
 
     @_warn_deprecated_filename_argument
     def __new__(cls, filename=None, *, progenitor_mass=None):
         """Model Initialization.
 
         Parameters
         ----------
         filename : str
-            Absolute or relative path to file with model data. This argument will be deprecated.
+            Absolute or relative path to file with model data. This argument is deprecated.
 
         Other Parameters
         ----------------
         progenitor_mass: astropy.units.Quantity
             Mass of model progenitor in units Msun. Valid values are {progenitor_mass}.
         """
         if filename is not None:
             progenitor_mass = os.path.splitext(os.path.basename(filename))[0].split('_')[2]
             metadata = {'Progenitor mass': float(progenitor_mass[:-1]) * u.Msun}
             return loaders.Fornax_2021(os.path.abspath(filename), metadata)
 
         # Load from Parameters
-        check_valid_params(cls, progenitor_mass=progenitor_mass)
+        cls.check_valid_params(cls, progenitor_mass=progenitor_mass)
         if progenitor_mass.value.is_integer():
             filename = f'lum_spec_{int(progenitor_mass.value):2d}M_r10000_dat.h5'
         else:
             filename = f'lum_spec_{progenitor_mass.value:.2f}M_r10000_dat.h5'
 
         metadata = {'Progenitor mass': progenitor_mass}
```

### Comparing `snewpy-1.3b2/python/snewpy/models/loaders.py` & `snewpy-1.4b1/python/snewpy/models/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,38 +38,23 @@
         Raises
         ------
         FileNotFoundError
             If a file for the chosen model parameters cannot be found
         """
         # Open the requested filename using the model downloader.
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            # Read FITS table using the astropy reader.
-            simtab = Table.read(datafile.path)
+        # Read FITS table using the astropy reader.
+        simtab = Table.read(datafile)
 
         self.filename = os.path.basename(filename)
         super().__init__(simtab, metadata)
 
 
-class Sukhbold_2015(PinchedModel):
-    def __init__(self, filename, metadata={}):
-        """
-        Parameters
-        ----------
-        filename : str
-            Absolute or relative path to FITS file with model data.
-        """
-        # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            # Read FITS table using the astropy reader.
-            simtab = Table.read(datafile.path)
-
-        self.filename = os.path.basename(filename)
-        super().__init__(simtab, metadata)
+class Sukhbold_2015(Nakazato_2013):
+    pass
 
 
 class Tamborra_2014(_GarchingArchiveModel):
     pass
 
 
 class Bollig_2016(_GarchingArchiveModel):
@@ -92,25 +77,23 @@
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to FITS file with model data.
         """
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            # Open luminosity file.
-            with tarfile.open(datafile.path) as tf:
-
-                # Extract luminosity data.
-                dataname = 's{:d}_{}_timeseries.dat'.format(int(metadata['Progenitor mass'].value), metadata['EOS'])
-
-                # Read FITS table using the astropy reader.
-                simtab = ascii.read(tf.extractfile(dataname), names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
-                                                                     'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
-                                                                     'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'])
+        # Open luminosity file.
+        with tarfile.open(datafile) as tf:
+            # Extract luminosity data.
+            dataname = 's{:d}_{}_timeseries.dat'.format(int(metadata['Progenitor mass'].value), metadata['EOS'])
+            # Read FITS table using the astropy reader.
+            simtab = ascii.read(tf.extractfile(dataname), names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
+                                                                    'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
+                                                                    'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'])
+
         simtab['ALPHA_NU_E'] = (2.0 * simtab['E_NU_E'] ** 2 - simtab['RMS_NU_E'] ** 2) / (
                 simtab['RMS_NU_E'] ** 2 - simtab['E_NU_E'] ** 2)
         simtab['ALPHA_NU_E_BAR'] = (2.0 * simtab['E_NU_E_BAR'] ** 2 - simtab['RMS_NU_E_BAR'] ** 2) / (
                 simtab['RMS_NU_E_BAR'] ** 2 - simtab['E_NU_E_BAR'] ** 2)
         simtab['ALPHA_NU_X'] = (2.0 * simtab['E_NU_X'] ** 2 - simtab['RMS_NU_X'] ** 2) / (
                 simtab['RMS_NU_X'] ** 2 - simtab['E_NU_X'] ** 2)
 
@@ -127,56 +110,19 @@
         Parameters
         ----------
         filename : str
             Absolute or relative path to FITS file with model data.
         """
 
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            simtab = Table.read(datafile.path,
-                                names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
-                                       'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
-                                       'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'],
-                                format='ascii')
-
-        header = ascii.read(simtab.meta['comments'], delimiter='=', format='no_header', names=['key', 'val'])
-        tbounce = float(header['val'][0])
-        simtab['TIME'] -= tbounce
-
-        simtab['ALPHA_NU_E'] = (2.0*simtab['E_NU_E']**2 - simtab['RMS_NU_E']**2) / \
-            (simtab['RMS_NU_E']**2 - simtab['E_NU_E']**2)
-        simtab['ALPHA_NU_E_BAR'] = (2.0*simtab['E_NU_E_BAR']**2 - simtab['RMS_NU_E_BAR']**2) / \
-            (simtab['RMS_NU_E_BAR']**2 - simtab['E_NU_E_BAR']**2)
-        simtab['ALPHA_NU_X'] = (2.0*simtab['E_NU_X']**2 - simtab['RMS_NU_X']**2) / \
-            (simtab['RMS_NU_X']**2 - simtab['E_NU_X']**2)
-
-        # SYB: double-check on this factor of 4. Should be factor of 2?
-        simtab['L_NU_X'] /= 4.0
-
-        self.filename = os.path.basename(filename)
-
-        super().__init__(simtab, metadata)
-
-
-class Zha_2021(PinchedModel):
-    def __init__(self, filename, metadata={}):
-        """
-        Parameters
-        ----------
-        filename : str
-            Absolute or relative path to file prefix, we add nue/nuebar/nux
-        """
-        # Open the requested filename using the model downloader.
-        datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            simtab = Table.read(datafile.path,
-                                names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
-                                       'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
-                                       'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'],
-                                format='ascii')
+        simtab = Table.read(datafile,
+                            names=['TIME', 'L_NU_E', 'L_NU_E_BAR', 'L_NU_X',
+                                    'E_NU_E', 'E_NU_E_BAR', 'E_NU_X',
+                                    'RMS_NU_E', 'RMS_NU_E_BAR', 'RMS_NU_X'],
+                            format='ascii')
 
         header = ascii.read(simtab.meta['comments'], delimiter='=', format='no_header', names=['key', 'val'])
         tbounce = float(header['val'][0])
         simtab['TIME'] -= tbounce
 
         simtab['ALPHA_NU_E'] = (2.0*simtab['E_NU_E']**2 - simtab['RMS_NU_E']**2) / \
             (simtab['RMS_NU_E']**2 - simtab['E_NU_E']**2)
@@ -194,54 +140,57 @@
         simtab['L_NU_X'][simtab['L_NU_X'] < 0] = 1
 
         self.filename = os.path.basename(filename)
 
         super().__init__(simtab, metadata)
 
 
+class Zha_2021(OConnor_2015):
+    pass
+
+
 class Warren_2020(PinchedModel):
     def __init__(self, filename, metadata={}):
         """
         Parameters
         ----------
         filename : str
             Absolute or relative path to file prefix, we add nue/nuebar/nux
         """
         # Open the requested filename using the model downloader.
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
 
-        with datafile.open():
-            # Open luminosity file.
-            # Read data from HDF5 files, then store.
-            f = h5py.File(datafile.path, 'r')
-
-            simtab = Table()
-
-            for i in range(len(f['nue_data']['lum'])):
-                if f['sim_data']['shock_radius'][i][1] > 0.00001:
-                    bounce = f['sim_data']['shock_radius'][i][0]
-                    break
-
-            simtab['TIME'] = f['nue_data']['lum'][:, 0] - bounce
-            simtab['L_NU_E'] = f['nue_data']['lum'][:, 1] * 1e51
-            simtab['L_NU_E_BAR'] = f['nuae_data']['lum'][:, 1] * 1e51
-            simtab['L_NU_X'] = f['nux_data']['lum'][:, 1] * 1e51
-            simtab['E_NU_E'] = f['nue_data']['avg_energy'][:, 1]
-            simtab['E_NU_E_BAR'] = f['nuae_data']['avg_energy'][:, 1]
-            simtab['E_NU_X'] = f['nux_data']['avg_energy'][:, 1]
-            simtab['RMS_NU_E'] = f['nue_data']['rms_energy'][:, 1]
-            simtab['RMS_NU_E_BAR'] = f['nuae_data']['rms_energy'][:, 1]
-            simtab['RMS_NU_X'] = f['nux_data']['rms_energy'][:, 1]
-
-            simtab['ALPHA_NU_E'] = (2.0 * simtab['E_NU_E'] ** 2 - simtab['RMS_NU_E'] ** 2) / \
-                (simtab['RMS_NU_E'] ** 2 - simtab['E_NU_E'] ** 2)
-            simtab['ALPHA_NU_E_BAR'] = (2.0 * simtab['E_NU_E_BAR'] ** 2 - simtab['RMS_NU_E_BAR']
-                                        ** 2) / (simtab['RMS_NU_E_BAR'] ** 2 - simtab['E_NU_E_BAR'] ** 2)
-            simtab['ALPHA_NU_X'] = (2.0 * simtab['E_NU_X'] ** 2 - simtab['RMS_NU_X'] ** 2) / \
-                (simtab['RMS_NU_X'] ** 2 - simtab['E_NU_X'] ** 2)
+        # Open luminosity file.
+        # Read data from HDF5 files, then store.
+        f = h5py.File(datafile, 'r')
+
+        simtab = Table()
+
+        for i in range(len(f['nue_data']['lum'])):
+            if f['sim_data']['shock_radius'][i][1] > 0.00001:
+                bounce = f['sim_data']['shock_radius'][i][0]
+                break
+
+        simtab['TIME'] = f['nue_data']['lum'][:, 0] - bounce
+        simtab['L_NU_E'] = f['nue_data']['lum'][:, 1] * 1e51
+        simtab['L_NU_E_BAR'] = f['nuae_data']['lum'][:, 1] * 1e51
+        simtab['L_NU_X'] = f['nux_data']['lum'][:, 1] * 1e51
+        simtab['E_NU_E'] = f['nue_data']['avg_energy'][:, 1]
+        simtab['E_NU_E_BAR'] = f['nuae_data']['avg_energy'][:, 1]
+        simtab['E_NU_X'] = f['nux_data']['avg_energy'][:, 1]
+        simtab['RMS_NU_E'] = f['nue_data']['rms_energy'][:, 1]
+        simtab['RMS_NU_E_BAR'] = f['nuae_data']['rms_energy'][:, 1]
+        simtab['RMS_NU_X'] = f['nux_data']['rms_energy'][:, 1]
+
+        simtab['ALPHA_NU_E'] = (2.0 * simtab['E_NU_E'] ** 2 - simtab['RMS_NU_E'] ** 2) / \
+            (simtab['RMS_NU_E'] ** 2 - simtab['E_NU_E'] ** 2)
+        simtab['ALPHA_NU_E_BAR'] = (2.0 * simtab['E_NU_E_BAR'] ** 2 - simtab['RMS_NU_E_BAR']
+                                    ** 2) / (simtab['RMS_NU_E_BAR'] ** 2 - simtab['E_NU_E_BAR'] ** 2)
+        simtab['ALPHA_NU_X'] = (2.0 * simtab['E_NU_X'] ** 2 - simtab['RMS_NU_X'] ** 2) / \
+            (simtab['RMS_NU_X'] ** 2 - simtab['E_NU_X'] ** 2)
 
         # Set model metadata.
         self.filename = os.path.basename(filename)
 
         super().__init__(simtab, metadata)
 
 
@@ -252,17 +201,16 @@
         ----------
         filename : str
             Absolute or relative path to file prefix, we add nue/nuebar/nux
         """
 
         # Open the requested filename using the model downloader.
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            # Read ASCII data.
-            simtab = Table.read(datafile.path, format='ascii')
+        # Read ASCII data.
+        simtab = Table.read(datafile, format='ascii')
 
         # Get grid of model times.
         simtab['TIME'] = simtab['Tpb[ms]'] << u.ms
         for f in [Flavor.NU_E, Flavor.NU_E_BAR, Flavor.NU_X]:
             fkey = re.sub('(E|X)_BAR', r'A\g<1>', f.name).lower()
             simtab[f'L_{f.name}'] = simtab[f'<L{fkey}>'] * 1e51 << u.erg / u.s
             simtab[f'E_{f.name}'] = simtab[f'<E{fkey}>'] << u.MeV
@@ -384,17 +332,16 @@
             self._flavorkeys = {Flavor.NU_E: 'nu0',
                                 Flavor.NU_E_BAR: 'nu1',
                                 Flavor.NU_X: 'nu2',
                                 Flavor.NU_X_BAR: 'nu2'}
 
             # Open the requested filename using the model downloader.
             datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-            with datafile.open():
-                # Open HDF5 data file.
-                self._h5file = h5py.File(datafile.path, 'r')
+            # Open HDF5 data file.
+            self._h5file = h5py.File(datafile, 'r')
 
             # Get grid of model times in seconds.
             self.time = self._h5file['nu0']['g0'].attrs['time'] * u.s
 
     def _read_fits(self, filename):
         """Read cached angular data from FITS.
 
@@ -652,17 +599,16 @@
         """
         # Set up model metadata.
         self.progenitor_mass = float(filename.split('/')[-1].split('_')[2][:-1]) * u.Msun
         self.metadata = metadata
 
         # Open the requested filename using the model downloader.
         datafile = _model_downloader.get_model_data(self.__class__.__name__, filename)
-        with datafile.open():
-            # Open HDF5 data file.
-            _h5file = h5py.File(datafile.path, 'r')
+        # Open HDF5 data file.
+        _h5file = h5py.File(datafile, 'r')
 
         self.time = _h5file['nu0'].attrs['time'] * u.s
 
         self.luminosity = {}
         self._E = {}
         self._dLdE = {}
         for flavor in Flavor:
```

### Comparing `snewpy-1.3b2/python/snewpy/models/model_files.yml` & `snewpy-1.4b1/python/snewpy/models/model_files.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 # Define remote locations of simulation files for each model.
 #  1. Model data on GitHub must provide the SNEWPY release version.
 #  2. Model data on Zenodo must provide the Zenodo record ID.
 models:
 
     Bollig_2016:
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     Fornax_2019: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     Fornax_2021: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     Kuroda_2020: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     Nakazato_2013: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     OConnor_2013: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     OConnor_2015: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
  
     Sukhbold_2015: 
         repository: github
-        release_version: 1.2
+        release_version: 1.3
  
     Tamborra_2014: 
         repository: github
-        release_version: 1.2
+        release_version: 1.4b1
  
     Walk_2018: 
         repository: github
-        release_version: 1.2
+        release_version: 1.4b1
  
     Walk_2019: 
         repository: github
-        release_version: 1.2
+        release_version: 1.4b1
 
     Warren_2020:
         repository: github
-        release_version: 1.2
+        release_version: 1.3
 
     Zha_2021: 
         repository: github
-        release_version: 1.2
+        release_version: 1.4b1
```

### Comparing `snewpy-1.3b2/python/snewpy/models/presn.py` & `snewpy-1.4b1/python/snewpy/models/presn.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         df = self.df_t(t)
         a, alpha, b = df.T
         Enu = np.expand_dims(E, 1)
         a = np.expand_dims(a, 0)
         alpha = np.expand_dims(alpha, 0)
         b = np.expand_dims(b, 0)
         fluence = a * Enu ** alpha * np.exp(-b * Enu) / (u.MeV * u.s)
-        result = {f: fluence * self.factor[f] for f in flavors}
+        result = {f: fluence.T * self.factor[f] for f in flavors}
         return result
 
 
 class Patton_2017(SupernovaModel):
     """Set up a presupernova model based on 
     [Kelly M. Patton et al 2017 ApJ 851 6, 
      https://doi.org/10.5281/zenodo.2598709]
@@ -99,15 +99,15 @@
         metadata = {'Progenitor Mass': self.progenitor_mass}
         super().__init__(times << u.hour, metadata)
 
     def get_initial_spectra(self, t, E, flavors=Flavor):
         t = np.array(-t.to_value("hour"), ndmin=1)
         E = np.array(E.to_value("MeV"), ndmin=1)
         flux = self.interpolated(t, E) / (u.MeV * u.s)
-        return {f: flux[f].T for f in flavors}
+        return {f: flux[f] for f in flavors}
 
 class Kato_2017(SupernovaModel):
     """Set up a presupernova model based on 
     [Chinami Kato et al 2017 ApJ 848 48]
     """
     def __init__(self, path):
         fluxes = {}
@@ -134,9 +134,9 @@
         metadata = {'Progenitor Mass': self.progenitor_mass}
         super().__init__(times << u.s, metadata)
 
     def get_initial_spectra(self, t, E, flavors=Flavor):
         t = np.array(-t.to_value("s"), ndmin=1)
         E = np.array(E.to_value("MeV"), ndmin=1)
         flux = self.interpolated(t, E) / (u.MeV * u.s)
-        return {f: flux[f].T for f in flavors}
+        return {f: flux[f] for f in flavors}
```

### Comparing `snewpy-1.3b2/python/snewpy/neutrino.py` & `snewpy-1.4b1/python/snewpy/neutrino.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     """Neutrino mass ordering: ``NORMAL`` or ``INVERTED``."""
     NORMAL = 1
     INVERTED = 2
 
 
 class Flavor(IntEnum):
     """Enumeration of CCSN Neutrino flavors."""
-    NU_E = 2
-    NU_E_BAR = 1
-    NU_X = 3
-    NU_X_BAR = 0
+    NU_E = 0
+    NU_X = 1
+    NU_E_BAR = 2
+    NU_X_BAR = 3
     
     def to_tex(self):
         """LaTeX-compatible string representations of flavor."""
         if '_BAR' in self.name:
             return r'$\overline{{\nu}}_{0}$'.format(self.name[3].lower())
         return r'$\{0}$'.format(self.name.lower())
```

### Comparing `snewpy-1.3b2/python/snewpy/snowglobes.py` & `snewpy-1.4b1/python/snewpy/snowglobes.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     times = 0.5*(tstart + tend)
 
     model_times = snmodel.get_time()
     model_tstart = model_times*1.0
     model_tend = model_times*1.0
 
     model_tstart[0] = model_times[0]
-    for i in range(1, len(model_times), 1):
+    for i in range(1, len(model_times)):
         model_tstart[i] = 0.5*(model_times[i]+model_times[i-1])
         model_tend[i-1] = model_tstart[i]
     model_tend[len(model_times)-1] = model_times[-1]
 
     if nbin > 1:
         starting_index = np.zeros(len(times), dtype=np.int64)
         ending_index = np.zeros(len(times), dtype=np.int64)
@@ -251,22 +251,20 @@
                 tb = tend
                 t = times
                 dt = tb-ta
 
             #first time bin of model in requested interval
             osc_spectra = snmodel.get_transformed_spectra(model_times[starting_index[i]], energy, flavor_transformation)
 
-            if dt < model_tend[starting_index[i]]-ta:
-                dt = dt
-            else:
+            if dt >= model_tend[starting_index[i]]-ta:
                 for flavor in Flavor:
                     osc_spectra[flavor] *= (model_tend[starting_index[i]]-ta)
 
                 #intermediate time bins of model in requested interval
-                for j in range(starting_index[i]+1, ending_index[i], 1):
+                for j in range(starting_index[i]+1, ending_index[i]):
                     temp_spectra = snmodel.get_transformed_spectra(model_times[j], energy, flavor_transformation)
                     for flavor in Flavor:
                         osc_spectra[flavor] += temp_spectra[flavor]*(model_tend[j]-model_tstart[j])
 
                 #last time bin of model in requested interval
                 temp_spectra = snmodel.get_transformed_spectra(
                     model_times[ending_index[i]], energy, flavor_transformation)
@@ -314,20 +312,21 @@
             info = tarfile.TarInfo(name=filename)
             info.size = len(output)
             tf.addfile(info, io.BytesIO(output))
 
     return os.path.join(model_dir, tfname)
 
 def simulate(SNOwGLoBESdir, tarball_path, detector_input="all", verbose=False, *, detector_effects=True):
-    """Takes as input the neutrino flux files and configures and runs the supernova script inside SNOwGLoBES, which outputs calculated event rates expected for a given (set of) detector(s). These event rates are given as a function of the neutrino energy and time, for each interaction channel.
+    """Calculate expected event rates for the given neutrino flux files and the given (set of) SNOwGLoBES detector(s).
+    These event rates are given as a function of the neutrino energy and time, for each interaction channel.
 
     Parameters
     ----------
-    SNOwGLoBESdir : str
-        Path to directory where SNOwGLoBES is installed.
+    SNOwGLoBESdir : str or None
+        Path to SNOwGLoBES directory. Set to ``None`` to automatically use the latest supported SNOwGLoBES release.
     tarball_path : str
         Path of compressed .tar file produced e.g. by ``generate_time_series()`` or ``generate_fluence()``.
     detector_input : str
         Name of detector. If ``"all"``, will use all detectors supported by SNOwGLoBES.
     verbose : bool
         [DEPRECATED, DO NOT USE.]
     detector_effects : bool
@@ -378,15 +377,15 @@
         return re_chan_label.sub(gen_label, c) 
 
 def collate(SNOwGLoBESdir, tarball_path, detector_input="", skip_plots=False, verbose=False, remove_generated_files=True, *, smearing=True):
     """Collates SNOwGLoBES output files and generates plots or returns a data table.
 
     Parameters
     ----------
-    SNOwGLoBESdir : str
+    SNOwGLoBESdir : str or None
         [DEPRECATED, DO NOT USE.]
     tarball_path : str
         Path of compressed .tar file produced e.g. by ``generate_time_series()`` or ``generate_fluence()``.
     detector_input : str
         [DEPRECATED, DO NOT USE. SNEWPY will use all detectors included in the tarball.]
     skip_plots: bool
         If False, it gives as output the plot of the energy distribution for each time bin and for each interaction channel.
@@ -478,15 +477,16 @@
                         data = np.concatenate([[index],data])
                         results[filename.name] = {'header':header,'data':data}
                         #optionally plot the results
                         if skip_plots is False:
                             plt.figure(dpi=300)
                             do_plot(table,(flux,det,w,s))
                             filename = tempdir/f'{filename_base}_log_plot.png'
-                            plt.savefig(filename.with_suffix('.png'), dpi=300, bbox_inches='tight')
+                            plt.savefig(filename, dpi=300, bbox_inches='tight')
+                            plt.close()
         #Make a tarfile with the condensed data files and plots
         output_name = Path(tarball_path).stem
         output_name = output_name[:output_name.rfind('.tar')]+'_SNOprocessed'
         output_path = Path(tarball_path).parent/(output_name+'.tar.gz')
         with tarfile.open(output_path, "w:gz") as tar:
             for file in tempdir.iterdir():
                 tar.add(file,arcname=output_name+'/'+file.name)
```

### Comparing `snewpy-1.3b2/python/snewpy/snowglobes_interface.py` & `snewpy-1.4b1/python/snewpy/snowglobes_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-The module ``snewpy.snowglobes_interface`` contains a low-level Python interface for SNOwGLoBES v1.2.
+The module ``snewpy.snowglobes_interface`` contains a low-level Python interface for SNOwGLoBES v1.3.
 
 .. note::
     Users should only use the high-level interface described above.
     This low-level interface is not guaranteed to be stable and may change at
     any time without warning, e.g. to support new SNOwGLoBES versions.
 """
 from pathlib import Path
@@ -12,16 +12,23 @@
 import os
 
 import logging
 logger = logging.getLogger(__name__)
 
 from tqdm.auto import tqdm
 
+import snowglobes_data
+import sys
+if sys.version_info >= (3, 9):
+    from importlib.resources import files
+else:
+    from importlib_resources import files
+
 def guess_material(detector):
-    if detector.startswith('wc') or detector.startswith('ice'):
+    if detector.startswith(('wc', 'ice', 'km3net')):
         mat = 'water'
     elif detector.startswith('d2O'):
         mat = 'heavywater'
     elif detector.startswith('ar'):
         mat = 'argon'
     elif detector.startswith('nova'):
         mat = 'nova_soup'
@@ -64,20 +71,22 @@
         detectors: str
             Name of detector. If ``"all"``, will use all detectors supported by SNOwGLoBES.
 
         detector_effects: bool
             If true, account for efficiency and smearing. If false, consider a perfect detector.
 
         base_dir:         Path or None
-            Path to the directory where the cross-section, detector, and channel files are located
-            If empty, try to get it from ``$SNOWGLOBES`` environment var
+            Path to the directory where the cross-section, detector, and channel files are located.
+            If empty, try to get it from ``$SNOWGLOBES`` environment var or the `snowglobes_data` module.
         """
-        if not base_dir:
-            base_dir = os.environ['SNOWGLOBES']
-        self.base_dir = Path(base_dir)
+        try:
+            self.base_dir = Path(base_dir if base_dir else os.environ['SNOWGLOBES'])
+        except KeyError:
+            print("Using snowglobes_data module ...")
+            self.base_dir = files(snowglobes_data)
         self._load_detectors(self.base_dir/'detector_configurations.dat', detectors)
         self._load_channels(self.base_dir/'channels')
         self.efficiencies = None
         self.smearings = None
         if detector_effects:
             self._load_efficiency_vectors(self.base_dir/'effic')
             self._load_smearing_matrices(self.base_dir/'smear')
@@ -93,58 +102,68 @@
             detectors = [detectors]
 
         self.detectors = df.set_index('name').T.filter(items=detectors)
         logger.info(f'read masses for detectors {list(self.detectors)}')
         logger.debug(f'detectors: {self.detectors}')
        
     def _load_channels(self, chan_dir):
-
-        def _read_binning(fname):
-            with open(fname) as f:
-                l = f.readline().strip()
-                if not l.startswith('%'):
-                    l = '% 200 0.0005 0.100 200 0.0005 0.100'
-                tokens = l.split(' ')[1:]
-                nsamples, smin,smax, nbins,emin,emax = [float(t) for t in tokens]
-                return {'e_true' :np.linspace(smin,smax,int(nsamples)+1),
-                        'e_smear':np.linspace(emin,emax,int(nbins)+1)
-                        }
-
         self.channels = {}
         self.binning = {}
         for f in chan_dir.glob('channels_*.dat'):
             material = f.stem[len('channels_'):]
-            df = pd.read_table(f,delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
+            # in SNOwGLoBES v1.3, there are three different formats of channel files
+            # We identify these based on their first line and read them in separately:
+            with open(f) as _f:
+                l = _f.readline().strip()
+            if l.startswith('%'):
+                # Format 1: explicit binning, same for all channels
+                tokens = l.split()[1:]
+                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
+            elif l.startswith('SN_nu'):
+                # Format 2: explicit binning, differs per channel
+                tokens = l.split()[6:]
+                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'], usecols=range(1,6))
+                # drop coherent scattering channels, which have different binning
+                df = df[df["name"].str.startswith('coh_') == False]
+            else:
+                # Format 3: no binning specified, use SNOwGLoBES default values
+                tokens = '% 200 0.0005 0.100 200 0.0005 0.100'.split()[1:]
+                df = pd.read_table(f, delim_whitespace=True, index_col=1, comment='%', names=['name','n','parity','flavor','weight'])
+
             self.channels[material] = df
-            self.binning[material] = _read_binning(f)
+
+            nsamples, smin, smax, nbins, emin, emax = [float(t) for t in tokens]
+            self.binning[material] = {'e_true': np.linspace(smin, smax, int(nsamples)+1),
+                                      'e_smear': np.linspace(emin, emax, int(nbins)+1)
+                                      }
         self.materials = list(self.channels.keys())
         self.chan_dir = chan_dir
         logger.info(f'read channels for materials: {self.materials}')
         logger.debug(f'channels: {self.channels}')
 
     def _load_efficiency_vectors(self, path):
         result = {}
         for detector in self.detectors:
             res_det = {}
-            for file in path.glob(f'effic_*_{detector}.dat'):
+            for file in (path/str(detector)).glob(f'effic_*_{detector}.dat'):
                 channel =  file.stem[len('effic_'):-len(detector)-1]
                 logger.debug(f'Reading file ({detector},{channel}): {file}')
                 with open(file) as f:
                     effs = np.fromiter(f.readlines()[0].split("{")[-1].split("}")[0].split(","), float)
                     res_det[channel]= effs
             result[detector]=res_det
         self.efficiencies = result 
         logger.info(f'read efficiencies for detectors: {list(self.efficiencies.keys())}')
         logger.debug(f'efficiencies: {self.efficiencies}')
 
     def _load_smearing_matrices(self, path):
         result = {}
         for detector in self.detectors:
             res_det = {}
-            for file in path.glob(f'smear*_{detector}.dat'):
+            for file in (path/str(detector)).glob(f'smear*_{detector}.dat'):
                 channel =  file.stem[len('smear_'):-len(detector)-1]
                 with open(file) as f:
                     lines = f.readlines()[1:-1]
                     while not "{" in lines[0]: lines = lines[1:]
                     while not "{" in lines[-1]: lines = lines[:-1]
                     matrix = np.zeros((len(lines),len(lines)))
                     for i,l in enumerate(lines):
```

### Comparing `snewpy-1.3b2/python/snewpy/test/simplerate_integrationtest.py` & `snewpy-1.4b1/python/snewpy/test/simplerate_integrationtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 """Integration test based on SNEWS2.0_rate_table_singleexample.py
 """
 import unittest
-import os
 from snewpy import snowglobes
 
 
 class TestSimpleRate(unittest.TestCase):
 
     def test_simplerate(self):
         """Integration test based on SNEWS2.0_rate_table_singleexample.py
         """
         # Hardcoded paths on GitHub Action runner machines
-        SNOwGLoBES_path = os.environ['SNOWGLOBES']
+        SNOwGLoBES_path = None
         SNEWPY_model_dir = "models/"
 
         distance = 10  # Supernova distance in kpc
         detector = "wc100kt30prct" #SNOwGLoBES detector for water Cerenkov
         modeltype = 'Bollig_2016' # Model type from snewpy.models
         model = 's11.2c' # Name of model
         transformation = 'AdiabaticMSW_NMO' # Desired flavor transformation
@@ -67,9 +66,9 @@
         sk_expected = 4486.929197175579
         sk_expected_smeared = 4044.841743901513
         sk_computed = 0.32 * total_events
         sk_computed_smeared = 0.32 * total_events_smeared
         discrepancy = abs(sk_computed - sk_expected)/sk_expected
         discrepancy_smeared = abs(sk_computed_smeared - sk_expected_smeared)/sk_expected_smeared
 
-        assert discrepancy < 0.001, f"Number of events computed for SK is {sk_computed}, should be {sk_expected}"
-        assert discrepancy_smeared < 0.001, f"Number of events computed for SK is {sk_computed}, should be {sk_expected}"
+        assert discrepancy < 0.001, f"Number of unsmeared events computed for SK is {sk_computed}, should be {sk_expected}"
+        assert discrepancy_smeared < 0.001, f"Number of smeared events computed for SK is {sk_computed_smeared}, should be {sk_expected_smeared}"
```

### Comparing `snewpy-1.3b2/python/snewpy/test/snewpy_test_suite.py` & `snewpy-1.4b1/python/snewpy/test/snewpy_test_suite.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/test/test_01_registry.py` & `snewpy-1.4b1/python/snewpy/test/test_01_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                   Fornax_2019,
                   Warren_2020,
                   Kuroda_2020,
                   Fornax_2021,
                   Zha_2021]
 
         for model in models:
-            for pc in model.param_combinations:
+            for pc in model.get_param_combinations():
                 model(**pc)  # Initialize
 
     def test_Nakazato_2013(self):
         """
         Instantiate a set of 'Nakazato 2013' models
         """
         for z in [0.004, 0.02]:
@@ -62,29 +62,34 @@
                     self.assertEqual(len(f), len(Flavor))
                     self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Tamborra_2014(self):
         """
         Instantiate a set of 'Tamborra 2014' models
         """
-        for mass in [20., 27.]:
-            model = Tamborra_2014(progenitor_mass=mass*u.Msun, eos='LS220')
-
-            self.assertEqual(model.metadata['EOS'], 'LS220')
-            self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
-
-            # Check that times are in proper units.
-            t = model.get_time()
-            self.assertTrue(t.unit, u.s)
-
-            # Check that we can compute flux dictionaries.
-            f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-            self.assertEqual(type(f), dict)
-            self.assertEqual(len(f), len(Flavor))
-            self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+        for mass in [11.2, 20., 27.]:
+            for angles in [1,2,3]:
+                if mass != 27. and angles > 1:
+                    with self.assertRaises(ValueError):
+                        model = Tamborra_2014(progenitor_mass=mass*u.Msun, eos='LS220', direction=angles)
+                else:
+                    model = Tamborra_2014(progenitor_mass=mass*u.Msun, eos='LS220',direction=angles)
+                    
+                    self.assertEqual(model.metadata['EOS'], 'LS220')
+                    self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
+                    
+                    # Check that times are in proper units.
+                    t = model.get_time()
+                    self.assertTrue(t.unit, u.s)
+                    
+                    # Check that we can compute flux dictionaries.
+                    f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                    self.assertEqual(type(f), dict)
+                    self.assertEqual(len(f), len(Flavor))
+                    self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_OConnor_2013(self):
         """
         Instantiate a set of "O'Connor 2015" models
         """
         for mass in list(range(12, 34)) + list(range(35, 61, 5)) + [70, 80, 100, 120]:
             for eos in ['LS220', 'HShen']:
@@ -165,47 +170,52 @@
             self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Walk_2018(self):
         """
         Instantiate a set of 'Walk 2018' models
         """
         mass = 15.
-        model = Walk_2018(progenitor_mass=mass*u.Msun)
+        for angles in [1,2,3]:
+            for rot in ['fast','slow','non']:
+                model = Walk_2018(progenitor_mass=mass*u.Msun, direction=angles, rotation=rot)
 
-        self.assertEqual(model.metadata['EOS'], 'LS220')
-        self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
+                self.assertEqual(model.metadata['EOS'], 'LS220')
+                self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
 
-        # Check that times are in proper units.
-        t = model.get_time()
-        self.assertTrue(t.unit, u.s)
+                # Check that times are in proper units.
+                t = model.get_time()
+                self.assertTrue(t.unit, u.s)
 
-        # Check that we can compute flux dictionaries.
-        f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-        self.assertEqual(type(f), dict)
-        self.assertEqual(len(f), len(Flavor))
-        self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+                # Check that we can compute flux dictionaries.
+                f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                self.assertEqual(type(f), dict)
+                self.assertEqual(len(f), len(Flavor))
+                self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Walk_2019(self):
         """
         Instantiate a set of 'Walk 2019' models
         """
-        model = Walk_2019(progenitor_mass=40*u.Msun, eos='LS220')
 
-        self.assertEqual(model.metadata['EOS'], 'LS220')
-        self.assertEqual(model.metadata['Progenitor mass'], 40*u.Msun)
+        for mass in [40.,75.]:
+            for angles in [1,2]:
+                model = Walk_2019(progenitor_mass=mass*u.Msun, direction=angles)
 
-        # Check that times are in proper units.
-        t = model.get_time()
-        self.assertTrue(t.unit, u.s)
+                self.assertEqual(model.metadata['EOS'], 'LS220')
+                self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
 
-        # Check that we can compute flux dictionaries.
-        f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-        self.assertEqual(type(f), dict)
-        self.assertEqual(len(f), len(Flavor))
-        self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+                # Check that times are in proper units.
+                t = model.get_time()
+                self.assertTrue(t.unit, u.s)
+
+                # Check that we can compute flux dictionaries.
+                f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                self.assertEqual(type(f), dict)
+                self.assertEqual(len(f), len(Flavor))
+                self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Fornax_2019(self):
         """
         Instantiate a set of 'Fornax 2019' models
         """
         for mass in [9, 10, 12, 13, 14, 15, 19, 25, 60]:
             model = Fornax_2019(progenitor_mass=mass*u.Msun)
```

### Comparing `snewpy-1.3b2/python/snewpy/test/test_02_models.py` & `snewpy-1.4b1/python/snewpy/test/test_02_models.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,26 +44,31 @@
                     self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Tamborra_2014(self):
         """
         Instantiate a set of 'Tamborra 2014' models
         """
         for mass in [20., 27.]:
-            mfile = 'Tamborra_2014/s{:.1f}c_3D_dir1'.format(mass)
-            model = Tamborra_2014(os.path.join(model_path, mfile), eos='LS220')
-
-            # Check that times are in proper units.
-            t = model.get_time()
-            self.assertTrue(t.unit, u.s)
-
-            # Check that we can compute flux dictionaries.
-            f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-            self.assertEqual(type(f), dict)
-            self.assertEqual(len(f), len(Flavor))
-            self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+            for direction in [1, 2, 3]:
+                mfile = 'Tamborra_2014/s{:.1f}c_3D_dir{}'.format(mass, direction)
+                if mass == 20. and direction > 1:
+                    with self.assertRaises(FileNotFoundError):
+                        model = Tamborra_2014(os.path.join(model_path, mfile), eos='LS220')
+                else:
+                    model = Tamborra_2014(os.path.join(model_path, mfile), eos='LS220')
+
+                    # Check that times are in proper units.
+                    t = model.get_time()
+                    self.assertTrue(t.unit, u.s)
+
+                    # Check that we can compute flux dictionaries.
+                    f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                    self.assertEqual(type(f), dict)
+                    self.assertEqual(len(f), len(Flavor))
+                    self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_OConnor_2013(self):
         """
         Instantiate a set of "O'Connor 2015" models
         """
         for mass in list(range(12, 34)) + list(range(35, 61, 5)) + [70, 80, 100, 120]:
             for eos in ['LS220', 'HShen']:
@@ -141,47 +146,50 @@
             self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Walk_2018(self):
         """
         Instantiate a set of 'Walk 2018' models
         """
         mass = 15.
-        mfile = 'Walk_2018/s{:.1f}c_3D_nonrot_dir1'.format(mass)
-        model = Walk_2018(os.path.join(model_path, mfile), eos='LS220')
+        for direction in [1,2,3]:
+            for rot in ['fast','slow','non']:
+                mfile = 'Walk_2018/s{:.1f}c_3D_{}rot_dir{}'.format(mass,rot,direction)
+                model = Walk_2018(os.path.join(model_path, mfile), eos='LS220')
 
-        # Check that times are in proper units.
-        t = model.get_time()
-        self.assertTrue(t.unit, u.s)
+                # Check that times are in proper units.
+                t = model.get_time()
+                self.assertTrue(t.unit, u.s)
 
-        # Check that we can compute flux dictionaries.
-        f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-        self.assertEqual(type(f), dict)
-        self.assertEqual(len(f), len(Flavor))
-        self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+                # Check that we can compute flux dictionaries.
+                f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                self.assertEqual(type(f), dict)
+                self.assertEqual(len(f), len(Flavor))
+                self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Walk_2019(self):
         """
         Instantiate a set of 'Walk 2019' models
         """
-        mass = 40.
-        mfile = 'Walk_2019/s{:.1f}c_3DBH_dir1'.format(mass)
-        model = Walk_2019(os.path.join(model_path, mfile), eos='LS220')
+        for mass in [40.,75.]:
+            for direction in [1,2]:
+                mfile = 'Walk_2019/s{:.1f}c_3DBH_dir{}'.format(mass,direction)
+                model = Walk_2019(os.path.join(model_path, mfile), eos='LS220')
 
-        self.assertEqual(model.metadata['EOS'], 'LS220')
-        self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
+                self.assertEqual(model.metadata['EOS'], 'LS220')
+                self.assertEqual(model.metadata['Progenitor mass'], mass*u.Msun)
 
-        # Check that times are in proper units.
-        t = model.get_time()
-        self.assertTrue(t.unit, u.s)
+                # Check that times are in proper units.
+                t = model.get_time()
+                self.assertTrue(t.unit, u.s)
 
-        # Check that we can compute flux dictionaries.
-        f = model.get_initial_spectra(0*u.s, 10*u.MeV)
-        self.assertEqual(type(f), dict)
-        self.assertEqual(len(f), len(Flavor))
-        self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
+                # Check that we can compute flux dictionaries.
+                f = model.get_initial_spectra(0*u.s, 10*u.MeV)
+                self.assertEqual(type(f), dict)
+                self.assertEqual(len(f), len(Flavor))
+                self.assertEqual(f[Flavor.NU_E].unit, 1/(u.erg * u.s))
 
     def test_Fornax_2019(self):
         """
         Instantiate a set of 'Fornax 2019' models
         """
         for mass in [9, 10, 12, 13, 14, 15, 19, 25, 60]:
             mfile = 'Fornax_2019/lum_spec_{}M.h5'.format(mass)
```

### Comparing `snewpy-1.3b2/python/snewpy/test/test_03_neutrino.py` & `snewpy-1.4b1/python/snewpy/test/test_03_neutrino.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/test/test_04_xforms.py` & `snewpy-1.4b1/python/snewpy/test/test_04_xforms.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/python/snewpy/test/test_05_snowglobes.py` & `snewpy-1.4b1/python/snewpy/test/test_05_snowglobes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
-import numpy as np
-from snewpy.snowglobes import simulate,collate, generate_time_series, generate_fluence, SimpleRate
+from snewpy.snowglobes import generate_fluence, SimpleRate
 from pathlib import Path
 import tarfile
 
 pytestmark=pytest.mark.snowglobes
 
 models = ['Bollig_2016/s11.2c', 'Bollig_2016/s27.0c']
 transformations = ['AdiabaticMSW_NMO','AdiabaticMSW_IMO']
@@ -53,16 +52,7 @@
 
 @pytest.mark.parametrize('detector, expected_total',crosscheck_table)
 def test_simplerate_smear_crosscheck(splr, detector, expected_total):
     flux = './models/Bollig_2016/fluence_Bollig_2016_s11.2c_AdiabaticMSW_NMO.dat'
     data = splr.run(flux,detector)
     total = data[0].weighted.smeared.sum().sum()
     assert total == pytest.approx(expected_total, 0.1)
-
-def process(tarball_name):
-    simulate(None,tarball_name,'icecube')
-    collate(None, tarball_name)
-
-@pytest.mark.timing
-def test_simulation_chain_benchmark(benchmark):
-    tarball_name='./models/Bollig_2016/fluence_Bollig_2016_s27.0c_AdiabaticMSW_IMO.tar.bz2'
-    r = benchmark(process,tarball_name)
```

### Comparing `snewpy-1.3b2/python/snewpy/to_snowglobes.py` & `snewpy-1.4b1/python/snewpy/to_snowglobes.py`

 * *Files identical despite different names*

### Comparing `snewpy-1.3b2/setup.py` & `snewpy-1.4b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,30 +32,30 @@
 #
 # Set other keywords for the setup function.
 #
 # Use entry_points to let `pip` create executable scripts for each target platform.
 # See https://setuptools.readthedocs.io/en/latest/userguide/entry_point.html
 # setup_keywords['entry_points'] = {'console_scripts': ['to_snowglobes = snewpy.to_snowglobes:generate_time_series', ], },
 setup_keywords['provides'] = [setup_keywords['name']]
-setup_keywords['python_requires'] = '>=3.7'
+setup_keywords['python_requires'] = '>=3.8'
 setup_keywords['zip_safe'] = False
 setup_keywords['packages'] = find_packages('python')
 setup_keywords['package_dir'] = {'': 'python'}
 setup_keywords['package_data'] = {'':['templates/*.glb', 'models/*.yml']}
 setup_keywords['cmdclass'] = {'version': SetVersion, 'sdist': DistutilsSdist}
 setup_keywords['test_suite']='snewpy.test.snewpy_test_suite.snewpy_test_suite'
 
 requires = []
 with open('requirements.txt', 'r') as f:
     for line in f:
         if line.strip():
             requires.append(line.strip())
 setup_keywords['install_requires'] = requires
 setup_keywords['extras_require'] = {  # Optional
-    'dev': ['pytest', 'pytest-benchmark'],
+    'dev': ['pytest'],
     'docs':['numpydoc']
 }
 #
 # Internal data directories.
 #
 #setup_keywords['data_files'] = [('snewpy/data/config', glob('data/config/*')),
 #                                ('snewpy/data/spectra', glob('data/spectra/*'))]
```

