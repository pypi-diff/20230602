# Comparing `tmp/T3SF-2.1.tar.gz` & `tmp/T3SF-2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T3SF-2.1.tar", last modified: Fri Jun  2 16:46:11 2023, max compression
+gzip compressed data, was "T3SF-2.1rc1.tar", last modified: Fri Jun  2 16:39:23 2023, max compression
```

## Comparing `T3SF-2.1.tar` & `T3SF-2.1rc1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.1/LICENSE
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.1/MANIFEST.in
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4745 2023-06-02 16:46:11.251280 T3SF-2.1/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-05-30 14:58:35.000000 T3SF-2.1/README.md
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-06-02 16:46:11.251280 T3SF-2.1/setup.cfg
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1124 2023-06-02 16:46:00.000000 T3SF-2.1/setup.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.247280 T3SF-2.1/src/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14869 2023-06-02 16:18:59.000000 T3SF-2.1/src/T3SF/T3SF.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/__init__.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/discord/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/discord/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-02 15:53:09.000000 T3SF-2.1/src/T3SF/discord/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10375 2023-06-02 16:23:53.000000 T3SF-2.1/src/T3SF/discord/discord.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/gui/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/gui/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4987 2023-06-02 16:22:50.000000 T3SF-2.1/src/T3SF/gui/core.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/gui/templates/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-05-30 15:48:00.000000 T3SF-2.1/src/T3SF/gui/templates/base.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/gui/templates/env_creation.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     8065 2023-06-02 16:23:01.000000 T3SF-2.1/src/T3SF/gui/templates/index.html
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/gui/templates/msel_viewer.html
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/logger/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/logger/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/logger/logger.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF/slack/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-05-30 14:58:35.000000 T3SF-2.1/src/T3SF/slack/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-05-30 16:20:25.000000 T3SF-2.1/src/T3SF/slack/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11646 2023-06-02 16:23:56.000000 T3SF-2.1/src/T3SF/slack/slack.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      682 2023-06-02 16:25:20.000000 T3SF-2.1/src/T3SF/utils.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:46:11.251280 T3SF-2.1/src/T3SF.egg-info/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4745 2023-06-02 16:46:11.000000 T3SF-2.1/src/T3SF.egg-info/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      665 2023-06-02 16:46:11.000000 T3SF-2.1/src/T3SF.egg-info/SOURCES.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-06-02 16:46:11.000000 T3SF-2.1/src/T3SF.egg-info/dependency_links.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-06-02 16:46:11.000000 T3SF-2.1/src/T3SF.egg-info/requires.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-06-02 16:46:11.000000 T3SF-2.1/src/T3SF.egg-info/top_level.txt
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.1rc1/LICENSE
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.1rc1/MANIFEST.in
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.409754 T3SF-2.1rc1/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-05-30 14:58:35.000000 T3SF-2.1rc1/README.md
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-06-02 16:39:23.409754 T3SF-2.1rc1/setup.cfg
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-06-02 16:38:11.000000 T3SF-2.1rc1/setup.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.405754 T3SF-2.1rc1/src/T3SF/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14869 2023-06-02 16:18:59.000000 T3SF-2.1rc1/src/T3SF/T3SF.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/__init__.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/discord/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/discord/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7356 2023-06-02 15:53:09.000000 T3SF-2.1rc1/src/T3SF/discord/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10375 2023-06-02 16:23:53.000000 T3SF-2.1rc1/src/T3SF/discord/discord.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4987 2023-06-02 16:22:50.000000 T3SF-2.1rc1/src/T3SF/gui/core.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/gui/templates/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-05-30 15:48:00.000000 T3SF-2.1rc1/src/T3SF/gui/templates/base.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     8065 2023-06-02 16:23:01.000000 T3SF-2.1rc1/src/T3SF/gui/templates/index.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/gui/templates/msel_viewer.html
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/logger/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/logger/logger.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF/slack/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-05-30 14:58:35.000000 T3SF-2.1rc1/src/T3SF/slack/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7129 2023-05-30 16:20:25.000000 T3SF-2.1rc1/src/T3SF/slack/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    11646 2023-06-02 16:23:56.000000 T3SF-2.1rc1/src/T3SF/slack/slack.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      682 2023-06-02 16:25:20.000000 T3SF-2.1rc1/src/T3SF/utils.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-06-02 16:39:23.409754 T3SF-2.1rc1/src/T3SF.egg-info/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      665 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/requires.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-06-02 16:39:23.000000 T3SF-2.1rc1/src/T3SF.egg-info/top_level.txt
```

### Comparing `T3SF-2.1/LICENSE` & `T3SF-2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/PKG-INFO` & `T3SF-2.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.1
+Version: 2.1rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.1/README.md` & `T3SF-2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/setup.py` & `T3SF-2.1rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="T3SF",
-    version="2.1",
+    version="2.1-rc1",
     author="BASE4 Security",
     author_email="jlanfranconi@base4sec.com",
     description="Technical Tabletop Exercises Simulation Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Base4Security/T3SF",
     project_urls={
```

### Comparing `T3SF-2.1/src/T3SF/T3SF.py` & `T3SF-2.1rc1/src/T3SF/T3SF.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/discord/bot.py` & `T3SF-2.1rc1/src/T3SF/discord/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/discord/discord.py` & `T3SF-2.1rc1/src/T3SF/discord/discord.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/gui/core.py` & `T3SF-2.1rc1/src/T3SF/gui/core.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/gui/templates/base.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/gui/templates/env_creation.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/env_creation.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/gui/templates/index.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/index.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/gui/templates/msel_viewer.html` & `T3SF-2.1rc1/src/T3SF/gui/templates/msel_viewer.html`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/logger/logger.py` & `T3SF-2.1rc1/src/T3SF/logger/logger.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/slack/bot.py` & `T3SF-2.1rc1/src/T3SF/slack/bot.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/slack/slack.py` & `T3SF-2.1rc1/src/T3SF/slack/slack.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF/utils.py` & `T3SF-2.1rc1/src/T3SF/utils.py`

 * *Files identical despite different names*

### Comparing `T3SF-2.1/src/T3SF.egg-info/PKG-INFO` & `T3SF-2.1rc1/src/T3SF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 2.1
+Version: 2.1rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 2.1 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.1rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
```

### Comparing `T3SF-2.1/src/T3SF.egg-info/SOURCES.txt` & `T3SF-2.1rc1/src/T3SF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

