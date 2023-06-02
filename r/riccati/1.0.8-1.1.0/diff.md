# Comparing `tmp/riccati-1.0.8.tar.gz` & `tmp/riccati-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riccati-1.0.8.tar", last modified: Mon Mar 20 19:00:34 2023, max compression
+gzip compressed data, was "riccati-1.1.0.tar", last modified: Fri Jun  2 15:34:10 2023, max compression
```

## Comparing `riccati-1.0.8.tar` & `riccati-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 19:00:23.000000 riccati-1.0.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-20 19:00:23.000000 riccati-1.0.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.111193 riccati-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.111193 riccati-1.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/ISSUE_TEMPLATE/issue-name.md
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.115193 riccati-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-20 19:00:23.000000 riccati-1.0.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-20 19:00:23.000000 riccati-1.0.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-20 19:00:23.000000 riccati-1.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-20 19:00:23.000000 riccati-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-20 19:00:34.123193 riccati-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-03-20 19:00:23.000000 riccati-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.115193 riccati-1.0.8/binder/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-20 19:00:23.000000 riccati-1.0.8/binder/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.119193 riccati-1.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1061269 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-20 19:00:23.000000 riccati-1.0.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-20 19:00:23.000000 riccati-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-20 19:00:23.000000 riccati-1.0.8/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-20 19:00:23.000000 riccati-1.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/chebutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/evolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/solversetup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/stepsize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-03-20 19:00:23.000000 riccati-1.0.8/riccati/tests/test_riccati.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 19:00:34.123193 riccati-1.0.8/riccati.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 19:00:34.000000 riccati-1.0.8/riccati.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 19:00:34.123193 riccati-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-03-20 19:00:23.000000 riccati-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 15:33:57.000000 riccati-1.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 15:33:57.000000 riccati-1.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/ISSUE_TEMPLATE/issue-name.md
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-02 15:33:57.000000 riccati-1.1.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 15:33:57.000000 riccati-1.1.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 15:33:57.000000 riccati-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 15:33:57.000000 riccati-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-02 15:33:57.000000 riccati-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-02 15:34:10.364724 riccati-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-02 15:33:57.000000 riccati-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/benchmarks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/data/eq237.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/fig1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-02 15:33:57.000000 riccati-1.1.0/benchmarks/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.360724 riccati-1.1.0/binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 15:33:57.000000 riccati-1.1.0/binder/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1062708 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81767 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 15:33:57.000000 riccati-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/joss-paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)   322295 2023-06-02 15:33:57.000000 riccati-1.1.0/joss-paper/timing-fig.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-06-02 15:33:57.000000 riccati-1.1.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 15:33:57.000000 riccati-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 15:33:57.000000 riccati-1.1.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 15:33:57.000000 riccati-1.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/chebutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13782 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/evolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/solversetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/stepsize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-06-02 15:33:57.000000 riccati-1.1.0/riccati/tests/test_riccati.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:34:10.364724 riccati-1.1.0/riccati.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 15:34:10.000000 riccati-1.1.0/riccati.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:34:10.364724 riccati-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-02 15:33:57.000000 riccati-1.1.0/setup.py
```

### Comparing `riccati-1.0.8/.github/ISSUE_TEMPLATE/issue-name.md` & `riccati-1.1.0/.github/ISSUE_TEMPLATE/issue-name.md`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/.github/workflows/tests.yml` & `riccati-1.1.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 on: 
   pull_request:
   push:
     branches:
       - master
       - docs
+      - joss-paper
   workflow_dispatch:
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
@@ -65,8 +66,23 @@
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
 
-
+  paper:
+    runs-on: ubuntu-latest
+    name: JOSS paper draft
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+      - name: Build draft pdf
+        uses: openjournals/openjournals-draft-action@master
+        with:
+          journal: joss
+          paper-path: joss-paper/paper.md
+      - name: Upload
+        uses: actions/upload-artifact@v1
+        with:
+          name: paper
+          path: joss-paper/paper.pdf
```

### Comparing `riccati-1.0.8/CONTRIBUTING.md` & `riccati-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/LICENSE` & `riccati-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/PKG-INFO` & `riccati-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.0.8
+Version: 1.1.0
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: plots
 License-File: LICENSE
 
+![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
+
+
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
 
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
```

### Comparing `riccati-1.0.8/README.md` & `riccati-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
+
+
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
 
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
```

### Comparing `riccati-1.0.8/docs/Makefile` & `riccati-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/docs/api.rst` & `riccati-1.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/docs/conf.py` & `riccati-1.1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,20 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
-exclude_patterns = []
+exclude_patterns = ["build"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 
 # -- Options for HTML output -------------------------------------------------
 
@@ -102,15 +102,15 @@
 # a list of builtin themes.
 #
 html_theme = 'sphinx_book_theme'
 html_copy_source = True
 html_show_sourcelink = True
 html_sourcelink_suffix = ""
 html_title = "riccati"
-#html_favicon = "bla.png"
+html_favicon = "favicon.ico"
 
 
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
```

### Comparing `riccati-1.0.8/docs/examples.ipynb` & `riccati-1.1.0/docs/examples.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931818181818182%*

 * *Differences: {"'cells'": "{insert: [(52, OrderedDict([('cell_type', 'markdown'), ('id', 'fe0975ab'), "*

 * *            "('metadata', OrderedDict()), ('source', ['## Benchmarks\\n', '\\n', '\\n', 'The "*

 * *            'left-hand-side of Fig. 5 in [the paper](https://arxiv.org/abs/2212.06924) describing '*

 * *            'the adaptive Riccati defect correction method (the algorithm behing `riccati`) shows '*

 * *            'a performance comparison between various other solvers developed for oscillatory '*

 * *            'second-order, line […]*

```diff
@@ -1115,14 +1115,57 @@
         {
             "cell_type": "markdown",
             "id": "f907ca82",
             "metadata": {},
             "source": [
                 "The progression of error is consistent with what we asked for -- $10^{-10}$ in the beginning and $10^{-8}$ in the oscillatory region."
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "fe0975ab",
+            "metadata": {},
+            "source": [
+                "## Benchmarks\n",
+                "\n",
+                "\n",
+                "The left-hand-side of Fig. 5 in [the paper](https://arxiv.org/abs/2212.06924) describing the adaptive Riccati defect correction method (the algorithm behing `riccati`) shows a performance comparison between various other solvers developed for oscillatory second-order, linear, homogeneous ODEs. The script to generate this figure is available in the `benchmarks/` folder in the Github repository. \n",
+                "\n",
+                "To run it, first make sure you have correctly initialized the git submodules in your cloned repository with\n",
+                "\n",
+                "```bash\n",
+                "git submodule init\n",
+                "git submodule update\n",
+                "```\n",
+                "\n",
+                "and that you have `gfortran` and `matlab` installed.\n",
+                "After [_installing riccati from source_](https://riccati.readthedocs.io/en/latest/installation/#from-source), and working from the installation directory, the benchmark script can be run as:\n",
+                "\n",
+                "```bash\n",
+                "cd benchmarks\n",
+                "pip install -r requirements.txt\n",
+                "python fig1.py\n",
+                "```"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f0107607",
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "44a46b99",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "celltoolbar": "Tags",
         "kernelspec": {
             "display_name": "riccatipip",
             "language": "python",
```

### Comparing `riccati-1.0.8/docs/index.rst` & `riccati-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/docs/installation.rst` & `riccati-1.1.0/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 If you installed from source
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Once you're in the installation directory, execute the tests via
 
 .. code-block:: bash
     
-   python -m pytest -v tests
+   python -m pytest -v
 
 
 If you used a package manager
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Change directory to the location of the installed package, which might be something like
 
@@ -84,10 +84,10 @@
 - virtualenv and pip: `<path-to-env>/lib/python<3.n>/site-packages/riccati` with `<path-to-env>` being the path to your virtual environment.
 
 Then execute the tests:
 
 .. code-block:: bash
 
     cd <location-of-riccati>
-    python -m pytest -v tests
+    python -m pytest -v
```

### Comparing `riccati-1.0.8/docs/quickstart.ipynb` & `riccati-1.1.0/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/__init__.py` & `riccati-1.1.0/riccati/__init__.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/chebutils.py` & `riccati-1.1.0/riccati/chebutils.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/evolve.py` & `riccati-1.1.0/riccati/evolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import warnings
 from riccati.chebutils import integrationm, interp
 from riccati.stepsize import choose_osc_stepsize, choose_nonosc_stepsize
 from riccati.step import osc_step, nonosc_step
+import warnings
 
 def osc_evolve(info, x0, x1, h, y0, epsres = 1e-12, epsh = 1e-12):
     """
     Allows continuous evolution between the independent variable values `x0`
     and `x1`. Starting from `x0` and `y = [y0, yd0]`, this function takes a
     Riccati step of size `h` or until `x1` is reached, and updates the
     attributes of `info` such that it can be called inside a `while` loop.
@@ -152,15 +153,15 @@
         hslo_ini = sign*min(1e8, np.abs(1/wnext))
         # Check if estimate for next stepsize would be out of range
         if sign*(info.x + hslo_ini) > sign*x1:
             hslo_ini = x1 - info.x
         info.h = choose_nonosc_stepsize(info, info.x, hslo_ini, epsh = epsh)  
     return success
 
-def solve(info, xi, xf, yi, dyi, eps = 1e-12, epsh = 1e-12, xeval = np.array([]), hard_stop = False):
+def solve(info, xi, xf, yi, dyi, eps = 1e-12, epsh = 1e-12, xeval = np.array([]), hard_stop = False, warn = False):
     """
     Solves y'' + 2gy' + w^2y = 0 on the interval (xi, xf), starting from the
     initial conditions y(xi) = yi, y'(xi) = dyi. Keeps the residual of the ODE
     below eps, and returns an interpolated solution (dense output) at points
     xeval.
 
     Parameters
@@ -178,28 +179,40 @@
     xeval: list
         List of x-values where the solution is to be interpolated (dense output) and returned.
     hard_stop: bool
         Whether to force the solver to have a potentially smaller last
         stepsize, in order to stop exactly at `xf` (rather than allowing the
         solver to step over it and get the value of the solution by
         interpolation).
+    warn: bool
+        Whether to display warnings, e.g. RuntimeWarnings, during a run. Due to
+        the high level of adaptivity in this algorithm, it may throw several
+        RuntimeWarnings even in a standard setup as it chooses the type of
+        step, stepsize, and other parameters. For this reason, all warnings are
+        silenced by default (`warn = False`). Set to `True` if you wish to see
+        the warnings.
 
     Returns
     -------
     xs: list [float]
         Values of the independent variable at the internal steps of the solver.
     ys, dys: list [complex]
         Values of the dependent variable and its derivative at the internal steps of the solver.
     successes: list [int]
         Has elements 1 and 0: 1 denoting each successful step, 0 denoting unsuccessful steps. 
     phases:  list [complex]
         Complex phase of the solution accumulated during each successful Riccati step.
     steptypes: list [int]
         Types of successful steps taken: 1 for Riccati and 0 for Chebyshev. 
     """
+    if warn == False:
+        warnings.simplefilter("ignore")
+    else:
+        warnings.simplefilter("default")
+
     w = info.w
     g = info.g
     Dn = info.Dn
     xn = info.xn
     n = info.n
     p = info.p
     hi = info.h0 # Initial stepsize for calculating derivatives
```

### Comparing `riccati-1.0.8/riccati/solversetup.py` & `riccati-1.1.0/riccati/solversetup.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/step.py` & `riccati-1.1.0/riccati/step.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/stepsize.py` & `riccati-1.1.0/riccati/stepsize.py`

 * *Files identical despite different names*

### Comparing `riccati-1.0.8/riccati/tests/test_riccati.py` & `riccati-1.1.0/riccati/tests/test_riccati.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     Neval = int(1e2)
     xeval = np.linspace(xi-10.0, xi, Neval) 
     # Turn on warnings
     warnings.simplefilter("always")
     with warnings.catch_warnings(record = True) as w:
         xs, ys, dys, ss, ps, stypes, yeval = solve(info, xi, xf, yi, dyi,\
                                                            xeval = xeval,\
-                                                           eps = eps, epsh = epsh)
+                                                           eps = eps, epsh = epsh, warn = True)
         assert "outside the integration range" in str(w[0].message) 
 
 def test_quadwts():
     a = 3.0
     f = lambda x: np.sin(a*x + 1.0)
     df = lambda x: a*np.cos(a*x + 1.0)
     for i in [16, 32]:
```

### Comparing `riccati-1.0.8/riccati.egg-info/PKG-INFO` & `riccati-1.1.0/riccati.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: riccati
-Version: 1.0.8
+Version: 1.1.0
 Summary: adaptive Riccati defect correction solver
 Home-page: 
 Author: Fruzsina J Agocs and Alex H Barnett
 Author-email: 
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: plots
 License-File: LICENSE
 
+![Riccati logo](https://github.com/fruzsinaagocs/riccati/blob/master/logo.png?raw=true)
+
+
 # riccati
 
 **A package implementing the adaptive Riccati defect correction (ARDC) method**
 
 
 [![Documentation Status](https://readthedocs.org/projects/riccati/badge/?version=latest)](https://riccati.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/fruzsinaagocs/riccati/branch/master/graph/badge.svg?token=XA47G7P1XM)](https://codecov.io/gh/fruzsinaagocs/riccati)
```

### Comparing `riccati-1.0.8/setup.py` & `riccati-1.1.0/setup.py`

 * *Files identical despite different names*

