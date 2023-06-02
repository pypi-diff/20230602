# Comparing `tmp/drukarnia_api-0.1.2.tar.gz` & `tmp/drukarnia_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drukarnia_api-0.1.2.tar", last modified: Fri Jun  2 05:35:33 2023, max compression
+gzip compressed data, was "dist/drukarnia_api-0.1.3.tar", last modified: Fri Jun  2 05:40:06 2023, max compression
```

## Comparing `drukarnia_api-0.1.2.tar` & `drukarnia_api-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:35:33.823318 drukarnia_api-0.1.2/
--rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia_api-0.1.2/LICENSE
--rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:35:33.822557 drukarnia_api-0.1.2/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)     1265 2023-06-02 04:59:01.000000 drukarnia_api-0.1.2/README.md
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:35:33.816769 drukarnia_api-0.1.2/drukarnia-api/
--rw-r--r--   0 andrej5    (501) staff       (20)       86 2023-06-02 04:04:41.000000 drukarnia_api-0.1.2/drukarnia-api/__init__.py
--rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia_api-0.1.2/drukarnia-api/article.py
--rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia_api-0.1.2/drukarnia-api/author.py
--rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia_api-0.1.2/drukarnia-api/connection.py
--rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia_api-0.1.2/drukarnia-api/drukarnia_api.py
-drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:35:33.821393 drukarnia_api-0.1.2/drukarnia_api.egg-info/
--rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:35:33.000000 drukarnia_api-0.1.2/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 andrej5    (501) staff       (20)      344 2023-06-02 05:35:33.000000 drukarnia_api-0.1.2/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 05:35:33.000000 drukarnia_api-0.1.2/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 andrej5    (501) staff       (20)      213 2023-06-02 05:35:33.000000 drukarnia_api-0.1.2/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 05:35:33.000000 drukarnia_api-0.1.2/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 05:35:33.823629 drukarnia_api-0.1.2/setup.cfg
--rw-r--r--   0 andrej5    (501) staff       (20)     1386 2023-06-02 05:35:31.000000 drukarnia_api-0.1.2/setup.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:40:06.533807 drukarnia_api-0.1.3/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1063 2023-06-02 04:09:32.000000 drukarnia_api-0.1.3/LICENSE
+-rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:40:06.532971 drukarnia_api-0.1.3/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)     1265 2023-06-02 04:59:01.000000 drukarnia_api-0.1.3/README.md
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:40:06.522035 drukarnia_api-0.1.3/drukarnia_api/
+-rw-r--r--   0 andrej5    (501) staff       (20)       86 2023-06-02 04:04:41.000000 drukarnia_api-0.1.3/drukarnia_api/__init__.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      555 2023-06-02 04:04:41.000000 drukarnia_api-0.1.3/drukarnia_api/article.py
+-rw-r--r--   0 andrej5    (501) staff       (20)     3250 2023-06-02 04:04:41.000000 drukarnia_api-0.1.3/drukarnia_api/author.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      680 2023-06-02 04:04:41.000000 drukarnia_api-0.1.3/drukarnia_api/connection.py
+-rw-r--r--   0 andrej5    (501) staff       (20)      862 2023-06-02 04:04:41.000000 drukarnia_api-0.1.3/drukarnia_api/drukarnia_api.py
+drwxr-xr-x   0 andrej5    (501) staff       (20)        0 2023-06-02 05:40:06.531257 drukarnia_api-0.1.3/drukarnia_api.egg-info/
+-rw-r--r--   0 andrej5    (501) staff       (20)     1947 2023-06-02 05:40:06.000000 drukarnia_api-0.1.3/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 andrej5    (501) staff       (20)      344 2023-06-02 05:40:06.000000 drukarnia_api-0.1.3/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)        1 2023-06-02 05:40:06.000000 drukarnia_api-0.1.3/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)      213 2023-06-02 05:40:06.000000 drukarnia_api-0.1.3/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       14 2023-06-02 05:40:06.000000 drukarnia_api-0.1.3/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 andrej5    (501) staff       (20)       38 2023-06-02 05:40:06.534183 drukarnia_api-0.1.3/setup.cfg
+-rw-r--r--   0 andrej5    (501) staff       (20)     1386 2023-06-02 05:39:53.000000 drukarnia_api-0.1.3/setup.py
```

### Comparing `drukarnia_api-0.1.2/LICENSE` & `drukarnia_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/PKG-INFO` & `drukarnia_api-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia_api-0.1.2/README.md` & `drukarnia_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/drukarnia-api/article.py` & `drukarnia_api-0.1.3/drukarnia_api/article.py`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/drukarnia-api/author.py` & `drukarnia_api-0.1.3/drukarnia_api/author.py`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/drukarnia-api/connection.py` & `drukarnia_api-0.1.3/drukarnia_api/connection.py`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/drukarnia-api/drukarnia_api.py` & `drukarnia_api-0.1.3/drukarnia_api/drukarnia_api.py`

 * *Files identical despite different names*

### Comparing `drukarnia_api-0.1.2/drukarnia_api.egg-info/PKG-INFO` & `drukarnia_api-0.1.3/drukarnia_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `drukarnia_api-0.1.2/setup.py` & `drukarnia_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia_api",
-    version="0.1.2",
+    version="0.1.3",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
@@ -33,11 +33,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
-    packages=["drukarnia-api"],
+    packages=["drukarnia_api"],
     include_package_data=True,
     install_requires=requirements
 )
```

