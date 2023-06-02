# Comparing `tmp/hcai-nova-server-nightly-0.1.8.dev202306021227.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.8.dev202306021506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.8.dev202306021227.tar", last modified: Fri Jun  2 12:27:50 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.8.dev202306021506.tar", last modified: Fri Jun  2 15:06:51 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227.tar` & `hcai-nova-server-nightly-0.1.8.dev202306021506.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.559885 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-02 12:27:50.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:27:50.563886 hcai-nova-server-nightly-0.1.8.dev202306021227/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-02 12:27:40.000000 hcai-nova-server-nightly-0.1.8.dev202306021227/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.378062 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-02 15:06:51.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3258 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9988 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7220 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:51.382062 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7846 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 15:06:51.386062 hcai-nova-server-nightly-0.1.8.dev202306021506/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-06-02 15:06:39.000000 hcai-nova-server-nightly-0.1.8.dev202306021506/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/PKG-INFO` & `hcai-nova-server-nightly-0.1.8.dev202306021506/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.8.dev202306021227
+Version: 0.1.8.dev202306021506
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.8.dev202306021227
+Version: 0.1.8.dev202306021506
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.8.dev202306021506/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from importlib.machinery import SourceFileLoader
 from hcai_datasets.hcai_nova_dynamic.hcai_nova_dynamic_iterable import (
     HcaiNovaDynamicIterable,
 )
 import ffmpegio
 import numpy as np
 from nova_server.utils import db_utils
-
-
+from flask import current_app
+import os
 extract = Blueprint("extract", __name__)
 
 
 @extract.route("/extract", methods=["POST"])
 def extract_thread():
     if request.method == "POST":
         request_form = request.form.to_dict()
@@ -41,18 +41,21 @@
         return jsonify(data)
 
 
 @thread_utils.ml_thread_wrapper
 def extract_data(request_form, app_context):
 
     # Initialize
+    #cml_dir = app_context.config["CML_DIR"]
+    #data_dir = app_context.config["DATA_DIR"]
+    cml_dir = os.environ["NOVA_CML_DIR"]
+    data_dir = os.environ["NOVA_DATA_DIR"]
+
     key = get_key_from_request_form(request_form)
     logger = log_utils.get_logger_for_thread(key)
-    cml_dir = app_context.config["CML_DIR"]
-    data_dir = app_context.config["DATA_DIR"]
 
     chain_file_path = Path(cml_dir).joinpath(
         PureWindowsPath(request_form["chainFilePath"])
     )
 
     log_conform_request = dict(request_form)
     log_conform_request["password"] = "---"
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This file contains the general logic for predicting annotations to the nova database"""
 import copy
+import os
 from pathlib import Path, PureWindowsPath
 from nova_server.utils import db_utils
 from flask import Blueprint, request, jsonify
 from nova_utils.ssi_utils.ssi_xml_utils import Trainer
 from importlib.machinery import SourceFileLoader
 from nova_server.utils.thread_utils import THREADS
 from nova_server.utils.status_utils import update_progress
@@ -37,16 +38,18 @@
         return jsonify(data)
 
 
 @thread_utils.ml_thread_wrapper
 def predict_data(request_form, app_context):
     key = get_key_from_request_form(request_form)
     logger = log_utils.get_logger_for_thread(key)
-    cml_dir = app_context.config["CML_DIR"]
-    data_dir = app_context.config["DATA_DIR"]
+    #cml_dir = app_context.config["CML_DIR"]
+    #data_dir = app_context.config["DATA_DIR"]
+    cml_dir = os.environ["NOVA_CML_DIR"]
+    data_dir = os.environ["NOVA_DATA_DIR"]
 
     log_conform_request = dict(request_form)
     log_conform_request["password"] = "---"
 
     logger.info("Action 'Predict' started.")
     status_utils.update_status(key, status_utils.JobStatus.RUNNING)
     trainer_file_path = Path(cml_dir).joinpath(
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/log_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import logging
 import threading
-import pathlib
+from pathlib import Path
+import os
 from nova_server.utils import status_utils
-
+from flask import current_app
 
 LOGS = {}
 
 
 def get_logfile_name_for_thread(log_key):
     return log_key + "-job_" + threading.current_thread().name
 
 
 def get_log_path_for_thread(log_key):
     name = get_logfile_name_for_thread(log_key)
-    # TODO: add  dynamic log path from config
-    return pathlib.Path(__file__).parent.parent / "logs" / (name + ".log")
+    log_dir = os.environ["NOVA_CML_DIR"]
+    return Path(log_dir) / (name + ".log")
 
 
 def init_logger(logger, log_key):
     print("Init logger" + str(threading.current_thread().name))
     try:
         log_path = get_log_path_for_thread(log_key)
         status_utils.set_log_path(log_key, log_path)
```

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.8.dev202306021227/setup.py` & `hcai-nova-server-nightly-0.1.8.dev202306021506/setup.py`

 * *Files identical despite different names*

