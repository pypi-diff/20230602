# Comparing `tmp/shellcheck_py-0.9.0.3.tar.gz` & `tmp/shellcheck_py-0.9.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcheck_py-0.9.0.3.tar", last modified: Thu Jun  1 22:46:05 2023, max compression
+gzip compressed data, was "shellcheck_py-0.9.0.4.tar", last modified: Thu Jun  1 23:43:05 2023, max compression
```

## Comparing `shellcheck_py-0.9.0.3.tar` & `shellcheck_py-0.9.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2023-06-01 22:33:55.000000 shellcheck_py-0.9.0.3/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1053 2023-06-01 22:45:45.000000 shellcheck_py-0.9.0.3/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5286 2023-06-01 22:45:48.000000 shellcheck_py-0.9.0.3/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 22:46:05.787488 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 22:46:05.000000 shellcheck_py-0.9.0.3/shellcheck_py.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2023-06-01 23:42:25.000000 shellcheck_py-0.9.0.4/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1053 2023-06-01 23:42:41.000000 shellcheck_py-0.9.0.4/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5286 2023-06-01 23:42:47.000000 shellcheck_py-0.9.0.4/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/top_level.txt
```

### Comparing `shellcheck_py-0.9.0.3/LICENSE` & `shellcheck_py-0.9.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.3/PKG-INFO` & `shellcheck_py-0.9.0.4/shellcheck_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shellcheck_py
-Version: 0.9.0.3
+Name: shellcheck-py
+Version: 0.9.0.4
 Summary: Python wrapper around invoking shellcheck (https://www.shellcheck.net/)
 Home-page: https://github.com/ryanrhee/shellcheck-py
 Author: Ryan Rhee
 Author-email: pypi@rhee.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.3
+    rev: v0.9.0.4
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.3/README.md` & `shellcheck_py-0.9.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.3
+    rev: v0.9.0.4
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.3/setup.cfg` & `shellcheck_py-0.9.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.3/setup.py` & `shellcheck_py-0.9.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         'zip',
         'ae58191b1ea4ffd9e5b15da9134146e636440302ce3e2f46863e8d71c8be1bbb',
     ),
 }
 POSTFIX_SHA256[('cygwin', 'x86_64')] = POSTFIX_SHA256[('win32', 'AMD64')]
 POSTFIX_SHA256[('darwin', 'arm64')] = POSTFIX_SHA256[('darwin', 'x86_64')]
 POSTFIX_SHA256[('linux', 'armv7l')] = POSTFIX_SHA256[('linux', 'armv6hf')]
-PY_VERSION = '3'
+PY_VERSION = '4'
 
 
 def get_download_url() -> tuple[str, str]:
     postfix, sha256 = POSTFIX_SHA256[(sys.platform, platform.machine())]
     url = (
         f'https://github.com/koalaman/shellcheck/releases/download/'
         f'v{SHELLCHECK_VERSION}/shellcheck-v{SHELLCHECK_VERSION}.{postfix}'
```

### Comparing `shellcheck_py-0.9.0.3/shellcheck_py.egg-info/PKG-INFO` & `shellcheck_py-0.9.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: shellcheck-py
-Version: 0.9.0.3
+Name: shellcheck_py
+Version: 0.9.0.4
 Summary: Python wrapper around invoking shellcheck (https://www.shellcheck.net/)
 Home-page: https://github.com/ryanrhee/shellcheck-py
 Author: Ryan Rhee
 Author-email: pypi@rhee.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,14 +40,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.3
+    rev: v0.9.0.4
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

