# Comparing `tmp/mkdocs-heti-plugin-0.1.4.tar.gz` & `tmp/mkdocs-heti-plugin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-heti-plugin-0.1.4.tar", last modified: Fri Jun  2 16:58:58 2023, max compression
+gzip compressed data, was "mkdocs-heti-plugin-0.1.5.tar", last modified: Fri Jun  2 17:09:58 2023, max compression
```

## Comparing `mkdocs-heti-plugin-0.1.4.tar` & `mkdocs-heti-plugin-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/css/heti.css
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/heti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:58.995375 mkdocs-heti-plugin-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 17:09:58.995375 mkdocs-heti-plugin-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:58.991376 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:58.991376 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/css/heti.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:58.995375 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/heti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:09:58.991376 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 17:09:58.000000 mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:09:58.995375 mkdocs-heti-plugin-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-02 17:09:47.000000 mkdocs-heti-plugin-0.1.5/setup.py
```

### Comparing `mkdocs-heti-plugin-0.1.4/LICENSE` & `mkdocs-heti-plugin-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.4/PKG-INFO` & `mkdocs-heti-plugin-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-heti-plugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MkDocs plugin that uses heti to improve Chinese typesetting
 Home-page: https://github.com/TonyCrane/mkdocs-heti-plugin
 Author: TonyCrane
 Author-email: me@tonycrane.cc
 License: MIT
 Keywords: mkdocs python markdown typesetting
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs-heti-plugin-0.1.4/README.md` & `mkdocs-heti-plugin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/plugin.py` & `mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/finder.py` & `mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def prepMatch(self, match, matchIndex, characterOffset):
         if not match.group():
             raise Exception("cannot handle zero-length matches")
         d = dict()
         idx = 1
         if len(match.groups()) != 1:
-            for i in range(3):
+            for i in range(len(match.groups())):
                 if match.group(i + 1):
                     idx = i + 1
         d["text"] = match.group(idx)
         d["endIndex"] = characterOffset + match.end(idx)
         d["startIndex"] = characterOffset + match.start(idx)
         d["index"] = matchIndex
         d["match"] = match
```

### Comparing `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/heti.py` & `mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin/utils/heti.py`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/PKG-INFO` & `mkdocs-heti-plugin-0.1.5/mkdocs_heti_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-heti-plugin
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MkDocs plugin that uses heti to improve Chinese typesetting
 Home-page: https://github.com/TonyCrane/mkdocs-heti-plugin
 Author: TonyCrane
 Author-email: me@tonycrane.cc
 License: MIT
 Keywords: mkdocs python markdown typesetting
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs-heti-plugin-0.1.4/setup.py` & `mkdocs-heti-plugin-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-heti-plugin',
-    version='0.1.4',
+    version='0.1.5',
     author='TonyCrane',
     author_email='me@tonycrane.cc',
     description='A MkDocs plugin that uses heti to improve Chinese typesetting',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown typesetting',
     url='https://github.com/TonyCrane/mkdocs-heti-plugin',
```

