# Comparing `tmp/FLAI_CAUSAL-1.0.5.tar.gz` & `tmp/FLAI_CAUSAL-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAI_CAUSAL-1.0.5.tar", last modified: Fri Jun  2 20:14:38 2023, max compression
+gzip compressed data, was "FLAI_CAUSAL-1.0.6.tar", last modified: Fri Jun  2 20:18:52 2023, max compression
```

## Comparing `FLAI_CAUSAL-1.0.5.tar` & `FLAI_CAUSAL-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:14:38.142559 FLAI_CAUSAL-1.0.5/
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:14:38.142559 FLAI_CAUSAL-1.0.5/FLAI/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/FLAI/__init__.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9020 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/FLAI/causal_graph.py
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/FLAI/data.py
-drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:14:38.142559 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:14:38.000000 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-02 20:14:38.000000 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/SOURCES.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-02 20:14:38.000000 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/dependency_links.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      124 2023-06-02 20:14:38.000000 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/requires.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-02 20:14:38.000000 FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/top_level.txt
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/LICENSE
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:14:38.142559 FLAI_CAUSAL-1.0.5/PKG-INFO
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      238 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/README.md
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-02 20:14:38.142559 FLAI_CAUSAL-1.0.5/setup.cfg
--rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1453 2023-06-02 20:14:01.000000 FLAI_CAUSAL-1.0.5/setup.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/FLAI/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/__init__.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     9020 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/causal_graph.py
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     5236 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/FLAI/data.py
+drwxr-xr-x   0 rugonzs   (1000) rugonzs   (1000)        0 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      251 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/SOURCES.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        1 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/dependency_links.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      144 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/requires.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)        5 2023-06-02 20:18:52.000000 FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/top_level.txt
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)    11357 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/LICENSE
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      554 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/PKG-INFO
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)      238 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/README.md
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)       38 2023-06-02 20:18:52.161269 FLAI_CAUSAL-1.0.6/setup.cfg
+-rw-r--r--   0 rugonzs   (1000) rugonzs   (1000)     1475 2023-06-02 20:18:18.000000 FLAI_CAUSAL-1.0.6/setup.py
```

### Comparing `FLAI_CAUSAL-1.0.5/FLAI/causal_graph.py` & `FLAI_CAUSAL-1.0.6/FLAI/causal_graph.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.5/FLAI/data.py` & `FLAI_CAUSAL-1.0.6/FLAI/data.py`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.5/FLAI_CAUSAL.egg-info/PKG-INFO` & `FLAI_CAUSAL-1.0.6/FLAI_CAUSAL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAI-CAUSAL
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FLAI_CAUSAL-1.0.5/LICENSE` & `FLAI_CAUSAL-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAI_CAUSAL-1.0.5/PKG-INFO` & `FLAI_CAUSAL-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAI_CAUSAL
-Version: 1.0.5
+Version: 1.0.6
 Summary: Library to creat causal model and mitigate the bias.
 Home-page: https://github.com/rugonzs/FLAI
 Author: Rubén González Sendino
 Author-email: rubo.g@icloud.com
 License: Apache-2.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `FLAI_CAUSAL-1.0.5/setup.py` & `FLAI_CAUSAL-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.0.5' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '1.0.6' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'FLAI_CAUSAL' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Rubén González Sendino' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'rubo.g@icloud.com' #Modificar con vuestros datos
 URL = 'https://github.com/rugonzs/FLAI' #Modificar con vuestros datos
 
 LICENSE = 'Apache-2.0 license' #Tipo de licencia
 DESCRIPTION = 'Library to creat causal model and mitigate the bias.' #Descripción corta
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8') #Referencia al documento README con una descripción más elaborada
 LONG_DESC_TYPE = "text/markdown"
 
 
 #Paquetes necesarios para que funcione la libreía. Se instalarán a la vez si no lo tuvieras ya instalado
 INSTALL_REQUIRES = [
-      'bnlearn==0.7.8','networkx==2.8.8','matplotlib==3.6.2','pgmpy==0.1.20','numpy==1.23.4', 'pandas==1.5.1','scikit-learn==1.0.2','scipy==1.9.3'
+      'bnlearn==0.7.8','networkx==2.8.8','matplotlib==3.6.2','pgmpy==0.1.20','numpy==1.23.4', 'pandas==1.5.1','scikit-learn==1.0.2','scipy==1.9.3','statsmodels==0.13.5'
       ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
```

