# Comparing `tmp/xtn-0.2.0.tar.gz` & `tmp/xtn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtn-0.2.0.tar", max compression
+gzip compressed data, was "xtn-0.3.0.tar", max compression
```

## Comparing `xtn-0.2.0.tar` & `xtn-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      458 2023-05-17 17:02:17.559755 xtn-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      575 2023-05-13 04:15:51.322967 xtn-0.2.0/README.md
--rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.2.0/xtn/__init__.py
--rw-r--r--   0        0        0    15534 2023-05-17 16:59:10.865759 xtn-0.2.0/xtn/_xtn.py
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 xtn-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      458 2023-06-02 19:16:46.582859 xtn-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      575 2023-05-13 04:15:51.322967 xtn-0.3.0/README.md
+-rw-r--r--   0        0        0      122 2023-05-12 15:09:11.486768 xtn-0.3.0/xtn/__init__.py
+-rw-r--r--   0        0        0    15761 2023-06-02 19:10:36.853649 xtn-0.3.0/xtn/_xtn.py
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 xtn-0.3.0/PKG-INFO
```

### Comparing `xtn-0.2.0/README.md` & `xtn-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `xtn-0.2.0/xtn/_xtn.py` & `xtn-0.3.0/xtn/_xtn.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     ARRAY_ELEMENT_MUST_START_WITH_PLUS = 6
     MISSING_COLON = 7
     UNMATCHED_CLOSE_MARKER = 8
     MISSING_CLOSE_MARKER = 9
     INDENTATION_MUST_BE_SPACE_OR_TAB = 10
     INDENTATION_MUST_NOT_BE_MIXED = 11
     INSUFFICIENT_INDENTATION = 12
+    ARRAY_ELEMENT_MUST_NOT_HAVE_A_KEY = 13
+    OBJECT_KEYS_CANNOT_BE_REPEATED = 14
+    INCORRECT_INDENTATION = 15
 
 
 class XtnException(Exception):
     def __init__(self, code: XtnErrorCode, message: str, *args: object) -> None:
         super().__init__(message, *args)
         self.code = code
         self.message = message
@@ -155,14 +158,17 @@
     mode: Literal[_Mode.OBJECT] = _Mode.OBJECT
 
     def set(self, name: str, value: dict[str, Any] | list | str, raise_error: Callable[[XtnErrorCode, str], NoReturn], convert_spaces: bool = True):
         # verify that name does not have disallowed characters
         name = _convert_spaces(name, True)
         if convert_spaces and isinstance(value, str):
             value = _convert_spaces(value, False)
+        if name in self.current:
+            raise_error(XtnErrorCode.OBJECT_KEYS_CANNOT_BE_REPEATED,
+                        f"Object keys cannot be repeated. {name} already exists.")
         if self.target is None:
             self.current[name] = value
             return None
         else:
             child = _make_Xtn(value)
             self.current[name] = child
             return child
@@ -176,16 +182,20 @@
     mode: Literal[_Mode.ARRAY] = _Mode.ARRAY
 
     def set(self, name: str, value: dict[str, Any] | list | str, raise_error: Callable[[XtnErrorCode, str], NoReturn], convert_spaces: bool = True):
         name = _convert_spaces(name, True)
         if convert_spaces and isinstance(value, str):
             value = _convert_spaces(value, False)
         if name != '+':
-            raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_START_WITH_PLUS,
-                        "An array element must start with a plus")
+            if name.startswith('+'):
+                raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_NOT_HAVE_A_KEY,
+                            "An array element cannot be named")
+            else:
+                raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_START_WITH_PLUS,
+                            "An array element must start with a plus")
         if self.target is None:
             self.current.append(value)
             return None
         else:
             child = _make_Xtn(value)
             self.current.append(child)
             return child
@@ -195,15 +205,14 @@
 class _MultilineState:
     start_line: int
     name: str
     parent_state: _ObjectState | _ArrayState
     indent: str
     indent_char: str = ' '
     exp_indent: str | None = None
-    cur_indent: str = ''
     text: str = ''
     target = None
     mode: Literal[_Mode.MULTILINE] = _Mode.MULTILINE
 
 
 def _load(f: TextIO, target: XtnObject | None) -> dict[str, Any]:
     top_level = {} if target is None else target.elements
@@ -243,56 +252,49 @@
     for i, orig_line in enumerate(f):
         line = orig_line
         state = stack[-1]
         if state.mode == _Mode.MULTILINE:
             if state.exp_indent is None:
                 if len(state.indent) > 0:
                     state.indent_char = state.indent[0]
-                    state.exp_indent = state.indent + \
-                        state.indent_char * (1 if state.indent_char == '\t' else 4)
+                    state.exp_indent = state.indent + state.indent_char * \
+                        (1 if state.indent_char == '\t' else 4)
                 elif line[:1] == '\t':
                     state.exp_indent = '\t'
                     state.indent_char = '\t'
                 else:
                     state.exp_indent = '    '
                     state.indent_char = ' '
-                state.cur_indent = state.exp_indent
-            cur_indent_len = len(state.cur_indent)
+            exp_indent_len = len(state.exp_indent)
             act_indent_len = 0
-            if cur_indent_len > 0:
-                prefix = line[0:cur_indent_len]
-                act_indent = prefix[:(
-                    len(prefix) - len(prefix.lstrip(state.exp_indent[0])))]
-                act_indent_len = len(act_indent)
-                prefix = prefix[act_indent_len:act_indent_len+1]
-                if act_indent_len < cur_indent_len and prefix.isspace() and prefix != '\n':
-                    raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED,
-                                f"Indentation for a complex text value can use either spaces or tabs but not both")
-                line = line[act_indent_len:]
-                if act_indent_len < cur_indent_len:
-                    state.cur_indent = act_indent
-            if act_indent_len < len(state.exp_indent):
-                close_ind = line.find('--', None, len(state.exp_indent) - act_indent_len)
-                if close_ind >= 0:
-                    prefix = line[:close_ind]
-                    if len(prefix) == 0 or prefix.isspace():
-                        if line[close_ind:(close_ind+4)] == '----' and (len(line) == close_ind + 4 or line[(close_ind+4):].isspace()):
-                            if act_indent_len + close_ind <= len(state.indent):
-                                if len(state.indent) > 0 and len(prefix.lstrip(state.indent_char)) != 0:
-                                    raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED, f"Indentation for a complex text value can use either spaces or tabs but not both")
-                                
-                                child_target = state.parent_state.set(state.name, state.text[0:-1], raise_error, convert_spaces=False)
-                                if child_target is not None:
-                                    child_target.force_multiline = True  # type: ignore
-                                    attach_comments(child_target)
-                                stack.pop()
-                                continue
-                            
-                        raise_error(XtnErrorCode.INSUFFICIENT_INDENTATION, f"Lines starting with two or more dashes must be indented by at least 4 spaces or a tab compared to the key line")
-            
+            prefix = line[0:exp_indent_len]
+            act_indent = prefix[:(
+                len(prefix) - len(prefix.lstrip(state.indent_char)))]
+            act_indent_len = len(act_indent)
+            prefix = prefix[act_indent_len:act_indent_len+1]
+            if act_indent_len < exp_indent_len and prefix.isspace() and prefix != '\n':
+                raise_error(XtnErrorCode.INDENTATION_MUST_NOT_BE_MIXED,
+                            f"Indentation for a complex text value can use either spaces or tabs but not both")
+            line = line[act_indent_len:]
+            if act_indent_len < exp_indent_len:
+                if line.startswith('----') and (len(line) == 4 or line[4:].isspace()):
+                    if act_indent_len == len(state.indent):
+                        child_target = state.parent_state.set(
+                            state.name, state.text[0:-1], raise_error, convert_spaces=False)
+                        if child_target is not None:
+                            child_target.force_multiline = True  # type: ignore
+                            attach_comments(child_target)
+                        stack.pop()
+                        continue
+                    raise_error(XtnErrorCode.INCORRECT_INDENTATION,
+                                f"The indentation on the closing line for a complex text value must exactly match the key line")
+                if prefix != '\n':
+                    raise_error(XtnErrorCode.INSUFFICIENT_INDENTATION,
+                                f"Lines of complex text must be indented by 4 spaces or a tab compared to the key line")
+
             state.text = state.text + line
         else:
             line = line.strip()
             if line.startswith('#'):
                 record_comment(line)
                 continue
             if (len(line) == 0):
@@ -301,15 +303,15 @@
             left, sep, right = line.partition(':')
             left = left.rstrip()
             right = right.lstrip()
             if sep == ':':
                 if len(left) == 0:
                     raise_error(XtnErrorCode.LINE_MUST_NOT_START_WITH_COLON,
                                 f"A line cannot start with a colon")
-                elif left.startswith('+') and state.mode == _Mode.OBJECT and not state.in_array:
+                elif left.startswith('+') and state.mode == _Mode.OBJECT:
                     raise_error(XtnErrorCode.PLUS_ENCOUNTERED_OUTSIDE_ARRAY,
                                 f"A line cannot start with a plus outside the context of an array")
 
                 if left.endswith('{}'):
                     if len(right) > 0:
                         raise_error(XtnErrorCode.OBJECT_MUST_BE_ON_NEW_LINE,
                                     f"An object must start on a new line")
@@ -325,15 +327,15 @@
                                     f"An array must start on a new line")
                     name = left[0:-2].rstrip()
                     obj = []
                     child_target = state.set(name, obj, raise_error)
                     attach_comments(child_target)
                     # type: ignore
                     stack.append(_ArrayState(
-                        start_line=i, current=obj, target=child_target))
+                        start_line=i, current=obj, target=child_target))  # type: ignore
                 elif left.endswith("''"):
                     indent = orig_line[:orig_line.find(left[0])]
                     if len(indent) > 0:
                         indent_char = indent[0]
                         if indent_char != ' ' and indent_char != '\t':
                             raise_error(XtnErrorCode.INDENTATION_MUST_BE_SPACE_OR_TAB,
                                         f"Indentation for a complex text value must be a space (32) or tab (9) character")
@@ -354,16 +356,24 @@
             elif left.startswith('----') and (len(left) == 4 or left[4:].isspace()):
                 attach_trailing_comments(stack[-1].target)
                 stack.pop()
                 if len(stack) == 0:
                     raise_error(XtnErrorCode.UNMATCHED_CLOSE_MARKER,
                                 "The close marker ---- does not match any open object or array")
             else:
-                raise_error(XtnErrorCode.MISSING_COLON,
-                            f"A colon was expected")
+                if state.mode == _Mode.ARRAY:
+                    if left[0] == '+':
+                        raise_error(XtnErrorCode.MISSING_COLON,
+                                    f"A colon was expected")
+                    else:
+                        raise_error(XtnErrorCode.ARRAY_ELEMENT_MUST_START_WITH_PLUS,
+                                    f"An array element must start with a plus")
+                else:
+                    raise_error(XtnErrorCode.MISSING_COLON,
+                                f"A colon was expected")
 
     i += 1
     if len(stack) > 1:
         raise_error(XtnErrorCode.MISSING_CLOSE_MARKER,
                     "A close marker ---- was expected")
     return top_level
```

### Comparing `xtn-0.2.0/PKG-INFO` & `xtn-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtn
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library for working with the xtn format
 Home-page: https://github.com/koustubhmoharir/xtn
 License: MIT
 Author: Koustubh Moharir
 Author-email: koustubhmoharir@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

