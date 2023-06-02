# Comparing `tmp/prostate-nomograms-0.0.3.tar.gz` & `tmp/prostate-nomograms-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prostate-nomograms-0.0.3.tar", last modified: Fri Jun  2 20:03:09 2023, max compression
+gzip compressed data, was "prostate-nomograms-0.0.4.tar", last modified: Fri Jun  2 20:07:32 2023, max compression
```

## Comparing `prostate-nomograms-0.0.3.tar` & `prostate-nomograms-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.292129 prostate-nomograms-0.0.3/
--rw-rw-rw-   0        0        0    11549 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3522 2023-06-02 20:03:09.291079 prostate-nomograms-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2912 2023-06-02 19:42:50.000000 prostate-nomograms-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.255999 prostate-nomograms-0.0.3/examples/
--rw-rw-rw-   0        0        0        0 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.3/examples/__init__.py
--rw-rw-rw-   0        0        0      150 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.3/examples/env_examples.py
--rw-rw-rw-   0        0        0     3569 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.3/examples/ex01-mskcc.py
--rw-rw-rw-   0        0        0     3781 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.3/examples/ex02-capra.py
--rw-rw-rw-   0        0        0     3914 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.3/examples/ex03-custom.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.258120 prostate-nomograms-0.0.3/prostate_nomograms/
--rw-rw-rw-   0        0        0      465 2023-06-02 20:02:12.000000 prostate-nomograms-0.0.3/prostate_nomograms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.273984 prostate-nomograms-0.0.3/prostate_nomograms/capra/
--rw-rw-rw-   0        0        0       34 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.3/prostate_nomograms/capra/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.276985 prostate-nomograms-0.0.3/prostate_nomograms/capra/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/capra/base/__init__.py
--rw-rw-rw-   0        0        0     1336 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.3/prostate_nomograms/capra/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2273 2023-05-31 23:11:28.000000 prostate-nomograms-0.0.3/prostate_nomograms/capra/base/survival_regression.py
--rw-rw-rw-   0        0        0    12184 2023-06-02 20:01:55.000000 prostate-nomograms-0.0.3/prostate_nomograms/capra/capra.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.279999 prostate-nomograms-0.0.3/prostate_nomograms/custom/
--rw-rw-rw-   0        0        0       36 2023-05-31 19:54:31.000000 prostate-nomograms-0.0.3/prostate_nomograms/custom/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.282986 prostate-nomograms-0.0.3/prostate_nomograms/custom/base/
--rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/custom/base/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.3/prostate_nomograms/custom/base/logistic_regression.py
--rw-rw-rw-   0        0        0     2192 2023-05-31 15:13:00.000000 prostate-nomograms-0.0.3/prostate_nomograms/custom/base/survival_regression.py
--rw-rw-rw-   0        0        0     9078 2023-05-31 22:07:18.000000 prostate-nomograms-0.0.3/prostate_nomograms/custom/custom.py
--rw-rw-rw-   0        0        0     1162 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.3/prostate_nomograms/enum.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.284129 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/
--rw-rw-rw-   0        0        0       86 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.289988 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/
--rw-rw-rw-   0        0        0       26 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/__init__.py
--rw-rw-rw-   0        0        0     9792 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/logistic_regression.py
--rw-rw-rw-   0        0        0    10577 2023-05-31 22:05:59.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/model.py
--rw-rw-rw-   0        0        0     2533 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/survival_regression.py
--rw-rw-rw-   0        0        0     5490 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/web_table_scraper.py
--rw-rw-rw-   0        0        0     2841 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.3/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:03:09.271983 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/
--rw-rw-rw-   0        0        0     3522 2023-06-02 20:03:09.000000 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-06-02 20:03:09.000000 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:03:09.000000 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-02 20:03:09.000000 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-02 20:03:09.000000 prostate-nomograms-0.0.3/prostate_nomograms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 20:03:09.292129 prostate-nomograms-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-06-02 20:02:12.000000 prostate-nomograms-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.494962 prostate-nomograms-0.0.4/
+-rw-rw-rw-   0        0        0    11549 2023-06-02 19:44:39.000000 prostate-nomograms-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3522 2023-06-02 20:07:32.494962 prostate-nomograms-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2912 2023-06-02 19:42:50.000000 prostate-nomograms-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.463710 prostate-nomograms-0.0.4/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.4/examples/__init__.py
+-rw-rw-rw-   0        0        0      150 2023-05-09 17:06:15.000000 prostate-nomograms-0.0.4/examples/env_examples.py
+-rw-rw-rw-   0        0        0     3569 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.4/examples/ex01-mskcc.py
+-rw-rw-rw-   0        0        0     3781 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.4/examples/ex02-capra.py
+-rw-rw-rw-   0        0        0     3914 2023-06-02 19:21:40.000000 prostate-nomograms-0.0.4/examples/ex03-custom.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.463710 prostate-nomograms-0.0.4/prostate_nomograms/
+-rw-rw-rw-   0        0        0      465 2023-06-02 20:07:04.000000 prostate-nomograms-0.0.4/prostate_nomograms/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.479336 prostate-nomograms-0.0.4/prostate_nomograms/capra/
+-rw-rw-rw-   0        0        0       34 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.4/prostate_nomograms/capra/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.479336 prostate-nomograms-0.0.4/prostate_nomograms/capra/base/
+-rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/capra/base/__init__.py
+-rw-rw-rw-   0        0        0     1336 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.4/prostate_nomograms/capra/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2273 2023-05-31 23:11:28.000000 prostate-nomograms-0.0.4/prostate_nomograms/capra/base/survival_regression.py
+-rw-rw-rw-   0        0        0    12184 2023-06-02 20:01:55.000000 prostate-nomograms-0.0.4/prostate_nomograms/capra/capra.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.479336 prostate-nomograms-0.0.4/prostate_nomograms/custom/
+-rw-rw-rw-   0        0        0       36 2023-05-31 19:54:31.000000 prostate-nomograms-0.0.4/prostate_nomograms/custom/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.479336 prostate-nomograms-0.0.4/prostate_nomograms/custom/base/
+-rw-rw-rw-   0        0        0      106 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/custom/base/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-06-01 15:55:16.000000 prostate-nomograms-0.0.4/prostate_nomograms/custom/base/logistic_regression.py
+-rw-rw-rw-   0        0        0     2192 2023-05-31 15:13:00.000000 prostate-nomograms-0.0.4/prostate_nomograms/custom/base/survival_regression.py
+-rw-rw-rw-   0        0        0     9078 2023-05-31 22:07:18.000000 prostate-nomograms-0.0.4/prostate_nomograms/custom/custom.py
+-rw-rw-rw-   0        0        0     1162 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.4/prostate_nomograms/enum.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.494962 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/
+-rw-rw-rw-   0        0        0       86 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.494962 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/
+-rw-rw-rw-   0        0        0       26 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/__init__.py
+-rw-rw-rw-   0        0        0     9792 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/logistic_regression.py
+-rw-rw-rw-   0        0        0    10577 2023-05-31 22:05:59.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/model.py
+-rw-rw-rw-   0        0        0     2533 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/survival_regression.py
+-rw-rw-rw-   0        0        0     5490 2023-05-31 14:34:11.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/web_table_scraper.py
+-rw-rw-rw-   0        0        0     2841 2023-06-02 19:10:35.000000 prostate-nomograms-0.0.4/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:07:32.479336 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/
+-rw-rw-rw-   0        0        0     3522 2023-06-02 20:07:32.000000 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-06-02 20:07:32.000000 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:07:32.000000 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-02 20:07:32.000000 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-06-02 20:07:32.000000 prostate-nomograms-0.0.4/prostate_nomograms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:07:32.494962 prostate-nomograms-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2023-06-02 20:07:04.000000 prostate-nomograms-0.0.4/setup.py
```

### Comparing `prostate-nomograms-0.0.3/LICENSE` & `prostate-nomograms-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/PKG-INFO` & `prostate-nomograms-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.3
+Version: 0.0.4
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.3/README.md` & `prostate-nomograms-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/examples/ex01-mskcc.py` & `prostate-nomograms-0.0.4/examples/ex01-mskcc.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/examples/ex02-capra.py` & `prostate-nomograms-0.0.4/examples/ex02-capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/examples/ex03-custom.py` & `prostate-nomograms-0.0.4/examples/ex03-custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/capra/base/logistic_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/capra/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/capra/base/survival_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/capra/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/capra/capra.py` & `prostate-nomograms-0.0.4/prostate_nomograms/capra/capra.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/custom/base/logistic_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/custom/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/custom/base/survival_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/custom/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/custom/custom.py` & `prostate-nomograms-0.0.4/prostate_nomograms/custom/custom.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/enum.py` & `prostate-nomograms-0.0.4/prostate_nomograms/enum.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/logistic_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/model.py` & `prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/model.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/survival_regression.py` & `prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/survival_regression.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/mskcc/base/web_table_scraper.py` & `prostate-nomograms-0.0.4/prostate_nomograms/mskcc/base/web_table_scraper.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py` & `prostate-nomograms-0.0.4/prostate_nomograms/mskcc/pre_radical_prostatectomy_nomogram.py`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms.egg-info/PKG-INFO` & `prostate-nomograms-0.0.4/prostate_nomograms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prostate-nomograms
-Version: 0.0.3
+Version: 0.0.4
 Summary: Prediction tools based on existing prostate cancer nomograms.
 Home-page: https://github.com/MaxenceLarose/prostate-nomograms
 Author: Maxence Larose
 Author-email: maxence.larose.1@ulaval.ca
 License: Apache License 2.0
 Keywords: cancer medical nomogram prediction prostate python3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prostate-nomograms-0.0.3/prostate_nomograms.egg-info/SOURCES.txt` & `prostate-nomograms-0.0.4/prostate_nomograms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prostate-nomograms-0.0.3/setup.py` & `prostate-nomograms-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="prostate-nomograms",
-    version="0.0.3",
+    version="0.0.4",
     author="Maxence Larose",
     author_email="maxence.larose.1@ulaval.ca",
     description="Prediction tools based on existing prostate cancer nomograms.",
     long_description=open('README.md', "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/MaxenceLarose/prostate-nomograms",
     license="Apache License 2.0",
@@ -15,14 +15,15 @@
     python_requires=">=3.7",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
+        "lxml",
         "numpy",
         "openpyxl",
         "pandas",
         "requests",
         "scikit-learn",
         "scikit-survival",
         "scipy"
```

