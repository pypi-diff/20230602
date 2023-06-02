# Comparing `tmp/peakrdl-html-2.8.0.tar.gz` & `tmp/peakrdl-html-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-html-2.8.0.tar", last modified: Mon Sep 19 04:04:58 2022, max compression
+gzip compressed data, was "peakrdl-html-2.9.0.tar", last modified: Fri Oct  7 04:39:32 2022, max compression
```

## Comparing `peakrdl-html-2.8.0.tar` & `peakrdl-html-2.9.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.361953 peakrdl-html-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1875 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/LICENSE-3RD-PARTY
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-09-19 04:04:58.361953 peakrdl-html-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-19 04:04:58.361953 peakrdl-html-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.341953 peakrdl-html-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.341953 peakrdl-html-2.8.0/src/peakrdl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.341953 peakrdl-html-2.8.0/src/peakrdl/html/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl/html/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.345953 peakrdl-html-2.8.0/src/peakrdl_html/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/__peakrdl__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19790 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     9127 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/search_indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.345953 peakrdl-html-2.8.0/src/peakrdl_html/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.341953 peakrdl-html-2.8.0/src/peakrdl_html/static/.launcher_data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.345953 peakrdl-html-2.8.0/src/peakrdl_html/static/.launcher_data/firefox/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/.launcher_data/firefox/user.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.345953 peakrdl-html-2.8.0/src/peakrdl_html/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/css/layout.css
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/css/normalize.css
--rw-r--r--   0 runner    (1001) docker     (121)    21251 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.341953 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.349953 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/
--rw-r--r--   0 runner    (1001) docker     (121)    40576 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (121)   142267 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (121)    40348 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (121)    14868 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   180720 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (121)   680510 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (121)   180500 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    86876 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (121)    67400 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.357953 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (121)   256056 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.eot
--rw-r--r--   0 runner    (1001) docker     (121)   600856 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   309728 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)   184912 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   266158 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.eot
--rw-r--r--   0 runner    (1001) docker     (121)   622572 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   323344 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   193308 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   268604 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.eot
--rw-r--r--   0 runner    (1001) docker     (121)   639388 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   328412 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff
--rw-r--r--   0 runner    (1001) docker     (121)   195704 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (121)   253461 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)   607720 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   309192 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)   182708 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.357953 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/
--rw-r--r--   0 runner    (1001) docker     (121)    79520 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-r--r--   0 runner    (1001) docker     (121)   170616 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    87624 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-r--r--   0 runner    (1001) docker     (121)    67312 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (121)    78331 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-r--r--   0 runner    (1001) docker     (121)   169064 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (121)    86288 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-r--r--   0 runner    (1001) docker     (121)    66444 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.361953 peakrdl-html-2.8.0/src/peakrdl_html/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    31948 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/BigInteger.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/address_search.js
--rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/content_search.js
--rw-r--r--   0 runner    (1001) docker     (121)     6697 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/field_testers.js
--rw-r--r--   0 runner    (1001) docker     (121)     4800 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/index_edit.js
--rw-r--r--   0 runner    (1001) docker     (121)    12440 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/main.js
--rw-r--r--   0 runner    (1001) docker     (121)     6182 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/nav.js
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/path_search.js
--rw-r--r--   0 runner    (1001) docker     (121)    12931 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/ral.js
--rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/search.js
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/sha1.js
--rw-r--r--   0 runner    (1001) docker     (121)     8331 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/js/sidebar.js
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-chrome.bat
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-edge.bat
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-firefox.bat
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.361953 peakrdl-html-2.8.0/src/peakrdl_html/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/addrmap.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/addrmap_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1782 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/field_description.html
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/group-like.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (121)     6955 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/index_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/mem.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/mem_base.html
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/reg.html
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/reg_base.html
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/regfile.html
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-19 04:04:57.000000 peakrdl-html-2.8.0/src/peakrdl_html/templates/regfile_base.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-19 04:04:58.345953 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3940 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-19 04:04:58.000000 peakrdl-html-2.8.0/src/peakrdl_html.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.044162 peakrdl-html-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1753 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/LICENSE-3RD-PARTY
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-10-07 04:39:32.044162 peakrdl-html-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3175 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-07 04:39:32.044162 peakrdl-html-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.028162 peakrdl-html-2.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.028162 peakrdl-html-2.9.0/src/peakrdl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.028162 peakrdl-html-2.9.0/src/peakrdl/html/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl/html/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      677 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1323 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/__peakrdl__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    20409 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9127 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/search_indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.028162 peakrdl-html-2.9.0/src/peakrdl_html/static/.launcher_data/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html/static/.launcher_data/firefox/
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/.launcher_data/firefox/user.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     2992 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/css/layout.css
+-rw-r--r--   0 runner    (1001) docker     (121)     6052 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/css/normalize.css
+-rw-r--r--   0 runner    (1001) docker     (121)    22327 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.028162 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/
+-rw-r--r--   0 runner    (1001) docker     (121)    40576 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   142267 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    40348 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    18168 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    14868 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   180720 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   680510 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (121)   180500 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    86876 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    67400 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.040162 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/
+-rw-r--r--   0 runner    (1001) docker     (121)   256056 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   600856 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   309728 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   184912 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   266158 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   622572 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   323344 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   193308 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   268604 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   639388 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   328412 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   195704 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)   253461 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   607720 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   309192 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (121)   182708 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.040162 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/
+-rw-r--r--   0 runner    (1001) docker     (121)    79520 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   170616 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    87624 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    67312 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (121)    78331 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (121)   169064 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)    86288 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (121)    66444 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.044162 peakrdl-html-2.9.0/src/peakrdl_html/static/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/address_search.js
+-rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/content_search.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6640 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/field_testers.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4768 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/index_edit.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14624 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (121)     6007 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/nav.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/path_search.js
+-rw-r--r--   0 runner    (1001) docker     (121)    29990 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/progressbar.min.js
+-rw-r--r--   0 runner    (1001) docker     (121)    14529 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/ral.js
+-rw-r--r--   0 runner    (1001) docker     (121)     7789 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/search.js
+-rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/sha1.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9256 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/js/sidebar.js
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-chrome.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-edge.bat
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-firefox.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.044162 peakrdl-html-2.9.0/src/peakrdl_html/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/addrmap.html
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/addrmap_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/field_description.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/group-like.html
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7124 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/index_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/mem.html
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/mem_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/reg.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/reg_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/regfile.html
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html/templates/regfile_base.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 04:39:32.032162 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5168 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-10-07 04:39:32.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-10-07 04:39:31.000000 peakrdl-html-2.9.0/src/peakrdl_html.egg-info/top_level.txt
```

### Comparing `peakrdl-html-2.8.0/LICENSE` & `peakrdl-html-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/PKG-INFO` & `peakrdl-html-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-html
-Version: 2.8.0
+Version: 2.9.0
 Summary: HTML documentation generator for SystemRDL-based register models
 Home-page: https://github.com/SystemRDL/PeakRDL-html
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-html
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-html/issues
```

### Comparing `peakrdl-html-2.8.0/README.md` & `peakrdl-html-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/setup.py` & `peakrdl-html-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl/html/__init__.py` & `peakrdl-html-2.9.0/src/peakrdl/html/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/__peakrdl__.py` & `peakrdl-html-2.9.0/src/peakrdl_html/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/exporter.py` & `peakrdl-html-2.9.0/src/peakrdl_html/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             List of properties to explicitly document.
             Nodes that have a property explicitly set will show its value in a
             table in the node's description.
             Use this to bring forward user-defined properties, or other built-in
             properties in your documentation.
         """
         self.output_dir = "" # type: str
-        self.RALIndex = [] # type: List[Dict[str, Any]]
+        self.RALData = [] # type: List[Dict[str, Any]]
         self.RootNodeIds = [] # type: List[int]
         self.current_id = -1
         self.footer = "" # type: str
         self.title = "" # type: str
         self.home_url = None # type: Optional[str]
         self.skip_not_present = True
 
@@ -149,39 +149,40 @@
         self.skip_not_present = kwargs.pop("skip_not_present", True) # type: ignore
 
         # Check for stray kwargs
         if kwargs:
             raise TypeError("got an unexpected keyword argument '%s'" % list(kwargs.keys())[0])
 
         self.output_dir = output_dir
-        self.RALIndex = []
+        self.RALData = []
         self.current_id = -1
         self.indexer = SearchIndexer()
 
         # Copy static files
         static_dir = os.path.join(os.path.dirname(__file__), "static")
         distutils.dir_util.copy_tree(static_dir, self.output_dir, preserve_mode=0, preserve_times=0)
         if self.user_static_dir:
             distutils.dir_util.copy_tree(self.user_static_dir, self.output_dir, preserve_mode=0, preserve_times=0)
 
         # Make sure output directory structure exists
         os.makedirs(self.output_dir, exist_ok=True)
         os.makedirs(os.path.join(self.output_dir, "content"), exist_ok=True)
         os.makedirs(os.path.join(self.output_dir, "search"), exist_ok=True)
+        os.makedirs(os.path.join(self.output_dir, "data"), exist_ok=True)
 
         # Traverse trees
         for node in nodes:
             if node.get_property('bridge'):
                 node.env.msg.warning(
                     "HTML generator does not have proper support for bridge addmaps yet. The 'bridge' property will be ignored.",
                     node.inst.property_src_ref.get('bridge', node.inst.inst_src_ref)
                 )
             self.visit_addressable_node(node)
 
-        # Write out RALIndex and other data to js file
+        # Write out RALData and other data
         self.write_ral_data()
 
         # Write main index.html
         self.write_index_page()
 
         # Write search index
         self.indexer.write_index_js(os.path.join(output_dir, "search"))
@@ -231,15 +232,15 @@
                     ral_field['disp'] = 'E'
 
                 ral_fields.append(ral_field)
 
             ral_entry['fields'] = ral_fields
 
         # Insert entry now to ensure proper position in list
-        self.RALIndex.append(ral_entry)
+        self.RALData.append(ral_entry)
 
         # Insert root nodes to list
         if parent_id is None:
             self.RootNodeIds.append(this_id)
 
         # Recurse to children
         children = OrderedDict()
@@ -253,30 +254,41 @@
         # Generate page for this node
         self.write_page(this_id, node, children)
 
         return this_id
 
 
     def write_ral_data(self) -> None:
+        N_RAL_NODES_PER_FILE = 16384
+        n_files = math.ceil(len(self.RALData)/N_RAL_NODES_PER_FILE)
+
+        # Write data index
         PageInfo = {
             "title" : self.title
         }
-        path = os.path.join(self.output_dir, "js/data.js")
-        with open(path, 'w', encoding='utf-8') as fp:
-            fp.write("var RALIndex = ")
-            fp.write(PeakRDLJSEncoder(separators=(',', ':')).encode(self.RALIndex))
-            fp.write(";\n")
-
-            fp.write("var RootNodeIds = ")
-            fp.write(PeakRDLJSEncoder(separators=(',', ':')).encode(self.RootNodeIds))
-            fp.write(";\n")
-
-            fp.write("var PageInfo = ")
-            fp.write(PeakRDLJSEncoder(separators=(',', ':')).encode(PageInfo))
-            fp.write(";\n")
+        path = os.path.join(self.output_dir, "data/data_index.js")
+        with open(path, 'w', encoding='utf-8') as f:
+            f.write("var N_RAL_FILES = %d;\n" % n_files)
+            f.write("var N_RAL_NODES_PER_FILE = %d;\n" % N_RAL_NODES_PER_FILE)
+
+            f.write("var RootNodeIds = ")
+            f.write(PeakRDLJSEncoder(separators=(',', ':')).encode(self.RootNodeIds))
+            f.write(";\n")
+
+            f.write("var PageInfo = ")
+            f.write(PeakRDLJSEncoder(separators=(',', ':')).encode(PageInfo))
+            f.write(";\n")
+
+        # Write RALData files
+        for file_idx in range(n_files):
+            start = file_idx * N_RAL_NODES_PER_FILE
+            end = min((file_idx + 1) * N_RAL_NODES_PER_FILE, len(self.RALData))
+            path = os.path.join(self.output_dir, "data/ral-data-%d.json" % file_idx)
+            with open(path, 'w', encoding='utf-8') as f:
+                f.write(PeakRDLJSEncoder(separators=(',', ':')).encode(self.RALData[start:end]))
 
 
     _template_map = {
         AddrmapNode : "addrmap.html",
         RegfileNode : "regfile.html",
         MemNode     : "mem.html",
         RegNode     : "reg.html",
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/search_indexer.py` & `peakrdl-html-2.9.0/src/peakrdl_html/search_indexer.py`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/css/layout.css` & `peakrdl-html-2.9.0/src/peakrdl_html/static/css/layout.css`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,18 @@
     width: 4.375em;
 }
 
 .crumb-idx {
     cursor:pointer;
 }
 
+#_AbsAddr div {
+    cursor: pointer;
+}
+
 #_SearchResults{
     margin: 0em;
 }
 
 #_SearchResults li{
     cursor:pointer;
     overflow: hidden;
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/css/normalize.css` & `peakrdl-html-2.9.0/src/peakrdl_html/static/css/normalize.css`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/css/theme.css` & `peakrdl-html-2.9.0/src/peakrdl_html/static/css/theme.css`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     --title-bg-color-hover: #2e8ece;
     --alt-row-bg-color:#f3f6f6;
     --inline-code-block-bg-color: #fff;
     --code-block-bg-color: #efc;
     --input-bg-color: #fff;
     --input-invalid-bg-color: #f99;
     --highlight-color: #f1c40f;
+    --progressbar-color: #f1c40f;
 
     --content-border-color: #e1e4e5;
     --strong-content-border-color: #aaa;
     --blockquote-bar-color: #ccc;
 
     --button-border-color: #949494;
     --button-text-color: #4c4c4c;
@@ -86,14 +87,15 @@
         --title-bg-color-hover: #2e8ece;
         --alt-row-bg-color:#222;
         --inline-code-block-bg-color: #111;
         --code-block-bg-color: #2a301f;
         --input-bg-color: #000;
         --input-invalid-bg-color: #A33;
         --highlight-color: #7e6500;
+        --progressbar-color: #7e6500;
 
         --content-border-color: #444;
         --strong-content-border-color: #555;
         --blockquote-bar-color: #444;
 
         --button-border-color: #6c6c6c;
         --button-text-color: #999;
@@ -273,14 +275,33 @@
     background-color: var(--highlight-color)!important;
 }
 
 mark {
     background-color: var(--highlight-color);
 }
 
+#_ProgressBar {
+    width: 15em;
+    margin: auto;
+}
+
+#_ProgressBar path {
+    stroke: var(--strong-content-border-color);
+    stroke-width: 3;
+}
+
+#_ProgressBar path + path {
+    stroke: var(--progressbar-color);
+    stroke-width: 8;
+}
+
+.progressbar-text {
+    color: var(--main-text-color)!important;
+}
+
 /* ------------------------------- Admonitions ------------------------------ */
 .admonition-title:before {
     font-family: "Font Awesome 5 Free";
     font-weight: bold;
     content: "\f06a";
     margin-right:4px;
 }
@@ -426,28 +447,29 @@
 }
 
 #_SBResizer:hover {
     background-color: rgba(128, 128, 128, 0.5);
 }
 
 .sb-button-strip {
-    padding: 0em 0.313em;
+    padding: 0em 0.3em 0.3em 0.3em;
 }
 
 .sb-button-strip button, .sb-button-strip a.button-link{
     background-color: inherit;
     background-image: none;
     border: none;
     width: 1.25em;
     height: 1.25em;
     font-size: 1.5em;
     text-align: center;
     vertical-align: middle;
     color: var(--title-text-color);
     padding: 0em;
+    border-radius: 3px;
 }
 
 .sb-button-strip button:hover, .sb-button-strip a.button-link:hover{
     color: var(--title-text-color-hover);
     background-color: var(--title-bg-color-hover);
     border: none;
 }
@@ -584,14 +606,56 @@
 }
 
 .node-info dd {
   grid-column: 2;
   margin-left: 0.5em;
 }
 
+#_AbsAddr div {
+    display: inline;
+    visibility: hidden;
+    color: var(--url-color);
+    margin-left: 1em;
+}
+#_AbsAddr div:hover {
+    color: var(--url-color-hover);
+}
+
+#_AbsAddr:hover div {
+    visibility: visible;
+}
+
+#_AbsAddr div::after {
+    font-family: "Font Awesome 5 Free";
+    font-weight: bold;
+    content: "\f05a";
+}
+
+div#_AbsAddrDetails {
+    display: none;
+    grid-column: 2;
+    margin-left: 0.5em;
+    border-left: solid 0.313em var(--blockquote-bar-color);
+    padding-left: 0.5em;
+}
+
+div#_AbsAddrDetails.open {
+    display: grid;
+}
+
+#_AbsAddrDetails dt{
+  grid-column: 1;
+}
+
+#_AbsAddrDetails dd {
+  grid-column: 2;
+  margin-left: 0.5em;
+}
+
+
 input.field-value-tester {
     border: solid 1px var(--strong-content-border-color);
     padding: 0.25em 0.5em;
     width: 9em;
 }
 
 select.field-value-enum-tester {
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/favicon.png` & `peakrdl-html-2.9.0/src/peakrdl_html/static/favicon.png`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.svg` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.svg` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/FontAwesome/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-bolditalic.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-italic.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/Lato/lato-regular.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.eot` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.eot`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2` & `peakrdl-html-2.9.0/src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/address_search.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/address_search.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -4,20 +4,20 @@
 class AddressSearch {
     static start(query) {
         query = query.slice(1, query.length);
         if (query == "") return;
 
         var addr;
         try {
-            addr = toBigInt(query);
+            addr = BigInt(query);
         } catch (error) {
-            addr = bigInt(-1);
+            addr = -1n;
         }
 
-        if (addr.lt(0)) return;
+        if (addr < 0) return;
 
         RootNodeIds.forEach(function(id) {
             var result = RAL.lookup_by_address(addr, id);
             if (result != null) {
                 var result_id = result[0];
                 var idx_stack = result[1];
                 var text_segments = [RAL.get_path(result_id, idx_stack)];
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/content_search.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/content_search.js`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/field_testers.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/field_testers.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 }
 
 function save_reg_state() {
     var addr_key = RAL.get_absolute_addr(CurrentID).toString(16);
     var reg_el = document.getElementById("_RegValueTester");
 
     var state = {};
-    state.value = toBigInt(reg_el.value);
+    state.value = BigInt(reg_el.value);
     state = userHooks.save_extra_reg_state(state)
     RegValueRegistery[addr_key] = state;
 }
 
 function get_reg_state() {
     var addr_key = RAL.get_absolute_addr(CurrentID).toString(16);
     if (addr_key in RegValueRegistery) {
@@ -66,41 +66,41 @@
         update_field_value_tester(i);
     }
     userHooks.onRegValueEditorChange();
 }
 
 function update_reg_value_tester() {
     // Update the register tester input based on all of the individual field inputs
-    var reg_value = bigInt(0);
+    var reg_value = 0n;
     var node = RAL.get_node(CurrentID);
     for (var i = 0; i < node.fields.length; i++) {
-        var msb = node.fields[i].msb;
-        var lsb = node.fields[i].lsb;
+        var msb = BigInt(node.fields[i].msb);
+        var lsb = BigInt(node.fields[i].lsb);
         var el = document.getElementById("_FieldValueTester" + node.fields[i].name);
-        var value = toBigInt(el.value);
-        var mask = bigInt(1).shiftLeft(msb - lsb + 1).subtract(1);
-        value = value.and(mask);
-        reg_value = reg_value.add(value.shiftLeft(lsb));
+        var value = BigInt(el.value);
+        var mask = (1n << (msb - lsb + 1n)) - 1n;
+        value = value & mask;
+        reg_value = reg_value + (value << lsb);
     }
     var reg_el = document.getElementById("_RegValueTester");
     reg_el.value = "0x" + reg_value.toString(16);
     reg_el.classList.remove("invalid");
     userHooks.onRegValueEditorChange();
 }
 
 function update_field_value_tester(idx) {
     var reg_el = document.getElementById("_RegValueTester");
-    var reg_value = toBigInt(reg_el.value);
+    var reg_value = BigInt(reg_el.value);
     var node = RAL.get_node(CurrentID);
 
-    var msb = node.fields[idx].msb;
-    var lsb = node.fields[idx].lsb;
-    var value = reg_value.shiftRight(lsb);
-    var mask = bigInt(1).shiftLeft(msb - lsb + 1).subtract(1);
-    value = value.and(mask);
+    var msb = BigInt(node.fields[idx].msb);
+    var lsb = BigInt(node.fields[idx].lsb);
+    var value = reg_value >> lsb;
+    var mask = (1n << (msb - lsb + 1n)) - 1n;
+    value = value & mask;
     var el = document.getElementById("_FieldValueTester" + node.fields[idx].name);
     el.value = format_field_value(idx, value);
     el.classList.remove("invalid");
 
     if ("encode" in RAL.get_node(CurrentID).fields[idx]) {
         var el = document.getElementById("_FieldValueEnumTester" + node.fields[idx].name);
         el.value = "0x" + value.toString(16);
@@ -161,26 +161,26 @@
     update_reg_value_tester();
     save_reg_state();
 }
 
 function onDecodedFieldInput(el) {
     var idx = RAL.lookup_field_idx(el.dataset.name);
     var node = RAL.get_node(CurrentID);
-    var msb = node.fields[idx].msb;
-    var lsb = node.fields[idx].lsb;
+    var msb = BigInt(node.fields[idx].msb);
+    var lsb = BigInt(node.fields[idx].lsb);
     var value;
 
     try {
-        value = toBigInt(el.value);
+        value = BigInt(el.value);
     } catch (error) {
-        value = bigInt(-1);
+        value = -1n;
     }
 
-    var max_value = bigInt(1).shiftLeft(msb - lsb + 1);
-    if (value.lt(0) || (value.geq(max_value))) {
+    var max_value = 1n << (msb - lsb + 1n);
+    if ((value < 0) || (value >= max_value)) {
         if (!el.classList.contains("invalid")) el.classList.add("invalid");
         return;
     }
     el.classList.remove("invalid");
 
     if ("encode" in node.fields[idx]) {
         var el2 = document.getElementById("_FieldValueEnumTester" + node.fields[idx].name);
@@ -189,20 +189,20 @@
     update_reg_value_tester();
     save_reg_state();
 }
 
 function onEncodedRegInput(el) {
     var value;
     try {
-        value = toBigInt(el.value);
+        value = BigInt(el.value);
     } catch (error) {
-        value = bigInt(-1);
+        value = -1n;
     }
 
-    if (value.lt(0)) {
+    if (value < 0) {
         if (!el.classList.contains("invalid")) el.classList.add("invalid");
         return;
     }
     el.classList.remove("invalid");
     update_field_value_testers();
     save_reg_state();
 }
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/index_edit.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/index_edit.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,15 +51,15 @@
             if (!isPositiveInteger(val)) return;
             if ((val < 0) || (val >= RAL.get_node(IndexEditState.id).dims[IndexEditState.dim])) return;
             RAL.get_node(IndexEditState.id).idxs[IndexEditState.dim] = val;
 
             update_crumbtrail();
             update_rdlfc_indexes();
             patch_url_path();
-            update_absolute_addr(RAL.get_absolute_addr(CurrentID));
+            update_absolute_addr();
             if (RAL.is_register(CurrentID)) {
                 init_reg_value();
             }
             userHooks.onAddressUpdate();
         }
     }
 }
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/main.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/main.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -43,30 +43,38 @@
         show_incompatibility_nag();
         return;
     }
 
     window.onpopstate = onPopState;
     window.onkeydown = onKeyDownMain;
 
-    // Determine what page id will be loaded
-    var url = new URL(window.location.href);
-    var path = url.searchParams.get("p", path);
-    var parsed_path = RAL.parse_path(path);
-    var id;
-    if (parsed_path == null) {
-        id = 0;
-    } else {
-        id = parsed_path[0];
-    }
+    RAL.load_ral_data().then(() => {
+            // Determine what page id will be loaded
+            var url = new URL(window.location.href);
+            var path = url.searchParams.get("p", path);
+            var parsed_path = RAL.parse_path(path);
+            var id;
+            if (parsed_path == null) {
+                id = 0;
+            } else {
+                id = parsed_path[0];
+            }
 
-    // Load content
-    Sidebar.init(id);
-    load_page_via_url();
-    init_index_edit();
-    userHooks.onPageLoad();
+            // Load content
+            Sidebar.init(id);
+            load_page_via_url();
+            init_index_edit();
+            userHooks.onPageLoad();
+        })
+        .catch(e => {
+            // Page load failed
+            if (window.location.protocol == "file:") {
+                show_file_protocol_nag();
+            }
+        });
 }
 
 function onKeyDownMain(ev) {
     if (!ev) ev = window.event;
     var unhandled;
 
     if (ev.ctrlKey && ev.key == "\\") {
@@ -266,16 +274,73 @@
             el.className = "crumb-separator";
             el.innerHTML = ".";
             crumb_el.appendChild(el);
         }
     }
 }
 
-function update_absolute_addr(addr) {
-    document.getElementById("_AbsAddr").innerHTML = "0x" + addr.toString(16);
+function onClickAbsAddrDetailsInfo() {
+    var details_el = document.getElementById("_AbsAddrDetails");
+    if (details_el.classList.contains("open")) {
+        details_el.classList.remove("open");
+    } else {
+        details_el.classList.add("open");
+    }
+}
+
+function update_absolute_addr() {
+    var addr = RAL.get_absolute_addr(CurrentID);
+    var addr_el = document.getElementById("_AbsAddr");
+    addr_el.innerHTML = "0x" + addr.toString(16);
+
+    var showmore_div = document.createElement("div");
+    showmore_div.onclick = onClickAbsAddrDetailsInfo;
+    addr_el.appendChild(showmore_div);
+
+    var ids = RAL.get_ancestors(CurrentID);
+    ids.push(CurrentID);
+
+    var details_el = document.getElementById("_AbsAddrDetails");
+
+    while (details_el.firstElementChild) {
+        details_el.firstElementChild.remove();
+    }
+
+    for (var i = 0; i < ids.length; i++) {
+        var id = ids[i];
+        var node = RAL.get_node(id);
+        var el;
+
+        el = document.createElement("dt");
+        el.innerHTML = node.name + ":";
+        details_el.appendChild(el);
+
+        el = document.createElement("dd");
+        el.innerHTML = "+ 0x" + node.offset.toString(16);
+        details_el.appendChild(el);
+
+        if (RAL.is_array(id)) {
+            for (var ii = 0; ii < node.idxs.length; ii++) {
+                el = document.createElement("dt");
+                el.innerHTML = "[" + node.idxs[ii] + "]:";
+                details_el.appendChild(el);
+
+
+                var mults = []
+                for (var j = ii + 1; j < node.dims.length; j++) {
+                    mults.push(node.dims[j].toString());
+                }
+                mults.push(node.idxs[ii].toString())
+                mults.push("0x" + node.stride.toString(16))
+                el = document.createElement("dd");
+                el.innerHTML = "+ " + mults.join("*");
+                details_el.appendChild(el);
+            }
+        }
+    }
 }
 
 function update_rdlfc_indexes() {
     var index_els = document.getElementsByClassName("rdlfc-index")
     var index_text = "";
     if (RAL.is_array(CurrentID)) {
         for (var i = 0; i < RAL.get_node(CurrentID).idxs.length; i++) {
@@ -347,14 +412,20 @@
     } else if (str.startsWith("0b")) {
         return (bigInt(str.substring(2), 2));
     } else {
         return (bigInt(str));
     }
 }
 
+function page_specific_key(key) {
+    var url = new URL(window.location.href);
+    key = url.origin + url.pathname + "::" + key;
+    return key;
+}
+
 //==============================================================================
 // Compatibility Workarounds
 //==============================================================================
 // IE does not support Number.isInteger
 function isPositiveInteger(num) {
     return ((num ^ 0) >>> 0) === num;
 }
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/nav.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/nav.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,34 +1,28 @@
 // This file is part of PeakRDL-html <https://github.com/SystemRDL/PeakRDL-html>.
 // and can be redistributed under the terms of GNU GPL v3 <https://www.gnu.org/licenses/>.
 
 async function load_page(id) {
     var awaitable = fetch_page_content(id);
     awaitable.then(text => {
-            // Page loaded successfully
-            CurrentID = id;
-            update_crumbtrail();
+        // Page loaded successfully
+        CurrentID = id;
+        update_crumbtrail();
 
-            var main_el = document.getElementById("_ContentContainer");
-            main_el.innerHTML = text;
-            update_absolute_addr(RAL.get_absolute_addr(id));
-            update_rdlfc_indexes();
-            if (RAL.is_register(id)) {
-                init_reg_value();
-                init_radix_buttons();
-            }
-            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
-            userHooks.onContentLoad();
-        })
-        .catch(e => {
-            // Page load failed
-            if (window.location.protocol == "file:") {
-                show_file_protocol_nag();
-            }
-        });
+        var main_el = document.getElementById("_ContentContainer");
+        main_el.innerHTML = text;
+        update_absolute_addr();
+        update_rdlfc_indexes();
+        if (RAL.is_register(id)) {
+            init_reg_value();
+            init_radix_buttons();
+        }
+        MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
+        userHooks.onContentLoad();
+    });
 
     return awaitable;
 }
 
 async function fetch_page_content(id) {
     var path = "content/" + RAL.get_node_uid(id) + ".html?ts=" + BUILD_TS;
     var awaitable = fetch(path)
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/path_search.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/path_search.js`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/ral.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/ral.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,36 +1,105 @@
 // This file is part of PeakRDL-html <https://github.com/SystemRDL/PeakRDL-html>.
 // and can be redistributed under the terms of GNU GPL v3 <https://www.gnu.org/licenses/>.
 
 class RAL {
+    static #ral_data_files = new Array(N_RAL_FILES).fill(null);
+
+    static async load_ral_data() {
+        this.#init_progressbar();
+
+        // Dispatch all JSON fetch requests in parallel
+        var fetches = [];
+        for (var i = 0; i < N_RAL_FILES; i++) {
+            var awaitable = this.#load_ral_file(i);
+            fetches.push(awaitable);
+        }
+        await Promise.all(fetches);
+    }
+
+    static async #load_ral_file(idx) {
+        var path = "data/ral-data-" + idx + ".json?ts=" + BUILD_TS;
+        var awaitable = fetch(path)
+            .then(response => {
+                if (!response.ok) {
+                    throw new Error("fetch failed");
+                }
+                return response.json();
+            })
+            .then(data => {
+                this.#increment_progressbar();
+                this.#ral_data_files[idx] = data;
+            })
+            .catch(e => {
+                this.#destroy_progressbar();
+                throw new Error("fetch failed");
+            });
+        return awaitable;
+    }
+
+    static #progress_points = 0;
+    static #progressbar = null;
+    static #init_progressbar() {
+        this.#progressbar = new ProgressBar.Circle("#_ProgressBar", {
+            strokeWidth: 10, // forces extra padding
+            trailWidth: 3,
+            text: {
+                value: "Loading..."
+            }
+        });
+
+        if (N_RAL_FILES == 1) {
+            // Only one object to load. animate progress as stand-in.
+            this.#progressbar.animate(1, {
+                duration: 400
+            });
+        }
+    }
+    static #increment_progressbar() {
+        this.#progress_points++;
+        this.#progressbar.set(this.#progress_points / N_RAL_FILES);
+        if (this.#progress_points == N_RAL_FILES) {
+            this.#destroy_progressbar();
+        }
+    }
+
+    static #destroy_progressbar() {
+        this.#progressbar.destroy();
+        this.#progressbar = null;
+    }
 
     static get_node(id) {
-        var node = RALIndex[id];
+        var file_idx = Math.floor(id / N_RAL_NODES_PER_FILE);
+        var idx = id % N_RAL_NODES_PER_FILE;
+        var node = this.#ral_data_files[file_idx][idx];
         this.#expand_bigint(node);
         return node;
     }
 
     static #expand_bigint(node) {
         // Check if RAL entry has been converted yet
         if (typeof node.offset !== 'string') return;
 
-        // Needs conversion from base-16 string --> bigInt object
-        node.offset = bigInt(node.offset, 16);
-        node.size = bigInt(node.size, 16);
-        if ('stride' in node) node.stride = bigInt(node.stride, 16);
+        // Needs conversion from base-16 string --> BigInt object
+        node.offset = BigInt("0x" + node.offset);
+        node.size = BigInt("0x" + node.size);
+        if ('stride' in node) node.stride = BigInt("0x" + node.stride);
 
         if (RAL.is_register_node(node)) {
             for (var i = 0; i < node.fields.length; i++) {
-                node.fields[i].reset = bigInt(node.fields[i].reset, 16);
+                node.fields[i].reset = BigInt("0x" + node.fields[i].reset);
             }
         }
     }
 
     static number_of_ids() {
-        return RALIndex.length;
+        return (
+            (this.#ral_data_files.length - 1) * N_RAL_FILES +
+            this.#ral_data_files[this.#ral_data_files.length - 1].length
+        );
     }
 
     static is_register(id) {
         return (this.is_register_node(this.get_node(id)));
     }
 
     static is_register_node(node) {
@@ -256,38 +325,38 @@
             for (var i = 0; i < node.idxs.length; i++) {
                 var sz = 1;
                 for (var j = i + 1; j < node.dims.length; j++) {
                     sz *= node.dims[j];
                 }
                 flat_idx += sz * node.idxs[i];
             }
-            return (node.offset.add(node.stride.multiply(flat_idx)));
+            return (node.offset + node.stride * BigInt(flat_idx));
         } else {
             return (node.offset);
         }
     }
 
     static get_absolute_addr(id) {
         var node = this.get_node(id);
         if (node.parent != null) {
-            return (this.get_absolute_addr(node.parent).add(this.get_addr_offset(id)));
+            return (this.get_absolute_addr(node.parent) + this.get_addr_offset(id));
         } else {
             return (this.get_addr_offset(id));
         }
     }
 
     static get_total_size(id) {
         var node = this.get_node(id);
         // Total size of entire array of this node
         if (this.is_array(id)) {
             var num_elements = 1;
             for (var i = 0; i < node.dims.length; i++) {
                 num_elements *= node.dims[i];
             }
-            return (node.stride.multiply(num_elements - 1).add(node.size));
+            return (node.stride * BigInt(num_elements - 1) + node.size);
         } else {
             return (node.size);
         }
     }
 
     static lookup_by_address(addr, root_id) {
         // Finds the deepest RAL node that contains addr
@@ -295,61 +364,61 @@
         //  [id, idx_stack]
         // Otherwise, returns null
         if (typeof root_id === "undefined") root_id = 0;
         var id = root_id;
         var idx_stack = [];
         var iter_count = 0;
 
-        if (addr.lt(this.get_node(id).offset)) return (null);
-        if (addr.geq(this.get_node(id).offset.add(this.get_total_size(id)))) return (null);
+        if (addr < this.get_node(id).offset) return (null);
+        if (addr >= (this.get_node(id).offset + this.get_total_size(id))) return (null);
 
         while (iter_count < 100) {
             iter_count++;
             // addr is definitely inside this node
 
             // Adjust addr to be relative to this node
-            addr = addr.subtract(this.get_node(id).offset);
+            addr = addr - this.get_node(id).offset;
 
             // Determine index stack entry for this node
             if (this.is_array(id)) {
                 var idxs = [];
 
                 // First check if address lands between sparse array entries
-                if (addr.mod(this.get_node(id).stride).geq(this.get_node(id).size)) {
+                if ((addr % this.get_node(id).stride) >= this.get_node(id).size) {
                     // missed! Give up and just return the parent node
                     if (this.get_node(id).parent == null) {
                         return (null);
                     } else {
                         return ([this.get_node(id).parent, idx_stack]);
                     }
                 }
 
                 // index of the flattened array
-                var flat_idx = addr.divide(this.get_node(id).stride).toJSNumber();
+                var flat_idx = Number(addr / this.get_node(id).stride);
 
                 // Re-construct dimensions
                 for (var dim = this.get_node(id).dims.length - 1; dim >= 0; dim--) {
                     var idx;
                     idx = flat_idx % this.get_node(id).dims[dim];
                     flat_idx = Math.floor(flat_idx / this.get_node(id).dims[dim]);
                     idxs.unshift(idx);
                 }
                 idx_stack.push(idxs);
 
                 // Adjust addr offset to be relative to this index
-                addr = addr.mod(this.get_node(id).stride);
+                addr = addr % this.get_node(id).stride;
             } else {
                 idx_stack.push([]);
             }
 
             // Search this node's children to see which child 'addr' is in
             var found_match = false;
             for (var i = 0; i < this.get_node(id).children.length; i++) {
                 var child = this.get_node(id).children[i];
-                if (addr.geq(this.get_node(child).offset) && addr.lt(this.get_node(child).offset.add(this.get_total_size(child)))) {
+                if ((addr >= this.get_node(child).offset) && (addr < (this.get_node(child).offset + this.get_total_size(child)))) {
                     // hit!
                     id = child;
                     found_match = true;
                     break;
                 }
             }
             if (!found_match) {
@@ -373,27 +442,8 @@
     }
 
     static get_node_uid(id) {
         var path = this.get_path(id, null, false);
         var uid = SHA1(path);
         return uid;
     }
-}
-
-
-
-function ral_expand_bigint(id) {
-    var node = RAL.get_node(id);
-    // Check if RAL entry has been converted yet
-    if (typeof node.offset !== 'string') return;
-
-    // Needs conversion from base-16 string --> bigInt object
-    node.offset = bigInt(node.offset, 16);
-    node.size = bigInt(node.size, 16);
-    if ('stride' in node) node.stride = bigInt(node.stride, 16);
-
-    if (RAL.is_register(id)) {
-        for (var i = 0; i < node.fields.length; i++) {
-            node.fields[i].reset = bigInt(node.fields[i].reset, 16);
-        }
-    }
 }
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/search.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/search.js`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/sha1.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/sha1.js`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/js/sidebar.js` & `peakrdl-html-2.9.0/src/peakrdl_html/static/js/sidebar.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -2,30 +2,42 @@
 // and can be redistributed under the terms of GNU GPL v3 <https://www.gnu.org/licenses/>.
 
 class Sidebar {
     static #selected_node_id = null;
     static #resizer_old_width = 0;
     static #resizer_start_x = 0;
 
+    static #mousemove_cb = null;
+    static #mouseup_cb = null;
+
     static init(first_id) {
         var el;
         // Initialize the sidebar
 
         // Bind event to resizer
+        this.#mousemove_cb = this.#onResizeMouseMove.bind(this);
+        this.#mouseup_cb = this.#onResizeMouseUp.bind(this);
         el = document.getElementById("_SBResizer")
-        el.addEventListener("mousedown", this.#onResizeMouseDown);
+        el.addEventListener("mousedown", this.#onResizeMouseDown.bind(this));
 
         // create the root node(s). Do not recurse
         el = document.getElementById("_SBTree");
         for (var i = 0; i < RootNodeIds.length; i++) {
             this.#create_node(el, RootNodeIds[i]);
         };
 
         // Create and expand nodes up to the current selected ID
         this.expand_to_id(first_id);
+
+        // restore sidebar width from previous session
+        var sb_width = localStorage.getItem(page_specific_key("sb_width"));
+        if (sb_width != null) {
+            var sb_el = document.getElementById("_SBContents");
+            sb_el.style.width = sb_width;
+        }
     }
 
     static expand_to_id(id) {
         // Create sidebar elements as needed up to the given ID
 
         // array of required ID lineage
         var id_chain = RAL.get_ancestors(id);
@@ -188,29 +200,33 @@
         this.#selected_node_id = id;
     }
 
     static #onResizeMouseDown(e) {
         var sb_el = document.getElementById("_SBContents");
         this.#resizer_old_width = sb_el.getBoundingClientRect().width;
         this.#resizer_start_x = e.clientX;
-        window.addEventListener('mousemove', this.#onResizeMouseMove);
-        window.addEventListener('mouseup', this.#onResizeMouseUp);
+        window.addEventListener('mousemove', this.#mousemove_cb);
+        window.addEventListener('mouseup', this.#mouseup_cb);
         e.preventDefault();
     }
 
     static #onResizeMouseMove(e) {
         var sb_el = document.getElementById("_SBContents");
         var new_width;
         new_width = this.#resizer_old_width + e.clientX - this.#resizer_start_x;
         sb_el.style.width = new_width + "px";
     }
 
     static #onResizeMouseUp(e) {
-        window.removeEventListener('mousemove', this.#onResizeMouseMove);
-        window.removeEventListener('mouseup', this.#onResizeMouseUp);
+        window.removeEventListener('mousemove', this.#mousemove_cb);
+        window.removeEventListener('mouseup', this.#mouseup_cb);
+
+        // remember sidebar width
+        var sb_el = document.getElementById("_SBContents");
+        localStorage.setItem(page_specific_key("sb_width"), sb_el.style.width);
     }
 
     static show() {
         document.getElementById("_Sidebar").style.display = "flex";
         document.getElementById("_Overlay").style.display = "block";
     }
 
@@ -222,30 +238,39 @@
     static scroll_into_view(id) {
         var node_el = this.#get_node_el(id);
         var tree_el = document.getElementById("_SBTreeContainer");
 
         var node_rect = node_el.getBoundingClientRect();
         var tree_rect = tree_el.getBoundingClientRect();
 
-        if ((node_rect.top < tree_rect.top) || (node_rect.bottom > tree_rect.bottom)) {
-            if (typeof node_el.scrollIntoView === "function") {
-                node_el.scrollIntoView();
-            }
+        if (
+            (node_rect.top < tree_rect.top) ||
+            (node_rect.bottom > tree_rect.bottom) ||
+            (node_rect.left < tree_rect.left) ||
+            (node_rect.right > tree_rect.right)
+        ) {
+            node_el.scrollIntoView({
+                block: "nearest",
+                inline: "start"
+            });
         }
     }
 }
 
 function onClickTreeFold(ev) {
     var el = ev.target.parentNode;
     var id = parseInt(el.dataset.id);
     if (el.classList.contains("leaf")) return;
 
     if (el.classList.contains("closed")) {
         // Open this node
         Sidebar.expand_node(id);
+
+        // may need to re-select current
+        Sidebar.select_node(CurrentID);
     } else {
         // Close this node
         Sidebar.collapse_node(id);
     }
 }
 
 function onClickTreeLink(ev) {
@@ -271,12 +296,15 @@
         refresh_target_scroll();
     });
     return (false);
 }
 
 function onClickTreeExpandAll() {
     Sidebar.expand_all()
+
+    // may need to re-select current
+    Sidebar.select_node(CurrentID);
 }
 
 function onClickTreeCollapseAll() {
     Sidebar.collapse_all()
 }
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-chrome.bat` & `peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-chrome.bat`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-edge.bat` & `peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-edge.bat`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/static/launcher-windows-firefox.bat` & `peakrdl-html-2.9.0/src/peakrdl_html/static/launcher-windows-firefox.bat`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/stringify.py` & `peakrdl-html-2.9.0/src/peakrdl_html/stringify.py`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/base.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/base.html`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 <div>
 <h1 id="_Content.name">{{(node.get_html_name() or node.get_property("name"))|safe}}</h1>
 
 
 <dl class="node-info">
     {%- block node_info %}
     <dt>Absolute Address:</dt><dd id="_AbsAddr" class="address"></dd>
+    <div id="_AbsAddrDetails"></div>
     <dt>Base Offset:</dt><dd class="address">{{"0x%x" % node.raw_address_offset}}</dd>
     <dt>Size:</dt><dd class="address">{{"0x%x" % node.size}}</dd>
     {%- if node.inst.is_array %}
     <dt>Array Dimensions:</dt><dd>{{node.inst.array_dimensions}}</dd>
     <dt>Array Stride:</dt><dd>+{{"0x%x" % node.inst.array_stride}}</dd>
     <dt>Total Size:</dt><dd class="address">{{"0x%x" % node.total_size}}</dd>
     {%- endif %}
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/field_description.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/field_description.html`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/group-like.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/group-like.html`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/index_base.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/index_base.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     <script type="text/x-mathjax-config">
         MathJax.Hub.Config({
           config: ["MMLorHTML.js"],
           jax: ["input/TeX", "output/HTML-CSS", "output/NativeMML"],
           extensions: ["MathMenu.js", "MathZoom.js"]
         });
     </script>
-    <script src="js/BigInteger.min.js?v={{version}}" type="text/javascript"></script>
+    <script src="js/progressbar.min.js?v={{version}}" type="text/javascript"></script>
     <script src="js/sha1.js?v={{version}}" type="text/javascript"></script>
-    <script src="js/data.js?ts={{build_ts}}" type="text/javascript"></script>
+    <script src="data/data_index.js?ts={{build_ts}}" type="text/javascript"></script>
     <script src="search/bkt_index.js?ts={{build_ts}}" type="text/javascript"></script>
     <script src="js/ral.js?v={{version}}" type="text/javascript"></script>
     <script src="js/main.js?v={{version}}" type="text/javascript"></script>
     <script src="js/nav.js?v={{version}}" type="text/javascript"></script>
     <script src="js/sidebar.js?v={{version}}" type="text/javascript"></script>
     <script src="js/index_edit.js?v={{version}}" type="text/javascript"></script>
     <script src="js/field_testers.js?v={{version}}" type="text/javascript"></script>
@@ -98,14 +98,20 @@
             </div>
 
             <div id="_Search" class="main limit-h">
                 <ul id="_SearchResults">
                 </ul>
             </div>
 
+
+            <div class="main stretchy limit-h"></div>
+            <div class="main limit-h">
+                <div id="_ProgressBar"></div>
+            </div>
+
             <div class="main stretchy limit-h"></div>
             <footer class="main limit-h">
                 <hr/>
                 {%- block footer %}
                 {{footer_text}}
                 {%- endblock footer %}
             </footer>
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/macros.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/macros.html`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html/templates/reg_base.html` & `peakrdl-html-2.9.0/src/peakrdl_html/templates/reg_base.html`

 * *Files identical despite different names*

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html.egg-info/PKG-INFO` & `peakrdl-html-2.9.0/src/peakrdl_html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-html
-Version: 2.8.0
+Version: 2.9.0
 Summary: HTML documentation generator for SystemRDL-based register models
 Home-page: https://github.com/SystemRDL/PeakRDL-html
 Author: Alex Mykyta
 Author-email: amykyta3@github.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/SystemRDL/PeakRDL-html
 Project-URL: Tracker, https://github.com/SystemRDL/PeakRDL-html/issues
```

### Comparing `peakrdl-html-2.8.0/src/peakrdl_html.egg-info/SOURCES.txt` & `peakrdl-html-2.9.0/src/peakrdl_html.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -55,22 +55,22 @@
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
 src/peakrdl_html/static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
-src/peakrdl_html/static/js/BigInteger.min.js
 src/peakrdl_html/static/js/address_search.js
 src/peakrdl_html/static/js/content_search.js
 src/peakrdl_html/static/js/field_testers.js
 src/peakrdl_html/static/js/index_edit.js
 src/peakrdl_html/static/js/main.js
 src/peakrdl_html/static/js/nav.js
 src/peakrdl_html/static/js/path_search.js
+src/peakrdl_html/static/js/progressbar.min.js
 src/peakrdl_html/static/js/ral.js
 src/peakrdl_html/static/js/search.js
 src/peakrdl_html/static/js/sha1.js
 src/peakrdl_html/static/js/sidebar.js
 src/peakrdl_html/templates/addrmap.html
 src/peakrdl_html/templates/addrmap_base.html
 src/peakrdl_html/templates/base.html
```

