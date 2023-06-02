# Comparing `tmp/semanticlayertools-0.2.1.tar.gz` & `tmp/semanticlayertools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticlayertools-0.2.1.tar", last modified: Fri Oct 28 15:54:36 2022, max compression
+gzip compressed data, was "semanticlayertools-0.2.2.tar", last modified: Fri Jun  2 18:12:37 2023, max compression
```

## Comparing `semanticlayertools-0.2.1.tar` & `semanticlayertools-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      218 2022-03-03 15:21:33.000000 semanticlayertools-0.2.1/AUTHORS.rst
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1086 2022-01-06 13:40:40.000000 semanticlayertools-0.2.1/LICENSE.md
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2153 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/PKG-INFO
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1420 2022-04-28 12:56:59.000000 semanticlayertools-0.2.1/README.md
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      104 2021-09-30 09:13:37.000000 semanticlayertools-0.2.1/pyproject.toml
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1026 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/setup.cfg
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.097248 semanticlayertools-0.2.1/src/
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.097248 semanticlayertools-0.2.1/src/semanticlayertools/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 semanticlayertools-0.2.1/src/semanticlayertools/__init__.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.097248 semanticlayertools-0.2.1/src/semanticlayertools/cleaning/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 semanticlayertools-0.2.1/src/semanticlayertools/cleaning/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4002 2022-10-11 08:57:14.000000 semanticlayertools-0.2.1/src/semanticlayertools/cleaning/text.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/src/semanticlayertools/clustering/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 10:26:40.000000 semanticlayertools-0.2.1/src/semanticlayertools/clustering/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     4158 2022-08-25 06:51:43.000000 semanticlayertools-0.2.1/src/semanticlayertools/clustering/infomap.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     6665 2022-06-01 08:14:56.000000 semanticlayertools-0.2.1/src/semanticlayertools/clustering/leiden.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    11073 2022-03-03 13:15:57.000000 semanticlayertools-0.2.1/src/semanticlayertools/clustering/reports.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/src/semanticlayertools/linkage/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-09-30 09:13:37.000000 semanticlayertools-0.2.1/src/semanticlayertools/linkage/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     8171 2022-08-17 11:30:23.000000 semanticlayertools-0.2.1/src/semanticlayertools/linkage/cocitation.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    32657 2022-10-28 15:52:49.000000 semanticlayertools-0.2.1/src/semanticlayertools/linkage/wordscore.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/src/semanticlayertools/metric/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2022-06-01 12:21:33.000000 semanticlayertools-0.2.1/src/semanticlayertools/metric/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     6603 2022-08-17 11:30:23.000000 semanticlayertools-0.2.1/src/semanticlayertools/metric/centralities.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     8971 2022-09-12 12:43:35.000000 semanticlayertools-0.2.1/src/semanticlayertools/metric/linguistic.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/src/semanticlayertools/pipelines/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-12-21 08:42:16.000000 semanticlayertools-0.2.1/src/semanticlayertools/pipelines/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     3505 2022-08-17 11:30:23.000000 semanticlayertools-0.2.1/src/semanticlayertools/pipelines/cocitetimeclusters.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     5974 2022-08-17 11:30:23.000000 semanticlayertools-0.2.1/src/semanticlayertools/pipelines/wordscorenet.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.101248 semanticlayertools-0.2.1/src/semanticlayertools/visual/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        0 2021-12-21 08:42:16.000000 semanticlayertools-0.2.1/src/semanticlayertools/visual/__init__.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)    10641 2022-04-28 12:56:59.000000 semanticlayertools-0.2.1/src/semanticlayertools/visual/citationnet.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     3760 2022-10-27 10:21:49.000000 semanticlayertools-0.2.1/src/semanticlayertools/visual/embedding.py
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     5706 2022-03-03 08:34:38.000000 semanticlayertools-0.2.1/src/semanticlayertools/visual/utils.py
-drwxrwxr-x   0 mvogl     (1000) mvogl     (1000)        0 2022-10-28 15:54:36.097248 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     2153 2022-10-28 15:54:36.000000 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/PKG-INFO
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)     1167 2022-10-28 15:54:36.000000 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/SOURCES.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)        1 2022-10-28 15:54:36.000000 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/dependency_links.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)      261 2022-10-28 15:54:36.000000 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/requires.txt
--rw-rw-r--   0 mvogl     (1000) mvogl     (1000)       19 2022-10-28 15:54:36.000000 semanticlayertools-0.2.1/src/semanticlayertools.egg-info/top_level.txt
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.794965 semanticlayertools-0.2.2/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      218 2022-03-04 07:55:30.000000 semanticlayertools-0.2.2/AUTHORS.rst
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1086 2022-01-06 14:36:54.000000 semanticlayertools-0.2.2/LICENSE.md
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     2440 2023-06-02 18:12:37.794965 semanticlayertools-0.2.2/PKG-INFO
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1707 2023-03-17 09:51:42.000000 semanticlayertools-0.2.2/README.md
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      104 2021-09-24 07:47:48.000000 semanticlayertools-0.2.2/pyproject.toml
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1052 2023-06-02 18:12:37.794965 semanticlayertools-0.2.2/setup.cfg
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.778965 semanticlayertools-0.2.2/src/
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.782965 semanticlayertools-0.2.2/src/semanticlayertools/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 07:44:54.000000 semanticlayertools-0.2.2/src/semanticlayertools/__init__.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.786965 semanticlayertools-0.2.2/src/semanticlayertools/cleaning/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 12:46:37.000000 semanticlayertools-0.2.2/src/semanticlayertools/cleaning/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4003 2023-06-02 16:23:43.000000 semanticlayertools-0.2.2/src/semanticlayertools/cleaning/text.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.786965 semanticlayertools-0.2.2/src/semanticlayertools/clustering/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-10-01 08:03:42.000000 semanticlayertools-0.2.2/src/semanticlayertools/clustering/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4158 2022-08-23 13:47:46.000000 semanticlayertools-0.2.2/src/semanticlayertools/clustering/infomap.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     6665 2022-05-13 11:06:58.000000 semanticlayertools-0.2.2/src/semanticlayertools/clustering/leiden.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    11119 2023-06-02 17:10:32.000000 semanticlayertools-0.2.2/src/semanticlayertools/clustering/reports.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.790965 semanticlayertools-0.2.2/src/semanticlayertools/linkage/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-09-24 12:46:16.000000 semanticlayertools-0.2.2/src/semanticlayertools/linkage/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    14581 2023-06-02 18:03:38.000000 semanticlayertools-0.2.2/src/semanticlayertools/linkage/citation.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    14233 2023-05-21 09:58:11.000000 semanticlayertools-0.2.2/src/semanticlayertools/linkage/worddistributions.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    32657 2022-11-21 08:25:18.000000 semanticlayertools-0.2.2/src/semanticlayertools/linkage/wordscore.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.790965 semanticlayertools-0.2.2/src/semanticlayertools/metric/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2022-06-03 07:49:30.000000 semanticlayertools-0.2.2/src/semanticlayertools/metric/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     6566 2023-05-30 14:41:42.000000 semanticlayertools-0.2.2/src/semanticlayertools/metric/centralities.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     8971 2022-09-20 06:32:04.000000 semanticlayertools-0.2.2/src/semanticlayertools/metric/linguistic.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.790965 semanticlayertools-0.2.2/src/semanticlayertools/pipelines/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-12-17 07:10:57.000000 semanticlayertools-0.2.2/src/semanticlayertools/pipelines/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     4545 2023-06-02 17:51:45.000000 semanticlayertools-0.2.2/src/semanticlayertools/pipelines/cocitetimeclusters.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     5974 2022-06-23 14:41:32.000000 semanticlayertools-0.2.2/src/semanticlayertools/pipelines/wordscorenet.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.794965 semanticlayertools-0.2.2/src/semanticlayertools/visual/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        0 2021-12-17 07:10:57.000000 semanticlayertools-0.2.2/src/semanticlayertools/visual/__init__.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)    10597 2023-02-24 13:46:41.000000 semanticlayertools-0.2.2/src/semanticlayertools/visual/citationnet.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     3760 2022-11-21 08:25:18.000000 semanticlayertools-0.2.2/src/semanticlayertools/visual/embedding.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     7568 2023-06-02 18:10:33.000000 semanticlayertools-0.2.2/src/semanticlayertools/visual/plotting.py
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     5706 2022-03-04 07:55:30.000000 semanticlayertools-0.2.2/src/semanticlayertools/visual/utils.py
+drwxrwxr-x   0 arbeit    (1003) arbeit    (1003)        0 2023-06-02 18:12:37.786965 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     2440 2023-06-02 18:12:37.000000 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/PKG-INFO
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)     1259 2023-06-02 18:12:37.000000 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/SOURCES.txt
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)        1 2023-06-02 18:12:37.000000 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/dependency_links.txt
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)      285 2023-06-02 18:12:37.000000 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/requires.txt
+-rw-rw-r--   0 arbeit    (1003) arbeit    (1003)       19 2023-06-02 18:12:37.000000 semanticlayertools-0.2.2/src/semanticlayertools.egg-info/top_level.txt
```

### Comparing `semanticlayertools-0.2.1/LICENSE.md` & `semanticlayertools-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/PKG-INFO` & `semanticlayertools-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticlayertools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create semantic layers using different methods for word linking.
 Home-page: https://gitlab.gwdg.de/modelsen/semanticlayertools
 Author: Malte Vogl
 Author-email: mvogl@mpiwg-berlin.mpg.de
 Project-URL: Project Home, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Bug Tracker, https://gitlab.gwdg.de/modelsen/semanticlayertools/-/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,20 +14,24 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: embeddml
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
+<img src="https://img.shields.io/badge/DHCodeReview-passed-brightgreen" alt="DHCodeReview" style="float: left; margin-right: 10px;" />[Review](https://github.com/DHCodeReview/DHCodeReview/issues/1)
+
 ## SemanticLayerTools
 
 Collects tools to create semantic layers in the socio-epistemic networks framework. Source material can be any structured corpus with metadata of authors, time, and at least one text column.
 
 Documentation is available on [ReadTheDocs](https://semanticlayertools.readthedocs.io/).
 
+Part of the code was reviewed by [Itay Zandbank](https://github.com/zmbq), thank you. 
+
 ## Installation
 
 tl;dr Use pip
 
 ~~~bash
 pip install semanticlayertools
 ~~~
```

### Comparing `semanticlayertools-0.2.1/README.md` & `semanticlayertools-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+<img src="https://img.shields.io/badge/DHCodeReview-passed-brightgreen" alt="DHCodeReview" style="float: left; margin-right: 10px;" />[Review](https://github.com/DHCodeReview/DHCodeReview/issues/1)
+
 ## SemanticLayerTools
 
 Collects tools to create semantic layers in the socio-epistemic networks framework. Source material can be any structured corpus with metadata of authors, time, and at least one text column.
 
 Documentation is available on [ReadTheDocs](https://semanticlayertools.readthedocs.io/).
 
+Part of the code was reviewed by [Itay Zandbank](https://github.com/zmbq), thank you. 
+
 ## Installation
 
 tl;dr Use pip
 
 ~~~bash
 pip install semanticlayertools
 ~~~
```

### Comparing `semanticlayertools-0.2.1/setup.cfg` & `semanticlayertools-0.2.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = semanticlayertools
-version = 0.2.1
+version = 0.2.2
 author = Malte Vogl
 author_email = mvogl@mpiwg-berlin.mpg.de
 description = Create semantic layers using different methods for word linking.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.gwdg.de/modelsen/semanticlayertools
 project_urls = 
@@ -27,14 +27,16 @@
 	scipy
 	spacy
 	textacy
 	pandas
 	infomap >= 2.3
 	igraph
 	leidenalg
+	datashader
+	scikit-image
 
 [options.extras_require]
 all = 
 	%(embeddml)s
 	%(dev)s
 dev = 
 	twine
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/cleaning/text.py` & `semanticlayertools-0.2.2/src/semanticlayertools/cleaning/text.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,8 +109,8 @@
         for ngramLen in range(ngramRange[0], ngramRange[1] + 1, 1):
             ngrams = zip(*[elem[i:] for i in range(ngramLen)])
             ngramList.append(list(ngrams))
     if debug is True:
         print(f"Created ngrams in {time.time() - starttime} sec.")
     extractedNgrams = [x for y in ngramList for x in y]
     reformated = ['#'.join(elem) for elem in extractedNgrams]
-    return reformated
+    return reformated
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/clustering/infomap.py` & `semanticlayertools-0.2.2/src/semanticlayertools/clustering/infomap.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/clustering/leiden.py` & `semanticlayertools-0.2.2/src/semanticlayertools/clustering/leiden.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/clustering/reports.py` & `semanticlayertools-0.2.2/src/semanticlayertools/clustering/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 import spacy
 import textacy
 import textacy.tm
 import pandas as pd
 import warnings
 
+from ..cleaning.text import htmlTags
+
 num_processes = multiprocessing.cpu_count()
 
 
 class ClusterReports():
     """Generate reporting on time-clusters.
 
     Generate reports to describe the content for all found clusters above a
@@ -94,21 +96,21 @@
         :returns: A textacy corpus file with english as the base language
         :rtype: `textacy.Corpus`
         """
         mainLanguageCorp = 'en_core_web_lg'
         nlp = spacy.load(mainLanguageCorp)
 
         docs = []
-        titles = dataframe[self.textcolumn].values
+        titles = dataframe.dropna(subset=self.textcolumn)[self.textcolumn].values
         for title in tqdm(titles, leave=False):
             try:
                 # text pre-processing
+                title = htmlTags(title)
                 title = re.sub("\n", " ", title)
                 title = re.sub("[\r|\t|\x0c|\d+]", "", title)  # noqa: W605
-                title = re.sub("[.,]", "", title)
                 title = re.sub("\\\'s", "'s", title)
                 title = title.lower()
 
                 doc = nlp(title)
 
                 tokens_without_sw = ' '.join([t.lemma_ for t in doc if not t.is_stop])
 
@@ -189,22 +191,22 @@
             except ValueError:
                 raise
         dfCluster = pd.concat(clusterdf, ignore_index=True)
         basedf = self.clusternodes.query('cluster == @cluster')
         inputnodes = set(basedf.node.values)
         notFound = inputnodes.difference(set(dfCluster[self.publicationIDcolumn].values))
         topAuthors = Counter(
-            [x for y in [x.split(';') for x in dfCluster[self.authorColumnName].fillna('').values] for x in y]
+            [x for y in dfCluster[self.authorColumnName].fillna('').values for x in y]
         ).most_common(21)
         authortext = ''
         for x in topAuthors:
             if x[0] != '':
                 authortext += f'\t{x[0]}: {x[1]}\n'
         topAffils = Counter(
-            [x for y in [x.split(';') for x in dfCluster[self.affiliationColumnName].fillna('').values] for x in y]
+            [x for y in dfCluster[self.affiliationColumnName].fillna('').values for x in y]
         ).most_common(21)
         affiltext = ''
         for x in topAffils:
             if x[0] != '':
                 affiltext += f'\t{x[0]}: {x[1]}\n'
         print(f'\tFinished base report for cluster {cluster}.')
         corpus = self.create_corpus(dfCluster)
@@ -263,15 +265,15 @@
 
         For all files in the metadata path, call `_mergeData` if the found
         year in the filename falls in the bounds.
 
         This step needs to be run once, the all cluster metadata is generated
         and can be reused.
         """
-        filenames = os.listdir(self.metadatapath)
+        filenames = [x for x in os.listdir(self.metadatapath) if x.endswith("json")]
         yearFiles = []
         for x in filenames:
             try:
                 year = int(re.findall(r'\d{4}', x)[0])
             except Exception:
                 raise
             if self.timerange[0] <= year <= self.timerange[1]:
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/linkage/wordscore.py` & `semanticlayertools-0.2.2/src/semanticlayertools/linkage/wordscore.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/metric/centralities.py` & `semanticlayertools-0.2.2/src/semanticlayertools/metric/centralities.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,15 @@
         self, centrality: str = "all",
         timerange: tuple = (1945, 2005), useGC: bool = True
     ):
         """Run calculation based on Pajek or NCol network data.
 
         By default timerange is limited to 1945 to 2005. Change accordingly.
         For centralities choose "all" or one of the following:
-            "authority"
-            "betweenness"
-            "closeness"
-            "degree"
+        "authority", "betweenness", "closeness", "degree"
         """
         self.centralities = {}
         self.timerange = timerange
         bins = 10 ** np.linspace(np.log10(0.00001), np.log10(1.0), 100)
         binsNormal = np.linspace(0, 1, 100)
         with open(f'{self.outPath}centralities_logbin.csv', 'a') as result:
             for year in tqdm(self.timerange):
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/metric/linguistic.py` & `semanticlayertools-0.2.2/src/semanticlayertools/metric/linguistic.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/pipelines/cocitetimeclusters.py` & `semanticlayertools-0.2.2/src/semanticlayertools/pipelines/cocitetimeclusters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 
 import time
 import os
 import multiprocessing
 
-from ..linkage.cocitation import Cocitations
+from ..linkage.citation import Couplings
 from ..clustering.leiden import TimeCluster
 from ..clustering.reports import ClusterReports
 
 num_processes = multiprocessing.cpu_count()
 
 
 def run(
     inputFilepath: str,
     outputPath: str,
     resolution: float,
     intersliceCoupling: float,
+    inputFileType: str = "files",
     minClusterSize: int = 1000,
     timerange: tuple = (1945, 2005),
+    timeWindow: int = 3,
+    pubIDColumnName: str = "nodeID",
     referenceColumnName: str = 'reference',
+    yearColumnName: str = "year",
     numberproc: int = num_processes,
     limitRefLength: bool = False,
+    useGC: bool = True,
+    skipCocite: bool = False,
     debug: bool = False
 ):
     """Runs all steps of the temporal clustering pipepline.
 
     Creates cocitation networks, finds temporal clusters, writes report files
     for large clusters.
 
@@ -31,59 +37,74 @@
     1000 nodes. Lists of references are assumed to be contained in column
     "reference".
 
     By default this routine takes all available cpu cores. Limit this
     to a lower value to allow parallel performance of other tasks.
 
     :param inputFilepath:  Path to corpora input data
-    :type text: str
+    :type inputFilepath: str
+    :param inputFileType:  Type of input data (files or dataframe, default: files)
+    :type inputFileType: str
     :param cociteOutpath: Output path for cocitation networks
-    :type text: str
+    :type cociteOutpath: str
     :param timeclusterOutpath: Output path for time clusters
-    :type text: str
+    :type timeclusterOutpath: str
     :param reportsOutpath: Output path for reports
-    :type text: str
+    :type reportsOutpath: str
     :param resolution: Main parameter for the clustering quality function (Constant Pots Model)
     :type resolution: float
     :param intersliceCoupling: Coupling parameter between two year slices, also influences cluster detection
     :type intersliceCoupling: float
     :param minClusterSize: The minimal cluster size, above which clusters are considered (default=1000)
     :type minClusterSize: int
     :param timerange: Time range to evalute clusters for (usefull for limiting computation time, default = (1945, 2005))
     :type timerange: tuple
+    :param timeWindow: Time window to join publications into (default: 3)
+    :type timeWindow: int
+    :param pubIDColumnName: Column name containing the IDs of publications
+    :type pubIDColumnName: str
+    :param referenceColumnName: Column name containing the references of a publication
+    :type referenceColumnName: str
+    :param yearColumnName: Column name containing the publiction year in integer format
+    :type yearColumnName: str
     :param referenceColumnName: Column name containing the references of a publication
     :type referenceColumnName: str
     :param numberProc: Number of CPUs the package is allowed to use (default=all)
     :type numberProc: int
     :param limitRefLength: Either False or integer giving the maximum number of references a considered publication is allowed to contain
     :type limitRefLength: bool or int
     """
     for subdir in ["cociteGraphs", "timeClusters", "reports"]:
-        os.makedirs(os.path.join(outputPath, subdir))
+        os.makedirs(os.path.join(outputPath, subdir), exist_ok=True)
     
     starttime = time.time()
-    cocites = Cocitations(
-        inpath=inputFilepath,
-        outpath=os.path.join(outputPath, "cociteGraphs"),
-        columnName=referenceColumnName,
-        numberProc=numberproc,
-        limitRefLength=limitRefLength,
-        timerange=timerange,
-        debug=debug
-    )
-    cocites.processFolder()
+    if skipCocite is False:
+        cocites = Couplings(
+            inpath=inputFilepath,
+            inputType=inputFileType,
+            outpath=os.path.join(outputPath, "cociteGraphs"),
+            pubIDColumn=pubIDColumnName,
+            referenceColumn=referenceColumnName,
+            dateColumn=yearColumnName,
+            numberProc=numberproc,
+            limitRefLength=limitRefLength,
+            timerange=timerange,
+            timeWindow=timeWindow,
+            debug=debug
+        )
+        cocites.getCocitationCoupling()
     timeclusters = TimeCluster(
         inpath=os.path.join(outputPath, "cociteGraphs"),
         outpath=os.path.join(outputPath, "timeClusters"),
         resolution=resolution,
         intersliceCoupling=intersliceCoupling,
         timerange=timerange,
-        debug=debug
+        useGC=useGC
     )
-    timeclfile, _ = timeclusters.optimize()
+    timeclfile, _ = timeclusters.optimize(minClusterSize)
     clusterreports = ClusterReports(
         infile=timeclfile,
         metadatapath=inputFilepath,
         outpath=os.path.join(outputPath, "reports"),
         numberProc=numberproc,
         minClusterSize=minClusterSize,
         timerange=(timerange[0], timerange[1] + 3)
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/pipelines/wordscorenet.py` & `semanticlayertools-0.2.2/src/semanticlayertools/pipelines/wordscorenet.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/visual/citationnet.py` & `semanticlayertools-0.2.2/src/semanticlayertools/visual/citationnet.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,17 +71,17 @@
         except TypeError:
             forcodes = '00:1.00'
         return forcodes
 
     def _editDF(self, inputdf, dftype='cite_l1', level2List=None):
         """Return reformated dataframe. """
         retCols = ['source', 'target', 'doi', 'year', 'title', 'times_cited', 'forcodes', 'level', 'is_input']
-        formatedFOR = inputdf.category_for.apply(lambda row: self._formatFOR(row))
+        formatedFOR = inputdf.category_for_2008.apply(lambda row: self._formatFOR(row))
         inputdf.insert(0, 'forcodes', formatedFOR)
-        inputdf.drop(['category_for'], axis=1, inplace=True)
+        inputdf.drop(['category_for_2008'], axis=1, inplace=True)
         inputdf.rename(columns={'id': 'source'}, inplace=True)
         if dftype in ['ref_l1', 'cite_l2', 'ref_l2']:
             outdf = inputdf.explode('reference_ids')
             outdf.rename(columns={'reference_ids': 'target'}, inplace=True)
             if dftype == 'cite_l2':
                 outdf = outdf.query('target.isin(@level2List)')
         elif dftype == 'cite_l1':
@@ -100,42 +100,42 @@
         return outdf[retCols]
 
     def _getMissing(self, idlist):
         """Get metadata for second level reference nodes."""
         retCols = ['source', 'doi', 'year', 'title', 'times_cited', 'forcodes', 'level', 'is_input']
         dfList = []
         if len(idlist) > 512:
-            for partlist in tqdm(np.array_split(idlist, round(len(idlist)/400))):
+            for partlist in tqdm(np.array_split(idlist, round(len(idlist) / 400))):
                 res = self.dsl.query_iterative(
                     f"""search
                           publications
                         where
                           id in {json.dumps(list(partlist))}
                         return
-                          publications[id+doi+times_cited+category_for+title+year]
+                          publications[id+doi+times_cited+category_for_2008+title+year]
                     """,
                     verbose=self._verbose
                 )
                 dfList.append(res.as_dataframe())
             retDF = pd.concat(dfList)
         else:
             res = self.dsl.query_iterative(
                 f"""search
                       publications
                     where
                       id in {json.dumps(list(idlist))}
                     return
-                      publications[id+doi+times_cited+category_for+title+year]
+                      publications[id+doi+times_cited+category_for_2008+title+year]
                 """,
                 verbose=self._verbose
             )
             retDF = res.as_dataframe()
-        formatedFOR = retDF.category_for.apply(lambda row: self._formatFOR(row))
+        formatedFOR = retDF.category_for_2008.apply(lambda row: self._formatFOR(row))
         retDF.insert(0, 'forcodes', formatedFOR)
-        retDF.drop(['category_for'], axis=1, inplace=True)
+        retDF.drop(['category_for_2008'], axis=1, inplace=True)
         retDF.rename(columns={'id': 'source'}, inplace=True)
         retDF.insert(0, 'level', 'ref_l3')
         retDF.insert(0, 'is_input', False)
         cleantitle = retDF.title.apply(lambda row: self._cleanTitleString(row))
         retDF.drop('title', axis=1, inplace=True)
         retDF.insert(0, 'title', cleantitle)
         return retDF[retCols]
@@ -147,15 +147,15 @@
         starttime = time.time()
         doi2id = self.dsl.query(
             f"""search
                   publications
                 where
                   doi = "{startDoi}"
                 return
-                  publications[id+authors+doi+times_cited+category_for+title+year+reference_ids]
+                  publications[id+authors+doi+times_cited+category_for_2008+title+year+reference_ids]
             """,
             verbose=self._verbose
         )
         querydf = doi2id.as_dataframe()
         if querydf.shape[0] == 0:
             return f"The dataset contains no entry for {startDoi}."
         elif querydf['times_cited'].iloc[0] >= self.citationLimit:
@@ -178,40 +178,40 @@
         ref1trgtList = list(self.dataframeList[0].target.values)
         cit1df = self.dsl.query_iterative(
             f"""search
                   publications
                 where
                   reference_ids = "{self.pubids}"
                 return
-                  publications[id+doi+times_cited+category_for+title+year+reference_ids]
+                  publications[id+doi+times_cited+category_for_2008+title+year+reference_ids]
             """,
             verbose=self._verbose)
         self.dataframeList.append(
             self._editDF(cit1df.as_dataframe(), dftype='cite_l1')
         )
         cit1SrcList = list(self.dataframeList[1].source.values)
         cit2df = self.dsl.query_iterative(
             f"""search
                   publications
                 where
                   reference_ids in {json.dumps(cit1SrcList)}
                 return
-                  publications[id+doi+times_cited+category_for+title+year+reference_ids]""",
+                  publications[id+doi+times_cited+category_for_2008+title+year+reference_ids]""",
             verbose=self._verbose
         )
         self.dataframeList.append(
             self._editDF(cit2df.as_dataframe(), dftype='cite_l2', level2List=cit1SrcList)
         )
         ref2df = self.dsl.query_iterative(
             f"""search
                   publications
                 where
                   id in {json.dumps(ref1trgtList)}
                 return
-                  publications[id+doi+times_cited+category_for+title+year+reference_ids]""",
+                  publications[id+doi+times_cited+category_for_2008+title+year+reference_ids]""",
             verbose=self._verbose
         )
         self.dataframeList.append(
             self._editDF(ref2df.as_dataframe(), dftype='ref_l2')
         )
         print(f'Finished queries in {time.time() - starttime} seconds.')
         return self
@@ -235,37 +235,35 @@
         )
         nodedata = nodeMetadata.source.unique()
         # dflinks = dflinks.query('~target.isin(@nodedata) or ~source.isin(@nodedata)')
         for idx, row in nodeMetadata.fillna('').iterrows():
             outformat['nodes'].append(
                 {
                     'id': row['source'],
-                    'attributes':
-                        {
-                            "title": row['title'],
-                            "doi": row["doi"],
-                            "nodeyear": row["year"],
-                            "ref-by-count": row["times_cited"],
-                            "is_input_DOI": row['is_input'],
-                            "category_for": row["forcodes"],
-                            'level': row['level']
-                        }
+                    'attributes': {
+                        "title": row['title'],
+                        "doi": row["doi"],
+                        "nodeyear": row["year"],
+                        "ref-by-count": row["times_cited"],
+                        "is_input_DOI": row['is_input'],
+                        "category_for": row["forcodes"],
+                        'level': row['level']
+                    }
                 }
             )
         for idx, row in dflinks.fillna('').iterrows():
             if row['source'] in nodedata and row['target'] in nodedata:
                 outformat['edges'].append(
                     {
                         'source': row['source'],
                         'target': row['target'],
-                        'attributes':
-                            {
-                                'year': row['year'],
-                                'level': row['level']
-                            }
+                        'attributes': {
+                            'year': row['year'],
+                            'level': row['level']
+                        }
                     }
                 )
         doiname = self.startDoi
         firstauthor = self.firstAuthor
         for key, val in self.stringClean.items():
             doiname = re.sub(key, val, doiname)
             firstauthor = re.sub(key, val, firstauthor)
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/visual/embedding.py` & `semanticlayertools-0.2.2/src/semanticlayertools/visual/embedding.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools/visual/utils.py` & `semanticlayertools-0.2.2/src/semanticlayertools/visual/utils.py`

 * *Files identical despite different names*

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools.egg-info/PKG-INFO` & `semanticlayertools-0.2.2/src/semanticlayertools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticlayertools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create semantic layers using different methods for word linking.
 Home-page: https://gitlab.gwdg.de/modelsen/semanticlayertools
 Author: Malte Vogl
 Author-email: mvogl@mpiwg-berlin.mpg.de
 Project-URL: Project Home, https://modelsen.mpiwg-berlin.mpg.de
 Project-URL: Bug Tracker, https://gitlab.gwdg.de/modelsen/semanticlayertools/-/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,20 +14,24 @@
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: embeddml
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
+<img src="https://img.shields.io/badge/DHCodeReview-passed-brightgreen" alt="DHCodeReview" style="float: left; margin-right: 10px;" />[Review](https://github.com/DHCodeReview/DHCodeReview/issues/1)
+
 ## SemanticLayerTools
 
 Collects tools to create semantic layers in the socio-epistemic networks framework. Source material can be any structured corpus with metadata of authors, time, and at least one text column.
 
 Documentation is available on [ReadTheDocs](https://semanticlayertools.readthedocs.io/).
 
+Part of the code was reviewed by [Itay Zandbank](https://github.com/zmbq), thank you. 
+
 ## Installation
 
 tl;dr Use pip
 
 ~~~bash
 pip install semanticlayertools
 ~~~
```

### Comparing `semanticlayertools-0.2.1/src/semanticlayertools.egg-info/SOURCES.txt` & `semanticlayertools-0.2.2/src/semanticlayertools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 src/semanticlayertools/cleaning/__init__.py
 src/semanticlayertools/cleaning/text.py
 src/semanticlayertools/clustering/__init__.py
 src/semanticlayertools/clustering/infomap.py
 src/semanticlayertools/clustering/leiden.py
 src/semanticlayertools/clustering/reports.py
 src/semanticlayertools/linkage/__init__.py
-src/semanticlayertools/linkage/cocitation.py
+src/semanticlayertools/linkage/citation.py
+src/semanticlayertools/linkage/worddistributions.py
 src/semanticlayertools/linkage/wordscore.py
 src/semanticlayertools/metric/__init__.py
 src/semanticlayertools/metric/centralities.py
 src/semanticlayertools/metric/linguistic.py
 src/semanticlayertools/pipelines/__init__.py
 src/semanticlayertools/pipelines/cocitetimeclusters.py
 src/semanticlayertools/pipelines/wordscorenet.py
 src/semanticlayertools/visual/__init__.py
 src/semanticlayertools/visual/citationnet.py
 src/semanticlayertools/visual/embedding.py
+src/semanticlayertools/visual/plotting.py
 src/semanticlayertools/visual/utils.py
```

