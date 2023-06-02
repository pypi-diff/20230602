# Comparing `tmp/python_jsonpath-0.7.0.tar.gz` & `tmp/python_jsonpath-0.7.1.tar.gz`

## Comparing `python_jsonpath-0.7.0.tar` & `python_jsonpath-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/__about__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/__init__.py
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/env.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/exceptions.py
--rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/filter.py
--rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/lex.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/match.py
--rw-r--r--   0        0        0    20411 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/parse.py
--rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/path.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/py.typed
--rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/selectors.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/stream.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/token.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/__init__.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/arguments.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/count.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/is_instance.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/keys.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/length.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/match.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/search.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/typeof.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/jsonpath/function_extensions/value.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/README.md
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/__about__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/__init__.py
+-rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/env.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/exceptions.py
+-rw-r--r--   0        0        0    13166 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/filter.py
+-rw-r--r--   0        0        0    11063 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/lex.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/match.py
+-rw-r--r--   0        0        0    20477 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/parse.py
+-rw-r--r--   0        0        0    11290 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/path.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/py.typed
+-rw-r--r--   0        0        0    23699 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/selectors.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/stream.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/token.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/arguments.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/count.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/is_instance.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/keys.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/length.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/match.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/search.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/typeof.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/jsonpath/function_extensions/value.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/README.md
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 python_jsonpath-0.7.1/PKG-INFO
```

### Comparing `python_jsonpath-0.7.0/jsonpath/__init__.py` & `python_jsonpath-0.7.1/jsonpath/__init__.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/env.py` & `python_jsonpath-0.7.1/jsonpath/env.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/exceptions.py` & `python_jsonpath-0.7.1/jsonpath/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/filter.py` & `python_jsonpath-0.7.1/jsonpath/filter.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/lex.py` & `python_jsonpath-0.7.1/jsonpath/lex.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/match.py` & `python_jsonpath-0.7.1/jsonpath/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/parse.py` & `python_jsonpath-0.7.1/jsonpath/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,14 +239,15 @@
             TOKEN_NIL: self.parse_nil,
             TOKEN_NONE: self.parse_nil,
             TOKEN_NULL: self.parse_nil,
             TOKEN_STRING: self.parse_string_literal,
             TOKEN_TRUE: self.parse_boolean,
             TOKEN_ROOT: self.parse_root_path,
             TOKEN_SELF: self.parse_self_path,
+            TOKEN_FILTER_CONTEXT: self.parse_filter_context_path,
         }
 
     def parse(self, stream: TokenStream) -> Iterable[JSONPathSelector]:
         """Parse a JSONPath from a stream of tokens."""
         if stream.current.kind == TOKEN_ROOT:
             stream.next_token()
         yield from self.parse_path(stream, in_filter=False)
```

### Comparing `python_jsonpath-0.7.0/jsonpath/path.py` & `python_jsonpath-0.7.1/jsonpath/path.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/selectors.py` & `python_jsonpath-0.7.1/jsonpath/selectors.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/stream.py` & `python_jsonpath-0.7.1/jsonpath/stream.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/token.py` & `python_jsonpath-0.7.1/jsonpath/token.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/arguments.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/arguments.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/count.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/count.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/is_instance.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/is_instance.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/match.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/match.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/search.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/search.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/jsonpath/function_extensions/typeof.py` & `python_jsonpath-0.7.1/jsonpath/function_extensions/typeof.py`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/.gitignore` & `python_jsonpath-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/LICENSE.txt` & `python_jsonpath-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/README.md` & `python_jsonpath-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/pyproject.toml` & `python_jsonpath-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python_jsonpath-0.7.0/PKG-INFO` & `python_jsonpath-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-jsonpath
-Version: 0.7.0
+Version: 0.7.1
 Summary: Another JSONPath implementation for Python.
 Project-URL: Documentation, https://jg-rp.github.io/python-jsonpath/
 Project-URL: Issues, https://github.com/jg-rp/python-jsonpath/issues
 Project-URL: Source, https://github.com/jg-rp/python-jsonpath
 Author-email: James Prior <jamesgr.prior@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-jsonpath Version: 0.7.0 Summary: Another
+Metadata-Version: 2.1 Name: python-jsonpath Version: 0.7.1 Summary: Another
 JSONPath implementation for Python. Project-URL: Documentation, https://jg-
 rp.github.io/python-jsonpath/ Project-URL: Issues, https://github.com/jg-rp/
 python-jsonpath/issues Project-URL: Source, https://github.com/jg-rp/python-
 jsonpath Author-email: James Prior
 prior@gmail.com> License-Expression: MIT License-File: LICENSE.txt Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
```

