# Comparing `tmp/googleapiutils2-0.8.4.tar.gz` & `tmp/googleapiutils2-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.8.4.tar", max compression
+gzip compressed data, was "googleapiutils2-0.8.5.tar", max compression
```

## Comparing `googleapiutils2-0.8.4.tar` & `googleapiutils2-0.8.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.4/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.4/README.md
--rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.4/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.4/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.4/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.4/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.4/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.4/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.4/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.4/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     9284 2023-06-02 03:12:44.689458 googleapiutils2-0.8.4/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    33788 2023-06-02 18:38:16.312935 googleapiutils2-0.8.4/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.8.4/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.4/googleapiutils2/utils.py
--rw-r--r--   0        0        0     1067 2023-06-02 18:39:50.555612 googleapiutils2-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.8.5/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.8.5/README.md
+-rw-r--r--   0        0        0      119 2023-06-02 03:26:51.461760 googleapiutils2-0.8.5/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-01 17:02:45.162747 googleapiutils2-0.8.5/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.8.5/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.8.5/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.8.5/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1105 2023-06-02 03:24:36.559913 googleapiutils2-0.8.5/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1460 2023-06-01 21:02:51.625940 googleapiutils2-0.8.5/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      198 2023-06-01 17:02:24.139670 googleapiutils2-0.8.5/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     9618 2023-06-02 19:09:36.958908 googleapiutils2-0.8.5/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    33788 2023-06-02 18:38:16.312935 googleapiutils2-0.8.5/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     5219 2023-06-02 18:15:23.863635 googleapiutils2-0.8.5/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     8927 2023-06-02 01:08:13.754688 googleapiutils2-0.8.5/googleapiutils2/utils.py
+-rw-r--r--   0        0        0     1067 2023-06-02 19:09:48.641713 googleapiutils2-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.8.5/PKG-INFO
```

### Comparing `googleapiutils2-0.8.4/LICENSE` & `googleapiutils2-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/README.md` & `googleapiutils2-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/drive/drive.py` & `googleapiutils2-0.8.5/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.8.5/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.8.5/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.8.5/googleapiutils2/sheets/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,23 +155,24 @@
 
 
 def expand_slices(
     row_ix: slice | int | EllipsisType,
     col_ix: slice | int | EllipsisType,
     shape: tuple[int, int] = DEFAULT_SHEET_SHAPE,
 ) -> str | None:
-    # TODO! optimize row ellipsis and col ellipsis types
-    # TODO! like 1:1, B:B, etc.
-
     def to_slice(ix: slice | int) -> slice:
         if isinstance(ix, slice):
             return ix
         elif isinstance(ix, str):
-            ix = A1_to_int(ix)
-            return slice(ix, ix)
+            if ":" in ix:
+                ix = ix.split(":")
+                return slice(A1_to_int(ix[0]), A1_to_int(ix[1]))
+            else:
+                ix = A1_to_int(ix)
+                return slice(ix, ix)
         elif isinstance(ix, int):
             return slice(ix, ix)
         elif ix is ...:
             return slice(..., ...)
         else:
             raise TypeError("Indices must be slices or integers.")
 
@@ -187,18 +188,27 @@
         start = 1 if start is ... else start
         stop = max_dim if stop is ... else stop
         # handle negative indices
         start = max_dim + start if start < 0 else start
         stop = max_dim + stop if stop < 0 else stop
         return slice(start, stop, step)
 
+    row_is_ellipsis = row_ix is ...
+    col_is_ellipsis = col_ix is ...
+
     row_ix, col_ix = to_slice(row_ix), to_slice(col_ix)  # type: ignore
     row_ix, col_ix = normalize_ix(row_ix, shape[0]), normalize_ix(col_ix, shape[1])  # type: ignore
-    row_ix, col_ix = slices_to_A1(row_ix, col_ix)  # type: ignore
 
+    if col_is_ellipsis:
+        return f"{row_ix.start}:{row_ix.stop}"
+    if row_is_ellipsis:
+        start, stop = int_to_A1(col_ix.start), int_to_A1(col_ix.stop)
+        return f"{start}:{stop}"
+
+    row_ix, col_ix = slices_to_A1(row_ix, col_ix)  # type: ignore
     return f"{row_ix}:{col_ix}" if row_ix != "" and col_ix != "" else None  # type: ignore
 
 
 def parse_sheet_slice_ixs(
     ixs: str | tuple[Any, ...], shape: tuple[int, int] = DEFAULT_SHEET_SHAPE
 ) -> tuple[str | None, str | None]:
     match ixs:
```

### Comparing `googleapiutils2-0.8.4/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.8.5/googleapiutils2/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.8.5/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/googleapiutils2/utils.py` & `googleapiutils2-0.8.5/googleapiutils2/utils.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.8.4/pyproject.toml` & `googleapiutils2-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.8.4"
+version = "0.8.5"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.8.4/PKG-INFO` & `googleapiutils2-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.8.4
+Version: 0.8.5
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

