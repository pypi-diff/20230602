# Comparing `tmp/Phusion-0.0.1.tar.gz` & `tmp/Phusion-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Phusion-0.0.1.tar", last modified: Thu Jun  1 13:29:13 2023, max compression
+gzip compressed data, was "Phusion-0.0.2.tar", last modified: Fri Jun  2 00:56:32 2023, max compression
```

## Comparing `Phusion-0.0.1.tar` & `Phusion-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-01 13:29:13.323029 Phusion-0.0.1/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-06-01 12:59:28.000000 Phusion-0.0.1/LICENSE.md
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      272 2023-06-01 13:29:13.319029 Phusion-0.0.1/PKG-INFO
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-01 13:29:13.319029 Phusion-0.0.1/Phusion/
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-01 13:02:37.000000 Phusion-0.0.1/Phusion/__init__.py
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     3677 2023-06-01 13:15:55.000000 Phusion-0.0.1/Phusion/main.py
-drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-01 13:29:13.319029 Phusion-0.0.1/Phusion.egg-info/
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      272 2023-06-01 13:29:13.000000 Phusion-0.0.1/Phusion.egg-info/PKG-INFO
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      213 2023-06-01 13:29:13.000000 Phusion-0.0.1/Phusion.egg-info/SOURCES.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-06-01 13:29:13.000000 Phusion-0.0.1/Phusion.egg-info/dependency_links.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       49 2023-06-01 13:29:13.000000 Phusion-0.0.1/Phusion.egg-info/entry_points.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        8 2023-06-01 13:29:13.000000 Phusion-0.0.1/Phusion.egg-info/top_level.txt
--rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-06-01 13:29:13.323029 Phusion-0.0.1/setup.cfg
--rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)      533 2023-06-01 13:23:55.000000 Phusion-0.0.1/setup.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-02 00:56:32.132009 Phusion-0.0.2/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)    34523 2023-06-02 00:14:03.000000 Phusion-0.0.2/LICENSE.md
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      272 2023-06-02 00:56:32.132009 Phusion-0.0.2/PKG-INFO
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-02 00:56:32.132009 Phusion-0.0.2/Phusion/
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-02 00:14:03.000000 Phusion-0.0.2/Phusion/__init__.py
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)     3816 2023-06-02 00:55:16.000000 Phusion-0.0.2/Phusion/main.py
+drwxrwxr-x   0 elookadin  (1000) elookadin  (1000)        0 2023-06-02 00:56:32.132009 Phusion-0.0.2/Phusion.egg-info/
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      272 2023-06-02 00:56:32.000000 Phusion-0.0.2/Phusion.egg-info/PKG-INFO
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)      213 2023-06-02 00:56:32.000000 Phusion-0.0.2/Phusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        1 2023-06-02 00:56:32.000000 Phusion-0.0.2/Phusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       49 2023-06-02 00:56:32.000000 Phusion-0.0.2/Phusion.egg-info/entry_points.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)        8 2023-06-02 00:56:32.000000 Phusion-0.0.2/Phusion.egg-info/top_level.txt
+-rw-rw-r--   0 elookadin  (1000) elookadin  (1000)       38 2023-06-02 00:56:32.132009 Phusion-0.0.2/setup.cfg
+-rwxrwxr-x   0 elookadin  (1000) elookadin  (1000)      533 2023-06-02 00:55:19.000000 Phusion-0.0.2/setup.py
```

### Comparing `Phusion-0.0.1/LICENSE.md` & `Phusion-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Phusion-0.0.1/Phusion/main.py` & `Phusion-0.0.2/Phusion/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     import subprocess
     import argparse
     import configparser
     import datetime
     import random
     import pandas as pd
 
-    image = 'iszatt/phusion:0.0.1'
+    image = 'iszatt/phusion:0.0.2'
 
     # No commands given prompt
     if len(sys.argv) == 1:
         print('No commands given? \nUse -h or --help for more information')
         sys.exit(1)
 
     # Finding the user
@@ -46,14 +46,15 @@
     # Parsing arguments
     parser = argparse.ArgumentParser(description=image)
 
     # Input/output options
     parser.add_argument('-i', '--input', required=True, type=valid_dir,  help='Path to PhageOrder output')
     parser.add_argument('-o', '--output', required=True, type=valid_dir, help='Direct output to specified location')
     parser.add_argument('--cluster', type=int, default=1, help='Clustering threshold (default=1)')
+    parser.add_argument('--pull_genomes', default='no', help='Downloads this number of close relatives (default=0)')
 
     # Adding flags
     parser.add_argument('-v', '--version', action="store_true", help='Print the version of the container this will activate')
     parser.add_argument('--show_console', action="store_true", help='Include this flag to write output to console')
     parser.add_argument('--manual', action="store_true", help='Enter container interactively')
 
     # Finish parsing arguments
@@ -92,11 +93,11 @@
             $(docker run -d \
             -v {input_path}:/craft/input \
             -v {output_path}:/craft/output \
             {image} sleep 1d) bash")
 
     else:
 
-        command = ["%s -v %s:/craft/input -v %s:/craft/output %s /craft/bin/phagecraft.sh %s" %
-                (docker, input_path, output_path, image, args.cluster)]
+        command = ["%s -v %s:/craft/input -v %s:/craft/output %s /craft/bin/phagecraft.sh %s %s" %
+                (docker, input_path, output_path, image, args.cluster, args.pull_genomes)]
         result = subprocess.Popen(command, shell=True)
         print(command)
```

### Comparing `Phusion-0.0.1/setup.py` & `Phusion-0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="Phusion",
-    version="0.0.1",
+    version="0.0.2",
     description="Python package used to aid with cocktail design.",
     url="https://github.com/JoshuaIszatt",
     author="Joshua Iszatt",
     author_email="joshiszatt@gmail.com",
     license="AGPL-3.0",
     install_requires=[""],
     python_requires=">3",
```

