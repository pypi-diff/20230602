# Comparing `tmp/erlenberg_ext-3.0.tar.gz` & `tmp/erlenberg_ext-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlenberg_ext-3.0.tar", last modified: Fri Jun  2 13:19:49 2023, max compression
+gzip compressed data, was "erlenberg_ext-3.1.tar", last modified: Fri Jun  2 13:22:17 2023, max compression
```

## Comparing `erlenberg_ext-3.0.tar` & `erlenberg_ext-3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:19:49.305442 erlenberg_ext-3.0/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)     1094 2022-12-10 23:42:16.000000 erlenberg_ext-3.0/LICENSE
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 13:19:49.305442 erlenberg_ext-3.0/PKG-INFO
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      558 2023-06-02 09:37:20.000000 erlenberg_ext-3.0/README.md
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:19:49.303442 erlenberg_ext-3.0/erlenberg_ext/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       33 2023-06-02 09:19:40.000000 erlenberg_ext-3.0/erlenberg_ext/__init__.py
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:19:49.304442 erlenberg_ext-3.0/erlenberg_ext/cryptScriptGenerator/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       51 2023-06-02 11:49:55.000000 erlenberg_ext-3.0/erlenberg_ext/cryptScriptGenerator/__init__.py
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)     3002 2023-04-21 13:05:05.000000 erlenberg_ext-3.0/erlenberg_ext/cryptScriptGenerator/__main__.py
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:19:49.305442 erlenberg_ext-3.0/erlenberg_ext/cryptTextGenerator/
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       49 2023-06-02 13:02:16.000000 erlenberg_ext-3.0/erlenberg_ext/cryptTextGenerator/__init__.py
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      600 2023-06-02 13:13:20.000000 erlenberg_ext-3.0/erlenberg_ext/cryptTextGenerator/__main__.py
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)     1322 2023-06-02 13:14:56.000000 erlenberg_ext-3.0/erlenberg_ext/simpleCrypt.py
-drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:19:49.304442 erlenberg_ext-3.0/erlenberg_ext.egg-info/
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/PKG-INFO
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      505 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/SOURCES.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)        1 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/dependency_links.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)      186 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/entry_points.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)       13 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/requires.txt
--rw-r--r--   0 pcuser    (1000) pcuser    (1000)       14 2023-06-02 13:19:49.000000 erlenberg_ext-3.0/erlenberg_ext.egg-info/top_level.txt
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      104 2022-12-10 21:33:18.000000 erlenberg_ext-3.0/pyproject.toml
--rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      712 2023-06-02 13:19:49.305442 erlenberg_ext-3.0/setup.cfg
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:22:17.005403 erlenberg_ext-3.1/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)     1094 2022-12-10 23:42:16.000000 erlenberg_ext-3.1/LICENSE
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 13:22:17.005403 erlenberg_ext-3.1/PKG-INFO
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      558 2023-06-02 09:37:20.000000 erlenberg_ext-3.1/README.md
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:22:17.003403 erlenberg_ext-3.1/erlenberg_ext/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       33 2023-06-02 09:19:40.000000 erlenberg_ext-3.1/erlenberg_ext/__init__.py
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:22:17.004403 erlenberg_ext-3.1/erlenberg_ext/cryptScriptGenerator/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       51 2023-06-02 11:49:55.000000 erlenberg_ext-3.1/erlenberg_ext/cryptScriptGenerator/__init__.py
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)     3002 2023-04-21 13:05:05.000000 erlenberg_ext-3.1/erlenberg_ext/cryptScriptGenerator/__main__.py
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:22:17.005403 erlenberg_ext-3.1/erlenberg_ext/cryptTextGenerator/
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)       49 2023-06-02 13:02:16.000000 erlenberg_ext-3.1/erlenberg_ext/cryptTextGenerator/__init__.py
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      600 2023-06-02 13:13:20.000000 erlenberg_ext-3.1/erlenberg_ext/cryptTextGenerator/__main__.py
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)     1323 2023-06-02 13:21:08.000000 erlenberg_ext-3.1/erlenberg_ext/simpleCrypt.py
+drwxr-xr-x   0 pcuser    (1000) pcuser    (1000)        0 2023-06-02 13:22:17.004403 erlenberg_ext-3.1/erlenberg_ext.egg-info/
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      935 2023-06-02 13:22:16.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/PKG-INFO
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      505 2023-06-02 13:22:17.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)        1 2023-06-02 13:22:16.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)      186 2023-06-02 13:22:16.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/entry_points.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)       13 2023-06-02 13:22:16.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/requires.txt
+-rw-r--r--   0 pcuser    (1000) pcuser    (1000)       14 2023-06-02 13:22:16.000000 erlenberg_ext-3.1/erlenberg_ext.egg-info/top_level.txt
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      104 2022-12-10 21:33:18.000000 erlenberg_ext-3.1/pyproject.toml
+-rwxrwxrwx   0 pcuser    (1000) pcuser    (1000)      712 2023-06-02 13:22:17.005403 erlenberg_ext-3.1/setup.cfg
```

### Comparing `erlenberg_ext-3.0/LICENSE` & `erlenberg_ext-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-3.0/PKG-INFO` & `erlenberg_ext-3.1/erlenberg_ext.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: erlenberg_ext
-Version: 3.0
+Name: erlenberg-ext
+Version: 3.1
 Summary: Some personal librarys for python (extended)
 Author: Tizian Erlenberg
 Author-email: mail@erlenberg.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `erlenberg_ext-3.0/README.md` & `erlenberg_ext-3.1/README.md`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-3.0/erlenberg_ext/cryptScriptGenerator/__main__.py` & `erlenberg_ext-3.1/erlenberg_ext/cryptScriptGenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-3.0/erlenberg_ext/cryptTextGenerator/__main__.py` & `erlenberg_ext-3.1/erlenberg_ext/cryptTextGenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `erlenberg_ext-3.0/erlenberg_ext/simpleCrypt.py` & `erlenberg_ext-3.1/erlenberg_ext/simpleCrypt.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     
     salt = base64.b64decode((enc_dict['salt']).encode('utf-8'))
     cyphertext = base64.b64decode((enc_dict['cyphertext']).encode('utf-8'))
     iterations = enc_dict['iterations']
     
     kdf = PBKDF2HMAC(
         algorithm=hashes.SHA256(),
-        length=32
+        length=32,
         salt=salt,
         iterations=iterations,
     )
     
     key = base64.urlsafe_b64encode(kdf.derive(password.encode()))
     f = Fernet(key)
     plaintext = f.decrypt(cyphertext).decode()
```

### Comparing `erlenberg_ext-3.0/erlenberg_ext.egg-info/PKG-INFO` & `erlenberg_ext-3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: erlenberg-ext
-Version: 3.0
+Name: erlenberg_ext
+Version: 3.1
 Summary: Some personal librarys for python (extended)
 Author: Tizian Erlenberg
 Author-email: mail@erlenberg.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `erlenberg_ext-3.0/setup.cfg` & `erlenberg_ext-3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = erlenberg_ext
-version = 3.0
+version = 3.1
 author = Tizian Erlenberg
 author_email = mail@erlenberg.net
 description = Some personal librarys for python (extended)
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
```

