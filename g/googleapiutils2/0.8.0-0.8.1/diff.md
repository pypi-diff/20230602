# Comparing `tmp/googleapiutils2-0.8.0.tar.gz` & `tmp/googleapiutils2-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.8.0.tar", max compression
+gzip compressed data, was "googleapiutils2-0.8.1.tar", max compression
```

## Comparing `googleapiutils2-0.8.0.tar` & `googleapiutils2-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.0/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.0/README.md
--rw-r--r--   0        0        0       96 2023-06-01 17:02:06.802855 googleapiutils2-0.8.0/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.0/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.0/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.0/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.0/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-01 21:02:11.670817 googleapiutils2-0.8.0/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.0/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.0/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.0/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    32483 2023-06-02 03:13:17.683151 googleapiutils2-0.8.0/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5211 2023-06-02 00:22:11.187687 googleapiutils2-0.8.0/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.0/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-02 03:17:33.664572 googleapiutils2-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.1/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.1/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.1/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.1/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.1/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.1/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.1/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.1/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.1/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.1/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.1/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    32483 2023-06-02 03:13:17.683151 googleapiutils2-0.8.1/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5211 2023-06-02 00:22:11.187687 googleapiutils2-0.8.1/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.1/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-02 03:30:14.699581 googleapiutils2-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.1/PKG-INFO
```

### Comparing `googleapiutils2-0.8.0/LICENSE` & `googleapiutils2-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/README.md` & `googleapiutils2-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/drive/drive.py` & `googleapiutils2-0.8.1/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.8.1/googleapiutils2/geocode/geocode.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     @staticmethod
     def _return_if_200(r: requests.Response) -> list[GeocodeResult] | None:
         if r.status_code == 200:
             try:
-                return r.json()
+                return r.json().get("results", None)
             except JSONDecodeError:
                 return None
         else:
             return None
 
     def geocode(self, address: str):
         url = update_url_params(Geocode.URL, {"address": address, "key": self.api_key})
```

### Comparing `googleapiutils2-0.8.0/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.8.1/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.8.1/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.8.1/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.8.1/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/googleapiutils2/utils.py` & `googleapiutils2-0.8.1/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.0/pyproject.toml` & `googleapiutils2-0.8.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.8.0"
+version = "0.8.1"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.8.0/PKG-INFO` & `googleapiutils2-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.8.0
+Version: 0.8.1
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

