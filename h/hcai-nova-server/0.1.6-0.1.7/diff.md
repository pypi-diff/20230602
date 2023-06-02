# Comparing `tmp/hcai-nova-server-0.1.6.tar.gz` & `tmp/hcai-nova-server-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-0.1.6.tar", last modified: Thu May 25 09:58:36 2023, max compression
+gzip compressed data, was "hcai-nova-server-0.1.7.tar", last modified: Fri Jun  2 12:26:41 2023, max compression
```

## Comparing `hcai-nova-server-0.1.6.tar` & `hcai-nova-server-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.954375 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 09:58:36.000000 hcai-nova-server-0.1.6/hcai_nova_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 09:58:36.958375 hcai-nova-server-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-25 09:58:19.000000 hcai-nova-server-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.265701 hcai-nova-server-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-02 12:26:41.000000 hcai-nova-server-0.1.7/hcai_nova_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:41.261701 hcai-nova-server-0.1.7/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:26:41.265701 hcai-nova-server-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-02 12:26:26.000000 hcai-nova-server-0.1.7/setup.py
```

### Comparing `hcai-nova-server-0.1.6/PKG-INFO` & `hcai-nova-server-0.1.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.6
+Version: 0.1.7
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.6/hcai_nova_server.egg-info/PKG-INFO` & `hcai-nova-server-0.1.7/hcai_nova_server.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.6
+Version: 0.1.7
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.6/hcai_nova_server.egg-info/SOURCES.txt` & `hcai-nova-server-0.1.7/hcai_nova_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/app.py` & `hcai-nova-server-0.1.7/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/cancel.py` & `hcai-nova-server-0.1.7/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/explain.py` & `hcai-nova-server-0.1.7/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/extract.py` & `hcai-nova-server-0.1.7/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/log.py` & `hcai-nova-server-0.1.7/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/predict.py` & `hcai-nova-server-0.1.7/nova_server/route/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,20 +132,23 @@
 
         logger.info("Saving predictions to database...")
 
         # TODO: Refactor to not use request form in upload
         request_form_copy = copy.copy(request_form)
         assert len(ss_ds_iter.sessions) == 1
         request_form_copy['sessions'] = ss_ds_iter.sessions[0]
-        db_utils.write_annotation_to_db(request_form_copy, annos, logger)
+
+        for anno in annos:
+            db_utils.write_annotation_to_db(request_form_copy, anno, logger)
         logger.info("...done")
 
     logger.info("Prediction completed!")
     status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
+'''Keep for later reference to implement polygons'''
     # model_script.ds_iter = ds_iter
     # model_script.request_form["sessions"] = session
     # model_script.request_form["roles"] = role
     #
     # logger.info("Execute preprocessing.")
     # model_script.preprocess()
     # logger.info("Preprocessing done.")
```

### Comparing `hcai-nova-server-0.1.6/nova_server/route/status.py` & `hcai-nova-server-0.1.7/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/route/train.py` & `hcai-nova-server-0.1.7/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/dataset_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/dataset_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "ip": request_form["server"].split(":")[0],
         "port": int(request_form["server"].split(":")[1]),
         "user": request_form["username"],
         "password": request_form["password"],
     }
 
     flattenSamples = False
-    if request_form["flattenSamples"] == "true":
+    if request_form.get("flattenSamples") == "true":
         flattenSamples = True
 
     ds_iter = HcaiNovaDynamicIterable(
         # Database Config
         db_config_path=None,  # os.path.join(os.path.dirname(os.path.abspath(__file__)), 'db.cfg'),
         db_config_dict=db_config_dict,
         # Dataset Config
```

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/explain_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/import_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/key_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/log_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/status_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/nova_server/utils/thread_utils.py` & `hcai-nova-server-0.1.7/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.6/setup.py` & `hcai-nova-server-0.1.7/setup.py`

 * *Files identical despite different names*

