# Comparing `tmp/honeybee-doe2-0.4.2.tar.gz` & `tmp/honeybee-doe2-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.4.2.tar", last modified: Fri May 26 01:07:28 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.4.3.tar", last modified: Fri Jun  2 14:56:59 2023, max compression
```

## Comparing `honeybee-doe2-0.4.2.tar` & `honeybee-doe2-0.4.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 01:07:28.000000 honeybee-doe2-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 01:06:33.000000 honeybee-doe2-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 14:56:59.000000 honeybee-doe2-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 14:56:03.000000 honeybee-doe2-0.4.3/setup.py
```

### Comparing `honeybee-doe2-0.4.2/LICENSE` & `honeybee-doe2-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/PKG-INFO` & `honeybee-doe2-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.4.2/README.md` & `honeybee-doe2-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.4.3/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.4.3/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.4.3/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/story.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         inp_obj = '\n"{self.display_name}"= FLOOR'.format(self=self) + \
             "\n   SHAPE           = POLYGON" + \
             '\n   POLYGON         = "Level_{self.story_no} Plg"'.format(self=self) + \
             '\n   AZIMUTH         = {}'.format(azimuth) + \
             '\n   X               = {}'.format(origin_pt.x) + \
             '\n   Y               = {}'.format(origin_pt.y) + \
             '\n   Z               = {}'.format(origin_pt.z) + \
-            '\n   SPACE-HEIGHT    = {self.space_height}'.format(self=self) + \
+            '\n   SPACE-HEIGHT    = {self.floor_to_floor_height}'.format(self=self) + \
             '\n   FLOOR-HEIGHT    = {self.floor_to_floor_height}'.format(self=self) + \
             '\n   ..\n'
         nl = '\n'
 
         return inp_obj + nl.join(str('\n'+f) for f in room_objs)
 
     def __repr__(self):
```

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.4.3/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.4.3/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.4.3/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2/writer.py` & `honeybee-doe2-0.4.3/honeybee_doe2/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,34 +48,35 @@
                     '..', '_')
 
             for ap in face.apertures:
                 ap.display_name = short_name(
                     clean_and_id_string(ap.display_name)).replace(
                     '..', '_')
 
-    window_constructions = [GlassType.from_hb_window_constr(
-        generic_construction_set.aperture_set.window_construction)]
+    window_constructions = [generic_construction_set.aperture_set.window_construction]
 
     for construction in hb_model.properties.energy.constructions:
         if isinstance(construction, WindowConstruction):
-            window_constructions.append(GlassType.from_hb_window_constr(construction))
+            window_constructions.append(construction)
+    wind_con_set = set(window_constructions)
+    win_con_to_inp = [GlassType.from_hb_window_constr(constr) for constr in wind_con_set]
 
     data = [
         hb_model.properties.doe2._header,
         fb.global_params,
         fb.ttrpddh,
         Title(title=str(hb_model.display_name)).to_inp(),
         rp.to_inp(),  # TODO unhardcode
         fb.comply,
         comp_data.to_inp(),
         sb_data.to_inp(),
         fb.mats_layers,
         hb_model.properties.doe2.mats_cons_layers,
         fb.glzCode,
-        '\n'.join(gt.to_inp() for gt in window_constructions),
+        '\n'.join(gt.to_inp() for gt in win_con_to_inp),
         fb.polygons,
         '\n'.join(s.story_poly for s in hb_model.properties.doe2.stories),
         fb.wallParams,
         hb_model.properties.doe2.fixed_shades,
         fb.miscCost,
         fb.perfCurve,
         fb.floorNspace,
```

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.4.3/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.4.2
+Version: 0.4.3
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.4.2/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.4.3/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.4.2/setup.py` & `honeybee-doe2-0.4.3/setup.py`

 * *Files identical despite different names*

