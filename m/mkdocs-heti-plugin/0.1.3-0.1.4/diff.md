# Comparing `tmp/mkdocs-heti-plugin-0.1.3.tar.gz` & `tmp/mkdocs-heti-plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-heti-plugin-0.1.3.tar", last modified: Wed Feb  8 03:10:35 2023, max compression
+gzip compressed data, was "mkdocs-heti-plugin-0.1.4.tar", last modified: Fri Jun  2 16:58:58 2023, max compression
```

## Comparing `mkdocs-heti-plugin-0.1.3.tar` & `mkdocs-heti-plugin-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/css/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/css/heti.css
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/heti.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 03:10:35.000000 mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 03:10:35.549043 mkdocs-heti-plugin-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-02-08 03:10:19.000000 mkdocs-heti-plugin-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/css/heti.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9754 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/heti.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 16:58:58.389898 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 16:58:58.000000 mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 16:58:58.393898 mkdocs-heti-plugin-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-02 16:58:45.000000 mkdocs-heti-plugin-0.1.4/setup.py
```

### Comparing `mkdocs-heti-plugin-0.1.3/LICENSE` & `mkdocs-heti-plugin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.3/PKG-INFO` & `mkdocs-heti-plugin-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-heti-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin that uses heti to improve Chinese typesetting
 Home-page: https://github.com/TonyCrane/mkdocs-heti-plugin
 Author: TonyCrane
 Author-email: me@tonycrane.cc
 License: MIT
 Keywords: mkdocs python markdown typesetting
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs-heti-plugin-0.1.3/README.md` & `mkdocs-heti-plugin-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/plugin.py` & `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/finder.py` & `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/finder.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,22 @@
         matchAggregation(self._textAggregation)
         return self._matches
 
     def prepMatch(self, match, matchIndex, characterOffset):
         if not match.group():
             raise Exception("cannot handle zero-length matches")
         d = dict()
-        d["text"] = match.group(1)
-        d["endIndex"] = characterOffset + match.end(1)
-        d["startIndex"] = characterOffset + match.start(1)
+        idx = 1
+        if len(match.groups()) != 1:
+            for i in range(3):
+                if match.group(i + 1):
+                    idx = i + 1
+        d["text"] = match.group(idx)
+        d["endIndex"] = characterOffset + match.end(idx)
+        d["startIndex"] = characterOffset + match.start(idx)
         d["index"] = matchIndex
         d["match"] = match
         return d
     
     def getAggregateText(self):
         self._elementFilter = self.options["filterElements"]
         self._forceContext = self.options["forceContext"]
@@ -143,24 +148,28 @@
                 startPortion = None
                 endPortion = None
                 innerPortions = []
                 match = matches.pop(0) if len(matches) else None
                 portionIndex = 0
                 if match is None:
                     break
-            elif (not doAvoidNode) and (hasattr(curNode, "children") or hasattr(curNode, "next_sibling")):
+            elif (
+                (not doAvoidNode) and 
+                ((hasattr(curNode, "children") and len(list(curNode.children)) > 0) or 
+                 (hasattr(curNode, "next_sibling") and curNode.next_sibling))
+            ):
                 if hasattr(curNode, "children") and len(list(curNode.children)) > 0:
                     nodeStack.append(curNode)
                     curNode = list(curNode.children)[0]
                 else:
                     curNode = curNode.next_sibling
                 continue
                 
             while True:
-                if hasattr(curNode, "next_sibling") and curNode.next_sibling:
+                if hasattr(curNode, "next_sibling") and curNode.next_sibling != None:
                     curNode = curNode.next_sibling
                     break
                 curNode = nodeStack.pop()
                 if curNode == node:
                     return
     
     def replaceMatch(self, match, startPortion, innerPortions, endPortion):
```

### Comparing `mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin/utils/heti.py` & `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin/utils/heti.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "dl", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", 
     "h4", "h5", "h6", "header", "hgroup", "hr", "main", "nav", "noscript", "ol", 
     "output", "p", "pre", "section", "ul", 
     "br", "li", "summary", "dt", "details", "rp", "rt", "rtc", 
     "script", "style", "img", "video", "audio", "canvas", "svg", "map", "object", 
     "input", "textarea", "select", "option", "optgroup", "button", 
     "table", "tbody", "thead", "th", "tr", "td", "caption", "col", "tfoot", "colgroup",
-    "ins", "del", "s"
+    "ins", "del", "s", "em"
 ]
 HETI_SKIPPED_ELEMENTS = [
     "br", "hr",
     "script", "style", "img", "video", "audio", "canvas", "svg", "map", "object",
     "input", "textarea", "select", "option", "optgroup", "button",
     "pre", "code", "heti-spacing", "heti-close"
 ]
```

### Comparing `mkdocs-heti-plugin-0.1.3/mkdocs_heti_plugin.egg-info/PKG-INFO` & `mkdocs-heti-plugin-0.1.4/mkdocs_heti_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-heti-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: A MkDocs plugin that uses heti to improve Chinese typesetting
 Home-page: https://github.com/TonyCrane/mkdocs-heti-plugin
 Author: TonyCrane
 Author-email: me@tonycrane.cc
 License: MIT
 Keywords: mkdocs python markdown typesetting
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mkdocs-heti-plugin-0.1.3/setup.py` & `mkdocs-heti-plugin-0.1.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(file_path) as file:
         content = file.read()
     return content if content else 'no content read'
 
 
 setup(
     name='mkdocs-heti-plugin',
-    version='0.1.3',
+    version='0.1.4',
     author='TonyCrane',
     author_email='me@tonycrane.cc',
     description='A MkDocs plugin that uses heti to improve Chinese typesetting',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown typesetting',
     url='https://github.com/TonyCrane/mkdocs-heti-plugin',
```

