# Comparing `tmp/fosslight_scanner-1.7.8.tar.gz` & `tmp/fosslight_scanner-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fosslight_scanner-1.7.8.tar", last modified: Mon Jan  2 08:25:09 2023, max compression
+gzip compressed data, was "dist/fosslight_scanner-1.7.9.tar", last modified: Mon Jan 30 00:29:31 2023, max compression
```

## Comparing `fosslight_scanner-1.7.8.tar` & `fosslight_scanner-1.7.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       59 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7925 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6167 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      178 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1522 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/
--rwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1400 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/_get_input.py
--rw-r--r--   0 runner    (1001) docker     (116)     2208 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/_help.py
--rw-r--r--   0 runner    (1001) docker     (116)    10147 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/_run_compare.py
--rw-r--r--   0 runner    (1001) docker     (116)     2321 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     7240 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/common.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    15447 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/fosslight_scanner.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/resources/
--rw-r--r--   0 runner    (1001) docker     (116)     2240 2023-01-02 08:24:59.000000 fosslight_scanner-1.7.8/src/fosslight_scanner/resources/bom_compare.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7925 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      619 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      105 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      178 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2023-01-02 08:25:09.000000 fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     7925 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     6167 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1522 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/
+-rwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     1400 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/_get_input.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2208 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/_help.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10147 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/_run_compare.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2321 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     7240 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)    15447 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/fosslight_scanner.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/resources/
+-rw-r--r--   0 runner    (1001) docker     (116)     2240 2023-01-30 00:29:22.000000 fosslight_scanner-1.7.9/src/fosslight_scanner/resources/bom_compare.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7925 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      619 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       18 2023-01-30 00:29:31.000000 fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/top_level.txt
```

### Comparing `fosslight_scanner-1.7.8/LICENSE` & `fosslight_scanner-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/PKG-INFO` & `fosslight_scanner-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight_scanner
-Version: 1.7.8
+Version: 1.7.9
 Summary: FOSSLight Scanner
 Home-page: https://github.com/fosslight/fosslight_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_scanner-1.7.8/README.md` & `fosslight_scanner-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/setup.py` & `fosslight_scanner-1.7.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open('requirements.txt', 'r', 'utf-8') as f:
     required = f.read().splitlines()
 
 if __name__ == "__main__":
     setup(
         name='fosslight_scanner',
-        version='1.7.8',
+        version='1.7.9',
         package_dir={"": "src"},
         packages=find_packages(where='src'),
         description='FOSSLight Scanner',
         long_description=readme,
         long_description_content_type='text/markdown',
         license='Apache-2.0',
         author='LG Electronics',
```

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/_get_input.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/_get_input.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/_help.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/_help.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/_run_compare.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/_run_compare.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/cli.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/cli.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/common.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/common.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/fosslight_scanner.py` & `fosslight_scanner-1.7.9/src/fosslight_scanner/fosslight_scanner.py`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner/resources/bom_compare.html` & `fosslight_scanner-1.7.9/src/fosslight_scanner/resources/bom_compare.html`

 * *Files identical despite different names*

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/PKG-INFO` & `fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fosslight-scanner
-Version: 1.7.8
+Version: 1.7.9
 Summary: FOSSLight Scanner
 Home-page: https://github.com/fosslight/fosslight_scanner
 Author: LG Electronics
 License: Apache-2.0
 Download-URL: https://github.com/fosslight/fosslight_scanner
 Description: <!--
         Copyright (c) 2021 LG Electronics
```

### Comparing `fosslight_scanner-1.7.8/src/fosslight_scanner.egg-info/SOURCES.txt` & `fosslight_scanner-1.7.9/src/fosslight_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

