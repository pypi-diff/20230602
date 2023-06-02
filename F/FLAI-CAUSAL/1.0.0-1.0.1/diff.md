# Comparing `tmp/FLAI_CAUSAL-1.0.0.tar.gz` & `tmp/FLAI_CAUSAL-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.0.tar", last modified: Fri Jun  2 19:32:36 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.0.1.tar", last modified: Fri Jun  2 19:41:57 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.0.tar` & `FLAI_CAUSAL-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:32:36.631971 FLAI_CAUSAL-1.0.0/
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:32:36.631971 FLAI_CAUSAL-1.0.0/FLAI/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/FLAI/__init__.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9020 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/FLAI/causal_graph.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/FLAI/data.py
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:32:36.631971 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      549 2023-06-02 19:32:36.000000 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-02 19:32:36.000000 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-02 19:32:36.000000 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       70 2023-06-02 19:32:36.000000 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-02 19:32:36.000000 FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/LICENSE
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      549 2023-06-02 19:32:36.631971 FLAI_CAUSAL-1.0.0/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      238 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/README.md
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-02 19:32:36.631971 FLAI_CAUSAL-1.0.0/setup.cfg
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1396 2023-06-02 19:32:07.000000 FLAI_CAUSAL-1.0.0/setup.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:41:57.513702 FLAI_CAUSAL-1.0.1/
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:41:57.513702 FLAI_CAUSAL-1.0.1/FLAI/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/FLAI/__init__.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9020 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/FLAI/causal_graph.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/FLAI/data.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 19:41:57.513702 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 19:41:57.000000 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-02 19:41:57.000000 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-02 19:41:57.000000 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       65 2023-06-02 19:41:57.000000 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-02 19:41:57.000000 FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/LICENSE
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 19:41:57.513702 FLAI_CAUSAL-1.0.1/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      238 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/README.md
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-02 19:41:57.513702 FLAI_CAUSAL-1.0.1/setup.cfg
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1394 2023-06-02 19:41:22.000000 FLAI_CAUSAL-1.0.1/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.0/FLAI/causal_graph.py` & `FLAI_CAUSAL-1.0.1/FLAI/causal_graph.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.0/FLAI/data.py` & `FLAI_CAUSAL-1.0.1/FLAI/data.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.0/FLAI_CAUSAL.egg-info/PKG-INFO` & `FLAI_CAUSAL-1.0.1/FLAI_CAUSAL.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FLAI-CAUSAL
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to creat causal model and mitigate the bias.
-Home-page: https://github.com/rugonzs
+Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAI
```

### Comparing `FLAI_CAUSAL-1.0.0/LICENSE` & `FLAI_CAUSAL-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.0/PKG-INFO` & `FLAI_CAUSAL-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: FLAI_CAUSAL
-Version: 1.0.0
+Version: 1.0.1
 Summary: Library to creat causal model and mitigate the bias.
-Home-page: https://github.com/rugonzs
+Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FLAI
```

### Comparing `FLAI_CAUSAL-1.0.0/setup.py` & `FLAI_CAUSAL-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.0.1' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
-URL = 'https://github.com/rugonzs' #Modificar con vuestros datos
+URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-      'bnlearn','networkx','matplotlib','pgmpy','numpy', 'itertools','math','pandas','sklearn'
+      'bnlearn','networkx','matplotlib','pgmpy','numpy', 'itertools','pandas','sklearn'
       ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

