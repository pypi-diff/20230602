# Comparing `tmp/gyoza-0.0.1.tar.gz` & `tmp/gyoza-0.0.2.tar.gz`

## Comparing `gyoza-0.0.1.tar` & `gyoza-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gyoza-0.0.1/src/example_package_gyoza/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gyoza-0.0.1/src/example_package_gyoza/example.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gyoza-0.0.1/LICENSE
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gyoza-0.0.1/README.md
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 gyoza-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 gyoza-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gyoza-0.0.2/src/gyoza/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gyoza-0.0.2/src/gyoza/example.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 gyoza-0.0.2/LICENSE
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gyoza-0.0.2/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 gyoza-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 gyoza-0.0.2/PKG-INFO
```

### Comparing `gyoza-0.0.1/LICENSE` & `gyoza-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gyoza-0.0.1/pyproject.toml` & `gyoza-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gyoza"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tim Dick", email="timdi@icloud.com" },
 ]
 description = "A package to study the latent representations of auditory events processing in the human brain."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `gyoza-0.0.1/PKG-INFO` & `gyoza-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyoza
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to study the latent representations of auditory events processing in the human brain.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Tim Dick <timdi@icloud.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

