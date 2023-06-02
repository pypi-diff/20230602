# Comparing `tmp/pyots-9.1.0a1.tar.gz` & `tmp/pyots-9.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.1.0a1.tar", last modified: Fri Jun  2 01:23:02 2023, max compression
+gzip compressed data, was "pyots-9.1.0a2.tar", last modified: Fri Jun  2 01:46:06 2023, max compression
```

## Comparing `pyots-9.1.0a1.tar` & `pyots-9.1.0a2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.629121 pyots-9.1.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 01:19:28.000000 pyots-9.1.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:23:02.633122 pyots-9.1.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 01:19:28.000000 pyots-9.1.0a1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 01:19:28.000000 pyots-9.1.0a1/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 01:19:28.000000 pyots-9.1.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 01:19:28.000000 pyots-9.1.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 01:23:02.633122 pyots-9.1.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 01:19:28.000000 pyots-9.1.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.629121 pyots-9.1.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 01:19:28.000000 pyots-9.1.0a1/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 01:19:28.000000 pyots-9.1.0a1/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.332594 pyots-9.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 01:43:23.000000 pyots-9.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 01:43:23.000000 pyots-9.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:46:06.332594 pyots-9.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 01:43:23.000000 pyots-9.1.0a2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 01:43:23.000000 pyots-9.1.0a2/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 01:43:23.000000 pyots-9.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 01:43:23.000000 pyots-9.1.0a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 01:46:06.332594 pyots-9.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 01:43:23.000000 pyots-9.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 01:43:23.000000 pyots-9.1.0a2/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 01:43:23.000000 pyots-9.1.0a2/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.328594 pyots-9.1.0a2/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 01:43:23.000000 pyots-9.1.0a2/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.332594 pyots-9.1.0a2/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:46:06.000000 pyots-9.1.0a2/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 01:46:06.000000 pyots-9.1.0a2/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:46:06.000000 pyots-9.1.0a2/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:46:06.000000 pyots-9.1.0a2/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 01:46:06.000000 pyots-9.1.0a2/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:46:06.332594 pyots-9.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 01:43:23.000000 pyots-9.1.0a2/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 01:43:23.000000 pyots-9.1.0a2/tests/test_ots_suite.py
```

### Comparing `pyots-9.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0a2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0a2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/.github/workflows/codeql.yml` & `pyots-9.1.0a2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/.github/workflows/release.yml` & `pyots-9.1.0a2/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     - name: Build wheel
       uses: pypa/cibuildwheel@v2.13.0
       with:
         output-dir: dist
       env:
         CIBW_BUILD: "cp38-* cp39-* cp310-* cp311-*"
-        CIBW_ARCHS_MACOS: x86_64 universal2
+        CIBW_ARCHS_MACOS: x86_64 arm64
         CIBW_ARCHS_LINUX: x86_64
         CIBW_MANYLINUX_X86_64_IMAGE: manylinux2014
         CIBW_SKIP: "*musllinux*"
         CIBW_BEFORE_ALL_LINUX: "yum install -y libuuid-devel"
 
     - name: Build sdist (Ubuntu only)
       if: matrix.os == 'ubuntu-latest'
@@ -92,10 +92,10 @@
         password: ${{ secrets.pypi_password }}
 
     - name: Create GitHub Release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
-        body: "{{ steps.date_tag.outputs.VERSION }}-released-${{ steps.date_tag.outputs.TODAY }}"
+        body: "${{ steps.date_tag.outputs.VERSION }}-released-${{ steps.date_tag.outputs.TODAY }}"
         prerelease: true
         files: ./dist/*
```

### Comparing `pyots-9.1.0a1/.github/workflows/run_tests.yml` & `pyots-9.1.0a2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/.gitignore` & `pyots-9.1.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/LICENSE` & `pyots-9.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/PKG-INFO` & `pyots-9.1.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0a1
+Version: 9.1.0a2
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0a1/README.md` & `pyots-9.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/build.py` & `pyots-9.1.0a2/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/setup.py` & `pyots-9.1.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/src/_pyots/bindings.cpp` & `pyots-9.1.0a2/src/_pyots/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/src/_pyots/pyots-context.h` & `pyots-9.1.0a2/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/src/pyots/__init__.py` & `pyots-9.1.0a2/src/pyots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0a2/src/pyots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0a1
+Version: 9.1.0a2
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0a1/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0a2/src/pyots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/tests/test_compare_ots_python.py` & `pyots-9.1.0a2/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a1/tests/test_ots_suite.py` & `pyots-9.1.0a2/tests/test_ots_suite.py`

 * *Files identical despite different names*

