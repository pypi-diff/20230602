# Comparing `tmp/webpy-framework-1.2.1.tar.gz` & `tmp/webpy-framework-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.2.1.tar", last modified: Mon May 29 14:37:04 2023, max compression
+gzip compressed data, was "webpy-framework-2.0.0.tar", last modified: Fri Jun  2 00:23:40 2023, max compression
```

## Comparing `webpy-framework-1.2.1.tar` & `webpy-framework-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.443269 webpy-framework-1.2.1/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     6599 2023-05-29 14:37:04.442014 webpy-framework-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.2.1/README.md
--rw-rw-rw-   0        0        0     1116 2023-05-29 14:36:36.000000 webpy-framework-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 14:37:04.443269 webpy-framework-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.423205 webpy-framework-1.2.1/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.2.1/webpy/__init__.py
--rw-rw-rw-   0        0        0    10802 2023-05-29 14:35:09.000000 webpy-framework-1.2.1/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.2.1/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.2.1/webpy/pysite_semantic_tags.py
--rw-rw-rw-   0        0        0      405 2023-05-28 16:34:47.000000 webpy-framework-1.2.1/webpy/pyx_snippets.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.439542 webpy-framework-1.2.1/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.654678 webpy-framework-2.0.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     7137 2023-06-02 00:23:40.652677 webpy-framework-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1750 2023-06-02 00:23:22.000000 webpy-framework-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 00:23:40.654678 webpy-framework-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.627027 webpy-framework-2.0.0/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/__init__.py
+-rw-rw-rw-   0        0        0    11982 2023-06-02 00:21:45.000000 webpy-framework-2.0.0/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/pysite_semantic_tags.py
+-rw-rw-rw-   0        0        0      405 2023-06-01 18:36:28.000000 webpy-framework-2.0.0/webpy/pyx_snippets.py
+drwxrwxrwx   0        0        0        0 2023-06-02 00:23:40.649605 webpy-framework-2.0.0/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     7137 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      200 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 00:23:40.000000 webpy-framework-2.0.0/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.2.1/LICENSE` & `webpy-framework-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.1/PKG-INFO` & `webpy-framework-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.2.1
+Version: 2.0.0
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,20 +23,29 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/webpy
 Project-URL: Documentation, https://webpy-framework.readthedocs.io/
-Keywords: framework,flask,web
+Keywords: framework,flask,web,server,html,markdown,pyx,wsgi,http,xml,asgi,deployment,uvicorn
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Framework :: Flask
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WebPy
 
 A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`. Docs are located [here](https://webpy-framework.readthedocs.io/).
```

### Comparing `webpy-framework-1.2.1/README.md` & `webpy-framework-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.1/pyproject.toml` & `webpy-framework-2.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,68 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.2.1"
+version = "2.0.0"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3",
     "Topic :: Text Processing :: Markup :: HTML",
-    "Operating System :: OS Independent"
+    "Operating System :: OS Independent",
+	"Topic :: Text Processing :: Markup :: Markdown",
+	"Topic :: Text Processing :: Markup :: XML",
+	"Framework :: Flask",
+	"Topic :: Internet :: WWW/HTTP :: HTTP Servers",
+	"Topic :: Internet :: WWW/HTTP :: WSGI :: Server",
+	"Intended Audience :: Developers",
+	"Intended Audience :: Information Technology",
+	"Topic :: Text Processing :: Markup",
+	"Topic :: Software Development :: Build Tools"
+]
+keywords = [
+	"framework",
+	"flask",
+	"web",
+	"server",
+	"html",
+	"markdown",
+	"pyx",
+	"wsgi",
+	"http",
+	"xml",
+	"asgi",
+	"deployment",
+	"uvicorn"
 ]
-keywords = ["framework", "flask", "web"]
 dependencies = [
-	"flask >= 2.2.2",
-	"dill >= 0.3.5.1",
-	"python-minifier >= 2.8.0",
+	"flask >= 2.3.2",
+	"dill >= 0.3.6",
+	"python-minifier >= 2.9.0",
 	"dill >= 0.3.6",
 	"flask-session >= 0.5.0",
-	"flask-sqlalchemy >= 3.0.0",
+	"flask-sqlalchemy >= 3.0.3",
 	"py-domapi >= 1.0.0",
 	"pyx-pysite >= 1.0.3",
-	"marko >= 1.3.0"
+	"marko >= 1.3.0",
+	"waitress >= 2.1.2",
+	"asgiref >= 3.7.2",
+	"uvicorn >= 0.22.0"
 ]
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
 Documentation = "https://webpy-framework.readthedocs.io/"
 
 [project.scripts]
 webpy = "webpy.__main__:main"
-webpy-framework = "webpy.__main__:main"
+webpy-framework = "webpy.__main__:main"
+
+[tool.setuptools]
+packages = ["webpy"]
```

### Comparing `webpy-framework-1.2.1/webpy/__init__.py` & `webpy-framework-2.0.0/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.1/webpy/__main__.py` & `webpy-framework-2.0.0/webpy/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 	<head></head>
 	<body>
 		{html}
 	</body>
 </html>
 """)
 
-def build(force_debug: bool, compile_md: bool, compile_pyx: bool):
+def build(force_debug: bool, compile_md: bool, compile_pyx: bool, deploying: bool=False):
 	if compile_pyx: buildpyx()
 	if compile_md: buildmd()
 
 	conf = {}
 
 	if os.path.exists("config.json"):
 		with open("config.json", 'r') as f:
@@ -117,15 +117,15 @@
 		print("app object and webpy_setup function are missing from app.py!")
 
 	prerules = list(app.url_map.iter_rules())
 
 	# TODO: use TypedDict for this
 	routes: dict[str, dict[str, Union[dict[str, str], bytes, str]]] = {}
 
-	if not parse_fs_routes(app, "root", routes):
+	if not parse_fs_routes(app, "root", routes, {}):
 		exit(1)
 
 	with open("build.py", 'w') as f:
 		code = ""
 		for module in conf.get("imports", tuple()):
 			code+=f"import {module}\n"
 
@@ -191,17 +191,17 @@
 			
 			code+=(
 				f"route({route!r}, {','.join(f'{key}={value!r}' for key, value in config.items())})"
 				f"(appbind(loads({handler!r}), "
 				f"app, {route+'_handler'!r}))\n"
 			)
 
-		code+=(f"app.run({','.join(f'{key}={value!r}' for key, value in conf.items())})")
+		if not deploying: code+=(f"app.run({','.join(f'{key}={value!r}' for key, value in conf.items())})")
 
-		f.write(minify(code, rename_globals=True))
+		f.write(minify(code, rename_globals=True) if not deploying else minify(code))
 
 def run(
 		force_debug: bool,
 		compile_md: bool,
 		compile_pyx: bool,
 		reload_md: bool,
 		reload_pyx: bool
@@ -323,21 +323,45 @@
 		dumps(defaultrouteconf, indent='\t')
 	)
 
 	open(f"{name}/index.py", 'w').write(
 		defaultroutecode
 	)
 
-def webpy_compile(force_debug: bool, compile_md: bool, compile_pyx: bool):
-	build(force_debug, compile_md, compile_pyx)
+def webpy_compile(force_debug: bool, compile_md: bool, compile_pyx: bool, deploying: bool=False):
+	build(force_debug, compile_md, compile_pyx, deploying=deploying)
+
 	compile("build.py", "build.pyc", optimize=2)
 
 	try: os.remove("build.py")
 	except FileNotFoundError: pass
 
+def deploy(force_debug: bool, compile_md: bool, compile_pyx: bool):
+	print("creating build.pyc...")
+	webpy_compile(force_debug, compile_md, compile_pyx, deploying=True)
+	print("done creating build.pyc")
+
+	print("starting app with waitress...")
+
+	conf: dict[str] = {}
+
+	if os.path.exists("config.json"):
+		with open("config.json", 'r') as f:
+			conf = load(f)
+
+	try: subproc_call(
+		[
+			"waitress-serve",
+			"--host", str(conf.get("host", "127.0.0.1")),
+			"--port", str(conf.get("port", 5000)),
+			"build:app"
+		]
+	)
+	except KeyboardInterrupt: pass
+
 def buildpyx():
 	shell = ["powershell"] if os.name == "nt" else ["bash", "-c"]
 
 	for path, directories, files in os.walk(os.getcwd()):
 		for file in files:
 			file: str
 			if file.endswith(".pyx"):
@@ -372,17 +396,19 @@
 		choices=(
 		"run",
 		"build",
 		"new",
 		"route",
 		"compile",
 		"buildpyx",
-		"buildmd"
+		"buildmd",
+		"show",
+		"deploy"
 		),
-		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into build.py) --- webpy compile (like build but create build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html)"
+		help="Possible commands --- webpy new {projectname} (create a new project) --- webpy route {routename} (create a new route directory) --- webpy run (start the application) --- webpy build (compile root/ and app.py into build.py) --- webpy compile (like build but create build.pyc) --- webpy buildpyx (compile all .pyx to .py) --- webpy buildmd (compile all .md to .html) --- webpy show <info> (show info about the app) --- webpy deploy (deploy the app using Waitress)"
 	)
 
 	parser.add_argument("name", help="name to be used for 'new' or 'route' commands", default=None, nargs='?')
 
 	parser.add_argument("--no-compile-md", action="store_true", help="do not compile Markdown to HTML")
 	parser.add_argument("--no-compile-pyx", action="store_true", help="do not compile PyX to Python")
 	parser.add_argument("--no-reload-md", action="store_true", help="do not check for modifications in Markdown files while running")
@@ -442,9 +468,19 @@
 		buildpyx()
 		exit(0)
 
 	if cmd == "buildmd":
 		buildmd()
 		exit(0)
 
+	if cmd == "show":
+		if name not in ("routes", "overview"):
+			print("webpy: error: expected extra command name to be used with 'show'\n  e.g.\n\tshow routes - view application routes\n\tshow overview - view config, app properties, and config stats")
+			exit(1)
+		pass
+
+	if cmd == "deploy":
+		deploy(force_debug, compile_md, compile_pyx)
+		exit(0)
+
 if __name__ == "__main__":
 	main()
```

### Comparing `webpy-framework-1.2.1/webpy/fs_routes.py` & `webpy-framework-2.0.0/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.1/webpy/pysite_semantic_tags.py` & `webpy-framework-2.0.0/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.1/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-2.0.0/webpy_framework.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.2.1
+Version: 2.0.0
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -23,20 +23,29 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/User0332/webpy
 Project-URL: Documentation, https://webpy-framework.readthedocs.io/
-Keywords: framework,flask,web
+Keywords: framework,flask,web,server,html,markdown,pyx,wsgi,http,xml,asgi,deployment,uvicorn
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Framework :: Flask
+Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Server
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Text Processing :: Markup
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # WebPy
 
 A web framework built on top of Flask that allows you to add filesystem routes (in the `root/` folder of your project directory). Install it with `pip install webpy-framework`. Docs are located [here](https://webpy-framework.readthedocs.io/).
```

