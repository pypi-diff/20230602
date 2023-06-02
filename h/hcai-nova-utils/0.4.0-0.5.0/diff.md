# Comparing `tmp/hcai-nova-utils-0.4.0.tar.gz` & `tmp/hcai-nova-utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-0.4.0.tar", last modified: Mon May 22 14:54:42 2023, max compression
+gzip compressed data, was "hcai-nova-utils-0.5.0.tar", last modified: Fri Jun  2 12:31:02 2023, max compression
```

## Comparing `hcai-nova-utils-0.4.0.tar` & `hcai-nova-utils-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/db_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/db_utils/nova_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-02 12:31:02.000000 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-06-02 12:31:02.000000 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:31:02.000000 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-06-02 12:31:02.000000 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-02 12:31:02.000000 hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/nova_utils/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/db_utils/nova_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/interfaces/dataset_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6302 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7930 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:31:02.145174 hcai-nova-utils-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-06-02 12:30:50.000000 hcai-nova-utils-0.5.0/setup.py
```

### Comparing `hcai-nova-utils-0.4.0/PKG-INFO` & `hcai-nova-utils-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-0.5.0/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/nova_utils/db_utils/nova_types.py` & `hcai-nova-utils-0.5.0/nova_utils/db_utils/nova_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/nova_utils/interfaces/dataset_iterable.py` & `hcai-nova-utils-0.5.0/nova_utils/interfaces/dataset_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-0.5.0/nova_utils/interfaces/server_module.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
-from nova_utils.interfaces.dataset_iterable import DatasetIterable
-from nova_utils.db_utils.nova_types import DataTypes
-import numpy as np
+
+from nova_utils.ssi_utils.ssi_anno_utils import Anno
+
 
 REQUIREMENTS = []
 
 '''
 class Dataset(DatasetIterable):
     def __int__(self, *args, data: dict, **kwargs):
         super().__init__(*args, **kwargs)
@@ -42,15 +42,15 @@
         self.data = None
         self.output = None
         self.options = {}
 
         if self.request_form is not None:
             # Set Options
             logger.info("Setting options...")
-            if not request_form["optStr"] == "":
+            if request_form.get("optStr"):
                 for k, v in dict(
                         option.split("=") for option in request_form["optStr"].split(";")
                 ).items():
                     if v in ("True", "False"):
                         self.options[k] = True if v == "True" else False
                     elif v == "None":
                         self.options[k] = True if v == "True" else False
@@ -124,59 +124,23 @@
     Base class of a data predictor. Implement this interface if you want to write annotations to a database
     """
 
     def __init__(self, logger, request_form=None):
         super().__init__(logger, request_form)
 
     @abstractmethod
-    def to_anno(self, data):
+    def to_anno(self, data) -> list[Anno]:
         """Converts the output of process_data to the correct annotation format to upload them to the database.
         !THE OUTPUT FORMAT OF THIS FUNCTION IS NOT YET FULLY DEFINED AND WILL CHANGE IN FUTURE RELEASES!
 
         Args:
             data (object): Data output of process_data function
 
         Returns:
-            dict: A dictionary containing the predictions of the model in the correct annotation format.
-
-
-        Example:
-
-            Discrete annotation:
-                ::
-
-                    {
-                        '0.0_1.0' : {
-                            'speaker_1.audio' : {'id': '1', 'conf': 0.73}
-                            'speaker_2.audio' : {'id': '0', conf: 1.0}
-                        }
-                        ...
-                        'values': [],
-                        'confidences': []
-                    }
-
-            Continuous annotation:
-                ...
-            Free annotation:
-                ::
-
-                    {
-                        '0.0_1.0' : {
-                            'speaker_1.audio' : {'name': 'Hello', 'conf': 0.73}
-                            'speaker_2.audio' : {'name': '', conf: 1.0}
-                        }
-                        '1.0_2.0' : {
-                            'speaker_1.audio' : {'name': 'My Name', 'conf': 0.85}}
-                            'speaker_2.audio' : {'name': '', conf: 1.0}
-                        }
-                        ...
-                        'values': [],
-                        'confidences': []
-                    }
-
+            list: A list of annotation objects
         """
         raise NotImplemented
 
 
 class Extractor(Processor):
     """
     Base class of a feature extractor. Implement this interface in your own class to build a feature extractor.
@@ -204,12 +168,12 @@
         Each tuple has the form ( type (nova_types.DataTypes), sample_rate (double), data_chunk (numpy.ndarray) ). The shape of the data chunk should in the form of (n_frames, n_features)
         An arbitrary number of streams maybe returned.
 
         Example:
             ::
 
                 {
-                    'speaker_1.audio.mfcc[10ms,10ms,10ms]' : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] ),
-                    'speaker_2.audio.mfcc[10ms,10ms,10ms]' : ( DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] )
+                    'speaker_1.audio.mfcc[10ms,10ms,10ms]' : ( nova_utils.db_utils.nova_types.DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] ),
+                    'speaker_2.audio.mfcc[10ms,10ms,10ms]' : ( nova_utils.db_utils.nova_types.DataTypes.AUDIO, 100, [[0.0, 0.0, ... 0.0], [0.0, 0.0, ... 0.0] ... [0.0, 0.0, ... 0.0]] )
                 }
         """
         raise NotImplemented
```

### Comparing `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_data_types.py` & `hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_sample_list_utils.py` & `hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_sample_list_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import xml.etree.ElementTree as ET
 import numpy as np
 from nova_utils.ssi_utils.ssi_data_types import FileTypes, string_to_enum
 from nova_utils.ssi_utils.ssi_stream_utils import Stream
-from ssi_anno_utils import Scheme
 import os
 
 class Sample:
     def __init__(self, streams = [], user_id = None, class_id = None, score = 0):
         self.streams = streams
         self.user_id = user_id
         self.class_id = class_id
```

### Comparing `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_stream_utils.py` & `hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_xml_utils.py` & `hcai-nova-utils-0.5.0/nova_utils/ssi_utils/ssi_xml_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.4.0/setup.py` & `hcai-nova-utils-0.5.0/setup.py`

 * *Files identical despite different names*

