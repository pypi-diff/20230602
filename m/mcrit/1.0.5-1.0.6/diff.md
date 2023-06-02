# Comparing `tmp/mcrit-1.0.5.tar.gz` & `tmp/mcrit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.5.tar", last modified: Fri Jun  2 12:52:21 2023, max compression
+gzip compressed data, was "mcrit-1.0.6.tar", last modified: Fri Jun  2 13:44:05 2023, max compression
```

## Comparing `mcrit-1.0.5.tar` & `mcrit-1.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.536604 mcrit-1.0.5/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.5/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 12:52:21.536604 mcrit-1.0.5/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10783 2023-06-02 12:51:25.000000 mcrit-1.0.5/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.528604 mcrit-1.0.5/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.5/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.5/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.5/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.5/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-06-02 12:51:38.000000 mcrit-1.0.5/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.5/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.5/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.5/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.5/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.5/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.5/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.5/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.5/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.5/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.5/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.5/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.5/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.5/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.5/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.5/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.5/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.5/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.5/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.536604 mcrit-1.0.5/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.5/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.5/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.5/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.536604 mcrit-1.0.5/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.5/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.5/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.5/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.5/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25691 2023-06-02 12:31:24.000000 mcrit-1.0.5/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.5/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.5/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.5/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.5/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.5/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.5/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 12:52:21.532604 mcrit-1.0.5/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 12:52:21.000000 mcrit-1.0.5/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-06-02 12:52:21.000000 mcrit-1.0.5/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-06-02 12:52:21.000000 mcrit-1.0.5/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-06-02 12:52:21.000000 mcrit-1.0.5/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-06-02 12:52:21.000000 mcrit-1.0.5/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-06-02 12:52:21.536604 mcrit-1.0.5/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-06-02 12:50:32.000000 mcrit-1.0.5/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.467274 mcrit-1.0.6/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.6/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 13:44:05.467274 mcrit-1.0.6/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10783 2023-06-02 13:43:04.000000 mcrit-1.0.6/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.6/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.6/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.6/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.6/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-06-02 13:43:10.000000 mcrit-1.0.6/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.6/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.6/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.6/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.6/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.6/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.6/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.6/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.6/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.6/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.6/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.6/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.6/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.6/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.6/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.6/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.6/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.6/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.6/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25691 2023-06-02 12:31:24.000000 mcrit-1.0.6/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.6/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.6/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.6/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.6/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-06-02 13:44:05.467274 mcrit-1.0.6/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-06-02 13:43:00.000000 mcrit-1.0.6/setup.py
```

### Comparing `mcrit-1.0.5/LICENSE` & `mcrit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/PKG-INFO` & `mcrit-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.5
+Version: 1.0.6
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -121,15 +121,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
-         * 2023-06-02 v1.0.5: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
+         * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
          * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
```

### Comparing `mcrit-1.0.5/README.md` & `mcrit-1.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
- * 2023-06-02 v1.0.5: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
+ * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
  * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
  * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
```

### Comparing `mcrit-1.0.5/mcrit/Worker.py` & `mcrit-1.0.6/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/__main__.py` & `mcrit-1.0.6/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/client/McritClient.py` & `mcrit-1.0.6/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/client/McritConsole.py` & `mcrit-1.0.6/mcrit/client/McritConsole.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/config/ConfigInterface.py` & `mcrit-1.0.6/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/config/McritConfig.py` & `mcrit-1.0.6/mcrit/config/McritConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.5"
+    VERSION = "1.0.6"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.5/mcrit/config/MinHashConfig.py` & `mcrit-1.0.6/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/config/QueueConfig.py` & `mcrit-1.0.6/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.6/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/config/StorageConfig.py` & `mcrit-1.0.6/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/index/MinHashIndex.py` & `mcrit-1.0.6/mcrit/index/MinHashIndex.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/index/SearchCursor.py` & `mcrit-1.0.6/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.6/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.6/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/libs/mongoqueue.py` & `mcrit-1.0.6/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/libs/pymmh3.py` & `mcrit-1.0.6/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/libs/utility.py` & `mcrit-1.0.6/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.6/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.6/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.6/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.6/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.6/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.6/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/minhash/MinHash.py` & `mcrit-1.0.6/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/minhash/MinHasher.py` & `mcrit-1.0.6/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.6/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/queue/LocalQueue.py` & `mcrit-1.0.6/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/queue/QueueFactory.py` & `mcrit-1.0.6/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.6/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/BlocksResource.py` & `mcrit-1.0.6/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/FamilyResource.py` & `mcrit-1.0.6/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/FunctionResource.py` & `mcrit-1.0.6/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/JobResource.py` & `mcrit-1.0.6/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/MatchResource.py` & `mcrit-1.0.6/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/QueryResource.py` & `mcrit-1.0.6/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/SampleResource.py` & `mcrit-1.0.6/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/StatusResource.py` & `mcrit-1.0.6/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/application_routes.py` & `mcrit-1.0.6/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/server/utils.py` & `mcrit-1.0.6/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.6/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.6/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.6/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.6/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.6/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MatchingCache.py` & `mcrit-1.0.6/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MatchingResult.py` & `mcrit-1.0.6/mcrit/storage/MatchingResult.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.6/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.6/mcrit/storage/MongoDbStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/SampleEntry.py` & `mcrit-1.0.6/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/StorageFactory.py` & `mcrit-1.0.6/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit/storage/StorageInterface.py` & `mcrit-1.0.6/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.6/mcrit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.5
+Version: 1.0.6
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -121,15 +121,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
-         * 2023-06-02 v1.0.5: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
+         * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
          * 2023-03-17 v0.23.0: It is now possible to query matches for single SmdaFunctions (synchronously).
```

### Comparing `mcrit-1.0.5/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.6/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.5/setup.py` & `mcrit-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "smda>=1.3.0",
     "tqdm",
     "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="1.0.5",
+    version="1.0.6",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

