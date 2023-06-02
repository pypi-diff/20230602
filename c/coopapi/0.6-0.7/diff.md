# Comparing `tmp/coopapi-0.6.tar.gz` & `tmp/coopapi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopapi-0.6.tar", last modified: Thu Apr 13 18:19:53 2023, max compression
+gzip compressed data, was "coopapi-0.7.tar", last modified: Fri Jun  2 15:26:46 2023, max compression
```

## Comparing `coopapi-0.6.tar` & `coopapi-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.108485 coopapi-0.6/
--rw-rw-rw-   0        0        0     2838 2023-04-13 18:19:53.107494 coopapi-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.096465 coopapi-0.6/coopapi/
--rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.6/coopapi/__init__.py
--rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.6/coopapi/apiShell.py
--rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.6/coopapi/enums.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.6/coopapi/errors.py
--rw-rw-rw-   0        0        0     4883 2023-04-13 18:18:49.000000 coopapi-0.6/coopapi/http_request.py
--rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.6/coopapi/http_request_handlers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:19:53.106494 coopapi-0.6/coopapi.egg-info/
--rw-rw-rw-   0        0        0     2838 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.6/coopapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      279 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-13 18:19:53.000000 coopapi-0.6/coopapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 18:19:53.108485 coopapi-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1237 2023-04-13 18:19:29.000000 coopapi-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.989445 coopapi-0.7/
+-rw-rw-rw-   0        0        0     2838 2023-06-02 15:26:46.988444 coopapi-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2087 2023-01-10 15:30:28.000000 coopapi-0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.960482 coopapi-0.7/coopapi/
+-rw-rw-rw-   0        0        0      312 2023-02-15 15:23:58.000000 coopapi-0.7/coopapi/__init__.py
+-rw-rw-rw-   0        0        0     9526 2023-02-15 15:26:46.000000 coopapi-0.7/coopapi/apiShell.py
+-rw-rw-rw-   0        0        0      214 2023-02-23 19:25:03.000000 coopapi-0.7/coopapi/enums.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopapi-0.7/coopapi/errors.py
+-rw-rw-rw-   0        0        0     4883 2023-04-13 18:18:49.000000 coopapi-0.7/coopapi/http_request.py
+-rw-rw-rw-   0        0        0     4598 2023-02-23 20:53:41.000000 coopapi-0.7/coopapi/http_request_handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:26:46.986444 coopapi-0.7/coopapi.egg-info/
+-rw-rw-rw-   0        0        0     2838 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-10 15:32:25.000000 coopapi-0.7/coopapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      279 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 15:26:46.000000 coopapi-0.7/coopapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 15:26:46.989445 coopapi-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1237 2023-06-02 15:26:42.000000 coopapi-0.7/setup.py
```

### Comparing `coopapi-0.6/PKG-INFO` & `coopapi-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.6
+Version: 0.7
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.6/README.md` & `coopapi-0.7/README.md`

 * *Files identical despite different names*

### Comparing `coopapi-0.6/coopapi/apiShell.py` & `coopapi-0.7/coopapi/apiShell.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.6/coopapi/http_request.py` & `coopapi-0.7/coopapi/http_request.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.6/coopapi/http_request_handlers.py` & `coopapi-0.7/coopapi/http_request_handlers.py`

 * *Files identical despite different names*

### Comparing `coopapi-0.6/coopapi.egg-info/PKG-INFO` & `coopapi-0.7/coopapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopapi
-Version: 0.6
+Version: 0.7
 Summary: Tools for setting up an API. Built on the FastAPI framework
 Home-page: https://github.com/tylertjburns/coopapi
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopapi-0.6/setup.py` & `coopapi-0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopapi',
-      version='0.06',
+      version='0.07',
       description='Tools for setting up an API. Built on the FastAPI framework',
       url='https://github.com/tylertjburns/coopapi',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.5",
```

