# Comparing `tmp/treecker-1.2.0.tar.gz` & `tmp/treecker-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treecker-1.2.0.tar", last modified: Sat Apr  1 18:33:44 2023, max compression
+gzip compressed data, was "treecker-1.3.0.tar", last modified: Fri Jun  2 04:11:55 2023, max compression
```

## Comparing `treecker-1.2.0.tar` & `treecker-1.3.0.tar`

### file list

```diff
@@ -1,62 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.497306 treecker-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-04-01 18:33:05.000000 treecker-1.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-04-01 18:33:05.000000 treecker-1.2.0/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-01 18:33:05.000000 treecker-1.2.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-04-01 18:33:05.000000 treecker-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3176 2023-04-01 18:33:44.496306 treecker-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2436 2023-04-01 18:33:05.000000 treecker-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.483305 treecker-1.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.484305 treecker-1.2.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.484305 treecker-1.2.0/docs/source/practice/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.485305 treecker-1.2.0/docs/source/practice/examples/
--rw-rw-rw-   0 root         (0) root         (0)     2887 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/examples/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/examples/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/examples/vanilla.rst
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.487305 treecker-1.2.0/docs/source/practice/installation/
--rw-rw-rw-   0 root         (0) root         (0)     1466 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/installation/editable.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/installation/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      814 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/installation/regular.rst
--rw-rw-rw-   0 root         (0) root         (0)     3805 2023-04-01 18:33:05.000000 treecker-1.2.0/docs/source/practice/installation/venv.rst
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-01 18:33:05.000000 treecker-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 18:33:44.497306 treecker-1.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2987 2023-04-01 18:33:05.000000 treecker-1.2.0/setup.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.478304 treecker-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.488305 treecker-1.2.0/src/treecker/
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/__main__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.492305 treecker-1.2.0/src/treecker/core/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      988 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     2417 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/naming.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     3695 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/core/tree.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/default.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.494305 treecker-1.2.0/src/treecker/main/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/main/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2232 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/main/commit.py
--rw-rw-rw-   0 root         (0) root         (0)     1615 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/main/init.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/main/issues.py
--rw-rw-rw-   0 root         (0) root         (0)     2349 2023-04-01 18:33:05.000000 treecker-1.2.0/src/treecker/main/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.490305 treecker-1.2.0/src/treecker.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3176 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1249 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-01 18:33:44.000000 treecker-1.2.0/src/treecker.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.495305 treecker-1.2.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.480304 treecker-1.2.0/tests/material/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.495305 treecker-1.2.0/tests/material/inputs/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/material/inputs/commit-n.txt
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/material/inputs/commit-y.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.496306 treecker-1.2.0/tests/material/tracked/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/material/tracked/file.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:33:44.496306 treecker-1.2.0/tests/material/tracked/subdir/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/material/tracked/subdir/setup.sh
--rwxrwxrwx   0 root         (0) root         (0)     1365 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/references.json
--rwxrwxrwx   0 root         (0) root         (0)     6337 2023-04-01 18:33:05.000000 treecker-1.2.0/tests/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.786734 treecker-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-06-02 04:11:24.000000 treecker-1.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-06-02 04:11:24.000000 treecker-1.3.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-06-02 04:11:24.000000 treecker-1.3.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-02 04:11:24.000000 treecker-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-06-02 04:11:55.786734 treecker-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2425 2023-06-02 04:11:24.000000 treecker-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.778484 treecker-1.3.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.779400 treecker-1.3.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.779400 treecker-1.3.0/docs/source/practice/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.779400 treecker-1.3.0/docs/source/practice/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     2986 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/examples/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/examples/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/examples/vanilla.rst
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.780317 treecker-1.3.0/docs/source/practice/installation/
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/installation/editable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/installation/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      814 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/installation/regular.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2023-06-02 04:11:24.000000 treecker-1.3.0/docs/source/practice/installation/venv.rst
+-rw-rw-rw-   0 root         (0) root         (0)      964 2023-06-02 04:11:24.000000 treecker-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 04:11:55.786734 treecker-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3024 2023-06-02 04:11:24.000000 treecker-1.3.0/setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.776650 treecker-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.781234 treecker-1.3.0/src/treecker/
+-rw-rw-rw-   0 root         (0) root         (0)      415 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2386 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.783984 treecker-1.3.0/src/treecker/core/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4595 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/contents.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/display.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     5056 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/core/tree.py
+-rw-rw-rw-   0 root         (0) root         (0)      874 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/default.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.784900 treecker-1.3.0/src/treecker/main/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/main/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2259 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/main/commit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1615 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/main/init.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/main/issues.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2023-06-02 04:11:24.000000 treecker-1.3.0/src/treecker/main/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.783067 treecker-1.3.0/src/treecker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3165 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-02 04:11:55.000000 treecker-1.3.0/src/treecker.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.784900 treecker-1.3.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.777567 treecker-1.3.0/tests/material/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.785817 treecker-1.3.0/tests/material/corrupted/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/corrupted/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/corrupted/file.jpg
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/corrupted/file.pdf
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/corrupted/file.tar
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/corrupted/file.zip
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.785817 treecker-1.3.0/tests/material/inputs/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/inputs/commit-n.txt
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/inputs/commit-y.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.786734 treecker-1.3.0/tests/material/tracked/
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/tracked/file.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 04:11:55.786734 treecker-1.3.0/tests/material/tracked/subdir/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/material/tracked/subdir/setup.sh
+-rwxrwxrwx   0 root         (0) root         (0)     1343 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/references.json
+-rwxrwxrwx   0 root         (0) root         (0)     6737 2023-06-02 04:11:24.000000 treecker-1.3.0/tests/run.py
```

### Comparing `treecker-1.2.0/LICENSE.txt` & `treecker-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/PKG-INFO` & `treecker-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treecker
-Version: 1.2.0
+Version: 1.3.0
 Summary: Package to check the integrity of a directory.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/dustils/treecker
 Project-URL: Bug Tracker, https://gitlab.com/dustils/treecker/issues
 Project-URL: Documentation, https://dustils.gitlab.io/treecker
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -45,15 +45,15 @@
 The program can also check that the file and folder names match a regular expression.
 This allows to detect errors in the naming of files.
 These features are accessible via the following commands:
 
 * `init`: To create the first snapshot of a directory.
 * `status`: To display the changes since last snapshot.
 * `commit`: To save the change in a new snapshot.
-* `issues`: To display incorrectly named files and directories.
+* `issues`: To display misnamed or unreadable files.
 
 ## Installation
 
 You can find how to install the package in the [installation section](https://dustils.gitlab.io/treecker/practice/installation/index.html) of the documentation.
 
 ## Usage
```

### Comparing `treecker-1.2.0/README.md` & `treecker-1.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 The program can also check that the file and folder names match a regular expression.
 This allows to detect errors in the naming of files.
 These features are accessible via the following commands:
 
 * `init`: To create the first snapshot of a directory.
 * `status`: To display the changes since last snapshot.
 * `commit`: To save the change in a new snapshot.
-* `issues`: To display incorrectly named files and directories.
+* `issues`: To display misnamed or unreadable files.
 
 ## Installation
 
 You can find how to install the package in the [installation section](https://dustils.gitlab.io/treecker/practice/installation/index.html) of the documentation.
 
 ## Usage
```

### Comparing `treecker-1.2.0/docs/Makefile` & `treecker-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/docs/source/conf.py` & `treecker-1.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/docs/source/index.rst` & `treecker-1.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/docs/source/practice/examples/configuration.rst` & `treecker-1.3.0/docs/source/practice/examples/configuration.rst`

 * *Files 9% similar despite different names*

```diff
@@ -41,13 +41,17 @@
 A special configuration can be set up to track a directory.
 For this, add a configuration file called ``treecker.conf`` at the root of the tracked directory, that is, next to the ``treecker.json`` file.
 It is then possible to choose, among others, which file or directory names will be ignored in the tracking or in the name verification:
 
 .. code-block:: ini
 
    [treecker.core.naming]
-   ignore-patterns = README* LICENSE* CITATION* INSTALL* SETUP* MANIFEST* SOURCES* PKG-INFO Makefile *.php LC_MESSAGES en_US en_GB fr_FR
+   match = ([0-9]{8}T[0-9]{6}Z)?([a-z]|[0-9]|\.|-|_)*
 
    [treecker.core.snapshot]
-   ignore-patterns = __pycache__ .git
+   ignore = __pycache__ .git
+
+   [treecker.main.issues]
+   ignore_name = README* LICENSE* CITATION* INSTALL* SETUP* MANIFEST* SOURCES* PKG-INFO Makefile *.php LC_MESSAGES en_US en_GB fr_FR
+   ignore_contents = corrupted
 
 For more configuration options, see the default configuration file `default.conf <https://gitlab.com/dustils/treecker/-/blob/main/src/treecker/default.conf>`_.
```

### Comparing `treecker-1.2.0/docs/source/practice/examples/vanilla.rst` & `treecker-1.3.0/docs/source/practice/examples/vanilla.rst`

 * *Files 12% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 .. code-block:: bash
 
    treecker commit
 
 Display issues
 ~~~~~~~~~~~~~~
 
-To display incorrectly nammed files and directories, execute the following command.
+To display misnamed or unreadable files, execute the following command.
 
 .. code-block:: bash
 
    treecker issues
```

### Comparing `treecker-1.2.0/docs/source/practice/installation/editable.rst` & `treecker-1.3.0/docs/source/practice/installation/editable.rst`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/docs/source/practice/installation/regular.rst` & `treecker-1.3.0/docs/source/practice/installation/regular.rst`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/docs/source/practice/installation/venv.rst` & `treecker-1.3.0/docs/source/practice/installation/venv.rst`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/pyproject.toml` & `treecker-1.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,18 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Topic :: System :: Filesystems",
   "Intended Audience :: End Users/Desktop",
 ]
+dependencies = [
+  "Pillow>=9.5.0",
+  "PyPDF2>=3.0.0",
+]
 
 [tool.setuptools_scm]
 write_to = "src/treecker/_version.py"
 
 [project.scripts]
 treecker = "treecker.__main__:main"
```

### Comparing `treecker-1.2.0/setup.sh` & `treecker-1.3.0/setup.sh`

 * *Files 3% similar despite different names*

```diff
@@ -103,12 +103,13 @@
     flake8 $PATH_PACK $PATH_REPO/tests/run.py
 }
 
 # command to upload the package to PyPI
 upload()
 {
     python3 -m build
-    python3 -m twine upload dist/*.tar.gz dist/*-none-any.whl --skip-existing
+    dist=$(find dist -name "*.tar.gz" -o -name "*-none-any.whl")
+    python3 -m twine upload $dist --skip-existing
 }
 
 # install and activate the virtual environment
 install
```

### Comparing `treecker-1.2.0/src/treecker/__main__.py` & `treecker-1.3.0/src/treecker/__main__.py`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/src/treecker/core/colors.py` & `treecker-1.3.0/src/treecker/core/colors.py`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/src/treecker/core/snapshot.py` & `treecker-1.3.0/src/treecker/core/snapshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     -------
     dict
         Directory snapshot data.
 
     """
     logger.debug("taking snapshot of %s", directory)
     file = config.get(__name__, 'snap_file')
-    ignore = config.get(__name__, 'ignore_patterns').split()
+    ignore = config.get(__name__, 'ignore').split()
     ignore.append(file)
     date = datetime.now(timezone.utc).isoformat(timespec="seconds")
     node = tree_node(directory, ignore, hashing)
     snapshot = {
         'version': list(__version_tuple__),
         'date': date,
         'hash': hashing,
```

### Comparing `treecker-1.2.0/src/treecker/core/tree.py` & `treecker-1.3.0/src/treecker/core/tree.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """File tree structure.
 
 This module implements the functionalities related to the trees.
 
 """
 
 from fnmatch import fnmatch
-from hashlib import new
+from hashlib import new as new_hash
 from logging import getLogger
 from multiprocessing import Pool
 from os import stat
 from pathlib import Path
 
 from treecker import config
 
@@ -32,15 +32,15 @@
     str
         File hash value.
 
     """
     logger.debug("computing hash of %s", path)
     size = config.getint(__name__, 'block_size')
     algo = config.get(__name__, 'hash_algo')
-    hashing = new(algo)
+    hashing = new_hash(algo)
     with open(path, 'rb') as file:
         series = file.read(size)
         while len(series) > 0:
             hashing.update(series)
             series = file.read(size)
     value = hashing.hexdigest()
     return value
@@ -166,7 +166,53 @@
 
     """
     logger.debug("computing tree")
     node = subtree_node(Path(directory), ignore)
     if hashing:
         add_hash(directory, node)
     return node
+
+
+def get_differences(old, new, hashing, path=None):
+    """Return a list of the differences between two tree objects.
+
+    Parameters
+    ----------
+    old : dict
+        Old directory node.
+    new : dict
+        New directory node.
+    hashing : bool
+        Compare file hash values.
+    path : list
+        Initial path.
+
+    Returns
+    -------
+    list
+        Differences betwen the two nodes.
+
+    """
+    logger.debug("getting differences at %s", path)
+    if path is None:
+        path = []
+    listing = []
+    if isinstance(old, dict) and isinstance(new, dict):
+        for node in old:
+            if node in new:
+                listing += get_differences(
+                    old[node],
+                    new[node],
+                    hashing,
+                    path+[node],
+                )
+            else:
+                listing.append({'type': 'removed', 'path': path+[node]})
+        for node in new:
+            if node not in old:
+                listing.append({'type': 'added', 'path': path+[node]})
+    elif isinstance(old, dict) or isinstance(new, dict):
+        listing.append({'type': 'removed', 'path': path})
+        listing.append({'type': 'added', 'path': path})
+    elif (old[0] != new[0]) or hashing and (old[1] != new[1]):
+        listing.append({'type': 'edited', 'path': path})
+    return listing
```

### Comparing `treecker-1.2.0/src/treecker/default.conf` & `treecker-1.3.0/src/treecker/default.conf`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,49 @@
 red = \033[31m
 green = \033[32m
 yellow = \033[33m
 blue = \033[34m
 magenta = \033[35m
 cyan = \033[36m
 
-[treecker.core.comparison]
+[treecker.core.contents]
+patterns_pdf = *.pdf
+patterns_pic = *.png *.jpg *.gif *.jpeg
+patterns_tar = *.tar
+patterns_zip = *.zip
+block_size = 65536
+
+[treecker.core.display]
 color_added = green
 color_removed = red
 color_edited = yellow
 symbol_added = (+)
 symbol_removed = (-)
 symbol_edited = (!)
+color_issue = yellow
 
 [treecker.core.naming]
-color_issue = yellow
-match_pattern = ([a-z]|[0-9]|\.|-|_)*
-ignore_patterns =
+match = ([a-z]|[0-9]|\.|-|_)*
 
 [treecker.core.snapshot]
 snap_file = treecker.json
-ignore_patterns =
+ignore =
 
 [treecker.core.tree]
 hash_algo = md5
 block_size = 65536
 
 [treecker.main.commit]
 dir = .
 
 [treecker.main.init]
 dir = .
 hash = False
 
 [treecker.main.issues]
 dir = .
+ignore_name =
+ignore_contents =
 
 [treecker.main.status]
 dir = .
 hash = False
```

### Comparing `treecker-1.2.0/src/treecker/main/commit.py` & `treecker-1.3.0/src/treecker/main/commit.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 """
 
 from datetime import datetime, timezone
 from logging import getLogger
 from os.path import join
 
 from treecker import config
-from treecker.core.comparison import get_differences, differences_log
+from treecker.core.display import differences_log
 from treecker.core.snapshot import initialized, load, save, take
+from treecker.core.tree import get_differences
 
 
 logger = getLogger(__name__)
 
 
 def setup(parser):
     """Configure the parser for the module.
```

### Comparing `treecker-1.2.0/src/treecker/main/init.py` & `treecker-1.3.0/src/treecker/main/init.py`

 * *Files identical despite different names*

### Comparing `treecker-1.2.0/src/treecker/main/status.py` & `treecker-1.3.0/src/treecker/main/status.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 """
 
 from datetime import datetime, timezone
 from logging import getLogger
 from os.path import join
 
 from treecker import config
-from treecker.core.comparison import get_differences, differences_log
+from treecker.core.display import differences_log
 from treecker.core.snapshot import initialized, load, take
+from treecker.core.tree import get_differences
 
 
 logger = getLogger(__name__)
 
 
 def setup(parser):
     """Configure the parser for the module.
```

### Comparing `treecker-1.2.0/src/treecker.egg-info/PKG-INFO` & `treecker-1.3.0/src/treecker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treecker
-Version: 1.2.0
+Version: 1.3.0
 Summary: Package to check the integrity of a directory.
 Author-email: Dunstan Becht <dunstan.becht@orange.fr>
 Project-URL: Homepage, https://gitlab.com/dustils/treecker
 Project-URL: Bug Tracker, https://gitlab.com/dustils/treecker/issues
 Project-URL: Documentation, https://dustils.gitlab.io/treecker
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -45,15 +45,15 @@
 The program can also check that the file and folder names match a regular expression.
 This allows to detect errors in the naming of files.
 These features are accessible via the following commands:
 
 * `init`: To create the first snapshot of a directory.
 * `status`: To display the changes since last snapshot.
 * `commit`: To save the change in a new snapshot.
-* `issues`: To display incorrectly named files and directories.
+* `issues`: To display misnamed or unreadable files.
 
 ## Installation
 
 You can find how to install the package in the [installation section](https://dustils.gitlab.io/treecker/practice/installation/index.html) of the documentation.
 
 ## Usage
```

### Comparing `treecker-1.2.0/src/treecker.egg-info/SOURCES.txt` & `treecker-1.3.0/src/treecker.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,25 +20,32 @@
 src/treecker/__main__.py
 src/treecker/_version.py
 src/treecker/default.conf
 src/treecker.egg-info/PKG-INFO
 src/treecker.egg-info/SOURCES.txt
 src/treecker.egg-info/dependency_links.txt
 src/treecker.egg-info/entry_points.txt
+src/treecker.egg-info/requires.txt
 src/treecker.egg-info/top_level.txt
 src/treecker/core/__init__.py
 src/treecker/core/colors.py
-src/treecker/core/comparison.py
+src/treecker/core/contents.py
+src/treecker/core/display.py
 src/treecker/core/naming.py
 src/treecker/core/snapshot.py
 src/treecker/core/tree.py
 src/treecker/main/__init__.py
 src/treecker/main/commit.py
 src/treecker/main/init.py
 src/treecker/main/issues.py
 src/treecker/main/status.py
 tests/references.json
 tests/run.py
+tests/material/corrupted/file.gif
+tests/material/corrupted/file.jpg
+tests/material/corrupted/file.pdf
+tests/material/corrupted/file.tar
+tests/material/corrupted/file.zip
 tests/material/inputs/commit-n.txt
 tests/material/inputs/commit-y.txt
 tests/material/tracked/file.txt
 tests/material/tracked/subdir/setup.sh
```

### Comparing `treecker-1.2.0/tests/references.json` & `treecker-1.3.0/tests/references.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'issues'": "{0: {insert: [(0, 'UP')], delete: [0]}, 1: {insert: [(0, 'spa ce')], delete: [0]}, "*

 * *             "2: {insert: [(0, 'a.tar.gz')], delete: [0]}}"}*

```diff
@@ -175,35 +175,23 @@
             [
                 49
             ]
         ]
     ],
     "issues": [
         [
-            {
-                "UP": [
-                    10
-                ]
-            },
+            "UP",
             1
         ],
         [
-            {
-                "spa ce": [
-                    2
-                ]
-            },
+            "spa ce",
             1
         ],
         [
-            {
-                "a.tar.gz": [
-                    2
-                ]
-            },
+            "a.tar.gz",
             0
         ]
     ],
     "test_node_hash": {
         "subdir": {
             "setup.sh": [
                 49,
```

### Comparing `treecker-1.2.0/tests/run.py` & `treecker-1.3.0/tests/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 
 This script executes the unit tests for the package.
 
 """
 
 from contextlib import contextmanager, redirect_stdout
 from json import load, dumps
+from os import listdir
 from pathlib import Path
 from shutil import copytree, rmtree
 from subprocess import CalledProcessError, run
 from sys import stderr
 from tempfile import TemporaryDirectory, TemporaryFile
 from unittest import main, TestCase
 
-from treecker.core import comparison, naming, snapshot, tree
+from treecker.core import contents, naming, snapshot, tree
 from treecker.main import commit, init, issues, status
 
 
 dir_tests = Path(__file__).parent
 dir_material = dir_tests/'material'
 
 with open(dir_tests/'references.json', 'r', encoding='utf-8') as ref_file:
@@ -126,21 +127,31 @@
                     snapshot.save(tracked, snap1)
                     snap2 = snapshot.load(tracked)
                     self.assertDictEqual(snap1, snap2)
 
     def test_naming_issues(self):
         """Test naming issues."""
         for node, length in ref['issues']:
-            data = naming.get_issues(node)
+            data = naming.name_issues(node)
             self.assertEqual(len(data), length)
 
+    def test_contents_issues(self):
+        """Test contents issues."""
+        corrupted = dir_material/'corrupted'
+        for file in listdir(corrupted):
+            with self.subTest(file=file):
+                path = corrupted/file
+                if path.is_file():
+                    listing = contents.file_issues(path)
+                    self.assertEqual(len(listing), 1)
+
     def test_differences(self):
         """Test identification of differences."""
         for node1, node2, hashing, length in ref['differences']:
-            data = comparison.get_differences(node1, node2, hashing)
+            data = tree.get_differences(node1, node2, hashing)
             self.assertEqual(length, len(data))
 
 
 class TestMain(TestCase):
     """Class for testing main subpackage."""
 
     def test_init(self):
```

