# Comparing `tmp/render_engine_youtube_embed-2023.3.2a1.tar.gz` & `tmp/render_engine_youtube_embed-2023.6.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine_youtube_embed-2023.3.2a1.tar", last modified: Wed Mar 29 06:35:10 2023, max compression
+gzip compressed data, was "render_engine_youtube_embed-2023.6.2a1.tar", last modified: Fri Jun  2 13:14:10 2023, max compression
```

## Comparing `render_engine_youtube_embed-2023.3.2a1.tar` & `render_engine_youtube_embed-2023.6.2a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.823507 render_engine_youtube_embed-2023.3.2a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.819507 render_engine_youtube_embed-2023.3.2a1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.819507 render_engine_youtube_embed-2023.3.2a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.819507 render_engine_youtube_embed-2023.3.2a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-29 06:35:10.823507 render_engine_youtube_embed-2023.3.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 06:35:10.823507 render_engine_youtube_embed-2023.3.2a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.819507 render_engine_youtube_embed-2023.3.2a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.819507 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed/youtube_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.823507 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-29 06:35:10.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-29 06:35:10.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 06:35:10.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-29 06:35:10.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 06:35:10.000000 render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 06:35:10.823507 render_engine_youtube_embed-2023.3.2a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-29 06:34:52.000000 render_engine_youtube_embed-2023.3.2a1/tests/test_link_detect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.131380 render_engine_youtube_embed-2023.6.2a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 13:14:10.131380 render_engine_youtube_embed-2023.6.2a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.123380 render_engine_youtube_embed-2023.6.2a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed/youtube_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-02 13:14:10.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 13:14:10.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 13:14:10.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 13:14:10.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-02 13:14:10.000000 render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 13:14:10.127380 render_engine_youtube_embed-2023.6.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 13:13:49.000000 render_engine_youtube_embed-2023.6.2a1/tests/test_link_detect.py
```

### Comparing `render_engine_youtube_embed-2023.3.2a1/.devcontainer/devcontainer.json` & `render_engine_youtube_embed-2023.6.2a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/.github/workflows/publish.yml` & `render_engine_youtube_embed-2023.6.2a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/.gitignore` & `render_engine_youtube_embed-2023.6.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/CODE_OF_CONDUCT.md` & `render_engine_youtube_embed-2023.6.2a1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/LICENSE` & `render_engine_youtube_embed-2023.6.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/PKG-INFO` & `render_engine_youtube_embed-2023.6.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine_youtube_embed
-Version: 2023.3.2a1
+Version: 2023.6.2a1
 Summary: A Render Engine Plugin for replacing Youtube Links with Embed Links
 Project-URL: homepage, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Project-URL: repository, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_youtube_embed-2023.3.2a1/README.md` & `render_engine_youtube_embed-2023.6.2a1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/pyproject.toml` & `render_engine_youtube_embed-2023.6.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed/youtube_embed.py` & `render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed/youtube_embed.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-import dataclasses
 import typing
 import re
+from urllib.parse import urlsplit
 
 import logging
 import itertools
 
 
 def extract_youtube_id(url: str) -> str:
     """
     Extract the video id from a youtube url
     """
 
-    matches = (
-        ('https://www.youtube.com/watch?v=', '='),
-        ('https://www.youtube.com/watch/', '/'),
-        ('https://www.youtube.com/shorts/', '/'),
-        ('https://youtu.be/', '/'),
-    )
-
-    for matcher, splitter in matches:
-        if url.startswith(matcher):
-            return url.split(splitter)[-1]
+    # split the url from the query string
+    url = re.sub(r'\<\/{0,1}p\>', '', url)
+    url = urlsplit(url)
+    print(url)
+    
+    # check for v in the query string
+    if 'v' in url.query:
+        return url.query.split('=')[-1]
+
+    else:
+        return url.path.split('/')[-1]
+
+
 
 
 def get_all_links(content: str) -> typing.Generator[str, None, None]:
     """get all youtube link types"""
 
-    youtube_links = r'^ *https://www.youtube.com/watch\?v=[\w\d_]+ *$'
-    youtube_slash_links = r'^ *https://www.youtube.com/watch\/[\w\d_]+ *$'
-    youtube_shortlinks = r'^ *https://youtu.be/[\w\d_]+ *$'
-    youtube_shorts = r'^ *https://www.youtube.com/shorts/[\w\d_]+ *$'
+    youtube_links = r'^ *<p>https://www.youtube.com/watch\?v=[\w\d_]+</p> *$'
+    youtube_slash_links = r'^ *<p>https://www.youtube.com/watch\/[\w\d_]+</p> *$'
+    youtube_shortlinks = r'^ *<p>https://youtu.be/[\w\d_]+</p> *$'
+    youtube_shorts = r'^ *<p>https://www.youtube.com/shorts/[\w\d_]+</p> *$'
 
     links = [youtube_links, youtube_slash_links, youtube_shortlinks, youtube_shorts]
     link_groups = [re.findall(link_type, content, re.MULTILINE) for link_type in links]
 
     return itertools.chain(*link_groups)
 
 def replace_youtube_links_with_embeds(content: str) -> str:
```

### Comparing `render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO` & `render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine-youtube-embed
-Version: 2023.3.2a1
+Version: 2023.6.2a1
 Summary: A Render Engine Plugin for replacing Youtube Links with Embed Links
 Project-URL: homepage, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Project-URL: repository, https://github.com/kjaymiller/render-engine-youtube-link-embed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `render_engine_youtube_embed-2023.3.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt` & `render_engine_youtube_embed-2023.6.2a1/src/render_engine_youtube_embed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine_youtube_embed-2023.3.2a1/tests/test_link_detect.py` & `render_engine_youtube_embed-2023.6.2a1/tests/test_link_detect.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,25 @@
+import pytest
 
 from render_engine_youtube_embed.youtube_embed import (
     extract_youtube_id,
     replace_youtube_links_with_embeds,
 )
 
-def test_youtube_links_found():
+@pytest.mark.parametrize(
+    "test_url, expected_id",
+    [
+        ("<p>https://www.youtube.com/watch?v=5qap5aO4i9A</p>", "5qap5aO4i9A"),
+        ("<p>https://www.youtube.com/watch/5qap5aO4i9A</p>", "5qap5aO4i9A"),
+        ("<p>https://www.youtube.com/shorts/5qap5aO4i9A</p>", "5qap5aO4i9A"),
+        ("<p>https://youtu.be/5qap5aO4i9A<p>", "5qap5aO4i9A"),
+    ]
+)
+def test_youtube_links_found(test_url, expected_id):
     """Test that youtube links are found"""
-    test_url = "https://www.youtube.com/watch?v=5qap5aO4i9A"
-    assert extract_youtube_id(test_url) == "5qap5aO4i9A"
-
-def test_youtube_slash_link():
-    """Tests that youtube links with a slash are found"""
-    test_url = "https://www.youtube.com/watch/5qap5aO4i9A"
-    assert extract_youtube_id(test_url) == "5qap5aO4i9A"
-
-def test_youtube_shorts_link():
-    """Tests that youtube shorts links are found"""
-    test_url = "https://www.youtube.com/shorts/5qap5aO4i9A"
-    assert extract_youtube_id(test_url) == "5qap5aO4i9A"
-
-def test_youtube_shortlinks_found():
-    """Test that youtube shortlinks are found"""
-    test_url = "https://youtu.be/5qap5aO4i9A"
-    assert extract_youtube_id(test_url) == "5qap5aO4i9A"
+    assert extract_youtube_id(test_url) == expected_id
 
 def test_youtube_link_replaced_with_embed():
     """Tests that youtube links are replaced with embeds"""
-    test_url = "https://www.youtube.com/watch?v=5qap5aO4i9A"
+    test_url = "<p>https://www.youtube.com/watch?v=5qap5aO4i9A</p>"
     expected_text = "<iframe width='560' height='315' src='https://www.youtube.com/embed/5qap5aO4i9A' frameborder='0' allow='accelerometer; autoplay; clipboard-write; encrypted-media;' allowfullscreen></iframe>"
     assert replace_youtube_links_with_embeds(test_url) == expected_text
```

