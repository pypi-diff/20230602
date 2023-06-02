# Comparing `tmp/BingImageCreator-0.4.0.tar.gz` & `tmp/BingImageCreator-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BingImageCreator-0.4.0.tar", last modified: Fri Jun  2 16:02:18 2023, max compression
+gzip compressed data, was "BingImageCreator-0.4.1.tar", last modified: Fri Jun  2 16:45:55 2023, max compression
```

## Comparing `BingImageCreator-0.4.0.tar` & `BingImageCreator-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.098942 BingImageCreator-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:02:18.000000 BingImageCreator-0.4.0/src/BingImageCreator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16168 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/src/BingImageCreator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:02:18.102942 BingImageCreator-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 16:01:57.000000 BingImageCreator-0.4.0/test/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 16:45:55.000000 BingImageCreator-0.4.1/src/BingImageCreator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16130 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/src/BingImageCreator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:45:55.904468 BingImageCreator-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-02 16:45:23.000000 BingImageCreator-0.4.1/test/test_example.py
```

### Comparing `BingImageCreator-0.4.0/LICENSE` & `BingImageCreator-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.0/PKG-INFO` & `BingImageCreator-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.0
+Version: 0.4.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.0/README.md` & `BingImageCreator-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `BingImageCreator-0.4.0/setup.py` & `BingImageCreator-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="BingImageCreator",
-    version="0.4.0",
+    version="0.4.1",
     license="GNU General Public License v2.0",
     author="Antonio Cheong",
     author_email="acheong@student.dalat.org",
     description="High quality image generation by Microsoft. Reverse engineered API.",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/acheong08/BingImageCreator",
```

### Comparing `BingImageCreator-0.4.0/src/BingImageCreator.egg-info/PKG-INFO` & `BingImageCreator-0.4.1/src/BingImageCreator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BingImageCreator
-Version: 0.4.0
+Version: 0.4.1
 Summary: High quality image generation by Microsoft. Reverse engineered API.
 Home-page: https://github.com/acheong08/BingImageCreator
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/BingImageCreator/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `BingImageCreator-0.4.0/src/BingImageCreator.py` & `BingImageCreator-0.4.1/src/BingImageCreator.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             self.debug(sending_message)
         url_encoded_prompt = requests.utils.quote(prompt)
         payload = f"q={url_encoded_prompt}&qs=ds"
         # https://www.bing.com/images/create?q=<PROMPT>&rt=3&FORM=GENCRE
         url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=4&FORM=GENCRE"
         response = self.session.post(
             url,
-            follow_redirects=False,
+            allow_redirects=False,
             data=payload,
             timeout=200,
         )
         # check for content waring message
         if "this prompt is being reviewed" in response.text.lower():
             if self.debug_file:
                 self.debug(f"ERROR: {error_being_reviewed_prompt}")
@@ -122,21 +122,20 @@
         ):
             if self.debug_file:
                 self.debug(f"ERROR: {error_unsupported_lang}")
             raise Exception(error_unsupported_lang)
         if response.status_code != 302:
             # if rt4 fails, try rt3
             url = f"{BING_URL}/images/create?q={url_encoded_prompt}&rt=3&FORM=GENCRE"
-            response3 = self.session.post(url, follow_redirects=False, timeout=200)
-            if response3.status_code != 302:
+            response = self.session.post(url, allow_redirects=False, timeout=200)
+            if response.status_code != 302:
                 if self.debug_file:
                     self.debug(f"ERROR: {error_redirect}")
-                print(f"ERROR: {response3.text}")
+                print(f"ERROR: {response.text}")
                 raise Exception(error_redirect)
-            response = response3
         # Get redirect URL
         redirect_url = response.headers["Location"].replace("&nfy=1", "")
         request_id = redirect_url.split("id=")[-1]
         self.session.get(f"{BING_URL}{redirect_url}")
         # https://www.bing.com/images/create/async/results/{ID}?q={PROMPT}
         polling_url = f"{BING_URL}/images/create/async/results/{request_id}?q={url_encoded_prompt}"
         # Poll for results
```

### Comparing `BingImageCreator-0.4.0/test/test_example.py` & `BingImageCreator-0.4.1/test/test_example.py`

 * *Files identical despite different names*

