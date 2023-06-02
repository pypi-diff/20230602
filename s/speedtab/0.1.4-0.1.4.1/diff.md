# Comparing `tmp/speedtab-0.1.4.tar.gz` & `tmp/speedtab-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.1.4.tar", max compression
+gzip compressed data, was "speedtab-0.1.4.1.tar", max compression
```

## Comparing `speedtab-0.1.4.tar` & `speedtab-0.1.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      565 2023-05-24 14:59:45.962392 speedtab-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.4/speedtab/__init__.py
--rw-r--r--   0        0        0    49953 2023-05-24 14:57:04.407916 speedtab-0.1.4/speedtab/client.py
--rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4/speedtab/enums.py
--rw-r--r--   0        0        0     1730 2023-05-19 11:23:08.076916 speedtab-0.1.4/speedtab/formats.py
--rw-r--r--   0        0        0      781 2023-05-24 14:59:58.215209 speedtab-0.1.4/setup.py
--rw-r--r--   0        0        0      806 2023-05-24 14:59:58.215209 speedtab-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      567 2023-06-02 10:10:18.360384 speedtab-0.1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      352 2022-09-07 08:00:08.177672 speedtab-0.1.4.1/speedtab/__init__.py
+-rw-r--r--   0        0        0    49953 2023-05-24 14:57:04.407916 speedtab-0.1.4.1/speedtab/client.py
+-rw-r--r--   0        0        0     6192 2023-05-19 11:01:11.239027 speedtab-0.1.4.1/speedtab/enums.py
+-rw-r--r--   0        0        0     1724 2023-06-02 10:10:18.366392 speedtab-0.1.4.1/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2023-06-02 10:11:19.248435 speedtab-0.1.4.1/setup.py
+-rw-r--r--   0        0        0      808 2023-06-02 10:11:19.248435 speedtab-0.1.4.1/PKG-INFO
```

### Comparing `speedtab-0.1.4/pyproject.toml` & `speedtab-0.1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.1.4"
+version = "0.1.4.1"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.1.4/speedtab/client.py` & `speedtab-0.1.4.1/speedtab/client.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4/speedtab/enums.py` & `speedtab-0.1.4.1/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.1.4/speedtab/formats.py` & `speedtab-0.1.4.1/speedtab/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 class Scientific(BaseNumberFormat):
     def __init__(self, pattern: str = '0.00E+00'):
         super().__init__('SCIENTIFIC', pattern)
 
 
 class Border:
     def __init__(self, style: Enum, width: int, color: Color):
-        self.style = style.value
+        self.style = style
         self.width = width
         self.color = color.color
```

### Comparing `speedtab-0.1.4/setup.py` & `speedtab-0.1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.1.4',
+    'version': '0.1.4.1',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.1.4/PKG-INFO` & `speedtab-0.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

