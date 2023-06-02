# Comparing `tmp/kthutils-1.3.tar.gz` & `tmp/kthutils-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthutils-1.3.tar", max compression
+gzip compressed data, was "kthutils-1.4.tar", max compression
```

## Comparing `kthutils-1.3.tar` & `kthutils-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.3/LICENSE
--rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.3/README.md
--rw-r--r--   0        0        0      721 2023-05-26 15:55:06.744988 kthutils-1.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.3/src/kthutils/.gitignore
--rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.3/src/kthutils/Makefile
--rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.3/src/kthutils/__init__.py
--rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.3/src/kthutils/cli.nw
--rw-r--r--   0        0        0      281 2023-05-26 15:56:15.589305 kthutils-1.3/src/kthutils/cli.py
--rw-r--r--   0        0        0      770 2023-05-26 15:56:15.589305 kthutils-1.3/src/kthutils/credentials.py
--rw-r--r--   0        0        0    17844 2023-05-26 15:54:52.740964 kthutils-1.3/src/kthutils/ug.nw
--rw-r--r--   0        0        0     9315 2023-05-26 15:56:15.593305 kthutils-1.3/src/kthutils/ug.py
--rw-r--r--   0        0        0      745 2023-05-26 15:56:06.429250 kthutils-1.3/tests/test_ug.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.4/LICENSE
+-rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.4/README.md
+-rw-r--r--   0        0        0      721 2023-06-02 08:49:19.161273 kthutils-1.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.4/src/kthutils/.gitignore
+-rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.4/src/kthutils/Makefile
+-rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.4/src/kthutils/__init__.py
+-rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.4/src/kthutils/cli.nw
+-rw-r--r--   0        0        0      281 2023-06-02 08:49:46.453760 kthutils-1.4/src/kthutils/cli.py
+-rw-r--r--   0        0        0      770 2023-06-02 08:49:46.457759 kthutils-1.4/src/kthutils/credentials.py
+-rw-r--r--   0        0        0    18168 2023-06-02 08:48:48.120726 kthutils-1.4/src/kthutils/ug.nw
+-rw-r--r--   0        0        0     9317 2023-06-02 08:49:46.457759 kthutils-1.4/src/kthutils/ug.py
+-rw-r--r--   0        0        0      745 2023-06-02 08:50:09.986183 kthutils-1.4/tests/test_ug.py
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.4/PKG-INFO
```

### Comparing `kthutils-1.3/LICENSE` & `kthutils-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kthutils-1.3/README.md` & `kthutils-1.4/README.md`

 * *Files identical despite different names*

### Comparing `kthutils-1.3/pyproject.toml` & `kthutils-1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kthutils"
-version = "1.3"
+version = "1.4"
 description = "Various tools for automation at KTH"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/kthutils"
 include = ["*/**/*.py"]
```

### Comparing `kthutils-1.3/src/kthutils/cli.nw` & `kthutils-1.4/src/kthutils/cli.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.3/src/kthutils/credentials.py` & `kthutils-1.4/src/kthutils/credentials.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.3/src/kthutils/ug.nw` & `kthutils-1.4/src/kthutils/ug.nw`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 <<helper functions>>
 
 class UGsession:
   """
   Maintains a session to the UG Editor APIs.
   """
-  BASE_URL = "https://app.kth.se/ug-gruppeditor"
+  BASE_URL = <<the UG group editor base URL>>
 
   def __init__(self, username, password):
     """
     Requires `username` and `password` which are the normal credentials for 
     logging in through https://login.ug.kth.se.
 
     All API requests are performed as this user.
@@ -43,14 +43,23 @@
 
 <<set up typer cli>>
 
 if __name__ == "__main__":
   <<run typer cli>>
 @
 
+The URL to the UG editor changed at some point around the shift from May to 
+June 2023,
+The URL is essentially the same, but after the change it must have the slash 
+(\enquote{/}) at the end.
+Without that slash, we get a 404 instead of what we expect.
+<<the UG group editor base URL>>=
+"https://app.kth.se/ug-gruppeditor/"
+@
+
 
 \section{Tests}
 
 We provide tests for the class.
 We create a [[ug]] object and will add test functions to [[<<test functions>>]] 
 as we add methods to [[<<UG methods>>]].
 <<test ug.py>>=
@@ -106,15 +115,15 @@
 [[weblogin.AutologinSession]]
 together with the KTH UG login handler
 [[weblogin.kth.UGlogin]]
 for that.
 <<UG constructor>>=
 self.__session = weblogin.AutologinSession([
       weblogin.kth.UGlogin(username, password,
-                          self.BASE_URL)
+                           self.BASE_URL)
   ])
 @
 
 
 \section{Listing editable groups}
 
 The first thing we want to do is to be able to list all groups.
```

### Comparing `kthutils-1.3/src/kthutils/ug.py` & `kthutils-1.4/src/kthutils/ug.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,26 +28,26 @@
 
   return name, desc
 
 class UGsession:
   """
   Maintains a session to the UG Editor APIs.
   """
-  BASE_URL = "https://app.kth.se/ug-gruppeditor"
+  BASE_URL = "https://app.kth.se/ug-gruppeditor/"
 
   def __init__(self, username, password):
     """
     Requires `username` and `password` which are the normal credentials for 
     logging in through https://login.ug.kth.se.
 
     All API requests are performed as this user.
     """
     self.__session = weblogin.AutologinSession([
           weblogin.kth.UGlogin(username, password,
-                              self.BASE_URL)
+                               self.BASE_URL)
       ])
     self.cache = {}
 
   @ct.cachedmethod(operator.attrgetter("cache"),
     key=ft.partial(ct.keys.hashkey, "list_editable_groups"))
   def list_editable_groups(self):
     """
```

### Comparing `kthutils-1.3/tests/test_ug.py` & `kthutils-1.4/tests/test_ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.3/PKG-INFO` & `kthutils-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthutils
-Version: 1.3
+Version: 1.4
 Summary: Various tools for automation at KTH
 Home-page: https://github.com/dbosk/kthutils
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

