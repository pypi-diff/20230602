# Comparing `tmp/cmdsave-1.0.2.tar.gz` & `tmp/cmdsave-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdsave-1.0.2.tar", last modified: Fri Jun  2 19:02:00 2023, max compression
+gzip compressed data, was "cmdsave-1.0.3.tar", last modified: Fri Jun  2 19:15:24 2023, max compression
```

## Comparing `cmdsave-1.0.2.tar` & `cmdsave-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.502120 cmdsave-1.0.2/
--rw-rw-rw-   0        0        0     1909 2023-06-02 19:02:00.502120 cmdsave-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1741 2023-06-02 18:44:34.000000 cmdsave-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.488156 cmdsave-1.0.2/cmdsave/
--rw-rw-rw-   0        0        0     4419 2023-06-02 16:19:57.000000 cmdsave-1.0.2/cmdsave/cmdsave.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:02:00.501123 cmdsave-1.0.2/cmdsave.egg-info/
--rw-rw-rw-   0        0        0     1909 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 19:02:00.000000 cmdsave-1.0.2/cmdsave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 19:02:00.502120 cmdsave-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      606 2023-06-02 19:01:53.000000 cmdsave-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:15:24.739848 cmdsave-1.0.3/
+-rw-rw-rw-   0        0        0     2032 2023-06-02 19:15:24.739848 cmdsave-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1741 2023-06-02 18:44:34.000000 cmdsave-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 19:15:24.727279 cmdsave-1.0.3/cmdsave/
+-rw-rw-rw-   0        0        0     4419 2023-06-02 16:19:57.000000 cmdsave-1.0.3/cmdsave/cmdsave.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:15:24.738851 cmdsave-1.0.3/cmdsave.egg-info/
+-rw-rw-rw-   0        0        0     2032 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 19:15:24.000000 cmdsave-1.0.3/cmdsave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:15:24.739848 cmdsave-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      861 2023-06-02 19:15:13.000000 cmdsave-1.0.3/setup.py
```

### Comparing `cmdsave-1.0.2/PKG-INFO` & `cmdsave-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: cmdsave
-Version: 1.0.2
-Platform: Windows
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-
 # CMDSave - Command Line Application for Saving and Managing Terminal Commands for Later Use
 
 > **This application is only supported on Windows.**
 
 This application allows you to save and manage terminal commands for easy reference and execution. It provides a command-line interface (CLI) to interact with the application and perform various operations such as saving commands, listing saved commands, deleting commands, and editing the command file.
 
 ## Usage Commands
```

### Comparing `cmdsave-1.0.2/README.md` & `cmdsave-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: cmdsave
+Version: 1.0.3
+Summary: 💾 CMDs
+Keywords: save,cli,console,terminal,prductivity
+Platform: Windows
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
 # CMDSave - Command Line Application for Saving and Managing Terminal Commands for Later Use
 
 > **This application is only supported on Windows.**
 
 This application allows you to save and manage terminal commands for easy reference and execution. It provides a command-line interface (CLI) to interact with the application and perform various operations such as saving commands, listing saved commands, deleting commands, and editing the command file.
 
 ## Usage Commands
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmdsave-1.0.2/cmdsave/cmdsave.py` & `cmdsave-1.0.3/cmdsave/cmdsave.py`

 * *Files identical despite different names*

### Comparing `cmdsave-1.0.2/cmdsave.egg-info/PKG-INFO` & `cmdsave-1.0.3/cmdsave.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: cmdsave
-Version: 1.0.2
+Version: 1.0.3
+Summary: 💾 CMDs
+Keywords: save,cli,console,terminal,prductivity
 Platform: Windows
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 # CMDSave - Command Line Application for Saving and Managing Terminal Commands for Later Use
 
 > **This application is only supported on Windows.**
 
 This application allows you to save and manage terminal commands for easy reference and execution. It provides a command-line interface (CLI) to interact with the application and perform various operations such as saving commands, listing saved commands, deleting commands, and editing the command file.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cmdsave-1.0.2/setup.py` & `cmdsave-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 
 setup(
     name='cmdsave',
-    version='1.0.2',
+    version='1.0.3',
     readme="README.md",
+    description="💾 CMDs",
     long_description=Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     packages=['cmdsave'],
     install_requires=[
         'argparse',
         'tabulate',
         'keyboard',
@@ -17,10 +18,18 @@
     entry_points={
         'console_scripts': [
             'cmds = cmdsave.cmdsave:main',
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3.10",
+        "Operating System :: Microsoft :: Windows",
     ],
     platforms=['Windows'],
+    repository='https://github.com/lenzfliker/cmdsave',
+    keywords=[
+        'save',
+        'cli',
+        'console',
+        'terminal',
+        'prductivity',]
 )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

