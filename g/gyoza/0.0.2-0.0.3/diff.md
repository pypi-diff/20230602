# Comparing `tmp/gyoza-0.0.2.tar.gz` & `tmp/gyoza-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "gyoza-0.0.3.tar", last modified: Fri Jun  2 11:53:52 2023, max compression
```

## Comparing `gyoza-0.0.2.tar` & `gyoza-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gyoza-0.0.2/src/gyoza/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gyoza-0.0.2/src/gyoza/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gyoza-0.0.2/LICENSE
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gyoza-0.0.2/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 gyoza-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 gyoza-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.590000 gyoza-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-06-02 09:45:10.000000 gyoza-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      877 2023-06-02 11:53:54.000000 gyoza-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-06-02 09:48:40.000000 gyoza-0.0.3/README.md
+-rw-rw-rw-   0        0        0      762 2023-06-02 11:53:24.000000 gyoza-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 11:53:54.000000 gyoza-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      173 2023-06-02 11:51:40.000000 gyoza-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.640000 gyoza-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.660000 gyoza-0.0.3/src/gyoza/
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:30:44.000000 gyoza-0.0.3/src/gyoza/__init__.py
+-rw-rw-rw-   0        0        0      113 2023-06-02 11:31:44.000000 gyoza-0.0.3/src/gyoza/example.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.750000 gyoza-0.0.3/src/gyoza/sub_package_A/
+-rw-rw-rw-   0        0        0        0 2023-06-02 11:33:14.000000 gyoza-0.0.3/src/gyoza/sub_package_A/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-06-02 11:52:58.000000 gyoza-0.0.3/src/gyoza/sub_package_A/module_A.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.790000 gyoza-0.0.3/src/gyoza/sub_package_B/
+-rw-rw-rw-   0        0        0        0 2023-06-02 11:33:16.000000 gyoza-0.0.3/src/gyoza/sub_package_B/__init__.py
+-rw-rw-rw-   0        0        0       99 2023-06-02 11:51:50.000000 gyoza-0.0.3/src/gyoza/sub_package_B/module_B.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:53:52.700000 gyoza-0.0.3/src/gyoza.egg-info/
+-rw-rw-rw-   0        0        0      877 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 11:53:54.000000 gyoza-0.0.3/src/gyoza.egg-info/top_level.txt
```

### Comparing `gyoza-0.0.2/LICENSE` & `gyoza-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.2/pyproject.toml` & `gyoza-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools >= 61.0.0"]
+build-backend = "setuptools.build_meta"
+
+[tool.setuptools.packages.find]
+where = ["src"]
 
 [project]
 name = "gyoza"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Tim Dick", email="timdi@icloud.com" },
 ]
 description = "A package to study the latent representations of auditory events processing in the human brain."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gyoza-0.0.2/PKG-INFO` & `gyoza-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1
-Name: gyoza
-Version: 0.0.2
-Summary: A package to study the latent representations of auditory events processing in the human brain.
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Author-email: Tim Dick <timdi@icloud.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: librosa>=0.10.0.post2
-Description-Content-Type: text/markdown
-
-# Gyoza 
-## A library for explaining latent representations during auditory event recognition in the human brain.
-### Master thesis project of Tim Dick
-https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
+Metadata-Version: 2.1
+Name: gyoza
+Version: 0.0.3
+Summary: A package to study the latent representations of auditory events processing in the human brain.
+Author-email: Tim Dick <timdi@icloud.com>
+Project-URL: Homepage, https://github.com/pypa/sampleproject
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Gyoza 
+## A library for explaining latent representations during auditory event recognition in the human brain.
+### Master thesis project of Tim Dick
+https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
```

