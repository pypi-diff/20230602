# Comparing `tmp/render_engine_rss-2023.4.1a2.tar.gz` & `tmp/render_engine_rss-2023.6.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_rss-2023.4.1a2.tar", last modified: Wed Apr  5 04:07:52 2023, max compression
+gzip compressed data, was "render_engine_rss-2023.6.1a1.tar", last modified: Fri Jun  2 06:00:05 2023, max compression
```

## Comparing `render_engine_rss-2023.4.1a2.tar` & `render_engine_rss-2023.6.1a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.537238 render_engine_rss-2023.4.1a2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.devcontainer/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.537238 render_engine_rss-2023.4.1a2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.537238 render_engine_rss-2023.4.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.537238 render_engine_rss-2023.4.1a2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.533238 render_engine_rss-2023.4.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.537238 render_engine_rss-2023.4.1a2/src/render_engine_rss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/src/render_engine_rss/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/collection.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-05 04:07:52.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-05 04:07:52.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 04:07:52.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-05 04:07:52.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-05 04:07:52.000000 render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 04:07:52.541238 render_engine_rss-2023.4.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/test/test_output.rss
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/test/test_rssCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-05 04:07:31.000000 render_engine_rss-2023.4.1a2/test/test_rssfeedpageparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.devcontainer/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.866780 render_engine_rss-2023.6.1a1/src/render_engine_rss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/src/render_engine_rss/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/collection.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 06:00:05.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-02 06:00:05.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 06:00:05.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-02 06:00:05.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 06:00:05.000000 render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 06:00:05.870780 render_engine_rss-2023.6.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/test/test_output.rss
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/test/test_rssCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-02 05:59:51.000000 render_engine_rss-2023.6.1a1/test/test_rssfeedpageparser.py
```

### Comparing `render_engine_rss-2023.4.1a2/.devcontainer/devcontainer.json` & `render_engine_rss-2023.6.1a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/.github/dependabot.yml` & `render_engine_rss-2023.6.1a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/.github/workflows/publish.yaml` & `render_engine_rss-2023.6.1a1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/.gitignore` & `render_engine_rss-2023.6.1a1/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -478,8 +478,8 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
-*/__pycache__/
+__pycache__
```

### Comparing `render_engine_rss-2023.4.1a2/.vscode/settings.json` & `render_engine_rss-2023.6.1a1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/pyproject.toml` & `render_engine_rss-2023.6.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/requirements.txt` & `render_engine_rss-2023.6.1a1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev pyproject.toml
 #
-attrs==22.2.0
+attrs==23.1.0
     # via pytest
 click==8.1.3
     # via typer
 dtyper==2.1.0
     # via render-engine
 feedparser==6.0.10
     # via render-engine-rss (pyproject.toml)
@@ -26,45 +26,45 @@
     # via render-engine
 markupsafe==2.1.2
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via render-engine
-packaging==23.0
+packaging==23.1
     # via pytest
 pluggy==1.0.0
     # via
     #   pytest
     #   render-engine
-pygments==2.14.0
+pygments==2.15.1
     # via rich
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   pytest-mock
     #   render-engine-rss (pyproject.toml)
 pytest-mock==3.10.0
     # via render-engine-rss (pyproject.toml)
 python-dateutil==2.8.2
     # via render-engine
 python-frontmatter==1.0.0
     # via render-engine
 python-slugify==8.0.1
     # via render-engine
 pyyaml==6.0
     # via python-frontmatter
-render-engine==2023.3.1b14
+render-engine==2023.5.2a1
     # via render-engine-rss (pyproject.toml)
-rich==13.3.3
+rich==13.3.5
     # via render-engine
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via python-dateutil
 smmap==5.0.0
     # via gitdb
 text-unidecode==1.3
     # via python-slugify
-typer==0.7.0
+typer==0.9.0
     # via
     #   dtyper
     #   render-engine
```

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss/.vscode/settings.json` & `render_engine_rss-2023.6.1a1/src/render_engine_rss/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/collection.cpython-311.pyc` & `render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/collection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss/__pycache__/parsers.cpython-311.pyc` & `render_engine_rss-2023.6.1a1/src/render_engine_rss/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss/collection.py` & `render_engine_rss-2023.6.1a1/src/render_engine_rss/collection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-from typing import Any
 from .parsers import RSSFeedPageParser
-import pluggy
 import feedparser
-from render_engine.collection import Collection
+from render_engine.blog import Blog
 
 
-class RSSCollection(Collection):
+class RSSCollection(Blog):
     PageParser = RSSFeedPageParser
     content_path = str
     sort_by = "published_parsed"
-    sort_reverse = True
 
-    def __init__(self, plugins: list = []):
+    def __init__(self):
         self.content = feedparser.parse(self.content_path)
-        super().__init__(plugins=plugins)
+        super().__init__()
 
     def get_partial_collection(self):
         for page in self.iter_content_path():
             yield self.get_page(page)
 
     def iter_content_path(self):
         return self.content.entries
```

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss/parsers.py` & `render_engine_rss-2023.6.1a1/src/render_engine_rss/parsers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import pathlib
-import feedparser
 from typing import Any
 
 from render_engine.parsers.base_parsers import BasePageParser
 
 
 def parse_rss_feed_entry(entry: dict) -> dict[str, Any]:
     if image := entry.get("image", None):
@@ -18,21 +16,24 @@
         elif isinstance(content, str):
             return entry, content
 
     elif content := entry.pop("summary", None):
         if isinstance(content, str):
             return entry, content
 
+        elif isinstance(content, dict):
+            return entry, content["summary"]
+
     return entry, ""
 
 
 class RSSFeedPageParser(BasePageParser):
     @staticmethod
     def parse_content_path(content: dict) -> tuple[dict[str, Any], str]:
-        """Fething content and atttributes from a content_path"""
+        """Fetching content and atttributes from a content_path"""
         return parse_rss_feed_entry(content)
 
     @staticmethod
     def parse_content(content: str) -> tuple[dict[str, Any], str]:
         return parse_rss_feed_entry(content)
```

### Comparing `render_engine_rss-2023.4.1a2/src/render_engine_rss.egg-info/SOURCES.txt` & `render_engine_rss-2023.6.1a1/src/render_engine_rss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/test/test_output.rss` & `render_engine_rss-2023.6.1a1/test/test_output.rss`

 * *Files identical despite different names*

### Comparing `render_engine_rss-2023.4.1a2/test/test_rssCollection.py` & `render_engine_rss-2023.6.1a1/test/test_rssCollection.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,42 +5,46 @@
     content_path = "./test/test_output.rss"
     template = "test.html"
 
 class TestRSSCollection:
 
     collection = SimpleRSSCollection()
 
-    @pytest.mark.skip()
     def test_collection_parses_url(self):
         """
-        Test taht the collection can parse a feed url into pages
-        17 Mar 2023 - With feedparser having a 'cgi deprecation warning' this test is to ensure we can still parse a url
+        Test the collection can parse a feed url into pages
+        17 Mar 2023 - With feedparser having a 'cgi deprecation warning'
+        this test is to ensure we can still parse a url
         
         # TODO: Figure out test for url parsing.
         """
-        assert len(list(self.collection.__iter__())) == 1 
+        assert len([p for p in self.collection.__iter__()]) == 2 
 
 
     @pytest.mark.parametrize(
             "index, title",
             [
                 (0, "Test Title 1"),
                 (1, "Test Title 2")
             ],
     )
     def test_collection_parses_pages_string(self, index, title):
         """Test that the collection can parse a feed into pages
-        17 Mar 2023 - With feedparser having a 'cgi deprecation warning' this test is to ensure we can still parse a filepath
+        17 Mar 2023 - With feedparser having a 'cgi deprecation warning'
+        this test is to ensure we can still parse a filepath
         """
         assert [x.title for x in self.collection][index] == title
 
 
     def test_collection_includes_template(self):
         """Test that the collection can parse a feed into pages with templates"""
         for x in self.collection:
             assert x.template == "test.html"
 
 
     def test_collection_sorts_by_published_parsed(self):
         """Test that the collection can parse a feed into pages with templates"""
 
-        assert self.collection.sorted_pages[0].title == "Test Title 2"
+        assert self.collection.sorted_pages[0].title == "Test Title 2"
+
+    def test_parse_collection_object(self):
+        assert self.
```

### Comparing `render_engine_rss-2023.4.1a2/test/test_rssfeedpageparser.py` & `render_engine_rss-2023.6.1a1/test/test_rssfeedpageparser.py`

 * *Files identical despite different names*

