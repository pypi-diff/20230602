# Comparing `tmp/triessentials-0.1.6.tar.gz` & `tmp/triessentials-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triessentials-0.1.6.tar", max compression
+gzip compressed data, was "triessentials-0.1.7.tar", max compression
```

## Comparing `triessentials-0.1.6.tar` & `triessentials-0.1.7.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      362 2023-06-02 16:03:23.405359 triessentials-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      369 2023-06-02 16:03:03.361378 triessentials-0.1.6/triessentials/__init__.py
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-06-02 16:08:43.658699 triessentials-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-06-02 16:08:54.622683 triessentials-0.1.7/triessentials/__init__.py
+-rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.7/PKG-INFO
```

