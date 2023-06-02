# Comparing `tmp/passlock-1.0.7.tar.gz` & `tmp/passlock-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passlock-1.0.7.tar", last modified: Fri Jun  2 17:13:26 2023, max compression
+gzip compressed data, was "passlock-1.0.8.tar", last modified: Fri Jun  2 17:26:53 2023, max compression
```

## Comparing `passlock-1.0.7.tar` & `passlock-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:13:26.037962 passlock-1.0.7/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     7277 2023-06-01 15:11:43.000000 passlock-1.0.7/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/passlock/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.7/passlock/__init__.py
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:13:26.037962 passlock-1.0.7/passlock.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     7591 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:13:25.000000 passlock-1.0.7/passlock.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:13:26.037962 passlock-1.0.7/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      754 2023-06-02 17:13:24.000000 passlock-1.0.7/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6083 2023-06-02 17:26:53.659196 passlock-1.0.8/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     5769 2023-06-02 17:26:36.000000 passlock-1.0.8/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/passlock/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        0 2023-06-02 16:51:00.000000 passlock-1.0.8/passlock/__init__.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-02 17:26:53.659196 passlock-1.0.8/passlock.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6083 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      233 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       53 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        9 2023-06-02 17:26:53.000000 passlock-1.0.8/passlock.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-02 17:26:53.659196 passlock-1.0.8/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      754 2023-06-02 17:26:51.000000 passlock-1.0.8/setup.py
```

### Comparing `passlock-1.0.7/setup.py` & `passlock-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="passlock",
-    version="1.0.7",
+    version="1.0.8",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
```

