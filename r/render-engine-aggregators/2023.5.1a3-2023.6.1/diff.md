# Comparing `tmp/render_engine_aggregators-2023.5.1a3.tar.gz` & `tmp/render_engine_aggregators-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_aggregators-2023.5.1a3.tar", last modified: Mon May 15 14:46:10 2023, max compression
+gzip compressed data, was "render_engine_aggregators-2023.6.1.tar", last modified: Fri Jun  2 12:40:45 2023, max compression
```

## Comparing `render_engine_aggregators-2023.5.1a3.tar` & `render_engine_aggregators-2023.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.743439 render_engine_aggregators-2023.5.1a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.739439 render_engine_aggregators-2023.5.1a3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.github/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.739439 render_engine_aggregators-2023.5.1a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.739439 render_engine_aggregators-2023.5.1a3/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 14:46:10.743439 render_engine_aggregators-2023.5.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:46:10.743439 render_engine_aggregators-2023.5.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.735439 render_engine_aggregators-2023.5.1a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.739439 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators/feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.743439 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-15 14:46:10.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-15 14:46:10.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:46:10.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 14:46:10.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:46:10.000000 render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:46:10.743439 render_engine_aggregators-2023.5.1a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 14:45:51.000000 render_engine_aggregators-2023.5.1a3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.328022 render_engine_aggregators-2023.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.324022 render_engine_aggregators-2023.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.github/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.324022 render_engine_aggregators-2023.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.324022 render_engine_aggregators-2023.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 12:40:45.328022 render_engine_aggregators-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 12:40:45.328022 render_engine_aggregators-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.324022 render_engine_aggregators-2023.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.324022 render_engine_aggregators-2023.6.1/src/render_engine_aggregators/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators/feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.328022 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-02 12:40:45.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-02 12:40:45.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 12:40:45.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 12:40:45.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-02 12:40:45.000000 render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 12:40:45.328022 render_engine_aggregators-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 12:40:25.000000 render_engine_aggregators-2023.6.1/tests/test.py
```

### Comparing `render_engine_aggregators-2023.5.1a3/.github/CODE_OF_CONDUCT.md` & `render_engine_aggregators-2023.6.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/.github/LICENSE` & `render_engine_aggregators-2023.6.1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/.github/dependabot.yml` & `render_engine_aggregators-2023.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/.github/workflows/publish.yml` & `render_engine_aggregators-2023.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/.gitignore` & `render_engine_aggregators-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/.vscode/settings.json` & `render_engine_aggregators-2023.6.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/pyproject.toml` & `render_engine_aggregators-2023.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "render_engine_aggregators"
 dynamic = ["version"]
 description = "aggregate multiple collections"
 readme = "README.md"
 
 dependencies = [
-    "render-engine"
+    "render-engine>=2023.6.1"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "ruff",
     "black",
```

### Comparing `render_engine_aggregators-2023.5.1a3/requirements.txt` & `render_engine_aggregators-2023.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine_aggregators-2023.5.1a3/src/render_engine_aggregators.egg-info/SOURCES.txt` & `render_engine_aggregators-2023.6.1/src/render_engine_aggregators.egg-info/SOURCES.txt`

 * *Files identical despite different names*

