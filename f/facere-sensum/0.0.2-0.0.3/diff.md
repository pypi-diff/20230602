# Comparing `tmp/facere_sensum-0.0.2.tar.gz` & `tmp/facere_sensum-0.0.3.tar.gz`

## Comparing `facere_sensum-0.0.2.tar` & `facere_sensum-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/log.csv
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/requirements.txt
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.github/workflows/lints.yaml
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/facere_sensum.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/src/facere_sensum/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/ref.csv
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/test/test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/LICENSE
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/README.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 facere_sensum-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/log.csv
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/requirements.txt
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.github/workflows/lints.yaml
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/src/facere_sensum/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/src/facere_sensum/facere_sensum.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/ref.csv
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/test/test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 facere_sensum-0.0.3/PKG-INFO
```

### Comparing `facere_sensum-0.0.2/.github/workflows/lints.yaml` & `facere_sensum-0.0.3/.github/workflows/lints.yaml`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.2/src/facere_sensum/facere_sensum.py` & `facere_sensum-0.0.3/src/facere_sensum/facere_sensum.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 '''
 
 from argparse import ArgumentParser
 import datetime
 import numpy as np
 import pandas as pd
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 def score_manual(metric):
     '''
     Get metric score as a direct user input.
     'metric' is the metric text description.
     '''
     while True:
```

### Comparing `facere_sensum-0.0.2/test/test.py` & `facere_sensum-0.0.3/test/test.py`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.2/.gitignore` & `facere_sensum-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.2/LICENSE` & `facere_sensum-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.2/README.md` & `facere_sensum-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `facere_sensum-0.0.2/pyproject.toml` & `facere_sensum-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "facere-sensum"
-dynamic = ["version"]
+dynamic = [
+    "version",
+    "dependencies"
+]
 authors = [
   { name = "Serge Lunev" },
 ]
 description = "facere-sensum: make sense of the turmoil"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `facere_sensum-0.0.2/PKG-INFO` & `facere_sensum-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facere-sensum
-Version: 0.0.2
+Version: 0.0.3
 Summary: facere-sensum: make sense of the turmoil
 Project-URL: Homepage, https://github.com/lunarserge/facere-sensum
 Project-URL: Bug Tracker, https://github.com/lunarserge/facere-sensum/issues
 Author: Serge Lunev
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

