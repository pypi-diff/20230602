# Comparing `tmp/daffi_terminals-1.0.3.tar.gz` & `tmp/daffi_terminals-1.0.4.tar.gz`

## Comparing `daffi_terminals-1.0.3.tar` & `daffi_terminals-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,22 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/__about__.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/main.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/router/__init__.py
--rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/router/router.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/router/static/index.html
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/worker/__init__.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/daffi_terminals/worker/worker.py
--rw-r--r--   0        0        0   122142 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/docs/img/2.png
--rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/docs/img/intro.png
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 daffi_terminals-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/__about__.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/main.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/__init__.py
+-rw-r--r--   0        0        0     8235 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/router.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/index.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/css/fullscreen.min.css
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/css/main.css
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/css/xterm.min.css
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/img/favicon.ico
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/js/main.js
+-rw-r--r--   0        0        0    21004 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/js/popper.min.js
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/js/xterm-addon-fit.min.js
+-rw-r--r--   0        0        0   251949 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/router/static/js/xterm.min.js
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/worker/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/daffi_terminals/worker/worker.py
+-rw-r--r--   0        0        0   122142 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/docs/img/2.png
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/docs/img/intro.png
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/README.md
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 daffi_terminals-1.0.4/PKG-INFO
```

### Comparing `daffi_terminals-1.0.3/daffi_terminals/main.py` & `daffi_terminals-1.0.4/daffi_terminals/main.py`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/daffi_terminals/router/router.py` & `daffi_terminals-1.0.4/daffi_terminals/router/router.py`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/daffi_terminals/router/static/index.html` & `daffi_terminals-1.0.4/daffi_terminals/router/static/index.html`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/daffi_terminals/worker/worker.py` & `daffi_terminals-1.0.4/daffi_terminals/worker/worker.py`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/docs/img/2.png` & `daffi_terminals-1.0.4/docs/img/2.png`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/docs/img/intro.png` & `daffi_terminals-1.0.4/docs/img/intro.png`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/.gitignore` & `daffi_terminals-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/LICENSE.txt` & `daffi_terminals-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/README.md` & `daffi_terminals-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `daffi_terminals-1.0.3/pyproject.toml` & `daffi_terminals-1.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -60,16 +60,19 @@
 Source = "https://github.com/600apples/dafi-terminals"
 
 [tool.hatch.version]
 path = "daffi_terminals/__about__.py"
 
 [tool.hatch.build]
 include = [
-  "docs/img/*.*",
+  "docs/img/*.png",
   "daffi_terminals/router/static/*.*",
+  "daffi_terminals/router/static/js/*.*",
+  "daffi_terminals/router/static/css/*.*",
+  "daffi_terminals/router/static/img/*.*",
   "**/*.py",
 ]
 
 [tool.hatch.envs.default.overrides]
 env.GITHUB_ACTIONS.env-vars = "COVERAGE_REPORT="
 
 [tool.hatch.envs.default]
```

### Comparing `daffi_terminals-1.0.3/PKG-INFO` & `daffi_terminals-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffi-terminals
-Version: 1.0.3
+Version: 1.0.4
 Summary: Remote terminal control
 Project-URL: Source, https://github.com/600apples/dafi-terminals
 Author-email: Volodymyr Boiko <600apples@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: async,debug,debugging,distributed,embedded,iot,python,remote,remote control,rpc,ssh,stream,webssh
 Classifier: Development Status :: 4 - Beta
```

