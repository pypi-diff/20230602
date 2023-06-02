# Comparing `tmp/dart-tools-0.3.0.tar.gz` & `tmp/dart-tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.0.tar", last modified: Tue May 23 22:12:46 2023, max compression
+gzip compressed data, was "dart-tools-0.3.1.tar", last modified: Fri Jun  2 19:23:08 2023, max compression
```

## Comparing `dart-tools-0.3.0.tar` & `dart-tools-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.047203 dart-tools-0.3.0/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.0/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-23 22:12:46.046810 dart-tools-0.3.0/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.0/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.042158 dart-tools-0.3.0/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.0/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    11987 2023-05-23 22:10:51.000000 dart-tools-0.3.0/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.0/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-05-23 22:12:46.045940 dart-tools-0.3.0/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-05-23 22:12:45.000000 dart-tools-0.3.0/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-05-23 22:01:53.000000 dart-tools-0.3.0/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-05-23 22:12:46.047360 dart-tools-0.3.0/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.315989 dart-tools-0.3.1/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.1/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:23:08.315562 dart-tools-0.3.1/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.1/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.311247 dart-tools-0.3.1/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.1/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    12882 2023-06-02 19:22:02.000000 dart-tools-0.3.1/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.1/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.315029 dart-tools-0.3.1/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-02 19:22:02.000000 dart-tools-0.3.1/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-02 19:23:08.316203 dart-tools-0.3.1/setup.cfg
```

### Comparing `dart-tools-0.3.0/LICENSE` & `dart-tools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.0/PKG-INFO` & `dart-tools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.0 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.1 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.0/README.md` & `dart-tools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.0/dart/dart.py` & `dart-tools-0.3.1/dart/dart.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 _CLIENT_DUID_KEY = "clientDuid"
 _HOST_KEY = "host"
 _HOSTS_KEY = "hosts"
 _CSRF_TOKEN_KEY = "csrfToken"
 _SESSION_ID_KEY = "sessionId"
 
 _DUID_CHARS = string.ascii_lowercase + string.ascii_uppercase + string.digits + "-_"
+_PRIORITY_MAP = {0: "Critical", 1: "High", 2: "Medium", 3: "Low"}
+_SIZES = {1, 2, 3, 5, 8}
 _COMPLETED_STATUS_KINDS = {"Finished", "Canceled"}
 _DEFAULT_DESCRIPTION = {
     "root": {
         "direction": None,
         "format": "",
         "indent": 0,
         "type": "root",
@@ -276,71 +278,80 @@
     _check_response_and_maybe_exit(response)
     res = response.json()
     if not res["isLoggedIn"]:
         _print_login_failure_message_and_exit()
     return res
 
 
-def begin_task():
+def _begin_task(config, session, user_email, get_task):
     _Git.ensure_no_unstaged_changes()
     _Git.ensure_on_main_or_intended()
 
+    task = get_task()
+
+    response = session.post(_COPY_BRANCH_URL_FRAG, json={"duid": task["duid"]})
+    _check_response_and_maybe_exit(response)
+
+    branch_name = _Git.make_task_name(user_email, task)
+    _Git.checkout_branch(branch_name)
+
+    print(
+        f"Started work on [{task['title']}]({_get_task_url(config.host, task['duid'])}) on branch {branch_name}"
+    )
+
+
+def begin_task():
     config = _Config()
     session = _Session(config)
 
     user_bundle = _get_full_user_bundle(session)
-
     user = user_bundle["user"]
-    user_duid = user["duid"]
-    active_duid = next(
-        e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
-    )
-    unterm_status_duids = {
-        e["duid"]
-        for e in user_bundle["statuses"]
-        if e["kind"] not in _COMPLETED_STATUS_KINDS
-    }
-    filtered_tasks = [
-        e
-        for e in user_bundle["tasks"]
-        if not e["inTrash"]
-        and e["dartboardDuid"] == active_duid
-        and user_duid in e["assigneeDuids"]
-        and e["statusDuid"] in unterm_status_duids
-        and e["drafterDuid"] is None
-    ]
-    filtered_tasks.sort(key=lambda e: e["order"])
-
-    chosen_task = filtered_tasks[
-        pick(
-            [e["title"] for e in filtered_tasks],
-            "Which of your active, unfinalized tasks are you beginning work on?",
-            "→",
-        )[1]
-    ]
 
-    response = session.post(_COPY_BRANCH_URL_FRAG, json={"duid": chosen_task["duid"]})
-    _check_response_and_maybe_exit(response)
+    def _get_task():
+        user_duid = user["duid"]
+        active_duid = next(
+            e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
+        )
+        unterm_status_duids = {
+            e["duid"]
+            for e in user_bundle["statuses"]
+            if e["kind"] not in _COMPLETED_STATUS_KINDS
+        }
+        filtered_tasks = [
+            e
+            for e in user_bundle["tasks"]
+            if not e["inTrash"]
+            and e["dartboardDuid"] == active_duid
+            and user_duid in e["assigneeDuids"]
+            and e["statusDuid"] in unterm_status_duids
+            and e["drafterDuid"] is None
+        ]
+        filtered_tasks.sort(key=lambda e: e["order"])
 
-    branch_name = _Git.make_task_name(user["email"], chosen_task)
-    _Git.checkout_branch(branch_name)
+        return filtered_tasks[
+            pick(
+                [e["title"] for e in filtered_tasks],
+                "Which of your active, unfinalized tasks are you beginning work on?",
+                "→",
+            )[1]
+        ]
+
+    _begin_task(config, session, user["email"], _get_task)
 
-    print(
-        f"Started work on [{chosen_task['title']}]({_get_task_url(config.host, chosen_task['duid'])}) on branch {branch_name}"
-    )
     print("Done.")
 
 
-def create_task(title):
+def create_task(title, should_begin, priority_int, size):
     config = _Config()
     session = _Session(config)
 
     user_bundle = _get_full_user_bundle(session)
 
-    user_duid = user_bundle["user"]["duid"]
+    user = user_bundle["user"]
+    user_duid = user["duid"]
     active_duid = next(
         e["duid"] for e in user_bundle["dartboards"] if e["kind"] == "Active"
     )
     first_order = min(
         e["order"] for e in user_bundle["tasks"] if e["dartboardDuid"] == active_duid
     )
     order = get_orders_between(None, first_order, 1)[0]
@@ -357,22 +368,26 @@
         "order": order,
         "title": title,
         "description": _DEFAULT_DESCRIPTION,
         "statusDuid": status_duid,
         "assigneeDuids": [user_duid],
         "subscriberDuids": [user_duid],
         "tagDuids": [],
-        "priority": None,
-        "size": None,
+        "priority": _PRIORITY_MAP[priority_int],
+        "size": size,
         "dueAt": None,
     }
     response = session.post(_CREATE_TASK_URL_FRAG, json={"item": task})
     _check_response_and_maybe_exit(response)
 
     print(f"Created task [{task['title']}]({_get_task_url(config.host, task['duid'])})")
+
+    if should_begin:
+        _begin_task(config, session, user["email"], lambda: task)
+
     print("Done.")
 
 
 def cli():
     if _VERSION_CMD in sys.argv:
         print_version()
         sys.exit(0)
@@ -385,21 +400,36 @@
         required=True,
         metavar=f"{{{_LOGIN_CMD},{_CREATE_TASK_CMD},{_BEGIN_TASK_CMD}}}",
     )
 
     set_host_parser = subparsers.add_parser(_SET_HOST_CMD, aliases="s")
     set_host_parser.add_argument("host", help="the new host: {prod|dev|[URL]}")
     set_host_parser.set_defaults(func=set_host)
+
     login_parser = subparsers.add_parser(_LOGIN_CMD, aliases="l", help="login")
     login_parser.set_defaults(func=login)
+
     create_task_parser = subparsers.add_parser(
         _CREATE_TASK_CMD, aliases="c", help="create a new task"
     )
     create_task_parser.add_argument("title", help="the title of the task")
+    create_task_parser.add_argument(
+        "-b",
+        dest="should_begin",
+        action="store_true",
+        help="begin work on the task after creation",
+    )
+    create_task_parser.add_argument(
+        "-p", dest="priority_int", type=int, choices=_PRIORITY_MAP.keys(), help="priority"
+    )
+    create_task_parser.add_argument(
+        "-i", dest="size", type=int, choices=_SIZES, help="size"
+    )
     create_task_parser.set_defaults(func=create_task)
+
     begin_task_parser = subparsers.add_parser(
         _BEGIN_TASK_CMD, aliases="b", help="begin work on a task"
     )
     begin_task_parser.set_defaults(func=begin_task)
 
     args = vars(parser.parse_args())
     func = args.pop("func")
```

### Comparing `dart-tools-0.3.0/dart/order_manager.py` & `dart-tools-0.3.1/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.0/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.1/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.0
+Version: 0.3.1
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.0 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.1 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.0/pyproject.toml` & `dart-tools-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.0"
+version = "0.3.1"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

