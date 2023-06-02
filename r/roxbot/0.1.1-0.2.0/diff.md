# Comparing `tmp/roxbot-0.1.1.tar.gz` & `tmp/roxbot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-0.1.1.tar", last modified: Thu May 25 17:52:26 2023, max compression
+gzip compressed data, was "roxbot-0.2.0.tar", last modified: Fri Jun  2 11:19:13 2023, max compression
```

## Comparing `roxbot-0.1.1.tar` & `roxbot-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-25 17:52:14.000000 roxbot-0.1.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 17:52:26.588015 roxbot-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1598 2023-05-25 17:52:14.000000 roxbot-0.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-05-25 17:52:26.589015 roxbot-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1467 2023-05-25 17:52:14.000000 roxbot-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.585015 roxbot-0.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.587015 roxbot-0.1.1/src/roxbot/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-25 17:52:14.000000 roxbot-0.1.1/src/roxbot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-05-25 17:52:14.000000 roxbot-0.1.1/src/roxbot/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/src/roxbot.egg-info/
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 17:52:26.000000 roxbot-0.1.1/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 17:52:26.588015 roxbot-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-05-25 17:52:14.000000 roxbot-0.1.1/tests/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.414440 roxbot-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2023-06-02 11:19:04.000000 roxbot-0.2.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 11:19:13.414440 roxbot-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-06-02 11:19:04.000000 roxbot-0.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-06-02 11:19:13.414440 roxbot-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-02 11:19:04.000000 roxbot-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.409441 roxbot-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.411440 roxbot-0.2.0/src/roxbot/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     5874 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     5020 2023-06-02 11:19:04.000000 roxbot-0.2.0/src/roxbot/vectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.413441 roxbot-0.2.0/src/roxbot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 11:19:13.000000 roxbot-0.2.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:19:13.414440 roxbot-0.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2780 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_gps.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2023-06-02 11:19:04.000000 roxbot-0.2.0/tests/test_vectors.py
```

### Comparing `roxbot-0.1.1/LICENCE` & `roxbot-0.2.0/LICENCE`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021 Jev Kuznetsov <jev.kuznetsov@gmail.com>
+Copyright (c) 2023 ROX Automation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `roxbot-0.1.1/README.md` & `roxbot-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 ---
 
 KISS robootics framework
 
 
 ## Development
 
+**Please develop inside the container**, this will ensure all the required checks (`pylint` & `mypy`) as well as formatting (`black`)
+
 If you are not familiar with devcontainers, read [Developing inside a Container](https://code.visualstudio.com/docs/devcontainers/containers) first
 
 1. Clone this repository
-2. open dir in *VS Code `vscode .`
+2. open dir in *VS Code* `vscode .`
 3. rebuild and reopen in container (you'll need `Dev Containers` extension)
 
 **note**: if a container with `devcontainer` name already exists, an error will occur. You can remove it with
 `docker container prune -f`
 
 
 ### What goes where
```

### Comparing `roxbot-0.1.1/setup.py` & `roxbot-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,23 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
         else:
             raise RuntimeError("Unable to find version string.")
 
 
 # please keep this lean and mean. Add dev requirements to .devcontainer/requirments.txt
-requirements = ["click"]
+requirements = ["click", "pymap3d", "pynmea2"]
 
 test_requirements = [
     "pytest>=3",
 ]
 
 setup(
-    author="Jev Kuznetsov",
-    author_email="jev.kuznetsov@gmail.com",
+    author="ROX Autmation",
+    author_email="dev@roxautomation.com",
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.10",
     ],
```

