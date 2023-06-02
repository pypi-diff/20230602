# Comparing `tmp/portchoice-0.3.1.tar.gz` & `tmp/portchoice-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portchoice-0.3.1.tar", max compression
+gzip compressed data, was "portchoice-0.3.2.tar", max compression
```

## Comparing `portchoice-0.3.1.tar` & `portchoice-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2022-10-29 12:06:25.965071 portchoice-0.3.1/portchoice/__init__.py
--rw-r--r--   0        0        0    14724 2023-02-05 19:42:38.209912 portchoice-0.3.1/portchoice/design.py
--rw-r--r--   0        0        0     4735 2023-02-05 19:51:22.664145 portchoice-0.3.1/portchoice/generate.py
--rw-r--r--   0        0        0    44471 2023-02-05 19:53:22.054235 portchoice-0.3.1/portchoice/models.py
--rw-r--r--   0        0        0     6537 2023-02-05 19:46:18.840897 portchoice-0.3.1/portchoice/utils.py
--rw-r--r--   0        0        0      461 2023-02-05 19:54:01.377091 portchoice-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      715 2023-02-05 19:54:29.199859 portchoice-0.3.1/setup.py
--rw-r--r--   0        0        0      490 2023-02-05 19:54:29.200123 portchoice-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2022-10-29 12:06:25.965071 portchoice-0.3.2/portchoice/__init__.py
+-rw-r--r--   0        0        0    14724 2023-02-05 19:42:38.209912 portchoice-0.3.2/portchoice/design.py
+-rw-r--r--   0        0        0     4735 2023-02-05 19:51:22.664145 portchoice-0.3.2/portchoice/generate.py
+-rw-r--r--   0        0        0    44471 2023-02-05 19:53:22.054235 portchoice-0.3.2/portchoice/models.py
+-rw-r--r--   0        0        0     6537 2023-02-05 19:46:18.840897 portchoice-0.3.2/portchoice/utils.py
+-rw-r--r--   0        0        0      454 2023-06-02 08:49:34.765147 portchoice-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      709 2023-06-02 08:50:29.036122 portchoice-0.3.2/setup.py
+-rw-r--r--   0        0        0      535 2023-06-02 08:50:29.036407 portchoice-0.3.2/PKG-INFO
```

### Comparing `portchoice-0.3.1/portchoice/design.py` & `portchoice-0.3.2/portchoice/design.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.1/portchoice/generate.py` & `portchoice-0.3.2/portchoice/generate.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.1/portchoice/models.py` & `portchoice-0.3.2/portchoice/models.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.1/portchoice/utils.py` & `portchoice-0.3.2/portchoice/utils.py`

 * *Files identical despite different names*

### Comparing `portchoice-0.3.1/setup.py` & `portchoice-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 {'': ['*']}
 
 install_requires = \
 ['numdifftools>=0.9.40,<0.10.0', 'pandas>=1.4.2,<2.0.0', 'pyDOE2>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'portchoice',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Modules to design and estimate portfolio choice models',
     'long_description': None,
     'author': 'Jose Ignacio Hernandez',
     'author_email': 'j.i.hernandez@tudelft.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

