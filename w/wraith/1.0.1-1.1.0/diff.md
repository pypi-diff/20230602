# Comparing `tmp/wraith-1.0.1.tar.gz` & `tmp/wraith-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wraith-1.0.1.tar", last modified: Tue May 30 19:09:57 2023, max compression
+gzip compressed data, was "wraith-1.1.0.tar", last modified: Fri Jun  2 14:33:56 2023, max compression
```

## Comparing `wraith-1.0.1.tar` & `wraith-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 19:09:57.388242 wraith-1.0.1/
--rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 wraith-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1231 2023-05-30 19:09:57.372620 wraith-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1972 2023-05-30 18:40:49.000000 wraith-1.0.1/README.md
--rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 wraith-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 19:09:57.388242 wraith-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1339 2023-05-30 19:06:43.000000 wraith-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:09:57.372620 wraith-1.0.1/wraith.egg-info/
--rw-rw-rw-   0        0        0     1231 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-30 19:09:57.000000 wraith-1.0.1/wraith.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13657 2023-05-30 19:07:34.000000 wraith-1.0.1/wraith.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:33:56.634803 wraith-1.1.0/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 wraith-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1371 2023-06-02 14:33:56.633803 wraith-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2223 2023-06-02 14:31:23.000000 wraith-1.1.0/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 wraith-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 14:33:56.635802 wraith-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1464 2023-06-02 14:32:54.000000 wraith-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 14:33:56.629807 wraith-1.1.0/wraith.egg-info/
+-rw-rw-rw-   0        0        0     1371 2023-06-02 14:33:56.000000 wraith-1.1.0/wraith.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-06-02 14:33:56.000000 wraith-1.1.0/wraith.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 14:33:56.000000 wraith-1.1.0/wraith.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 14:33:56.000000 wraith-1.1.0/wraith.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 14:33:56.000000 wraith-1.1.0/wraith.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13767 2023-06-02 14:28:14.000000 wraith-1.1.0/wraith.py
```

### Comparing `wraith-1.0.1/LICENSE` & `wraith-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wraith-1.0.1/README.md` & `wraith-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,20 @@
 
 ### `choose(*values)`
 
 The `choose()` function returns a randomly chosen item from the specified list which can have as many items. For example, `choose("apple", "banana", "pear")` will return either "apple", "banana", or "pear".
 
 ## Support
 
-If you have any suggestions or ideas, please share them with me through e-mail. If you have any critics, be sure to e-mail as well. Also, please report any bugs you find - that way you help the rest of the community. Thank you for using Wraith!
+If you have any suggestions or ideas, please share them with me through e-mail. If you have any critics, be sure to e-mail as well. Also, please report any bugs you find - that way you help the rest of the community. Thank you for using Wraith!
+
+## Changelogs
+
+Welcome to 'The POSIX Update'!
+
+### New
+
+- added the new `clear()` function, which is the POSIX version of the `cls()` function
+
+### Changes
+
+- no longer needs Python 3.10 to run: for better Bash compatibility it's now 3.8
```

### Comparing `wraith-1.0.1/setup.py` & `wraith-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from setuptools import setup
 
 setup(
   name = "wraith",
-  version = "1.0.1",
+  version = "1.1.0",
   description = "All the power of Python...in the palm of your hand.",
   long_description = "Wraith is a module programmed by Omer Drkić that adds loads of new features and makes Python easier to use. The module adds some features that the developer felt like they were missing from Python. It also adds some extension to the 'math' library and to the actual Python environment, as well as some useful data manipulation tools.",
   author = "Omer Drkić",
   author_email = "omerdrkic2501@gmail.com",
   py_modules = [
     "wraith"
   ],
@@ -14,20 +14,23 @@
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Jupyter",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Boost Software License 1.0 (BSL-1.0)",
     "Natural Language :: English",
     "Operating System :: Microsoft",
+    "Operating System :: POSIX",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Interpreters",
     "Topic :: Software Development :: Libraries",
     "Typing :: Typed"
   ],
   license = "Boost Software License 1.0",
   install_requires = [
     "keyboard"
   ],
-  python_requires = ">=3.10"
+  python_requires = ">=3.8"
 )
```

### Comparing `wraith-1.0.1/wraith.py` & `wraith-1.1.0/wraith.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,23 @@
 
 def chooseindex(index: int, *values):
   """
   Returns an item from the specified list using a zero-based index.
   """
   return values[index]
 
+def clear():
+  """
+  Clears the previous console output on POSIX.
+  """
+  o.system("clear")
+
 def cls():
   """
-  Clears the previous console output.
+  Clears the previous console output on Windows.
   """
   o.system("cls")
 
 def find(string: str, character: str):
   """
   Returns the number of times a character is repeated in the specified string.
   """
```

