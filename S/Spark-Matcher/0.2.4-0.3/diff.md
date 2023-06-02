# Comparing `tmp/Spark-Matcher-0.2.4.tar.gz` & `tmp/Spark-Matcher-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spark-Matcher-0.2.4.tar", last modified: Wed Jan 25 13:38:13 2023, max compression
+gzip compressed data, was "Spark-Matcher-0.3.tar", last modified: Fri Jun  2 13:00:37 2023, max compression
```

## Comparing `Spark-Matcher-0.2.4.tar` & `Spark-Matcher-0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.731878 Spark-Matcher-0.2.4/
--rw-r--r--   0 ZV41NN     (503) staff       (20)    18091 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/LICENSE
--rw-r--r--   0 ZV41NN     (503) staff       (20)     4533 2023-01-25 13:38:13.731272 Spark-Matcher-0.2.4/PKG-INFO
--rw-r--r--   0 ZV41NN     (503) staff       (20)     4065 2023-01-02 14:13:14.000000 Spark-Matcher-0.2.4/README.md
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.702745 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/
--rw-r--r--   0 ZV41NN     (503) staff       (20)     4533 2023-01-25 13:38:13.000000 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/PKG-INFO
--rw-r--r--   0 ZV41NN     (503) staff       (20)     1335 2023-01-25 13:38:13.000000 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/SOURCES.txt
--rw-r--r--   0 ZV41NN     (503) staff       (20)        1 2023-01-25 13:38:13.000000 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/dependency_links.txt
--rw-r--r--   0 ZV41NN     (503) staff       (20)      539 2023-01-25 13:38:13.000000 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/requires.txt
--rw-r--r--   0 ZV41NN     (503) staff       (20)       14 2023-01-25 13:38:13.000000 Spark-Matcher-0.2.4/Spark_Matcher.egg-info/top_level.txt
--rw-r--r--   0 ZV41NN     (503) staff       (20)       84 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/pyproject.toml
--rw-r--r--   0 ZV41NN     (503) staff       (20)       38 2023-01-25 13:38:13.731960 Spark-Matcher-0.2.4/setup.cfg
--rw-r--r--   0 ZV41NN     (503) staff       (20)     1362 2023-01-25 13:14:39.000000 Spark-Matcher-0.2.4/setup.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.706372 Spark-Matcher-0.2.4/spark_matcher/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       22 2023-01-25 13:14:39.000000 Spark-Matcher-0.2.4/spark_matcher/__init__.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.707901 Spark-Matcher-0.2.4/spark_matcher/activelearner/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       72 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/activelearner/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     9637 2023-01-04 09:12:24.000000 Spark-Matcher-0.2.4/spark_matcher/activelearner/active_learner.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.711216 Spark-Matcher-0.2.4/spark_matcher/blocker/
--rw-r--r--   0 ZV41NN     (503) staff       (20)      124 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/blocker/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     6497 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/blocker/block_learner.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)    12577 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/blocker/blocking_rules.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)       57 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/config.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.717502 Spark-Matcher-0.2.4/spark_matcher/data/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       32 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)   340434 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/acm.csv
--rw-r--r--   0 ZV41NN     (503) staff       (20)     4049 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/datasets.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)   325443 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/dblp.csv
--rw-r--r--   0 ZV41NN     (503) staff       (20)     6370 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/stoxx50.csv
--rw-r--r--   0 ZV41NN     (503) staff       (20)    30053 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/voters_1.csv
--rw-r--r--   0 ZV41NN     (503) staff       (20)    30042 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/data/voters_2.csv
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.721887 Spark-Matcher-0.2.4/spark_matcher/deduplicator/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       66 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/deduplicator/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)    14753 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/deduplicator/connected_components_calculator.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)    14009 2023-01-02 14:13:14.000000 Spark-Matcher-0.2.4/spark_matcher/deduplicator/deduplicator.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     5781 2023-01-02 14:13:14.000000 Spark-Matcher-0.2.4/spark_matcher/deduplicator/hierarchical_clustering.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.723284 Spark-Matcher-0.2.4/spark_matcher/matcher/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       51 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/matcher/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     5883 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/matcher/matcher.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.725253 Spark-Matcher-0.2.4/spark_matcher/matching_base/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       67 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/matching_base/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)    10835 2023-01-06 09:28:41.000000 Spark-Matcher-0.2.4/spark_matcher/matching_base/matching_base.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.726676 Spark-Matcher-0.2.4/spark_matcher/sampler/
--rw-r--r--   0 ZV41NN     (503) staff       (20)      100 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/sampler/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)    14962 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/sampler/training_sampler.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.727941 Spark-Matcher-0.2.4/spark_matcher/scorer/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       48 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/scorer/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     3097 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/scorer/scorer.py
-drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-01-25 13:38:13.730054 Spark-Matcher-0.2.4/spark_matcher/similarity_metrics/
--rw-r--r--   0 ZV41NN     (503) staff       (20)       83 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/similarity_metrics/__init__.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     3929 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/similarity_metrics/similarity_metrics.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     3752 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/table_checkpointer.py
--rw-r--r--   0 ZV41NN     (503) staff       (20)     2880 2022-08-24 10:39:46.000000 Spark-Matcher-0.2.4/spark_matcher/utils.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.454727 Spark-Matcher-0.3/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    18091 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/LICENSE
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     4531 2023-06-02 13:00:37.454457 Spark-Matcher-0.3/PKG-INFO
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     4065 2023-01-02 14:13:14.000000 Spark-Matcher-0.3/README.md
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.430721 Spark-Matcher-0.3/Spark_Matcher.egg-info/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     4531 2023-06-02 13:00:37.000000 Spark-Matcher-0.3/Spark_Matcher.egg-info/PKG-INFO
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     1335 2023-06-02 13:00:37.000000 Spark-Matcher-0.3/Spark_Matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 ZV41NN     (503) staff       (20)        1 2023-06-02 13:00:37.000000 Spark-Matcher-0.3/Spark_Matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 ZV41NN     (503) staff       (20)      539 2023-06-02 13:00:37.000000 Spark-Matcher-0.3/Spark_Matcher.egg-info/requires.txt
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       14 2023-06-02 13:00:37.000000 Spark-Matcher-0.3/Spark_Matcher.egg-info/top_level.txt
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       84 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/pyproject.toml
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       38 2023-06-02 13:00:37.454789 Spark-Matcher-0.3/setup.cfg
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     1360 2023-06-02 12:19:56.000000 Spark-Matcher-0.3/setup.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.432922 Spark-Matcher-0.3/spark_matcher/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       20 2023-06-02 12:19:56.000000 Spark-Matcher-0.3/spark_matcher/__init__.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.433887 Spark-Matcher-0.3/spark_matcher/activelearner/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       72 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/activelearner/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     9637 2023-01-04 09:12:24.000000 Spark-Matcher-0.3/spark_matcher/activelearner/active_learner.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.437641 Spark-Matcher-0.3/spark_matcher/blocker/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)      124 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/blocker/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     6497 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/blocker/block_learner.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    12577 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/blocker/blocking_rules.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       57 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/config.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.444711 Spark-Matcher-0.3/spark_matcher/data/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       32 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)   340434 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/acm.csv
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     4049 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/datasets.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)   325443 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/dblp.csv
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     6370 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/stoxx50.csv
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    30053 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/voters_1.csv
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    30042 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/data/voters_2.csv
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.446520 Spark-Matcher-0.3/spark_matcher/deduplicator/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       66 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/deduplicator/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    15191 2023-06-02 12:15:19.000000 Spark-Matcher-0.3/spark_matcher/deduplicator/connected_components_calculator.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    14009 2023-01-02 14:13:14.000000 Spark-Matcher-0.3/spark_matcher/deduplicator/deduplicator.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     5781 2023-01-02 14:13:14.000000 Spark-Matcher-0.3/spark_matcher/deduplicator/hierarchical_clustering.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.447339 Spark-Matcher-0.3/spark_matcher/matcher/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       51 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/matcher/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     5883 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/matcher/matcher.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.450972 Spark-Matcher-0.3/spark_matcher/matching_base/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       67 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/matching_base/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    10835 2023-01-06 09:28:41.000000 Spark-Matcher-0.3/spark_matcher/matching_base/matching_base.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.451978 Spark-Matcher-0.3/spark_matcher/sampler/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)      100 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/sampler/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)    14962 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/sampler/training_sampler.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.452948 Spark-Matcher-0.3/spark_matcher/scorer/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       48 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/scorer/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     3097 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/scorer/scorer.py
+drwxr-xr-x   0 ZV41NN     (503) staff       (20)        0 2023-06-02 13:00:37.453995 Spark-Matcher-0.3/spark_matcher/similarity_metrics/
+-rw-r--r--   0 ZV41NN     (503) staff       (20)       83 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/similarity_metrics/__init__.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     3929 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/similarity_metrics/similarity_metrics.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     3752 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/table_checkpointer.py
+-rw-r--r--   0 ZV41NN     (503) staff       (20)     2880 2022-08-24 10:39:46.000000 Spark-Matcher-0.3/spark_matcher/utils.py
```

### Comparing `Spark-Matcher-0.2.4/LICENSE` & `Spark-Matcher-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/PKG-INFO` & `Spark-Matcher-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spark-Matcher
-Version: 0.2.4
+Version: 0.3
 Summary: Record matching and entity resolution at scale in Spark
 Author: Ahmet Bayraktar, Stan Leisink, Frits Hermans
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `Spark-Matcher-0.2.4/README.md` & `Spark-Matcher-0.3/README.md`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/Spark_Matcher.egg-info/PKG-INFO` & `Spark-Matcher-0.3/Spark_Matcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Spark-Matcher
-Version: 0.2.4
+Version: 0.3
 Summary: Record matching and entity resolution at scale in Spark
 Author: Ahmet Bayraktar, Stan Leisink, Frits Hermans
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `Spark-Matcher-0.2.4/Spark_Matcher.egg-info/SOURCES.txt` & `Spark-Matcher-0.3/Spark_Matcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/Spark_Matcher.egg-info/requires.txt` & `Spark-Matcher-0.3/Spark_Matcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/setup.py` & `Spark-Matcher-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 base_doc_packages = base_packages + doc_packages
 dev_packages = base_packages + doc_packages + util_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='Spark-Matcher',
-      version='0.2.4',
+      version='0.3',
       author="Ahmet Bayraktar, Stan Leisink, Frits Hermans",
       description="Record matching and entity resolution at scale in Spark",
       long_description=long_description,
       long_description_content_type="text/markdown",
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
```

### Comparing `Spark-Matcher-0.2.4/spark_matcher/activelearner/active_learner.py` & `Spark-Matcher-0.3/spark_matcher/activelearner/active_learner.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/blocker/block_learner.py` & `Spark-Matcher-0.3/spark_matcher/blocker/block_learner.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/blocker/blocking_rules.py` & `Spark-Matcher-0.3/spark_matcher/blocker/blocking_rules.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/acm.csv` & `Spark-Matcher-0.3/spark_matcher/data/acm.csv`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/datasets.py` & `Spark-Matcher-0.3/spark_matcher/data/datasets.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/dblp.csv` & `Spark-Matcher-0.3/spark_matcher/data/dblp.csv`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/stoxx50.csv` & `Spark-Matcher-0.3/spark_matcher/data/stoxx50.csv`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/voters_1.csv` & `Spark-Matcher-0.3/spark_matcher/data/voters_1.csv`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/data/voters_2.csv` & `Spark-Matcher-0.3/spark_matcher/data/voters_2.csv`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/deduplicator/connected_components_calculator.py` & `Spark-Matcher-0.3/spark_matcher/deduplicator/connected_components_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #          Stan Leisink
 #          Frits Hermans
 
 from typing import List, Tuple
 
 from graphframes import GraphFrame
 from pyspark.sql import functions as F, types as T, DataFrame, Window
+from pyspark.sql.utils import AnalysisException
 
 from spark_matcher.table_checkpointer import TableCheckpointer
 
 
 class ConnectedComponentsCalculator:
 
     def __init__(self, scored_pairs_table: DataFrame, max_edges_clustering: int,
@@ -51,15 +52,21 @@
 
         Args:
             scores_table: a pairs table with similarity scores for each pair
         Returns:
             a spark dataframe containing the connected components of a graph of scored pairs.
         """
         graph = self._create_graph(scores_table)
-        connected_components = graph.connectedComponents()
+        # Since graphframes 0.3.0, checkpointing is used for the connected components algorithm. The Spark cluster might
+        # not allow writing checkpoints. In such case we fall back to the graphx algorithm that doesn't require
+        # checkpointing.
+        try:
+            connected_components = graph.connectedComponents()
+        except AnalysisException:
+            connected_components = graph.connectedComponents(algorithm='graphx')
         return self.table_checkpointer(connected_components, checkpoint_name)
 
     @staticmethod
     def _add_component_id_to_scores_table(scores_table: DataFrame, connected_components: DataFrame) -> DataFrame:
         """
         This function joins the initial connected-component identifiers to the scored pairs table. For each scored pair,
         a component identifier indicating to which subgraph a pair belongs is added.
```

### Comparing `Spark-Matcher-0.2.4/spark_matcher/deduplicator/deduplicator.py` & `Spark-Matcher-0.3/spark_matcher/deduplicator/deduplicator.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/deduplicator/hierarchical_clustering.py` & `Spark-Matcher-0.3/spark_matcher/deduplicator/hierarchical_clustering.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/matcher/matcher.py` & `Spark-Matcher-0.3/spark_matcher/matcher/matcher.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/matching_base/matching_base.py` & `Spark-Matcher-0.3/spark_matcher/matching_base/matching_base.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/sampler/training_sampler.py` & `Spark-Matcher-0.3/spark_matcher/sampler/training_sampler.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/scorer/scorer.py` & `Spark-Matcher-0.3/spark_matcher/scorer/scorer.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/similarity_metrics/similarity_metrics.py` & `Spark-Matcher-0.3/spark_matcher/similarity_metrics/similarity_metrics.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/table_checkpointer.py` & `Spark-Matcher-0.3/spark_matcher/table_checkpointer.py`

 * *Files identical despite different names*

### Comparing `Spark-Matcher-0.2.4/spark_matcher/utils.py` & `Spark-Matcher-0.3/spark_matcher/utils.py`

 * *Files identical despite different names*

