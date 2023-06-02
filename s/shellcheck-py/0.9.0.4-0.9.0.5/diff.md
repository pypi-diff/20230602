# Comparing `tmp/shellcheck_py-0.9.0.4.tar.gz` & `tmp/shellcheck_py-0.9.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellcheck_py-0.9.0.4.tar", last modified: Thu Jun  1 23:43:05 2023, max compression
+gzip compressed data, was "shellcheck_py-0.9.0.5.tar", last modified: Fri Jun  2 00:04:40 2023, max compression
```

## Comparing `shellcheck_py-0.9.0.4.tar` & `shellcheck_py-0.9.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2023-06-01 23:42:25.000000 shellcheck_py-0.9.0.4/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1053 2023-06-01 23:42:41.000000 shellcheck_py-0.9.0.4/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5286 2023-06-01 23:42:47.000000 shellcheck_py-0.9.0.4/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-01 23:43:05.619574 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-01 23:43:05.000000 shellcheck_py-0.9.0.4/shellcheck_py.egg-info/top_level.txt
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-02 00:04:40.007607 shellcheck_py-0.9.0.5/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1066 2023-06-01 23:42:25.000000 shellcheck_py-0.9.0.5/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-02 00:04:40.007607 shellcheck_py-0.9.0.5/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1053 2023-06-02 00:04:22.000000 shellcheck_py-0.9.0.5/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      661 2023-06-02 00:04:40.007607 shellcheck_py-0.9.0.5/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5286 2023-06-02 00:04:25.000000 shellcheck_py-0.9.0.5/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-02 00:04:40.007607 shellcheck_py-0.9.0.5/shellcheck_py.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1686 2023-06-02 00:04:39.000000 shellcheck_py-0.9.0.5/shellcheck_py.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      184 2023-06-02 00:04:39.000000 shellcheck_py-0.9.0.5/shellcheck_py.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-02 00:04:39.000000 shellcheck_py-0.9.0.5/shellcheck_py.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        6 2023-06-02 00:04:39.000000 shellcheck_py-0.9.0.5/shellcheck_py.egg-info/top_level.txt
```

### Comparing `shellcheck_py-0.9.0.4/LICENSE` & `shellcheck_py-0.9.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.4/PKG-INFO` & `shellcheck_py-0.9.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcheck_py
-Version: 0.9.0.4
+Version: 0.9.0.5
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
-    rev: v0.9.0.4
+    rev: v0.9.0.5
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.4/README.md` & `shellcheck_py-0.9.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 
 See [pre-commit] for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.9.0.4
+    rev: v0.9.0.5
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

### Comparing `shellcheck_py-0.9.0.4/setup.cfg` & `shellcheck_py-0.9.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `shellcheck_py-0.9.0.4/setup.py` & `shellcheck_py-0.9.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         'zip',
         'ae58191b1ea4ffd9e5b15da9134146e636440302ce3e2f46863e8d71c8be1bbb',
     ),
 }
 POSTFIX_SHA256[('cygwin', 'x86_64')] = POSTFIX_SHA256[('win32', 'AMD64')]
 POSTFIX_SHA256[('darwin', 'arm64')] = POSTFIX_SHA256[('darwin', 'x86_64')]
 POSTFIX_SHA256[('linux', 'armv7l')] = POSTFIX_SHA256[('linux', 'armv6hf')]
-PY_VERSION = '4'
+PY_VERSION = '5'
 
 
 def get_download_url() -> tuple[str, str]:
     postfix, sha256 = POSTFIX_SHA256[(sys.platform, platform.machine())]
     url = (
         f'https://github.com/koalaman/shellcheck/releases/download/'
         f'v{SHELLCHECK_VERSION}/shellcheck-v{SHELLCHECK_VERSION}.{postfix}'
```

### Comparing `shellcheck_py-0.9.0.4/shellcheck_py.egg-info/PKG-INFO` & `shellcheck_py-0.9.0.5/shellcheck_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellcheck-py
-Version: 0.9.0.4
+Version: 0.9.0.5
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
-    rev: v0.9.0.4
+    rev: v0.9.0.5
     hooks:
     -   id: shellcheck
 ```
 
 [shellcheck]: https://shellcheck.net
 [pre-commit]: https://pre-commit.com
```

