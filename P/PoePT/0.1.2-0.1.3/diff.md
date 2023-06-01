# Comparing `tmp/PoePT-0.1.2.tar.gz` & `tmp/PoePT-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PoePT-0.1.2.tar", last modified: Sun May 28 14:23:53 2023, max compression
+gzip compressed data, was "PoePT-0.1.3.tar", last modified: Thu Jun  1 22:19:16 2023, max compression
```

## Comparing `PoePT-0.1.2.tar` & `PoePT-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 14:23:53.688218 PoePT-0.1.2/
--rw-rw-rw-   0        0        0     2253 2023-05-28 14:23:53.688218 PoePT-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 14:23:53.683688 PoePT-0.1.2/PoePT.egg-info/
--rw-rw-rw-   0        0        0     2253 2023-05-28 14:23:53.000000 PoePT-0.1.2/PoePT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-05-28 14:23:53.000000 PoePT-0.1.2/PoePT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 14:23:53.000000 PoePT-0.1.2/PoePT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-28 14:23:53.000000 PoePT-0.1.2/PoePT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 14:23:53.000000 PoePT-0.1.2/PoePT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1603 2023-05-28 13:38:40.000000 PoePT-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 14:23:53.686208 PoePT-0.1.2/poept/
--rw-rw-rw-   0        0        0       47 2023-05-28 14:01:55.000000 PoePT-0.1.2/poept/__init__.py
--rw-rw-rw-   0        0        0     5109 2023-05-28 14:09:51.000000 PoePT-0.1.2/poept/poept.py
--rw-rw-rw-   0        0        0       42 2023-05-28 14:23:53.688218 PoePT-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      924 2023-05-28 14:23:30.000000 PoePT-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 22:19:16.005160 PoePT-0.1.3/
+-rw-rw-rw-   0        0        0     4784 2023-06-01 22:19:16.004157 PoePT-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 22:19:16.000820 PoePT-0.1.3/PoePT.egg-info/
+-rw-rw-rw-   0        0        0     4784 2023-06-01 22:19:15.000000 PoePT-0.1.3/PoePT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-06-01 22:19:15.000000 PoePT-0.1.3/PoePT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 22:19:15.000000 PoePT-0.1.3/PoePT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-01 22:19:15.000000 PoePT-0.1.3/PoePT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 22:19:15.000000 PoePT-0.1.3/PoePT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4134 2023-06-01 22:15:43.000000 PoePT-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 22:19:16.003153 PoePT-0.1.3/poept/
+-rw-rw-rw-   0        0        0       47 2023-05-31 13:42:11.000000 PoePT-0.1.3/poept/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-06-01 22:13:50.000000 PoePT-0.1.3/poept/poept.py
+-rw-rw-rw-   0        0        0       42 2023-06-01 22:19:16.005160 PoePT-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      954 2023-06-01 22:19:09.000000 PoePT-0.1.3/setup.py
```

### Comparing `PoePT-0.1.2/setup.py` & `PoePT-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup
 
 with open('readme.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='PoePT',
-    version='0.1.2',
+    version='0.1.3',
     description='Python package for interacting with the POE chatbot',
     author='Saikyo0',
     author_email='mamaexus@gmail.com',
     url='https://github.com/saikyo0/PoePT',
     packages=['poept'],
     install_requires=[
         'selenium',
-        'webdriver_manager'
+        'webdriver_manager',
+        'SpeechRecognition'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

