# Comparing `tmp/Subsearch-2.35.1.tar.gz` & `tmp/Subsearch-2.36.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Subsearch-2.35.1.tar", last modified: Thu May 25 15:54:31 2023, max compression
+gzip compressed data, was "Subsearch-2.36.0rc1.tar", last modified: Fri Jun  2 15:07:12 2023, max compression
```

## Comparing `Subsearch-2.35.1.tar` & `Subsearch-2.36.0rc1.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.718924 Subsearch-2.35.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 15:54:14.000000 Subsearch-2.35.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-25 15:54:14.000000 Subsearch-2.35.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-25 15:54:31.718924 Subsearch-2.35.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-05-25 15:54:14.000000 Subsearch-2.35.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-25 15:54:14.000000 Subsearch-2.35.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:54:31.718924 Subsearch-2.35.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 15:54:14.000000 Subsearch-2.35.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.706924 Subsearch-2.35.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/Subsearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 15:54:31.000000 Subsearch-2.35.1/src/Subsearch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9672 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/data_initializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9637 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/data_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/guid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/languages.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/gui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/gui/assets/btn/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/btn/btn_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/btn/btn_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/btn/btn_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/btn/btn_rest.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.710924 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_tri_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_tri_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/dark.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.714924 Subsearch-2.35.1/src/subsearch/gui/assets/icon/
--rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/icon/subsearch.ico
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/icon/subsearch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.714924 Subsearch-2.35.1/src/subsearch/gui/assets/scale/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_trough_hor.png
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_trough_vert.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scale/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.714924 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_left.png
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_right.png
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/separator.png
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/scrollbar/sizegrip.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.714924 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/language_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/language_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/language_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_hover.png
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_press.png
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_rest.png
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/assets/ttk_style.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tab_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.718924 Subsearch-2.35.1/src/subsearch/gui/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tabs/dowload_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tabs/language_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tabs/search_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tabs/settings_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/gui/tkinter_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.718924 Subsearch-2.35.1/src/subsearch/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/providers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/providers/opensubtitles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/providers/subscene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/providers/yifysubtitles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:54:31.718924 Subsearch-2.35.1/src/subsearch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/imdb_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/io_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/io_winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/mutex_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-25 15:54:14.000000 Subsearch-2.35.1/src/subsearch/utils/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.392326 Subsearch-2.36.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-02 15:07:12.392326 Subsearch-2.36.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:07:12.392326 Subsearch-2.36.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.360325 Subsearch-2.36.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.364325 Subsearch-2.36.0rc1/src/Subsearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 15:07:12.000000 Subsearch-2.36.0rc1/src/Subsearch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.368325 Subsearch-2.36.0rc1/src/subsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.368325 Subsearch-2.36.0rc1/src/subsearch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/data_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/data_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/languages.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.368325 Subsearch-2.36.0rc1/src/subsearch/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.372326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.372326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/btn/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/btn/btn_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/btn/btn_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/btn/btn_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/btn/btn_rest.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.376326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_tri_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_tri_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_tri_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_tri_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/checkbox/check_unsel_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/dark.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.376326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)   105808 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/icon/subsearch.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/icon/subsearch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.380326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_trough_hor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_trough_vert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.384326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_hor_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_right.png
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_thumb.png
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/scroll_vert_trough.png
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/scrollbar/sizegrip.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.388326 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/language_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/language_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/language_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_press.png
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/assets/ttk_style.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tab_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.388326 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/dowload_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/language_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/search_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tabs/settings_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/gui/tkinter_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.388326 Subsearch-2.36.0rc1/src/subsearch/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/providers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/providers/opensubtitles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/providers/subscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/providers/yifysubtitles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 15:07:12.392326 Subsearch-2.36.0rc1/src/subsearch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/app_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/imdb_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/io_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/io_winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/mutex_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-02 15:06:58.000000 Subsearch-2.36.0rc1/src/subsearch/utils/update.py
```

### Comparing `Subsearch-2.35.1/LICENSE` & `Subsearch-2.36.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/PKG-INFO` & `Subsearch-2.36.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.35.1
+Version: 2.36.0rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.35.1/README.md` & `Subsearch-2.36.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/pyproject.toml` & `Subsearch-2.36.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Programming Language :: Python :: 3.11",
     "Operating System :: Microsoft :: Windows",
     "Topic :: Multimedia :: Video",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop"
 ]
-dependencies = ["selectolax==0.3.13", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0"]
+dependencies = ["selectolax==0.3.14", "cloudscraper==1.2.71", "num2words==0.5.12", "packaging==23.1", "requests==2.31.0"]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/vagabondHustler/subsearch"
 
 [project.scripts]
 subsearch = "subsearch:main"
@@ -41,15 +41,15 @@
 exclude = ["examples*", "tools*", "subsearch.test*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "subsearch.data.__version__"}
 
 [project.optional-dependencies]
 optional = ["black==23.3.0", "isort==5.12.0", "twine==4.0.2", "build==0.10.0", "cx_Freeze==6.15.0", "mypy==1.3.0", "pipreqs==0.4.13"]
-dev = ["pytest==7.3.1", "pytest-cov==4.1.0", "tox==4.5.1"]
+dev = ["pytest==7.3.1", "pytest-cov==4.1.0", "tox==4.5.2"]
 
 
 [tool.pytest.ini_options]
 filterwarnings =[
     'ignore::DeprecationWarning'
 ]
 log_cli = true
```

### Comparing `Subsearch-2.35.1/setup.py` & `Subsearch-2.36.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/Subsearch.egg-info/PKG-INFO` & `Subsearch-2.36.0rc1/src/Subsearch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.35.1
+Version: 2.36.0rc1
 Summary: Subsearch - Download subtitles for movies and shows, automatically with one easy mouse click.
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subsearch,subscene,opensubtitles,yifysubtitles,download,subtitles,movies,shows,automatically,scrape
 Platform: win32
```

### Comparing `Subsearch-2.35.1/src/Subsearch.egg-info/SOURCES.txt` & `Subsearch-2.36.0rc1/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 src/subsearch/gui/tabs/settings_tab.py
 src/subsearch/providers/__init__.py
 src/subsearch/providers/generic.py
 src/subsearch/providers/opensubtitles.py
 src/subsearch/providers/subscene.py
 src/subsearch/providers/yifysubtitles.py
 src/subsearch/utils/__init__.py
+src/subsearch/utils/app_integrity.py
 src/subsearch/utils/exceptions.py
 src/subsearch/utils/file_manager.py
 src/subsearch/utils/imdb_lookup.py
 src/subsearch/utils/io_json.py
 src/subsearch/utils/io_winreg.py
 src/subsearch/utils/log.py
 src/subsearch/utils/mutex_synchronizer.py
```

### Comparing `Subsearch-2.35.1/src/subsearch/__init__.py` & `Subsearch-2.36.0rc1/src/subsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/core.py` & `Subsearch-2.36.0rc1/src/subsearch/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import ctypes
 import time
 
 from subsearch.data import __version__, app_paths, video_data
 from subsearch.data.data_objects import DownloadData, PrettifiedDownloadData
 from subsearch.gui import tab_manager
 from subsearch.providers import opensubtitles, subscene, yifysubtitles
-from subsearch.utils import file_manager, io_json, io_winreg, log, string_parser
+from subsearch.utils import (
+    app_integrity,
+    file_manager,
+    io_json,
+    io_winreg,
+    log,
+    string_parser,
+)
 
 
 class Initializer:
     def __init__(self) -> None:
-        file_manager.create_directory(app_paths.appdata_local)
-        file_manager.create_directory(app_paths.tmpdir)
-        io_json.create_application_config()
+        app_integrity.initialize_application()
         self.app_config = io_json.get_app_config()
         if video_data is not None:
             file_manager.create_directory(video_data.subs_directory)
             self.file_exist = True
             self.file_hash = file_manager.get_hash(video_data.file_path)
         else:
             self.file_exist = False
@@ -68,21 +73,22 @@
 
 class AppSteps(Initializer):
     def __init__(self) -> None:
         self.start = time.perf_counter()
         Initializer.__init__(self)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {__version__}")
         if io_winreg.registry_key_exists() is False and io_json.get_json_key("context_menu"):
-            io_json.create_application_config()
+            io_json.create_application_config_json()
             io_winreg.add_context_menu()
         if io_winreg.registry_key_exists() and io_winreg.key_no_value() and io_json.get_json_key("context_menu"):
             io_winreg.add_context_menu()
         if self.file_exist is False:
             tab_manager.open_tab("search")
             return None
+        self.foreign_only = io_json.get_json_key("foreign_only")
 
         if " " in video_data.filename:
             log.warning_spaces_in_filename()
         log.output_header("Search started")
 
     def _provider_opensubtitles(self) -> None:
         if self.skip_step.opensubtitles():
@@ -175,14 +181,16 @@
 class SkipStep:
     def __init__(self, cls):
         self.cls = cls
 
     def opensubtitles(self) -> bool:
         if self.cls.file_exist is False:
             return True
+        if self.cls.foreign_only:
+            return True
         if io_json.check_language_compatibility("opensubtitles") is False:
             return True
         if (
             self.cls.app_config.providers["opensubtitles_hash"] is False
             and self.cls.app_config.providers["opensubtitles_site"] is False
         ):
             return True
@@ -196,14 +204,16 @@
         if self.cls.app_config.providers["subscene_site"] is False:
             return True
         return False
 
     def yifysubtitles(self) -> bool:
         if self.cls.file_exist is False:
             return True
+        if self.cls.foreign_only:
+            return True
         if io_json.check_language_compatibility("yifysubtitles") is False:
             return True
         if self.cls.release_data.tvseries:
             return True
         if self.cls.provider_urls.yifysubtitles == "N/A":
             return True
         if self.cls.app_config.providers["yifysubtitles_site"] is False:
```

### Comparing `Subsearch-2.35.1/src/subsearch/data/data_initializer.py` & `Subsearch-2.36.0rc1/src/subsearch/data/data_initializer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/data/data_objects.py` & `Subsearch-2.36.0rc1/src/subsearch/data/data_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 @dataclass(order=True)
 class LanguageData:
     name: str
     alpha_1: str
     alpha_2b: str
     incompatibility: list[str]
+    subscene_id: int
 
 
 @dataclass(order=True)
 class ProviderAlphaCodeData:
     provider: str
     alpha_code: str
 
@@ -87,14 +88,15 @@
         providers (dict[str, bool]): A dictionary storing user's preferences regarding subtitle providers.
         hearing_impaired (bool): Boolean flag indicating if the subtitle is for hearing-impaired people.
         non_hearing_impaired (bool): Boolean flag indicating if the subtitle is not for hearing-impaired people.
     """
 
     current_language: str
     subtitle_type: dict[str, bool]
+    foreign_only: bool
     percentage_threshold: int
     rename_best_match: bool
     context_menu: bool
     context_menu_icon: bool
     manual_download_fail: bool
     manual_download_mode: bool
     show_terminal: bool
@@ -103,14 +105,23 @@
     log_to_file: bool
     file_extensions: dict[str, bool]
     providers: dict[str, bool]
     hearing_impaired: bool
     non_hearing_impaired: bool
 
 
+@dataclass(order=True)
+class SubsceneCookie:
+    dark_theme: bool
+    sort_subtitle_by_date: str
+    language_filter: int
+    hearing_impaired: bool
+    foreigen_only: bool
+
+
 @dataclass(frozen=True, order=True)
 class ReleaseData:
     """
     Data class representing data associated with a media release.
 
     Attributes:
         title (str): Title of the media.
```

### Comparing `Subsearch-2.35.1/src/subsearch/gui/__init__.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/dark.tcl` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/dark.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/icon/subsearch.ico` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/icon/subsearch.ico`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_disabled.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_hover.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_pressed.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/scale/scale_thumb_rest.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/scale/scale_thumb_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_hover.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_press.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/download_rest.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/download_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_hover.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_press.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/search_rest.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/search_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_hover.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_hover.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_press.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_press.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/tabs/settings_rest.png` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/tabs/settings_rest.png`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/assets/ttk_style.tcl` & `Subsearch-2.36.0rc1/src/subsearch/gui/assets/ttk_style.tcl`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tab_manager.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tab_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
         self.configure(bg=GUI_DATA.colors.dark_grey)
         search_tab.Providers(self).pack(anchor="center")
         tk.Frame(self, height=80, bg=GUI_DATA.colors.dark_grey).pack(anchor="center", expand=True)
         search_tab.SubtitleType(self).pack(anchor="center")
         search_tab.SearchThreshold(self).pack(anchor="center")
+        search_tab.ForeignOnly(self).pack(anchor="center")
         search_tab.RenameBestMatch(self).pack(anchor="center")
 
 
 class TabSettings(tk.Frame):
     def __init__(self, parent) -> None:
         tk.Frame.__init__(self, parent, width=GUI_DATA.size.root_width, height=GUI_DATA.size.root_height)
         self.configure(bg=GUI_DATA.colors.dark_grey)
@@ -154,37 +155,37 @@
     Returns:
         None: This function does not return anything, it manipulates the GUI instead.
     """
     try:
         formatted_data: list[PrettifiedDownloadData] = kwargs["formatted_data"]
     except KeyError:
         formatted_data = None  # type: ignore
-    root = initalize_root()
+    root = initialize_root()
     set_theme("dark")
     tkinter_utils.set_custom_btn_styles()
     tabs = {
         "language": TabLanguage(root),
         "search": TabSearch(root),
         "settings": TabSettings(root),
         "download": TabDownload(root, formatted_data),
     }
     footer = TabManager(root, tabs, active_tab.lower())
     footer.place(y=GUI_DATA.size.root_height - 82)
     root.mainloop()
 
 
-def initalize_root():
+def initialize_root():
     """
     Initialize the root Tkinter window for the Subsearch application.
 
     Returns:
         tk.Tk: The initialized Tkinter root window.
     """
     if io_json.APPCON_JSON.exists() is False:
-        io_json.create_application_config()
+        io_json.create_application_config_json()
     if io_json.get_json_key("context_menu"):
         io_winreg.add_context_menu()
     root = tk.Tk(className=f"Subsearch")
     root.configure(background=GUI_DATA.colors.dark_grey)
     root.iconbitmap(app_paths.icon)
     root.geometry(tkinter_utils.WindowPosition.set(root))  # type: ignore
     root.resizable(False, False)
```

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tabs/dowload_tab.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tabs/dowload_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tabs/language_tab.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tabs/language_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tabs/search_tab.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tabs/search_tab.py`

 * *Files 7% similar despite different names*

```diff
@@ -209,14 +209,26 @@
 
     def update_config(self) -> None:
         update_svar = self.current_value.get()
         io_json.set_config_key_value("percentage_threshold", update_svar)
         tkinter_utils.VarColorPicker(self.string_var, self.clabel, True)
 
 
+class ForeignOnly(tkinter_utils.ToggleableFrameButton):
+    """
+    Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
+
+    Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
+    """
+
+    def __init__(self, parent) -> None:
+        text = f"If 'True', 'OpenSubtitles, Yifysubtitles' will be automatically skipped."
+        tkinter_utils.ToggleableFrameButton.__init__(self, parent, "Foreign language only", "foreign_only", tip_text=text)
+
+
 class RenameBestMatch(tkinter_utils.ToggleableFrameButton):
     """
     Inherits from the tk_tools.ToggleableFrameButton class and create toggleable button widget with different settings.
 
     Class corresponds to a specific setting in the configuration file and has a unique label, configuration key, and other optional attributes.
     """
```

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tabs/settings_tab.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tabs/settings_tab.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/gui/tkinter_utils.py` & `Subsearch-2.36.0rc1/src/subsearch/gui/tkinter_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,23 +310,27 @@
         parent (tk.Widget): The parent widget.
         setting_label (str): Name of the setting to be displayeed.
         config_key (str): Key in the configuration file where the state is stored.
         write_to_reg (bool, optional): Whether to also write the state to registry. Defaults to False.
         show_if_exe (bool, optional): Only show the button if the program is not running from an executable. Defaults to True.
     """
 
-    def __init__(self, parent, setting_label: str, config_key: str, write_to_reg: bool = False, show_if_exe=True) -> None:
+    def __init__(
+        self, parent, setting_label: str, config_key: str, write_to_reg: bool = False, show_if_exe=True, tip_text=None
+    ) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=GUI_DATA.colors.dark_grey)
         self.string_var = tk.StringVar()
         self.string_var.set(f"{io_json.get_json_key(config_key)}")
         self.setting_name = setting_label
         self.config_key = config_key
         self.write_to_reg = write_to_reg
         self.show_if_exe = show_if_exe
+        self.tip_text = tip_text
+        self.tip_present = False
         if show_if_exe is False and file_manager.running_from_exe():
             return None
         label = tk.Label(self, text=self.setting_name)
         label.configure(DEFAULT_LABEL_CONFIG)
         label.grid(DEFAULT_LABEL_GRID)
         btn_toggle = ttk.Button(
             self,
@@ -347,23 +351,30 @@
             event: The tkinter event object.
         """
         btn = event.widget
         if btn["text"] == "True":
             btn.bind("<ButtonRelease-1>", self.button_set_false)
         if btn["text"] == "False":
             btn.bind("<ButtonRelease-1>", self.button_set_true)
+        if self.tip_text is not None and self.tip_present is False:
+            self.tip = ToolTip(btn, btn, self.tip_text)
+            self.tip.show()
+            self.tip_present = True
 
     def leave_button(self, event) -> None:
         """
         Function called when the mouse leaves the button area.
 
         Args:
             event: The tkinter event object.
         """
         btn = event.widget
+        if self.tip_present:
+            self.tip.hide()
+            self.tip_present = False
 
     def button_set_true(self, event) -> None:
         """
         Function called when the button is set to True.
 
         Args:
             event: The tkinter event object.
```

### Comparing `Subsearch-2.35.1/src/subsearch/providers/opensubtitles.py` & `Subsearch-2.36.0rc1/src/subsearch/providers/opensubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/providers/subscene.py` & `Subsearch-2.36.0rc1/src/subsearch/providers/subscene.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,24 @@
             pass
         elif hi_sub is False and item.css_matches("td.a40"):
             return True
         elif regular_sub is False and item.css_matches("td.a41"):
             return True
         return False
 
-    def find_subtitles(self, url: str, hi_sub: bool, regular_sub: bool) -> dict[str, str]:
+    def find_subtitles(self, url: str, hi_sub: bool, regular_sub: bool, subscene_header) -> dict[str, str]:
         subtitles: dict[str, str] = {}
-        tree = generic.get_html_parser(url)
+        tree = generic.get_html_parser(url, subscene_header)
         products = tree.css("tr")
         for item in products[1:]:
             if self.skip_item(item, hi_sub, regular_sub):
                 continue
             node = item.css_first("a")
+            if node.child.text_content == "upload":
+                continue
             subtitle_href = node.attributes["href"]
             filename = item.css_first("span:nth-child(2)").child.text_content.strip()
             subtitles[filename] = f"https://subscene.com{subtitle_href}"
         return subtitles
 
     def get_download_url(self, url: str) -> str:
         tree = generic.get_html_parser(url)
@@ -65,23 +67,24 @@
             return [f"{self.title} - {self.season_ordinal} season"]
         return [f"{self.title} ({self.year})", f"{self.title} ({(self.year-1)})"]
 
     def parse_site_results(self) -> list | list[DownloadData]:
         to_be_sorted: list[PrettifiedDownloadData] = []
         _to_be_downloaded: dict[str, str] = {}
         to_be_downloaded: dict[str, str] = {}
-
+        custom_subscene_header = generic.CustomSubsceneHeader(self.app_config)
+        header = custom_subscene_header.create_header()
         # find title
         definitive_match = self._definitive_match()
         found_title_url = self.find_title(self.url_subscene, self.current_language, definitive_match)
         if not found_title_url:
             return []
 
         # search for subtitles
-        subtitle_data = self.find_subtitles(found_title_url, self.hi_sub, self.non_hi_sub)
+        subtitle_data = self.find_subtitles(found_title_url, self.hi_sub, self.non_hi_sub, header)
         for key, value in subtitle_data.items():
             pct_result = string_parser.calculate_match(key, self.release)
             log.output_match("subscene", pct_result, key)
             formatted_data = generic.prettify_download_data("subscene", key, value, pct_result)
             to_be_sorted.append(formatted_data)
             if self.is_threshold_met(key, pct_result) is False or self.manual_download_mode:
                 continue
```

### Comparing `Subsearch-2.35.1/src/subsearch/providers/yifysubtitles.py` & `Subsearch-2.36.0rc1/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/exceptions.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/file_manager.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/imdb_lookup.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/imdb_lookup.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/io_json.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/io_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 from typing import Any, Union
 
 from subsearch.data import SUPPORTED_FILE_EXTENSIONS, SUPPORTED_PROVIDERS, app_paths
 from subsearch.data.data_objects import AppConfig, LanguageData, ProviderAlphaCodeData
+from subsearch.utils import file_manager
 from subsearch.utils.exceptions import ProviderNotImplemented
 
 APPCON_JSON = Path(app_paths.appdata_local) / "application_config.json"
 LANGS_JSON = Path(app_paths.data) / "languages.json"
 
 
 def get_json_data(json_file: Path = APPCON_JSON) -> Any:
@@ -74,42 +75,49 @@
     """
     with open(json_file, "w") as f:
         f.seek(0)
         json.dump(data, f, indent=4)
         f.truncate()
 
 
-def create_application_config() -> None:
+def retrieve_application_config() -> dict[str, Any]:
+    subtitle_types = ["hearing_impaired", "non_hearing_impaired"]
+    data = {
+        "current_language": "english",
+        "subtitle_type": dict.fromkeys(subtitle_types, True),
+        "foreign_only": False,
+        "percentage_threshold": 90,
+        "rename_best_match": True,
+        "context_menu": True,
+        "context_menu_icon": True,
+        "manual_download_fail": True,
+        "manual_download_mode": False,
+        "use_threading": True,
+        "multiple_app_instances": False,
+        "show_terminal": False,
+        "log_to_file": False,
+        "file_extensions": dict.fromkeys(SUPPORTED_FILE_EXTENSIONS, True),
+        "providers": dict.fromkeys(SUPPORTED_PROVIDERS, True),
+    }
+    return data
+
+
+def create_config_file() -> None:
     """
-    Creates application_config.json file and set the default values.
+    Creates application_config.json file and set the default values if it doesn't exist and.
 
     Returns:
         None.
     """
     if APPCON_JSON.exists():
         return None
-    subtitle_types = ["hearing_impaired", "non_hearing_impaired"]
-    data = {}
-    data["current_language"] = "english"
-    data["subtitle_type"] = dict.fromkeys(subtitle_types, True)
-    data["percentage_threshold"] = 90
-    data["rename_best_match"] = True
-    data["context_menu"] = True
-    data["context_menu_icon"] = True
-    data["manual_download_fail"] = True
-    data["manual_download_mode"] = False
-    data["use_threading"] = True
-    data["multiple_app_instances"] = False
-    data["show_terminal"] = False
-    data["log_to_file"] = False
-    data["file_extensions"] = dict.fromkeys(SUPPORTED_FILE_EXTENSIONS, True)
-    data["providers"] = dict.fromkeys(SUPPORTED_PROVIDERS, True)
+    application_config = retrieve_application_config()
     with open(APPCON_JSON, "w", encoding="utf-8") as file:
         file.seek(0)
-        json.dump(data, file, indent=4)
+        json.dump(application_config, file, indent=4)
         file.truncate()
 
 
 def get_app_config() -> AppConfig:
     """
     Returns an instance of AppConfig that contains the current configuration settings.
 
@@ -140,14 +148,19 @@
         language = get_json_key("current_language")
 
     data = get_json_data(LANGS_JSON)
     language_data = LanguageData(**data[language])
     return language_data
 
 
+def get_language_data_value(key: str):
+    data = get_language_data()
+    return data[key]
+
+
 def get_available_languages() -> dict:
     return get_json_data(LANGS_JSON)
 
 
 def get_provider_alpha_code_type(provider: str) -> ProviderAlphaCodeData:
     """
     Generates ProviderAlphaCodeType object containing provider and its associated alpha code.
```

### Comparing `Subsearch-2.35.1/src/subsearch/utils/io_winreg.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/io_winreg.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/log.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,16 @@
     Returns:
         None
     """
     if src_.is_file():
         type = "file"
     elif src_.is_dir():
         type = "directory"
+    else:
+        return None
 
     src = src_.relative_to(src_.parent.parent) if src_ else None
     dst = dst_.relative_to(dst_.parent.parent) if dst_ else None
 
     action_messages: dict[str, str] = {
         "remove": rf"Removing {type}: ...\{src}",
         "rename": rf"Renaming {type}: ...\{src} -> ...\{dst}",
```

### Comparing `Subsearch-2.35.1/src/subsearch/utils/mutex_synchronizer.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/mutex_synchronizer.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/string_parser.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/string_parser.py`

 * *Files identical despite different names*

### Comparing `Subsearch-2.35.1/src/subsearch/utils/update.py` & `Subsearch-2.36.0rc1/src/subsearch/utils/update.py`

 * *Files identical despite different names*

