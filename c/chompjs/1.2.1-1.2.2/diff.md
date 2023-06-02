# Comparing `tmp/chompjs-1.2.1.tar.gz` & `tmp/chompjs-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chompjs-1.2.1.tar", last modified: Thu May 11 01:41:46 2023, max compression
+gzip compressed data, was "chompjs-1.2.2.tar", last modified: Fri Jun  2 12:09:29 2023, max compression
```

## Comparing `chompjs-1.2.1.tar` & `chompjs-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/
--rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.2.1/LICENSE
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.2.1/MANIFEST.in
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-05-11 01:41:46.058902 chompjs-1.2.1/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     6290 2023-05-10 13:40:46.000000 chompjs-1.2.1/README.md
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/_chompjs/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1735 2023-04-21 12:26:12.000000 chompjs-1.2.1/_chompjs/buffer.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      976 2023-04-21 12:26:15.000000 chompjs-1.2.1/_chompjs/buffer.h
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     5281 2023-05-11 01:40:03.000000 chompjs-1.2.1/_chompjs/module.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    12315 2023-05-08 02:40:08.000000 chompjs-1.2.1/_chompjs/parser.c
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3132 2023-05-08 02:40:08.000000 chompjs-1.2.1/_chompjs/parser.h
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/chompjs/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       55 2023-05-08 02:17:42.000000 chompjs-1.2.1/chompjs/__init__.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3468 2023-05-08 04:32:36.000000 chompjs-1.2.1/chompjs/chompjs.py
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    10944 2023-05-08 03:23:28.000000 chompjs-1.2.1/chompjs/test_parser.py
-drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-05-11 01:41:46.058902 chompjs-1.2.1/chompjs.egg-info/
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/PKG-INFO
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/SOURCES.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/dependency_links.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2023-05-11 01:41:46.000000 chompjs-1.2.1/chompjs.egg-info/top_level.txt
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2023-05-11 01:41:46.058902 chompjs-1.2.1/setup.cfg
--rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1764 2023-05-11 01:40:03.000000 chompjs-1.2.1/setup.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-06-02 12:09:29.464223 chompjs-1.2.2/
+-rw-r--r--   0 mariusz   (1000) mariusz   (1000)     1062 2020-02-27 18:25:01.000000 chompjs-1.2.2/LICENSE
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       15 2022-08-22 13:00:05.000000 chompjs-1.2.2/MANIFEST.in
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-06-02 12:09:29.464223 chompjs-1.2.2/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     6290 2023-05-10 13:40:46.000000 chompjs-1.2.2/README.md
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-06-02 12:09:29.464223 chompjs-1.2.2/_chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1822 2023-06-02 12:06:52.000000 chompjs-1.2.2/_chompjs/buffer.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      976 2023-04-21 12:26:15.000000 chompjs-1.2.2/_chompjs/buffer.h
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     5281 2023-05-11 01:40:03.000000 chompjs-1.2.2/_chompjs/module.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    12483 2023-06-02 12:06:49.000000 chompjs-1.2.2/_chompjs/parser.c
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3269 2023-06-02 12:06:49.000000 chompjs-1.2.2/_chompjs/parser.h
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-06-02 12:09:29.464223 chompjs-1.2.2/chompjs/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       55 2023-05-08 02:17:42.000000 chompjs-1.2.2/chompjs/__init__.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     3468 2023-05-08 04:32:36.000000 chompjs-1.2.2/chompjs/chompjs.py
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)    11074 2023-06-02 12:06:49.000000 chompjs-1.2.2/chompjs/test_parser.py
+drwxrwxr-x   0 mariusz   (1000) mariusz   (1000)        0 2023-06-02 12:09:29.464223 chompjs-1.2.2/chompjs.egg-info/
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     8897 2023-06-02 12:09:29.000000 chompjs-1.2.2/chompjs.egg-info/PKG-INFO
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)      314 2023-06-02 12:09:29.000000 chompjs-1.2.2/chompjs.egg-info/SOURCES.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)        1 2023-06-02 12:09:29.000000 chompjs-1.2.2/chompjs.egg-info/dependency_links.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       17 2023-06-02 12:09:29.000000 chompjs-1.2.2/chompjs.egg-info/top_level.txt
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)       38 2023-06-02 12:09:29.464223 chompjs-1.2.2/setup.cfg
+-rw-rw-r--   0 mariusz   (1000) mariusz   (1000)     1764 2023-06-02 12:08:51.000000 chompjs-1.2.2/setup.py
```

### Comparing `chompjs-1.2.1/LICENSE` & `chompjs-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.1/PKG-INFO` & `chompjs-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chompjs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Parsing JavaScript objects into Python dictionaries
 Home-page: https://github.com/Nykakin/chompjs
 Author: Mariusz Obajtek
 Author-email: nykakin@gmail.com
 License: UNKNOWN
 Description: # Chompjs
```

### Comparing `chompjs-1.2.1/README.md` & `chompjs-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.1/_chompjs/buffer.c` & `chompjs-1.2.2/_chompjs/buffer.c`

 * *Files 12% similar despite different names*

```diff
@@ -36,15 +36,20 @@
 void push_string(struct CharBuffer* buffer, const char* value, size_t len) {
     check_capacity(buffer, len);
     memcpy(buffer->data + buffer->index, value, len);
     buffer->index += len;
 }
 
 void push_number(struct CharBuffer* buffer, long value) {
-    int size_in_chars = (int)((ceil(log10(value))));
+    int size_in_chars;
+    if (value == 0) {
+        size_in_chars = 2;
+    } else {
+        size_in_chars = floor(log10(value)) + 2;
+    }
     check_capacity(buffer, size_in_chars);
     buffer->index += sprintf(buffer->data + buffer->index, "%ld", value);
 }
 
 void pop(struct CharBuffer* buffer) {
     buffer->index -= 1;
 }
```

### Comparing `chompjs-1.2.1/_chompjs/buffer.h` & `chompjs-1.2.2/_chompjs/buffer.h`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.1/_chompjs/module.c` & `chompjs-1.2.2/_chompjs/module.c`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.1/_chompjs/parser.c` & `chompjs-1.2.2/_chompjs/parser.c`

 * *Files 2% similar despite different names*

```diff
@@ -270,38 +270,28 @@
             
     return &states[ERROR_STATE];
 }
 
 struct State* handle_numeric(struct Lexer* lexer) {
     char c = next_char(lexer);
     if(c >= 49 && c <= 57) { // 1-9 range
-        do {
-            if(c != '_') {
-                emit(c, lexer);
-            } else {
-                lexer->input_position += 1;
-            }
-            c = tolower(lexer->input[lexer->input_position]);
-        } while(isdigit(c) || c == '.' || c == 'e' || c == 'E' || c == '+' || c =='-' || c == '_');
-        if(last_char(lexer) == '.') {
-            emit_in_place('0', lexer);
-        }
+        return handle_numeric_standard_base(lexer);
     } else if(c == '.') {
         emit_in_place('0', lexer);
         emit('.', lexer);
-        return handle_numeric(lexer);
+        return handle_numeric_standard_base(lexer);
     } else if(c == '-') {
         emit('-', lexer);
         return handle_numeric(lexer);
     } else if(c == '0') {
         char nc = tolower(lexer->input[lexer->input_position+1]);
         if(nc == '.') {
             emit('0', lexer);
             emit('.', lexer);
-            return handle_numeric(lexer);
+            return handle_numeric_standard_base(lexer);
         } else if(nc == 'x' || nc == 'X') {
             return handle_numeric_non_standard_base(lexer, 16);
         } else if(nc == 'o' || nc == 'O') {
             lexer->input_position += 2;
             return handle_numeric_non_standard_base(lexer, 8);
         } else if(isdigit(nc)) {
             return handle_numeric_non_standard_base(lexer, 8);
@@ -314,14 +304,30 @@
         }
     } else {
         return &states[ERROR_STATE];
     }
     return &states[JSON_STATE];
 }
 
+struct State* handle_numeric_standard_base(struct Lexer* lexer) {
+    char c = next_char(lexer);
+    do {
+        if(c != '_') {
+            emit(c, lexer);
+        } else {
+            lexer->input_position += 1;
+        }
+        c = tolower(lexer->input[lexer->input_position]);
+    } while(isdigit(c) || c == '.' || c == 'e' || c == 'E' || c == '+' || c =='-' || c == '_');
+    if(last_char(lexer) == '.') {
+        emit_in_place('0', lexer);
+    }
+    return &states[JSON_STATE];
+}
+
 struct State* handle_numeric_non_standard_base(struct Lexer* lexer, int base) {
     char* end;
     long n = strtol(lexer->input + lexer->input_position, &end, base);
     emit_number_in_place(n, lexer);
     lexer->input_position = end - lexer->input;
     return &states[JSON_STATE];
 }
```

### Comparing `chompjs-1.2.1/_chompjs/parser.h` & `chompjs-1.2.2/_chompjs/parser.h`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 struct State* end(struct Lexer* lexer);
 struct State* error(struct Lexer* lexer);
 
 /*
     Helper functions used in "value" state
     * handle_quoted - handles quoted strings
     * handle_numeric - handle numbers
+    * handle_numeric_standard_base - handle numbers in standard base-10
     * handle_numeric_non_standard_base - handle numbers in non-standard bases (hex, oct)
     * handle_unrecognized - save all unrecognized data as a string
 */
 struct State* handle_quoted(struct Lexer* lexer);
 struct State* handle_numeric(struct Lexer* lexer);
+struct State* handle_numeric_standard_base(struct Lexer* lexer);
 struct State* handle_numeric_non_standard_base(struct Lexer* lexer, int base);
 struct State* handle_unrecognized(struct Lexer* lexer);
 
 /**
     State wrapper
 */
 struct State {
```

### Comparing `chompjs-1.2.1/chompjs/chompjs.py` & `chompjs-1.2.2/chompjs/chompjs.py`

 * *Files identical despite different names*

### Comparing `chompjs-1.2.1/chompjs/test_parser.py` & `chompjs-1.2.2/chompjs/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -167,14 +167,18 @@
         ("[-.32]", [-0.32]),
         ("[12.]", [12.0]),
         ("[-12.]", [-12.0]),
         ("[12.32]", [12.32]),
         ("[-12.12]", [-12.12]),
         ("[3.1415926]", [3.1415926]),
         ("[.123456789]", [.123456789]),
+        ("[.0123]", [0.0123]),
+        ("[0.0123]", [0.0123]),
+        ("[-.0123]", [-0.0123]),
+        ("[-0.0123]", [-0.0123]),
         ("[3.1E+12]", [3.1E+12]),
         ("[3.1e+12]", [3.1E+12]),
         ("[.1e-23]", [.1e-23]),
         ("[.1e-23]", [.1e-23]),
     )
     def test_float_numeric_values(self, in_data, expected_data):
         result = parse_js_object(in_data)
```

### Comparing `chompjs-1.2.1/chompjs.egg-info/PKG-INFO` & `chompjs-1.2.2/chompjs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chompjs
-Version: 1.2.1
+Version: 1.2.2
 Summary: Parsing JavaScript objects into Python dictionaries
 Home-page: https://github.com/Nykakin/chompjs
 Author: Mariusz Obajtek
 Author-email: nykakin@gmail.com
 License: UNKNOWN
 Description: # Chompjs
```

### Comparing `chompjs-1.2.1/setup.py` & `chompjs-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     sources=['_chompjs/module.c', '_chompjs/parser.c', '_chompjs/buffer.c'],
     extra_compile_args=extra_compile_args,
     extra_link_args=extra_link_args,
 )
 
 setup(
     name='chompjs',
-    version='1.2.1',
+    version='1.2.2',
     description='Parsing JavaScript objects into Python dictionaries',
     author='Mariusz Obajtek',
     author_email='nykakin@gmail.com',
     keywords='parsing parser JavaScript json json5 webscrapping',
     python_requires='>=3',
     ext_modules=[chompjs_extension],
     classifiers=[
```

