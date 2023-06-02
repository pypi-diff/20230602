# Comparing `tmp/render_engine_microblog-2023.4.1a5.tar.gz` & `tmp/render_engine_microblog-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_microblog-2023.4.1a5.tar", last modified: Sun Apr 16 21:52:11 2023, max compression
+gzip compressed data, was "render_engine_microblog-2023.6.1.tar", last modified: Fri Jun  2 06:03:53 2023, max compression
```

## Comparing `render_engine_microblog-2023.4.1a5.tar` & `render_engine_microblog-2023.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-16 21:52:11.000000 render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:52:11.578457 render_engine_microblog-2023.4.1a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-16 21:51:57.000000 render_engine_microblog-2023.4.1a5/tests/test_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.859848 render_engine_microblog-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-02 06:03:53.859848 render_engine_microblog-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12098 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:03:53.859848 render_engine_microblog-2023.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.855848 render_engine_microblog-2023.6.1/src/render_engine_microblog/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.859848 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-02 06:03:53.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-02 06:03:53.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:03:53.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 06:03:53.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 06:03:53.000000 render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:03:53.859848 render_engine_microblog-2023.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-02 06:03:40.000000 render_engine_microblog-2023.6.1/tests/test_collection.py
```

### Comparing `render_engine_microblog-2023.4.1a5/.DS_Store` & `render_engine_microblog-2023.6.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/.devcontainer/devcontainer.json` & `render_engine_microblog-2023.6.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/.github/workflows/publish.yml` & `render_engine_microblog-2023.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/.gitignore` & `render_engine_microblog-2023.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/.vscode/settings.json` & `render_engine_microblog-2023.6.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/CODE_OF_CONDUCT.md` & `render_engine_microblog-2023.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/LICENSE.md` & `render_engine_microblog-2023.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/PKG-INFO` & `render_engine_microblog-2023.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine_microblog
-Version: 2023.4.1a5
+Version: 2023.6.1
 Summary: Microblog Parser and Collection for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_microblog/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_microblog/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `render_engine_microblog-2023.4.1a5/README.md` & `render_engine_microblog-2023.6.1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/pyproject.toml` & `render_engine_microblog-2023.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/requirements.txt` & `render_engine_microblog-2023.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/src/render_engine_microblog/collection.py` & `render_engine_microblog-2023.6.1/src/render_engine_microblog/collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from dateutil import parser
-from render_engine.blog import Blog, BlogPost
+from render_engine.blog import Blog
+from render_engine.page import Page
 from render_engine.parsers.markdown import MarkdownPageParser
 
-class MicroBlogPost(BlogPost):
+class MicroBlogPost(Page):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.content = self._content
 
     @property
     def _slug(self):
         for attr in ["date_published", "date"]:
```

### Comparing `render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/PKG-INFO` & `render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine-microblog
-Version: 2023.4.1a5
+Version: 2023.6.1
 Summary: Microblog Parser and Collection for Render Engine
 Project-URL: homepage, https://github.com/kjaymiller/render_engine_microblog/
 Project-URL: repository, https://github.com/kjaymiller/render_engine_microblog/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.md
```

### Comparing `render_engine_microblog-2023.4.1a5/src/render_engine_microblog.egg-info/SOURCES.txt` & `render_engine_microblog-2023.6.1/src/render_engine_microblog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine_microblog-2023.4.1a5/tests/test_collection.py` & `render_engine_microblog-2023.6.1/tests/test_collection.py`

 * *Files identical despite different names*

