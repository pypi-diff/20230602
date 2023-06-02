# Comparing `tmp/telegramweb-4.0.tar.gz` & `tmp/telegramweb-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramweb-4.0.tar", last modified: Fri Jun  2 10:59:11 2023, max compression
+gzip compressed data, was "telegramweb-4.1.tar", last modified: Fri Jun  2 11:07:28 2023, max compression
```

## Comparing `telegramweb-4.0.tar` & `telegramweb-4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:59:11.072016 telegramweb-4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 10:58:52.000000 telegramweb-4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 10:58:52.000000 telegramweb-4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-06-02 10:59:11.072016 telegramweb-4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-02 10:58:52.000000 telegramweb-4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:59:11.072016 telegramweb-4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-02 10:58:52.000000 telegramweb-4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:59:11.072016 telegramweb-4.0/telegram_news/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/displaypolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:59:11.072016 telegramweb-4.0/telegram_news/template/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/template/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-02 10:58:52.000000 telegramweb-4.0/telegram_news/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:59:11.072016 telegramweb-4.0/telegramweb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10319 2023-06-02 10:59:11.000000 telegramweb-4.0/telegramweb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 10:59:11.000000 telegramweb-4.0/telegramweb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:59:11.000000 telegramweb-4.0/telegramweb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 10:59:11.000000 telegramweb-4.0/telegramweb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 10:59:11.000000 telegramweb-4.0/telegramweb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-02 11:07:12.000000 telegramweb-4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 11:07:12.000000 telegramweb-4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-02 11:07:28.294269 telegramweb-4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-02 11:07:12.000000 telegramweb-4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:07:28.294269 telegramweb-4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:07:12.000000 telegramweb-4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegram_news/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/displaypolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegram_news/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44162 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/template/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17293 2023-06-02 11:07:12.000000 telegramweb-4.1/telegram_news/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:07:28.294269 telegramweb-4.1/telegramweb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 11:07:28.000000 telegramweb-4.1/telegramweb.egg-info/top_level.txt
```

### Comparing `telegramweb-4.0/LICENSE` & `telegramweb-4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/PKG-INFO` & `telegramweb-4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.0
+Version: 4.1
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
 Classifier: Topic :: Office/Business :: News/Diary
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
   <br>Telegram-news<br>
 </h1>
```

### Comparing `telegramweb-4.0/README.md` & `telegramweb-4.1/README.md`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/setup.py` & `telegramweb-4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 ]
 
 DESCRIPTION = 'Python package for automatically fetching and pushing news by Telegram.'
 LONG_DESCRIPTION = open("README.md").read()
 
 setup(
     name='telegramweb',
-    version='4.0',
+    version='4.1',
     author='craziks',
     author_email='chandrashekharpanday07@gmail.com',
     url='https://github.com/craziks-creator/telegram-web',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
-    python_requires='>=3.5',
+    python_requires='>=3.8',
     install_requires=requires,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.8",
         "Intended Audience :: Developers",
         "Topic :: Education",
         "Topic :: Office/Business :: News/Diary",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `telegramweb-4.0/telegram_news/__init__.py` & `telegramweb-4.1/telegram_news/__init__.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegram_news/constant.py` & `telegramweb-4.1/telegram_news/constant.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegram_news/displaypolicy.py` & `telegramweb-4.1/telegram_news/displaypolicy.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegram_news/ratelimit.py` & `telegramweb-4.1/telegram_news/ratelimit.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegram_news/template/common.py` & `telegramweb-4.1/telegram_news/template/common.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegram_news/utils.py` & `telegramweb-4.1/telegram_news/utils.py`

 * *Files identical despite different names*

### Comparing `telegramweb-4.0/telegramweb.egg-info/PKG-INFO` & `telegramweb-4.1/telegramweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: telegramweb
-Version: 4.0
+Version: 4.1
 Summary: Python package for automatically fetching and pushing news by Telegram.
 Home-page: https://github.com/craziks-creator/telegram-web
 Author: craziks
 Author-email: chandrashekharpanday07@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Education
 Classifier: Topic :: Office/Business :: News/Diary
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/ESWZY/telegram-news/master/docs/images/banner.png" alt="Telegram-news">
   <br>Telegram-news<br>
 </h1>
```

