# Comparing `tmp/asyncwhois-1.0.5.tar.gz` & `tmp/asyncwhois-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/josepho/Desktop/workspace-py/asyncwhois/dist/.tmp-ugh_mzo6/asyncwhois-1.0.5.tar", last modified: Wed Apr  5 14:16:31 2023, max compression
+gzip compressed data, was "/Users/josepho/Desktop/workspace-py/asyncwhois/dist/.tmp-7_y4nv7r/asyncwhois-1.0.6.tar", last modified: Fri Jun  2 17:46:45 2023, max compression
```

## Comparing `asyncwhois-1.0.5.tar` & `asyncwhois-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/
--rw-r--r--   0 josepho    (502) staff       (20)     1088 2022-01-20 03:14:56.000000 asyncwhois-1.0.5/LICENSE
--rw-r--r--   0 josepho    (502) staff       (20)       68 2022-01-20 03:14:56.000000 asyncwhois-1.0.5/MANIFEST.in
--rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/PKG-INFO
--rw-r--r--   0 josepho    (502) staff       (20)     6649 2023-03-01 02:03:52.000000 asyncwhois-1.0.5/README.md
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois/
--rw-r--r--   0 josepho    (502) staff       (20)     9039 2023-04-05 14:16:01.000000 asyncwhois-1.0.5/asyncwhois/__init__.py
--rw-r--r--   0 josepho    (502) staff       (20)      166 2023-02-20 17:06:00.000000 asyncwhois-1.0.5/asyncwhois/errors.py
--rw-r--r--   0 josepho    (502) staff       (20)    10440 2023-04-05 14:03:21.000000 asyncwhois-1.0.5/asyncwhois/parse.py
--rw-r--r--   0 josepho    (502) staff       (20)    14205 2023-02-20 17:06:00.000000 asyncwhois-1.0.5/asyncwhois/parse_rir.py
--rw-r--r--   0 josepho    (502) staff       (20)    66855 2023-04-05 14:03:21.000000 asyncwhois-1.0.5/asyncwhois/parse_tld.py
--rw-r--r--   0 josepho    (502) staff       (20)    11885 2023-03-01 02:03:52.000000 asyncwhois-1.0.5/asyncwhois/pywhois.py
--rw-r--r--   0 josepho    (502) staff       (20)     9394 2023-04-05 14:03:21.000000 asyncwhois-1.0.5/asyncwhois/query.py
--rw-r--r--   0 josepho    (502) staff       (20)    72921 2023-03-01 02:03:52.000000 asyncwhois-1.0.5/asyncwhois/servers.py
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/
--rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/PKG-INFO
--rw-r--r--   0 josepho    (502) staff       (20)      561 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/SOURCES.txt
--rw-r--r--   0 josepho    (502) staff       (20)        1 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/dependency_links.txt
--rw-r--r--   0 josepho    (502) staff       (20)       61 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/requires.txt
--rw-r--r--   0 josepho    (502) staff       (20)       11 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/asyncwhois.egg-info/top_level.txt
--rw-r--r--   0 josepho    (502) staff       (20)      239 2022-01-20 03:14:56.000000 asyncwhois-1.0.5/pyproject.toml
--rw-r--r--   0 josepho    (502) staff       (20)     1017 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/setup.cfg
--rw-r--r--   0 josepho    (502) staff       (20)     1787 2023-03-03 02:48:10.000000 asyncwhois-1.0.5/setup.py
-drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-04-05 14:16:31.000000 asyncwhois-1.0.5/tests/
--rw-r--r--   0 josepho    (502) staff       (20)      609 2023-02-20 17:06:00.000000 asyncwhois-1.0.5/tests/test_not_found.py
--rw-r--r--   0 josepho    (502) staff       (20)     2610 2023-02-28 22:25:51.000000 asyncwhois-1.0.5/tests/test_package_methods.py
--rw-r--r--   0 josepho    (502) staff       (20)     1668 2022-04-26 19:29:46.000000 asyncwhois-1.0.5/tests/test_parser_methods.py
--rw-r--r--   0 josepho    (502) staff       (20)    60537 2023-04-05 14:03:21.000000 asyncwhois-1.0.5/tests/test_parser_output.py
--rw-r--r--   0 josepho    (502) staff       (20)     1261 2023-02-20 17:06:00.000000 asyncwhois-1.0.5/tests/test_pywhois.py
--rw-r--r--   0 josepho    (502) staff       (20)     1309 2022-04-26 20:37:44.000000 asyncwhois-1.0.5/tests/test_query.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/
+-rw-r--r--   0 josepho    (502) staff       (20)     1088 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/LICENSE
+-rw-r--r--   0 josepho    (502) staff       (20)       68 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/MANIFEST.in
+-rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/PKG-INFO
+-rw-r--r--   0 josepho    (502) staff       (20)     6649 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/README.md
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois/
+-rw-r--r--   0 josepho    (502) staff       (20)     9039 2023-06-02 17:46:32.000000 asyncwhois-1.0.6/asyncwhois/__init__.py
+-rw-r--r--   0 josepho    (502) staff       (20)      166 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/asyncwhois/errors.py
+-rw-r--r--   0 josepho    (502) staff       (20)    10440 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/asyncwhois/parse.py
+-rw-r--r--   0 josepho    (502) staff       (20)    14205 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/asyncwhois/parse_rir.py
+-rw-r--r--   0 josepho    (502) staff       (20)    66855 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/asyncwhois/parse_tld.py
+-rw-r--r--   0 josepho    (502) staff       (20)    11885 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/asyncwhois/pywhois.py
+-rw-r--r--   0 josepho    (502) staff       (20)     9906 2023-06-02 17:46:32.000000 asyncwhois-1.0.6/asyncwhois/query.py
+-rw-r--r--   0 josepho    (502) staff       (20)    72921 2023-03-01 02:03:52.000000 asyncwhois-1.0.6/asyncwhois/servers.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/
+-rw-r--r--   0 josepho    (502) staff       (20)     7732 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/PKG-INFO
+-rw-r--r--   0 josepho    (502) staff       (20)      561 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/SOURCES.txt
+-rw-r--r--   0 josepho    (502) staff       (20)        1 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/dependency_links.txt
+-rw-r--r--   0 josepho    (502) staff       (20)       61 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/requires.txt
+-rw-r--r--   0 josepho    (502) staff       (20)       11 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/asyncwhois.egg-info/top_level.txt
+-rw-r--r--   0 josepho    (502) staff       (20)      239 2022-01-20 03:14:56.000000 asyncwhois-1.0.6/pyproject.toml
+-rw-r--r--   0 josepho    (502) staff       (20)     1017 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/setup.cfg
+-rw-r--r--   0 josepho    (502) staff       (20)     1787 2023-03-03 02:48:10.000000 asyncwhois-1.0.6/setup.py
+drwxr-xr-x   0 josepho    (502) staff       (20)        0 2023-06-02 17:46:45.000000 asyncwhois-1.0.6/tests/
+-rw-r--r--   0 josepho    (502) staff       (20)      609 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/tests/test_not_found.py
+-rw-r--r--   0 josepho    (502) staff       (20)     2610 2023-02-28 22:25:51.000000 asyncwhois-1.0.6/tests/test_package_methods.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1668 2022-04-26 19:29:46.000000 asyncwhois-1.0.6/tests/test_parser_methods.py
+-rw-r--r--   0 josepho    (502) staff       (20)    60537 2023-04-05 14:03:21.000000 asyncwhois-1.0.6/tests/test_parser_output.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1261 2023-02-20 17:06:00.000000 asyncwhois-1.0.6/tests/test_pywhois.py
+-rw-r--r--   0 josepho    (502) staff       (20)     1309 2022-04-26 20:37:44.000000 asyncwhois-1.0.6/tests/test_query.py
```

### Comparing `asyncwhois-1.0.5/LICENSE` & `asyncwhois-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/PKG-INFO` & `asyncwhois-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.0.5
+Version: 1.0.6
 Summary: asyncio-friendly Python module for WHOIS and RDAP queries.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.0.5/README.md` & `asyncwhois-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois/__init__.py` & `asyncwhois-1.0.6/asyncwhois/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "rdap_ipv4",
     "rdap_ipv6",
     "rdap_asn",
     "whois_domain",
     "whois_ipv4",
     "whois_ipv6",
 ]
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 
 def whois_domain(
     domain: str,
     authoritative_only: bool = False,
     proxy_url: str = None,
     timeout: int = 10,
```

### Comparing `asyncwhois-1.0.5/asyncwhois/parse.py` & `asyncwhois-1.0.6/asyncwhois/parse.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois/parse_rir.py` & `asyncwhois-1.0.6/asyncwhois/parse_rir.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois/parse_tld.py` & `asyncwhois-1.0.6/asyncwhois/parse_tld.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois/pywhois.py` & `asyncwhois-1.0.6/asyncwhois/pywhois.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois/query.py` & `asyncwhois-1.0.6/asyncwhois/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -140,17 +140,21 @@
                 # concatenate query outputs
                 self.query_chain += query_output
             # parse response for the referred WHOIS server name
             whois_server = self._find_match(regex, query_output)
             whois_server = whois_server.lower()
             if whois_server and whois_server != server:
                 # recursive call to find more authoritative server
-                query_output = self._do_query(
+                authoritative_output = self._do_query(
                     whois_server, data, self.whois_server_regex
                 )
+                # check for empty responses; only update query_output if
+                # there was a complete response from the authoritative server
+                if authoritative_output:
+                    query_output = authoritative_output
         # return the WHOIS query output
         return query_output
 
     async def _aio_do_query(self, server: str, data: str, regex: str):
         # connect to whois://<server>:43
         async with self._aio_create_connection(
             (server, self.whois_port), self.proxy_url
@@ -163,17 +167,21 @@
                 # concatenate query outputs
                 self.query_chain += query_output
             # parse response for the referred WHOIS server name
             whois_server = self._find_match(regex, query_output)
             whois_server = whois_server.lower()
             if whois_server and whois_server != server:
                 # recursive call to find the authoritative server
-                query_output = await self._aio_do_query(
+                authoritative_output = await self._aio_do_query(
                     whois_server, data, self.whois_server_regex
                 )
+                # check for empty responses; only update query_output if
+                # there was a complete response from the authoritative server
+                if authoritative_output:
+                    query_output = authoritative_output
         # return the WHOIS query output
         return query_output
 
 
 class DomainQuery(Query):
     def __init__(
         self,
```

### Comparing `asyncwhois-1.0.5/asyncwhois/servers.py` & `asyncwhois-1.0.6/asyncwhois/servers.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/asyncwhois.egg-info/PKG-INFO` & `asyncwhois-1.0.6/asyncwhois.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncwhois
-Version: 1.0.5
+Version: 1.0.6
 Summary: asyncio-friendly Python module for WHOIS and RDAP queries.
 Home-page: https://github.com/pogzyb/asyncwhois
 Author: Joseph Obarzanek
 Author-email: pogzyb@umich.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pogzyb/asyncwhois/issues
 Classifier: Environment :: Web Environment
```

### Comparing `asyncwhois-1.0.5/asyncwhois.egg-info/SOURCES.txt` & `asyncwhois-1.0.6/asyncwhois.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/setup.cfg` & `asyncwhois-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/setup.py` & `asyncwhois-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_not_found.py` & `asyncwhois-1.0.6/tests/test_not_found.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_package_methods.py` & `asyncwhois-1.0.6/tests/test_package_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_parser_methods.py` & `asyncwhois-1.0.6/tests/test_parser_methods.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_parser_output.py` & `asyncwhois-1.0.6/tests/test_parser_output.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_pywhois.py` & `asyncwhois-1.0.6/tests/test_pywhois.py`

 * *Files identical despite different names*

### Comparing `asyncwhois-1.0.5/tests/test_query.py` & `asyncwhois-1.0.6/tests/test_query.py`

 * *Files identical despite different names*

