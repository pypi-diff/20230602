# Comparing `tmp/konko-0.0.3.tar.gz` & `tmp/konko-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konko-0.0.3.tar", last modified: Fri Jun  2 18:58:30 2023, max compression
+gzip compressed data, was "konko-0.0.4.tar", last modified: Fri Jun  2 19:01:28 2023, max compression
```

## Comparing `konko-0.0.3.tar` & `konko-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 18:58:30.682011 konko-0.0.3/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 18:58:30.681881 konko-0.0.3/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.3/README.md
-drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 18:58:30.681747 konko-0.0.3/konko.egg-info/
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/PKG-INFO
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      177 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/SOURCES.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/dependency_links.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        4 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/requires.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 18:58:30.000000 konko-0.0.3/konko.egg-info/top_level.txt
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-06-02 18:58:04.000000 konko-0.0.3/pyproject.toml
--rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-06-02 18:58:30.682049 konko-0.0.3/setup.cfg
--rw-r--r--   0 uday.kanwar   (501) staff       (20)      184 2023-06-02 18:57:59.000000 konko-0.0.3/setup.py
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:01:28.938056 konko-0.0.4/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 19:01:28.937892 konko-0.0.4/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       29 2023-06-01 17:28:19.000000 konko-0.0.4/README.md
+drwxr-xr-x   0 uday.kanwar   (501) staff       (20)        0 2023-06-02 19:01:28.937690 konko-0.0.4/konko.egg-info/
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      254 2023-06-02 19:01:28.000000 konko-0.0.4/konko.egg-info/PKG-INFO
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      149 2023-06-02 19:01:28.000000 konko-0.0.4/konko.egg-info/SOURCES.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 19:01:28.000000 konko-0.0.4/konko.egg-info/dependency_links.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)        1 2023-06-02 19:01:28.000000 konko-0.0.4/konko.egg-info/top_level.txt
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      304 2023-06-02 19:00:12.000000 konko-0.0.4/pyproject.toml
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)       38 2023-06-02 19:01:28.938098 konko-0.0.4/setup.cfg
+-rw-r--r--   0 uday.kanwar   (501) staff       (20)      147 2023-06-02 19:01:06.000000 konko-0.0.4/setup.py
```

