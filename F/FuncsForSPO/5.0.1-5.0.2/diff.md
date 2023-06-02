# Comparing `tmp/FuncsForSPO-5.0.1.tar.gz` & `tmp/FuncsForSPO-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.0.1.tar", last modified: Fri Jun  2 19:59:20 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.0.2.tar", last modified: Fri Jun  2 20:02:08 2023, max compression
```

## Comparing `FuncsForSPO-5.0.1.tar` & `FuncsForSPO-5.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.379192 FuncsForSPO-5.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.303745 FuncsForSPO-5.0.1/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.415459 FuncsForSPO-5.0.1/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.1/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.1/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.441959 FuncsForSPO-5.0.1/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.1/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.468141 FuncsForSPO-5.0.1/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.1/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.224914 FuncsForSPO-5.0.1/FuncsForSPO/fgpt/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.641578 FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/
--rw-rw-rw-   0        0        0     3066 2023-06-02 19:46:45.000000 FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3541 2023-06-02 19:10:17.000000 FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/base.py
--rw-rw-rw-   0        0        0     1134 2023-06-02 19:53:39.000000 FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.699048 FuncsForSPO-5.0.1/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.254887 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.775870 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.824789 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.845481 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.918906 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.960316 FuncsForSPO-5.0.1/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.993458 FuncsForSPO-5.0.1/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.1/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.045891 FuncsForSPO-5.0.1/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.1/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.073785 FuncsForSPO-5.0.1/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.1/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.120325 FuncsForSPO-5.0.1/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.1/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.1/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.153831 FuncsForSPO-5.0.1/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.1/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.1/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:20.171283 FuncsForSPO-5.0.1/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.1/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 19:59:19.396162 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-02 19:59:18.000000 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1458 2023-06-02 19:59:19.000000 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 19:59:18.000000 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-02 19:59:18.000000 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      396 2023-06-02 19:59:18.000000 FuncsForSPO-5.0.1/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.1/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-02 19:59:20.371474 FuncsForSPO-5.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 19:59:20.383196 FuncsForSPO-5.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2291 2023-06-02 19:58:56.000000 FuncsForSPO-5.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.713035 FuncsForSPO-5.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.128139 FuncsForSPO-5.0.2/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.196207 FuncsForSPO-5.0.2/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.2/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.2/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.211251 FuncsForSPO-5.0.2/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.2/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.223380 FuncsForSPO-5.0.2/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.2/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.114204 FuncsForSPO-5.0.2/FuncsForSPO/fgpt/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.253370 FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/
+-rw-rw-rw-   0        0        0     3066 2023-06-02 19:46:45.000000 FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3541 2023-06-02 19:10:17.000000 FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/base.py
+-rw-rw-rw-   0        0        0     1134 2023-06-02 19:53:39.000000 FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.267011 FuncsForSPO-5.0.2/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.120692 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.298504 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.319046 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.326056 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.350111 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.366194 FuncsForSPO-5.0.2/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.383161 FuncsForSPO-5.0.2/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.2/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.403328 FuncsForSPO-5.0.2/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.2/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.487868 FuncsForSPO-5.0.2/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.2/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.564176 FuncsForSPO-5.0.2/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.2/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.2/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.591624 FuncsForSPO-5.0.2/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.2/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.2/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.617940 FuncsForSPO-5.0.2/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.2/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:02:08.181059 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-02 20:02:07.000000 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2023-06-02 20:02:08.000000 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:02:07.000000 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-02 20:02:07.000000 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      396 2023-06-02 20:02:07.000000 FuncsForSPO-5.0.2/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.2/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-02 20:02:08.703353 FuncsForSPO-5.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:02:08.714010 FuncsForSPO-5.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2291 2023-06-02 20:02:02.000000 FuncsForSPO-5.0.2/setup.py
```

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.0.2/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/base.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.0.2/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.0.2/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.0.2/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.1
+Version: 5.0.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.1/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.0.2/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/LICENSE` & `FuncsForSPO-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/PKG-INFO` & `FuncsForSPO-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.1
+Version: 5.0.2
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.1/README.md` & `FuncsForSPO-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.1/setup.py` & `FuncsForSPO-5.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.0.1'
+version = '5.0.2'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

