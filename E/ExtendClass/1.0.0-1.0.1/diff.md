# Comparing `tmp/ExtendClass-1.0.0.tar.gz` & `tmp/ExtendClass-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExtendClass-1.0.0.tar", last modified: Fri Jun  2 14:10:59 2023, max compression
+gzip compressed data, was "ExtendClass-1.0.1.tar", last modified: Fri Jun  2 14:21:45 2023, max compression
```

## Comparing `ExtendClass-1.0.0.tar` & `ExtendClass-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:10:59.973126 ExtendClass-1.0.0/
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:10:59.973126 ExtendClass-1.0.0/ExtendClass/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1665 2023-06-02 14:02:32.000000 ExtendClass-1.0.0/ExtendClass/Extension.py
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:07:51.000000 ExtendClass-1.0.0/ExtendClass/__init__.py
-drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:10:59.973126 ExtendClass-1.0.0/ExtendClass.egg-info/
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-02 14:10:59.000000 ExtendClass-1.0.0/ExtendClass.egg-info/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      215 2023-06-02 14:10:59.000000 ExtendClass-1.0.0/ExtendClass.egg-info/SOURCES.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-02 14:10:59.000000 ExtendClass-1.0.0/ExtendClass.egg-info/dependency_links.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       12 2023-06-02 14:10:59.000000 ExtendClass-1.0.0/ExtendClass.egg-info/top_level.txt
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2023-06-02 14:05:22.000000 ExtendClass-1.0.0/LICENSE
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-02 14:10:59.973126 ExtendClass-1.0.0/PKG-INFO
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      121 2023-06-02 14:05:22.000000 ExtendClass-1.0.0/README.md
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-02 14:10:59.973126 ExtendClass-1.0.0/setup.cfg
--rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      977 2023-06-02 14:10:45.000000 ExtendClass-1.0.0/setup.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:21:45.565569 ExtendClass-1.0.1/
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:21:45.561569 ExtendClass-1.0.1/ExtendClass/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)     1665 2023-06-02 14:02:32.000000 ExtendClass-1.0.1/ExtendClass/Extension.py
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       28 2023-06-02 14:21:06.000000 ExtendClass-1.0.1/ExtendClass/__init__.py
+drwxrwxr-x   0 rodrigo   (1000) rodrigo   (1000)        0 2023-06-02 14:21:45.565569 ExtendClass-1.0.1/ExtendClass.egg-info/
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-02 14:21:45.000000 ExtendClass-1.0.1/ExtendClass.egg-info/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      215 2023-06-02 14:21:45.000000 ExtendClass-1.0.1/ExtendClass.egg-info/SOURCES.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)        1 2023-06-02 14:21:45.000000 ExtendClass-1.0.1/ExtendClass.egg-info/dependency_links.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       12 2023-06-02 14:21:45.000000 ExtendClass-1.0.1/ExtendClass.egg-info/top_level.txt
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)    35149 2023-06-02 14:05:22.000000 ExtendClass-1.0.1/LICENSE
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      727 2023-06-02 14:21:45.565569 ExtendClass-1.0.1/PKG-INFO
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      121 2023-06-02 14:05:22.000000 ExtendClass-1.0.1/README.md
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)       38 2023-06-02 14:21:45.565569 ExtendClass-1.0.1/setup.cfg
+-rw-rw-r--   0 rodrigo   (1000) rodrigo   (1000)      977 2023-06-02 14:21:35.000000 ExtendClass-1.0.1/setup.py
```

### Comparing `ExtendClass-1.0.0/ExtendClass/Extension.py` & `ExtendClass-1.0.1/ExtendClass/Extension.py`

 * *Files identical despite different names*

### Comparing `ExtendClass-1.0.0/ExtendClass.egg-info/PKG-INFO` & `ExtendClass-1.0.1/ExtendClass.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExtendClass
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python lib to extend classes
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,extend,class,extend class,extendclass,extend-class,extend_class,extendclass
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ExtendClass-1.0.0/LICENSE` & `ExtendClass-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ExtendClass-1.0.0/PKG-INFO` & `ExtendClass-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ExtendClass
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python lib to extend classes
 Author: Rodrigo Santos de Carvalho
 Author-email: <rodrigosc2401@gmail.com>
 Keywords: python,extend,class,extend class,extendclass,extend-class,extend_class,extendclass
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ExtendClass-1.0.0/setup.py` & `ExtendClass-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'A python lib to extend classes'
 LONG_DESCRIPTION = 'A python lib to extend classes. Inject methods in a class without inheritance. It access protected methods and attributes.'
 
 # Setting up
 setup(
     name="ExtendClass",
     version=VERSION,
```

