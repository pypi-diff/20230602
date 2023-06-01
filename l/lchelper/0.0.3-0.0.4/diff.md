# Comparing `tmp/lchelper-0.0.3.tar.gz` & `tmp/lchelper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lchelper-0.0.3.tar", last modified: Thu Jun  1 04:30:58 2023, max compression
+gzip compressed data, was "lchelper-0.0.4.tar", last modified: Thu Jun  1 21:58:12 2023, max compression
```

## Comparing `lchelper-0.0.3.tar` & `lchelper-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:30:58.958541 lchelper-0.0.3/
--rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:30:58.958151 lchelper-0.0.3/PKG-INFO
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:30:58.955420 lchelper-0.0.3/lchelper/
--rw-r--r--   0 edwhan     (501) staff       (20)        0 2023-06-01 04:00:06.000000 lchelper-0.0.3/lchelper/__init__.py
--rw-r--r--   0 edwhan     (501) staff       (20)       19 2023-06-01 04:30:48.000000 lchelper-0.0.3/lchelper/constants.py
--rw-r--r--   0 edwhan     (501) staff       (20)       95 2023-06-01 04:01:18.000000 lchelper-0.0.3/lchelper/linkedlist.py
-drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 04:30:58.957565 lchelper-0.0.3/lchelper.egg-info/
--rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 04:30:58.000000 lchelper-0.0.3/lchelper.egg-info/PKG-INFO
--rw-r--r--   0 edwhan     (501) staff       (20)      202 2023-06-01 04:30:58.000000 lchelper-0.0.3/lchelper.egg-info/SOURCES.txt
--rw-r--r--   0 edwhan     (501) staff       (20)        1 2023-06-01 04:30:58.000000 lchelper-0.0.3/lchelper.egg-info/dependency_links.txt
--rw-r--r--   0 edwhan     (501) staff       (20)        9 2023-06-01 04:30:58.000000 lchelper-0.0.3/lchelper.egg-info/top_level.txt
--rw-r--r--   0 edwhan     (501) staff       (20)       38 2023-06-01 04:30:58.958664 lchelper-0.0.3/setup.cfg
--rw-r--r--   0 edwhan     (501) staff       (20)      315 2023-06-01 04:30:31.000000 lchelper-0.0.3/setup.py
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 21:58:12.109925 lchelper-0.0.4/
+-rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 21:58:12.109572 lchelper-0.0.4/PKG-INFO
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 21:58:12.106752 lchelper-0.0.4/lchelper/
+-rw-r--r--   0 edwhan     (501) staff       (20)        0 2023-06-01 04:00:06.000000 lchelper-0.0.4/lchelper/__init__.py
+-rw-r--r--   0 edwhan     (501) staff       (20)       19 2023-06-01 21:57:57.000000 lchelper-0.0.4/lchelper/constants.py
+-rw-r--r--   0 edwhan     (501) staff       (20)       95 2023-06-01 04:01:18.000000 lchelper-0.0.4/lchelper/linkedlist.py
+drwxr-xr-x   0 edwhan     (501) staff       (20)        0 2023-06-01 21:58:12.109033 lchelper-0.0.4/lchelper.egg-info/
+-rw-r--r--   0 edwhan     (501) staff       (20)       52 2023-06-01 21:58:12.000000 lchelper-0.0.4/lchelper.egg-info/PKG-INFO
+-rw-r--r--   0 edwhan     (501) staff       (20)      202 2023-06-01 21:58:12.000000 lchelper-0.0.4/lchelper.egg-info/SOURCES.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)        1 2023-06-01 21:58:12.000000 lchelper-0.0.4/lchelper.egg-info/dependency_links.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)        9 2023-06-01 21:58:12.000000 lchelper-0.0.4/lchelper.egg-info/top_level.txt
+-rw-r--r--   0 edwhan     (501) staff       (20)       38 2023-06-01 21:58:12.110044 lchelper-0.0.4/setup.cfg
+-rw-r--r--   0 edwhan     (501) staff       (20)      241 2023-06-01 21:57:57.000000 lchelper-0.0.4/setup.py
```

