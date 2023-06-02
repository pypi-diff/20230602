# Comparing `tmp/FuncsForSPO-4.44.2.tar.gz` & `tmp/FuncsForSPO-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-4.44.2.tar", last modified: Thu Jun  1 11:59:18 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.0.0.tar", last modified: Fri Jun  2 19:56:09 2023, max compression
```

## Comparing `FuncsForSPO-4.44.2.tar` & `FuncsForSPO-5.0.0.tar`

### file list

```diff
@@ -1,60 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.416564 FuncsForSPO-4.44.2/
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:17.941861 FuncsForSPO-4.44.2/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.044283 FuncsForSPO-4.44.2/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-4.44.2/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-4.44.2/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.059910 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.076741 FuncsForSPO-4.44.2/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-4.44.2/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.091910 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:17.931086 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.114232 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.147309 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.158227 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.182931 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9918 2023-06-01 11:55:59.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.202973 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.253542 FuncsForSPO-4.44.2/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-4.44.2/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.275635 FuncsForSPO-4.44.2/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-4.44.2/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.291670 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-4.44.2/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.309305 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.324150 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.336515 FuncsForSPO-4.44.2/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-4.44.2/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:59:18.020959 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8027 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1331 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      350 2023-06-01 11:59:17.000000 FuncsForSPO-4.44.2/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-4.44.2/LICENSE
--rw-rw-rw-   0        0        0     8027 2023-06-01 11:59:18.411051 FuncsForSPO-4.44.2/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-4.44.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-01 11:59:18.417569 FuncsForSPO-4.44.2/setup.cfg
--rw-rw-rw-   0        0        0     2177 2023-06-01 11:59:05.000000 FuncsForSPO-4.44.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.812399 FuncsForSPO-5.0.0/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.172320 FuncsForSPO-5.0.0/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.278449 FuncsForSPO-5.0.0/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.0/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.0/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.309569 FuncsForSPO-5.0.0/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.0/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.327627 FuncsForSPO-5.0.0/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.0/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.149250 FuncsForSPO-5.0.0/FuncsForSPO/fgpt/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.365887 FuncsForSPO-5.0.0/FuncsForSPO/fgpt/pdfanalyser/
+-rw-rw-rw-   0        0        0     3066 2023-06-02 19:46:45.000000 FuncsForSPO-5.0.0/FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3541 2023-06-02 19:10:17.000000 FuncsForSPO-5.0.0/FuncsForSPO/fgpt/pdfanalyser/base.py
+-rw-rw-rw-   0        0        0     1134 2023-06-02 19:53:39.000000 FuncsForSPO-5.0.0/FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.384687 FuncsForSPO-5.0.0/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.159582 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.416505 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.448218 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.460776 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.500811 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.523471 FuncsForSPO-5.0.0/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.546460 FuncsForSPO-5.0.0/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.0/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.571473 FuncsForSPO-5.0.0/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.0/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.593863 FuncsForSPO-5.0.0/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.0/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.616308 FuncsForSPO-5.0.0/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.0/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.0/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.636586 FuncsForSPO-5.0.0/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.0/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.0/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.650248 FuncsForSPO-5.0.0/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.0/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:56:09.259136 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-02 19:56:08.000000 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1458 2023-06-02 19:56:08.000000 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:56:08.000000 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-02 19:56:08.000000 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      379 2023-06-02 19:56:08.000000 FuncsForSPO-5.0.0/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.0/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-02 19:56:09.803378 FuncsForSPO-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:56:09.813907 FuncsForSPO-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2241 2023-06-02 19:55:49.000000 FuncsForSPO-5.0.0/setup.py
```

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.0.0/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,27 +177,24 @@
                         else:
                             wait=False
                             sleep(3)
                             if prints:
                                 print('OCR Concluido!')
             verifica_se_baixou_o_arquivo(self.DOWNLOAD_DIR, '.txt')            
         except Exception as e:
-            self.DRIVER.quit()
-            faz_log(f'Ocorreu um erro: {repr(e)}', 'c*')
-
+            print('Ocorreu um erro!')
+            print(str(e))
+            
 
+            
     def recupera_texto(self) -> str:
-        try:
-            if self.get_text_into_code:
-                try:
-                    file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
-                    file_txt = file_txts[-1]
-                    text = None
-                    with open(file_txt, mode='r', encoding='utf-16-le') as f:
-                        text = f.read()
-                    shutil.rmtree(self.DOWNLOAD_DIR)
-                    return text
-                except IndexError:
-                    raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
-        except Exception:
-            self.DRIVER.quit()
-            raise FalhaAoRecuperarOcr(f'Ocorreu um erro na recuperação que causou um Exception: {repr(e)}')
+        if self.get_text_into_code:
+            try:
+                file_txts = arquivos_com_caminho_absoluto_do_arquivo(self.DOWNLOAD_DIR)
+                file_txt = file_txts[-1]
+                text = None
+                with open(file_txt, mode='r', encoding='utf-16-le') as f:
+                    text = f.read()
+                shutil.rmtree(self.DOWNLOAD_DIR)
+                return text
+            except IndexError:
+                raise FalhaAoRecuperarOcr('Ocorreu um erro na recuperação que causou um IndexError, provavelmente não baixou o arquivo.')
```

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.0.0/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.0.0/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.0.0/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.44.2
+Version: 5.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.44.2/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.0.0/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 FuncsForSPO.egg-info/top_level.txt
 FuncsForSPO/femails/__init__.py
 FuncsForSPO/femails/femails.py
 FuncsForSPO/fexceptions/__init__.py
 FuncsForSPO/fexceptions/exceptions.py
 FuncsForSPO/fftp/__init__.py
 FuncsForSPO/fftp/fftp.py
+FuncsForSPO/fgpt/pdfanalyser/__pdfanalyser.py
+FuncsForSPO/fgpt/pdfanalyser/base.py
+FuncsForSPO/fgpt/pdfanalyser/pdfanalyser.py
 FuncsForSPO/fopenpyxl/__init__.py
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
 FuncsForSPO/fpdf/fcompress/__compress_online.py
 FuncsForSPO/fpdf/fcompress/__init__.py
 FuncsForSPO/fpdf/fcompress/compress.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
```

### Comparing `FuncsForSPO-4.44.2/LICENSE` & `FuncsForSPO-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/PKG-INFO` & `FuncsForSPO-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 4.44.2
+Version: 5.0.0
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-4.44.2/README.md` & `FuncsForSPO-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-4.44.2/setup.py` & `FuncsForSPO-5.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '4.44.2'
+version = '5.0.0'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -18,14 +18,15 @@
         description=u'Funções Para Melhorar Desenvolvimento de Robôs com Selenium',
         
         packages= [
             os.path.join('FuncsForSPO', 'femails'),
             os.path.join('FuncsForSPO', 'fexceptions'),
             os.path.join('FuncsForSPO', 'fftp'),
             os.path.join('FuncsForSPO', 'fpdf'),
+            os.path.join('FuncsForSPO', 'fgpt', 'pdfanalyser'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'fcompress'),
             os.path.join('FuncsForSPO', 'fpdf', 'fimgpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'fhtml_to_pdf'),
             os.path.join('FuncsForSPO', 'fopenpyxl'),
             os.path.join('FuncsForSPO', 'fpysimplegui'),
             os.path.join('FuncsForSPO', 'fpython'),
```

