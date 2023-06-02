# Comparing `tmp/timor_locations-0.0.6.tar.gz` & `tmp/timor_locations-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timor_locations-0.0.6.tar", max compression
+gzip compressed data, was "timor_locations-0.0.7.tar", max compression
```

## Comparing `timor_locations-0.0.6.tar` & `timor_locations-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1029 2023-05-24 16:20:08.175041 timor_locations-0.0.6/README.md
--rw-r--r--   0        0        0     1808 2023-05-29 08:16:23.791217 timor_locations-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/__init__.py
--rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.6/timor_locations/admin.py
--rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.6/timor_locations/api.py
--rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/gis_functions.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/management/commands/__init__.py
--rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.6/timor_locations/management/commands/create_topology.py
--rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.6/timor_locations/management/commands/import_timor_geo_data.py
--rw-r--r--   0        0        0     2285 2023-05-29 00:25:54.388811 timor_locations-0.0.6/timor_locations/management/commands/suco_to_topology.sql
--rw-r--r--   0        0        0     1752 2023-05-29 07:15:14.297109 timor_locations-0.0.6/timor_locations/management/commands/timor_topology.py
--rw-r--r--   0        0        0      354 2023-05-29 06:55:35.209591 timor_locations-0.0.6/timor_locations/management/commands/topology_to_topojson.py
--rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.6/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
--rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.6/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
--rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.6/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
--rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.6/timor_locations/migrations/0005_topojson.py
--rw-r--r--   0        0        0      858 2023-05-29 07:19:27.523903 timor_locations-0.0.6/timor_locations/migrations/0006_timortopology_edgemap.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/migrations/__init__.py
--rw-r--r--   0        0        0     5209 2023-05-29 08:07:50.870268 timor_locations-0.0.6/timor_locations/models.py
--rw-r--r--   0        0        0     1610 2023-05-29 05:01:43.145478 timor_locations-0.0.6/timor_locations/router.py
--rw-r--r--   0        0        0      977 2023-05-29 05:00:30.661276 timor_locations-0.0.6/timor_locations/schemas.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/settings.py
--rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.6/timor_locations/urls.py
--rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.6/timor_locations/wsgi.py
--rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 timor_locations-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1190 2023-06-02 03:25:13.675411 timor_locations-0.0.7/README.md
+-rw-r--r--   0        0        0     1808 2023-06-02 03:21:14.708827 timor_locations-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.7/timor_locations/admin.py
+-rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.7/timor_locations/api.py
+-rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/gis_functions.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.7/timor_locations/management/commands/create_topology.py
+-rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data.py
+-rw-r--r--   0        0        0     3909 2023-06-02 03:10:57.153981 timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data_2022.py
+-rw-r--r--   0        0        0     2285 2023-05-29 00:25:54.388811 timor_locations-0.0.7/timor_locations/management/commands/suco_to_topology.sql
+-rw-r--r--   0        0        0     1752 2023-05-29 07:15:14.297109 timor_locations-0.0.7/timor_locations/management/commands/timor_topology.py
+-rw-r--r--   0        0        0      354 2023-05-29 06:55:35.209591 timor_locations-0.0.7/timor_locations/management/commands/topology_to_topojson.py
+-rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
+-rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
+-rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
+-rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.7/timor_locations/migrations/0005_topojson.py
+-rw-r--r--   0        0        0      858 2023-05-29 07:19:27.523903 timor_locations-0.0.7/timor_locations/migrations/0006_timortopology_edgemap.py
+-rw-r--r--   0        0        0     1252 2023-06-02 01:12:21.187814 timor_locations-0.0.7/timor_locations/migrations/0007_aldeia_delete_edgemap_delete_timortopology.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/migrations/__init__.py
+-rw-r--r--   0        0        0     5311 2023-06-02 00:07:51.970584 timor_locations-0.0.7/timor_locations/models.py
+-rw-r--r--   0        0        0     1610 2023-05-29 05:01:43.145478 timor_locations-0.0.7/timor_locations/router.py
+-rw-r--r--   0        0        0      977 2023-05-29 05:00:30.661276 timor_locations-0.0.7/timor_locations/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/settings.py
+-rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.7/timor_locations/urls.py
+-rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/wsgi.py
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 timor_locations-0.0.7/PKG-INFO
```

### Comparing `timor_locations-0.0.6/README.md` & `timor_locations-0.0.7/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Timor GIS
 
 Timor Leste GIS data as Django models
 This initial release uses administrative boundariew from Estrada, tweaked to include Atauro as a separate entity, with pcode which are intended to match existing data from PNDS.
 
+Data inputs are stored as `gpkg` files in Git LFS.
+
 ## Environment
 
 This is intended to be compatible with:
 
 - Django 4.1+
 - Python 3.10+
 
 ```sh
 gh repo clone catalpainternational/timor_locations
 cd timor_locations
 poetry install
 ```
 
+### Development
+
+ - When developing please install prerequisites with `poetry install --with dev --no-root`
+
 ### Pre Commit
 
 If `pre-commit` is installed your code will be checked before commit.
 This includes
 
 - black
 - flake8
```

### Comparing `timor_locations-0.0.6/pyproject.toml` & `timor_locations-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [tool.ruff]
 line-length = 119
 exclude = ['migrations']
 
 [tool.poetry]
 name = "timor-locations"
-version = "0.0.6"
+version = "0.0.7"
 description = "Timor-Leste geographic datasets"
 authors = [
   "Joshua Brooks <josh@catalpa.io>",
   "Anders Hofstee <anders@catalpa.io>",
 ]
 exclude = ["tests", "sl_tests", "timor_locations/data", "docs"]
 license = "GPLv3"
```

### Comparing `timor_locations-0.0.6/timor_locations/gis_functions.py` & `timor_locations-0.0.7/timor_locations/gis_functions.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/management/commands/create_topology.py` & `timor_locations-0.0.7/timor_locations/management/commands/create_topology.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/management/commands/import_timor_geo_data.py` & `timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/management/commands/suco_to_topology.sql` & `timor_locations-0.0.7/timor_locations/management/commands/suco_to_topology.sql`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/management/commands/timor_topology.py` & `timor_locations-0.0.7/timor_locations/management/commands/timor_topology.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0001_initial.py` & `timor_locations-0.0.7/timor_locations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py` & `timor_locations-0.0.7/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py` & `timor_locations-0.0.7/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py` & `timor_locations-0.0.7/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0005_topojson.py` & `timor_locations-0.0.7/timor_locations/migrations/0005_topojson.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/migrations/0006_timortopology_edgemap.py` & `timor_locations-0.0.7/timor_locations/migrations/0006_timortopology_edgemap.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/models.py` & `timor_locations-0.0.7/timor_locations/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,18 @@
     municipality = models.ForeignKey(Municipality, on_delete=models.PROTECT, null=True)
 
 
 class Suco(TimorGeoArea):
     adminpost = models.ForeignKey(AdministrativePost, on_delete=models.PROTECT, null=True)
 
 
+class Aldeia(TimorGeoArea):
+    suco = models.ForeignKey(Suco, on_delete=models.PROTECT, null=True)
+
+
 class TopoJson(models.Model):
     """
     Stores topology instances developed from other geo information
     """
 
     id = models.SlugField(primary_key=True, max_length=2048)
     name = models.CharField(null=True, blank=True, max_length=2048)
```

### Comparing `timor_locations-0.0.6/timor_locations/router.py` & `timor_locations-0.0.7/timor_locations/router.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/timor_locations/schemas.py` & `timor_locations-0.0.7/timor_locations/schemas.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.6/PKG-INFO` & `timor_locations-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timor-locations
-Version: 0.0.6
+Version: 0.0.7
 Summary: Timor-Leste geographic datasets
 Home-page: https://github.com/catalpainternational/timor_locations
 License: GPLv3
 Author: Joshua Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -18,27 +18,33 @@
 Description-Content-Type: text/markdown
 
 # Timor GIS
 
 Timor Leste GIS data as Django models
 This initial release uses administrative boundariew from Estrada, tweaked to include Atauro as a separate entity, with pcode which are intended to match existing data from PNDS.
 
+Data inputs are stored as `gpkg` files in Git LFS.
+
 ## Environment
 
 This is intended to be compatible with:
 
 - Django 4.1+
 - Python 3.10+
 
 ```sh
 gh repo clone catalpainternational/timor_locations
 cd timor_locations
 poetry install
 ```
 
+### Development
+
+ - When developing please install prerequisites with `poetry install --with dev --no-root`
+
 ### Pre Commit
 
 If `pre-commit` is installed your code will be checked before commit.
 This includes
 
 - black
 - flake8
```

