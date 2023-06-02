# Comparing `tmp/road_data_scraper-0.0.6.tar.gz` & `tmp/road_data_scraper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "road_data_scraper-0.0.6.tar", last modified: Sun Dec 26 13:33:23 2021, max compression
+gzip compressed data, was "road_data_scraper-0.0.8.tar", last modified: Tue Dec 28 16:44:31 2021, max compression
```

## Comparing `road_data_scraper-0.0.6.tar` & `road_data_scraper-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      914 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.949634 road_data_scraper-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.949634 road_data_scraper-0.0.6/src/road_data_scraper/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/src/road_data_scraper/report/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/report/report.py
--rw-r--r--   0 runner    (1001) docker     (121)     6534 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/report/road_data_report_template.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/src/road_data_scraper/steps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/steps/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/steps/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-12-26 13:33:11.000000 road_data_scraper-0.0.6/src/road_data_scraper/steps/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-26 13:33:23.953635 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      688 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-26 13:33:23.000000 road_data_scraper-0.0.6/src/road_data_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4338 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      914 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/src/road_data_scraper/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4177 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/main.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/src/road_data_scraper/report/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6534 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/report/road_data_report_template.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/src/road_data_scraper/steps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/steps/download.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2510 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/steps/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4769 2021-12-28 16:44:21.000000 road_data_scraper-0.0.8/src/road_data_scraper/steps/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 16:44:31.119566 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-28 16:44:31.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2021-12-28 16:44:31.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 16:44:31.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 16:44:30.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-12-28 16:44:31.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-28 16:44:31.000000 road_data_scraper-0.0.8/src/road_data_scraper.egg-info/top_level.txt
```

### Comparing `road_data_scraper-0.0.6/LICENSE` & `road_data_scraper-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/PKG-INFO` & `road_data_scraper-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: road_data_scraper
-Version: 0.0.6
+Version: 0.0.8
 Summary: Scrapes and Cleans WebTRIS Traffic Flow API
 Home-page: UNKNOWN
 Author: Dominic Bean
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `road_data_scraper-0.0.6/README.md` & `road_data_scraper-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/setup.cfg` & `road_data_scraper-0.0.8/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = road_data_scraper
-version = 0.0.6
+version = 0.0.8
 description = Scrapes and Cleans WebTRIS Traffic Flow API
 author = Dominic Bean
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/main.py` & `road_data_scraper-0.0.8/src/road_data_scraper/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,43 +23,53 @@
     format="%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s",
     level=logging.INFO,
     datefmt="%Y-%m-%d %H:%M:%S",
     handlers=[RichHandler()],
 )
 
 
-def run(config):
+def run(config, api_run):
+
+    if api_run:
+
+        def my_ast(*args):
+            return args[0]
+
+    else:
+
+        def my_ast(*args):
+            return ast.literal_eval(*args)
 
     start_time = time.time()
 
     logging.info(f"Using {THREAD_POOL} threads")
 
     data_path, metadata_path, report_path, run_id_path = file_handler(config)
 
     logging.getLogger().addHandler(
         logging.FileHandler(f"{metadata_path}/road_data_pipeline.log")
     )
 
-    start_date = ast.literal_eval(config["user_settings"]["start_date"])
-    end_date = ast.literal_eval(config["user_settings"]["end_date"])
+    start_date = my_ast(config["user_settings"]["start_date"])
+    end_date = my_ast(config["user_settings"]["end_date"])
 
     if not start_date and not end_date:
 
         # 2-month API data lag (date today minus two months)
         date_object_today = datetime.strptime(time.strftime("%Y-%m"), "%Y-%m")
         minus_two_months = date_object_today - relativedelta(months=2)
 
         year, month = map(int, minus_two_months.strftime("%Y %m").split())
         last_day_of_month = calendar.monthrange(year, month)[1]
 
         start_date = f"{year}-{month}-01"
         end_date = f"{year}-{month}-{last_day_of_month}"
 
-    test_run = ast.literal_eval(config["user_settings"]["test_run"])
-    generate_report = ast.literal_eval(config["user_settings"]["generate_report"])
+    test_run = my_ast(config["user_settings"]["test_run"])
+    generate_report = my_ast(config["user_settings"]["generate_report"])
 
     logging.info("Getting Road Sensor Lookup Table")
 
     sensor_tables, lookup_df = get_sites_by_sensor()
     lookup_df.to_csv(f"{str(metadata_path)}/road_data_sensor_lookup.csv", index=False)
 
     midas_metadata, tmu_metadata, tame_metadata = get_site_urls(
@@ -100,29 +110,32 @@
         test_run=test_run,
         run_id_path=data_path,
     )
 
     if generate_report:
         run_reports(lookup_df, report_path, start_date, end_date)
 
-    dump_config(config, metadata_path)
+    if api_run:
+        dump_config(config, metadata_path, api_run=True)
+    else:
+        dump_config(config, metadata_path, api_run=False)
 
-    gcp_storage = ast.literal_eval(config["user_settings"]["gcp_storage"])
+    gcp_storage = my_ast(config["user_settings"]["gcp_storage"])
 
     if gcp_storage:
 
-        gcp_bucket_name = ast.literal_eval(config["user_settings"]["gcp_bucket_name"])
-        gcp_folder_name = ast.literal_eval(config["user_settings"]["gcp_blob_name"])
-        gcp_credentials = ast.literal_eval(config["user_settings"]["gcp_credentials"])
+        gcp_bucket_name = my_ast(config["user_settings"]["gcp_bucket_name"])
+        gcp_folder_name = my_ast(config["user_settings"]["gcp_blob_name"])
+        gcp_credentials = my_ast(config["user_settings"]["gcp_credentials"])
 
         gcp_upload_from_directory(
             run_id_path, gcp_bucket_name, gcp_folder_name, gcp_credentials
         )
 
-    rm_dir = ast.literal_eval(config["user_settings"]["rm_dir"])
+    rm_dir = my_ast(config["user_settings"]["rm_dir"])
 
     if rm_dir:
         logging.info(
             f"Removing {run_id_path[run_id_path.find('output_data/'):].split('/')[1]} folder."
         )
         shutil.rmtree(Path(run_id_path))
```

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/report/report.py` & `road_data_scraper-0.0.8/src/road_data_scraper/report/report.py`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/report/road_data_report_template.ipynb` & `road_data_scraper-0.0.8/src/road_data_scraper/report/road_data_report_template.ipynb`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/steps/download.py` & `road_data_scraper-0.0.8/src/road_data_scraper/steps/download.py`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/steps/file_handler.py` & `road_data_scraper-0.0.8/src/road_data_scraper/steps/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,21 +34,24 @@
 
     logging.info(f"Making Report Directory at: {report_path}")
     report_path.mkdir(parents=True, exist_ok=True)
 
     return data_path, metadata_path, report_path, run_id_path
 
 
-def dump_config(config, full_path):
+def dump_config(config, full_path, api_run):
 
     logging.info(f"Dumping config.ini for Run at {full_path}")
 
-    config_dict = {
-        section: dict(config.items(section)) for section in config.sections()
-    }
+    if api_run:
+        config_dict = config
+    else:
+        config_dict = {
+            section: dict(config.items(section)) for section in config.sections()
+        }
 
     with open(f"{str(full_path)}/config_metadata.txt", "w") as file:
         print(config_dict, file=file)
 
 
 def gcp_upload_from_directory(
     directory_path: str,
```

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper/steps/metadata.py` & `road_data_scraper-0.0.8/src/road_data_scraper/steps/metadata.py`

 * *Files identical despite different names*

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper.egg-info/PKG-INFO` & `road_data_scraper-0.0.8/src/road_data_scraper.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: road-data-scraper
-Version: 0.0.6
+Version: 0.0.8
 Summary: Scrapes and Cleans WebTRIS Traffic Flow API
 Home-page: UNKNOWN
 Author: Dominic Bean
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `road_data_scraper-0.0.6/src/road_data_scraper.egg-info/SOURCES.txt` & `road_data_scraper-0.0.8/src/road_data_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

