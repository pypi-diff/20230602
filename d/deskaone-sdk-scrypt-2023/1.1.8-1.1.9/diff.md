# Comparing `tmp/deskaone_sdk_scrypt_2023-1.1.8.tar.gz` & `tmp/deskaone_sdk_scrypt_2023-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.8.tar", max compression
+gzip compressed data, was "deskaone_sdk_scrypt_2023-1.1.9.tar", max compression
```

## Comparing `deskaone_sdk_scrypt_2023-1.1.8.tar` & `deskaone_sdk_scrypt_2023-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      754 2023-05-26 04:51:14.415501 deskaone_sdk_scrypt_2023-1.1.8/pyproject.toml
--rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.8/README.md
--rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/__init__.py
--rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Client/__init__.py
--rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Database/__init__.py
--rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
--rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
--rw-r--r--   0        0        0      491 2023-05-26 04:50:24.591278 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
--rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
--rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Color.py
--rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
--rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
--rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
--rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Random.py
--rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
--rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
--rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
--rw-r--r--   0        0        0     3613 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
--rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
--rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.8/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-02 10:56:15.171255 deskaone_sdk_scrypt_2023-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-05-02 07:07:11.877144 deskaone_sdk_scrypt_2023-1.1.9/README.md
+-rw-r--r--   0        0        0      388 2023-05-12 00:00:42.632394 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/__init__.py
+-rw-r--r--   0        0        0     6046 2023-05-24 06:59:06.082419 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py
+-rw-r--r--   0        0        0      801 2023-05-02 07:04:46.927664 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py
+-rw-r--r--   0        0        0     3329 2023-05-06 12:05:36.923716 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py
+-rw-r--r--   0        0        0     2939 2023-05-24 06:59:15.474420 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-02 10:56:16.775256 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/__init__.py
+-rw-r--r--   0        0        0     8784 2023-04-04 14:12:43.119086 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py
+-rw-r--r--   0        0        0      390 2023-02-27 03:32:49.658333 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Color.py
+-rw-r--r--   0        0        0    11727 2023-03-27 20:05:25.868396 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py
+-rw-r--r--   0        0        0     2434 2023-05-05 18:27:43.486614 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py
+-rw-r--r--   0        0        0    34717 2023-05-19 13:16:00.694179 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py
+-rw-r--r--   0        0        0      959 2023-04-04 14:10:53.173754 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py
+-rw-r--r--   0        0        0      262 2023-03-29 02:18:08.551085 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Reset.py
+-rw-r--r--   0        0        0      254 2023-04-02 03:21:50.044410 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Reverse.py
+-rw-r--r--   0        0        0     2964 2023-05-02 07:04:46.855661 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py
+-rw-r--r--   0        0        0     3577 2023-06-02 10:50:19.635539 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py
+-rw-r--r--   0        0        0     2662 2023-03-09 14:27:56.886653 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py
+-rw-r--r--   0        0        0    13598 2023-05-04 06:48:40.563985 deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py
+-rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.9/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 deskaone_sdk_scrypt_2023-1.1.9/PKG-INFO
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/pyproject.toml` & `deskaone_sdk_scrypt_2023-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deskaone-sdk-scrypt-2023"
-version = "1.1.8"
+version = "1.1.9"
 description = ""
 authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "deskaone_sdk_scrypt_2023", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Client/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Client/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Database/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Internal/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Internal/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/AWSViker.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Crypto.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Proxy.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Random.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Random.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Timer.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Timer.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/Typer.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/Typer.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,19 @@
         return message
     
     @staticmethod
     def Print(message: any, Refresh: Optional[bool] = None, Enter: Optional[bool] = None, isTimer: Optional[bool] = None): # type: ignore
         if Refresh is None and Enter is None:raise Error('Refresh True or False / Enter True or False')
         if Enter is True:
             sys.stdout.write(f'{Typer.Parse_Text(" ")}\r')
-            sys.stdout.write(f'{Typer.Parse_Text(message)}{Color.WHITE}\n')
+            sys.stdout.write(f'{message}{Color.WHITE}\n')
             sys.stdout.write(f'{Typer.Parse_Text(" ")}\r')
             sys.stdout.flush()
         if Refresh is True:
-            sys.stdout.write(f'{Typer.Parse_Text(message)}{Color.WHITE}\r')
+            sys.stdout.write(f'{message}{Color.WHITE}\r')
             if isTimer is False:sys.stdout.write(f'{Typer.Parse_Text(" ")}\r')
 
     @staticmethod
     def Line(Normal: Optional[bool] = None, Bold: Optional[bool] = None):
         if Normal is None and Bold is None:raise Error('Normal True or False / Bold True or False')
         if Normal is True:sys.stdout.write(
             f'{Typer.Parse_Text_Line("-", Normal=True)}{Color.BLUE}[{Color.YELLOW}{datetime.datetime.now().strftime("%d/%m/%Y, %H:%M:%S")}{Color.BLUE}]{Color.WHITE}{Typer.Parse_Text_Line("-", Normal=True)}{Color.WHITE}\n')
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/UserAgent.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py` & `deskaone_sdk_scrypt_2023-1.1.9/src/deskaone_sdk_scrypt_2023/Utils/WebShare/__init__.py`

 * *Files identical despite different names*

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/setup.py` & `deskaone_sdk_scrypt_2023-1.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'random-user-agent>=1.0.1,<2.0.0',
  'requests[socks]>=2.28.2,<3.0.0',
  'sqlalchemy==1.4.29']
 
 setup_kwargs = {
     'name': 'deskaone-sdk-scrypt-2023',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': '',
     'long_description': 'xxxxxxxxxxxxxxxx',
     'author': 'Antoni Oktha Fernandes',
     'author_email': '37358597+DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `deskaone_sdk_scrypt_2023-1.1.8/PKG-INFO` & `deskaone_sdk_scrypt_2023-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deskaone-sdk-scrypt-2023
-Version: 1.1.8
+Version: 1.1.9
 Summary: 
 Author: Antoni Oktha Fernandes
 Author-email: 37358597+DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

