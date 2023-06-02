# Comparing `tmp/uium-0.3.5.tar.gz` & `tmp/uium-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uium-0.3.5.tar", max compression
+gzip compressed data, was "uium-0.3.6.tar", max compression
```

## Comparing `uium-0.3.5.tar` & `uium-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.5/LICENSE
--rw-r--r--   0        0        0     1478 2023-05-31 14:31:31.522383 uium-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.5/README.md
--rw-r--r--   0        0        0     1044 2023-05-31 14:31:44.340728 uium-0.3.5/uium/__init__.py
--rw-r--r--   0        0        0     1579 2023-05-30 16:23:02.395487 uium-0.3.5/uium/_auto_electron.py
--rw-r--r--   0        0        0     3242 2023-05-31 14:22:37.155376 uium-0.3.5/uium/_install_driver.py
--rw-r--r--   0        0        0       14 2023-05-30 15:45:01.782811 uium-0.3.5/uium/_mirror.py
--rw-r--r--   0        0        0      137 2023-05-30 16:24:23.007397 uium-0.3.5/uium/_uium.py
--rw-r--r--   0        0        0       14 2023-05-30 15:44:58.897076 uium-0.3.5/uium/_webdriver_manager.py
--rw-r--r--   0        0        0      914 2023-05-31 14:23:25.829837 uium-0.3.5/uium/selenium.py
--rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-03 00:20:26.000000 uium-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1478 2023-06-02 07:32:58.819073 uium-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      596 2023-05-30 02:29:40.011464 uium-0.3.6/README.md
+-rw-r--r--   0        0        0     1035 2023-06-02 07:33:26.354098 uium-0.3.6/uium/__init__.py
+-rw-r--r--   0        0        0     1579 2023-05-30 16:23:02.395487 uium-0.3.6/uium/_auto_electron.py
+-rw-r--r--   0        0        0     3242 2023-05-31 14:22:37.155376 uium-0.3.6/uium/_install_driver.py
+-rw-r--r--   0        0        0       14 2023-05-30 15:45:01.782811 uium-0.3.6/uium/_mirror.py
+-rw-r--r--   0        0        0      137 2023-05-30 16:24:23.007397 uium-0.3.6/uium/_uium.py
+-rw-r--r--   0        0        0       14 2023-05-30 15:44:58.897076 uium-0.3.6/uium/_webdriver_manager.py
+-rw-r--r--   0        0        0      914 2023-05-31 14:23:25.829837 uium-0.3.6/uium/selenium.py
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 uium-0.3.6/PKG-INFO
```

### Comparing `uium-0.3.5/LICENSE` & `uium-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uium-0.3.5/pyproject.toml` & `uium-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uium"
-version = "0.3.5"
+version = "0.3.6"
 description = "An interesting python package"
 authors = ["Mark Hoo <markhoo@foxmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/MarkHoo/uium"
 repository = "https://github.com/MarkHoo/uium"
 classifiers = [
@@ -33,13 +33,13 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MarkHoo/uium/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 undetected-chromedriver = "^3.4.7"
-selenium = "^4.9.1"
+selenium = "^4.0.0"
 webdriver-manager = "^3.8.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `uium-0.3.5/README.md` & `uium-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `uium-0.3.5/uium/__init__.py` & `uium-0.3.6/uium/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service as ChromiumService
 # webdriver manager modules
 from webdriver_manager.chrome import ChromeDriverManager
 from webdriver_manager.core.utils import ChromeType
 
 
-__all__ = ["_uium", "Chrome", "ChromeOptions", "webdriver", "Options", "ChromiumService", "ChromeDriverManager", "ChromeType"]
-__version__ = "v0.3.5"
+__all__ = ["Chrome", "ChromeOptions", "webdriver", "Options", "ChromiumService", "ChromeDriverManager", "ChromeType"]
+__version__ = "v0.3.6"
 
 
 """
 TODO:
 - 集成Chrome驱动管理
 - 集成隐藏Chrome指纹防反爬
 - 根据ip来自动选择最近的ChromeDriver镜像点
```

### Comparing `uium-0.3.5/uium/_auto_electron.py` & `uium-0.3.6/uium/_auto_electron.py`

 * *Files identical despite different names*

### Comparing `uium-0.3.5/uium/_install_driver.py` & `uium-0.3.6/uium/_install_driver.py`

 * *Files identical despite different names*

### Comparing `uium-0.3.5/uium/selenium.py` & `uium-0.3.6/uium/selenium.py`

 * *Files identical despite different names*

### Comparing `uium-0.3.5/PKG-INFO` & `uium-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uium
-Version: 0.3.5
+Version: 0.3.6
 Summary: An interesting python package
 Home-page: https://github.com/MarkHoo/uium
 License: Apache-2.0
 Author: Mark Hoo
 Author-email: markhoo@foxmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: selenium (>=4.9.1,<5.0.0)
+Requires-Dist: selenium (>=4.0.0,<5.0.0)
 Requires-Dist: undetected-chromedriver (>=3.4.7,<4.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/MarkHoo/uium/issues
 Project-URL: Repository, https://github.com/MarkHoo/uium
 Description-Content-Type: text/markdown
 
 # uium
```

