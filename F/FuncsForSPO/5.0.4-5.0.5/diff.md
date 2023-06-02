# Comparing `tmp/FuncsForSPO-5.0.4.tar.gz` & `tmp/FuncsForSPO-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.0.4.tar", last modified: Fri Jun  2 20:08:30 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.0.5.tar", last modified: Fri Jun  2 20:13:53 2023, max compression
```

## Comparing `FuncsForSPO-5.0.4.tar` & `FuncsForSPO-5.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.870268 FuncsForSPO-5.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.335844 FuncsForSPO-5.0.4/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.436758 FuncsForSPO-5.0.4/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.4/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.4/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.472470 FuncsForSPO-5.0.4/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.4/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.485262 FuncsForSPO-5.0.4/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.4/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.498744 FuncsForSPO-5.0.4/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.505632 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.557013 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     3066 2023-06-02 19:46:45.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3541 2023-06-02 19:10:17.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1134 2023-06-02 19:53:39.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.581829 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.601375 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.610288 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.633363 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.654658 FuncsForSPO-5.0.4/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.667310 FuncsForSPO-5.0.4/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.4/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.683695 FuncsForSPO-5.0.4/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.4/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.697453 FuncsForSPO-5.0.4/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.4/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.718643 FuncsForSPO-5.0.4/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.4/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.4/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.731529 FuncsForSPO-5.0.4/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.4/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.4/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.738539 FuncsForSPO-5.0.4/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.4/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-02 20:08:30.423246 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-02 20:08:30.000000 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1520 2023-06-02 20:08:30.000000 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 20:08:30.000000 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-02 20:08:30.000000 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      377 2023-06-02 20:08:30.000000 FuncsForSPO-5.0.4/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.4/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-02 20:08:30.864700 FuncsForSPO-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 20:08:30.871270 FuncsForSPO-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2297 2023-06-02 20:08:21.000000 FuncsForSPO-5.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:53.153635 FuncsForSPO-5.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.234872 FuncsForSPO-5.0.5/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.328451 FuncsForSPO-5.0.5/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.0.5/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.0.5/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.358932 FuncsForSPO-5.0.5/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.0.5/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.405375 FuncsForSPO-5.0.5/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.0.5/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.425457 FuncsForSPO-5.0.5/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.0.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.436624 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.472015 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-06-02 20:13:06.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3541 2023-06-02 19:10:17.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.514708 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9269 2023-02-23 17:57:32.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1599 2022-11-17 11:12:03.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.547374 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.559757 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.606330 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9692 2023-02-23 17:58:42.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5052 2023-05-29 21:06:22.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.628872 FuncsForSPO-5.0.5/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.663841 FuncsForSPO-5.0.5/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    68328 2023-05-26 14:44:35.000000 FuncsForSPO-5.0.5/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.702240 FuncsForSPO-5.0.5/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.0.5/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.738525 FuncsForSPO-5.0.5/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39076 2023-05-11 16:23:08.000000 FuncsForSPO-5.0.5/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.778071 FuncsForSPO-5.0.5/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.0.5/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.0.5/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.813485 FuncsForSPO-5.0.5/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.0.5/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.0.5/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.837524 FuncsForSPO-5.0.5/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.0.5/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 20:13:52.310272 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-02 20:13:51.000000 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1520 2023-06-02 20:13:52.000000 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 20:13:51.000000 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-06-02 20:13:51.000000 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      377 2023-06-02 20:13:51.000000 FuncsForSPO-5.0.5/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.0.5/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-02 20:13:53.136072 FuncsForSPO-5.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 20:13:53.154743 FuncsForSPO-5.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2297 2023-06-02 20:13:45.000000 FuncsForSPO-5.0.5/setup.py
```

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.0.5/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
 https://pdf.ai/
 
 Esse robô envia o PDF para o site https://pdf.ai/
     e recupera um arquivo txt com a resposta do GPT
 """
+from FuncsForSPO.fpdf.fanalyser.base import *
+
 class ErroPDFAIException(Exception):
     pass
 
-from FuncsForSPO.fgpt.pdfanalyser.base import *
-
 class GPTPDF(Bot):    
     def __init__(self, file_pdf: str, credentials:tuple, prompt:str, headless: bool=True) -> str:
         self.PDF_PATH = os.path.abspath(file_pdf)
         self.PROMPT = prompt
         self.HEADLESS = headless
         self.CREDENTIALS = credentials
         super().__init__(self.HEADLESS)
```

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from FuncsForSPO.fgpt.pdfanalyser.__pdfanalyser import *
+from FuncsForSPO.fpdf.fanalyser.__pdfanalyser import *
 
 def analyse_pdf_with_gpt(file_pdf:str, prompt:str, credentials:tuple, headless=True) -> str:
     """
     DIREITOS RESERVADOS / RIGHTS RESERVED / DERECHOS RESERVADOS
 
     https://pdf.ai/
```

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.0.5/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.0.5/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.0.5/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.4
+Version: 5.0.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.4/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.0.5/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/LICENSE` & `FuncsForSPO-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/PKG-INFO` & `FuncsForSPO-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.0.4
+Version: 5.0.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.0.4/README.md` & `FuncsForSPO-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.0.4/setup.py` & `FuncsForSPO-5.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.0.4'
+version = '5.0.5'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
```

