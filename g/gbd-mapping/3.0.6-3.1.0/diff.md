# Comparing `tmp/gbd_mapping-3.0.6.tar.gz` & `tmp/gbd_mapping-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbd_mapping-3.0.6.tar", last modified: Tue Jul  5 20:47:37 2022, max compression
+gzip compressed data, was "gbd_mapping-3.1.0.tar", last modified: Thu Jun  1 23:20:50 2023, max compression
```

## Comparing `gbd_mapping-3.0.6.tar` & `gbd_mapping-3.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2655 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3267 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.399568 gbd_mapping-3.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.399568 gbd_mapping-3.0.6/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.399568 gbd_mapping-3.0.6/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     7649 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/gbd_mapping.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/gbd_mapping_generator.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.395568 gbd_mapping-3.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.403568 gbd_mapping-3.0.6/src/gbd_mapping/
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15212 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/base_template.py
--rw-r--r--   0 runner    (1001) docker     (121)   421863 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/cause.py
--rw-r--r--   0 runner    (1001) docker     (121)    42887 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/cause_template.py
--rw-r--r--   0 runner    (1001) docker     (121)   403799 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/covariate.py
--rw-r--r--   0 runner    (1001) docker     (121)   282616 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/covariate_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     2451 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/etiology.py
--rw-r--r--   0 runner    (1001) docker     (121)     2895 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/etiology_template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/id.py
--rw-r--r--   0 runner    (1001) docker     (121)   223458 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/risk_factor.py
--rw-r--r--   0 runner    (1001) docker     (121)    18704 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/risk_factor_template.py
--rw-r--r--   0 runner    (1001) docker     (121)   761067 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/sequela.py
--rw-r--r--   0 runner    (1001) docker     (121)   441749 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping/sequela_template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-05 20:47:37.000000 gbd_mapping-3.0.6/src/gbd_mapping.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/src/gbd_mapping_generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/base_template_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/build_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/cause_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/covariate_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    15512 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2199 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/etiology_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/globals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/id_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6611 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/risk_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/sequela_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     9631 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/src/gbd_mapping_generator/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-05 20:47:37.407568 gbd_mapping-3.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-05 20:47:27.000000 gbd_mapping-3.0.6/tests/test_gbd_mapping_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.234713 gbd_mapping-3.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.238713 gbd_mapping-3.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.238713 gbd_mapping-3.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/gbd_mapping.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/gbd_mapping_generator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.234713 gbd_mapping-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.242713 gbd_mapping-3.1.0/src/gbd_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   421863 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42887 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/cause_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   403799 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   282616 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/covariate_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/etiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/etiology_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223458 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/risk_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18704 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/risk_factor_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)   761067 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/sequela.py
+-rw-r--r--   0 runner    (1001) docker     (123)   441749 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping/sequela_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.242713 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 23:20:50.000000 gbd_mapping-3.1.0/src/gbd_mapping.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/src/gbd_mapping_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/base_template_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/build_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/cause_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/covariate_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/etiology_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/id_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/risk_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/sequela_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/src/gbd_mapping_generator/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:50.246713 gbd_mapping-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 23:20:35.000000 gbd_mapping-3.1.0/tests/test_gbd_mapping_generator.py
```

### Comparing `gbd_mapping-3.0.6/CHANGELOG.rst` & `gbd_mapping-3.1.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+**3.1.0 - 06/01/23**
+
+ - Update vivarium_gbd_access pin 
+ - Support Python 3.8-3.11 
+ - Update git actions to remove warnings
+
 **3.0.6 - 07/05/22**
 
  - Add CODEOWNERS
 
 **3.0.5 - 05/05/22**
 
  - Fix black and click dependency conflict in CI.
```

### Comparing `gbd_mapping-3.0.6/CODE_OF_CONDUCT.rst` & `gbd_mapping-3.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/CONTRIBUTING.rst` & `gbd_mapping-3.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/LICENSE.txt` & `gbd_mapping-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/PKG-INFO` & `gbd_mapping-3.1.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,58 @@
-Metadata-Version: 2.1
-Name: gbd_mapping
-Version: 3.0.6
-Summary: A programmatically accessible mapping of gbd entities.
-Home-page: https://github.com/ihmeuw/gbd_mapping
-Author: The vivarium developers
-Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: GBD Mapping
-        ===========
-        
-        .. image:: https://badge.fury.io/py/gbd-mapping.svg
-            :target: https://badge.fury.io/py/gbd-mapping
-        
-        .. image:: https://travis-ci.org/ihmeuw/gbd_mapping.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/gbd_mapping
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/gbd_mapping/badge/?version=latest
-            :target: https://gbd_mapping.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        Mapping of Global Burden of Disease (GBD) entities to their metadata.
-        
-        There are two packages offered in this distribution.  The first, the ``gbd_mapping_generator``
-        is a set of scripts that define templates and data gathering code used to produce the second, the ``gbd_mapping``.
-        The ``gbd_mapping_generator`` package will not function without access to the IHME cluster and some of our
-        internally used data access libraries. Mapping updates are managed by an automated toolchain, so this shouldn't
-        be an issue.
-        
-        The ``gbd_mapping`` is a programmatically accessible (and TAB-complete-able) set of mappings for GBD entities
-        including:
-        
-         - Causes
-         - Risks
-         - Covariates
-         - Etiologies
-         - Sequelae
-        
-        You can install ``gbd_mapping`` from PyPI with pip:
-        
-          ``> pip install gbd_mapping``
-        
-        or build it from source with
-        
-          ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
-        
-          ``> cd gbd_mapping``
-        
-          ``> pip install .``
-        
-        
-        Development and Mapping Generation
-        ++++++++++++++++++++++++++++++++++
-        
-        In order to generate or regenerate the mappings from data, you must have access to
-        the Institute for Health Metrics and Evaluation cluster and internal PyPI server.
-        Contact <collijk@uw.edu> if you need further instructions on that.
-        
-        Given proper permissions, you can set up this library in development mode with
-        
-            ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
-        
-            ``> cd gbd_mapping``
-        
-            ``> pip install -e .['dev']``
-        
-Platform: UNKNOWN
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: data
-Provides-Extra: dev
+GBD Mapping
+===========
+
+.. image:: https://badge.fury.io/py/gbd-mapping.svg
+    :target: https://badge.fury.io/py/gbd-mapping
+
+.. image:: https://travis-ci.org/ihmeuw/gbd_mapping.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/gbd_mapping
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/gbd_mapping/badge/?version=latest
+    :target: https://gbd_mapping.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+Mapping of Global Burden of Disease (GBD) entities to their metadata.
+
+There are two packages offered in this distribution.  The first, the ``gbd_mapping_generator``
+is a set of scripts that define templates and data gathering code used to produce the second, the ``gbd_mapping``.
+The ``gbd_mapping_generator`` package will not function without access to the IHME cluster and some of our
+internally used data access libraries. Mapping updates are managed by an automated toolchain, so this shouldn't
+be an issue.
+
+The ``gbd_mapping`` is a programmatically accessible (and TAB-complete-able) set of mappings for GBD entities
+including:
+
+ - Causes
+ - Risks
+ - Covariates
+ - Etiologies
+ - Sequelae
+
+You can install ``gbd_mapping`` from PyPI with pip:
+
+  ``> pip install gbd_mapping``
+
+or build it from source with
+
+  ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
+
+  ``> cd gbd_mapping``
+
+  ``> pip install .``
+
+
+Development and Mapping Generation
+++++++++++++++++++++++++++++++++++
+
+In order to generate or regenerate the mappings from data, you must have access to
+the Institute for Health Metrics and Evaluation cluster and internal PyPI server.
+Contact <collijk@uw.edu> if you need further instructions on that.
+
+Given proper permissions, you can set up this library in development mode with
+
+    ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
+
+    ``> cd gbd_mapping``
+
+    ``> pip install -e .['dev']``
```

### Comparing `gbd_mapping-3.0.6/README.rst` & `gbd_mapping-3.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: gbd_mapping
+Version: 3.1.0
+Summary: A programmatically accessible mapping of gbd entities.
+Home-page: https://github.com/ihmeuw/gbd_mapping
+Author: The vivarium developers
+Author-email: vivarium.dev@gmail.com
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: data
+Provides-Extra: dev
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
 GBD Mapping
 ===========
 
 .. image:: https://badge.fury.io/py/gbd-mapping.svg
     :target: https://badge.fury.io/py/gbd-mapping
 
 .. image:: https://travis-ci.org/ihmeuw/gbd_mapping.svg?branch=master
```

### Comparing `gbd_mapping-3.0.6/docs/Makefile` & `gbd_mapping-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/docs/source/conf.py` & `gbd_mapping-3.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/docs/source/gbd_mapping.rst` & `gbd_mapping-3.1.0/docs/source/gbd_mapping.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/docs/source/gbd_mapping_generator.rst` & `gbd_mapping-3.1.0/docs/source/gbd_mapping_generator.rst`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/setup.py` & `gbd_mapping-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "click",
         "numpy",
         "pandas",
         "pyyaml",
     ]
 
     data_requires = [
-        "vivarium-gbd-access>=3.0.5",
+        "vivarium-gbd-access>=3.0.7",
     ]
 
     test_requirements = [
         "pytest",
         "pytest-mock",
     ]
```

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/base_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/base_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/cause.py` & `gbd_mapping-3.1.0/src/gbd_mapping/cause.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/cause_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/cause_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/covariate.py` & `gbd_mapping-3.1.0/src/gbd_mapping/covariate.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/covariate_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/covariate_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/etiology.py` & `gbd_mapping-3.1.0/src/gbd_mapping/etiology.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/etiology_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/etiology_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/id.py` & `gbd_mapping-3.1.0/src/gbd_mapping/id.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/risk_factor.py` & `gbd_mapping-3.1.0/src/gbd_mapping/risk_factor.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/risk_factor_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/risk_factor_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/sequela.py` & `gbd_mapping-3.1.0/src/gbd_mapping/sequela.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping/sequela_template.py` & `gbd_mapping-3.1.0/src/gbd_mapping/sequela_template.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping.egg-info/PKG-INFO` & `gbd_mapping-3.1.0/src/gbd_mapping.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 Metadata-Version: 2.1
 Name: gbd-mapping
-Version: 3.0.6
+Version: 3.1.0
 Summary: A programmatically accessible mapping of gbd entities.
 Home-page: https://github.com/ihmeuw/gbd_mapping
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
-License: UNKNOWN
-Description: GBD Mapping
-        ===========
-        
-        .. image:: https://badge.fury.io/py/gbd-mapping.svg
-            :target: https://badge.fury.io/py/gbd-mapping
-        
-        .. image:: https://travis-ci.org/ihmeuw/gbd_mapping.svg?branch=master
-            :target: https://travis-ci.org/ihmeuw/gbd_mapping
-            :alt: Latest Version
-        
-        .. image:: https://readthedocs.org/projects/gbd_mapping/badge/?version=latest
-            :target: https://gbd_mapping.readthedocs.io/en/latest/?badge=latest
-            :alt: Latest Docs
-        
-        Mapping of Global Burden of Disease (GBD) entities to their metadata.
-        
-        There are two packages offered in this distribution.  The first, the ``gbd_mapping_generator``
-        is a set of scripts that define templates and data gathering code used to produce the second, the ``gbd_mapping``.
-        The ``gbd_mapping_generator`` package will not function without access to the IHME cluster and some of our
-        internally used data access libraries. Mapping updates are managed by an automated toolchain, so this shouldn't
-        be an issue.
-        
-        The ``gbd_mapping`` is a programmatically accessible (and TAB-complete-able) set of mappings for GBD entities
-        including:
-        
-         - Causes
-         - Risks
-         - Covariates
-         - Etiologies
-         - Sequelae
-        
-        You can install ``gbd_mapping`` from PyPI with pip:
-        
-          ``> pip install gbd_mapping``
-        
-        or build it from source with
-        
-          ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
-        
-          ``> cd gbd_mapping``
-        
-          ``> pip install .``
-        
-        
-        Development and Mapping Generation
-        ++++++++++++++++++++++++++++++++++
-        
-        In order to generate or regenerate the mappings from data, you must have access to
-        the Institute for Health Metrics and Evaluation cluster and internal PyPI server.
-        Contact <collijk@uw.edu> if you need further instructions on that.
-        
-        Given proper permissions, you can set up this library in development mode with
-        
-            ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
-        
-            ``> cd gbd_mapping``
-        
-            ``> pip install -e .['dev']``
-        
-Platform: UNKNOWN
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: data
 Provides-Extra: dev
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+GBD Mapping
+===========
+
+.. image:: https://badge.fury.io/py/gbd-mapping.svg
+    :target: https://badge.fury.io/py/gbd-mapping
+
+.. image:: https://travis-ci.org/ihmeuw/gbd_mapping.svg?branch=master
+    :target: https://travis-ci.org/ihmeuw/gbd_mapping
+    :alt: Latest Version
+
+.. image:: https://readthedocs.org/projects/gbd_mapping/badge/?version=latest
+    :target: https://gbd_mapping.readthedocs.io/en/latest/?badge=latest
+    :alt: Latest Docs
+
+Mapping of Global Burden of Disease (GBD) entities to their metadata.
+
+There are two packages offered in this distribution.  The first, the ``gbd_mapping_generator``
+is a set of scripts that define templates and data gathering code used to produce the second, the ``gbd_mapping``.
+The ``gbd_mapping_generator`` package will not function without access to the IHME cluster and some of our
+internally used data access libraries. Mapping updates are managed by an automated toolchain, so this shouldn't
+be an issue.
+
+The ``gbd_mapping`` is a programmatically accessible (and TAB-complete-able) set of mappings for GBD entities
+including:
+
+ - Causes
+ - Risks
+ - Covariates
+ - Etiologies
+ - Sequelae
+
+You can install ``gbd_mapping`` from PyPI with pip:
+
+  ``> pip install gbd_mapping``
+
+or build it from source with
+
+  ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
+
+  ``> cd gbd_mapping``
+
+  ``> pip install .``
+
+
+Development and Mapping Generation
+++++++++++++++++++++++++++++++++++
+
+In order to generate or regenerate the mappings from data, you must have access to
+the Institute for Health Metrics and Evaluation cluster and internal PyPI server.
+Contact <collijk@uw.edu> if you need further instructions on that.
+
+Given proper permissions, you can set up this library in development mode with
+
+    ``> git clone https://github.com/ihmeuw/gbd_mapping.git``
+
+    ``> cd gbd_mapping``
+
+    ``> pip install -e .['dev']``
```

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping.egg-info/SOURCES.txt` & `gbd_mapping-3.1.0/src/gbd_mapping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/base_template_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/base_template_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/build_mapping.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/build_mapping.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/cause_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/cause_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/covariate_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/covariate_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/data.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/data.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/etiology_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/etiology_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/id_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/id_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/risk_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/risk_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/sequela_builder.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/sequela_builder.py`

 * *Files identical despite different names*

### Comparing `gbd_mapping-3.0.6/src/gbd_mapping_generator/util.py` & `gbd_mapping-3.1.0/src/gbd_mapping_generator/util.py`

 * *Files identical despite different names*

