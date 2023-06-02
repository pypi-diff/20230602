# Comparing `tmp/CustomXMLParser-1.0.5.tar.gz` & `tmp/CustomXMLParser-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CustomXMLParser-1.0.5.tar", last modified: Tue Mar 28 01:53:39 2023, max compression
+gzip compressed data, was "dist\CustomXMLParser-1.0.6.tar", last modified: Fri Jun  2 03:47:07 2023, max compression
```

## Comparing `CustomXMLParser-1.0.5.tar` & `CustomXMLParser-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser/
--rw-rw-rw-   0        0        0     5494 2023-02-22 04:53:37.000000 CustomXMLParser-1.0.5/CustomXMLParser/README.py
--rw-rw-rw-   0        0        0      130 2023-02-22 04:30:06.000000 CustomXMLParser-1.0.5/CustomXMLParser/__init__.py
--rw-rw-rw-   0        0        0    11998 2023-03-28 01:31:58.000000 CustomXMLParser-1.0.5/CustomXMLParser/main.py
--rw-rw-rw-   0        0        0     1678 2023-03-28 01:46:38.000000 CustomXMLParser-1.0.5/CustomXMLParser/version.py
-drwxrwxrwx   0        0        0        0 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/
--rw-rw-rw-   0        0        0     7380 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/CustomXMLParser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7380 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5497 2023-03-02 04:47:20.000000 CustomXMLParser-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-03-28 01:53:39.000000 CustomXMLParser-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1555 2023-02-22 05:10:17.000000 CustomXMLParser-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 03:47:07.000000 CustomXMLParser-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-02 03:47:07.000000 CustomXMLParser-1.0.6/CustomXMLParser/
+-rw-rw-rw-   0        0        0     5494 2023-02-22 04:53:37.000000 CustomXMLParser-1.0.6/CustomXMLParser/README.py
+-rw-rw-rw-   0        0        0      130 2023-02-22 04:30:06.000000 CustomXMLParser-1.0.6/CustomXMLParser/__init__.py
+-rw-rw-rw-   0        0        0    12046 2023-06-02 03:46:32.000000 CustomXMLParser-1.0.6/CustomXMLParser/main.py
+-rw-rw-rw-   0        0        0     1678 2023-06-02 03:46:46.000000 CustomXMLParser-1.0.6/CustomXMLParser/version.py
+drwxrwxrwx   0        0        0        0 2023-06-02 03:47:07.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/
+-rw-rw-rw-   0        0        0     7380 2023-06-02 03:47:06.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-06-02 03:47:06.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 03:47:06.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-02 03:47:06.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-02 03:47:06.000000 CustomXMLParser-1.0.6/CustomXMLParser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7380 2023-06-02 03:47:07.000000 CustomXMLParser-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5497 2023-03-02 04:47:20.000000 CustomXMLParser-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 03:47:07.000000 CustomXMLParser-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1555 2023-02-22 05:10:17.000000 CustomXMLParser-1.0.6/setup.py
```

### Comparing `CustomXMLParser-1.0.5/CustomXMLParser/README.py` & `CustomXMLParser-1.0.6/CustomXMLParser/README.py`

 * *Files identical despite different names*

### Comparing `CustomXMLParser-1.0.5/CustomXMLParser/main.py` & `CustomXMLParser-1.0.6/CustomXMLParser/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             if in_d.get(self.data_key) and in_d.get(self.header_key) and in_d.get(self.header_key, {}).get(self.table_key):
                 rows = [row.split(',') for row in in_d.get(self.data_key, '').split('\n')]
                 rows = list(zip(*rows))
                 raw_header: List[Dict] = in_d.get(self.header_key, {}).get(self.table_key, [])
                 missing_element = self.data_key if len(rows) < len(raw_header) else self.header_key
                 if len(rows) != len(raw_header):
                     if self.verbose:
-                        print(f"Header and rows for [{element_name}] do not match. [{missing_element}] is incomplete.", 'red')
+                        print(f"Header and rows for [{element_name}] do not match. [{missing_element}] is incomplete.", color='red')
                 else:
                     for i, _dict in enumerate(raw_header):
                         out_d[element_name][_dict.get(self.header_text_key)] = rows[i]
         else:
             for key, value in in_d.items():  # recurse the dict...
                 if isinstance(value, dict):
                     if self.name_key in in_d:
@@ -172,30 +172,30 @@
                 _children = parents.get(key, {})
                 for path in value:
                     if "*" in path: # Do wild-card (list) lookup...
                         keys = path.split(',')
                         formatted_key, root_key, tmp_payLoad = format_key(keys, True, payload)
                         if not formatted_key and not root_key:
                             if self.verbose:
-                                print(f"Key [{key}] resource {value} is not available.", 'orange')
+                                print(f"Key [{key}] resource {value} is not available.", color='orange')
                             continue # this means resource is not avaiable
                         if tmp_payLoad.get(root_key):
                             try:
                                 out_d[key] = eval(f'tmp_payLoad{formatted_key}')
                             except KeyError:
                                 pass # this means resource is not available...
                         else:
                             # This means it's wild card list...
                             for k, v in tmp_payLoad.items():
                                 out_d[key][k] = {}
                                 try:
                                     out_d[key][k].update(eval(f'v["{root_key}"]{formatted_key}'))
                                 except KeyError:
                                     if self.verbose:
-                                        print(f"Resource {formatted_key} is not available.", 'orange')
+                                        print(f"Resource {formatted_key} is not available.", color='orange')
                                     pass # it means resource is not available...
                                 if _children:
                                     for child in _children:
                                         out_d[key][k].update(summarize({child: config.get(child, [])}, _children, v, {}))
                     else:
                         # Do direct lookup...
                         keys = path.split(',')
@@ -209,27 +209,27 @@
 
     def parse(self, file: str) -> Dict:
         parsed_content = {}
         st = time.perf_counter()
         if self.parser_type == 'raw':
             parsed_content = self._load_file(file)
             if self.verbose:
-                print(f'Raw xml2dict parsing.', 'green')
+                print(f'Raw xml2dict parsing.', color='green')
         else:
             unformatted_dict = self._xml_to_dict(self._load_file(file), {})
             if not self.config_file:
                 parsed_content =  unformatted_dict
                 if self.verbose:
-                    print(f'Unformatted custom parsing.', 'green')
+                    print(f'Unformatted custom parsing.', color='green')
             else:
                 if not self._config:
                     self._config = self._load_file(self.config_file, 'utf-8', 'json')
                 parsed_content = self._format_dict(unformatted_dict[next(iter(unformatted_dict))])
                 if self.verbose:
-                    print(f'Formatted custom parsing.', 'green')
+                    print(f'Formatted custom parsing.', color='green')
             if self.verbose:
-                [print(f'"{key}" table is empty.', 'orange') for key, value in parsed_content.items() if not value]
+                [print(f'"{key}" table is empty.', color='orange') for key, value in parsed_content.items() if not value]
         if self.verbose:
-            print(f'Parsing time: {time.perf_counter() - st:0.2f}s', 'green', attr=['b'])
+            print(f'Parsing time: {time.perf_counter() - st:0.2f}s', color='green', attr=['b'])
         return parsed_content
 
 XmlParser.__doc__ = LONG_DESCRIPTION
```

### Comparing `CustomXMLParser-1.0.5/CustomXMLParser/version.py` & `CustomXMLParser-1.0.6/CustomXMLParser/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 __author__ = "Muhammad Hamdan <mhamdan.dev@gmail.com>"
 __copyright__ = """
 BSD 3-Clause License
 
 Copyright (c) 2023, Muhammad Hamdan, and Intel Corporation
 All rights reserved.
```

### Comparing `CustomXMLParser-1.0.5/CustomXMLParser.egg-info/PKG-INFO` & `CustomXMLParser-1.0.6/CustomXMLParser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomXMLParser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Libary that allows for customized parsing of XML files using a set of configurations. Output is a dictonary. This library builds on the xml2dict library.
 Home-page: https://github.com/mhamdan91/CustomXMLParser
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Custom XML to Dict Parser
         ==============================
```

### Comparing `CustomXMLParser-1.0.5/PKG-INFO` & `CustomXMLParser-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CustomXMLParser
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python Libary that allows for customized parsing of XML files using a set of configurations. Output is a dictonary. This library builds on the xml2dict library.
 Home-page: https://github.com/mhamdan91/CustomXMLParser
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Custom XML to Dict Parser
         ==============================
```

### Comparing `CustomXMLParser-1.0.5/README.md` & `CustomXMLParser-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `CustomXMLParser-1.0.5/setup.py` & `CustomXMLParser-1.0.6/setup.py`

 * *Files identical despite different names*

