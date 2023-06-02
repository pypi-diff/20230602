# Comparing `tmp/utracto-0.0.8.tar.gz` & `tmp/utracto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utracto-0.0.8.tar", last modified: Wed May 10 13:46:33 2023, max compression
+gzip compressed data, was "utracto-0.0.9.tar", last modified: Fri Jun  2 13:37:11 2023, max compression
```

## Comparing `utracto-0.0.8.tar` & `utracto-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.840000 utracto-0.0.8/
--rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-05-10 13:46:34.000000 utracto-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 13:46:34.000000 utracto-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1094 2023-05-10 13:04:52.000000 utracto-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.840000 utracto-0.0.8/utracto/
--rw-rw-rw-   0        0        0       74 2023-05-10 13:46:14.000000 utracto-0.0.8/utracto/__init__.py
--rw-rw-rw-   0        0        0     2703 2023-05-10 13:34:02.000000 utracto-0.0.8/utracto/core.py
--rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.8/utracto/example.py
--rw-rw-rw-   0        0        0     5822 2023-05-10 13:10:26.000000 utracto-0.0.8/utracto/tracking.py
--rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.8/utracto/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:46:33.850000 utracto-0.0.8/utracto.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 13:46:34.000000 utracto-0.0.8/utracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 13:37:11.730000 utracto-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3251 2023-06-02 13:37:12.000000 utracto-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2750 2023-05-12 14:07:10.000000 utracto-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 13:37:12.000000 utracto-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1120 2023-05-12 14:08:56.000000 utracto-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:37:11.740000 utracto-0.0.9/utracto/
+-rw-rw-rw-   0        0        0       74 2023-06-02 13:33:22.000000 utracto-0.0.9/utracto/__init__.py
+-rw-rw-rw-   0        0        0     2704 2023-05-12 14:32:10.000000 utracto-0.0.9/utracto/core.py
+-rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.9/utracto/example.py
+-rw-rw-rw-   0        0        0     5822 2023-05-10 13:10:26.000000 utracto-0.0.9/utracto/tracking.py
+-rw-rw-rw-   0        0        0     5191 2023-05-12 14:08:04.000000 utracto-0.0.9/utracto/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 13:37:11.750000 utracto-0.0.9/utracto.egg-info/
+-rw-rw-rw-   0        0        0     3251 2023-06-02 13:37:12.000000 utracto-0.0.9/utracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-02 13:37:12.000000 utracto-0.0.9/utracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 13:37:12.000000 utracto-0.0.9/utracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-02 13:37:12.000000 utracto-0.0.9/utracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 13:37:12.000000 utracto-0.0.9/utracto.egg-info/top_level.txt
```

### Comparing `utracto-0.0.8/LICENSE` & `utracto-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `utracto-0.0.8/PKG-INFO` & `utracto-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.8
+Version: 0.0.9
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -29,17 +29,59 @@
   <img src="https://user-images.githubusercontent.com/70629561/207111838-6ec3ba60-fd52-47ad-a469-17a29df74513.png" width="600" />
 </p>
 
 This angular map is to be used with a forked version of [DIPY](https://github.com/DelinteNicolas/dipy).
 
 ## Installing & importing
 
+### Online install
+
+The UNRAVEL package is available through ```pip install``` under the name ```utracto```. Note that the online version might not always be up to date with the latest changes.
+
+```
+pip install utracto
+```
+To upgrade the current version : ```pip install utracto --upgrade```.
+
+To install a specific version of the package use
+```
+pip install utracto==0.0.8
+```
+All available versions are listed in [PyPI](https://pypi.org/project/utracto/). The package names follow the rules of [semantic versioning](https://semver.org/).
+
 ### Local install
 
 If you want to download the latest version directly from GitHub, you can clone this repository
 ```
 git clone https://github.com/DelinteNicolas/UTracto.git
 ```
+For a more frequent use of the library, you may wish to permanently add the package to your current Python environment. Navigate to the folder where this repository was cloned or downloaded (the folder containing the ```setup.py``` file) and install the package as follows
+```
+cd UTracto
+pip install .
+```
+
+If you have an existing install, and want to ensure package and dependencies are updated use --upgrade
+```
+pip install --upgrade .
+```
+### Importing
+At the top of your Python scripts, import the library as
+```
+import utracto
+```
+
+### Checking current version installed
+
+The version of the UNRAVEL package installed can be displayed by typing the following command in your python environment
+```
+utracto.__version__
+``` 
+
+### Uninstalling
+```
+pip uninstall utracto
+```
 
 ## Example data and code
 
 An example use of the main methods and outputs of UTracto is written in the `example.py` file.
```

### Comparing `utracto-0.0.8/README.md` & `utracto-0.0.9/utracto.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: utracto
+Version: 0.0.9
+Summary: Implementation of UTracto
+Home-page: https://github.com/DelinteNicolas/UTracto
+Author: Nicolas Delinte
+Author-email: nicolas.delinte@uclouvain.be
+License: GNU General Public License v3.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # U-fiber tractography
 
 Welcome to the UTracto's Github repository!
 
 [![PyPI](https://img.shields.io/pypi/v/utracto?label=pypi%20package)](https://pypi.org/project/utracto/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/utracto)](https://pypi.org/project/utracto/)
 ![GitHub repo size](https://img.shields.io/github/repo-size/DelinteNicolas/UTracto)
@@ -14,17 +29,59 @@
   <img src="https://user-images.githubusercontent.com/70629561/207111838-6ec3ba60-fd52-47ad-a469-17a29df74513.png" width="600" />
 </p>
 
 This angular map is to be used with a forked version of [DIPY](https://github.com/DelinteNicolas/dipy).
 
 ## Installing & importing
 
+### Online install
+
+The UNRAVEL package is available through ```pip install``` under the name ```utracto```. Note that the online version might not always be up to date with the latest changes.
+
+```
+pip install utracto
+```
+To upgrade the current version : ```pip install utracto --upgrade```.
+
+To install a specific version of the package use
+```
+pip install utracto==0.0.8
+```
+All available versions are listed in [PyPI](https://pypi.org/project/utracto/). The package names follow the rules of [semantic versioning](https://semver.org/).
+
 ### Local install
 
 If you want to download the latest version directly from GitHub, you can clone this repository
 ```
 git clone https://github.com/DelinteNicolas/UTracto.git
 ```
+For a more frequent use of the library, you may wish to permanently add the package to your current Python environment. Navigate to the folder where this repository was cloned or downloaded (the folder containing the ```setup.py``` file) and install the package as follows
+```
+cd UTracto
+pip install .
+```
+
+If you have an existing install, and want to ensure package and dependencies are updated use --upgrade
+```
+pip install --upgrade .
+```
+### Importing
+At the top of your Python scripts, import the library as
+```
+import utracto
+```
+
+### Checking current version installed
+
+The version of the UNRAVEL package installed can be displayed by typing the following command in your python environment
+```
+utracto.__version__
+``` 
+
+### Uninstalling
+```
+pip uninstall utracto
+```
 
 ## Example data and code
 
 An example use of the main methods and outputs of UTracto is written in the `example.py` file.
```

### Comparing `utracto-0.0.8/setup.py` & `utracto-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     license='GNU General Public License v3.0',
     packages=['utracto'],
     install_requires=['dipy',
                       'nibabel',
                       'numpy',
                       'tqdm',
 			    'pilab-binama',
+			    'unravel-python',
                       ],
 
     classifiers=['Development Status :: 4 - Beta',
                  'Intended Audience :: Science/Research',
                  'Natural Language :: English',
                  'Programming Language :: Python'],
 )
```

### Comparing `utracto-0.0.8/utracto/core.py` & `utracto-0.0.9/utracto/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         Minimum value of wmfod[:,:,:,0] to be considered as white mater.
         The default is 0.1.
     interface : float, optional
         Value of wmfod[:,:,:,0] to be considered at the interface between grey
         and white mater. The default is 0.08.
     interface_thickness : int, optional
         Thickness of the grey/white matter interface. The default is 3.
-    wm_deep : TYPE, optional
+    wm_deep : float, optional
         Value above which we are in deep white matter. The default is 0.35.
     smooth_factor : float, optional
         Gaussian filter factor. The default is .85.
     float_type : bool, optional
         If True then output is in float. The default is False.
     only_WM : bool, optional
         If True, the angular map is only in areas of white matter.
```

### Comparing `utracto-0.0.8/utracto/tracking.py` & `utracto-0.0.9/utracto/tracking.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.8/utracto/utils.py` & `utracto-0.0.9/utracto/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import numpy as np
 from tqdm import tqdm
 from dipy.data import get_sphere
 from dipy.reconst.shm import sh_to_sf, sf_to_sh
 from dipy.io.streamline import load_tractogram, save_tractogram
-from TIME.core import angle_difference
+from unravel.core import angle_difference
 
 
 def _flip_m_neg(sh, sh_order: int, full_basis: bool = False):
     '''
 
 
     Parameters
@@ -172,15 +172,15 @@
         point = streams_data[p]
         previous_point = streams_data[p-1]
         next_point = streams_data[p+1]
 
         v1 = (point-previous_point)
         v2 = (next_point-point)
 
-        ang = angle_difference(v1, v2)
+        ang = angle_difference(v1, v2, direction=True)
 
         if ang > max_angle:
 
             stream_num = _find_low_nearest(streams._offsets, p+1)
 
             streams._offsets = np.insert(streams._offsets, stream_num+1, p+1)
```

