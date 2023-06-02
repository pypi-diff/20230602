# Comparing `tmp/pylibffm-0.1.0.tar.gz` & `tmp/pylibffm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibffm-0.1.0.tar", last modified: Thu Jun  1 12:20:58 2023, max compression
+gzip compressed data, was "pylibffm-0.2.1.tar", last modified: Fri Jun  2 12:47:44 2023, max compression
```

## Comparing `pylibffm-0.1.0.tar` & `pylibffm-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,59 @@
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-06-01 12:20:58.907648 pylibffm-0.1.0/
--rw-r--r--   0 julien    (1000) julien    (1000)     1064 2023-06-01 12:19:53.000000 pylibffm-0.1.0/LICENSE
--rw-r--r--   0 julien    (1000) julien    (1000)       75 2023-06-01 12:19:53.000000 pylibffm-0.1.0/MANIFEST.in
--rw-r--r--   0 julien    (1000) julien    (1000)      149 2023-06-01 12:20:58.907648 pylibffm-0.1.0/PKG-INFO
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-06-01 12:20:58.907648 pylibffm-0.1.0/pylibffm/
--rw-r--r--   0 julien    (1000) julien    (1000)       24 2023-06-01 12:19:53.000000 pylibffm-0.1.0/pylibffm/__init__.py
--rw-r--r--   0 julien    (1000) julien    (1000)     4761 2023-06-01 12:19:53.000000 pylibffm-0.1.0/pylibffm/pylibffm.py
-drwxr-xr-x   0 julien    (1000) julien    (1000)        0 2023-06-01 12:20:58.907648 pylibffm-0.1.0/pylibffm.egg-info/
--rw-r--r--   0 julien    (1000) julien    (1000)      149 2023-06-01 12:20:58.000000 pylibffm-0.1.0/pylibffm.egg-info/PKG-INFO
--rw-r--r--   0 julien    (1000) julien    (1000)      229 2023-06-01 12:20:58.000000 pylibffm-0.1.0/pylibffm.egg-info/SOURCES.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        1 2023-06-01 12:20:58.000000 pylibffm-0.1.0/pylibffm.egg-info/dependency_links.txt
--rw-r--r--   0 julien    (1000) julien    (1000)       12 2023-06-01 12:20:58.000000 pylibffm-0.1.0/pylibffm.egg-info/requires.txt
--rw-r--r--   0 julien    (1000) julien    (1000)        9 2023-06-01 12:20:58.000000 pylibffm-0.1.0/pylibffm.egg-info/top_level.txt
--rw-r--r--   0 julien    (1000) julien    (1000)       38 2023-06-01 12:20:58.907648 pylibffm-0.1.0/setup.cfg
--rw-r--r--   0 julien    (1000) julien    (1000)      941 2023-06-01 12:19:53.000000 pylibffm-0.1.0/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.2.1/LICENSE
+-rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.2.1/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:47:44.786581 pylibffm-0.2.1/PKG-INFO
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.782581 pylibffm-0.2.1/libffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       31 2023-06-01 12:37:52.000000 pylibffm-0.2.1/libffm/.git
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1478 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/COPYRIGHT
+-rw-rw-r--   0 julien    (1003) julien    (1003)      626 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/Makefile
+-rw-rw-r--   0 julien    (1003) julien    (1003)      697 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/Makefile.win
+-rw-rw-r--   0 julien    (1003) julien    (1003)     8692 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/README
+-rwxrwxr-x   0 julien    (1003) julien    (1003)    71240 2023-06-02 07:29:22.000000 pylibffm-0.2.1/libffm/ffm-predict
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2396 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/ffm-predict.cpp
+-rwxrwxr-x   0 julien    (1003) julien    (1003)    75448 2023-06-02 07:29:21.000000 pylibffm-0.2.1/libffm/ffm-train
+-rw-rw-r--   0 julien    (1003) julien    (1003)     5214 2023-06-02 07:25:19.000000 pylibffm-0.2.1/libffm/ffm-train.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)    19754 2023-06-02 07:04:48.000000 pylibffm-0.2.1/libffm/ffm.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1133 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/ffm.h
+-rw-rw-r--   0 julien    (1003) julien    (1003)      570 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/timer.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)      232 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/timer.h
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1975 2023-06-02 07:29:15.000000 pylibffm-0.2.1/libffm/tmp.ffm
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1360 2023-06-02 07:29:27.000000 pylibffm-0.2.1/libffm/tmp.ffm.bin
+-rw-rw-r--   0 julien    (1003) julien    (1003)      141 2023-06-02 07:29:27.000000 pylibffm-0.2.1/libffm/tmp.ffm.model
+-rw-rw-r--   0 julien    (1003) julien    (1003)      361 2023-06-01 12:37:51.000000 pylibffm-0.2.1/libffm-makefile
+-rw-rw-r--   0 julien    (1003) julien    (1003)      724 2023-06-01 12:37:51.000000 pylibffm-0.2.1/makefile
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pybind11/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1271 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.appveyor.yml
+-rw-rw-r--   0 julien    (1003) julien    (1003)      996 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.clang-format
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2605 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.clang-tidy
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2196 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1308 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.codespell-ignore-lines
+-rw-rw-r--   0 julien    (1003) julien    (1003)       33 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.git
+-rw-rw-r--   0 julien    (1003) julien    (1003)       18 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.gitattributes
+-rw-rw-r--   0 julien    (1003) julien    (1003)      502 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.gitignore
+-rw-rw-r--   0 julien    (1003) julien    (1003)     3600 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 julien    (1003) julien    (1003)       62 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.readthedocs.yml
+-rw-rw-r--   0 julien    (1003) julien    (1003)    12067 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/CMakeLists.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1684 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/LICENSE
+-rw-rw-r--   0 julien    (1003) julien    (1003)      247 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)     7686 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/README.rst
+-rw-rw-r--   0 julien    (1003) julien    (1003)      688 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/SECURITY.md
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2765 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/noxfile.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2360 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/pyproject.toml
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1452 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     4877 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pylibffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.2.1/pylibffm/__init__.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     5288 2023-06-02 07:22:36.000000 pylibffm-0.2.1/pylibffm/api.py
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 12:43:03.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 12:43:08.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 12:42:46.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 12:42:52.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 12:42:57.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pylibffm.egg-info/
+-rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1195 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-02 12:47:44.786581 pylibffm-0.2.1/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1006 2023-06-02 12:46:19.000000 pylibffm-0.2.1/setup.py
```

### Comparing `pylibffm-0.1.0/LICENSE` & `pylibffm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibffm-0.1.0/pylibffm/pylibffm.py` & `pylibffm-0.2.1/pylibffm/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
+
 import pathlib
+import uuid
 
-from . import wrapper
-import scipy.sparse as sparse
 import numpy as np
-import uuid
+import scipy.sparse as sparse
+
+from . import wrapper
 
 __all__ = ["Model", "train", "load"]
 
 
 class Model:
     """A model obtained from train or load. Can be saved and used to predict."""
 
@@ -97,14 +99,23 @@
         if valid_x is None or valid_y is None:
             raise ValueError("no validation set provided for auto-stop")
         if valid_y.ndim != 1 or fields.ndim != 1:
             raise ValueError("invalid input matrix shapes")
         if valid_x.shape[0] != valid_y.shape[0] or valid_x.shape[1] != fields.shape[0]:
             raise ValueError("input matrix shapes do not match")
 
+    # x is converted to float within the C++ wrapper because x is relatively large
+    # y and fields are converted to float here because they are small
+    # The C++ wrapper will give an error on wrong array types, so this won't cause hidden bugs
+    fields = fields.astype(np.int32, copy=False)
+    train_y = (train_y > 0).astype(np.float32, copy=False) * 2 - 1
+    if options["auto_stop"]:
+        valid_y = (valid_y > 0).astype(np.float32, copy=False) * 2 - 1
+
+    pathlib.Path(tmpdir).mkdir(parents=True, exist_ok=True)
     train_path = f"{tmpdir}/{uuid.uuid4().hex}"
     wrapper.arr2bin(
         train_x.shape[0],
         train_x.shape[1],
         train_y,
         fields,
         train_x.data,
```

### Comparing `pylibffm-0.1.0/setup.py` & `pylibffm-0.2.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import setuptools
-from distutils.command.install import install as DistutilsInstall
-import subprocess
 
 name = "pylibffm"
-version = "0.1.0"
+version = "0.2.1"
 author = "ntumlgroup"
 license = "MIT License"
 description = "A library wrapping libffm"
 
 packages = setuptools.find_packages()
 install_requires = ["scipy", "numpy"]
 
-
-class MakeThenInstall(DistutilsInstall):
-    def run(self):
-        subprocess.call("make", shell=True, executable="/bin/bash")
-        DistutilsInstall.run(self)
-
-
+# Extension modules are completely useless, because they are in effect a dumber and duplicate makefile.
+# As it stands, there are __zero__ ways of calling out to make during installation,
+# so the current solution is to distribute all binaries and pretend it's part of the source files.
 if __name__ == "__main__":
     setuptools.setup(
         name=name,
         version=version,
         author=author,
         license=license,
         # license_file=license_file,
         description=description,
         # long_description=long_description,
         # url=url,
         # project_urls=project_urls,
         # classifiers=classifiers,
         packages=packages,
+        package_data={
+            "pylibffm": ["wrapper*.so"],
+        },
         install_requires=install_requires,
-        cmdclass={"install": MakeThenInstall},
     )
```

