# Comparing `tmp/mecoda-nat-0.5.8.tar.gz` & `tmp/mecoda-nat-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecoda-nat-0.5.8.tar", last modified: Fri Mar 25 13:21:39 2022, max compression
+gzip compressed data, was "mecoda-nat-0.6.0.tar", last modified: Fri Jun  2 13:45:57 2023, max compression
```

## Comparing `mecoda-nat-0.5.8.tar` & `mecoda-nat-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 anomalia  (1000) anomalia  (1000)        0 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)    35149 2021-10-27 16:58:18.000000 mecoda-nat-0.5.8/LICENSE
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)    11419 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/PKG-INFO
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)     8669 2021-11-04 19:25:13.000000 mecoda-nat-0.5.8/README.md
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)       38 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/setup.cfg
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)     1423 2022-03-25 13:19:44.000000 mecoda-nat-0.5.8/setup.py
-drwxrwxr-x   0 anomalia  (1000) anomalia  (1000)        0 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/src/
-drwxrwxr-x   0 anomalia  (1000) anomalia  (1000)        0 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/src/mecoda_nat/
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)      312 2022-03-25 08:13:10.000000 mecoda-nat-0.5.8/src/mecoda_nat/__init__.py
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)    11934 2022-03-25 13:17:42.000000 mecoda-nat-0.5.8/src/mecoda_nat/mecoda_nat.py
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)     2316 2021-11-17 15:57:54.000000 mecoda-nat-0.5.8/src/mecoda_nat/models.py
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)        0 2021-10-27 16:58:18.000000 mecoda-nat-0.5.8/src/mecoda_nat/py.typed
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)     1646 2022-02-17 13:01:13.000000 mecoda-nat-0.5.8/src/mecoda_nat/views.py
-drwxrwxr-x   0 anomalia  (1000) anomalia  (1000)        0 2022-03-25 13:21:39.539823 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)    11419 2022-03-25 13:21:39.000000 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/PKG-INFO
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)      344 2022-03-25 13:21:39.000000 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/SOURCES.txt
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)        1 2022-03-25 13:21:39.000000 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/dependency_links.txt
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)       36 2022-03-25 13:21:39.000000 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/requires.txt
--rw-rw-r--   0 anomalia  (1000) anomalia  (1000)       11 2022-03-25 13:21:39.000000 mecoda-nat-0.5.8/src/mecoda_nat.egg-info/top_level.txt
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-06-02 13:45:57.591753 mecoda-nat-0.6.0/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11422 2023-06-02 13:45:57.591753 mecoda-nat-0.6.0/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     8669 2022-12-21 20:25:44.000000 mecoda-nat-0.6.0/README.md
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       38 2023-06-02 13:45:57.591753 mecoda-nat-0.6.0/setup.cfg
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1426 2023-06-02 13:43:36.000000 mecoda-nat-0.6.0/setup.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-06-02 13:45:57.587753 mecoda-nat-0.6.0/src/
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-06-02 13:45:57.591753 mecoda-nat-0.6.0/src/mecoda_nat/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      312 2022-12-21 20:25:44.000000 mecoda-nat-0.6.0/src/mecoda_nat/__init__.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    15797 2023-06-01 11:02:03.000000 mecoda-nat-0.6.0/src/mecoda_nat/mecoda_nat.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     2281 2023-06-01 08:43:40.000000 mecoda-nat-0.6.0/src/mecoda_nat/models.py
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        0 2022-12-21 20:25:44.000000 mecoda-nat-0.6.0/src/mecoda_nat/py.typed
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)     1646 2022-12-21 20:25:44.000000 mecoda-nat-0.6.0/src/mecoda_nat/views.py
+drwxr-xr-x   0 anomalia  (1000) anomalia  (1000)        0 2023-06-02 13:45:57.591753 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)    11422 2023-06-02 13:45:57.000000 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/PKG-INFO
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)      336 2023-06-02 13:45:57.000000 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/SOURCES.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)        1 2023-06-02 13:45:57.000000 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/dependency_links.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       36 2023-06-02 13:45:57.000000 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/requires.txt
+-rw-r--r--   0 anomalia  (1000) anomalia  (1000)       11 2023-06-02 13:45:57.000000 mecoda-nat-0.6.0/src/mecoda_nat.egg-info/top_level.txt
```

### Comparing `mecoda-nat-0.5.8/PKG-INFO` & `mecoda-nat-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mecoda-nat
-Version: 0.5.8
+Version: 0.6.0
 Summary: Library to download information collected in Natusfera API.
 Home-page: https://github.com/pynomaly/mecoda-nat
 Author: Ana Alvarez
-Author-email: anomalia@disroot.org
+Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Description: ![](docs/logo-cos4cloud-middle.png)
         
         Library to extract information collected in the Natusfera API. This library is part of MECODA (ModulE for Citizen Observatory Data Analysis), aimed to facilitate analysis and viewing of citizen science data.
         
         
         # Instalation
```

### Comparing `mecoda-nat-0.5.8/README.md` & `mecoda-nat-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mecoda-nat-0.5.8/setup.py` & `mecoda-nat-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="mecoda-nat",
-    version="0.5.8",
+    version="0.6.0",
     description="Library to download information collected in Natusfera API.",
     author="Ana Alvarez",
-    author_email="anomalia@disroot.org",
+    author_email="ana.alvarez@icm.csic.es",
     license="GNU General Public License v3",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/pynomaly/mecoda-nat",
     packages=find_packages("src"),
     package_dir={"": "src"},
     package_data={"mecoda_nat": ["py.typed"]},
```

### Comparing `mecoda-nat-0.5.8/src/mecoda_nat/models.py` & `mecoda-nat-0.6.0/src/mecoda_nat/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     iconic_taxon: Optional[str] = None
     taxon_id: Optional[int] = None
     taxon_name: Optional[str] = None
     taxon_ancestry: Optional[str] = None
     latitude: Optional[float] = None
     longitude: Optional[float] = None
     place_name: Optional[str] = None
-    place_id: Optional[int] = None
     quality_grade: Optional[str] = None 
     user_id: Optional[int] = None
     user_login: Optional[str] = None
     photos: List[Photo] = []
     num_identification_agreements: Optional[int] = None
     num_identification_disagreements: Optional[int] = None
     identifications_count: Optional[int] = None
```

### Comparing `mecoda-nat-0.5.8/src/mecoda_nat/views.py` & `mecoda-nat-0.6.0/src/mecoda_nat/views.py`

 * *Files identical despite different names*

### Comparing `mecoda-nat-0.5.8/src/mecoda_nat.egg-info/PKG-INFO` & `mecoda-nat-0.6.0/src/mecoda_nat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mecoda-nat
-Version: 0.5.8
+Version: 0.6.0
 Summary: Library to download information collected in Natusfera API.
 Home-page: https://github.com/pynomaly/mecoda-nat
 Author: Ana Alvarez
-Author-email: anomalia@disroot.org
+Author-email: ana.alvarez@icm.csic.es
 License: GNU General Public License v3
 Description: ![](docs/logo-cos4cloud-middle.png)
         
         Library to extract information collected in the Natusfera API. This library is part of MECODA (ModulE for Citizen Observatory Data Analysis), aimed to facilitate analysis and viewing of citizen science data.
         
         
         # Instalation
```

