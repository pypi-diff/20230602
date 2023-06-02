# Comparing `tmp/mkdocs_exporter-3.0.2.tar.gz` & `tmp/mkdocs_exporter-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-3.0.2.tar", max compression
+gzip compressed data, was "mkdocs_exporter-3.0.3.tar", max compression
```

## Comparing `mkdocs_exporter-3.0.2.tar` & `mkdocs_exporter-3.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.0.2/LICENSE
--rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.0.2/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1973 2023-05-29 15:28:16.602647 mkdocs_exporter-3.0.2/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.2/mkdocs_exporter/config.py
--rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.0.2/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.2/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1040 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4869 2023-05-30 20:15:51.466325 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2215 2023-05-27 18:11:03.211214 mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4115 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.0.2/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.0.2/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.0.2/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.2/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1618 2023-05-30 20:18:11.926283 mkdocs_exporter-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-08 13:15:16.904792 mkdocs_exporter-3.0.3/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-29 18:27:56.949905 mkdocs_exporter-3.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-08 15:45:32.453553 mkdocs_exporter-3.0.3/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1973 2023-06-02 10:45:00.862475 mkdocs_exporter-3.0.3/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0      264 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/config.py
+-rw-r--r--   0        0        0       96 2023-05-08 19:25:05.801769 mkdocs_exporter-3.0.3/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1935 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-06 21:44:34.488343 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:00:48.574613 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1121 2023-05-30 17:10:15.899396 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:48:51.834620 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-27 12:57:36.091210 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1040 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4869 2023-05-30 20:15:51.466325 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2181 2023-06-02 10:50:17.882385 mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     3860 2023-06-02 10:45:22.632469 mkdocs_exporter-3.0.3/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-07 12:23:00.605366 mkdocs_exporter-3.0.3/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:51.163540 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-08 14:16:39.063540 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      599 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1317 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-27 16:58:36.537218 mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1618 2023-06-02 11:12:57.682011 mkdocs_exporter-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mkdocs_exporter-3.0.3/PKG-INFO
```

### Comparing `mkdocs_exporter-3.0.2/LICENSE` & `mkdocs_exporter-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/README.md` & `mkdocs_exporter-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/browser.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/page.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugin.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,14 @@
       await self.browser.launch()
 
     preprocessor = Preprocessor(theme=page.theme)
     base = os.path.dirname(page.file.abs_dest_path)
     root = base.replace(unquote(page.url).rstrip('/'), '', 1).rstrip('/')
 
     preprocessor.preprocess(page.html)
-    preprocessor.remove_scripts()
     preprocessor.set_attribute('details:not([open])', 'open', 'open')
     page.theme.preprocess(preprocessor)
 
     for stylesheet in self.stylesheets:
       with open(stylesheet, 'r', encoding='utf-8') as file:
         preprocessor.stylesheet(file.read())
     for script in self.scripts:
```

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,24 +107,14 @@
     for selector in selectors:
       for element in self.html.select(selector):
         element.decompose()
 
     return self
 
 
-  def remove_scripts(self, predicate: Callable[[Any], bool] = lambda _: True) -> Preprocessor:
-    """Remove all script tags."""
-
-    for element in self.html.find_all('script'):
-      if predicate(element):
-        element.decompose()
-
-    return self
-
-
   def set_attribute(self, selector: str, key: str, value: str) -> Preprocessor:
     """Set an attribute on elements matching the given selector."""
 
     for element in self.html.select(selector):
       element.attrs[key] = value
 
     return self
```

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-3.0.3/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/theme.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/material/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-3.0.3/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-3.0.2/pyproject.toml` & `mkdocs_exporter-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "3.0.2"
+version = "3.0.3"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-3.0.2/PKG-INFO` & `mkdocs_exporter-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 3.0.2
+Version: 3.0.3
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.0.2 Summary: A highly-
+Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.0.3 Summary: A highly-
 configurable plugin for MkDocs that exports your pages to PDF files. Home-page:
 https://github.com/adrienbrignon/mkdocs-exporter Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon Author-email: adrien@brignon.dev Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

