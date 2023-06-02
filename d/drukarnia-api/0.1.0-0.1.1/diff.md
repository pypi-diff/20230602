# Comparing `tmp/drukarnia-api-0.1.0.tar.gz` & `tmp/drukarnia-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drukarnia-api-0.1.0.tar", last modified: Fri Jun  2 04:29:38 2023, max compression
+gzip compressed data, was "dist/drukarnia-api-0.1.1.tar", last modified: Fri Jun  2 05:01:09 2023, max compression
```

## Comparing `drukarnia-api-0.1.0.tar` & `drukarnia-api-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 04:29:38.643619 drukarnia-api-0.1.0/
--rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia-api-0.1.0/LICENSE
--rw-r--r--   0 andrej5    (501) staff       (20)     1991 2023-06-02 04:29:38.643146 drukarnia-api-0.1.0/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)     1310 2023-06-02 04:14:32.000000 drukarnia-api-0.1.0/README.md
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 04:29:38.639264 drukarnia-api-0.1.0/drukarnia-api/
--rw-r--r--   0 andrej5    (501) staff       (20)       86 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/drukarnia-api/__init__.py
--rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/drukarnia-api/article.py
--rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/drukarnia-api/author.py
--rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/drukarnia-api/connection.py
--rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/drukarnia-api/drukarnia_api.py
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 04:29:38.642240 drukarnia-api-0.1.0/drukarnia_api.egg-info/
--rw-r--r--   0 andrej5    (501) staff       (20)     1991 2023-06-02 04:29:38.000000 drukarnia-api-0.1.0/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)      308 2023-06-02 04:29:38.000000 drukarnia-api-0.1.0/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 04:29:38.000000 drukarnia-api-0.1.0/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 04:29:38.000000 drukarnia-api-0.1.0/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 04:29:38.643906 drukarnia-api-0.1.0/setup.cfg
--rw-r--r--   0 andrej5    (501) staff       (20)     1293 2023-06-02 04:04:41.000000 drukarnia-api-0.1.0/setup.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:01:09.270351 drukarnia-api-0.1.1/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia-api-0.1.1/LICENSE
+-rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:01:09.270019 drukarnia-api-0.1.1/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)     1265 2023-06-02 04:59:01.000000 drukarnia-api-0.1.1/README.md
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:01:09.266828 drukarnia-api-0.1.1/drukarnia-api/
+-rw-r--r--   0 andrej5    (501) staff       (20)       86 2023-06-02 04:04:41.000000 drukarnia-api-0.1.1/drukarnia-api/__init__.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia-api-0.1.1/drukarnia-api/article.py
+-rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia-api-0.1.1/drukarnia-api/author.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia-api-0.1.1/drukarnia-api/connection.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia-api-0.1.1/drukarnia-api/drukarnia_api.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:01:09.269466 drukarnia-api-0.1.1/drukarnia_api.egg-info/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:01:09.000000 drukarnia-api-0.1.1/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)      308 2023-06-02 05:01:09.000000 drukarnia-api-0.1.1/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 05:01:09.000000 drukarnia-api-0.1.1/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 05:01:09.000000 drukarnia-api-0.1.1/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 05:01:09.270582 drukarnia-api-0.1.1/setup.cfg
+-rw-r--r--   0 andrej5    (501) staff       (20)     1293 2023-06-02 04:47:11.000000 drukarnia-api-0.1.1/setup.py
```

### Comparing `drukarnia-api-0.1.0/LICENSE` & `drukarnia-api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.0/PKG-INFO` & `drukarnia-api-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,22 +16,22 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drukarnia-api
 
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/aac75e2b8f63500ac70bce5244cbf507bf973b73/LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
 `drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, which provides various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the ***Drukarnia API***, allowing users to integrate Drukarnia's features seamlessly into their applications.
 
 Please note that the library is currently in its early development stages and supports only information search. However, future updates will expand its capabilities to include posting articles, comments, and more.
 
-For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***]([overview.ipynb](https://github.com/androu-sys/drukarnia-api/overview.ipynb)).
+For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
```

### Comparing `drukarnia-api-0.1.0/README.md` & `drukarnia-api-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # drukarnia-api
 
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/aac75e2b8f63500ac70bce5244cbf507bf973b73/LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
 `drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, which provides various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the ***Drukarnia API***, allowing users to integrate Drukarnia's features seamlessly into their applications.
 
 Please note that the library is currently in its early development stages and supports only information search. However, future updates will expand its capabilities to include posting articles, comments, and more.
 
-For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***]([overview.ipynb](https://github.com/androu-sys/drukarnia-api/overview.ipynb)).
+For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
 
 ## Contributing
 
-Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
+Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.0/drukarnia-api/article.py` & `drukarnia-api-0.1.1/drukarnia-api/article.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.0/drukarnia-api/author.py` & `drukarnia-api-0.1.1/drukarnia-api/author.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.0/drukarnia-api/connection.py` & `drukarnia-api-0.1.1/drukarnia-api/connection.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.0/drukarnia-api/drukarnia_api.py` & `drukarnia-api-0.1.1/drukarnia-api/drukarnia_api.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.0/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.1/drukarnia_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,22 +16,22 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # drukarnia-api
 
 
-[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/aac75e2b8f63500ac70bce5244cbf507bf973b73/LICENSE)
+[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/androu-sys/drukarnia-api/blob/main/LICENSE)
 
 ## Overview
 `drukarnia-api` is a Python library designed as a wrapper for the ***Drukarnia API***, which provides various functionalities for interacting with the Drukarnia platform. It simplifies the process of accessing and manipulating data from the ***Drukarnia API***, allowing users to integrate Drukarnia's features seamlessly into their applications.
 
 Please note that the library is currently in its early development stages and supports only information search. However, future updates will expand its capabilities to include posting articles, comments, and more.
 
-For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***]([overview.ipynb](https://github.com/androu-sys/drukarnia-api/overview.ipynb)).
+For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
 pip install drukarnia-api
 ```
```

### Comparing `drukarnia-api-0.1.0/setup.py` & `drukarnia-api-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.0",
+    version="0.1.1",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

