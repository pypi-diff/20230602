# Comparing `tmp/pyots-9.1.0b1.tar.gz` & `tmp/pyots-9.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.1.0b1.tar", last modified: Fri Jun  2 02:59:57 2023, max compression
+gzip compressed data, was "pyots-9.1.0b2.tar", last modified: Fri Jun  2 03:22:21 2023, max compression
```

## Comparing `pyots-9.1.0b1.tar` & `pyots-9.1.0b2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.738918 pyots-9.1.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 02:56:32.000000 pyots-9.1.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 02:56:32.000000 pyots-9.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 02:59:57.742918 pyots-9.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 02:56:32.000000 pyots-9.1.0b1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 02:56:32.000000 pyots-9.1.0b1/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 02:56:32.000000 pyots-9.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 02:56:32.000000 pyots-9.1.0b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 02:59:57.746919 pyots-9.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 02:56:32.000000 pyots-9.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 02:56:32.000000 pyots-9.1.0b1/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 02:56:32.000000 pyots-9.1.0b1/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 02:56:32.000000 pyots-9.1.0b1/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 02:59:57.000000 pyots-9.1.0b1/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 02:59:57.000000 pyots-9.1.0b1/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:59:57.000000 pyots-9.1.0b1/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:59:57.000000 pyots-9.1.0b1/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 02:59:57.000000 pyots-9.1.0b1/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:59:57.742918 pyots-9.1.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 02:56:32.000000 pyots-9.1.0b1/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 02:56:32.000000 pyots-9.1.0b1/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.330149 pyots-9.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 03:19:16.000000 pyots-9.1.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 03:19:16.000000 pyots-9.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 03:22:21.330149 pyots-9.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 03:19:16.000000 pyots-9.1.0b2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 03:19:16.000000 pyots-9.1.0b2/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 03:19:16.000000 pyots-9.1.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 03:19:16.000000 pyots-9.1.0b2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 03:22:21.330149 pyots-9.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 03:19:16.000000 pyots-9.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 03:19:16.000000 pyots-9.1.0b2/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.326149 pyots-9.1.0b2/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 03:22:21.000000 pyots-9.1.0b2/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:22:21.330149 pyots-9.1.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 03:19:16.000000 pyots-9.1.0b2/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 03:19:16.000000 pyots-9.1.0b2/tests/test_ots_suite.py
```

### Comparing `pyots-9.1.0b1/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0b2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0b2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/.github/workflows/codeql.yml` & `pyots-9.1.0b2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/.github/workflows/release.yml` & `pyots-9.1.0b2/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -93,10 +93,10 @@
         password: ${{ secrets.pypi_password }}
 
     - name: Create GitHub Release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
-        body: '${{ steps.date_tag.outputs.VERSION }}-released-${{ steps.date_tag.outputs.TODAY }}\n[Upstream OTS v${{ steps.date_tag.outputs.VERSION }} Release Notes](https://github.com/khaledhosny/ots/releases/tag/v${{ steps.date_tag.outputs.VERSION }})'
+        body: '${{ steps.date_tag.outputs.VERSION }} released ${{ steps.date_tag.outputs.TODAY }} - [Upstream OTS v${{ steps.date_tag.outputs.VERSION }} Release Notes](https://github.com/khaledhosny/ots/releases/tag/v${{ steps.date_tag.outputs.VERSION }})'
         prerelease: true
         files: ./dist/*
```

### Comparing `pyots-9.1.0b1/.github/workflows/run_tests.yml` & `pyots-9.1.0b2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/.gitignore` & `pyots-9.1.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/LICENSE` & `pyots-9.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/PKG-INFO` & `pyots-9.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0b1
+Version: 9.1.0b2
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0b1/README.md` & `pyots-9.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/build.py` & `pyots-9.1.0b2/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/setup.py` & `pyots-9.1.0b2/setup.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/src/_pyots/bindings.cpp` & `pyots-9.1.0b2/src/_pyots/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/src/_pyots/pyots-context.h` & `pyots-9.1.0b2/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/src/pyots/__init__.py` & `pyots-9.1.0b2/src/pyots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0b2/src/pyots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0b1
+Version: 9.1.0b2
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0b1/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0b2/src/pyots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/tests/test_compare_ots_python.py` & `pyots-9.1.0b2/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0b1/tests/test_ots_suite.py` & `pyots-9.1.0b2/tests/test_ots_suite.py`

 * *Files identical despite different names*

