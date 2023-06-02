# Comparing `tmp/timor_locations-0.0.7.tar.gz` & `tmp/timor_locations-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timor_locations-0.0.7.tar", max compression
+gzip compressed data, was "timor_locations-0.0.8.tar", max compression
```

## Comparing `timor_locations-0.0.7.tar` & `timor_locations-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1190 2023-06-02 03:25:13.675411 timor_locations-0.0.7/README.md
--rw-r--r--   0        0        0     1808 2023-06-02 03:21:14.708827 timor_locations-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/__init__.py
--rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.7/timor_locations/admin.py
--rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.7/timor_locations/api.py
--rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/gis_functions.py
--rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/management/commands/__init__.py
--rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.7/timor_locations/management/commands/create_topology.py
--rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data.py
--rw-r--r--   0        0        0     3909 2023-06-02 03:10:57.153981 timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data_2022.py
--rw-r--r--   0        0        0     2285 2023-05-29 00:25:54.388811 timor_locations-0.0.7/timor_locations/management/commands/suco_to_topology.sql
--rw-r--r--   0        0        0     1752 2023-05-29 07:15:14.297109 timor_locations-0.0.7/timor_locations/management/commands/timor_topology.py
--rw-r--r--   0        0        0      354 2023-05-29 06:55:35.209591 timor_locations-0.0.7/timor_locations/management/commands/topology_to_topojson.py
--rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
--rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
--rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.7/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
--rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.7/timor_locations/migrations/0005_topojson.py
--rw-r--r--   0        0        0      858 2023-05-29 07:19:27.523903 timor_locations-0.0.7/timor_locations/migrations/0006_timortopology_edgemap.py
--rw-r--r--   0        0        0     1252 2023-06-02 01:12:21.187814 timor_locations-0.0.7/timor_locations/migrations/0007_aldeia_delete_edgemap_delete_timortopology.py
--rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/migrations/__init__.py
--rw-r--r--   0        0        0     5311 2023-06-02 00:07:51.970584 timor_locations-0.0.7/timor_locations/models.py
--rw-r--r--   0        0        0     1610 2023-05-29 05:01:43.145478 timor_locations-0.0.7/timor_locations/router.py
--rw-r--r--   0        0        0      977 2023-05-29 05:00:30.661276 timor_locations-0.0.7/timor_locations/schemas.py
--rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.7/timor_locations/settings.py
--rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.7/timor_locations/urls.py
--rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.7/timor_locations/wsgi.py
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 timor_locations-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1190 2023-06-02 03:25:13.675411 timor_locations-0.0.8/README.md
+-rw-r--r--   0        0        0     1808 2023-06-02 03:59:02.677634 timor_locations-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.8/timor_locations/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.8/timor_locations/admin.py
+-rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.8/timor_locations/api.py
+-rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.8/timor_locations/gis_functions.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.8/timor_locations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.8/timor_locations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1458 2023-06-02 03:31:43.296718 timor_locations-0.0.8/timor_locations/management/commands/create_topology.py
+-rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.8/timor_locations/management/commands/import_timor_geo_data.py
+-rw-r--r--   0        0        0     3966 2023-06-02 03:31:43.312715 timor_locations-0.0.8/timor_locations/management/commands/import_timor_geo_data_2022.py
+-rw-r--r--   0        0        0     2285 2023-05-29 00:25:54.388811 timor_locations-0.0.8/timor_locations/management/commands/suco_to_topology.sql
+-rw-r--r--   0        0        0     1810 2023-06-02 03:31:43.296718 timor_locations-0.0.8/timor_locations/management/commands/timor_topology.py
+-rw-r--r--   0        0        0      356 2023-06-02 03:31:43.272722 timor_locations-0.0.8/timor_locations/management/commands/topology_to_topojson.py
+-rw-r--r--   0        0        0     3014 2023-06-02 03:30:49.915010 timor_locations-0.0.8/timor_locations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.8/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
+-rw-r--r--   0        0        0     1401 2023-06-02 03:30:49.919009 timor_locations-0.0.8/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
+-rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.8/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
+-rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.8/timor_locations/migrations/0005_topojson.py
+-rw-r--r--   0        0        0      858 2023-05-29 07:19:27.523903 timor_locations-0.0.8/timor_locations/migrations/0006_timortopology_edgemap.py
+-rw-r--r--   0        0        0     1252 2023-06-02 03:30:49.911011 timor_locations-0.0.8/timor_locations/migrations/0007_aldeia_delete_edgemap_delete_timortopology.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.8/timor_locations/migrations/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-02 03:31:43.356707 timor_locations-0.0.8/timor_locations/models.py
+-rw-r--r--   0        0        0     1610 2023-05-29 05:01:43.145478 timor_locations-0.0.8/timor_locations/router.py
+-rw-r--r--   0        0        0      977 2023-05-29 05:00:30.661276 timor_locations-0.0.8/timor_locations/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:14:46.583565 timor_locations-0.0.8/timor_locations/settings.py
+-rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.8/timor_locations/urls.py
+-rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.8/timor_locations/wsgi.py
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 timor_locations-0.0.8/PKG-INFO
```

### Comparing `timor_locations-0.0.7/README.md` & `timor_locations-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/pyproject.toml` & `timor_locations-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [tool.ruff]
 line-length = 119
 exclude = ['migrations']
 
 [tool.poetry]
 name = "timor-locations"
-version = "0.0.7"
+version = "0.0.8"
 description = "Timor-Leste geographic datasets"
 authors = [
   "Joshua Brooks <josh@catalpa.io>",
   "Anders Hofstee <anders@catalpa.io>",
 ]
 exclude = ["tests", "sl_tests", "timor_locations/data", "docs"]
 license = "GPLv3"
```

### Comparing `timor_locations-0.0.7/timor_locations/gis_functions.py` & `timor_locations-0.0.8/timor_locations/gis_functions.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data.py` & `timor_locations-0.0.8/timor_locations/management/commands/import_timor_geo_data.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/management/commands/import_timor_geo_data_2022.py` & `timor_locations-0.0.8/timor_locations/management/commands/import_timor_geo_data_2022.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from importlib import resources
 
 from django.contrib.gis.gdal import DataSource
 from django.contrib.gis.utils import LayerMapping
 from django.core.management.base import BaseCommand
 from django.db import connection
 
-from timor_locations.models import Aldeia, AdministrativePost, Municipality, Suco
+from timor_locations.models import AdministrativePost, Aldeia, Municipality, Suco
 
 aldeia_mapping = {"geom": "MULTIPOLYGON", "name": "ALDEIA", "pcode": "NewAldCode"}
 SOURCE_GEO = resources.files("timor_locations.data").joinpath("aldeias_2022.gpkg")
 
 
 class Command(BaseCommand):
     help = "Import Timor data from source shapefiles."
@@ -31,60 +31,62 @@
         self.stdout.write(self.style.SUCCESS("Saving aldeias from the gpkg file"))
         # lm.save()
 
         self.stdout.write(self.style.SUCCESS("Adding admin posts and municipalities"))
 
         layer = ds[0]
         # Fetch the ID & name of aldeia suco, pa, mun
-        names = zip(*(layer.get_fields(f) for f in ("NewAldCode", "NewSucoCod", "NewPostAdC", "NewMunCode", "ALDEIA", "SUCO", "P_ADMIN", "MUNICIPIO")))
+        names = zip(
+            *(
+                layer.get_fields(f)
+                for f in (
+                    "NewAldCode",
+                    "NewSucoCod",
+                    "NewPostAdC",
+                    "NewMunCode",
+                    "ALDEIA",
+                    "SUCO",
+                    "P_ADMIN",
+                    "MUNICIPIO",
+                )
+            )
+        )
 
         ids: set[int] = set()
 
         for NewAldCode, NewSucoCod, NewPostAdC, NewMunCode, ALDEIA, SUCO, P_ADMIN, MUNICIPIO in names:
-            
             print(NewAldCode, NewSucoCod, NewPostAdC, NewMunCode, ALDEIA, SUCO, P_ADMIN, MUNICIPIO)
 
-
             if NewMunCode not in ids:
-                municipality,_ = Municipality.objects.get_or_create(
-                    pcode=NewMunCode,
-                    name=MUNICIPIO
-                )
+                municipality, _ = Municipality.objects.get_or_create(pcode=NewMunCode, name=MUNICIPIO)
                 ids.add(NewMunCode)
                 self.stdout.write(self.style.SUCCESS(f"ADDED {municipality}"))
 
             if NewPostAdC not in ids:
-                adminpost,_ = AdministrativePost.objects.get_or_create(
-                    pcode=NewPostAdC,
-                    name=P_ADMIN,
-                    municipality_id=NewMunCode
+                adminpost, _ = AdministrativePost.objects.get_or_create(
+                    pcode=NewPostAdC, name=P_ADMIN, municipality_id=NewMunCode
                 )
                 ids.add(NewPostAdC)
                 self.stdout.write(self.style.SUCCESS(f"ADDED {adminpost}"))
 
             if NewSucoCod not in ids:
-                suco,_ = Suco.objects.get_or_create(
-                    pcode=NewSucoCod,
-                    name=SUCO,
-                    adminpost_id = NewPostAdC
-                )
+                suco, _ = Suco.objects.get_or_create(pcode=NewSucoCod, name=SUCO, adminpost_id=NewPostAdC)
                 ids.add(NewSucoCod)
                 self.stdout.write(self.style.SUCCESS(f"ADDED {suco}"))
 
-            aldeia = Aldeia.objects.get(
-                pcode=NewAldCode
-            )
+            aldeia = Aldeia.objects.get(pcode=NewAldCode)
             aldeia.suco_id = NewSucoCod
             aldeia.save()
             ids.add(NewAldCode)
             self.stdout.write(self.style.SUCCESS(f"ADDED {aldeia}"))
 
-
         self.stdout.write(
-            self.style.SUCCESS("Populate the suco / admin post / municipality geometries based on the Aldeia geometries")
+            self.style.SUCCESS(
+                "Populate the suco / admin post / municipality geometries based on the Aldeia geometries"
+            )
         )
         with connection.cursor() as c:
             c.execute(
                 """
                 UPDATE timor_locations_suco sc
                     SET geom = (SELECT st_multi(st_union(geom)) FROM timor_locations_aldeia a WHERE a.suco_id = sc.pcode);
                 UPDATE timor_locations_administrativepost ap
```

### Comparing `timor_locations-0.0.7/timor_locations/management/commands/suco_to_topology.sql` & `timor_locations-0.0.8/timor_locations/management/commands/suco_to_topology.sql`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/management/commands/timor_topology.py` & `timor_locations-0.0.8/timor_locations/management/commands/timor_topology.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-
 from django.core.management.base import BaseCommand
 from django.db import connection
+
 from timor_locations import models
 
 
 class Command(BaseCommand):
     help = "Commands necessary to build timor 'topology' layer in postgis"
 
-
     def handle(self, *args, **options):
-
         topology_schema_name = "topo"
 
         precision = 1e-6
         tolerance = 0
-        srid=4326
+        srid = 4326
 
         # Which table name and column name to use for the "topo" references
         schema_name = "public"
         table_name = models.TimorTopology._meta.db_table
         column_name = "topo"
-        geomtype="POLYGON"
+        geomtype = "POLYGON"
 
         self.stdout.write(self.style.SUCCESS("Creating topology"))
         with connection.cursor() as c:
             c.execute(f"SELECT topology.DropTopology('{topology_schema_name}')")
             c.execute(f"SELECT topology.CreateTopology('{topology_schema_name}', {srid}, {precision});")
             # Add topology from the 'suco' table
             c.execute(f"DROP TABLE IF EXISTS {schema_name}.{table_name}")
             c.execute(f"CREATE TABLE {schema_name}.{table_name} (pcode int PRIMARY KEY)")
-            c.execute(f"SELECT topology.AddTopoGeometryColumn('{topology_schema_name}', '{schema_name}', '{table_name}', '{column_name}', '{geomtype}');")
-            
+            c.execute(
+                f"SELECT topology.AddTopoGeometryColumn('{topology_schema_name}', '{schema_name}', '{table_name}', '{column_name}', '{geomtype}');"
+            )
+
             for model in models.Municipality, models.AdministrativePost, models.Suco:
                 self.stdout.write(self.style.SUCCESS(f"import {model.objects.count()} geoms from {model}"))
 
-                c.execute(f"""
+                c.execute(
+                    f"""
                     INSERT INTO {schema_name}.{table_name} (pcode, {column_name})
                     SELECT  pcode, topology.toTopoGeom(geom, '{topology_schema_name}', 1, {tolerance})
                     FROM {model._meta.db_table}
-                    """)
+                    """
+                )
```

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0001_initial.py` & `timor_locations-0.0.8/timor_locations/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 4.2.1 on 2023-05-24 07:32
 
 import django.contrib.gis.db.models.fields
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = []
```

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py` & `timor_locations-0.0.8/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py` & `timor_locations-0.0.8/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 4.2.1 on 2023-05-24 13:34
 
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
         ("timor_locations", "0002_remove_administrativepost_id_remove_municipality_id_and_more"),
     ]
```

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py` & `timor_locations-0.0.8/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0005_topojson.py` & `timor_locations-0.0.8/timor_locations/migrations/0005_topojson.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0006_timortopology_edgemap.py` & `timor_locations-0.0.8/timor_locations/migrations/0006_timortopology_edgemap.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/migrations/0007_aldeia_delete_edgemap_delete_timortopology.py` & `timor_locations-0.0.8/timor_locations/migrations/0007_aldeia_delete_edgemap_delete_timortopology.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by Django 4.2.1 on 2023-06-02 01:12
 
 import django.contrib.gis.db.models.fields
-from django.db import migrations, models
 import django.db.models.deletion
+from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('timor_locations', '0006_timortopology_edgemap'),
     ]
```

### Comparing `timor_locations-0.0.7/timor_locations/models.py` & `timor_locations-0.0.8/timor_locations/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,23 +77,21 @@
         to fetch the GeoJSON.
         """
         if not hasattr(self, "geojson"):
             return MultiPolygon.construct(**json.loads(self.geom.json))
         return MultiPolygon.construct(**json.loads(self.geojson))
 
     def as_feature(self):
-        properties = dict(name = self.name, id=self.pcode, kind=self._meta.model_name)
+        properties = dict(name=self.name, id=self.pcode, kind=self._meta.model_name)
 
         for optional in ("adminpost_id", "municipality_id", "adminpost_name", "municipality_name"):
             if hasattr(self, optional):
                 properties[optional] = getattr(self, optional)
-            
-        return Feature.construct(
-            type="Feature", id=self.pcode, properties=properties, geometry=self.as_multipolygon()
-        )
+
+        return Feature.construct(type="Feature", id=self.pcode, properties=properties, geometry=self.as_multipolygon())
 
     @classmethod
     def all_features(cls, **kwargs) -> FeatureCollection:
         """
         Returns a FeatureCollection with **ALL** features from Municipality, Admin Post, and Suco
         """
         return FeatureCollection.construct(
@@ -104,14 +102,15 @@
                 *Suco.objects.as_feature_list(**kwargs),
             ],
         )
 
     @classmethod
     def topology(cls):
         import topojson
+
         return topojson.Topology(cls.all_features().json())
 
 
 class Municipality(TimorGeoArea):
     pass
```

### Comparing `timor_locations-0.0.7/timor_locations/router.py` & `timor_locations-0.0.8/timor_locations/router.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/timor_locations/schemas.py` & `timor_locations-0.0.8/timor_locations/schemas.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.7/PKG-INFO` & `timor_locations-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timor-locations
-Version: 0.0.7
+Version: 0.0.8
 Summary: Timor-Leste geographic datasets
 Home-page: https://github.com/catalpainternational/timor_locations
 License: GPLv3
 Author: Joshua Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

