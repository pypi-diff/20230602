# Comparing `tmp/playwrightcapture-1.20.0.tar.gz` & `tmp/playwrightcapture-1.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.20.0.tar", max compression
+gzip compressed data, was "playwrightcapture-1.20.1.tar", max compression
```

## Comparing `playwrightcapture-1.20.0.tar` & `playwrightcapture-1.20.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.0/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.0/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.0/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    29544 2023-05-31 08:32:38.199235 playwrightcapture-1.20.0/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.0/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.0/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.0/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1734 2023-05-31 08:34:19.983617 playwrightcapture-1.20.0/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.20.0/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.20.1/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.20.1/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.20.1/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    30154 2023-06-02 13:20:55.055317 playwrightcapture-1.20.1/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.20.1/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.20.1/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.20.1/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1734 2023-06-02 13:23:02.048025 playwrightcapture-1.20.1/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.20.1/PKG-INFO
```

### Comparing `playwrightcapture-1.20.0/LICENSE` & `playwrightcapture-1.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.0/README.md` & `playwrightcapture-1.20.1/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.0/playwrightcapture/capture.py` & `playwrightcapture-1.20.1/playwrightcapture/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import asyncio
 import json
 import logging
 import os
 import random
+import re
 import time
 
 from tempfile import NamedTemporaryFile
 from typing import Optional, Dict, List, Union, Any, TypedDict, Literal
 
 import dateparser
 
@@ -172,32 +173,43 @@
         return self._headers
 
     @headers.setter
     def headers(self, headers: Optional[Union[str, Dict[str, str]]]) -> None:
         if not headers:
             return
         if isinstance(headers, str):
+            new_headers: Dict[str, str] = {}
             for header_line in headers.splitlines():
                 if header_line and ':' in header_line:
                     splitted = header_line.split(':', 1)
                     if splitted and len(splitted) == 2:
                         header, h_value = splitted
-                        if header and h_value:
-                            self._headers[header.strip()] = h_value.strip()
+                        if header.strip() and h_value.strip():
+                            new_headers[header.strip()] = h_value.strip()
         elif isinstance(headers, dict):
             # Check if they are valid
-            safe_headers = {name: value for name, value in headers.items() if isinstance(name, str) and isinstance(value, str) and name.strip() and value.strip()}
-            if safe_headers != headers:
+            new_headers = {name.strip(): value.strip() for name, value in headers.items() if isinstance(name, str) and isinstance(value, str) and name.strip() and value.strip()}
+            if new_headers != headers:
                 self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')
-            self._headers = safe_headers
         else:
             # This shouldn't happen, but somehow it does
             self.logger.critical(f'Headers contains invalid values:\n{json.dumps(headers, indent=2)}')  # type: ignore[unreachable]
             return
 
+        # Validate the new headers, only a subset of characters are accepted
+        # https://developers.cloudflare.com/rules/transform/request-header-modification/reference/header-format
+        for name, value in new_headers.items():
+            if re.match(r'^[\w-]+$', name) is None:
+                self.logger.warning(f'Invalid HTTP Header name: {name}')
+                continue
+            if not value.isprintable():
+                self.logger.warning(f'Invalid HTTP Header value: {value}')
+                continue
+            self._headers[name] = value
+
     @property
     def viewport(self) -> Optional[ViewportSize]:
         return self._viewport
 
     @viewport.setter
     def viewport(self, viewport: Optional[Dict[str, int]]) -> None:
         if not viewport:
```

### Comparing `playwrightcapture-1.20.0/playwrightcapture/helpers.py` & `playwrightcapture-1.20.1/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.20.0/pyproject.toml` & `playwrightcapture-1.20.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.20.0"
+version = "1.20.1"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.20.0/PKG-INFO` & `playwrightcapture-1.20.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.20.0
+Version: 1.20.1
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

