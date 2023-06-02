# Comparing `tmp/SRIrepo-0.2.tar.gz` & `tmp/SRIrepo-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SRIrepo-0.2.tar", last modified: Fri Jun  2 06:40:08 2023, max compression
+gzip compressed data, was "dist\SRIrepo-0.3.tar", last modified: Fri Jun  2 07:07:58 2023, max compression
```

## Comparing `SRIrepo-0.2.tar` & `SRIrepo-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/
--rw-rw-rw-   0        0        0      428 2023-06-02 06:40:08.000000 SRIrepo-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo/
--rw-rw-rw-   0        0        0     1765 2023-06-02 06:35:23.000000 SRIrepo-0.2/SRIrepo/SRIrepo.py
--rw-rw-rw-   0        0        0       41 2023-06-01 07:15:45.000000 SRIrepo-0.2/SRIrepo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/
--rw-rw-rw-   0        0        0      428 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 06:40:08.000000 SRIrepo-0.2/SRIrepo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 06:40:08.000000 SRIrepo-0.2/setup.cfg
--rw-rw-rw-   0        0        0      526 2023-06-02 06:40:04.000000 SRIrepo-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:07:58.000000 SRIrepo-0.3/
+-rw-rw-rw-   0        0        0      428 2023-06-02 07:07:58.000000 SRIrepo-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo/
+-rw-rw-rw-   0        0        0     1710 2023-06-02 07:04:27.000000 SRIrepo-0.3/SRIrepo/SRIrepo.py
+-rw-rw-rw-   0        0        0       41 2023-06-01 07:15:45.000000 SRIrepo-0.3/SRIrepo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/
+-rw-rw-rw-   0        0        0      428 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 07:07:58.000000 SRIrepo-0.3/SRIrepo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:07:58.000000 SRIrepo-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      515 2023-06-02 07:04:36.000000 SRIrepo-0.3/setup.py
```

### Comparing `SRIrepo-0.2/SRIrepo/SRIrepo.py` & `SRIrepo-0.3/SRIrepo/SRIrepo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-
 import pandas as pd
-import warnings 
-warnings.filterwarnings("ignore")
 
 data = pd.read_excel(r'Pharma_entity_list.xlsx')
 
 def get_pharma_entities(text):
     global Company_list
     global output
     Company_List = []
```

### Comparing `SRIrepo-0.2/setup.py` & `SRIrepo-0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import codecs
 import os
 
 setup(
   name = 'SRIrepo',
   packages = ['SRIrepo'],
-  version = '0.2',
+  version = '0.3',
   description = 'Finds Pharma drug names in a string',
   long_description='This library will tokenize your unstructured text and find the pharma entities in the text. Code: import SRIrepo as SRI   SRI. get_pharma_entities("Abbvie and Merck are two companies and one of them produces a drug called Humira")',
   author = 'Marcel Tino',
   keywords = ['drug'],
-  install_requires=['pandas','warnings']
+  install_requires=['pandas']
 )
```

