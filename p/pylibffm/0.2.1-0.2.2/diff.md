# Comparing `tmp/pylibffm-0.2.1.tar.gz` & `tmp/pylibffm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibffm-0.2.1.tar", last modified: Fri Jun  2 12:47:44 2023, max compression
+gzip compressed data, was "pylibffm-0.2.2.tar", last modified: Fri Jun  2 12:52:25 2023, max compression
```

## Comparing `pylibffm-0.2.1.tar` & `pylibffm-0.2.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.2.1/LICENSE
--rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.2.1/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:47:44.786581 pylibffm-0.2.1/PKG-INFO
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.782581 pylibffm-0.2.1/libffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       31 2023-06-01 12:37:52.000000 pylibffm-0.2.1/libffm/.git
--rw-rw-r--   0 julien    (1003) julien    (1003)     1478 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/COPYRIGHT
--rw-rw-r--   0 julien    (1003) julien    (1003)      626 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/Makefile
--rw-rw-r--   0 julien    (1003) julien    (1003)      697 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/Makefile.win
--rw-rw-r--   0 julien    (1003) julien    (1003)     8692 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/README
--rwxrwxr-x   0 julien    (1003) julien    (1003)    71240 2023-06-02 07:29:22.000000 pylibffm-0.2.1/libffm/ffm-predict
--rw-rw-r--   0 julien    (1003) julien    (1003)     2396 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/ffm-predict.cpp
--rwxrwxr-x   0 julien    (1003) julien    (1003)    75448 2023-06-02 07:29:21.000000 pylibffm-0.2.1/libffm/ffm-train
--rw-rw-r--   0 julien    (1003) julien    (1003)     5214 2023-06-02 07:25:19.000000 pylibffm-0.2.1/libffm/ffm-train.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)    19754 2023-06-02 07:04:48.000000 pylibffm-0.2.1/libffm/ffm.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)     1133 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/ffm.h
--rw-rw-r--   0 julien    (1003) julien    (1003)      570 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/timer.cpp
--rw-rw-r--   0 julien    (1003) julien    (1003)      232 2023-06-01 12:37:54.000000 pylibffm-0.2.1/libffm/timer.h
--rw-rw-r--   0 julien    (1003) julien    (1003)     1975 2023-06-02 07:29:15.000000 pylibffm-0.2.1/libffm/tmp.ffm
--rw-rw-r--   0 julien    (1003) julien    (1003)     1360 2023-06-02 07:29:27.000000 pylibffm-0.2.1/libffm/tmp.ffm.bin
--rw-rw-r--   0 julien    (1003) julien    (1003)      141 2023-06-02 07:29:27.000000 pylibffm-0.2.1/libffm/tmp.ffm.model
--rw-rw-r--   0 julien    (1003) julien    (1003)      361 2023-06-01 12:37:51.000000 pylibffm-0.2.1/libffm-makefile
--rw-rw-r--   0 julien    (1003) julien    (1003)      724 2023-06-01 12:37:51.000000 pylibffm-0.2.1/makefile
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pybind11/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1271 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.appveyor.yml
--rw-rw-r--   0 julien    (1003) julien    (1003)      996 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.clang-format
--rw-rw-r--   0 julien    (1003) julien    (1003)     2605 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.clang-tidy
--rw-rw-r--   0 julien    (1003) julien    (1003)     2196 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.cmake-format.yaml
--rw-rw-r--   0 julien    (1003) julien    (1003)     1308 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.codespell-ignore-lines
--rw-rw-r--   0 julien    (1003) julien    (1003)       33 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.git
--rw-rw-r--   0 julien    (1003) julien    (1003)       18 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.gitattributes
--rw-rw-r--   0 julien    (1003) julien    (1003)      502 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.gitignore
--rw-rw-r--   0 julien    (1003) julien    (1003)     3600 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.pre-commit-config.yaml
--rw-rw-r--   0 julien    (1003) julien    (1003)       62 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/.readthedocs.yml
--rw-rw-r--   0 julien    (1003) julien    (1003)    12067 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/CMakeLists.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)     1684 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/LICENSE
--rw-rw-r--   0 julien    (1003) julien    (1003)      247 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)     7686 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/README.rst
--rw-rw-r--   0 julien    (1003) julien    (1003)      688 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/SECURITY.md
--rw-rw-r--   0 julien    (1003) julien    (1003)     2765 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/noxfile.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     2360 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/pyproject.toml
--rw-rw-r--   0 julien    (1003) julien    (1003)     1452 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     4877 2023-06-01 12:37:54.000000 pylibffm-0.2.1/pybind11/setup.py
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pylibffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.2.1/pylibffm/__init__.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     5288 2023-06-02 07:22:36.000000 pylibffm-0.2.1/pylibffm/api.py
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 12:43:03.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 12:43:08.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 12:42:46.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 12:42:52.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 12:42:57.000000 pylibffm-0.2.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:47:44.786581 pylibffm-0.2.1/pylibffm.egg-info/
--rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)     1195 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/requires.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-02 12:47:44.000000 pylibffm-0.2.1/pylibffm.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-02 12:47:44.786581 pylibffm-0.2.1/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     1006 2023-06-02 12:46:19.000000 pylibffm-0.2.1/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:52:25.637311 pylibffm-0.2.2/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1064 2023-06-01 12:37:51.000000 pylibffm-0.2.2/LICENSE
+-rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.2.2/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:52:25.637311 pylibffm-0.2.2/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      815 2023-06-02 12:35:18.000000 pylibffm-0.2.2/README.md
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:52:25.637311 pylibffm-0.2.2/libffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       31 2023-06-01 12:37:52.000000 pylibffm-0.2.2/libffm/.git
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1478 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/COPYRIGHT
+-rw-rw-r--   0 julien    (1003) julien    (1003)      626 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/Makefile
+-rw-rw-r--   0 julien    (1003) julien    (1003)      697 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/Makefile.win
+-rw-rw-r--   0 julien    (1003) julien    (1003)     8692 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/README
+-rwxrwxr-x   0 julien    (1003) julien    (1003)    71240 2023-06-02 07:29:22.000000 pylibffm-0.2.2/libffm/ffm-predict
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2396 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/ffm-predict.cpp
+-rwxrwxr-x   0 julien    (1003) julien    (1003)    75448 2023-06-02 07:29:21.000000 pylibffm-0.2.2/libffm/ffm-train
+-rw-rw-r--   0 julien    (1003) julien    (1003)     5214 2023-06-02 07:25:19.000000 pylibffm-0.2.2/libffm/ffm-train.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)    19754 2023-06-02 07:04:48.000000 pylibffm-0.2.2/libffm/ffm.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1133 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/ffm.h
+-rw-rw-r--   0 julien    (1003) julien    (1003)      570 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/timer.cpp
+-rw-rw-r--   0 julien    (1003) julien    (1003)      232 2023-06-01 12:37:54.000000 pylibffm-0.2.2/libffm/timer.h
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1975 2023-06-02 07:29:15.000000 pylibffm-0.2.2/libffm/tmp.ffm
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1360 2023-06-02 07:29:27.000000 pylibffm-0.2.2/libffm/tmp.ffm.bin
+-rw-rw-r--   0 julien    (1003) julien    (1003)      141 2023-06-02 07:29:27.000000 pylibffm-0.2.2/libffm/tmp.ffm.model
+-rw-rw-r--   0 julien    (1003) julien    (1003)      361 2023-06-01 12:37:51.000000 pylibffm-0.2.2/libffm-makefile
+-rw-rw-r--   0 julien    (1003) julien    (1003)      724 2023-06-01 12:37:51.000000 pylibffm-0.2.2/makefile
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:52:25.637311 pylibffm-0.2.2/pybind11/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1271 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.appveyor.yml
+-rw-rw-r--   0 julien    (1003) julien    (1003)      996 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.clang-format
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2605 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.clang-tidy
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2196 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.cmake-format.yaml
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1308 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.codespell-ignore-lines
+-rw-rw-r--   0 julien    (1003) julien    (1003)       33 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.git
+-rw-rw-r--   0 julien    (1003) julien    (1003)       18 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.gitattributes
+-rw-rw-r--   0 julien    (1003) julien    (1003)      502 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.gitignore
+-rw-rw-r--   0 julien    (1003) julien    (1003)     3600 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.pre-commit-config.yaml
+-rw-rw-r--   0 julien    (1003) julien    (1003)       62 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/.readthedocs.yml
+-rw-rw-r--   0 julien    (1003) julien    (1003)    12067 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/CMakeLists.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1684 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/LICENSE
+-rw-rw-r--   0 julien    (1003) julien    (1003)      247 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)     7686 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/README.rst
+-rw-rw-r--   0 julien    (1003) julien    (1003)      688 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/SECURITY.md
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2765 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/noxfile.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     2360 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/pyproject.toml
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1452 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     4877 2023-06-01 12:37:54.000000 pylibffm-0.2.2/pybind11/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:52:25.637311 pylibffm-0.2.2/pylibffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.2.2/pylibffm/__init__.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     5288 2023-06-02 07:22:36.000000 pylibffm-0.2.2/pylibffm/api.py
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 12:43:03.000000 pylibffm-0.2.2/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 12:43:08.000000 pylibffm-0.2.2/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 12:42:46.000000 pylibffm-0.2.2/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 12:42:52.000000 pylibffm-0.2.2/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 12:42:57.000000 pylibffm-0.2.2/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-02 12:52:25.637311 pylibffm-0.2.2/pylibffm.egg-info/
+-rw-rw-r--   0 julien    (1003) julien    (1003)      149 2023-06-02 12:52:25.000000 pylibffm-0.2.2/pylibffm.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1205 2023-06-02 12:52:25.000000 pylibffm-0.2.2/pylibffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-02 12:52:25.000000 pylibffm-0.2.2/pylibffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-02 12:52:25.000000 pylibffm-0.2.2/pylibffm.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-02 12:52:25.000000 pylibffm-0.2.2/pylibffm.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-02 12:52:25.637311 pylibffm-0.2.2/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1006 2023-06-02 12:51:46.000000 pylibffm-0.2.2/setup.py
```

### Comparing `pylibffm-0.2.1/LICENSE` & `pylibffm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/COPYRIGHT` & `pylibffm-0.2.2/libffm/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/Makefile` & `pylibffm-0.2.2/libffm/Makefile`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/Makefile.win` & `pylibffm-0.2.2/libffm/Makefile.win`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/README` & `pylibffm-0.2.2/libffm/README`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm-predict` & `pylibffm-0.2.2/libffm/ffm-predict`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm-predict.cpp` & `pylibffm-0.2.2/libffm/ffm-predict.cpp`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm-train` & `pylibffm-0.2.2/libffm/ffm-train`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm-train.cpp` & `pylibffm-0.2.2/libffm/ffm-train.cpp`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm.cpp` & `pylibffm-0.2.2/libffm/ffm.cpp`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/ffm.h` & `pylibffm-0.2.2/libffm/ffm.h`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/timer.cpp` & `pylibffm-0.2.2/libffm/timer.cpp`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/tmp.ffm` & `pylibffm-0.2.2/libffm/tmp.ffm`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/libffm/tmp.ffm.bin` & `pylibffm-0.2.2/libffm/tmp.ffm.bin`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/makefile` & `pylibffm-0.2.2/makefile`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.appveyor.yml` & `pylibffm-0.2.2/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.clang-format` & `pylibffm-0.2.2/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.clang-tidy` & `pylibffm-0.2.2/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.cmake-format.yaml` & `pylibffm-0.2.2/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.codespell-ignore-lines` & `pylibffm-0.2.2/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/.pre-commit-config.yaml` & `pylibffm-0.2.2/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/CMakeLists.txt` & `pylibffm-0.2.2/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/LICENSE` & `pylibffm-0.2.2/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/README.rst` & `pylibffm-0.2.2/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/SECURITY.md` & `pylibffm-0.2.2/pybind11/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/noxfile.py` & `pylibffm-0.2.2/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/pyproject.toml` & `pylibffm-0.2.2/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/setup.cfg` & `pylibffm-0.2.2/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pybind11/setup.py` & `pylibffm-0.2.2/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/api.py` & `pylibffm-0.2.2/pylibffm/api.py`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so` & `pylibffm-0.2.2/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so` & `pylibffm-0.2.2/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so` & `pylibffm-0.2.2/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so` & `pylibffm-0.2.2/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so` & `pylibffm-0.2.2/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.2.1/pylibffm.egg-info/SOURCES.txt` & `pylibffm-0.2.2/pylibffm.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+README.md
 libffm-makefile
 makefile
 setup.py
 libffm/.git
 libffm/COPYRIGHT
 libffm/Makefile
 libffm/Makefile.win
```

### Comparing `pylibffm-0.2.1/setup.py` & `pylibffm-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 name = "pylibffm"
-version = "0.2.1"
+version = "0.2.2"
 author = "ntumlgroup"
 license = "MIT License"
 description = "A library wrapping libffm"
 
 packages = setuptools.find_packages()
 install_requires = ["scipy", "numpy"]
```

