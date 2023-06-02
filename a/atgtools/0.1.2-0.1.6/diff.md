# Comparing `tmp/atgtools-0.1.2.tar.gz` & `tmp/atgtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atgtools-0.1.2.tar", max compression
+gzip compressed data, was "atgtools-0.1.6.tar", max compression
```

## Comparing `atgtools-0.1.2.tar` & `atgtools-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,14 @@
--rw-r--r--   0        0        0       22 2022-06-01 13:52:33.288798 atgtools-0.1.2/atgtools/__init__.py
--rw-r--r--   0        0        0     3049 2022-06-01 14:02:33.681867 atgtools-0.1.2/atgtools/atg.py
--rw-r--r--   0        0        0     1029 2022-06-01 13:47:37.250506 atgtools-0.1.2/atgtools/richard.py
--rw-r--r--   0        0        0      405 2022-03-31 12:15:37.597087 atgtools-0.1.2/atgtools/theme.ini
--rw-r--r--   0        0        0      392 2022-06-01 14:05:24.113651 atgtools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      724 2022-06-01 14:06:35.959982 atgtools-0.1.2/setup.py
--rw-r--r--   0        0        0      401 2022-06-01 14:06:35.960187 atgtools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-12-27 20:34:28.449518 atgtools-0.1.6/LICENSE
+-rw-r--r--   0        0        0       42 2023-01-13 00:12:49.053646 atgtools-0.1.6/atg/__init__.py
+-rw-r--r--   0        0        0       40 2022-12-27 21:26:29.838677 atgtools-0.1.6/atg/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-27 21:30:01.611243 atgtools-0.1.6/atg/commands/__init__.py
+-rw-r--r--   0        0        0     1001 2023-06-02 05:48:05.206587 atgtools-0.1.6/atg/commands/app.py
+-rw-r--r--   0        0        0        0 2023-01-02 21:05:25.738793 atgtools-0.1.6/atg/commands/lefse/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-30 07:51:50.960928 atgtools-0.1.6/atg/commands/lefse/app.py
+-rw-r--r--   0        0        0      116 2023-05-30 08:03:12.772845 atgtools-0.1.6/atg/commands/lefse/lefse.py
+-rw-r--r--   0        0        0        0 2022-12-27 21:56:20.186577 atgtools-0.1.6/atg/commands/tools/__init__.py
+-rw-r--r--   0        0        0     2029 2023-05-30 12:17:15.709029 atgtools-0.1.6/atg/commands/tools/app.py
+-rw-r--r--   0        0        0     1690 2023-05-30 11:43:19.857717 atgtools-0.1.6/atg/commands/tools/manifest.py
+-rw-r--r--   0        0        0     1137 2023-06-02 05:48:16.619082 atgtools-0.1.6/atg/utils.py
+-rw-r--r--   0        0        0      526 2023-06-02 05:48:33.555038 atgtools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 atgtools-0.1.6/PKG-INFO
```

