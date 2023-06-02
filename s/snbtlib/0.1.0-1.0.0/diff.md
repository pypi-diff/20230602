# Comparing `tmp/snbtlib-0.1.0.tar.gz` & `tmp/snbtlib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snbtlib-0.1.0.tar", last modified: Wed May 24 01:39:48 2023, max compression
+gzip compressed data, was "snbtlib-1.0.0.tar", last modified: Fri Jun  2 05:48:00 2023, max compression
```

## Comparing `snbtlib-0.1.0.tar` & `snbtlib-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.035952 snbtlib-0.1.0/
--rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      716 2023-05-24 01:39:48.035952 snbtlib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 01:39:48.036951 snbtlib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      558 2023-05-24 01:39:29.000000 snbtlib-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.032951 snbtlib-0.1.0/snbtlib/
--rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-0.1.0/snbtlib/__init__.py
--rw-rw-rw-   0        0        0     7388 2023-05-24 01:38:42.000000 snbtlib-0.1.0/snbtlib/formatter.py
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.034953 snbtlib-0.1.0/snbtlib.egg-info/
--rw-rw-rw-   0        0        0      716 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-24 01:39:48.000000 snbtlib-0.1.0/snbtlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 01:39:48.035952 snbtlib-0.1.0/test/
--rw-rw-rw-   0        0        0      197 2023-04-18 02:16:35.000000 snbtlib-0.1.0/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.443722 snbtlib-1.0.0/
+-rw-rw-rw-   0        0        0     1085 2023-02-07 06:40:54.000000 snbtlib-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      716 2023-06-02 05:48:00.443722 snbtlib-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-03-08 06:57:28.000000 snbtlib-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 05:48:00.443722 snbtlib-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-05-24 01:43:44.000000 snbtlib-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.439722 snbtlib-1.0.0/snbtlib/
+-rw-rw-rw-   0        0        0      302 2023-04-18 02:12:57.000000 snbtlib-1.0.0/snbtlib/__init__.py
+-rw-rw-rw-   0        0        0     7009 2023-06-02 05:46:10.000000 snbtlib-1.0.0/snbtlib/formatter.py
+drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.442721 snbtlib-1.0.0/snbtlib.egg-info/
+-rw-rw-rw-   0        0        0      716 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      214 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 05:48:00.000000 snbtlib-1.0.0/snbtlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 05:48:00.442721 snbtlib-1.0.0/test/
+-rw-rw-rw-   0        0        0      224 2023-05-24 02:31:49.000000 snbtlib-1.0.0/test/test.py
```

### Comparing `snbtlib-0.1.0/LICENSE` & `snbtlib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snbtlib-0.1.0/PKG-INFO` & `snbtlib-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.1.0
+Version: 1.0.0
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

### Comparing `snbtlib-0.1.0/setup.py` & `snbtlib-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='snbtlib',
-    version='0.1.0',
+    version='1.0.0',
     keywords='minecraft',
     description='a formatter for snbt from minecraft',
     long_description=long_description,
     license='MIT License',
     url='',
     author='Tryanks',
     author_email='tryanks@outlook.com',
```

### Comparing `snbtlib-0.1.0/snbtlib/formatter.py` & `snbtlib-1.0.0/snbtlib/formatter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 from io import StringIO
 from json import dumps as j_dumps, loads as j_loads
+from re import compile, sub
+
+annotation = compile(r'^\s+?//.*$')
+annotation2 = compile(r'^\s+?#.*$')
 
 
 class SnbtReader:
     text = ''
     index = 0
 
     def __init__(self, t: str):
+        # Annotation filter
+        t = t.replace('\r', '')
+        t = sub(annotation, '', t)
+        t = sub(annotation2, '', t)
         self.text = t
 
     def next(self):
         self.index += 1
         if self.index - 1 >= len(self.text):
             return False
         if self.text[self.index - 1].isspace() and not self.text[self.index - 1] == '\n':
@@ -24,29 +32,30 @@
         return self.text[self.index - 1]
 
     def get_point(self):
         return self.text[self.index - 1]
 
     def last(self):
         self.index -= 1
+        return self.text[self.index - 1]
 
 
 class Token:
     EMPTY = -1
     BEGIN_DICT = 0
-    END_DICT = 1
-    BEGIN_LIST = 2
-    END_LIST = 3
-    ENTER = 4
-    COLON = 5
-    STRING = 6
-    NUMBER = 7
-    KEY = 8
-    BOOL = 9
-    INTEGER = 10
+    COLON = 2
+    END_DICT = 4
+    BEGIN_LIST = 5
+    END_LIST = 6
+    ENTER = 7
+    STRING = 8
+    STRING_IN_QUOTE = 999
+    NUMBER = 9
+    BOOL = 10
+    INTEGER = 11
 
 
 class TokenElement:
     type = Token.EMPTY
     value = ''
 
 
@@ -77,15 +86,15 @@
             snbt_dict = list_iterator(iterator)
             break
     if format:
         return j_dumps(snbt_dict, ensure_ascii=False, indent=4)
     return snbt_dict
 
 
-def dumps(json, indent=0):
+def dumps(json, indent=0, compact=False):
     if type(json) == str:
         json = j_loads(json)
     text = ''
     if type(json) == dict:
         if not json:
             text += '{ }\n'
         else:
@@ -108,15 +117,15 @@
             else:
                 text += '[\n'
             indent += 1
             for value in json:
                 text += indent * '\t' + type_return(value, indent)
             text += (indent - 1) * '\t' + ']\n'
 
-    return text
+    return text if not compact else Compatible(text)
 
 
 def type_return(value, indent=0):
     text = ''
     if type(value) in (dict, list):
         text += dumps(value, indent)
     elif type(value) == str:
@@ -128,37 +137,42 @@
         text += 'true' if value else 'false'
         text += '\n'
     return text
 
 
 def dict_iterator(token):
     tdict = {}
+    key = ''
     while i := token.next():
-        if i.type == Token.KEY:
-            key = i.value
+        if i.type == Token.COLON:
             next_i = token.next()
             if next_i.type == Token.BEGIN_DICT:
                 tdict[key] = dict_iterator(token)
             elif next_i.type == Token.BEGIN_LIST:
                 tdict[key] = list_iterator(token)
-            elif next_i.type in (Token.BOOL, Token.STRING, Token.NUMBER):
+            elif next_i.type in (Token.BOOL, Token.STRING, Token.NUMBER, Token.STRING_IN_QUOTE):
                 tdict[key] = next_i.value
         elif i.type == Token.END_DICT:
             break
+        key = i.value
+        if key.startswith('$number$'):
+            key = key[8:]
+        if i.type == Token.STRING_IN_QUOTE:
+            key = f'"{key}"'
     return tdict
 
 
 def list_iterator(token):
     tlist = []
     while i := token.next():
         if i.type == Token.BEGIN_DICT:
             tlist.append(dict_iterator(token))
         elif i.type == Token.BEGIN_LIST:
             tlist.append(list_iterator(token))
-        elif i.type in (Token.BOOL, Token.STRING, Token.NUMBER, Token.INTEGER):
+        elif i.type in (Token.BOOL, Token.STRING, Token.NUMBER, Token.INTEGER, Token.STRING_IN_QUOTE):
             tlist.append(i.value)
         elif i.type == Token.END_LIST:
             break
     return tlist
 
 
 def snbt_to_token_list(t):
@@ -168,33 +182,31 @@
         token = TokenElement()
         if i == '{':
             token.type = Token.BEGIN_DICT
             token.value = '{'
         elif i == '[':
             token.type = Token.BEGIN_LIST
             token.value = '['
+        elif i == ':':
+            token.type = Token.COLON
+            token.value = ':'
         elif i in '-0123456789':
-            if reader.snext() == ':':
-                reader.last()
-                token = KeyBuilder(token, reader)
-            else:
-                reader.last()
-                token.type = Token.NUMBER
-                token.value = NumberBuilder(reader)
+            token.type = Token.NUMBER
+            token.value = NumberBuilder(reader)
         elif i == ']':
             token.type = Token.END_LIST
             token.value = ']'
         elif i == '}':
             token.type = Token.END_DICT
             token.value = '}'
         elif i in ',\n':
             token.type = Token.ENTER
             token.value = '\n'
         else:
-            token = KeyBuilder(token, reader)
+            token.value, token.type = StringBuilder(reader)
         token_list.append(token)
     return token_list
 
 
 def NumberBuilder(r):
     s = StringIO()
     s.write(r.get_point())
@@ -204,67 +216,37 @@
             break
         s.write(i)
     return '$number$' + s.getvalue()
 
 
 def StringBuilder(r):
     s = StringIO()
-    while i := r.snext():
-        if i == '\\':
-            s.write('\\')
-            s.write(r.snext())
-            continue
-        elif i == '"':
-            break
-        s.write(i)
-    return s.getvalue()
-
-
-def KeyBuilder(token, r):
-    s = ''
-    stringStatus = False
-    numberStatus = False
+    type = Token.STRING
     if r.get_point() == '"':
-        stringStatus = True
-    elif r.get_point() in '0123456789':
-        r.last()
-        numberStatus = True
-    else:
-        s += r.get_point()
-    token.type = Token.KEY
-    while i := r.snext():
-        if stringStatus:
+        type = Token.STRING_IN_QUOTE
+        while i := r.snext():
             if i == '\\':
-                s += '\\'
-                s += r.snext()
+                s.write('\\')
+                s.write(r.snext())
                 continue
             elif i == '"':
-                if r.snext() == ':':
-                    s = f'"{s}"'
-                    break
-                else:
-                    if not r.get_point().isspace() and not r.get_point() in ',]}':
-                        r.last()
-                        s += '\\'
-                        s += r.get_point()
-                        continue
-                    else:
-                        r.last()
-                        token.type = Token.STRING
-                        break
-        if numberStatus:
-            if i in '0123456789':
-                s += i
-            if r.snext() == ':':
                 break
-        if i == ':' and not stringStatus:
-            break
-        s += i
-        if s in ('true', 'false'):
-            token.type = Token.BOOL
-            s = True if s == 'true' else False
-            break
-        elif s == 'I;':
-            token.type = Token.INTEGER
-            break
-    token.value = s
-    return token
+            s.write(i)
+    else:
+        r.last()
+        while i := r.next():
+            if i in '},\n:[]' or i.isspace():
+                r.last()
+                break
+            s.write(i)
+    return s.getvalue(), type
+
+
+def Compatible(text):  # Thanks for XDawned
+    if not text:
+        return ''
+    else:
+        lines = text.splitlines()
+        for i in range(len(lines)-1):
+            if lines[i][-1] not in '[{' and lines[i+1].strip()[0] not in ']}':
+                lines[i] += ','
+        return '\n'.join(lines)
```

### Comparing `snbtlib-0.1.0/snbtlib.egg-info/PKG-INFO` & `snbtlib-1.0.0/snbtlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snbtlib
-Version: 0.1.0
+Version: 1.0.0
 Summary: a formatter for snbt from minecraft
 Home-page: 
 Author: Tryanks
 Author-email: tryanks@outlook.com
 License: MIT License
 Keywords: minecraft
 Platform: any
```

