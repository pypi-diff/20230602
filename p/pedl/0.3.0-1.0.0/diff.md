# Comparing `tmp/pedl-0.3.0.tar.gz` & `tmp/pedl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pedl-0.3.0.tar", last modified: Thu Jun 24 15:55:15 2021, max compression
+gzip compressed data, was "pedl-1.0.0.tar", last modified: Fri Jun  2 13:28:26 2023, max compression
```

## Comparing `pedl-0.3.0.tar` & `pedl-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,58 @@
-drwxr-xr-x   0 leonweber   (501) staff       (20)        0 2021-06-24 15:55:15.628905 pedl-0.3.0/
--rw-r--r--   0 leonweber   (501) staff       (20)     7131 2021-06-24 15:55:15.628724 pedl-0.3.0/PKG-INFO
--rw-r--r--   0 leonweber   (501) staff       (20)     5648 2021-06-24 15:51:49.000000 pedl-0.3.0/README.md
-drwxr-xr-x   0 leonweber   (501) staff       (20)        0 2021-06-24 15:55:15.598920 pedl-0.3.0/pedl/
--rw-r--r--   0 leonweber   (501) staff       (20)       22 2021-06-24 15:55:12.000000 pedl-0.3.0/pedl/__init__.py
--rw-r--r--   0 leonweber   (501) staff       (20)     9163 2021-06-24 15:19:59.000000 pedl-0.3.0/pedl/cli.py
-drwxr-xr-x   0 leonweber   (501) staff       (20)        0 2021-06-24 15:55:15.624930 pedl-0.3.0/pedl/data/
--rw-r--r--   0 leonweber   (501) staff       (20) 18171360 2021-06-16 14:22:40.000000 pedl-0.3.0/pedl/data/HOM_AllOrganism.rpt
--rw-r--r--   0 leonweber   (501) staff       (20)  5179646 2021-06-21 11:44:13.000000 pedl-0.3.0/pedl/data/geneid_to_name.json
--rw-r--r--   0 leonweber   (501) staff       (20)   716415 2021-06-18 08:39:27.000000 pedl-0.3.0/pedl/data/uniprot2geneid.json
--rw-r--r--   0 leonweber   (501) staff       (20)     1634 2021-06-18 11:36:35.000000 pedl-0.3.0/pedl/database.py
--rw-r--r--   0 leonweber   (501) staff       (20)     5032 2021-06-17 13:00:41.000000 pedl-0.3.0/pedl/dataset.py
--rw-------   0 leonweber   (501) staff       (20)     1748 2021-06-15 10:59:15.000000 pedl-0.3.0/pedl/model.py
--rw-r--r--   0 leonweber   (501) staff       (20)    30022 2021-06-24 15:25:29.000000 pedl-0.3.0/pedl/utils.py
-drwxr-xr-x   0 leonweber   (501) staff       (20)        0 2021-06-24 15:55:15.599861 pedl-0.3.0/pedl.egg-info/
--rw-r--r--   0 leonweber   (501) staff       (20)     7131 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/PKG-INFO
--rw-r--r--   0 leonweber   (501) staff       (20)      368 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/SOURCES.txt
--rw-r--r--   0 leonweber   (501) staff       (20)        1 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/dependency_links.txt
--rw-r--r--   0 leonweber   (501) staff       (20)       40 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/entry_points.txt
--rw-r--r--   0 leonweber   (501) staff       (20)       83 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/requires.txt
--rw-r--r--   0 leonweber   (501) staff       (20)        5 2021-06-24 15:55:15.000000 pedl-0.3.0/pedl.egg-info/top_level.txt
--rw-r--r--   0 leonweber   (501) staff       (20)       38 2021-06-24 15:55:15.628956 pedl-0.3.0/setup.cfg
--rw-r--r--   0 leonweber   (501) staff       (20)      697 2021-06-24 15:54:58.000000 pedl-0.3.0/setup.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.607981 pedl-1.0.0/
+-rw-r--r--   0 leon       (501) staff       (20)     5929 2023-06-02 13:28:26.607852 pedl-1.0.0/PKG-INFO
+-rw-r--r--   0 leon       (501) staff       (20)     5637 2023-06-02 13:25:24.000000 pedl-1.0.0/README.md
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.586580 pedl-1.0.0/pedl/
+-rw-r--r--   0 leon       (501) staff       (20)       22 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)     4898 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/bert_for_distant_supervision.py
+-rw-r--r--   0 leon       (501) staff       (20)     4242 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/build_training_set.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587725 pedl-1.0.0/pedl/configs/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      501 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/build_training_set.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587920 pedl-1.0.0/pedl/configs/database/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/database/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      452 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/database/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588018 pedl-1.0.0/pedl/configs/elastic/
+-rw-r--r--   0 leon       (501) staff       (20)       67 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/elastic/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588201 pedl-1.0.0/pedl/configs/entities/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/entities/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)       96 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/entities/default.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588295 pedl-1.0.0/pedl/configs/hydra/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/hydra/__init__.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.588867 pedl-1.0.0/pedl/configs/hydra/help/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/hydra/help/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      967 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/build_training_set_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)     1109 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/excel_summarize_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)     1549 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/predict_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      745 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/pubtator_elasticsearch_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      823 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/hydra/help/rebuild_pubtator_index_help.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      858 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/predict.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      116 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/pubtator_elaticsearch.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      503 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/rebuild_pubtator_index.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      849 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/summarize.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.589144 pedl-1.0.0/pedl/configs/type/
+-rw-r--r--   0 leon       (501) staff       (20)       21 2023-06-02 13:27:53.000000 pedl-1.0.0/pedl/configs/type/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)      556 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/type/drug_protein.yaml
+-rw-r--r--   0 leon       (501) staff       (20)      476 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/configs/type/protein_protein.yaml
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.605622 pedl-1.0.0/pedl/data/
+-rw-r--r--   0 leon       (501) staff       (20) 18171360 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/HOM_AllOrganism.rpt
+-rw-r--r--   0 leon       (501) staff       (20)  5179646 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/geneid_to_name.json
+-rw-r--r--   0 leon       (501) staff       (20)   716415 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/data/uniprot2geneid.json
+-rw-r--r--   0 leon       (501) staff       (20)    18740 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/data_getter.py
+-rw-r--r--   0 leon       (501) staff       (20)     1634 2022-12-02 15:16:45.000000 pedl-1.0.0/pedl/database.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.606782 pedl-1.0.0/pedl/datasets/
+-rw-r--r--   0 leon       (501) staff       (20)        0 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/datasets/__init__.py
+-rw-r--r--   0 leon       (501) staff       (20)     5473 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/datasets/pedl_dataset.py
+-rw-r--r--   0 leon       (501) staff       (20)     7997 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/predict.py
+-rw-r--r--   0 leon       (501) staff       (20)     8640 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/pubtator_elasticsearch.py
+-rw-r--r--   0 leon       (501) staff       (20)     1112 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/rebuild_pubtator_index.py
+-rw-r--r--   0 leon       (501) staff       (20)    13091 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/summarize.py
+-rw-r--r--   0 leon       (501) staff       (20)    18176 2023-05-15 11:13:55.000000 pedl-1.0.0/pedl/utils.py
+drwxr-xr-x   0 leon       (501) staff       (20)        0 2023-06-02 13:28:26.587167 pedl-1.0.0/pedl.egg-info/
+-rw-r--r--   0 leon       (501) staff       (20)     5929 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/PKG-INFO
+-rw-r--r--   0 leon       (501) staff       (20)     1362 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/SOURCES.txt
+-rw-r--r--   0 leon       (501) staff       (20)        1 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/dependency_links.txt
+-rw-r--r--   0 leon       (501) staff       (20)      246 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/entry_points.txt
+-rw-r--r--   0 leon       (501) staff       (20)      161 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/requires.txt
+-rw-r--r--   0 leon       (501) staff       (20)        5 2023-06-02 13:28:26.000000 pedl-1.0.0/pedl.egg-info/top_level.txt
+-rw-r--r--   0 leon       (501) staff       (20)       38 2023-06-02 13:28:26.608040 pedl-1.0.0/setup.cfg
+-rw-r--r--   0 leon       (501) staff       (20)     1304 2023-06-02 13:27:53.000000 pedl-1.0.0/setup.py
```

### Comparing `pedl-0.3.0/pedl/data/HOM_AllOrganism.rpt` & `pedl-1.0.0/pedl/data/HOM_AllOrganism.rpt`

 * *Files identical despite different names*

### Comparing `pedl-0.3.0/pedl/data/geneid_to_name.json` & `pedl-1.0.0/pedl/data/geneid_to_name.json`

 * *Files identical despite different names*

### Comparing `pedl-0.3.0/pedl/data/uniprot2geneid.json` & `pedl-1.0.0/pedl/data/uniprot2geneid.json`

 * *Files identical despite different names*

### Comparing `pedl-0.3.0/pedl/database.py` & `pedl-1.0.0/pedl/database.py`

 * *Files identical despite different names*

### Comparing `pedl-0.3.0/setup.py` & `pedl-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name='pedl',
-    version='0.3.0',
+    version='1.0.0',
     description='Search the biomedical literature for protein interactions and'
                 'protein associations.',
     url='https://github.com/leonweber/pedl',
     author='Leon Weber',
     author_email='leonweber@posteo.de',
     license='MIT',
     packages=find_packages(),
     install_requires=required,
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
-    entry_points={"console_scripts": ["pedl=pedl.cli:main"]},
-    package_data={"pedl": ["data/*"]}
-)
+    entry_points={"console_scripts": ["pedl-summarize=pedl.summarize:summarize",
+                                      "pedl-rebuild_pubtator_index=pedl.rebuild_pubtator_index:rebuild_pubtator_index",
+                                      "pedl-build_training_set=pedl.build_training_set:build_training_set",
+                                      "pedl-extract=pedl.predict:predict"]},
+    package_data={"pedl": ["data/*",
+                           'configs/*',
+                           'configs/database/*',
+                           'configs/entities/*',
+                           'configs/elastic/*',
+                           'configs/type/*',
+                           'configs/hydra/help/*']}
+)
```

