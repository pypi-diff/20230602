# Comparing `tmp/all-fives-domino-1.0.7.tar.gz` & `tmp/all-fives-domino-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all-fives-domino-1.0.7.tar", last modified: Sat May 27 06:35:13 2023, max compression
+gzip compressed data, was "all-fives-domino-1.0.8.tar", last modified: Fri Jun  2 12:17:29 2023, max compression
```

## Comparing `all-fives-domino-1.0.7.tar` & `all-fives-domino-1.0.8.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.849013 all-fives-domino-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      802 2023-05-27 06:35:13.845013 all-fives-domino-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-27 06:34:57.000000 all-fives-domino-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.833013 all-fives-domino-1.0.7/all_fives_domino.egg-info/
--rw-r--r--   0 root         (0) root         (0)      802 2023-05-27 06:35:13.000000 all-fives-domino-1.0.7/all_fives_domino.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1347 2023-05-27 06:35:13.000000 all-fives-domino-1.0.7/all_fives_domino.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-27 06:35:13.000000 all-fives-domino-1.0.7/all_fives_domino.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-27 06:35:13.000000 all-fives-domino-1.0.7/all_fives_domino.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-27 06:35:13.849013 all-fives-domino-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.7/src/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/main/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/main/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.7/src/main/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/main/game/
--rw-r--r--   0 root         (0) root         (0)     2987 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/main/game/DominoRound.py
--rw-r--r--   0 root         (0) root         (0)     2603 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/main/game/Piece.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/main/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.837013 all-fives-domino-1.0.7/src/main/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4864 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/main/game/__pycache__/DominoRound.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     4585 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/main/game/__pycache__/Piece.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.7/src/main/game/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.841013 all-fives-domino-1.0.7/src/main/player/
--rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.7/src/main/player/Brain.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/main/player/Hand.py
--rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/main/player/Player.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/main/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.841013 all-fives-domino-1.0.7/src/main/player/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2005 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/main/player/__pycache__/Hand.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/main/player/__pycache__/Player.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/main/player/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.841013 all-fives-domino-1.0.7/src/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.841013 all-fives-domino-1.0.7/src/test/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.7/src/test/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.845013 all-fives-domino-1.0.7/src/test/game/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.7/src/test/game/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.845013 all-fives-domino-1.0.7/src/test/game/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.7/src/test/game/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)    26801 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)     1411 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/test/game/test_pieces.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/test/game/test_round.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.845013 all-fives-domino-1.0.7/src/test/player/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 22:06:49.000000 all-fives-domino-1.0.7/src/test/player/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-27 06:35:13.845013 all-fives-domino-1.0.7/src/test/player/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.7/src/test/player/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 root         (0) root         (0)     8551 2023-05-27 06:34:56.000000 all-fives-domino-1.0.7/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-27 06:34:49.000000 all-fives-domino-1.0.7/src/test/player/test_hand.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-27 06:34:59.000000 all-fives-domino-1.0.7/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-02 12:17:14.000000 all-fives-domino-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/all_fives_domino.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-02 12:17:29.000000 all-fives-domino-1.0.8/all_fives_domino.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      798 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.785643 all-fives-domino-1.0.8/src/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/main/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/game/
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-02 12:17:05.000000 all-fives-domino-1.0.8/src/main/game/DominoRound.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/game/Piece.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     5709 2023-06-02 12:17:13.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/DominoRound.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     4585 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/Piece.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/main/game/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.789643 all-fives-domino-1.0.8/src/main/player/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-05-25 21:10:41.000000 all-fives-domino-1.0.8/src/main/player/Brain.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/player/Hand.py
+-rw-r--r--   0 root         (0) root         (0)      380 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/main/player/Player.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/main/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/main/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/Hand.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/Player.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/main/player/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/main/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 12:17:05.000000 all-fives-domino-1.0.8/src/main/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/test/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/game/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 20:33:44.000000 all-fives-domino-1.0.8/src/test/game/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.793644 all-fives-domino-1.0.8/src/test/game/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-25 20:34:42.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)    26801 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      551 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/game/test_pieces.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/game/test_round.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/src/test/player/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-26 22:06:49.000000 all-fives-domino-1.0.8/src/test/player/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 12:17:29.797644 all-fives-domino-1.0.8/src/test/player/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-05-26 22:11:06.000000 all-fives-domino-1.0.8/src/test/player/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 root         (0) root         (0)     8551 2023-05-27 06:34:56.000000 all-fives-domino-1.0.8/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-27 06:34:49.000000 all-fives-domino-1.0.8/src/test/player/test_hand.py
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-02 12:17:16.000000 all-fives-domino-1.0.8/version.txt
```

### Comparing `all-fives-domino-1.0.7/LICENSE` & `all-fives-domino-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/PKG-INFO` & `all-fives-domino-1.0.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.7
+Version: 1.0.8
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=12+tests&color=success&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=54%25&color=yellow&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=50%25&color=orange&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.7/all_fives_domino.egg-info/PKG-INFO` & `all-fives-domino-1.0.8/all_fives_domino.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-fives-domino
-Version: 1.0.7
+Version: 1.0.8
 Summary: Abstractions around cloud file interfaces (WIP)
 Home-page: https://github.com/Informanthik/all-fives-domino
 Author: Jothapunkt
 Author-email: jakob-hoefner@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -12,15 +12,15 @@
 All Fives Domino
 ================
 
 Simple version of a domino variant
 
 ![image](https://img.shields.io/pypi/v/jhdata?style=flat-square)
 ![image](https://img.shields.io/static/v1?label=pytest&message=12+tests&color=success&style=flat-square)
-![image](https://img.shields.io/static/v1?label=coverage&message=54%25&color=yellow&style=flat-square)
+![image](https://img.shields.io/static/v1?label=coverage&message=50%25&color=orange&style=flat-square)
 
 ## Installing
 
 Install the [PyPI Package](https://pypi.org/project/all-fives-domino/):
 
     pip install all-fives-domino
```

### Comparing `all-fives-domino-1.0.7/all_fives_domino.egg-info/SOURCES.txt` & `all-fives-domino-1.0.8/all_fives_domino.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/main/player/Brain.py
 src/main/player/Hand.py
 src/main/player/Player.py
 src/main/player/__init__.py
 src/main/player/__pycache__/Hand.cpython-311.pyc
 src/main/player/__pycache__/Player.cpython-311.pyc
 src/main/player/__pycache__/__init__.cpython-311.pyc
+src/main/ui/__init__.py
 src/test/__init__.py
 src/test/__pycache__/__init__.cpython-311.pyc
 src/test/game/__init__.py
 src/test/game/test_pieces.py
 src/test/game/test_round.py
 src/test/game/__pycache__/__init__.cpython-311.pyc
 src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc
```

### Comparing `all-fives-domino-1.0.7/setup.py` & `all-fives-domino-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/main/game/Piece.py` & `all-fives-domino-1.0.8/src/main/game/Piece.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/main/game/__pycache__/DominoRound.cpython-311.pyc` & `all-fives-domino-1.0.8/src/main/game/__pycache__/DominoRound.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x792d7164 (Fri May 26 22:06:49 2023 UTC)
-files sz: 2987
+moddate:  0xc1dd7964 (Fri Jun  2 12:17:05 2023 UTC)
+files sz: 3981
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -57,18 +57,18 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 9
          flags     : 0
          code
             0x970065005a0164005a0264016402640364026404650364051900000000
-            00000000006606640684045a04640784005a05640884005a066507641464
-            0a65086602640b8405a6000000ab0000000000000000005a09640c84005a
-            0a6415640e650b640a6508640f6503650864106602190000000000000000
-            006606641184055a0c641284005a0d641384005a0e64105300
+            00000000006606640684045a04640784005a05640884005a066507641564
+            0a6508640b65096604640c8405a6000000ab0000000000000000005a0a64
+            0d84005a0b6416640f650c640a6508641065036508641166021900000000
+            00000000006606641284055a0d641384005a0e641484005a0f64115300
            7           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DominoRound')
                        8 STORE_NAME               2 (__qualname__)
          
            8          10 LOAD_CONST               1 ('brain1')
@@ -90,55 +90,57 @@
          
           22          48 LOAD_CONST               8 (<code object get_required_starting_piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 22>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               6 (get_required_starting_piece)
          
           44          54 LOAD_NAME                7 (staticmethod)
          
-          45          56 LOAD_CONST              20 ((28,))
+          45          56 LOAD_CONST              21 ((28,))
                       58 LOAD_CONST              10 ('piece')
                       60 LOAD_NAME                8 (Piece)
-                      62 BUILD_TUPLE              2
-                      64 LOAD_CONST              11 (<code object score_piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 44>)
-                      66 MAKE_FUNCTION            5 (defaults, annotations)
-         
-          44          68 PRECALL                  0
-                      72 CALL                     0
-         
-          45          82 STORE_NAME               9 (score_piece)
-         
-          53          84 LOAD_CONST              12 (<code object score, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 53>)
-                      86 MAKE_FUNCTION            0
-                      88 STORE_NAME              10 (score)
-         
-          57          90 LOAD_CONST              21 ((False,))
-                      92 LOAD_CONST              14 ('player')
-                      94 LOAD_NAME               11 (Player)
-                      96 LOAD_CONST              10 ('piece')
-                      98 LOAD_NAME                8 (Piece)
-                     100 LOAD_CONST              15 ('origin')
-                     102 LOAD_NAME                3 (Union)
-                     104 LOAD_NAME                8 (Piece)
-                     106 LOAD_CONST              16 (None)
-                     108 BUILD_TUPLE              2
-                     110 BINARY_SUBSCR
-                     120 BUILD_TUPLE              6
-                     122 LOAD_CONST              17 (<code object play, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 57>)
-                     124 MAKE_FUNCTION            5 (defaults, annotations)
-                     126 STORE_NAME              12 (play)
-         
-          80         128 LOAD_CONST              18 (<code object valid_options, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 80>)
-                     130 MAKE_FUNCTION            0
-                     132 STORE_NAME              13 (valid_options)
-         
-          83         134 LOAD_CONST              19 (<code object run, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 83>)
-                     136 MAKE_FUNCTION            0
-                     138 STORE_NAME              14 (run)
-                     140 LOAD_CONST              16 (None)
-                     142 RETURN_VALUE
+                      62 LOAD_CONST              11 ('return')
+                      64 LOAD_NAME                9 (int)
+                      66 BUILD_TUPLE              4
+                      68 LOAD_CONST              12 (<code object score_piece, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 44>)
+                      70 MAKE_FUNCTION            5 (defaults, annotations)
+         
+          44          72 PRECALL                  0
+                      76 CALL                     0
+         
+          45          86 STORE_NAME              10 (score_piece)
+         
+          76          88 LOAD_CONST              13 (<code object score, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 76>)
+                      90 MAKE_FUNCTION            0
+                      92 STORE_NAME              11 (score)
+         
+          80          94 LOAD_CONST              22 ((False,))
+                      96 LOAD_CONST              15 ('player')
+                      98 LOAD_NAME               12 (Player)
+                     100 LOAD_CONST              10 ('piece')
+                     102 LOAD_NAME                8 (Piece)
+                     104 LOAD_CONST              16 ('origin')
+                     106 LOAD_NAME                3 (Union)
+                     108 LOAD_NAME                8 (Piece)
+                     110 LOAD_CONST              17 (None)
+                     112 BUILD_TUPLE              2
+                     114 BINARY_SUBSCR
+                     124 BUILD_TUPLE              6
+                     126 LOAD_CONST              18 (<code object play, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 80>)
+                     128 MAKE_FUNCTION            5 (defaults, annotations)
+                     130 STORE_NAME              13 (play)
+         
+         103         132 LOAD_CONST              19 (<code object valid_options, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 103>)
+                     134 MAKE_FUNCTION            0
+                     136 STORE_NAME              14 (valid_options)
+         
+         106         138 LOAD_CONST              20 (<code object run, file "/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py", line 106>)
+                     140 MAKE_FUNCTION            0
+                     142 STORE_NAME              15 (run)
+                     144 LOAD_CONST              17 (None)
+                     146 RETURN_VALUE
          consts
             'DominoRound'
             'brain1'
             'Brain'
             'brain2'
             'begins'
             ('Brain', None)
@@ -359,75 +361,182 @@
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'get_required_starting_piece'
                firstlineno 22
                lnotab 0x02080e0104020e01080120021c01180108011c01180108fe02f9
             28
             'piece'
+            'return'
             code
                argcount  : 2
-               nlocals   : 3
-               stacksize : 2
+               nlocals   : 4
+               stacksize : 7
                flags     : 3
                code
-                  0x970064017d027c006a00000000000000000080127c006a010000000000
-                  00000067006b020000000072077c006a02000000000000000053007c0253
-                  00
+                  0x97007c0164016b0000000000720f7401000000000000000000006402a6
+                  010000ab010000000000000000820164017d027c006a0100000000000000
+                  0080117c006a020000000000000000730a7c027c006a0300000000000000
+                  007a0d00007d027c006a02000000000000000073077c006a010000000000
+                  000000801f7c006a01000000000000000080477409000000000000000000
+                  007c006a020000000000000000a6010000ab01000000000000000064046b
+                  0200000000722f7c006a050000000000000000720b7c027c006a03000000
+                  00000000007a0d00007d026e1d7c027c00a0060000000000000000000000
+                  0000000000000000007c006a010000000000000000a6010000ab01000000
+                  00000000007a0d00007d027c006a07000000000000000072287409000000
+                  000000000000007c006a020000000000000000a6010000ab010000000000
+                  00000064056b020000000072107c027c006a080000000000000000640119
+                  0000000000000000007a0d00007d027c006a02000000000000000044005d
+                  1d7d037c027413000000000000000000006a0a00000000000000007c037c
+                  0164047a0a0000a6020000ab0200000000000000007a0d00007d028c1e7c
+                  025300
                 44           0 RESUME                   0
                
-                46           2 LOAD_CONST               1 (0)
-                             4 STORE_FAST               2 (piece_score)
-               
-                48           6 LOAD_FAST                0 (piece)
-                             8 LOAD_ATTR                0 (linked_to)
-                            18 POP_JUMP_FORWARD_IF_NOT_NONE    18 (to 56)
-                            20 LOAD_FAST                0 (piece)
-                            22 LOAD_ATTR                1 (linked)
-                            32 BUILD_LIST               0
-                            34 COMPARE_OP               2 (==)
-                            40 POP_JUMP_FORWARD_IF_FALSE     7 (to 56)
-               
-                49          42 LOAD_FAST                0 (piece)
-                            44 LOAD_ATTR                2 (points)
-                            54 RETURN_VALUE
+                50           2 LOAD_FAST                1 (depth)
+                             4 LOAD_CONST               1 (0)
+                             6 COMPARE_OP               0 (<)
+                            12 POP_JUMP_FORWARD_IF_FALSE    15 (to 44)
+               
+                51          14 LOAD_GLOBAL              1 (NULL + Exception)
+                            26 LOAD_CONST               2 ('Recursion too deep, some pieces linked in a loop?')
+                            28 PRECALL                  1
+                            32 CALL                     1
+                            42 RAISE_VARARGS            1
+               
+                53     >>   44 LOAD_CONST               1 (0)
+                            46 STORE_FAST               2 (score)
+               
+                56          48 LOAD_FAST                0 (piece)
+                            50 LOAD_ATTR                1 (linked_to)
+                            60 POP_JUMP_FORWARD_IF_NOT_NONE    17 (to 96)
+                            62 LOAD_FAST                0 (piece)
+                            64 LOAD_ATTR                2 (linked)
+                            74 POP_JUMP_FORWARD_IF_TRUE    10 (to 96)
+               
+                57          76 LOAD_FAST                2 (score)
+                            78 LOAD_FAST                0 (piece)
+                            80 LOAD_ATTR                3 (points)
+                            90 BINARY_OP               13 (+=)
+                            94 STORE_FAST               2 (score)
+               
+                60     >>   96 LOAD_FAST                0 (piece)
+                            98 LOAD_ATTR                2 (linked)
+                           108 POP_JUMP_FORWARD_IF_TRUE     7 (to 124)
+                           110 LOAD_FAST                0 (piece)
+                           112 LOAD_ATTR                1 (linked_to)
+                           122 POP_JUMP_FORWARD_IF_NOT_NONE    31 (to 186)
+                       >>  124 LOAD_FAST                0 (piece)
+                           126 LOAD_ATTR                1 (linked_to)
+                           136 POP_JUMP_FORWARD_IF_NOT_NONE    71 (to 280)
+                           138 LOAD_GLOBAL              9 (NULL + len)
+                           150 LOAD_FAST                0 (piece)
+                           152 LOAD_ATTR                2 (linked)
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 LOAD_CONST               4 (1)
+                           178 COMPARE_OP               2 (==)
+                           184 POP_JUMP_FORWARD_IF_FALSE    47 (to 280)
+               
+                61     >>  186 LOAD_FAST                0 (piece)
+                           188 LOAD_ATTR                5 (is_double)
+                           198 POP_JUMP_FORWARD_IF_FALSE    11 (to 222)
+               
+                62         200 LOAD_FAST                2 (score)
+                           202 LOAD_FAST                0 (piece)
+                           204 LOAD_ATTR                3 (points)
+                           214 BINARY_OP               13 (+=)
+                           218 STORE_FAST               2 (score)
+                           220 JUMP_FORWARD            29 (to 280)
+               
+                64     >>  222 LOAD_FAST                2 (score)
+                           224 LOAD_FAST                0 (piece)
+                           226 LOAD_METHOD              6 (unlinked_side)
+                           248 LOAD_FAST                0 (piece)
+                           250 LOAD_ATTR                1 (linked_to)
+                           260 PRECALL                  1
+                           264 CALL                     1
+                           274 BINARY_OP               13 (+=)
+                           278 STORE_FAST               2 (score)
+               
+                67     >>  280 LOAD_FAST                0 (piece)
+                           282 LOAD_ATTR                7 (is_crossing)
+                           292 POP_JUMP_FORWARD_IF_FALSE    40 (to 374)
+                           294 LOAD_GLOBAL              9 (NULL + len)
+                           306 LOAD_FAST                0 (piece)
+                           308 LOAD_ATTR                2 (linked)
+                           318 PRECALL                  1
+                           322 CALL                     1
+                           332 LOAD_CONST               5 (3)
+                           334 COMPARE_OP               2 (==)
+                           340 POP_JUMP_FORWARD_IF_FALSE    16 (to 374)
+               
+                68         342 LOAD_FAST                2 (score)
+                           344 LOAD_FAST                0 (piece)
+                           346 LOAD_ATTR                8 (sides)
+                           356 LOAD_CONST               1 (0)
+                           358 BINARY_SUBSCR
+                           368 BINARY_OP               13 (+=)
+                           372 STORE_FAST               2 (score)
+               
+                71     >>  374 LOAD_FAST                0 (piece)
+                           376 LOAD_ATTR                2 (linked)
+                           386 GET_ITER
+                       >>  388 FOR_ITER                29 (to 448)
+                           390 STORE_FAST               3 (linked_piece)
+               
+                72         392 LOAD_FAST                2 (score)
+                           394 LOAD_GLOBAL             19 (NULL + Piece)
+                           406 LOAD_ATTR               10 (score_piece)
+                           416 LOAD_FAST                3 (linked_piece)
+                           418 LOAD_FAST                1 (depth)
+                           420 LOAD_CONST               4 (1)
+                           422 BINARY_OP               10 (-)
+                           426 PRECALL                  2
+                           430 CALL                     2
+                           440 BINARY_OP               13 (+=)
+                           444 STORE_FAST               2 (score)
+                           446 JUMP_BACKWARD           30 (to 388)
                
-                51     >>   56 LOAD_FAST                2 (piece_score)
-                            58 RETURN_VALUE
+                74     >>  448 LOAD_FAST                2 (score)
+                           450 RETURN_VALUE
                consts
-                  None
+                  "\n        Calculate the score for a piece and it's attached pieces\n        "
                   0
-               names      ('linked_to', 'linked', 'points')
-               varnames   ('piece', 'depth', 'piece_score')
+                  'Recursion too deep, some pieces linked in a loop?'
+                  None
+                  1
+                  3
+               names      ('Exception', 'linked_to', 'linked', 'points', 'len', 'is_double', 'unlinked_side', 'is_crossing', 'sides', 'Piece', 'score_piece')
+               varnames   ('piece', 'depth', 'score', 'linked_piece')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'score_piece'
                firstlineno 44
-               lnotab 0x0202040224010e02
+               lnotab 0x02060c011e0204031c0114035a010e0116023a033e01200312013802
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a6010000ab0100000000000000007d017c006a0200
                   0000000000000078016a0300000000000000007c017a0d000063025f0300
                   0000000000000064005300
-                53           0 RESUME                   0
+                76           0 RESUME                   0
                
-                54           2 LOAD_FAST                0 (self)
+                77           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (score_piece)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (origin)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (score)
                
-                55          54 LOAD_FAST                0 (self)
+                78          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (current_player)
                             66 COPY                     1
                             68 LOAD_ATTR                3 (score)
                             78 LOAD_FAST                1 (score)
                             80 BINARY_OP               13 (+=)
                             84 SWAP                     2
                             86 STORE_ATTR               3 (score)
@@ -437,15 +546,15 @@
                   None
                names      ('score_piece', 'origin', 'current_player', 'score')
                varnames   ('self', 'score')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'score'
-               firstlineno 53
+               firstlineno 76
                lnotab 0x02013401
             False
             'player'
             'origin'
             None
             code
                argcount  : 5
@@ -463,108 +572,108 @@
                   04a6010000ab01000000000000000082017c027c005f0600000000000000
                   006e157c03a00700000000000000000000000000000000000000007c02a6
                   010000ab01000000000000000001007c00a0080000000000000000000000
                   000000000000000000a6000000ab00000000000000000001007c006a0900
                   000000000000007c006a0a00000000000000006b0200000000720e7c006a
                   0b00000000000000007c005f090000000000000000640053007c006a0a00
                   000000000000007c005f09000000000000000064005300
-                57           0 RESUME                   0
+                80           0 RESUME                   0
                
-                58           2 LOAD_FAST                2 (piece)
+                81           2 LOAD_FAST                2 (piece)
                              4 LOAD_FAST                1 (player)
                              6 LOAD_ATTR                0 (hand)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE    19 (to 58)
                
-                59          20 LOAD_GLOBAL              3 (NULL + Exception)
+                82          20 LOAD_GLOBAL              3 (NULL + Exception)
                             32 LOAD_CONST               1 ('Player attempted to play ')
                             34 LOAD_FAST                2 (piece)
                             36 FORMAT_VALUE             0
                             38 LOAD_CONST               2 (", but it's not in their hand")
                             40 BUILD_STRING             3
                             42 PRECALL                  1
                             46 CALL                     1
                             56 RAISE_VARARGS            1
                
-                61     >>   58 LOAD_FAST                2 (piece)
+                84     >>   58 LOAD_FAST                2 (piece)
                             60 LOAD_ATTR                2 (is_double)
                             70 POP_JUMP_FORWARD_IF_FALSE    16 (to 104)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_ATTR                3 (has_crossing)
                             84 POP_JUMP_FORWARD_IF_FALSE     9 (to 104)
                             86 LOAD_FAST                4 (close)
                             88 POP_JUMP_FORWARD_IF_FALSE     7 (to 104)
                
-                62          90 LOAD_CONST               3 (True)
+                85          90 LOAD_CONST               3 (True)
                             92 LOAD_FAST                2 (piece)
                             94 STORE_ATTR               4 (closed)
                
-                64     >>  104 LOAD_FAST                1 (player)
+                87     >>  104 LOAD_FAST                1 (player)
                            106 LOAD_ATTR                0 (hand)
                            116 LOAD_METHOD              5 (pop)
                            138 LOAD_FAST                2 (piece)
                            140 PRECALL                  1
                            144 CALL                     1
                            154 POP_TOP
                
-                66         156 LOAD_FAST                3 (origin)
+                89         156 LOAD_FAST                3 (origin)
                            158 POP_JUMP_FORWARD_IF_NOT_NONE    41 (to 242)
                
-                67         160 LOAD_FAST                0 (self)
+                90         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                6 (origin)
                            172 POP_JUMP_FORWARD_IF_NONE    26 (to 226)
                
-                68         174 LOAD_GLOBAL              3 (NULL + Exception)
+                91         174 LOAD_GLOBAL              3 (NULL + Exception)
                            186 LOAD_CONST               1 ('Player attempted to play ')
                            188 LOAD_FAST                2 (piece)
                            190 FORMAT_VALUE             0
                            192 LOAD_CONST               4 (' as origin, but there is already origin piece ')
                
-                69         194 LOAD_FAST                0 (self)
+                92         194 LOAD_FAST                0 (self)
                            196 LOAD_ATTR                6 (origin)
                
-                68         206 FORMAT_VALUE             0
+                91         206 FORMAT_VALUE             0
                            208 BUILD_STRING             4
                            210 PRECALL                  1
                            214 CALL                     1
                            224 RAISE_VARARGS            1
                
-                70     >>  226 LOAD_FAST                2 (piece)
+                93     >>  226 LOAD_FAST                2 (piece)
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               6 (origin)
                            240 JUMP_FORWARD            21 (to 284)
                
-                72     >>  242 LOAD_FAST                3 (origin)
+                95     >>  242 LOAD_FAST                3 (origin)
                            244 LOAD_METHOD              7 (append)
                            266 LOAD_FAST                2 (piece)
                            268 PRECALL                  1
                            272 CALL                     1
                            282 POP_TOP
                
-                73     >>  284 LOAD_FAST                0 (self)
+                96     >>  284 LOAD_FAST                0 (self)
                            286 LOAD_METHOD              8 (score)
                            308 PRECALL                  0
                            312 CALL                     0
                            322 POP_TOP
                
-                75         324 LOAD_FAST                0 (self)
+                98         324 LOAD_FAST                0 (self)
                            326 LOAD_ATTR                9 (current_player)
                            336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR               10 (player1)
                            348 COMPARE_OP               2 (==)
                            354 POP_JUMP_FORWARD_IF_FALSE    14 (to 384)
                
-                76         356 LOAD_FAST                0 (self)
+                99         356 LOAD_FAST                0 (self)
                            358 LOAD_ATTR               11 (player2)
                            368 LOAD_FAST                0 (self)
                            370 STORE_ATTR               9 (current_player)
                            380 LOAD_CONST               0 (None)
                            382 RETURN_VALUE
                
-                78     >>  384 LOAD_FAST                0 (self)
+               101     >>  384 LOAD_FAST                0 (self)
                            386 LOAD_ATTR               10 (player1)
                            396 LOAD_FAST                0 (self)
                            398 STORE_ATTR               9 (current_player)
                            408 LOAD_CONST               0 (None)
                            410 RETURN_VALUE
                consts
                   None
@@ -574,94 +683,94 @@
                   ' as origin, but there is already origin piece '
                names      ('hand', 'Exception', 'is_double', 'has_crossing', 'closed', 'pop', 'origin', 'append', 'score', 'current_player', 'player1', 'player2')
                varnames   ('self', 'player', 'piece', 'origin', 'close')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'play'
-               firstlineno 57
+               firstlineno 80
                lnotab
                   0x02011201260220010e02340204010e0114010cff140210022a01280220
                   011c02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970067005300
-                80           0 RESUME                   0
+               103           0 RESUME                   0
                
-                81           2 BUILD_LIST               0
+               104           2 BUILD_LIST               0
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'hand')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'valid_options'
-               firstlineno 80
+               firstlineno 103
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d017c01811c7c00a001000000000000000000
                   00000000000000000000007c006a0200000000000000007c016400a60300
                   00ab0300000000000000000100090009008c02
-                83           0 RESUME                   0
+               106           0 RESUME                   0
                
-                84           2 LOAD_FAST                0 (self)
+               107           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_required_starting_piece)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               1 (starting_piece)
                
-                85          42 LOAD_FAST                1 (starting_piece)
+               108          42 LOAD_FAST                1 (starting_piece)
                             44 POP_JUMP_FORWARD_IF_NONE    28 (to 102)
                
-                86          46 LOAD_FAST                0 (self)
+               109          46 LOAD_FAST                0 (self)
                             48 LOAD_METHOD              1 (play)
                             70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (current_player)
                             82 LOAD_FAST                1 (starting_piece)
                             84 LOAD_CONST               0 (None)
                             86 PRECALL                  3
                             90 CALL                     3
                            100 POP_TOP
                
-                88     >>  102 NOP
+               111     >>  102 NOP
                
-                89     >>  104 NOP
+               112     >>  104 NOP
                
-                88         106 JUMP_BACKWARD            2 (to 104)
+               111         106 JUMP_BACKWARD            2 (to 104)
                consts
                   None
                names      ('get_required_starting_piece', 'play', 'current_player')
                varnames   ('self', 'starting_piece')
                freevars   ()
                cellvars   ()
                filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
                name       'run'
-               firstlineno 83
+               firstlineno 106
                lnotab 0x0201280104013802020102ff
             (28,)
             (False,)
-         names      ('__name__', '__module__', '__qualname__', 'Union', '__init__', 'deal_hand', 'get_required_starting_piece', 'staticmethod', 'Piece', 'score_piece', 'score', 'Player', 'play', 'valid_options', 'run')
+         names      ('__name__', '__module__', '__qualname__', 'Union', '__init__', 'deal_hand', 'get_required_starting_piece', 'staticmethod', 'Piece', 'int', 'score_piece', 'score', 'Player', 'play', 'valid_options', 'run')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
          name       'DominoRound'
          firstlineno 7
-         lnotab 0x0a0120080606061602010cff0e010208060426170603
+         lnotab 0x0a01200806060616020110ff0e01021f060426170603
       'DominoRound'
       None
    names      ('typing', 'Union', 'List', 'Tuple', 'src.main.game.Piece', 'domino_set', 'Piece', 'src.main.player.Player', 'Player', 'DominoRound')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/root/informanthik-runner/_work/all-fives-domino/all-fives-domino/src/main/game/DominoRound.py'
```

### Comparing `all-fives-domino-1.0.7/src/main/game/__pycache__/Piece.cpython-311.pyc` & `all-fives-domino-1.0.8/src/main/game/__pycache__/Piece.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/main/player/Hand.py` & `all-fives-domino-1.0.8/src/main/player/Hand.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/main/player/__pycache__/Hand.cpython-311.pyc` & `all-fives-domino-1.0.8/src/main/player/__pycache__/Hand.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/main/player/__pycache__/Player.cpython-311.pyc` & `all-fives-domino-1.0.8/src/main/player/__pycache__/Player.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.8/src/test/game/__pycache__/test_pieces.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.8/src/test/game/__pycache__/test_round.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/test/game/test_pieces.py` & `all-fives-domino-1.0.8/src/test/game/test_pieces.py`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc` & `all-fives-domino-1.0.8/src/test/player/__pycache__/test_hand.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `all-fives-domino-1.0.7/src/test/player/test_hand.py` & `all-fives-domino-1.0.8/src/test/player/test_hand.py`

 * *Files identical despite different names*

