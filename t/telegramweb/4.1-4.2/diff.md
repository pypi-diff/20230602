# Comparing `tmp/telegramweb-4.1.tar.gz` & `tmp/telegramweb-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-4.1.tar", last modified: Fri Jun  2 11:07:28 2023, max compression
+gzip compressed data, was "telegramweb-4.2.tar", last modified: Fri Jun  2 11:21:12 2023, max compression
```

## Comparing `telegramweb-4.1.tar` & `telegramweb-4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 11:07:12.000000 telegramweb-4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 11:07:12.000000 telegramweb-4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-02 11:07:28.294269 telegramweb-4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-02 11:07:12.000000 telegramweb-4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:07:28.294269 telegramweb-4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:07:12.000000 telegramweb-4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:21:12.850451 telegramweb-4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 11:20:55.000000 telegramweb-4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 11:20:55.000000 telegramweb-4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-02 11:21:12.850451 telegramweb-4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-02 11:20:55.000000 telegramweb-4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:21:12.850451 telegramweb-4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-02 11:20:55.000000 telegramweb-4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:21:12.850451 telegramweb-4.2/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:21:12.850451 telegramweb-4.2/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-02 11:20:55.000000 telegramweb-4.2/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:21:12.850451 telegramweb-4.2/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-06-02 11:21:12.000000 telegramweb-4.2/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 11:21:12.000000 telegramweb-4.2/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:21:12.000000 telegramweb-4.2/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 11:21:12.000000 telegramweb-4.2/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:21:12.000000 telegramweb-4.2/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-4.1/LICENSE` & `telegramweb-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/PKG-INFO` & `telegramweb-4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.1
+Version: 4.2
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
@@ -285,9 +284,7 @@
 Feel free to contact with me if you have any question. Also welcome any contribute.
 
 If you build a channel by this, don't forget to share that good news with us!
 
 ## License
 
 Licensed under the MIT License.
-
-
```

### Comparing `telegramweb-4.1/README.md` & `telegramweb-4.2/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/setup.py` & `telegramweb-4.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup, find_packages
 
 requires = [
     'requests',
     'SQLAlchemy',
     'beautifulsoup4',
-    'psycopg2',
+    'psycopg2-binary',
     'lxml',
     'xmltodict',
+    'postgresql'
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='4.1',
+    version='4.2',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `telegramweb-4.1/telegram_news/__init__.py` & `telegramweb-4.2/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegram_news/constant.py` & `telegramweb-4.2/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegram_news/displaypolicy.py` & `telegramweb-4.2/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegram_news/ratelimit.py` & `telegramweb-4.2/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegram_news/template/common.py` & `telegramweb-4.2/telegram_news/template/common.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegram_news/utils.py` & `telegramweb-4.2/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.1/telegramweb.egg-info/PKG-INFO` & `telegramweb-4.2/telegramweb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.1
+Version: 4.2
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
@@ -285,9 +284,7 @@
 Feel free to contact with me if you have any question. Also welcome any contribute.
 
 If you build a channel by this, don't forget to share that good news with us!
 
 ## License
 
 Licensed under the MIT License.
-
-
```

