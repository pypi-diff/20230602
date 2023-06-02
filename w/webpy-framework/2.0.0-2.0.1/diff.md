# Comparing `tmp/webpy-framework-2.0.0.tar.gz` & `tmp/webpy-framework-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-2.0.0.tar", last modified: Fri Jun  2 00:23:40 2023, max compression
+gzip compressed data, was "webpy-framework-2.0.1.tar", last modified: Fri Jun  2 17:09:43 2023, max compression
```

## Comparing `webpy-framework-2.0.0.tar` & `webpy-framework-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.654678 webpy-framework-2.0.0/
--rw-rw-rw-   0        0        0     1090 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     7137 2023-06-02 00:23:40.652677 webpy-framework-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/README.md
--rw-rw-rw-   0        0        0     1750 2023-06-02 00:23:22.000000 webpy-framework-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 00:23:40.654678 webpy-framework-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.627027 webpy-framework-2.0.0/webpy/
--rw-rw-rw-   0        0        0     1968 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/__init__.py
--rw-rw-rw-   0        0        0    11982 2023-06-02 00:21:45.000000 webpy-framework-2.0.0/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/pysite_semantic_tags.py
--rw-rw-rw-   0        0        0      405 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/pyx_snippets.py
-drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.649605 webpy-framework-2.0.0/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     7137 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7137 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/README.md
+-rw-rw-rw-   0        0        0     1750 2023-06-02 17:09:19.000000 webpy-framework-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.160506 webpy-framework-2.0.1/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/webpy/__init__.py
+-rw-rw-rw-   0        0        0    12004 2023-06-02 17:05:44.000000 webpy-framework-2.0.1/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-06-02 17:08:18.000000 webpy-framework-2.0.1/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/webpy/pysite_semantic_tags.py
+-rw-rw-rw-   0        0        0      407 2023-06-02 17:07:58.000000 webpy-framework-2.0.1/webpy/pyx_snippets.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.210496 webpy-framework-2.0.1/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     7137 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      200 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-2.0.0/LICENSE` & `webpy-framework-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.0/PKG-INFO` & `webpy-framework-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 2.0.0
+Version: 2.0.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `webpy-framework-2.0.0/README.md` & `webpy-framework-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.0/pyproject.toml` & `webpy-framework-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "2.0.0"
+version = "2.0.1"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
```

### Comparing `webpy-framework-2.0.0/webpy/__init__.py` & `webpy-framework-2.0.1/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.0/webpy/__main__.py` & `webpy-framework-2.0.1/webpy/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 				f"route({route!r}, {','.join(f'{key}={value!r}' for key, value in config.items())})"
 				f"(appbind(loads({handler!r}), "
 				f"app, {route+'_handler'!r}))\n"
 			)
 
 		if not deploying: code+=(f"app.run({','.join(f'{key}={value!r}' for key, value in conf.items())})")
 
-		f.write(minify(code, rename_globals=True) if not deploying else minify(code))
+		f.write(minify(code, rename_globals=True) if not deploying else minify(code, rename_globals=False))
 
 def run(
 		force_debug: bool,
 		compile_md: bool,
 		compile_pyx: bool,
 		reload_md: bool,
 		reload_pyx: bool
```

### Comparing `webpy-framework-2.0.0/webpy/fs_routes.py` & `webpy-framework-2.0.1/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.0/webpy/pysite_semantic_tags.py` & `webpy-framework-2.0.1/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.0/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-2.0.1/webpy_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 2.0.0
+Version: 2.0.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

