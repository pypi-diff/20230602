# Comparing `tmp/triessentials-0.1.5.tar.gz` & `tmp/triessentials-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triessentials-0.1.5.tar", max compression
+gzip compressed data, was "triessentials-0.1.6.tar", max compression
```

## Comparing `triessentials-0.1.5.tar` & `triessentials-0.1.6.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      362 2023-05-30 02:11:42.538767 triessentials-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      318 2023-05-30 02:11:35.650783 triessentials-0.1.5/triessentials/__init__.py
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-06-02 16:03:23.405359 triessentials-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-06-02 16:03:03.361378 triessentials-0.1.6/triessentials/__init__.py
+-rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.6/PKG-INFO
```

