# Comparing `tmp/FuncsForSPO-5.0.7.tar.gz` & `tmp/FuncsForSPO-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.0.7.tar", last modified: Fri Jun  2 21:24:32 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.0.8.tar", last modified: Fri Jun  2 21:31:22 2023, max compression
```

## Comparing `FuncsForSPO-5.0.7.tar` & `FuncsForSPO-5.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.720553 FuncsForSPO-5.0.7/
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.060608 FuncsForSPO-5.0.7/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.179158 FuncsForSPO-5.0.7/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.7/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.7/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.207353 FuncsForSPO-5.0.7/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.7/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.225397 FuncsForSPO-5.0.7/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.7/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.255823 FuncsForSPO-5.0.7/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.271205 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.318913 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     3848 2023-06-02 21:22:25.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3545 2023-06-02 20:31:43.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.348866 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.387167 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.398580 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.430726 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.453353 FuncsForSPO-5.0.7/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.476282 FuncsForSPO-5.0.7/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.7/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.498188 FuncsForSPO-5.0.7/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.7/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.517264 FuncsForSPO-5.0.7/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.7/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.539076 FuncsForSPO-5.0.7/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.7/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.7/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.556129 FuncsForSPO-5.0.7/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.7/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.7/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.567375 FuncsForSPO-5.0.7/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.7/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 21:24:32.160040 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-02 21:24:31.000000 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1520 2023-06-02 21:24:31.000000 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 21:24:31.000000 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-02 21:24:31.000000 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      377 2023-06-02 21:24:31.000000 FuncsForSPO-5.0.7/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.7/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-02 21:24:32.709534 FuncsForSPO-5.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 21:24:32.721564 FuncsForSPO-5.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2297 2023-06-02 21:24:23.000000 FuncsForSPO-5.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:22.342812 FuncsForSPO-5.0.8/
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:20.642508 FuncsForSPO-5.0.8/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.126243 FuncsForSPO-5.0.8/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.8/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.8/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.257372 FuncsForSPO-5.0.8/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.8/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.341183 FuncsForSPO-5.0.8/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.8/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.387292 FuncsForSPO-5.0.8/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.8/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.409109 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.606193 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     3992 2023-06-02 21:30:55.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3545 2023-06-02 20:31:43.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.654483 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.718556 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.738608 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.806689 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.855454 FuncsForSPO-5.0.8/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.912678 FuncsForSPO-5.0.8/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.8/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.960935 FuncsForSPO-5.0.8/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.8/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.998112 FuncsForSPO-5.0.8/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.8/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:22.047683 FuncsForSPO-5.0.8/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.8/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.8/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:22.109284 FuncsForSPO-5.0.8/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.8/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.8/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:22.131777 FuncsForSPO-5.0.8/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.8/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:31:21.080157 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-02 21:31:18.000000 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1520 2023-06-02 21:31:19.000000 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 21:31:18.000000 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-02 21:31:18.000000 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      377 2023-06-02 21:31:18.000000 FuncsForSPO-5.0.8/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.8/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-02 21:31:22.332293 FuncsForSPO-5.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 21:31:22.344325 FuncsForSPO-5.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2297 2023-06-02 21:31:07.000000 FuncsForSPO-5.0.8/setup.py
```

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.0.8/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
                 espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'button[data-octo-click="oauth_application_authorization"]'))
             except (NoSuchElementException, TimeoutException):
                 pass
             
 
             while True:
                 try:
+                    faz_log('Limpando documentos anteriores')
                     elements = espera_e_retorna_lista_de_elementos(self.WDW3, (By.CSS_SELECTOR, 'tbody>tr>td:last-child>button'))
                     for i in elements:
                         i.click()
                         espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'h3~div>button'))
                         espera_elemento_sair_do_dom(self.WDW, (By.CSS_SELECTOR, 'h3~div>button'))
                         break
                 except (NoSuchElementException, TimeoutException):
@@ -54,18 +55,20 @@
             except (NoSuchElementException, TimeoutException):
                 pass
 
             espera_input_limpa_e_envia_send_keys(self.WDW30, 'Coloque no inicio da sua resposta: "IA" e me responda em português. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]'))
             espera_elemento_disponivel_e_clica(self.WDW30, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]~button'))
 
             while True:
+                faz_log('Aguardando resposta...')
                 text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, '#__next main>div~div>div~div>div>div>div>div~div'))
                 if 'IA' in text:
                     break
                 else:
+                    sleep(2)
                     continue
             self.DRIVER.get('https://pdf.ai/documents')
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'tbody>tr>td:last-child>button'))
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'h3~div>button'))
             sleep(.5)
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'a[href="/auth/account"]~button'))
             self.DRIVER.quit()
```

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.0.8/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.0.8/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.0.8/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.7
+Version: 5.0.8
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.7/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.0.8/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/LICENSE` & `FuncsForSPO-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/PKG-INFO` & `FuncsForSPO-5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.7
+Version: 5.0.8
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.7/README.md` & `FuncsForSPO-5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.7/setup.py` & `FuncsForSPO-5.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.0.7'
+version = '5.0.8'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

