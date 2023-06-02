# Comparing `tmp/drukarnia-api-0.1.5.tar.gz` & `tmp/drukarnia-api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drukarnia-api-0.1.5.tar", last modified: Fri Jun  2 05:49:22 2023, max compression
+gzip compressed data, was "dist/drukarnia-api-0.1.6.tar", last modified: Fri Jun  2 06:02:32 2023, max compression
```

## Comparing `drukarnia-api-0.1.5.tar` & `drukarnia-api-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:49:22.754413 drukarnia-api-0.1.5/
--rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia-api-0.1.5/LICENSE
--rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:49:22.754037 drukarnia-api-0.1.5/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)     1265 2023-06-02 04:59:01.000000 drukarnia-api-0.1.5/README.md
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:49:22.749968 drukarnia-api-0.1.5/drukarnia_api/
--rw-r--r--   0 andrej5    (501) staff       (20)       86 2023-06-02 04:04:41.000000 drukarnia-api-0.1.5/drukarnia_api/__init__.py
--rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia-api-0.1.5/drukarnia_api/article.py
--rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia-api-0.1.5/drukarnia_api/author.py
--rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia-api-0.1.5/drukarnia_api/connection.py
--rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia-api-0.1.5/drukarnia_api/drukarnia_api.py
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:49:22.753318 drukarnia-api-0.1.5/drukarnia_api.egg-info/
--rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:49:22.000000 drukarnia-api-0.1.5/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)      344 2023-06-02 05:49:22.000000 drukarnia-api-0.1.5/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 05:49:22.000000 drukarnia-api-0.1.5/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 andrej5    (501) staff       (20)      213 2023-06-02 05:49:22.000000 drukarnia-api-0.1.5/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 05:49:22.000000 drukarnia-api-0.1.5/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 05:49:22.754594 drukarnia-api-0.1.5/setup.cfg
--rw-r--r--   0 andrej5    (501) staff       (20)     1386 2023-06-02 05:49:18.000000 drukarnia-api-0.1.5/setup.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:02:32.943882 drukarnia-api-0.1.6/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia-api-0.1.6/LICENSE
+-rw-r--r--   0 andrej5    (501) staff       (20)     1954 2023-06-02 06:02:32.943486 drukarnia-api-0.1.6/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)     1272 2023-06-02 06:01:45.000000 drukarnia-api-0.1.6/README.md
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:02:32.937919 drukarnia-api-0.1.6/drukarnia_api/
+-rw-r--r--   0 andrej5    (501) staff       (20)       87 2023-06-02 06:00:56.000000 drukarnia-api-0.1.6/drukarnia_api/__init__.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia-api-0.1.6/drukarnia_api/_drukarnia_api.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia-api-0.1.6/drukarnia_api/article.py
+-rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia-api-0.1.6/drukarnia_api/author.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia-api-0.1.6/drukarnia_api/connection.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 06:02:32.942518 drukarnia-api-0.1.6/drukarnia_api.egg-info/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1954 2023-06-02 06:02:32.000000 drukarnia-api-0.1.6/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)      345 2023-06-02 06:02:32.000000 drukarnia-api-0.1.6/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 06:02:32.000000 drukarnia-api-0.1.6/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)      213 2023-06-02 06:02:32.000000 drukarnia-api-0.1.6/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 06:02:32.000000 drukarnia-api-0.1.6/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 06:02:32.944065 drukarnia-api-0.1.6/setup.cfg
+-rw-r--r--   0 andrej5    (501) staff       (20)     1386 2023-06-02 06:01:21.000000 drukarnia-api-0.1.6/setup.py
```

### Comparing `drukarnia-api-0.1.5/LICENSE` & `drukarnia-api-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.5/PKG-INFO` & `drukarnia-api-0.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -29,13 +29,13 @@
 
 For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
-pip install drukarnia-api
+pip install drukarnia-api==0.1.6
 ```
 
 ## Contributing
 
 Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.5/README.md` & `drukarnia-api-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
-pip install drukarnia-api
+pip install drukarnia-api==0.1.6
 ```
 
 ## Contributing
 
 Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.5/drukarnia_api/article.py` & `drukarnia-api-0.1.6/drukarnia_api/article.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.5/drukarnia_api/author.py` & `drukarnia-api-0.1.6/drukarnia_api/author.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.5/drukarnia_api/connection.py` & `drukarnia-api-0.1.6/drukarnia_api/connection.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.5/drukarnia_api/drukarnia_api.py` & `drukarnia-api-0.1.6/drukarnia_api/_drukarnia_api.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-0.1.5/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-0.1.6/drukarnia_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.5
+Version: 0.1.6
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -29,13 +29,13 @@
 
 For a detailed overview of the available functionalities and how to use them, please refer to the [***Functionality Overview File***](https://github.com/androu-sys/drukarnia-api/blob/main/overview.ipynb).
 
 ## Installation
 You can install `drukarnia-api` using pip:
 
 ```bash
-pip install drukarnia-api
+pip install drukarnia-api==0.1.6
 ```
 
 ## Contributing
 
 Contributions to `drukarnia-api` are welcome! If you find any issues or have suggestions for improvement, please open an issue or submit a pull request on the GitHub repository: https://github.com/androu-sys/drukarnia-api.
```

### Comparing `drukarnia-api-0.1.5/setup.py` & `drukarnia-api-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="0.1.5",
+    version="0.1.6",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

