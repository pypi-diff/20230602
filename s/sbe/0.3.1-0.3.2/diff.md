# Comparing `tmp/sbe-0.3.1.tar.gz` & `tmp/sbe-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbe-0.3.1.tar", last modified: Sun Nov 13 07:16:59 2022, max compression
+gzip compressed data, was "sbe-0.3.2.tar", last modified: Fri Jun  2 06:05:35 2023, max compression
```

## Comparing `sbe-0.3.1.tar` & `sbe-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2022-11-13 07:16:59.113420 sbe-0.3.1/
--rw-r--r--   0 chris      (501) staff       (20)     1121 2022-05-06 07:17:57.000000 sbe-0.3.1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     2694 2022-11-13 07:16:59.113242 sbe-0.3.1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2486 2022-05-06 07:17:57.000000 sbe-0.3.1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2022-11-13 07:16:59.111744 sbe-0.3.1/sbe/
--rw-r--r--   0 chris      (501) staff       (20)    37273 2022-11-13 07:13:35.000000 sbe-0.3.1/sbe/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2022-11-13 07:16:59.112904 sbe-0.3.1/sbe.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2694 2022-11-13 07:16:59.000000 sbe-0.3.1/sbe.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      176 2022-11-13 07:16:59.000000 sbe-0.3.1/sbe.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2022-11-13 07:16:59.000000 sbe-0.3.1/sbe.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       15 2022-11-13 07:16:59.000000 sbe-0.3.1/sbe.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)        4 2022-11-13 07:16:59.000000 sbe-0.3.1/sbe.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2022-11-13 07:16:59.113461 sbe-0.3.1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)      405 2022-11-13 07:13:51.000000 sbe-0.3.1/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-02 06:05:35.051496 sbe-0.3.2/
+-rw-r--r--   0 chris      (501) staff       (20)     1121 2022-05-06 07:17:57.000000 sbe-0.3.2/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     2694 2023-06-02 06:05:35.051366 sbe-0.3.2/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2486 2022-05-06 07:17:57.000000 sbe-0.3.2/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-02 06:05:35.050074 sbe-0.3.2/sbe/
+-rw-r--r--   0 chris      (501) staff       (20)    37240 2023-06-02 06:03:23.000000 sbe-0.3.2/sbe/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-06-02 06:05:35.051161 sbe-0.3.2/sbe.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     2694 2023-06-02 06:05:35.000000 sbe-0.3.2/sbe.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      176 2023-06-02 06:05:35.000000 sbe-0.3.2/sbe.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2023-06-02 06:05:35.000000 sbe-0.3.2/sbe.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)       15 2023-06-02 06:05:35.000000 sbe-0.3.2/sbe.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)        4 2023-06-02 06:05:35.000000 sbe-0.3.2/sbe.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2023-06-02 06:05:35.051545 sbe-0.3.2/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)      405 2023-06-02 06:04:22.000000 sbe-0.3.2/setup.py
```

### Comparing `sbe-0.3.1/LICENSE` & `sbe-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbe-0.3.1/PKG-INFO` & `sbe-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbe
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/kizzx2/sbe-python
 Author: Chris Yuen
 Author-email: chris@kizzx2.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sbe-python
```

### Comparing `sbe-0.3.1/README.md` & `sbe-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `sbe-0.3.1/sbe/__init__.py` & `sbe-0.3.2/sbe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,14 @@
 
         m = self.messages[header.value['templateId']]
 
         cursor = Cursor(0)
         format_str_parts = []
         for f in m.fields:
             if isinstance(f, Group):
-                assert cursor.val >= header.value['blockLength']
                 if cursor.val < header.value['blockLength']:
                     format_str_parts.append(str(header.value['blockLength'] - cursor.val) + 'x')
                     cursor.val = header.value['blockLength']
             part = _unpack_format(self, f, '', buffer[body_offset:], cursor)
             if part:
                 format_str_parts.append(part)
         format_str = '<' + ''.join(format_str_parts)
@@ -672,15 +671,15 @@
     schema: Schema, composite: Composite,
     obj: dict, fmt: list, vals: list, cursor: Cursor
 ):
     for t in composite.types:
         if isinstance(t, Composite):
             _walk_fields_encode_composite(schema, t, obj[t.name], fmt, vals, cursor)
 
-        else:
+        elif t.presence != Presence.CONSTANT:
             t1 = t.primitiveType
             if t1 == PrimitiveType.CHAR:
                 if t.length > 1:
                     fmt.append(str(t.length) + "s")
                     vals.append(obj[t.name].encode())
                     cursor.val += t.length
             else:
```

### Comparing `sbe-0.3.1/sbe.egg-info/PKG-INFO` & `sbe-0.3.2/sbe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbe
-Version: 0.3.1
+Version: 0.3.2
 Home-page: https://github.com/kizzx2/sbe-python
 Author: Chris Yuen
 Author-email: chris@kizzx2.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sbe-python
```

