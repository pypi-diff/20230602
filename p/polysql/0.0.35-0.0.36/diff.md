# Comparing `tmp/polysql-0.0.35.tar.gz` & `tmp/polysql-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polysql-0.0.35.tar", last modified: Thu Apr 20 12:12:11 2023, max compression
+gzip compressed data, was "polysql-0.0.36.tar", last modified: Fri Jun  2 10:54:02 2023, max compression
```

## Comparing `polysql-0.0.35.tar` & `polysql-0.0.36.tar`

### file list

```diff
@@ -1,32 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.612486 polysql-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-20 12:08:48.000000 polysql-0.0.35/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 12:12:11.612486 polysql-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-20 12:08:48.000000 polysql-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.548486 polysql-0.0.35/bigquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.580485 polysql-0.0.35/bigquery/src/
--rw-r--r--   0 runner    (1001) docker     (123)   219260 2023-04-20 12:08:59.000000 polysql-0.0.35/bigquery/src/grammar.json
--rw-r--r--   0 runner    (1001) docker     (123)   195118 2023-04-20 12:10:06.000000 polysql-0.0.35/bigquery/src/node-types.json
--rw-r--r--   0 runner    (1001) docker     (123) 21579946 2023-04-20 12:10:06.000000 polysql-0.0.35/bigquery/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-20 12:08:48.000000 polysql-0.0.35/bigquery/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.580485 polysql-0.0.35/bigquery/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-20 12:10:06.000000 polysql-0.0.35/bigquery/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.548486 polysql-0.0.35/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.580485 polysql-0.0.35/bindings/python/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-20 12:08:48.000000 polysql-0.0.35/bindings/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.580485 polysql-0.0.35/polysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 12:12:11.000000 polysql-0.0.35/polysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 12:12:11.000000 polysql-0.0.35/polysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 12:12:11.000000 polysql-0.0.35/polysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-20 12:12:11.000000 polysql-0.0.35/polysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-20 12:12:11.000000 polysql-0.0.35/polysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.548486 polysql-0.0.35/postgres/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.612486 polysql-0.0.35/postgres/src/
--rw-r--r--   0 runner    (1001) docker     (123)   200173 2023-04-20 12:10:08.000000 polysql-0.0.35/postgres/src/grammar.json
--rw-r--r--   0 runner    (1001) docker     (123)   186032 2023-04-20 12:11:12.000000 polysql-0.0.35/postgres/src/node-types.json
--rw-r--r--   0 runner    (1001) docker     (123) 22736139 2023-04-20 12:11:12.000000 polysql-0.0.35/postgres/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-04-20 12:08:48.000000 polysql-0.0.35/postgres/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 12:12:11.612486 polysql-0.0.35/postgres/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-20 12:11:12.000000 polysql-0.0.35/postgres/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 12:08:48.000000 polysql-0.0.35/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 12:12:11.612486 polysql-0.0.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-20 12:08:48.000000 polysql-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.503056 polysql-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 10:51:25.000000 polysql-0.0.36/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 10:54:02.503056 polysql-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 10:51:25.000000 polysql-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.451055 polysql-0.0.36/bigquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/bigquery/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   219260 2023-06-02 10:51:34.000000 polysql-0.0.36/bigquery/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (123)   195118 2023-06-02 10:52:26.000000 polysql-0.0.36/bigquery/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (123) 21579946 2023-06-02 10:52:26.000000 polysql-0.0.36/bigquery/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-02 10:51:25.000000 polysql-0.0.36/bigquery/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/bigquery/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-02 10:52:26.000000 polysql-0.0.36/bigquery/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.451055 polysql-0.0.36/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/bindings/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-02 10:51:25.000000 polysql-0.0.36/bindings/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.451055 polysql-0.0.36/jinja2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/jinja2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     9060 2023-06-02 10:51:33.000000 polysql-0.0.36/jinja2/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-02 10:51:33.000000 polysql-0.0.36/jinja2/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55374 2023-06-02 10:51:33.000000 polysql-0.0.36/jinja2/src/parser.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/jinja2/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-02 10:51:33.000000 polysql-0.0.36/jinja2/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.475055 polysql-0.0.36/polysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 10:54:02.000000 polysql-0.0.36/polysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-02 10:54:02.000000 polysql-0.0.36/polysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:54:02.000000 polysql-0.0.36/polysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 10:54:02.000000 polysql-0.0.36/polysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 10:54:02.000000 polysql-0.0.36/polysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.451055 polysql-0.0.36/postgres/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.503056 polysql-0.0.36/postgres/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   200173 2023-06-02 10:52:28.000000 polysql-0.0.36/postgres/src/grammar.json
+-rw-r--r--   0 runner    (1001) docker     (123)   186032 2023-06-02 10:53:16.000000 polysql-0.0.36/postgres/src/node-types.json
+-rw-r--r--   0 runner    (1001) docker     (123) 22736139 2023-06-02 10:53:16.000000 polysql-0.0.36/postgres/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8698 2023-06-02 10:51:25.000000 polysql-0.0.36/postgres/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:54:02.503056 polysql-0.0.36/postgres/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-02 10:53:16.000000 polysql-0.0.36/postgres/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-02 10:51:25.000000 polysql-0.0.36/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:54:02.503056 polysql-0.0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-02 10:51:25.000000 polysql-0.0.36/setup.py
```

### Comparing `polysql-0.0.35/bigquery/src/grammar.json` & `polysql-0.0.36/bigquery/src/grammar.json`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/bigquery/src/node-types.json` & `polysql-0.0.36/bigquery/src/node-types.json`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/bigquery/src/parser.c` & `polysql-0.0.36/bigquery/src/parser.c`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/bigquery/src/scanner.cc` & `polysql-0.0.36/bigquery/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/bigquery/src/tree_sitter/parser.h` & `polysql-0.0.36/bigquery/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/postgres/src/grammar.json` & `polysql-0.0.36/postgres/src/grammar.json`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/postgres/src/node-types.json` & `polysql-0.0.36/postgres/src/node-types.json`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/postgres/src/parser.c` & `polysql-0.0.36/postgres/src/parser.c`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/postgres/src/scanner.cc` & `polysql-0.0.36/postgres/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/postgres/src/tree_sitter/parser.h` & `polysql-0.0.36/jinja2/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `polysql-0.0.35/setup.py` & `polysql-0.0.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             ],
         )
         install.run(self)
 
 
 setup(
     name="polysql",
-    version="0.0.35",
+    version="0.0.36",
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Grammar and parser used to parse SQL",
     packages=["polysql"],
     package_dir={
         "polysql": "bindings/python",
         "polysql.bigquery": "bigquery/src",
```

