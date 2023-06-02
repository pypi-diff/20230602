# Comparing `tmp/konko-0.0.2.tar.gz` & `tmp/konko-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.2.tar", last modified: Fri Jun  2 17:52:44 2023, max compression
+gzip compressed data, was "konko-0.0.3.tar", last modified: Fri Jun  2 18:58:30 2023, max compression
```

## Comparing `konko-0.0.2.tar` & `konko-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 17:52:44.053315 konko-0.0.2/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 17:52:44.053193 konko-0.0.2/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.2/README.md
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-06-02 17:52:35.000000 konko-0.0.2/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-06-02 17:52:44.053355 konko-0.0.2/setup.cfg
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 17:52:44.052109 konko-0.0.2/src/
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 17:52:44.052586 konko-0.0.2/src/konko/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       30 2023-06-02 17:48:57.000000 konko-0.0.2/src/konko/__init__.py
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       41 2023-06-02 17:22:38.000000 konko-0.0.2/src/konko/generate.py
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 17:52:44.053055 konko-0.0.2/src/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 17:52:44.000000 konko-0.0.2/src/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      200 2023-06-02 17:52:44.000000 konko-0.0.2/src/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 17:52:44.000000 konko-0.0.2/src/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        6 2023-06-02 17:52:44.000000 konko-0.0.2/src/konko.egg-info/top_level.txt
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 18:58:30.682011 konko-0.0.3/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 18:58:30.681881 konko-0.0.3/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.3/README.md
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 18:58:30.681747 konko-0.0.3/konko.egg-info/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      177 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/SOURCES.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/dependency_links.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        4 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/requires.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/top_level.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-06-02 18:58:04.000000 konko-0.0.3/pyproject.toml
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-06-02 18:58:30.682049 konko-0.0.3/setup.cfg
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      184 2023-06-02 18:57:59.000000 konko-0.0.3/setup.py
```

