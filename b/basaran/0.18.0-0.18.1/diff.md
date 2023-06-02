# Comparing `tmp/basaran-0.18.0.tar.gz` & `tmp/basaran-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basaran-0.18.0.tar", last modified: Mon May 22 01:40:41 2023, max compression
+gzip compressed data, was "basaran-0.18.1.tar", last modified: Fri Jun  2 04:51:04 2023, max compression
```

## Comparing `basaran-0.18.0.tar` & `basaran-0.18.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.213176 basaran-0.18.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-22 01:38:26.000000 basaran-0.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 01:38:26.000000 basaran-0.18.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 01:40:41.213176 basaran-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-22 01:38:26.000000 basaran-0.18.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.209175 basaran-0.18.0/basaran/
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.209175 basaran-0.18.0/basaran/static/
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/static/playground.css
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/static/playground.js
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/static/presets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.209175 basaran-0.18.0/basaran/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/templates/default.chat.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/templates/playground.html
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-22 01:38:26.000000 basaran-0.18.0/basaran/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.209175 basaran-0.18.0/basaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 01:40:41.000000 basaran-0.18.0/basaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-22 01:40:41.000000 basaran-0.18.0/basaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 01:40:41.000000 basaran-0.18.0/basaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 01:40:41.000000 basaran-0.18.0/basaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 01:40:41.000000 basaran-0.18.0/basaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 01:40:41.213176 basaran-0.18.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-22 01:38:26.000000 basaran-0.18.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.213176 basaran-0.18.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-22 01:38:26.000000 basaran-0.18.0/tests/test_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-22 01:38:26.000000 basaran-0.18.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-22 01:38:26.000000 basaran-0.18.0/tests/test_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 01:40:41.213176 basaran-0.18.0/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-22 01:38:26.000000 basaran-0.18.0/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-22 01:38:26.000000 basaran-0.18.0/utils/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.066489 basaran-0.18.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-02 04:48:11.000000 basaran-0.18.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 04:48:11.000000 basaran-0.18.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-02 04:51:04.066489 basaran-0.18.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-06-02 04:48:11.000000 basaran-0.18.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran/
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/playground.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/playground.js
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/static/presets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/basaran/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/templates/default.chat.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/templates/playground.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 04:48:11.000000 basaran-0.18.1/basaran/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.058489 basaran-0.18.1/basaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 04:51:04.000000 basaran-0.18.1/basaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:51:04.066489 basaran-0.18.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-02 04:48:11.000000 basaran-0.18.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-02 04:48:11.000000 basaran-0.18.1/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:51:04.062489 basaran-0.18.1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-02 04:48:11.000000 basaran-0.18.1/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-02 04:48:11.000000 basaran-0.18.1/utils/render.py
```

### Comparing `basaran-0.18.0/LICENSE` & `basaran-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/PKG-INFO` & `basaran-0.18.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.18.0
+Version: 0.18.1
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.18.0/README.md` & `basaran-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/__init__.py` & `basaran-0.18.1/basaran/__init__.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/__main__.py` & `basaran-0.18.1/basaran/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,17 +75,34 @@
         else:
             dtype_fn = dtype
 
         # If an option appears in both the query parameters and the request
         # body, the former takes precedence.
         if key in request.args:
             options[key] = request.args.get(key, dtype(), type=dtype_fn)
-        elif payload and key in payload and isinstance(payload[key], dtypes):
+        elif (
+            isinstance(payload, dict)
+            and key in payload
+            and isinstance(payload[key], dtypes)
+        ):
             options[key] = dtype(payload[key])
 
+        # Temporary workaround for multiple prompts (#198).
+        if (
+            key == "prompt"
+            and isinstance(payload, dict)
+            and key in payload
+            and isinstance(payload[key], list)
+        ):
+            prompts = payload[key]
+            if len(prompts) == 1:
+                options[key] = prompts[0]
+            elif len(prompts) > 1:
+                abort(400, description="only one prompt is supported")
+
     return options
 
 
 @app.route("/")
 def render_playground():
     """Render model playground."""
     if SERVER_NO_PLAYGROUND:
```

### Comparing `basaran-0.18.0/basaran/choice.py` & `basaran-0.18.1/basaran/choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/model.py` & `basaran-0.18.1/basaran/model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/static/playground.css` & `basaran-0.18.1/basaran/static/playground.css`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/static/playground.js` & `basaran-0.18.1/basaran/static/playground.js`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/static/presets.json` & `basaran-0.18.1/basaran/static/presets.json`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/templates/playground.html` & `basaran-0.18.1/basaran/templates/playground.html`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran/tokenizer.py` & `basaran-0.18.1/basaran/tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/basaran.egg-info/PKG-INFO` & `basaran-0.18.1/basaran.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basaran
-Version: 0.18.0
+Version: 0.18.1
 Summary: Open-source alternative to the OpenAI text completion API
 Author: Hyperonym
 Author-email: prompt@hyperonym.org
 License: MIT
 Keywords: api,huggingface,nlp,openai,transformer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `basaran-0.18.0/basaran.egg-info/SOURCES.txt` & `basaran-0.18.1/basaran.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/setup.py` & `basaran-0.18.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Script for building and distributing Python packages.
 """
 from setuptools import find_packages, setup
 
-VERSION = "0.18.0"
+VERSION = "0.18.1"
 
 setup(
     name="basaran",
     version=VERSION,
     description="Open-source alternative to the OpenAI text completion API",
     long_description="Basaran is an open-source alternative to the OpenAI "
     "text completion API. It provides a compatible streaming API for your "
```

### Comparing `basaran-0.18.0/tests/test_choice.py` & `basaran-0.18.1/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/tests/test_model.py` & `basaran-0.18.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/tests/test_tokenizer.py` & `basaran-0.18.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/utils/download.py` & `basaran-0.18.1/utils/download.py`

 * *Files identical despite different names*

### Comparing `basaran-0.18.0/utils/render.py` & `basaran-0.18.1/utils/render.py`

 * *Files identical despite different names*

