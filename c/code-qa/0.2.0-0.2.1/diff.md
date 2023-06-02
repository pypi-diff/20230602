# Comparing `tmp/code_qa-0.2.0.tar.gz` & `tmp/code_qa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_qa-0.2.0.tar", max compression
+gzip compressed data, was "code_qa-0.2.1.tar", max compression
```

## Comparing `code_qa-0.2.0.tar` & `code_qa-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.2.0/LICENSE
--rw-r--r--   0        0        0      830 2023-06-01 13:56:57.750398 code_qa-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.2.0/code_qa/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-01 13:30:54.044136 code_qa-0.2.0/code_qa/cli.py
--rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.2.0/code_qa/logger.py
--rw-r--r--   0        0        0     1149 2023-06-01 13:56:57.755987 code_qa-0.2.0/code_qa/utils.py
--rw-r--r--   0        0        0      484 2023-06-01 13:57:02.643554 code_qa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1711 1970-01-01 00:00:00.000000 code_qa-0.2.0/setup.py
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 code_qa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-01 11:29:07.858435 code_qa-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2148 2023-06-02 04:27:10.766067 code_qa-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 11:28:22.025812 code_qa-0.2.1/code_qa/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-01 13:30:54.044136 code_qa-0.2.1/code_qa/cli.py
+-rw-r--r--   0        0        0      167 2023-06-01 11:57:41.557031 code_qa-0.2.1/code_qa/logger.py
+-rw-r--r--   0        0        0     1149 2023-06-02 02:24:31.211012 code_qa-0.2.1/code_qa/utils.py
+-rw-r--r--   0        0        0      583 2023-06-02 04:27:16.934517 code_qa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3141 1970-01-01 00:00:00.000000 code_qa-0.2.1/setup.py
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 code_qa-0.2.1/PKG-INFO
```

### Comparing `code_qa-0.2.0/LICENSE` & `code_qa-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_qa-0.2.0/code_qa/cli.py` & `code_qa-0.2.1/code_qa/cli.py`

 * *Files identical despite different names*

### Comparing `code_qa-0.2.0/code_qa/utils.py` & `code_qa-0.2.1/code_qa/utils.py`

 * *Files identical despite different names*

