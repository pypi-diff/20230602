# Comparing `tmp/markdown_gds-0.3.0.tar.gz` & `tmp/markdown_gds-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_gds-0.3.0.tar", max compression
+gzip compressed data, was "markdown_gds-0.4.0.tar", max compression
```

## Comparing `markdown_gds-0.3.0.tar` & `markdown_gds-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1091 2022-08-05 13:56:44.101531 markdown_gds-0.3.0/LICENSE
--rw-r--r--   0        0        0       36 2022-08-05 11:40:52.963385 markdown_gds-0.3.0/markdown_gds/__init__.py
--rw-r--r--   0        0        0     1412 2023-04-27 12:34:46.359257 markdown_gds-0.3.0/markdown_gds/extension.py
--rw-r--r--   0        0        0      411 2023-04-27 12:43:57.563866 markdown_gds-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 markdown_gds-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-08-05 13:56:44.101531 markdown_gds-0.4.0/LICENSE
+-rw-r--r--   0        0        0       36 2022-08-05 11:40:52.963385 markdown_gds-0.4.0/markdown_gds/__init__.py
+-rw-r--r--   0        0        0     1902 2023-06-02 13:59:51.139183 markdown_gds-0.4.0/markdown_gds/extension.py
+-rw-r--r--   0        0        0      411 2023-06-02 14:00:05.386291 markdown_gds-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 markdown_gds-0.4.0/PKG-INFO
```

### Comparing `markdown_gds-0.3.0/LICENSE` & `markdown_gds-0.4.0/LICENSE`

 * *Files identical despite different names*

