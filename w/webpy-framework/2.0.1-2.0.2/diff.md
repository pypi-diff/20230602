# Comparing `tmp/webpy-framework-2.0.1.tar.gz` & `tmp/webpy-framework-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-2.0.1.tar", last modified: Fri Jun  2 17:09:43 2023, max compression
+gzip compressed data, was "webpy-framework-2.0.2.tar", last modified: Fri Jun  2 17:56:26 2023, max compression
```

## Comparing `webpy-framework-2.0.1.tar` & `webpy-framework-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/LICENSE
--rw-rw-rw-   0        0        0     7137 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/README.md
--rw-rw-rw-   0        0        0     1750 2023-06-02 17:09:19.000000 webpy-framework-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-02 17:09:43.215983 webpy-framework-2.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.160506 webpy-framework-2.0.1/webpy/
--rw-rw-rw-   0        0        0     1968 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/webpy/__init__.py
--rw-rw-rw-   0        0        0    12004 2023-06-02 17:05:44.000000 webpy-framework-2.0.1/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-06-02 17:08:18.000000 webpy-framework-2.0.1/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-06-01 18:36:28.000000 webpy-framework-2.0.1/webpy/pysite_semantic_tags.py
--rw-rw-rw-   0        0        0      407 2023-06-02 17:07:58.000000 webpy-framework-2.0.1/webpy/pyx_snippets.py
-drwxrwxrwx   0        0        0        0 2023-06-02 17:09:43.210496 webpy-framework-2.0.1/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     7137 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      200 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-02 17:09:43.000000 webpy-framework-2.0.1/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 17:56:26.163698 webpy-framework-2.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 18:36:28.000000 webpy-framework-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0     7137 2023-06-02 17:56:26.163698 webpy-framework-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-06-01 18:36:28.000000 webpy-framework-2.0.2/README.md
+-rw-rw-rw-   0        0        0     1750 2023-06-02 17:54:59.000000 webpy-framework-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 17:56:26.166209 webpy-framework-2.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 17:56:26.127965 webpy-framework-2.0.2/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-06-01 18:36:28.000000 webpy-framework-2.0.2/webpy/__init__.py
+-rw-rw-rw-   0        0        0    12026 2023-06-02 17:54:28.000000 webpy-framework-2.0.2/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-06-02 17:08:18.000000 webpy-framework-2.0.2/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-06-01 18:36:28.000000 webpy-framework-2.0.2/webpy/pysite_semantic_tags.py
+-rw-rw-rw-   0        0        0      407 2023-06-02 17:07:58.000000 webpy-framework-2.0.2/webpy/pyx_snippets.py
+drwxrwxrwx   0        0        0        0 2023-06-02 17:56:26.159075 webpy-framework-2.0.2/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     7137 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      200 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 17:56:26.000000 webpy-framework-2.0.2/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-2.0.1/LICENSE` & `webpy-framework-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.1/PKG-INFO` & `webpy-framework-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 2.0.1
+Version: 2.0.2
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `webpy-framework-2.0.1/README.md` & `webpy-framework-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.1/pyproject.toml` & `webpy-framework-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "2.0.1"
+version = "2.0.2"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
```

### Comparing `webpy-framework-2.0.1/webpy/__init__.py` & `webpy-framework-2.0.2/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.1/webpy/__main__.py` & `webpy-framework-2.0.2/webpy/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,25 +120,24 @@
 
 	# TODO: use TypedDict for this
 	routes: dict[str, dict[str, Union[dict[str, str], bytes, str]]] = {}
 
 	if not parse_fs_routes(app, "root", routes, {}):
 		exit(1)
 
-	with open("build.py", 'w') as f:
+	with open("webpy_build.py", 'w') as f:
 		code = ""
 		for module in conf.get("imports", tuple()):
 			code+=f"import {module}\n"
 
 		code+=(
 			f"""from dill import loads
-from webpy import appbind
-from flask import Flask
+from webpy import appbind, App
 
-app = Flask(
+app = App(
 	{app.import_name!r},
 	{app.static_url_path!r},
 	{app.static_folder!r},
 	{conf.get("static_host", None)!r},
 	{app.url_map.host_matching!r},
 	{app.subdomain_matching!r},
 	{app.template_folder!r},
@@ -156,22 +155,22 @@
 			if rule.endpoint == "static": continue
 			
 			code+=(
 				f"""
 app.add_url_rule(
 	{rule.rule!r}, 
 	{rule.endpoint!r},
-	dill.loads({dill.dumps(app.view_functions[rule.endpoint])!r}),
+	loads({dill.dumps(app.view_functions[rule.endpoint])!r}),
 	methods={list(rule.methods)!r},
 	defaults={rule.defaults!r},
 	subdomain={rule.subdomain!r},
 	build_only={rule.build_only!r},
 	strict_slashes={rule.strict_slashes!r},
 	merge_slashes={rule.merge_slashes!r},
-	redirect_to=dill.loads({dill.dumps(rule.redirect_to)!r}),
+	redirect_to=loads({dill.dumps(rule.redirect_to)!r}),
 	alias={rule.alias!r},
 	host={rule.host!r},
 	websocket={rule.websocket!r}
 )	
 """
 			)
 
@@ -326,38 +325,38 @@
 	open(f"{name}/index.py", 'w').write(
 		defaultroutecode
 	)
 
 def webpy_compile(force_debug: bool, compile_md: bool, compile_pyx: bool, deploying: bool=False):
 	build(force_debug, compile_md, compile_pyx, deploying=deploying)
 
-	compile("build.py", "build.pyc", optimize=2)
+	compile("webpy_build.py", "webpy_build.pyc", optimize=2)
 
-	try: os.remove("build.py")
+	try: os.remove("webpy_build.py")
 	except FileNotFoundError: pass
 
 def deploy(force_debug: bool, compile_md: bool, compile_pyx: bool):
-	print("creating build.pyc...")
+	print("creating webpy_build.pyc...")
 	webpy_compile(force_debug, compile_md, compile_pyx, deploying=True)
-	print("done creating build.pyc")
+	print("done creating webpy_build.pyc")
 
 	print("starting app with waitress...")
 
 	conf: dict[str] = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
 			conf = load(f)
 
 	try: subproc_call(
 		[
 			"waitress-serve",
 			"--host", str(conf.get("host", "127.0.0.1")),
 			"--port", str(conf.get("port", 5000)),
-			"build:app"
+			"webpy_build:app"
 		]
 	)
 	except KeyboardInterrupt: pass
 
 def buildpyx():
 	shell = ["powershell"] if os.name == "nt" else ["bash", "-c"]
 
@@ -400,15 +399,15 @@
 		"route",
 		"compile",
 		"buildpyx",
 		"buildmd",
 		"show",
 		"deploy"
 		),
-		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into build.py) --- webpy compile (like build but create build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html) --- webpy show <info> (show info about the app) --- webpy deploy (deploy the app using Waitress)"
+		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into webpy_build.py) --- webpy compile (like build but create webpy_build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html) --- webpy show <info> (show info about the app) --- webpy deploy (deploy the app using Waitress)"
 	)
 
 	parser.add_argument("name", help="name to be used for 'new' or 'route' commands", default=None, nargs='?')
 
 	parser.add_argument("--no-compile-md", action="store_true", help="do not compile Markdown to HTML")
 	parser.add_argument("--no-compile-pyx", action="store_true", help="do not compile PyX to Python")
 	parser.add_argument("--no-reload-md", action="store_true", help="do not check for modifications in Markdown files while running")
```

### Comparing `webpy-framework-2.0.1/webpy/fs_routes.py` & `webpy-framework-2.0.2/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.1/webpy/pysite_semantic_tags.py` & `webpy-framework-2.0.2/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-2.0.1/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-2.0.2/webpy_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 2.0.1
+Version: 2.0.2
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

