# Comparing `tmp/pyots-9.1.0a0.tar.gz` & `tmp/pyots-9.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.1.0a0.tar", last modified: Fri Jun  2 00:39:14 2023, max compression
+gzip compressed data, was "pyots-9.1.0a1.tar", last modified: Fri Jun  2 01:23:02 2023, max compression
```

## Comparing `pyots-9.1.0a0.tar` & `pyots-9.1.0a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 00:35:42.000000 pyots-9.1.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 00:39:14.214023 pyots-9.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 00:35:42.000000 pyots-9.1.0a0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 00:35:42.000000 pyots-9.1.0a0/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 00:35:42.000000 pyots-9.1.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 00:35:42.000000 pyots-9.1.0a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 00:39:14.214023 pyots-9.1.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 00:35:42.000000 pyots-9.1.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 00:35:42.000000 pyots-9.1.0a0/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 00:35:42.000000 pyots-9.1.0a0/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.629121 pyots-9.1.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 01:19:28.000000 pyots-9.1.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 01:19:28.000000 pyots-9.1.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:23:02.633122 pyots-9.1.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 01:19:28.000000 pyots-9.1.0a1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 01:19:28.000000 pyots-9.1.0a1/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 01:19:28.000000 pyots-9.1.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 01:19:28.000000 pyots-9.1.0a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 01:23:02.633122 pyots-9.1.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 01:19:28.000000 pyots-9.1.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.629121 pyots-9.1.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 01:19:28.000000 pyots-9.1.0a1/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 01:23:02.000000 pyots-9.1.0a1/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:23:02.633122 pyots-9.1.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 01:19:28.000000 pyots-9.1.0a1/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 01:19:28.000000 pyots-9.1.0a1/tests/test_ots_suite.py
```

### Comparing `pyots-9.1.0a0/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0a1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0a1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/.github/workflows/codeql.yml` & `pyots-9.1.0a1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/.github/workflows/release.yml` & `pyots-9.1.0a1/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     - name: Build sdist (Ubuntu only)
       if: matrix.os == 'ubuntu-latest'
       run: |
         python setup.py sdist
 
     - name: Upload build artifacts
-      uses: actions/upload-artifact@v2
+      uses: actions/upload-artifact@v3
       with:
         name: wheelstorage
         path: ./dist/*
         if-no-files-found: error
         retention-days: 30
 
   publish_release:
@@ -71,20 +71,20 @@
     - name: Get date & flat tag
       id: date_tag
       run: |
         export DATE=$(TZ=US/Pacific date +'%Y-%m-%d')
         echo $DATE
         export FLAT_TAG=$(echo ${GITHUB_REF##*/} | sed 's/\.//g')
         echo $FLAT_TAG
-        echo ::set-output name=TODAY::$DATE
-        echo ::set-output name=VERSION::$FLAT_TAG
+        echo "TODAY={$DATE}" >> "$GITHUB_OUTPUT"
+        echo "VERSION={$FLAT_TAG}" >> "$GITHUB_OUTPUT"
       shell: bash
 
     - name: Download release assets
-      uses: actions/download-artifact@v2
+      uses: actions/download-artifact@v3
       with:
         name: wheelstorage
         path: dist
 
     - name: Publish dist(s) to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
@@ -92,10 +92,10 @@
         password: ${{ secrets.pypi_password }}
 
     - name: Create GitHub Release
       uses: softprops/action-gh-release@v1
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
-        body: '{{ steps.date_tag.outputs.VERSION }}-released-${{ steps.date_tag.outputs.TODAY }}'
+        body: "{{ steps.date_tag.outputs.VERSION }}-released-${{ steps.date_tag.outputs.TODAY }}"
         prerelease: true
         files: ./dist/*
```

### Comparing `pyots-9.1.0a0/.github/workflows/run_tests.yml` & `pyots-9.1.0a1/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/.gitignore` & `pyots-9.1.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/LICENSE` & `pyots-9.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/PKG-INFO` & `pyots-9.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0a0
+Version: 9.1.0a1
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0a0/README.md` & `pyots-9.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/build.py` & `pyots-9.1.0a1/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/setup.py` & `pyots-9.1.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/src/_pyots/bindings.cpp` & `pyots-9.1.0a1/src/_pyots/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/src/_pyots/pyots-context.h` & `pyots-9.1.0a1/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/src/pyots/__init__.py` & `pyots-9.1.0a1/src/pyots/__init__.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0a1/src/pyots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.1.0a0
+Version: 9.1.0a1
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyots-9.1.0a0/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0a1/src/pyots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/tests/test_compare_ots_python.py` & `pyots-9.1.0a1/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.1.0a0/tests/test_ots_suite.py` & `pyots-9.1.0a1/tests/test_ots_suite.py`

 * *Files identical despite different names*

