# Comparing `tmp/easycheck-0.9.1.tar.gz` & `tmp/easycheck-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck-0.9.1.tar", last modified: Fri Jun  2 10:56:26 2023, max compression
+gzip compressed data, was "easycheck-0.9.2.tar", last modified: Fri Jun  2 11:05:59 2023, max compression
```

## Comparing `easycheck-0.9.1.tar` & `easycheck-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.026688 easycheck-0.9.1/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2021-01-27 07:58:06.000000 easycheck-0.9.1/LICENSE
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24060 2023-06-02 10:56:26.025693 easycheck-0.9.1/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    20352 2023-06-02 10:56:23.000000 easycheck-0.9.1/README.rst
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.000683 easycheck-0.9.1/easycheck/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      614 2023-06-02 10:17:55.000000 easycheck-0.9.1/easycheck/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    38722 2023-06-02 10:38:03.000000 easycheck-0.9.1/easycheck/easycheck.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      865 2023-03-01 16:15:06.000000 easycheck-0.9.1/easycheck/tmp.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 10:56:26.021731 easycheck-0.9.1/easycheck.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24060 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      253 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-06-02 10:56:25.000000 easycheck-0.9.1/easycheck.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-02 10:56:26.026688 easycheck-0.9.1/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1134 2023-06-02 10:56:23.000000 easycheck-0.9.1/setup.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 11:05:59.099382 easycheck-0.9.2/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2021-01-27 07:58:06.000000 easycheck-0.9.2/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24042 2023-06-02 11:05:59.097379 easycheck-0.9.2/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    20334 2023-06-02 11:04:22.000000 easycheck-0.9.2/README.rst
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 11:05:59.056233 easycheck-0.9.2/easycheck/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      614 2023-06-02 10:17:55.000000 easycheck-0.9.2/easycheck/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    38722 2023-06-02 10:38:03.000000 easycheck-0.9.2/easycheck/easycheck.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      865 2023-03-01 16:15:06.000000 easycheck-0.9.2/easycheck/tmp.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-06-02 11:05:59.092319 easycheck-0.9.2/easycheck.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    24042 2023-06-02 11:05:58.000000 easycheck-0.9.2/easycheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      253 2023-06-02 11:05:58.000000 easycheck-0.9.2/easycheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-06-02 11:05:58.000000 easycheck-0.9.2/easycheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-06-02 11:05:58.000000 easycheck-0.9.2/easycheck.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-06-02 11:05:58.000000 easycheck-0.9.2/easycheck.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-06-02 11:05:59.100374 easycheck-0.9.2/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1134 2023-06-02 11:05:55.000000 easycheck-0.9.2/setup.py
```

### Comparing `easycheck-0.9.1/LICENSE` & `easycheck-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easycheck-0.9.1/PKG-INFO` & `easycheck-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: easycheck
-Version: 0.9.1
+Version: 0.9.2
 Summary: A tool for checking conditions in Python
 Home-page: https://github.com/nyggus/easycheck
 Author: Nyggus, Ke Boan & Darsoo
 Author-email: nyggus@gmail.com
 License: MIT
 Description: easycheck
         =========
-        .. image:: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml/badge.svg
-           :target: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml
+        .. image:: https://github.com/nyggus/easycheck/actions/workflows/check.yml/badge.svg
+           :target: https://github.com/nyggus/easycheck/actions/workflows/check.yml
         .. image:: https://codecov.io/github/nyggus/easycheck/branch/master/graph/badge.svg?token=EH4TLHQQWC 
            :target: https://codecov.io/github/nyggus/easycheck
         .. image:: https://img.shields.io/pypi/l/easycheck.svg
            :target: https://pypi.org/project/easycheck     
         .. image:: https://img.shields.io/pypi/v/easycheck.svg
            :target: https://pypi.org/project/easycheck     
         .. image:: https://img.shields.io/pypi/wheel/easycheck
```

### Comparing `easycheck-0.9.1/README.rst` & `easycheck-0.9.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 easycheck
 =========
-.. image:: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml/badge.svg
-   :target: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml
+.. image:: https://github.com/nyggus/easycheck/actions/workflows/check.yml/badge.svg
+   :target: https://github.com/nyggus/easycheck/actions/workflows/check.yml
 .. image:: https://codecov.io/github/nyggus/easycheck/branch/master/graph/badge.svg?token=EH4TLHQQWC 
    :target: https://codecov.io/github/nyggus/easycheck
 .. image:: https://img.shields.io/pypi/l/easycheck.svg
    :target: https://pypi.org/project/easycheck     
 .. image:: https://img.shields.io/pypi/v/easycheck.svg
    :target: https://pypi.org/project/easycheck     
 .. image:: https://img.shields.io/pypi/wheel/easycheck
```

### Comparing `easycheck-0.9.1/easycheck/__init__.py` & `easycheck-0.9.2/easycheck/__init__.py`

 * *Files identical despite different names*

### Comparing `easycheck-0.9.1/easycheck/easycheck.py` & `easycheck-0.9.2/easycheck/easycheck.py`

 * *Files identical despite different names*

### Comparing `easycheck-0.9.1/easycheck/tmp.py` & `easycheck-0.9.2/easycheck/tmp.py`

 * *Files identical despite different names*

### Comparing `easycheck-0.9.1/easycheck.egg-info/PKG-INFO` & `easycheck-0.9.2/easycheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: easycheck
-Version: 0.9.1
+Version: 0.9.2
 Summary: A tool for checking conditions in Python
 Home-page: https://github.com/nyggus/easycheck
 Author: Nyggus, Ke Boan & Darsoo
 Author-email: nyggus@gmail.com
 License: MIT
 Description: easycheck
         =========
-        .. image:: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml/badge.svg
-           :target: https://github.com/nyggus/easycheck/actions/workflows/python-package.yml
+        .. image:: https://github.com/nyggus/easycheck/actions/workflows/check.yml/badge.svg
+           :target: https://github.com/nyggus/easycheck/actions/workflows/check.yml
         .. image:: https://codecov.io/github/nyggus/easycheck/branch/master/graph/badge.svg?token=EH4TLHQQWC 
            :target: https://codecov.io/github/nyggus/easycheck
         .. image:: https://img.shields.io/pypi/l/easycheck.svg
            :target: https://pypi.org/project/easycheck     
         .. image:: https://img.shields.io/pypi/v/easycheck.svg
            :target: https://pypi.org/project/easycheck     
         .. image:: https://img.shields.io/pypi/wheel/easycheck
```

### Comparing `easycheck-0.9.1/setup.py` & `easycheck-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 extras_requirements = {
     "dev": ["pytest", "wheel", "black"],
 }
 
 setuptools.setup(
     name="easycheck",
-    version="0.9.1",
+    version="0.9.2",
     author="Nyggus, Ke Boan & Darsoo",
     author_email="nyggus@gmail.com",
     license="MIT",
     description="A tool for checking conditions in Python",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/nyggus/easycheck",
```

