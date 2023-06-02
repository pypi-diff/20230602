# Comparing `tmp/dart-tools-0.3.1.tar.gz` & `tmp/dart-tools-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.3.1.tar", last modified: Fri Jun  2 19:23:08 2023, max compression
+gzip compressed data, was "dart-tools-0.3.2.tar", last modified: Fri Jun  2 19:36:14 2023, max compression
```

## Comparing `dart-tools-0.3.1.tar` & `dart-tools-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.315989 dart-tools-0.3.1/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.1/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:23:08.315562 dart-tools-0.3.1/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.1/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.311247 dart-tools-0.3.1/dart/
--rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.1/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    12882 2023-06-02 19:22:02.000000 dart-tools-0.3.1/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.1/dart/order_manager.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:23:08.315029 dart-tools-0.3.1/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/dependency_links.txt
--rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-02 19:23:08.000000 dart-tools-0.3.1/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-02 19:22:02.000000 dart-tools-0.3.1/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-02 19:23:08.316203 dart-tools-0.3.1/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.269804 dart-tools-0.3.2/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.3.2/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:36:14.269264 dart-tools-0.3.2/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     1510 2023-04-03 00:03:57.000000 dart-tools-0.3.2/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.265427 dart-tools-0.3.2/dart/
+-rw-r--r--   0 zack       (501) staff       (20)       64 2023-02-28 04:01:58.000000 dart-tools-0.3.2/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    12953 2023-06-02 19:35:29.000000 dart-tools-0.3.2/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)     1709 2023-02-28 02:57:20.000000 dart-tools-0.3.2/dart/order_manager.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2023-06-02 19:36:14.268422 dart-tools-0.3.2/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     4358 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)      290 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zack       (501) staff       (20)       34 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       14 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2023-06-02 19:36:14.000000 dart-tools-0.3.2/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1744 2023-06-02 19:34:24.000000 dart-tools-0.3.2/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2023-06-02 19:36:14.270093 dart-tools-0.3.2/setup.cfg
```

### Comparing `dart-tools-0.3.1/LICENSE` & `dart-tools-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.1/PKG-INFO` & `dart-tools-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.1 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.2 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.1/README.md` & `dart-tools-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.1/dart/dart.py` & `dart-tools-0.3.2/dart/dart.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,23 +410,29 @@
 
     create_task_parser = subparsers.add_parser(
         _CREATE_TASK_CMD, aliases="c", help="create a new task"
     )
     create_task_parser.add_argument("title", help="the title of the task")
     create_task_parser.add_argument(
         "-b",
+        "--begin",
         dest="should_begin",
         action="store_true",
         help="begin work on the task after creation",
     )
     create_task_parser.add_argument(
-        "-p", dest="priority_int", type=int, choices=_PRIORITY_MAP.keys(), help="priority"
+        "-p",
+        "--priority",
+        dest="priority_int",
+        type=int,
+        choices=_PRIORITY_MAP.keys(),
+        help="priority",
     )
     create_task_parser.add_argument(
-        "-i", dest="size", type=int, choices=_SIZES, help="size"
+        "-i", "--size", type=int, choices=_SIZES, help="size"
     )
     create_task_parser.set_defaults(func=create_task)
 
     begin_task_parser = subparsers.add_parser(
         _BEGIN_TASK_CMD, aliases="b", help="begin work on a task"
     )
     begin_task_parser.set_defaults(func=begin_task)
```

### Comparing `dart-tools-0.3.1/dart/order_manager.py` & `dart-tools-0.3.2/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.3.1/dart_tools.egg-info/PKG-INFO` & `dart-tools-0.3.2/dart_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.3.1 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.3.2 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.3.1/pyproject.toml` & `dart-tools-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.3.1"
+version = "0.3.2"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

