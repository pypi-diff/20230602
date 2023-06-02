# Comparing `tmp/jaaql-monitor-1.2.63.tar.gz` & `tmp/jaaql-monitor-1.2.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.63.tar", last modified: Thu Jun  1 08:52:39 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.64.tar", last modified: Fri Jun  2 01:45:35 2023, max compression
```

## Comparing `jaaql-monitor-1.2.63.tar` & `jaaql-monitor-1.2.64.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:52:39.230172 jaaql-monitor-1.2.63/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.63/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-06-01 08:52:39.230172 jaaql-monitor-1.2.63/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.63/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 08:52:39.227174 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-06-01 08:52:39.000000 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-01 08:52:39.000000 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:52:39.000000 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-01 08:52:39.000000 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 08:52:39.000000 jaaql-monitor-1.2.63/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-01 08:52:39.229175 jaaql-monitor-1.2.63/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.63/monitor/__init__.py
--rw-rw-rw-   0        0        0    28230 2023-06-01 08:52:06.000000 jaaql-monitor-1.2.63/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-01 08:52:27.000000 jaaql-monitor-1.2.63/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-01 08:52:39.230172 jaaql-monitor-1.2.63/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.63/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/
+-rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.64/LICENSE.txt
+-rw-rw-rw-   0        0        0     1475 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.64/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.127843 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1475 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.130842 jaaql-monitor-1.2.64/monitor/
+-rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.64/monitor/__init__.py
+-rw-rw-rw-   0        0        0    29060 2023-06-02 01:44:22.000000 jaaql-monitor-1.2.64/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-02 01:45:21.000000 jaaql-monitor-1.2.64/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.64/setup.py
```

### Comparing `jaaql-monitor-1.2.63/LICENSE.txt` & `jaaql-monitor-1.2.64/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.63/PKG-INFO` & `jaaql-monitor-1.2.64/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.63
+Version: 1.2.64
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.63/README.md` & `jaaql-monitor-1.2.64/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.63/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.64/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.63
+Version: 1.2.64
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-monitor-1.2.63/monitor/main.py` & `jaaql-monitor-1.2.64/monitor/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 MARKER__jaaql_bypass = "jaaql_bypass "
 
 ENDPOINT__oauth = "/oauth/token"
 ENDPOINT__submit = "/submit"
 ENDPOINT__attach = "/accounts"
 ENDPOINT__dispatchers = "/internal/dispatchers"
 ENDPOINT__wipe = "/internal/clean"
+ENDPOINT__freeze = "/internal/freeze"
+ENDPOINT__defrost = "/internal/defrost"
 
 COMMAND__initialiser = "\\"
 COMMAND__reset_short = "\\r"
 COMMAND__reset = "\\reset"
 COMMAND__go_short = "\g"
 COMMAND__go = "\go"
 COMMAND__print_short = "\p"
@@ -30,14 +32,16 @@
 COMMAND__wipe_dbms = "\wipe dbms"
 COMMAND__switch_jaaql_account_to = "\switch jaaql account to "
 COMMAND__connect_to_database = "\connect to database "
 COMMAND__register_jaaql_account_with = "\\register jaaql account with "
 COMMAND__attach_email_account = "\\attach email account "
 COMMAND__quit_short = "\q"
 COMMAND__quit = "\quit"
+COMMAND__freeze_instance = "\\freeze instance"
+COMMAND__defrost_instance = "\defrost instance"
 
 CONNECT_FOR_CREATEDB = " for createdb"
 
 DEFAULT_CONNECTION = "default"
 DEFAULT_EMAIL_ACCOUNT = "default"
 
 LINE_LENGTH_MAX = 115
@@ -387,14 +391,23 @@
     get_message(state, err, line_offset, print_buffer)
 
 
 def print_error(state, err, line_offset: int = 0):
     get_message(state, err, line_offset, dump_buffer(state, ""))
 
 
+def freeze_defrost_instance(state: State, freeze: bool):
+    endpoint = ENDPOINT__freeze if freeze else ENDPOINT__defrost
+    verb = "freezing" if freeze else "defrosting"
+    res = state.request_handler(METHOD__post, endpoint, handle_error=False)
+
+    if res.status_code != 200:
+        print_error(state, "Error " + verb + " jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
+
+
 def wipe_jaaql_box(state: State):
     res = state.request_handler(METHOD__post, ENDPOINT__wipe, handle_error=False)
 
     if res.status_code != 200:
         print_error(state, "Error wiping jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
 
 
@@ -489,14 +502,18 @@
             fetched_line = fetched_line.strip()  # Ignore the line terminator e.g. \r\n
             if fetched_line == COMMAND__go or fetched_line == COMMAND__go_short:
                 on_go(state)
             elif fetched_line == COMMAND__reset or fetched_line == COMMAND__reset_short:
                 state.fetched_query = ""
             elif fetched_line == COMMAND__print or fetched_line == COMMAND__print_short:
                 dump_buffer(state)
+            elif fetched_line == COMMAND__freeze_instance:
+                freeze_defrost_instance(state, freeze=True)
+            elif fetched_line == COMMAND__defrost_instance:
+                freeze_defrost_instance(state, freeze=False)
             elif len(state.fetched_query.strip()) != 0:
                 print_error(state, "Tried to execute the command '" + fetched_line + "' but buffer was non empty.")
             elif fetched_line == COMMAND__wipe_dbms:
                 wipe_jaaql_box(state)
             elif fetched_line.startswith(COMMAND__switch_jaaql_account_to):
                 candidate_connection_name = fetched_line.split(COMMAND__switch_jaaql_account_to)[1]
                 connection_name = parse_user_printing_any_errors(state, candidate_connection_name)
```

### Comparing `jaaql-monitor-1.2.63/setup.py` & `jaaql-monitor-1.2.64/setup.py`

 * *Files identical despite different names*

