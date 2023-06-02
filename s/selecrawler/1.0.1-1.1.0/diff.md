# Comparing `tmp/SeleCrawler-1.0.1.tar.gz` & `tmp/selecrawler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeleCrawler-1.0.1.tar", last modified: Fri Jun  2 19:23:56 2023, max compression
+gzip compressed data, was "selecrawler-1.1.0.tar", last modified: Fri Jun  2 19:44:38 2023, max compression
```

## Comparing `SeleCrawler-1.0.1.tar` & `selecrawler-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.481648 SeleCrawler-1.0.1/
--rw-rw-rw-   0        0        0      393 2023-06-02 19:23:56.481648 SeleCrawler-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.403524 SeleCrawler-1.0.1/SeleCrawler.egg-info/
--rw-rw-rw-   0        0        0      393 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-06-02 19:23:55.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-02 19:23:54.000000 SeleCrawler-1.0.1/SeleCrawler.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 19:23:56.466028 SeleCrawler-1.0.1/selecrawler/
--rw-rw-rw-   0        0        0       37 2023-03-24 07:37:15.000000 SeleCrawler-1.0.1/selecrawler/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-06-02 19:22:35.000000 SeleCrawler-1.0.1/selecrawler/browsing.py
--rw-rw-rw-   0        0        0     7871 2023-06-02 19:12:37.000000 SeleCrawler-1.0.1/selecrawler/controller.py
--rw-rw-rw-   0        0        0       42 2023-06-02 19:23:56.512895 SeleCrawler-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      680 2023-06-02 18:19:24.000000 SeleCrawler-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:44:38.616074 selecrawler-1.1.0/
+-rw-rw-rw-   0        0        0      393 2023-06-02 19:44:38.584828 selecrawler-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 19:44:38.506703 selecrawler-1.1.0/SeleCrawler.egg-info/
+-rw-rw-rw-   0        0        0      393 2023-06-02 19:44:36.000000 selecrawler-1.1.0/SeleCrawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-06-02 19:44:37.000000 selecrawler-1.1.0/SeleCrawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:44:36.000000 selecrawler-1.1.0/SeleCrawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-06-02 19:44:36.000000 selecrawler-1.1.0/SeleCrawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 19:44:36.000000 selecrawler-1.1.0/SeleCrawler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 19:44:38.553712 selecrawler-1.1.0/selecrawler/
+-rw-rw-rw-   0        0        0       50 2023-06-02 19:43:00.000000 selecrawler-1.1.0/selecrawler/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-06-02 19:22:35.000000 selecrawler-1.1.0/selecrawler/browsing.py
+-rw-rw-rw-   0        0        0     7881 2023-06-02 19:41:38.000000 selecrawler-1.1.0/selecrawler/controller.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:44:38.662948 selecrawler-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      680 2023-06-02 19:44:06.000000 selecrawler-1.1.0/setup.py
```

### Comparing `SeleCrawler-1.0.1/selecrawler/browsing.py` & `selecrawler-1.1.0/selecrawler/browsing.py`

 * *Files identical despite different names*

### Comparing `SeleCrawler-1.0.1/selecrawler/controller.py` & `selecrawler-1.1.0/selecrawler/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     pass
 
 
 def logg(msg, color):
     # debg('='*50)
     # debg(msg)
     # debg('='*50)
+    pass
 
 
 def proxies_plugin(username, proxypass, endpoint, port):
     manifest_json = """
     {
         "version": "1.0.0",
         "manifest_version": 2,
```

### Comparing `SeleCrawler-1.0.1/setup.py` & `selecrawler-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup_args = dict(
-    name='SeleCrawler',
-    version='1.0.1',
+    name='selecrawler',
+    version='1.1.0',
     description='Collection Of Tools To Ease Selenium Operation',
     packages=find_packages(),
     author='Gee Tech Labs',
     author_email='geetechlabs@gmail.com',
     keywords=['SeleCrawler', 'Sele Crawler', 'Selenium Crawler', 'Selenium', 'Crawler', 'Browser', 'BrowserAutomation', 'Automation', 'Webdriver', 'web', 'driver', 'web driver']
 )
```

