# Comparing `tmp/hh_ui_check-0.1.0.tar.gz` & `tmp/hh_ui_check-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hh_ui_check-0.1.0.tar", max compression
+gzip compressed data, was "hh_ui_check-0.1.1.tar", max compression
```

## Comparing `hh_ui_check-0.1.0.tar` & `hh_ui_check-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424825 hh_ui_check-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.0/hh_ui_check/__init__.py
--rw-r--r--   0        0        0     3709 2023-06-02 03:11:51.900039 hh_ui_check-0.1.0/hh_ui_check/diff.py
--rw-r--r--   0        0        0     2088 2023-06-02 03:11:51.915520 hh_ui_check-0.1.0/hh_ui_check/hist_compare.py
--rw-r--r--   0        0        0      479 2023-06-02 03:11:51.921769 hh_ui_check-0.1.0/hh_ui_check/horizen.py
--rw-r--r--   0        0        0      597 2023-06-02 03:11:51.926405 hh_ui_check-0.1.0/hh_ui_check/main.py
--rw-r--r--   0        0        0      583 2023-06-02 03:11:51.937183 hh_ui_check-0.1.0/hh_ui_check/overlapping.py
--rw-r--r--   0        0        0      447 2023-06-02 03:11:51.942201 hh_ui_check-0.1.0/hh_ui_check/substract.py
--rw-r--r--   0        0        0      382 2023-06-02 03:11:53.883775 hh_ui_check-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 hh_ui_check-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424825 hh_ui_check-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 03:09:39.424775 hh_ui_check-0.1.1/hh_ui_check/__init__.py
+-rw-r--r--   0        0        0     3709 2023-06-02 03:11:51.900039 hh_ui_check-0.1.1/hh_ui_check/diff.py
+-rw-r--r--   0        0        0     2088 2023-06-02 03:11:51.915520 hh_ui_check-0.1.1/hh_ui_check/hist_compare.py
+-rw-r--r--   0        0        0      479 2023-06-02 03:11:51.921769 hh_ui_check-0.1.1/hh_ui_check/horizen.py
+-rwxr-xr-x   0        0        0      620 2023-06-02 04:58:30.868371 hh_ui_check-0.1.1/hh_ui_check/main.py
+-rw-r--r--   0        0        0      583 2023-06-02 03:11:51.937183 hh_ui_check-0.1.1/hh_ui_check/overlapping.py
+-rw-r--r--   0        0        0      447 2023-06-02 03:11:51.942201 hh_ui_check-0.1.1/hh_ui_check/substract.py
+-rw-r--r--   0        0        0      382 2023-06-02 04:59:51.769302 hh_ui_check-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 hh_ui_check-0.1.1/PKG-INFO
```

### Comparing `hh_ui_check-0.1.0/hh_ui_check/diff.py` & `hh_ui_check-0.1.1/hh_ui_check/diff.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.0/hh_ui_check/hist_compare.py` & `hh_ui_check-0.1.1/hh_ui_check/hist_compare.py`

 * *Files identical despite different names*

### Comparing `hh_ui_check-0.1.0/hh_ui_check/main.py` & `hh_ui_check-0.1.1/hh_ui_check/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import sys
 import os
 import cv2
 import numpy as np
 
 from horizen import getHorizen
 from substract import getSubstract
```

### Comparing `hh_ui_check-0.1.0/hh_ui_check/overlapping.py` & `hh_ui_check-0.1.1/hh_ui_check/overlapping.py`

 * *Files identical despite different names*

