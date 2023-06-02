# Comparing `tmp/pyots-9.0.0.tar.gz` & `tmp/pyots-9.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyots-9.0.0.tar", last modified: Thu Sep 15 15:21:30 2022, max compression
+gzip compressed data, was "pyots-9.1.0a0.tar", last modified: Fri Jun  2 00:39:14 2023, max compression
```

## Comparing `pyots-9.0.0.tar` & `pyots-9.1.0a0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-15 15:18:28.000000 pyots-9.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.080217 pyots-9.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      538 2022-09-15 15:18:28.000000 pyots-9.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-09-15 15:18:28.000000 pyots-9.0.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-09-15 15:18:28.000000 pyots-9.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-15 15:18:28.000000 pyots-9.0.0/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-09-15 15:18:28.000000 pyots-9.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-09-15 15:18:28.000000 pyots-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-09-15 15:21:30.084217 pyots-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2022-09-15 15:18:28.000000 pyots-9.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)     2403 2022-09-15 15:18:28.000000 pyots-9.0.0/build.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-15 15:18:28.000000 pyots-9.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-15 15:18:28.000000 pyots-9.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-15 15:21:30.084217 pyots-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    10091 2022-09-15 15:18:28.000000 pyots-9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.080217 pyots-9.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/src/_pyots/
--rw-r--r--   0 runner    (1001) docker     (121)     4148 2022-09-15 15:18:28.000000 pyots-9.0.0/src/_pyots/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-09-15 15:18:28.000000 pyots-9.0.0/src/_pyots/pyots-context.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/src/pyots/
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-09-15 15:18:28.000000 pyots-9.0.0/src/pyots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/src/pyots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5683 2022-09-15 15:21:30.000000 pyots-9.0.0/src/pyots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-09-15 15:21:30.000000 pyots-9.0.0/src/pyots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 15:21:30.000000 pyots-9.0.0/src/pyots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 15:21:30.000000 pyots-9.0.0/src/pyots.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-15 15:21:30.000000 pyots-9.0.0/src/pyots.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 15:21:30.084217 pyots-9.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2987 2022-09-15 15:18:28.000000 pyots-9.0.0/tests/test_compare_ots_python.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-09-15 15:18:28.000000 pyots-9.0.0/tests/test_ots_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-02 00:35:42.000000 pyots-9.1.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-02 00:35:42.000000 pyots-9.1.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 00:39:14.214023 pyots-9.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-02 00:35:42.000000 pyots-9.1.0a0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-06-02 00:35:42.000000 pyots-9.1.0a0/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-02 00:35:42.000000 pyots-9.1.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 00:35:42.000000 pyots-9.1.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 00:39:14.214023 pyots-9.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-06-02 00:35:42.000000 pyots-9.1.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.210023 pyots-9.1.0a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/_pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/_pyots/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/_pyots/pyots-context.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/pyots/
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 00:35:42.000000 pyots-9.1.0a0/src/pyots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/src/pyots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 00:39:14.000000 pyots-9.1.0a0/src/pyots.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:39:14.214023 pyots-9.1.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-02 00:35:42.000000 pyots-9.1.0a0/tests/test_compare_ots_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-02 00:35:42.000000 pyots-9.1.0a0/tests/test_ots_suite.py
```

### Comparing `pyots-9.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pyots-9.1.0a0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pyots-9.1.0a0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/.github/workflows/release.yml` & `pyots-9.1.0a0/.github/workflows/release.yml`

 * *Files 5% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 
     - name: Log reason (manual run only)
       if: github.event_name == 'workflow_dispatch'
       run: |
         echo "Reason for triggering: ${{ github.event.inputs.reason }}"
 
     - name: Check out
-      uses: actions/checkout@v2
+      uses: actions/checkout@v3
       with:
         fetch-depth: 0  # unshallow fetch for setuptools-scm
 
     - name: Install Python 3.9
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.9'
 
     - name: Build wheel
-      uses: pypa/cibuildwheel@v2.3.0
+      uses: pypa/cibuildwheel@v2.13.0
       with:
         output-dir: dist
       env:
-        CIBW_BUILD: "cp37-* cp38-* cp39-* cp310-*"
+        CIBW_BUILD: "cp38-* cp39-* cp310-* cp311-*"
         CIBW_ARCHS_MACOS: x86_64 universal2
         CIBW_ARCHS_LINUX: x86_64
         CIBW_MANYLINUX_X86_64_IMAGE: manylinux2014
         CIBW_SKIP: "*musllinux*"
         CIBW_BEFORE_ALL_LINUX: "yum install -y libuuid-devel"
 
     - name: Build sdist (Ubuntu only)
```

### Comparing `pyots-9.0.0/.github/workflows/run_tests.yml` & `pyots-9.1.0a0/.github/workflows/run_tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Log reason (manual run only)
       if: github.event_name == 'workflow_dispatch'
       run: |
         echo "Reason for triggering: ${{ github.event.inputs.reason }}"
 
     - name: Set up Python 3.8
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
```

### Comparing `pyots-9.0.0/.gitignore` & `pyots-9.1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/LICENSE` & `pyots-9.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/PKG-INFO` & `pyots-9.1.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.0.0
+Version: 9.1.0a0
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyots (PYthon OT Sanitizer)
@@ -30,15 +30,15 @@
 ![macOS](https://img.shields.io/badge/-macOS-lightgrey) ![ubuntu](https://img.shields.io/badge/-ubuntu-lightgrey)
 
 Python wrapper for [OpenType Sanitizer](https://github.com/khaledhosny/ots), also known as just "OTS". It is similar to and partially based on [ots-python](https://github.com/googlefonts/ots-python), but builds OTS as a Python C Extension (instead of as an executable and calling through `subprocess` as ots-python does).
 
 **NOTE:** Although this package is similar to **ots-python**, it is _not_ a drop-in replacement for it, as the Python API is different.
 
 ## Requirements
-The project builds `pip`-installable wheels for Python 3.7, 3.8, 3.9 or 3.10 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
+The project builds `pip`-installable wheels for Python 3.8, 3.9, 3.10 or 3.11 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
 
 ## Installation with `pip`
 If you just want to _use_ `pyots`, you can simply run `python -m pip install -U pyots` (in one of the supported platforms/Python versions) which will install pre-built, compiled, ready-to-use Python wheels. Then you can skip down to the [Use](#Use) section.
 
 ## Installation/setup for developing `pyots`
 If you'd like to tinker with the `pyots` code, you will want to get your local setup ready:
  - clone this repo
```

### Comparing `pyots-9.0.0/README.md` & `pyots-9.1.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ![macOS](https://img.shields.io/badge/-macOS-lightgrey) ![ubuntu](https://img.shields.io/badge/-ubuntu-lightgrey)
 
 Python wrapper for [OpenType Sanitizer](https://github.com/khaledhosny/ots), also known as just "OTS". It is similar to and partially based on [ots-python](https://github.com/googlefonts/ots-python), but builds OTS as a Python C Extension (instead of as an executable and calling through `subprocess` as ots-python does).
 
 **NOTE:** Although this package is similar to **ots-python**, it is _not_ a drop-in replacement for it, as the Python API is different.
 
 ## Requirements
-The project builds `pip`-installable wheels for Python 3.7, 3.8, 3.9 or 3.10 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
+The project builds `pip`-installable wheels for Python 3.8, 3.9, 3.10 or 3.11 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
 
 ## Installation with `pip`
 If you just want to _use_ `pyots`, you can simply run `python -m pip install -U pyots` (in one of the supported platforms/Python versions) which will install pre-built, compiled, ready-to-use Python wheels. Then you can skip down to the [Use](#Use) section.
 
 ## Installation/setup for developing `pyots`
 If you'd like to tinker with the `pyots` code, you will want to get your local setup ready:
  - clone this repo
```

### Comparing `pyots-9.0.0/build.py` & `pyots-9.1.0a0/build.py`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/setup.py` & `pyots-9.1.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,27 +189,26 @@
                 # response is not seekable so we first download *.tar.xz to an
                 # in-memory file, and then extract all files to the output_dir
                 f = io.BytesIO()
                 with urlopen(self.url) as response:
                     f.write(response.read())
                 f.seek(0)
 
-            # use hashlib to verify the SHA-256 hash
-            actual_sha256 = hashlib.sha256(f.getvalue()).hexdigest()
-            if actual_sha256 != self.sha256:
-                from distutils.errors import DistutilsSetupError
-
-                raise DistutilsSetupError(
-                    "invalid SHA-256 checksum:\n"
-                    "actual:   {}\n"
-                    "expected: {}".format(actual_sha256, self.sha256)
-                )
+                # use hashlib to verify the SHA-256 hash
+                actual_sha256 = hashlib.sha256(f.getvalue()).hexdigest()
+                if actual_sha256 != self.sha256:
+                    from distutils.errors import DistutilsSetupError
+
+                    raise DistutilsSetupError(
+                        "invalid SHA-256 checksum:\n"
+                        "actual:   {}\n"
+                        "expected: {}".format(actual_sha256, self.sha256)
+                    )
 
-            log.info("unarchiving {} to {}".format(archive_name, output_dir))
-            if not self.dry_run:
+                log.info("unarchiving {} to {}".format(archive_name, output_dir))
                 with lzma.open(f) as xz:
                     with tarfile.open(fileobj=xz) as tar:
                         filelist = tar.getmembers()
                         first = filelist[0]
                         if not (first.isdir() and first.name.startswith("ots")):  # noqa: E501
                             from distutils.errors import DistutilsSetupError
 
@@ -262,32 +261,32 @@
     'download': Download,
     'egg_info': CustomEggInfo
 }
 
 pyots_mod = Extension(
     name='_pyots',
     libraries=['z'],
-    extra_compile_args=['-fPIC', '-std=c++17'],
+    extra_compile_args=['-fPIC', '-std=c++11'],
     extra_objects=_get_extra_objects(),
     include_dirs=_get_include_dirs(),
     sources=_get_sources(),
 )
 
 with io.open("README.md", encoding="utf-8") as readme:
     long_description = readme.read()
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Testing',
     'License :: OSI Approved :: BSD License',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Operating System :: MacOS :: MacOS X',
     'Operating System :: POSIX :: Linux',
 ]
 
 setup(
     author='Adobe Type team & friends',
     author_email='afdko@adobe.com',
```

### Comparing `pyots-9.0.0/src/_pyots/bindings.cpp` & `pyots-9.1.0a0/src/_pyots/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 #include "ots-memory-stream.h"
 #include "pyots-context.h"
 
 
 static PyObject* method_sanitize(PyObject* self, PyObject* args) {
   PyObject* pyInFilenameObj;
   PyObject* pyOutFilenameObj;
-  bool quiet;
+  int quiet = 0;
   int kwFontIndex = -1;
 
   /* parse the Python args */
-  if (!PyArg_ParseTuple(args, "O&O&pi",
+  if (!PyArg_ParseTuple(args, "O&O&ii",
                         PyUnicode_FSConverter, &pyInFilenameObj,
                         PyUnicode_FSConverter, &pyOutFilenameObj,
                         &quiet,
                         &kwFontIndex)) {
     return NULL;
   }
```

### Comparing `pyots-9.0.0/src/_pyots/pyots-context.h` & `pyots-9.1.0a0/src/_pyots/pyots-context.h`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/src/pyots/__init__.py` & `pyots-9.1.0a0/src/pyots/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     Returns an OTSResult with the following attributes:
         sanitized (bool)    File was successfully sanitized
         modified (bool)     Modifications were necessary to sanitize the input
                             file (SEE README.md!)
         messages (string)   Messages generated during sanitzation (empty if
                             'quiet' was specified as True).
     """
-    # (san, mod, rmsg) = _pyots._sanitize(input, output or os.devnull, quiet, font_index)
     (san, mod, rmsg) = _pyots._sanitize(input, output or '', quiet, font_index)
 
     if rmsg is not None:
         if isinstance(rmsg, bytes):
             msg = rmsg.decode('ascii', errors='backslashreplace')
         else:
             msg = rmsg
```

### Comparing `pyots-9.0.0/src/pyots.egg-info/PKG-INFO` & `pyots-9.1.0a0/src/pyots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyots
-Version: 9.0.0
+Version: 9.1.0a0
 Summary: Python wrapper for ot-sanitizer
 Home-page: https://github.com/adobe-type-tools/pyots
 Author: Adobe Type team & friends
 Author-email: afdko@adobe.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyots (PYthon OT Sanitizer)
@@ -30,15 +30,15 @@
 ![macOS](https://img.shields.io/badge/-macOS-lightgrey) ![ubuntu](https://img.shields.io/badge/-ubuntu-lightgrey)
 
 Python wrapper for [OpenType Sanitizer](https://github.com/khaledhosny/ots), also known as just "OTS". It is similar to and partially based on [ots-python](https://github.com/googlefonts/ots-python), but builds OTS as a Python C Extension (instead of as an executable and calling through `subprocess` as ots-python does).
 
 **NOTE:** Although this package is similar to **ots-python**, it is _not_ a drop-in replacement for it, as the Python API is different.
 
 ## Requirements
-The project builds `pip`-installable wheels for Python 3.7, 3.8, 3.9 or 3.10 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
+The project builds `pip`-installable wheels for Python 3.8, 3.9, 3.10 or 3.11 under Mac or Linux. It is possible this project will build and run with other Pythons and other operating systems, but it has only been tested with the listed configurations.
 
 ## Installation with `pip`
 If you just want to _use_ `pyots`, you can simply run `python -m pip install -U pyots` (in one of the supported platforms/Python versions) which will install pre-built, compiled, ready-to-use Python wheels. Then you can skip down to the [Use](#Use) section.
 
 ## Installation/setup for developing `pyots`
 If you'd like to tinker with the `pyots` code, you will want to get your local setup ready:
  - clone this repo
```

### Comparing `pyots-9.0.0/src/pyots.egg-info/SOURCES.txt` & `pyots-9.1.0a0/src/pyots.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 build.py
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
+.github/workflows/codeql.yml
 .github/workflows/release.yml
 .github/workflows/run_tests.yml
 /home/runner/work/pyots/pyots/src/_pyots/bindings.cpp
 src/_pyots/bindings.cpp
 src/_pyots/pyots-context.h
 src/pyots/__init__.py
 src/pyots.egg-info/PKG-INFO
```

### Comparing `pyots-9.0.0/tests/test_compare_ots_python.py` & `pyots-9.1.0a0/tests/test_compare_ots_python.py`

 * *Files identical despite different names*

### Comparing `pyots-9.0.0/tests/test_ots_suite.py` & `pyots-9.1.0a0/tests/test_ots_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
         r = pyots.sanitize(f)
 
         if r.sanitized:
             count += 1
             print("[bad] unexpected success on", f, "\n".join(r.messages))
 
-    assert not count, f"{count} file{'s were' if count != 1 else 'was'} sanitized when expected to be sanitized."  # noqa: E501
+    assert not count, f"{count} file{'s were' if count != 1 else 'was'} sanitized successfully when expected to fail."  # noqa: E501
 
 
 def test_ots_fuzzing():
 
     tld = TEST_FONTS_DIR / "fuzzing"
 
     count = 0
```

