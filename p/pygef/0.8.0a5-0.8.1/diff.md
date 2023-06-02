# Comparing `tmp/pygef-0.8.0a5.tar.gz` & `tmp/pygef-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygef-0.8.0a5.tar", last modified: Tue Mar  7 11:55:42 2023, max compression
+gzip compressed data, was "pygef-0.8.1.tar", last modified: Fri Jun  2 08:16:52 2023, max compression
```

## Comparing `pygef-0.8.0a5.tar` & `pygef-0.8.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.710400 pygef-0.8.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-07 11:55:10.000000 pygef-0.8.0a5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-03-07 11:55:42.710400 pygef-0.8.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-03-07 11:55:10.000000 pygef-0.8.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-03-07 11:55:10.000000 pygef-0.8.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 11:55:42.710400 pygef-0.8.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-07 11:55:10.000000 pygef-0.8.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.706400 pygef-0.8.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.710400 pygef-0.8.0a5/src/pygef/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.710400 pygef-0.8.0a5/src/pygef/broxml/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/parse_bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/parse_cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/broxml/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.710400 pygef-0.8.0a5/src/pygef/gef/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/expressions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23964 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/gef.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/gef/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-03-07 11:55:10.000000 pygef-0.8.0a5/src/pygef/shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:55:42.710400 pygef-0.8.0a5/src/pygef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-03-07 11:55:42.000000 pygef-0.8.0a5/src/pygef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-07 11:55:42.000000 pygef-0.8.0a5/src/pygef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 11:55:42.000000 pygef-0.8.0a5/src/pygef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-07 11:55:42.000000 pygef-0.8.0a5/src/pygef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-07 11:55:42.000000 pygef-0.8.0a5/src/pygef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-02 08:16:42.000000 pygef-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-02 08:16:52.963508 pygef-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-02 08:16:42.000000 pygef-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-02 08:16:42.000000 pygef-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:16:52.963508 pygef-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 08:16:42.000000 pygef-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/broxml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/parse_bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/parse_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/gef/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9298 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/gef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/parse_bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/parse_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/top_level.txt
```

### Comparing `pygef-0.8.0a5/LICENSE.txt` & `pygef-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygef-0.8.0a5/PKG-INFO` & `pygef-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygef
-Version: 0.8.0a5
+Version: 0.8.1
 Summary: Parse soil measurument data.
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `pygef-0.8.0a5/README.md` & `pygef-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pygef-0.8.0a5/pyproject.toml` & `pygef-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygef"
-version = "0.8.0a5"
+version = "0.8.1"
 description = "Parse soil measurument data."
 dependencies = [
-    "polars[pyarrow]>=0.14.28",
-    "matplotlib>=3.4.2",
-    "lxml==4.9.1",
-    "gef-file-to-map==0.1.0",
+    "polars[pyarrow]>=0.16.3,<0.19",
+    "matplotlib>=3.6,<4.0",
+    "lxml>=4.9.1,<5.0",
+    "gef-file-to-map>=0.1,<0.2",
 ]
 requires-python = ">=3.9"
 license = { file = "LICENSE.txt" }
 readme = "README.md"
 keywords = ["gef"]
 
 [project.urls]
```

### Comparing `pygef-0.8.0a5/src/pygef/broxml/mapping.py` & `pygef-0.8.1/src/pygef/broxml/mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 class _MappingParameters:
     @lru_cache(1)
     def dist_table(self) -> pl.DataFrame:
         mapping = self.bro_to_dict()
         return pl.DataFrame(
             {
-                "geotechnical_soil_name": list(mapping.keys()),
-                "soil_dist": list(mapping.values()),
+                "geotechnicalSoilName": list(mapping.keys()),
+                "soilDistribution": list(mapping.values()),
             }
-        ).sort("geotechnical_soil_name")
+        ).sort("geotechnicalSoilName")
 
     @lru_cache(1)
     def bro_to_dict(self) -> dict[str, pl.Series]:
         # SoilNameISO14688
         # > https://publiek.broservices.nl/bro/refcodes/v1/codes?domain=urn%3Abro%3Abhrgt%3AGeotechnicalSoilName&version=latest
         # SoilNameNEN5104
         # > https://publiek.broservices.nl/bro/refcodes/v1/codes?domain=urn%3Abro%3Abhrgt%3ASoilNameNEN5104&version=latest
@@ -59,19 +59,19 @@
             "sterkZandigGrind": [0.0, 0.6, 0.4, 0.0, 0.0, 0.0],
             "uiterstZandigGrind": [0.0, 0.5, 0.5, 0.0, 0.0, 0.0],  # SoilNameNEN5104
             "siltigGrind": [0.0, 0.7, 0.0, 0.3, 0.0, 0.0],
             "keiigGrind": [0.3, 0.7, 0.0, 0.0, 0.0, 0.0],
             "zand": [0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
             "zandMetKeien": [0.3, 0.0, 0.7, 0.0, 0.0, 0.0],
             "zandMetKeitjes": [0.3, 0.0, 0.7, 0.0, 0.0, 0.0],
-            "zwakGrindigZand": [0.2, 0.0, 0.8, 0.0, 0.0, 0.0],
-            "sterkGrindigZand": [0.4, 0.0, 0.6, 0.0, 0.0, 0.0],
+            "zwakGrindigZand": [0.0, 0.2, 0.8, 0.0, 0.0, 0.0],
+            "sterkGrindigZand": [0.0, 0.4, 0.6, 0.0, 0.0, 0.0],
             "siltigZand": [0.0, 0.0, 0.7, 0.3, 0.0, 0.0],
             "zwakSiltigZand": [0.0, 0.0, 0.8, 0.2, 0.0, 0.0],  # SoilNameNEN5104
-            "matigSiltigZand": [0.0, 0.0, 0.8, 0.2, 0.0, 0.0],  # SoilNameNEN5104
+            "matigSiltigZand": [0.0, 0.0, 0.7, 0.3, 0.0, 0.0],  # SoilNameNEN5104
             "sterkSiltigZand": [0.0, 0.0, 0.6, 0.4, 0.0, 0.0],  # SoilNameNEN5104
             "uiterstSiltigZand": [0.0, 0.0, 0.5, 0.5, 0.0, 0.0],  # SoilNameNEN5104
             "siltigZandMetGrind": [0.0, 0.15, 0.7, 0.15, 0.0, 0.0],
             "kleiigZand": [0.0, 0.0, 0.7, 0.0, 0.3, 0.0],
             "kleiigZandMetGrind": [0.0, 0.15, 0.7, 0.0, 0.15, 0.0],
             "silt": [0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
             "siltMetKeien": [0.3, 0.0, 0.0, 0.7, 0.0, 0.0],
@@ -84,21 +84,21 @@
             "sterkZandigSiltMetGrind": [0.0, 0.2, 0.2, 0.6, 0.0, 0.0],
             "klei": [0.0, 0.0, 0.0, 0.0, 1.0, 0.0],
             "kleiMetKeien": [0.3, 0.0, 0.0, 0.0, 0.7, 0.0],
             "kleiMetKeitjes": [0.3, 0.0, 0.0, 0.0, 0.7, 0.0],
             "zwakGrindigeKlei": [0.0, 0.2, 0.0, 0.0, 0.8, 0.0],
             "sterkGrindigeKlei": [0.0, 0.4, 0.0, 0.0, 0.6, 0.0],
             "zwakZandigeKlei": [0.0, 0.0, 0.2, 0.0, 0.8, 0.0],
-            "matigZandigeKlei": [0.0, 0.0, 0.2, 0.0, 0.8, 0.0],  # SoilNameNEN5104
+            "matigZandigeKlei": [0.0, 0.0, 0.3, 0.0, 0.7, 0.0],  # SoilNameNEN5104
             "zwakZandigeKleiMetGrind": [0.0, 0.1, 0.1, 0.0, 0.8, 0.0],
             "sterkZandigeKlei": [0.0, 0.0, 0.4, 0.0, 0.6, 0.0],
             "sterkZandigeKleiMetGrind": [0.0, 0.2, 0.2, 0.0, 0.6, 0.0],
             "organischKlei": [0.0, 0.0, 0.0, 0.0, 0.6, 0.4],
             "matigSiltigeKlei": [0.0, 0.0, 0.0, 0.2, 0.8, 0.0],  # SoilNameNEN5104
-            "uiterstSiltigeKlei": [0.0, 0.0, 0.0, 0.4, 0.6, 0.0],  # SoilNameNEN5104
+            "uiterstSiltigeKlei": [0.0, 0.0, 0.0, 0.5, 0.5, 0.0],  # SoilNameNEN5104
             "sterkSiltigeKlei": [0.0, 0.0, 0.0, 0.3, 0.7, 0.0],  # SoilNameNEN5104
             "zwakSiltigeKlei": [0.0, 0.0, 0.0, 0.1, 0.9, 0.0],  # SoilNameNEN5104
             "sterkZandigeLeem": [0.1, 0.25, 0.1, 0.45, 0.05, 0.05],  # SoilNameNEN5104
             "zwakZandigeLeem": [0.1, 0.15, 0.1, 0.45, 0.1, 0.1],  # SoilNameNEN5104
             "detritus": [0.0, 0.0, 0.0, 0.0, 0.0, 1.0],
             "detritusNietGespecificeerd": [
                 0.0,
```

### Comparing `pygef-0.8.0a5/src/pygef/broxml/parse_bore.py` & `pygef-0.8.1/src/pygef/broxml/parse_bore.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import re
 from pathlib import Path
 
 from lxml import etree
 
 from pygef.bore import BoreData
 from pygef.broxml import resolvers
-from pygef.broxml.mapping import MAPPING_PARAMETERS
 from pygef.broxml.xml_parser import read_xml
 
 # maps keyword argument to:
 # xpath: query passed to elementree.find
 # resolver: A function that converts the string to the proper datatype
 #           Fn(str) -> Any
 # el-atrr: Optional: attribute of an element taken before send to resolver
@@ -72,14 +71,19 @@
 BORE_ATTRIBS_V2 = {
     "bro_id": {"xpath": "brocom:broId"},
     "research_report_date": {
         "xpath": "./researchReportDate/brocom:date",
         "resolver": resolvers.parse_date,
         "el-attr": "text",
     },
+    "groundwater_level": {
+        "xpath": "./boring/bhrgtcom:groundwaterLevel",
+        "resolver": resolvers.parse_float,
+        "el-attr": "text",
+    },
     "description_procedure": {
         "xpath": "./boreholeSampleDescription/bhrgtcom:descriptionProcedure",
         "el-attr": "text",
     },
     "delivered_location": {
         "xpath": "./deliveredLocation/bhrgtcom:location/gml:Point",
         "resolver": resolvers.parse_gml_location,
@@ -126,35 +130,21 @@
     "data": {
         "xpath": "./boreholeSampleDescription/bhrgtcom:descriptiveBoreholeLog",
         "resolver": resolvers.process_bore_result,
     },
 }
 
 
-def read_bore(
-    file: io.BytesIO | Path | str, include_soil_dist: bool = True
-) -> list[BoreData]:
+def read_bore(file: io.BytesIO | Path | str) -> list[BoreData]:
     if isinstance(file, str) and not os.path.exists(file):
         root = etree.fromstring(file).getroot()
     else:
         root = etree.parse(file).getroot()
     match = re.compile(r"xsd/.*/(\d\.\d)")
     matched = match.search(root.nsmap["bhrgtcom"])
 
     if matched is None:
         raise ValueError("could not find the brhtcom version")
     else:
         if 3.0 >= float(matched.group(1)) < 2.0:
             raise ValueError("only bhrgtcom/2.x is supported ")
-        all_bd = read_xml(root, BoreData, BORE_ATTRIBS_V2, "dispatchDocument")
-
-    if include_soil_dist:
-        out = []
-        for bore_data in all_bd:
-            tbl = MAPPING_PARAMETERS.dist_table()
-            bore_data.data = bore_data.data.join(
-                tbl, on="geotechnical_soil_name", how="left"
-            )
-            out.append(bore_data)
-        return out
-    else:
-        return all_bd
+        return read_xml(root, BoreData, BORE_ATTRIBS_V2, "dispatchDocument")
```

### Comparing `pygef-0.8.0a5/src/pygef/broxml/parse_cpt.py` & `pygef-0.8.1/src/pygef/broxml/parse_cpt.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,19 @@
         "el-attr": "text",
     },
     "quality_class": {
         "xpath": "./conePenetrometerSurvey/cptcommon:qualityClass",
         "resolver": resolvers.parse_quality_class,
         "el-attr": "text",
     },
+    "groundwater_level": {
+        "xpath": "./additionalInvestigation/cptcommon:groundwaterLevel",
+        "resolver": resolvers.parse_float,
+        "el-attr": "text",
+    },
     "predrilled_depth": {
         "xpath": "./conePenetrometerSurvey/cptcommon:trajectory/cptcommon:predrilledDepth",
         "resolver": resolvers.parse_float,
         "el-attr": "text",
     },
     "final_depth": {
         "xpath": "./conePenetrometerSurvey/cptcommon:trajectory/cptcommon:finalDepth",
@@ -174,15 +179,15 @@
     "delivered_vertical_position_offset": {
         "xpath": "./deliveredVerticalPosition/cptcommon:offset",
         "resolver": resolvers.parse_float,
         "el-attr": "text",
     },
     "delivered_vertical_position_datum": {
         "xpath": "./deliveredVerticalPosition/cptcommon:verticalDatum",
-        "resolver": resolvers.lower_text,
+        "resolver": resolvers.parse_local_vertical_reference_point_class,
         "el-attr": "text",
     },
     "delivered_vertical_position_reference_point": {
         "xpath": "./deliveredVerticalPosition/cptcommon:localVerticalReferencePoint",
         "resolver": resolvers.lower_text,
         "el-attr": "text",
     },
```

### Comparing `pygef-0.8.0a5/src/pygef/broxml/resolvers.py` & `pygef-0.8.1/src/pygef/broxml/resolvers.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import date, datetime
 from typing import Any, List
 from warnings import warn
 
 import polars as pl
 from lxml import etree
 
-from pygef.common import Location
+from pygef.common import Location, VerticalDatumClass
 from pygef.cpt import QualityClass
 
 
 def lower_text(val: str, **kwargs: dict[Any, Any]) -> str:
     return val.lower()
 
 
@@ -131,27 +131,23 @@
             sand_median_class.append(None)
 
     # merge NEN and ISO names
     geotechnical_soil_name = [
         word if word != "unknown" else geotechnical_soil_name_nen[i]
         for i, word in enumerate(geotechnical_soil_name_iso)
     ]
-    variables = locals()
     return pl.DataFrame(
         {
-            name: variables[name]
-            for name in [
-                "upper_boundary",
-                "lower_boundary",
-                "geotechnical_soil_name",
-                "color",
-                "dispersed_inhomogenity",
-                "organic_matter_content_class",
-                "sand_median_class",
-            ]
+            "upperBoundary": upper_boundary,
+            "lowerBoundary": lower_boundary,
+            "geotechnicalSoilName": geotechnical_soil_name,
+            "color": color,
+            "dispersedInhomogeneity": dispersed_inhomogenity,
+            "organicMatterContentClass": organic_matter_content_class,
+            "sandMedianClass": sand_median_class,
         }
     )
 
 
 def process_cpt_result(el: etree.Element, **kwargs: dict[Any, Any]) -> pl.DataFrame:
     """
     Parse the cpt data into a `DataFrame`
@@ -195,18 +191,19 @@
     # we strip the data because there is leading and trailing whitespace.
     data = el.find(f"{prefix}/cptcommon:values", namespaces=namespaces).text.strip()
     return pl.read_csv(
         data.encode(),
         new_columns=columns,
         columns=selection,
         has_header=False,
-        sep=delimiter,
+        separator=delimiter,
         eol_char=new_line_char,
         ignore_errors=True,
-    )
+        null_values="-999999",
+    ).drop_nulls("coneResistance")
 
 
 def parse_gml_location(el: etree.Element, **kwargs: dict[Any, Any]) -> Location:
     """Resolver for standardizedLocation/brocom:location"""
     srs_name = el.attrib["srsName"]
     pos = next(el.iterfind("./gml:pos", namespaces=kwargs["namespaces"])).text
     (x, y) = parse_position(pos)
@@ -225,14 +222,28 @@
         return QualityClass.Class4
     if val == "onbekend" or val == "unknown":
         return QualityClass.Unknown
     warn(f"quality class '{val}' is unknown")
     return QualityClass.Unknown
 
 
+def parse_local_vertical_reference_point_class(
+    val: str, **kwargs: dict[Any, Any]
+) -> VerticalDatumClass:
+    val = val.lower().strip()
+    if val == "nap":
+        return VerticalDatumClass.NAP
+    if val == "msl":
+        return VerticalDatumClass.MSL
+    if val == "lat":
+        return VerticalDatumClass.LAT
+    warn(f"vertical datum class '{val}' is unknown")
+    return VerticalDatumClass.Unknown
+
+
 def parse_position(pos: str) -> tuple[float, float]:
     """
     Parse a position tuple
 
     Parameters
     ----------
     pos
```

### Comparing `pygef-0.8.0a5/src/pygef/broxml/xml_parser.py` & `pygef-0.8.1/src/pygef/broxml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.0a5/src/pygef/common.py` & `pygef-0.8.1/src/pygef/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
+from enum import Enum
 from typing import List
 
 import polars as pl
 
 
 @dataclass
 class Location:
     """DataClass that holds the standardized location information"""
 
     srs_name: str
     x: float
     y: float
 
 
+class VerticalDatumClass(Enum):
+    """DataClass that holds the standardized vertical reference information"""
+
+    Unknown = "-1"
+    NAP = "31000"  # Normaal Amsterdams Peil
+    BOP = "32000"  # Ostend Level (GEF)
+    MSL = "49000"  # Mean Sea Level
+    LAT = "00001"  # Lowest Astronomical Tide
+    TAW = "32001"  # (GEF)
+
+
 def assign_multiple_columns(
     df: pl.DataFrame, columns: List[str], partial_df: pl.DataFrame
 ) -> pl.DataFrame:
     """
     Helper function to assign multiple columns
 
     :param df: original Dataframe
@@ -36,27 +48,31 @@
     :param df: DataFrame
     :param columns: columns names
     :return: DataFrame
     """
     return assign_multiple_columns(df, columns, df[columns] * 10**-3)
 
 
-def nap_to_depth(zid: float, ref: float) -> float:
+def offset_to_depth(ref: float | None, offset: float | None) -> float | None:
     """
     Transform depth with respect to reference level to depth
 
-    :param zid: surface reference level
+    :param offset: surface reference level
     :param ref: z
     :return: depth
     """
-    return -(ref - zid)
+    if offset is None or ref is None:
+        return None
+    return -(ref - offset)
 
 
-def depth_to_nap(zid: float, depth: float) -> float:
+def depth_to_offset(depth: float | None, offset: float | None) -> float | None:
     """
     Transform depth to depth with respect to reference level
 
-    :param zid: surface reference level
+    :param offset: surface reference level
     :param depth: z
     :return: depth with respect to reference level
     """
-    return zid - depth
+    if offset is None or depth is None:
+        return None
+    return offset - depth
```

### Comparing `pygef-0.8.0a5/src/pygef/exceptions.py` & `pygef-0.8.1/src/pygef/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.0a5/src/pygef/gef/mapping.py` & `pygef-0.8.1/src/pygef/gef/mapping.py`

 * *Files 19% similar despite different names*

```diff
@@ -282,7 +282,50 @@
             else:
                 return "grind"
 
         return "niet gedefinieerd"
 
 
 MAPPING_PARAMETERS = _MappingParameters()
+COLUMN_NAMES_BORE = [
+    "upperBoundary",  # 1
+    "lowerBoundary",  # 2
+    "lutumPercentage",  # 3
+    "siltPercentage",  # 4
+    "sandPercentage",  # 5
+    "gravelPercentage",  # 6
+    "organicMatterPercentage",  # 7
+    "sandMedianClass",  # 8
+    "gravelMedianClass",  # 9
+]
+MAP_QUANTITY_NUMBER_COLUMN_NAME_BORE = dict(enumerate(COLUMN_NAMES_BORE, 1))
+MAP_QUANTITY_NUMBER_COLUMN_NAME_CPT = {
+    1: "penetrationLength",
+    2: "coneResistance",
+    3: "localFriction",
+    4: "frictionRatio",
+    5: "porePressureU1",
+    6: "porePressureU2",
+    7: "porePressureU3",
+    8: "inclinationResultant",
+    9: "inclinationNS",
+    10: "inclinationEW",
+    11: "depth",
+    12: "elapsedTime",
+    13: "correctedConeResistance",
+    14: "netConeResistance",
+    15: "poreRatio",
+    16: "coneResistanceRatio",
+    17: "soilDensity",
+    18: "porePressure",
+    19: "verticalPorePressureTotal",
+    20: "verticalPorePressureEffective",
+    21: "inclinationX",
+    22: "inclinationY",
+    23: "electricalConductivity",
+    31: "magneticFieldStrengthX",
+    32: "magneticFieldStrengthY",
+    33: "magneticFieldStrengthZ",
+    34: "magneticFieldStrengthTotal",
+    35: "magneticInclination",
+    36: "magneticDeclination",
+}
```

### Comparing `pygef-0.8.0a5/src/pygef/gef/utils.py` & `pygef-0.8.1/src/pygef/gef/utils.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.0a5/src/pygef/plotting.py` & `pygef-0.8.1/src/pygef/plotting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,101 +1,112 @@
 from __future__ import annotations
 
 from typing import List, Tuple
 
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
+import matplotlib.ticker as plticker
 import numpy as np
-import polars as pl
 from matplotlib.gridspec import GridSpec
 
 from pygef.bore import BoreData
 from pygef.cpt import CPTData
 
 try:
     import contextily as ctx
 except ImportError:
     ctx = None
 
 FigureSize = (8, 12)
+TickLoc = plticker.MultipleLocator(base=0.5)
 
 
 def plot_cpt(
-    data: CPTData, ax: plt.Axes | None = None, dpi: int = 100
+    data: CPTData, ax: plt.Axes | None = None, dpi: int = 100, use_offset: bool = False
 ) -> Tuple[plt.Axes, plt.Axes, plt.Axes]:
     """
     Create a plot with three axes.
-        - cone_resistance [Mpa]
+        - cone_resistance [MPa]
         - friction_ratio [%] (twiny)
         - friction [MPa] (twiny)
 
     :param data: (BoreData) Bore data object
     :param ax: (Axes, optional) Axes object used to add axes
     :param dpi: (int, optional)  Default is 100 Resolution of the figure.
+    :param use_offset: (bool, optional)  Default is False Plot depth with respect to offset.
     """
-
-    df = data.data.select(
-        pl.when(pl.all().abs() > 1e4).then(None).otherwise(pl.all()).keep_name()
-    )
-    yname = "depth" if "depth" in df.columns else "penetrationLength"
+    df = data.data
+    if use_offset:
+        yname = "depthOffset"
+        label_name = "depth" if "depth" in data.columns else "penetrationLength"
+    else:
+        yname = "depth" if "depth" in data.columns else "penetrationLength"
+        label_name = yname
 
     if ax is None:
         fig = plt.figure(figsize=FigureSize, dpi=dpi, layout="tight")
         ax = fig.subplots(1, 1)
 
     p1 = None
+    p11 = None
+    p12 = None
     ax2 = ax.twiny()
     p2 = None
     ax3 = ax.twiny()
     p3 = None
     p4 = None
 
     axes = (ax, ax2, ax3)
 
     # set the properties on the coneResistance axes
     ax.xaxis.set_ticks_position("top")
     ax.xaxis.set_label_position("top")
     ax.spines["top"].set_position(("axes", 1))
     ax.set_xlim(0, 40)
-    ax.set_ylabel(f"{yname} [m]")
     ax.set_xlabel("$q_c$ [MPa]")
     ax.xaxis.label.set_color("#2d2e87")
-    ax.invert_yaxis()
+    if not use_offset:
+        ax.invert_yaxis()
+
+    # set axis label
+    if use_offset:
+        ax.set_ylabel(f"{label_name} [m w.r.t. vertical position offset]")
+    else:
+        ax.set_ylabel(f"{label_name} [m]")
 
     # create grid
     major_ticks = np.arange(0, 41, 5)
     minor_ticks = np.arange(0, 41, 2.5)
     ax.set_xticks(major_ticks)
     ax.set_xticks(minor_ticks, minor=True)
     ax.grid(which="both")
     ax.grid(which="minor", alpha=0.2)
     ax.grid(which="major", alpha=0.5)
+    ax.yaxis.set_major_locator(TickLoc)
 
     # set the properties on the localFriction axes
     ax2.xaxis.set_ticks_position("top")
     ax2.xaxis.set_label_position("top")
     ax2.spines["top"].set_position(("axes", 1.05))
     ax2.set_xlabel("$f_s$ [MPa]")
     ax2.set_xlim(0, 0.8)
     ax2.xaxis.label.set_color("#e04913")
-    ax2.invert_yaxis()
 
     # set the properties on the frictionRatio axes
     ax3.xaxis.set_ticks_position("top")
     ax3.xaxis.set_label_position("top")
     ax3.spines["top"].set_position(("axes", 1.1))
     ax3.set_xlabel("$R_f$ [%]")
     ax3.set_xlim(0, 16)
     ax3.invert_xaxis()
-    ax3.invert_yaxis()
     ax3.xaxis.label.set_color("tab:gray")
 
     # add data to figure
     # plot coneResistance
-    if "coneResistance" in df.columns:
+    if "coneResistance" in data.columns:
         (p1,) = ax.plot(
             df["coneResistance"], df[yname], color="#2d2e87", label="coneResistance"
         )
     # plot localFriction
     if "localFriction" in df.columns:
         (p2,) = ax2.plot(
             df["localFriction"], df[yname], color="#e04913", label="localFriction"
@@ -107,84 +118,118 @@
             df["frictionRatio"],
             df[yname],
             label="frictionRatio measured",
             color="tab:gray",
         )
 
     # plot computed frictionRatio
-    if "localFriction" in df.columns and "coneResistance" in df.columns:
+    if "frictionRatioComputed" in df.columns:
         (p4,) = ax3.plot(
-            df["localFriction"] / df["coneResistance"] * 100,
+            df["frictionRatioComputed"],
             df[yname],
             label="frictionRatio computed",
             ls="dashed",
             color="tab:gray",
         )
+    # add hlines
+    if data.groundwater_level is not None:
+        value = data.groundwater_level_offset if use_offset else data.groundwater_level
+        p11 = ax.axhline(
+            value,
+            label=f"groundwater level: {value:.2f}",
+            color="tab:blue",
+            ls="dashed",
+        )
+    if data.predrilled_depth is not None:
+        value = data.predrilled_depth_offset if use_offset else data.predrilled_depth
+        p12 = ax.axhline(
+            value,
+            label=f"predrilled depth: {value:.2f}",
+            color="tab:brown",
+            ls="dashed",
+        )
 
     # add legend
     ax.legend(
         loc="upper center",
-        title=f"CPT: {data.bro_id}",
-        handles=[i for i in [p1, p2, p3, p4] if i is not None],
+        title=f"CPT: {data.alias if data.bro_id is None else data.bro_id}",
+        handles=[i for i in [p1, p2, p3, p4, p11, p12] if i is not None],
     )
     return axes
 
 
 def plot_bore(
-    data: BoreData, ax: plt.Axes | None = None, dpi: int = 100, legend: bool = True
+    data: BoreData,
+    ax: plt.Axes | None = None,
+    dpi: int = 100,
+    legend: bool = True,
+    use_offset: bool = False,
 ) -> plt.Axes:
     """
     Create a plot with one axes.
         - soil distribution
 
     :param data: Bore data object
     :param ax: Axes object
     :param dpi: Default is 100 Resolution of the figure.
     :param legend: Default is True Add legend to the figure.
+    :param use_offset: (bool, optional)  Default is False Plot depth with respect to offset.
     """
+    if use_offset:
+        yupper = "upperBoundaryOffset"
+        ylower = "lowerBoundaryOffset"
+    else:
+        yupper = "upperBoundary"
+        ylower = "lowerBoundary"
 
     if ax is None:
         fig = plt.figure(figsize=FigureSize, dpi=dpi, layout="tight")
         ax = fig.subplots(1, 1)
 
     df = data.data
-    soil_dist = np.stack(df["soil_dist"].to_numpy())
+    soil_dist = np.stack(df["soilDistribution"].to_numpy())
     cum_soil_dist = soil_dist.cumsum(axis=1)
 
     # peat, clay, silt, sand, gravel, rocks
     legend_colors = ["#a76b29", "#578E57", "#0078C1", "#DBAD4B", "#708090", "#59626b"]
     legend_names = ["peat", "clay", "silt", "sand", "gravel", "rocks"]
-    ax.invert_yaxis()
-    ax.set_ylabel("depth [m]")
+    if not use_offset:
+        ax.invert_yaxis()
+    # set axis label
+    if use_offset:
+        ax.set_ylabel("depth [m w.r.t. vertical position offset]")
+    else:
+        ax.set_ylabel("depth [m]")
     ax.set_xlabel("cumulative soil fraction [-]")
+    ax.yaxis.set_major_locator(TickLoc)
 
     for i in range(5):
         ax.fill_betweenx(
-            np.array(list(zip(df["upper_boundary"], df["lower_boundary"]))).flatten(),
+            np.array(list(zip(df[yupper], df[ylower]))).flatten(),
             np.zeros(df.shape[0] * 2),
             np.repeat(cum_soil_dist[:, -(i + 1)], 2),
             color=legend_colors[i],
         )
 
     # add the name of the soil to the plot
     for row in df.rows(named=True):
-        y = (row["lower_boundary"] - row["upper_boundary"]) / 2 + row["upper_boundary"]
-        ax.annotate(text=row["geotechnical_soil_name"], xy=(0.25, y))
+        y = (row[ylower] - row[yupper]) / 2 + row[yupper]
+        ax.annotate(text=row["geotechnicalSoilName"], xy=(0.25, y))
 
     # add legend
     if legend:
         patches = [
             mpatches.Patch(color=color, label=key)
             for key, color in zip(legend_names, legend_colors)
         ]
         ax.legend(
             handles=patches,
             bbox_to_anchor=(1, 1),
             loc="upper left",
-            title=f"BHRgt: {data.bro_id}",
+            title=f"BHRgt: {data.alias if data.bro_id is None else data.bro_id}",
         )
 
     return ax
 
 
 def plot_merge(
     bore_data: BoreData, cpt_data: CPTData, dpi: int = 100, basemap: bool = True
@@ -209,33 +254,17 @@
     fig = plt.figure(figsize=FigureSize, dpi=dpi, layout="constrained")
     gs = GridSpec(2, 2, figure=fig, width_ratios=[2, 1], height_ratios=[1, 0.5])
     ax1 = fig.add_subplot(gs[0])
     ax2 = fig.add_subplot(gs[1], sharey=ax1)
     ax3 = fig.add_subplot(gs[2:])
     axes = [ax1, ax2, ax3]
 
-    # update depth to depth with respect to offset
-    # in the Netherlands this is usually NAP
-    yname = "depth" if "depth" in cpt_data.columns else "penetrationLength"
-    cpt_data.data = cpt_data.data.with_columns(
-        (cpt_data.delivered_vertical_position_offset - pl.col(yname)).alias(yname)
-    ).sort(yname, descending=True)
-    bore_data.data = bore_data.data.with_columns(
-        (bore_data.delivered_vertical_position_offset - pl.col("lower_boundary")).alias(
-            "lower_boundary"
-        ),
-        (bore_data.delivered_vertical_position_offset - pl.col("upper_boundary")).alias(
-            "upper_boundary"
-        ),
-    )
-
     # fill axes and update ylabels
-    _ = plot_cpt(cpt_data, ax1)
-    _ = plot_bore(bore_data, ax2, legend=False)
-    ax1.set_ylabel(f"{yname} [m w.r.t. vertical position offset]")
+    _ = plot_cpt(cpt_data, ax1, use_offset=True)
+    _ = plot_bore(bore_data, ax2, legend=False, use_offset=True)
     ax2.set_ylabel("")
 
     # plot BHRgt location
     ax3.scatter(
         bore_data.delivered_location.x,
         bore_data.delivered_location.y,
         marker="s",
```

### Comparing `pygef-0.8.0a5/src/pygef/shim.py` & `pygef-0.8.1/src/pygef/shim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 import io
 import os
 from pathlib import Path
 from typing import Any
 
-from pygef import broxml
+from typing_extensions import Literal
+
 from pygef.bore import BoreData
-from pygef.common import Location
+from pygef.broxml.parse_bore import read_bore as read_bore_xml
+from pygef.broxml.parse_cpt import read_cpt as read_cpt_xml
+from pygef.common import Location, VerticalDatumClass
 from pygef.cpt import CPTData, QualityClass
-from pygef.gef.gef import _GefBore, _GefCpt
+from pygef.gef.parse_bore import _GefBore
+from pygef.gef.parse_cpt import _GefCpt
 
 GEF_ID = "#GEFID"
 
 
 def is_gef_file(file: io.BytesIO | Path | str) -> bool:
     """
     gef files start with '#GEFID' so we check the content
@@ -28,51 +32,63 @@
         with open(file, errors="ignore") as f:
             return f.read(6).startswith(GEF_ID)
     if isinstance(file, str):
         return file[:6].startswith(GEF_ID)
     raise FileNotFoundError("Could not find the GEF file.")
 
 
-def read_bore(file: io.BytesIO | Path | str, index: int = 0) -> BoreData:
+def read_bore(
+    file: io.BytesIO | Path | str,
+    index: int = 0,
+    engine: Literal["auto", "gef", "xml"] = "auto",
+) -> BoreData:
     """
     Parse the bore file. Can either be BytesIO, Path or str
 
     :param file: bore file
     :param index: only valid for xml files
+    :param engine: default is "auto". parsing engine.
+        Please note that auto engine checks if the files starts with `#GEFID`.
     """
-    if is_gef_file(file):
+    if engine == "gef" or is_gef_file(file) and engine == "auto":
         if index > 0:
             raise ValueError("an index > 0 not supported for GEF files")
         if isinstance(file, io.BytesIO):
             return gef_bore_to_bore_data(_GefBore(string=file.read().decode()))
         if os.path.exists(file):
             return gef_bore_to_bore_data(_GefBore(path=file))
         else:
             return gef_bore_to_bore_data(_GefBore(string=file))
-    return broxml.read_bore(file)[index]
+    return read_bore_xml(file)[index]
 
 
-def read_cpt(file: io.BytesIO | Path | str, index: int = 0) -> CPTData:
+def read_cpt(
+    file: io.BytesIO | Path | str,
+    index: int = 0,
+    engine: Literal["auto", "gef", "xml"] = "auto",
+) -> CPTData:
     """
     Parse the cpt file. Can either be BytesIO, Path or str
 
     :param file: bore file
     :param index: only valid for xml files
+    :param engine: default is "auto". parsing engine.
+        Please note that auto engine checks if the files starts with `#GEFID`.
     """
-    if is_gef_file(file):
+
+    if engine == "gef" or is_gef_file(file) and engine == "auto":
         if index > 0:
             raise ValueError("an index > 0 not supported for GEF files")
         if isinstance(file, io.BytesIO):
             return gef_cpt_to_cpt_data(_GefCpt(string=file.read().decode()))
         if os.path.exists(file):
             return gef_cpt_to_cpt_data(_GefCpt(path=file))
         else:
             return gef_cpt_to_cpt_data(_GefCpt(string=file))
-
-    return broxml.read_cpt(file)[index]
+    return read_cpt_xml(file)[index]
 
 
 def convert_height_system_to_vertical_datum(height_system: float) -> str:
     if height_system == 31000.0:
         return "nap"
     else:
         return str(int(height_system))
@@ -84,18 +100,20 @@
     kwargs["delivered_location"] = Location(
         # all gef files are RD new
         srs_name="urn:ogc:def:crs:EPSG::28992",
         x=gef_cpt.x,
         y=gef_cpt.y,
     )
     kwargs["standardized_location"] = None
-    kwargs["bro_id"] = gef_cpt.project_id
+    kwargs["bro_id"] = None
+    kwargs["alias"] = gef_cpt.test_id
     kwargs["data"] = gef_cpt.df
     kwargs["research_report_date"] = None
     kwargs["cpt_standard"] = None
+    kwargs["groundwater_level"] = gef_cpt.groundwater_level
     kwargs["dissipationtest_performed"] = None
     kwargs["quality_class"] = QualityClass(gef_cpt.cpt_class)
     kwargs["predrilled_depth"] = gef_cpt.pre_excavated_depth
     kwargs["final_depth"] = gef_cpt.end_depth_of_penetration_test
     kwargs["cpt_description"] = ""
     kwargs["cpt_type"] = gef_cpt.type_of_cone_penetration_test
     kwargs["cone_surface_area"] = gef_cpt.nom_surface_area_cone_tip
@@ -150,15 +168,17 @@
     kwargs[
         "zlm_pore_pressure_u2_after"
     ] = gef_cpt.zero_measurement_ppt_u2_after_penetration_test
     kwargs[
         "zlm_pore_pressure_u3_after"
     ] = gef_cpt.zero_measurement_ppt_u3_after_penetration_test
     kwargs["delivered_vertical_position_offset"] = gef_cpt.zid
-    kwargs["delivered_vertical_position_datum"] = gef_cpt.height_system
+    kwargs["delivered_vertical_position_datum"] = VerticalDatumClass(
+        str(int(gef_cpt.height_system))
+    )
 
     # TODO! parse measurementtext 9 in gef?
     kwargs["delivered_vertical_position_reference_point"] = "unknown"
 
     return CPTData(**kwargs)
 
 
@@ -168,15 +188,17 @@
     kwargs["delivered_location"] = Location(
         # all gef files are RD new
         srs_name="urn:ogc:def:crs:EPSG::28992",
         x=gef_bore.x,
         y=gef_bore.y,
     )
     kwargs["standardized_location"] = None
-    kwargs["bro_id"] = gef_bore.project_id
+    kwargs["bro_id"] = None
+    kwargs["alias"] = gef_bore.test_id
+    kwargs["groundwater_level"] = None
     kwargs["research_report_date"] = None
     kwargs["description_procedure"] = "unknown"
     kwargs["delivered_vertical_position_offset"] = gef_bore.zid
     kwargs["delivered_vertical_position_datum"] = "unknown"
     kwargs["delivered_vertical_position_reference_point"] = "unknown"
     kwargs["bore_rock_reached"] = None
     kwargs["final_bore_depth"] = None
```

### Comparing `pygef-0.8.0a5/src/pygef.egg-info/PKG-INFO` & `pygef-0.8.1/src/pygef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygef
-Version: 0.8.0a5
+Version: 0.8.1
 Summary: Parse soil measurument data.
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `pygef-0.8.0a5/src/pygef.egg-info/SOURCES.txt` & `pygef-0.8.1/src/pygef.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 src/pygef/broxml/__init__.py
 src/pygef/broxml/mapping.py
 src/pygef/broxml/parse_bore.py
 src/pygef/broxml/parse_cpt.py
 src/pygef/broxml/resolvers.py
 src/pygef/broxml/xml_parser.py
 src/pygef/gef/__init__.py
-src/pygef/gef/expressions.py
 src/pygef/gef/gef.py
-src/pygef/gef/geo.py
 src/pygef/gef/mapping.py
+src/pygef/gef/parse_bore.py
+src/pygef/gef/parse_cpt.py
 src/pygef/gef/utils.py
```

