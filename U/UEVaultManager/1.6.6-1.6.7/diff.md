# Comparing `tmp/UEVaultManager-1.6.6.tar.gz` & `tmp/UEVaultManager-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UEVaultManager-1.6.6.tar", last modified: Thu Jun  1 11:22:23 2023, max compression
+gzip compressed data, was "UEVaultManager-1.6.7.tar", last modified: Fri Jun  2 09:48:47 2023, max compression
```

## Comparing `UEVaultManager-1.6.6.tar` & `UEVaultManager-1.6.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.836544 UEVaultManager-1.6.6/
--rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.6/LICENSE
--rw-rw-rw-   0        0        0     6127 2023-06-01 11:22:23.836544 UEVaultManager-1.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.795542 UEVaultManager-1.6.6/UEVaultManager/
--rw-rw-rw-   0        0        0      778 2023-06-01 11:22:08.000000 UEVaultManager-1.6.6/UEVaultManager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.801543 UEVaultManager-1.6.6/UEVaultManager/api/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/api/__init__.py
--rw-rw-rw-   0        0        0    25469 2023-05-25 16:36:39.000000 UEVaultManager-1.6.6/UEVaultManager/api/egs.py
--rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.6/UEVaultManager/api/uevm.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.804544 UEVaultManager-1.6.6/UEVaultManager/assets/
--rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/assets/UEVM_200x200.png
--rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.6/UEVaultManager/assets/checked_16.png
--rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/assets/main.ico
--rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.6/UEVaultManager/assets/unchecked_16.png
--rw-rw-rw-   0        0        0    73092 2023-06-01 11:05:19.000000 UEVaultManager-1.6.6/UEVaultManager/cli.py
--rw-rw-rw-   0        0        0    46806 2023-06-01 06:50:17.000000 UEVaultManager-1.6.6/UEVaultManager/core.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.804544 UEVaultManager-1.6.6/UEVaultManager/downloader/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.806545 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/__init__.py
--rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/manager.py
--rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.6/UEVaultManager/downloader/mp/workers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.810542 UEVaultManager-1.6.6/UEVaultManager/lfs/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/__init__.py
--rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/egl.py
--rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/eos.py
--rw-rw-rw-   0        0        0    23585 2023-05-26 09:04:11.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/uevmlfs.py
--rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/utils.py
--rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.6.6/UEVaultManager/lfs/windows_helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.817546 UEVaultManager-1.6.6/UEVaultManager/models/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/models/__init__.py
--rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.6.6/UEVaultManager/models/app.py
--rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.6.6/UEVaultManager/models/chunk.py
--rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.6/UEVaultManager/models/config.py
--rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.6/UEVaultManager/models/csv.py
--rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.6/UEVaultManager/models/downloading.py
--rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.6.6/UEVaultManager/models/egl.py
--rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.6/UEVaultManager/models/exceptions.py
--rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.6/UEVaultManager/models/json_manifest.py
--rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.6.6/UEVaultManager/models/manifest.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.818542 UEVaultManager-1.6.6/UEVaultManager/tkgui/
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-01 09:11:19.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.828546 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/
--rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
--rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditCellWindowClass.py
--rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditRowWindowClass.py
--rw-rw-rw-   0        0        0    32497 2023-06-01 06:46:43.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditableTableClass.py
--rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
--rw-rw-rw-   0        0        0    12788 2023-06-01 09:12:21.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/GUISettingsClass.py
--rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
--rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/SaferDictClass.py
--rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
--rw-rw-rw-   0        0        0    43199 2023-06-01 07:25:24.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiClass.py
--rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
--rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/WebImageClass.py
--rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/__init__.py
--rw-rw-rw-   0        0        0     9697 2023-05-31 17:11:24.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions.py
--rw-rw-rw-   0        0        0     7590 2023-06-01 11:21:26.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions_no_deps.py
--rw-rw-rw-   0        0        0     2631 2023-05-31 15:29:53.000000 UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/globals.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.835544 UEVaultManager-1.6.6/UEVaultManager/utils/
--rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.6/UEVaultManager/utils/__init__.py
--rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.6.6/UEVaultManager/utils/aliasing.py
--rw-rw-rw-   0        0        0     5897 2023-06-01 11:15:05.000000 UEVaultManager-1.6.6/UEVaultManager/utils/cli.py
--rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.6/UEVaultManager/utils/custom_parser.py
--rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.6.6/UEVaultManager/utils/egl_crypt.py
--rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.6/UEVaultManager/utils/env.py
--rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.6/UEVaultManager/utils/rolling_hash.py
--rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.6/UEVaultManager/utils/webview_login.py
-drwxrwxrwx   0        0        0        0 2023-06-01 11:22:23.799544 UEVaultManager-1.6.6/UEVaultManager.egg-info/
--rw-rw-rw-   0        0        0     6127 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2345 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      300 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-01 11:22:23.000000 UEVaultManager-1.6.6/UEVaultManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 11:22:23.837544 UEVaultManager-1.6.6/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.423394 UEVaultManager-1.6.7/
+-rw-rw-rw-   0        0        0    35823 2023-01-05 18:12:15.000000 UEVaultManager-1.6.7/LICENSE
+-rw-rw-rw-   0        0        0     6127 2023-06-02 09:48:47.423394 UEVaultManager-1.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5285 2023-05-23 13:48:41.000000 UEVaultManager-1.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.365395 UEVaultManager-1.6.7/UEVaultManager/
+-rw-rw-rw-   0        0        0      778 2023-06-01 13:30:53.000000 UEVaultManager-1.6.7/UEVaultManager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.372393 UEVaultManager-1.6.7/UEVaultManager/api/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/api/__init__.py
+-rw-rw-rw-   0        0        0    25471 2023-06-01 13:10:41.000000 UEVaultManager-1.6.7/UEVaultManager/api/egs.py
+-rw-rw-rw-   0        0        0     3142 2023-05-17 13:34:09.000000 UEVaultManager-1.6.7/UEVaultManager/api/uevm.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.375394 UEVaultManager-1.6.7/UEVaultManager/assets/
+-rw-rw-rw-   0        0        0    20282 2023-05-11 14:38:28.000000 UEVaultManager-1.6.7/UEVaultManager/assets/UEVM_200x200.png
+-rw-rw-rw-   0        0        0      432 2023-05-21 17:27:34.000000 UEVaultManager-1.6.7/UEVaultManager/assets/checked_16.png
+-rw-rw-rw-   0        0        0     4286 2023-05-11 14:38:28.000000 UEVaultManager-1.6.7/UEVaultManager/assets/main.ico
+-rw-rw-rw-   0        0        0      187 2023-05-21 17:27:58.000000 UEVaultManager-1.6.7/UEVaultManager/assets/unchecked_16.png
+-rw-rw-rw-   0        0        0    75996 2023-06-02 09:33:00.000000 UEVaultManager-1.6.7/UEVaultManager/cli.py
+-rw-rw-rw-   0        0        0    47699 2023-06-01 15:59:09.000000 UEVaultManager-1.6.7/UEVaultManager/core.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.376395 UEVaultManager-1.6.7/UEVaultManager/downloader/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.378394 UEVaultManager-1.6.7/UEVaultManager/downloader/mp/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/downloader/mp/__init__.py
+-rw-rw-rw-   0        0        0    38024 2023-05-31 17:12:12.000000 UEVaultManager-1.6.7/UEVaultManager/downloader/mp/manager.py
+-rw-rw-rw-   0        0        0    12365 2023-05-25 16:35:52.000000 UEVaultManager-1.6.7/UEVaultManager/downloader/mp/workers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.382394 UEVaultManager-1.6.7/UEVaultManager/lfs/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/__init__.py
+-rw-rw-rw-   0        0        0     3611 2023-05-11 14:38:28.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/egl.py
+-rw-rw-rw-   0        0        0     6428 2023-05-15 06:51:22.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/eos.py
+-rw-rw-rw-   0        0        0    23603 2023-06-02 09:07:47.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/uevmlfs.py
+-rw-rw-rw-   0        0        0      593 2023-05-15 06:35:46.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/utils.py
+-rw-rw-rw-   0        0        0     3927 2023-06-01 07:37:43.000000 UEVaultManager-1.6.7/UEVaultManager/lfs/windows_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.390395 UEVaultManager-1.6.7/UEVaultManager/models/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/models/__init__.py
+-rw-rw-rw-   0        0        0     5942 2023-06-01 07:24:48.000000 UEVaultManager-1.6.7/UEVaultManager/models/app.py
+-rw-rw-rw-   0        0        0     4513 2023-06-01 07:26:13.000000 UEVaultManager-1.6.7/UEVaultManager/models/chunk.py
+-rw-rw-rw-   0        0        0     2703 2023-05-20 09:18:48.000000 UEVaultManager-1.6.7/UEVaultManager/models/config.py
+-rw-rw-rw-   0        0        0     2133 2023-05-25 16:35:38.000000 UEVaultManager-1.6.7/UEVaultManager/models/csv.py
+-rw-rw-rw-   0        0        0     3627 2023-05-11 14:38:28.000000 UEVaultManager-1.6.7/UEVaultManager/models/downloading.py
+-rw-rw-rw-   0        0        0     5229 2023-06-01 07:14:54.000000 UEVaultManager-1.6.7/UEVaultManager/models/egl.py
+-rw-rw-rw-   0        0        0      256 2023-05-20 09:20:19.000000 UEVaultManager-1.6.7/UEVaultManager/models/exceptions.py
+-rw-rw-rw-   0        0        0     5893 2023-05-15 06:30:52.000000 UEVaultManager-1.6.7/UEVaultManager/models/json_manifest.py
+-rw-rw-rw-   0        0        0    30610 2023-06-01 07:29:35.000000 UEVaultManager-1.6.7/UEVaultManager/models/manifest.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.391397 UEVaultManager-1.6.7/UEVaultManager/tkgui/
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:41.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/__init__.py
+-rw-rw-rw-   0        0        0     1712 2023-06-02 07:57:24.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/main.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.403393 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/
+-rw-rw-rw-   0        0        0     6747 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py
+-rw-rw-rw-   0        0        0     4683 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditCellWindowClass.py
+-rw-rw-rw-   0        0        0     6674 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditRowWindowClass.py
+-rw-rw-rw-   0        0        0    33069 2023-06-02 06:58:20.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditableTableClass.py
+-rw-rw-rw-   0        0        0    14552 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py
+-rw-rw-rw-   0        0        0    12891 2023-06-01 13:36:01.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/GUISettingsClass.py
+-rw-rw-rw-   0        0        0    14067 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/ProgressWindowsClass.py
+-rw-rw-rw-   0        0        0     2251 2023-05-25 16:37:41.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/SaferDictClass.py
+-rw-rw-rw-   0        0        0     6089 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py
+-rw-rw-rw-   0        0        0    45155 2023-06-02 09:27:48.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/UEVMGuiClass.py
+-rw-rw-rw-   0        0        0      543 2023-05-25 16:37:42.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py
+-rw-rw-rw-   0        0        0     2230 2023-05-31 15:29:53.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/WebImageClass.py
+-rw-rw-rw-   0        0        0       16 2023-05-25 16:37:42.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/__init__.py
+-rw-rw-rw-   0        0        0     9704 2023-06-02 09:05:32.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/functions.py
+-rw-rw-rw-   0        0        0     7759 2023-06-02 07:59:54.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/functions_no_deps.py
+-rw-rw-rw-   0        0        0     3152 2023-06-02 09:13:08.000000 UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/globals.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.421394 UEVaultManager-1.6.7/UEVaultManager/utils/
+-rw-rw-rw-   0        0        0       16 2023-05-15 06:33:02.000000 UEVaultManager-1.6.7/UEVaultManager/utils/__init__.py
+-rw-rw-rw-   0        0        0     3691 2023-06-01 07:18:12.000000 UEVaultManager-1.6.7/UEVaultManager/utils/aliasing.py
+-rw-rw-rw-   0        0        0     5897 2023-06-01 11:15:05.000000 UEVaultManager-1.6.7/UEVaultManager/utils/cli.py
+-rw-rw-rw-   0        0        0     1342 2023-05-15 06:55:20.000000 UEVaultManager-1.6.7/UEVaultManager/utils/custom_parser.py
+-rw-rw-rw-   0        0        0    10410 2023-06-01 07:27:36.000000 UEVaultManager-1.6.7/UEVaultManager/utils/egl_crypt.py
+-rw-rw-rw-   0        0        0      503 2023-05-15 10:15:48.000000 UEVaultManager-1.6.7/UEVaultManager/utils/env.py
+-rw-rw-rw-   0        0        0      752 2023-05-15 06:58:00.000000 UEVaultManager-1.6.7/UEVaultManager/utils/rolling_hash.py
+-rw-rw-rw-   0        0        0     7260 2023-05-17 13:34:09.000000 UEVaultManager-1.6.7/UEVaultManager/utils/webview_login.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:48:47.369394 UEVaultManager-1.6.7/UEVaultManager.egg-info/
+-rw-rw-rw-   0        0        0     6127 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2345 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      300 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 09:48:47.000000 UEVaultManager-1.6.7/UEVaultManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:48:47.424394 UEVaultManager-1.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     3008 2023-05-23 12:39:50.000000 UEVaultManager-1.6.7/setup.py
```

### Comparing `UEVaultManager-1.6.6/LICENSE` & `UEVaultManager-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/PKG-INFO` & `UEVaultManager-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.6
+Version: 1.6.7
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.6 ## codename: Virgo+6
+ UEVaultManager ## version:1.6.7 ## codename: Virgo+7
```

### Comparing `UEVaultManager-1.6.6/README.md` & `UEVaultManager-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/__init__.py` & `UEVaultManager-1.6.7/UEVaultManager/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 UEVaultManager setup file.
 """
 import datetime
 
 year = datetime.date.today().year
 
 __name__ = 'UEVaultManager'
-__version__ = '1.6.6'
+__version__ = '1.6.7'
 # 0 Pegasus Seiya
 # 1 Dragon Shiryu
 # 2 Cygnus Hyoga
 # 3 Andromeda Shun
 # 4 Phoenix Ikki
 # 5 Leo Aiolia
 # 5 Virgo Shaka
-__codename__ = 'Virgo+6'
+__codename__ = 'Virgo+7'
 # 6 Libra Dohko
 # 7 Scorpio Milo
 # 8 Sagittarius Aiolos
 # 9 Capricorn Shura
 # 10 Aquarius Camus
 # 11 Pisces Aphrodite
 __author__ = 'Laurent Ongaro'
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/api/egs.py` & `UEVaultManager-1.6.7/UEVaultManager/api/egs.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,16 +429,16 @@
 
         soup = BeautifulSoup(r.content, 'html.parser')
         links = []
         group_elt = soup.find('div', attrs={'class': 'asset-list-group'})
 
         if "No content found" in group_elt.getText():
             self.log.info(f'{asset_name} has not been not found in marketplace.It has been added to the notfound_logger file')
-            if self.ignored_logger:
-                self.ignored_logger.info(asset_name)
+            if self.notfound_logger:
+                self.notfound_logger.info(asset_name)
             return [url, asset_name_in_url, GrabResult.CONTENT_NOT_FOUND.name]
 
         # find all links to assets that correspond to the search
         for link in group_elt.findAll('a', attrs={'class': 'mock-ellipsis-item mock-ellipsis-item-helper ellipsis-text'}):
             links.append(link.get('href'))
 
         # return the first one (probably the best choice)
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/api/uevm.py` & `UEVaultManager-1.6.7/UEVaultManager/api/uevm.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/assets/UEVM_200x200.png` & `UEVaultManager-1.6.7/UEVaultManager/assets/UEVM_200x200.png`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/assets/main.ico` & `UEVaultManager-1.6.7/UEVaultManager/assets/main.ico`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/cli.py` & `UEVaultManager-1.6.7/UEVaultManager/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from UEVaultManager.api.egs import create_empty_assets_extras, GrabResult
 from UEVaultManager.api.uevm import UpdateSeverity
 from UEVaultManager.core import AppCore
 from UEVaultManager.models.csv import CSV_headings
 from UEVaultManager.models.exceptions import InvalidCredentialsError
 from UEVaultManager.tkgui.main import init_gui
 from UEVaultManager.tkgui.modules.DisplayContentWindowClass import DisplayContentWindow
-from UEVaultManager.tkgui.modules.functions import custom_print  # simplier way to use the custom_print function
+from UEVaultManager.tkgui.modules.functions import custom_print, box_message  # simplier way to use the custom_print function
 from UEVaultManager.tkgui.modules.functions import json_print_key_val
 from UEVaultManager.tkgui.modules.ProgressWindowsClass import ProgressWindow
 from UEVaultManager.tkgui.modules.SaferDictClass import SaferDict
 from UEVaultManager.tkgui.modules.UEVMGuiClass import UEVMGui
 from UEVaultManager.tkgui.modules.UEVMGuiHiddenRootClass import UEVMGuiHiddenRoot
 from UEVaultManager.utils.cli import str_to_bool, check_and_create_path, create_list_from_string, str_is_bool
 from UEVaultManager.utils.custom_parser import HiddenAliasSubparsersAction
@@ -118,32 +118,21 @@
 
 class UEVaultManagerCLI:
     """
     Command line interface for UEVaultManager
     :param override_config: path to a config file to use instead of the default one
     :param api_timeout: timeout for API requests
     """
+    is_gui = False
 
     def __init__(self, override_config=None, api_timeout=None):
         self.core = AppCore(override_config, timeout=api_timeout)
         self.logger = logging.getLogger('Cli')
         self.logging_queue = None
 
-    def setup_threaded_logging(self) -> QueueListener:
-        """
-        Setup logging for the CLI
-        """
-        self.logging_queue = MPQueue(-1)
-        handler = logging.StreamHandler()
-        formatter = logging.Formatter('[%(name)s] %(levelname)s: %(message)s')
-        handler.setFormatter(formatter)
-        ql = QueueListener(self.logging_queue, handler)
-        ql.start()
-        return ql
-
     def _resolve_aliases(self, name: str) -> str:
         """
         Resolve an alias
         :param name: name to resolve
         :return: real name
         """
         # make sure aliases exist if not yet created
@@ -155,14 +144,41 @@
     @staticmethod
     def _print_json(data, pretty=False):
         if pretty:
             print(json.dumps(data, indent=2, sort_keys=True))
         else:
             print(json.dumps(data))
 
+    def _log_gui_wrapper(self, log_function, message: str, must_quit=False) -> None:
+        """
+        Wrapper for the log function to display a messagebox if the gui is active
+        :param log_function: function to use to log
+        :param message: message to log
+        """
+        if not UEVaultManagerCLI.is_gui:
+            log_function(message)
+            return
+        if must_quit:
+            box_message(message, level='critical')
+            self.core.clean_exit(1)
+        else:
+            box_message(message, level='error')
+
+    def setup_threaded_logging(self) -> QueueListener:
+        """
+        Setup logging for the CLI
+        """
+        self.logging_queue = MPQueue(-1)
+        handler = logging.StreamHandler()
+        formatter = logging.Formatter('[%(name)s] %(levelname)s: %(message)s')
+        handler.setFormatter(formatter)
+        ql = QueueListener(self.logging_queue, handler)
+        ql.start()
+        return ql
+
     def create_file_backup(self, file_src: str) -> None:
         """
         Create a backup of a file
         :param file_src: path to the file to back up
         """
         # make a backup of the existing file
 
@@ -323,15 +339,16 @@
                     'Stored credentials are still valid, if you wish to switch to a different '
                     'account, run "UEVaultManager auth --delete" and try again.'
                 )
                 return
         except ValueError:
             pass
         except InvalidCredentialsError:
-            self.logger.error('Stored credentials were found but were no longer valid. Continuing with login...')
+            message = 'Stored credentials were found but were no longer valid. Continuing with login...'
+            self._log_gui_wrapper(self.logger.error, message)
             self.core.uevmlfs.invalidate_userdata()
 
         # Force an update check and notice in case there are API changes
         self.core.check_for_updates(force=True)
         self.core.force_show_update = True
 
         if args.import_egs_auth:
@@ -341,16 +358,16 @@
                     self.logger.info('Successfully imported login session from EGS!')
                     self.logger.info(f'Now logged in as user "{self.core.uevmlfs.userdata["displayName"]}"')
                     return
                 else:
                     self.logger.warning('Login session from EGS seems to no longer be valid.')
                     self.core.clean_exit(1)
             except Exception as error:
-                self.logger.error(f'No EGS login session found, please login manually. (Exception: {error!r})')
-                self.core.clean_exit(1)
+                message = f'No EGS login session found, please login manually. (Exception: {error!r})'
+                self._log_gui_wrapper(self.logger.critical, message, True)
 
         exchange_token = ''
         auth_code = ''
         if not args.auth_code and not args.session_id:
             # only import here since pywebview import is slow
             from UEVaultManager.utils.webview_login import webview_available, do_webview_login
 
@@ -367,15 +384,16 @@
                     auth_code = tmp['authorizationCode']
                 else:
                     auth_code = auth_code.strip('"')
             else:
                 if do_webview_login(callback_code=self.core.auth_ex_token):
                     self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}" via WebView')
                 else:
-                    self.logger.error('WebView login attempt failed, please see log for details.')
+                    message = 'WebView login attempt failed, please see log for details.'
+                    self._log_gui_wrapper(self.logger.error, message)
                 return
         elif args.session_id:
             exchange_token = self.core.auth_sid(args.session_id)
         elif args.auth_code:
             auth_code = args.auth_code
         elif args.ex_token:
             exchange_token = args.ex_token
@@ -385,15 +403,16 @@
             return
 
         if exchange_token and self.core.auth_ex_token(exchange_token):
             self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}"')
         elif auth_code and self.core.auth_code(auth_code):
             self.logger.info(f'Successfully logged in as "{self.core.uevmlfs.userdata["displayName"]}"')
         else:
-            self.logger.error('Login attempt failed, please see log for details.')
+            message = 'Login attempt failed, please see log for details.'
+            self._log_gui_wrapper(self.logger.error, message)
 
     def list_assets(self, args) -> None:
         """
         List assets in the vault
         :param args: options passed to the command
         """
 
@@ -454,14 +473,16 @@
                                 # update the list in the CSV record
                                 _csv_record[index] = ','.join(folder_list)
                         index += 1
 
                 _csv_record[price_index + 1] = old_price
             return _csv_record
 
+        # end update_and_merge_csv_record_data
+
         def update_and_merge_json_record_data(_asset, _items_in_file, _no_float_value: float, _no_bool_false_value: bool) -> dict:
             """
             Updates the data of the asset with the data from the items in the file
             :param _asset: asset to update
             :param _items_in_file: list of items in the file
             :param _no_float_value:  value to use when no float data is available
             :param _no_bool_false_value: value (False) to use when no bool data is available
@@ -487,43 +508,57 @@
                         _items_in_file[_asset_id]['Price']
                     )  # NOTE: the 'old price' is the 'price' saved in the file, not the 'old_price' in the file
                 except Exception as _error:
                     self.logger.warning(f'Old price values can not be converted for asset {_asset_id}\nError:{_error!r}')
                 _json_record['Old price'] = old_price
             return _json_record
 
+        # end def update_and_merge_json_record_data
+
         if self.core.create_log_backup:
             self.create_log_file_backup()
 
         # open log file for assets if necessary
         self.core.setup_assets_logging()
         self.core.egs.notfound_logger = self.core.notfound_logger
         self.core.egs.ignored_logger = self.core.ignored_logger
 
         output = sys.stdout  # by default, we output to sys.stdout
 
+        if args.output:
+            file_src = args.output
+            # test if the folder is writable
+            if not check_and_create_path(file_src):
+                message = f'Could not create folder for {file_src}. Exiting...'
+                self._log_gui_wrapper(self.logger.critical, message, True)
+            # we try to open it for writing
+            if not os.access(file_src, os.W_OK):
+                self.logger.warning(f'Could not read CSV record from the file {file_src}')
+                message = f'Could not create result file {file_src}. Exiting...'
+                self._log_gui_wrapper(self.logger.critical, message, True)
+
         self.logger.info('Logging in...')
         if not self.core.login():
-            self.logger.error('Login failed, cannot continue!')
-            self.core.clean_exit(1)
+            message = 'Login failed, cannot continue!'
+            self._log_gui_wrapper(self.logger.critical, message, True)
 
         if args.force_refresh:
             self.logger.info(
                 'force_refresh option is active ...\nRefreshing asset list, this will take several minutes to acheived depending on the internet connection...'
             )
         else:
             self.logger.info('Getting asset list... (this may take a while)')
 
         if args.filter_category and args.filter_category != gui_g.s.default_category_for_all:
             gui_g.UEVM_filter_category = args.filter_category
             self.logger.info(f'The String "{args.filter_category}" will be search in Assets category')
 
         gui_g.progress_window_ref = None
         progress_window = None
-        if args.gui:
+        if UEVaultManagerCLI.is_gui:
             uewm_gui_exists, progress_window = init_progress_window(args=args, logger=self.logger, callback=self.core.get_asset_list)
             if uewm_gui_exists:
                 # if the main gui is running, we already have a tk.mainloop running
                 # we need to constantly update the progress bar
                 while not progress_window.must_end:
                     progress_window.update()
             else:
@@ -595,20 +630,15 @@
                         # get the data (it's a dict)
                         for csv_record in csv_file_content:
                             # noinspection PyTypeChecker
                             asset_id = csv_record['Asset_id']
                             assets_in_file[asset_id] = csv_record
                         output.close()
                 except (FileExistsError, OSError, UnicodeDecodeError, StopIteration):
-                    self.logger.warning(f'Could not read CSV record from the file {args.output}')
-
-                # write the content of the file to keep some data
-                if not check_and_create_path(file_src):
-                    self.logger.critical(f'Could not create folder for {file_src}')
-                    self.core.clean_exit(1)
+                    self.logger.warning(f'Could not read CSV record from the file {file_src}')
                 # reopen file for writing
                 output = open(file_src, 'w', encoding='utf-8')
             # end if args.output:
 
             try:
                 writer = csv.writer(output, dialect='excel-tab' if args.tsv else 'excel', lineterminator='\n')
                 writer.writerow(CSV_headings.keys())
@@ -625,34 +655,32 @@
                         if len(assets_in_file) > 0:
                             csv_record_merged = update_and_merge_csv_record_data(asset, assets_in_file, no_int_data)
                         else:
                             csv_record_merged = list(asset[1].values())
                         cpt += 1
                         writer.writerow(csv_record_merged)
                     except (OSError, UnicodeEncodeError, TypeError) as error:
-                        self.logger.error(f'Could not write CSV record for {asset_id} into {args.output}\nError:{error!r}')
-            except OSError:
-                self.logger.error(f'Could not write list result to {args.output}')
+                        message = f'Could not write CSV record for {asset_id} into {args.output}\nError:{error!r}'
+                        self.logger.error(message)
+            except (OSError, ValueError) as error:
+                message = f'Could not write list result to {args.output}: {error!r}'
+                self._log_gui_wrapper(self.logger.error, message)
+
         # end if args.csv or args.tsv:
 
         if args.json:
             if args.output:
                 file_src = args.output
                 # If the output file exists, we read its content to keep some data
                 try:
                     with open(file_src, 'r', encoding='utf-8') as output:
                         assets_in_file = json.load(output)
                         output.close()
                 except (FileExistsError, OSError, UnicodeDecodeError, StopIteration, json.decoder.JSONDecodeError):
                     self.logger.warning(f'Could not read Json record from the file {args.output}')
-
-                # write the content of the file to keep some data
-                if not check_and_create_path(file_src):
-                    self.logger.critical(f'Could not create folder for {file_src}')
-                    self.core.clean_exit(1)
                 # reopen file for writing
                 output = open(file_src, 'w', encoding='utf-8')
             # end if args.output:
 
             try:
                 cpt = 0
                 json_content = {}
@@ -670,29 +698,32 @@
                         json_record_merged = asset[1]
                     #      output.write(",\n")
                     try:
                         asset_id = json_record_merged['Asset_id']
                         json_content[asset_id] = json_record_merged
                         cpt += 1
                     except (OSError, UnicodeEncodeError, TypeError) as error:
-                        self.logger.error(f'Could not write Json record for {asset_id} into {args.output}\nError:{error!r}')
+                        message = f'Could not write Json record for {asset_id} into {args.output}\nError:{error!r}'
+                        self.logger.error(message)
 
                 json.dump(json_content, output, indent=2)
             except OSError:
-                self.logger.error(f'Could not write list result to {args.output}')
+                message = f'Could not write list result to {args.output}'
+                self._log_gui_wrapper(self.logger.error, message)
+
             # end if args.json:
 
-        if args.csv or args.tsv or args.json or args.input or args.gui:
+        if args.csv or args.tsv or args.json or UEVaultManagerCLI.is_gui:
             # close the opened file
             if output is not None:
                 output.close()
             self.logger.info(
                 f'\n======\n{cpt} assets have been printed or saved (without duplicates due to different UE versions)\nOperation Finished\n======\n'
             )
-            if args.gui:
+            if UEVaultManagerCLI.is_gui:
                 # During the editabletable initial rebuild_data process, the window will not close
                 # So we try to close it several times
                 max_tries = 3
                 progress_window.quit_on_close = True  # gentle quit
                 tries = 0
                 while progress_window is not None and progress_window.winfo_viewable() and tries < max_tries:
                     progress_window.close_window()
@@ -724,21 +755,21 @@
         # check if we even need to log in
         if args.override_manifest:
             self.logger.info(f'Loading manifest from "{args.override_manifest}"')
             manifest_data, _ = self.core.get_uri_manifest(args.override_manifest)
         else:
             self.logger.info(f'Logging in and downloading manifest for {args.app_name}')
             if not self.core.login():
-                self.logger.error('Login failed! Cannot continue with download process.')
-                self.core.clean_exit(1)
+                message = 'Login failed! Cannot continue with download process.'
+                self._log_gui_wrapper(self.logger.critical, message, True)
             update_meta = args.force_refresh
             item = self.core.get_item(args.app_name, update_meta=update_meta)
             if not item:
-                self.logger.critical(f'Could not fetch metadata for "{args.app_name}" (check spelling/account ownership)')
-                self.core.clean_exit(1)
+                message = f'Could not fetch metadata for "{args.app_name}" (check spelling/account ownership). Exiting...'
+                self._log_gui_wrapper(self.logger.critical, message, True)
             manifest_data, _ = self.core.get_cdn_manifest(item, platform='Windows')
 
         manifest = self.core.load_manifest(manifest_data)
         files = sorted(manifest.file_manifest_list.elements, key=lambda a: a.filename.lower())
 
         content = ''
         if args.hashlist:
@@ -761,15 +792,15 @@
                 content += fm.filename + '\n'
                 for t in fm.install_tags:
                     install_tags.add(t)
             if install_tags:
                 # use the log output so this isn't included when piping file list into file
                 self.logger.info(f'Install tags: {", ".join(sorted(install_tags))}')
 
-        if args.gui:
+        if UEVaultManagerCLI.is_gui:
             uewm_gui_exists, _ = init_display_window(self.logger)
             custom_print(content, keep_mode=False)  # as it, next print will not keep the content
             if not uewm_gui_exists:
                 gui_g.UEVM_gui_ref.mainloop()
         else:
             print(content)
 
@@ -777,16 +808,16 @@
         """
         Print the information about the vault and the available assets
         :param args: options passed to the command
         """
         if not args.offline:
             try:
                 if not self.core.login():
-                    self.logger.error('Log in failed!')
-                    self.core.clean_exit(1)
+                    message = 'Log in failed!'
+                    self._log_gui_wrapper(self.logger.critical, message, True)
             except ValueError:
                 pass
             # if automatic checks are off force an update here
             self.core.check_for_updates(force=True)
 
         if not self.core.uevmlfs.userdata:
             user_name = '<not logged in>'
@@ -823,15 +854,15 @@
                 json_content['Release summary'] = update_information['summary']
                 json_content['Release Url'] = update_information['release_url']
                 json_content['Update recommendation'] = update_information['severity']
 
         if args.json:
             return self._print_json(json_content, args.pretty_json)
 
-        if args.gui:
+        if UEVaultManagerCLI.is_gui:
             uewm_gui_exists, _ = init_display_window(self.logger)
             json_print_key_val(json_content, output_on_gui=True)
             if not uewm_gui_exists:
                 gui_g.UEVM_gui_ref.mainloop()
         else:
             json_print_key_val(json_content)
 
@@ -849,16 +880,16 @@
             manifest_uri = name_or_path
         else:
             app_name = self._resolve_aliases(name_or_path)
 
         if not args.offline and not manifest_uri:
             try:
                 if not self.core.login():
-                    self.logger.error('Log in failed!')
-                    self.core.clean_exit(1)
+                    message = 'Log in failed!'
+                    self._log_gui_wrapper(self.logger.critical, message, True)
             except ValueError:
                 pass
 
         # lists that will be printed or turned into JSON data
         info_items = dict(assets=list(), manifest=list(), install=list())
         InfoItem = namedtuple('InfoItem', ['name', 'json_name', 'value', 'json_value'])
 
@@ -1005,36 +1036,36 @@
                 elif isinstance(local_item.value, dict):
                     custom_print(f'- {local_item.name}:')
                     for k, v in local_item.value.items():
                         custom_print(f' + {k} : {v}')
                 else:
                     custom_print(f'- {local_item.name}: {local_item.value}')
 
-            if args.gui:
+            if UEVaultManagerCLI.is_gui:
                 uewm_gui_exists, _ = init_display_window(self.logger)
             else:
                 uewm_gui_exists = False
 
             if info_items.get('asset'):
-                custom_print('\nAsset Information:')
+                custom_print('Asset Information:')
                 for info_item in info_items['asset']:
                     print_info_item(info_item)
             if info_items.get('install'):
-                custom_print('\nInstallation information:')
+                custom_print('Installation information:')
                 for info_item in info_items['install']:
                     print_info_item(info_item)
             if info_items.get('manifest'):
-                custom_print('\nManifest information:')
+                custom_print('Manifest information:')
                 for info_item in info_items['manifest']:
                     print_info_item(info_item)
 
             if not any(info_items.values()):
                 custom_print('No asset information available.')
             custom_print(keep_mode=False)  # as it, next print will not keep the content
-            if args.gui and not uewm_gui_exists:
+            if UEVaultManagerCLI.is_gui and not uewm_gui_exists:
                 gui_g.UEVM_gui_ref.mainloop()
         else:
             json_out = dict(asset=dict(), install=dict(), manifest=dict())
             if info_items.get('asset'):
                 for info_item in info_items['asset']:
                     json_out['asset'][info_item.json_name] = info_item.json_value
             if info_items.get('install'):
@@ -1051,45 +1082,59 @@
 
     def cleanup(self, args) -> None:
         """
         Cleans up the local assets data folders and logs
         :param args: options passed to the command
         """
         before = self.core.uevmlfs.get_dir_size()
+        uewm_gui_exists = False
+        if UEVaultManagerCLI.is_gui:
+            uewm_gui_exists, _ = init_display_window(self.logger)
 
         # delete metadata
         if args.delete_metadata:
-            self.logger.debug('Removing app metadata...')
-            self.core.uevmlfs.clean_metadata()
+            message = 'Removing app metadata...'
+            custom_print(message)
+            self.core.uevmlfs.clean_metadata(app_names_to_keep=[])
 
         # delete extras data
         if args.delete_extras_data:
-            self.logger.debug('Removing app extras data...')
-            self.core.uevmlfs.clean_extras()
+            message = 'Removing app extras data...'
+            custom_print(message)
+            self.core.uevmlfs.clean_extras(app_names_to_keep=[])
 
         # delete log and backup
-        self.logger.debug('Removing logs and backups...')
+        message = 'Removing logs and backups...'
+        custom_print(message)
         self.core.uevmlfs.clean_logs_and_backups()
 
-        self.logger.debug('Removing manifests...')
+        message = 'Removing manifests...'
+        custom_print(message)
         self.core.uevmlfs.clean_manifests()
 
-        self.logger.debug('Removing tmp data')
+        message = 'Removing tmp data...'
+        custom_print(message)
         self.core.uevmlfs.clean_tmp_data()
 
         after = self.core.uevmlfs.get_dir_size()
-        self.logger.info(f'Cleanup complete! Removed {(before - after) / 1024 / 1024:.02f} MiB.')
+        message = f'Cleanup complete! Removed {(before - after) / 1024 / 1024:.02f} MiB.'
+        self.logger.info(message)
+        custom_print(message, keep_mode=False)
+
+        if not uewm_gui_exists:
+            gui_g.UEVM_gui_ref.mainloop()
 
     def get_token(self, args) -> None:
         """
         Gets the access token for the current user
         :param args: options passed to the command
         """
         if not self.core.login(force_refresh=args.bearer):
-            self.logger.error('Login failed!')
+            message = 'Log in failed!'
+            self._log_gui_wrapper(self.logger.critical, message)
             return
 
         if args.bearer:
             args.json = True
             token = dict(
                 token_type='bearer',
                 access_token=self.core.egs.user['access_token'],
@@ -1124,17 +1169,24 @@
         gui_g.UEVM_log_ref = self.logger
         gui_g.UEVM_cli_ref = self
 
         # set output file name from the input one. Used by the "rebuild file content" button (or rebuild_data method)
         init_gui_args(args, additional_args={'output': input_filename})
         rebuild = False
         if not os.path.isfile(input_filename):
-            input_filename = gui_fn.create_empty_file(input_filename)
+            is_valid, input_filename = gui_fn.create_empty_file(input_filename)
             rebuild = True
-
+            if not is_valid:
+                message = f'Error while creating the empty result file with the given path. The following file {input_filename} will be used as default'
+                self._log_gui_wrapper(self.logger.error, message)
+                # fix invalid input/output file name in arguments to avoid futher errors in file path checks
+                args.input = input_filename
+                args.output = input_filename
+                gui_g.UEVM_cli_args['input'] = input_filename
+                gui_g.UEVM_cli_args['output'] = input_filename
         gui_g.UEVM_gui_ref = UEVMGui(
             title=gui_g.s.app_title,
             width=gui_g.s.app_width,
             height=gui_g.s.app_height,
             icon=app_icon_filename,
             screen_index=0,
             file=input_filename,
@@ -1154,15 +1206,15 @@
         if parser is None:
             parser = gui_g.UEVM_parser_ref
         if parser is None:
             return
         uewm_gui_exists = False
 
         if args.full_help or forced:
-            if args.gui:
+            if UEVaultManagerCLI.is_gui:
                 uewm_gui_exists, _ = init_display_window()
             custom_print(keep_mode=False, text=parser.format_help())
 
             # Commands that should not be shown in full help/list of commands (e.g. aliases)
             _hidden_commands = {'download', 'update', 'repair', 'get-token', 'verify-asset', 'list-assets'}
             # Print the help for all the subparsers. Thanks stackoverflow!
             custom_print(text='Individual command help:')
@@ -1184,15 +1236,15 @@
                 subprocess.Popen(['cmd', '/K', 'echo>nul'])
         else:
             # on non-windows systems
             # UEVaultManagerCLI.print_help(args, parser=parser, forced=True)
             UEVaultManagerCLI.print_version()
             return
 
-        if args.gui and not uewm_gui_exists:
+        if UEVaultManagerCLI.is_gui and not uewm_gui_exists:
             gui_g.UEVM_gui_ref.mainloop()
 
     @staticmethod
     def print_version():
         """
         Prints the version of UEVaultManager and exit
         """
@@ -1408,14 +1460,19 @@
 
     cli.core.engine_version_for_obsolete_assets = cli.core.uevmlfs.config.get('UEVaultManager', 'engine_version_for_obsolete_assets', fallback='4.26')
 
     # if --yes is used as part of the subparsers arguments manually set the flag in the main parser.
     if '-y' in extra or '--yes' in extra:
         args.yes = True
 
+    try:
+        UEVaultManagerCLI.is_gui = args.gui
+    except (AttributeError, KeyError):
+        UEVaultManagerCLI.is_gui = False
+
     # technically args.func() with set defaults could work (see docs on subparsers)
     # but that would require all funcs to accept args and extra...
     try:
         if args.subparser_name == 'auth':
             cli.auth(args)
         elif args.subparser_name in {'list', 'list-assets'}:
             cli.list_assets(args)
@@ -1426,18 +1483,21 @@
         elif args.subparser_name == 'info':
             cli.info(args)
         elif args.subparser_name == 'cleanup':
             cli.cleanup(args)
         elif args.subparser_name == 'get-token':
             cli.get_token(args)
         elif args.subparser_name in {'edit', 'edit-assets'}:
+            args.gui = True
+            UEVaultManagerCLI.is_gui = True
             cli.edit_assets(args)
         elif start_in_edit_mode:
-            args.subparser_name = 'edit'
             args.gui = True
+            UEVaultManagerCLI.is_gui = True
+            args.subparser_name = 'edit'
             args.input = init_gui(False)
             cli.edit_assets(args)
     except KeyboardInterrupt:
         cli.logger.info('Command was aborted via KeyboardInterrupt, cleaning up...')
 
     # Disable the update message if JSON/TSV/CSV outputs are used
     disable_update_message = False
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/core.py` & `UEVaultManager-1.6.7/UEVaultManager/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,38 +117,42 @@
         self.engine_version_for_obsolete_assets = '4.26'
 
     def setup_assets_logging(self) -> None:
         """
         Setup logging for ignored, not found and bad data assets
         """
 
-        def create_logger(logger_name: str, filename_log: str) -> None:
+        def create_logger(logger_name: str, filename_log: str):
             """
             Create a logger for ignored, not found and bad data assets
             :param logger_name:   
             :param filename_log: 
             :return: 
             """
             filename_log = filename_log.replace('~/.config', self.uevmlfs.path)
             if check_and_create_path(filename_log):
                 handler = logging.FileHandler(filename_log, mode='w')
                 handler.setFormatter(formatter)
                 logger = logging.Logger(logger_name, 'INFO')
                 logger.addHandler(handler)
                 logger.info(message)
+                return logger
+            else:
+                self.log.warning(f'Unable to create logger for file: {filename_log}')
+                return None
 
         formatter = logging.Formatter('%(message)s')
         message = f"-----\n{datetime.now().strftime(self.default_datetime_format)} Log Started\n-----\n"
 
         if self.ignored_assets_filename_log:
-            create_logger('IgnoredAssets', self.ignored_assets_filename_log)
+            self.ignored_logger = create_logger('IgnoredAssets', self.ignored_assets_filename_log)
         if self.notfound_assets_filename_log:
-            create_logger('NotFoundAssets', self.notfound_assets_filename_log)
+            self.notfound_logger = create_logger('NotFoundAssets', self.notfound_assets_filename_log)
         if self.bad_data_assets_filename_log:
-            create_logger('BadDataAssets', self.bad_data_assets_filename_log)
+            self.bad_data_logger = create_logger('BadDataAssets', self.bad_data_assets_filename_log)
 
     def auth_sid(self, sid) -> str:
         """
         Handles getting an exchange code from an id
         :param sid: session id
         :return: exchange code
         """
@@ -492,15 +496,21 @@
 
                 # log the asset if the title in metadata and the title in the marketplace grabbed page are not identical
                 if eg_extras['page_title'] != '' and eg_extras['page_title'] != apps[name].app_title:
                     self.log.warning(f'{name} has incoherent data. It has been added to the bad_data_logger file')
                     eg_extras['grab_result'] = GrabResult.INCONSISTANT_DATA.name
                     if self.bad_data_logger:
                         self.bad_data_logger.info(name)
-
+            else:
+                # if we don't process extras, we still need to add the asset to the log corresponding to their grab_result
+                eg_extras = self.uevmlfs.assets_extras_data[app_name]
+                if eg_extras['grab_result'] == GrabResult.INCONSISTANT_DATA.name and self.bad_data_logger:
+                    self.bad_data_logger.info(name)
+                if eg_extras['grab_result'] == GrabResult.CONTENT_NOT_FOUND.name and self.notfound_logger:
+                    self.notfound_logger.info(name)
             # compute process time and average in s
             end_time = datetime.now()
             process_time = (end_time - start_time).total_seconds()
             self.process_time_average['time'] += process_time
             self.process_time_average['count'] += 1
 
             if fetch_list.get(name):
@@ -518,14 +528,15 @@
             self.log.info(
                 f'--- END fetching data in {name}{thread_data}. Time For Processing={process_time:.3f}s # Still {len(fetch_list)} assets to process'
             )
             if gui_g.progress_window_ref is not None and not gui_g.progress_window_ref.update_and_continue(increment=1):
                 self.thread_executor_must_stop = True
                 return False
             return True
+        # end of fetch_asset_meta
 
         _ret = []
         meta_updated = False
 
         # fetch asset information for Windows, all installed platforms, and the specified one
         platforms = {'Windows'}
         platforms |= {platform}
@@ -642,15 +653,15 @@
                 self.log.debug(f'Scheduling metadata and extras update for {app_name}')
                 # namespace/catalog item are the same for all platforms, so we can just use the first one
                 _ga = next(iter(app_assets.values()))
                 fetch_list[app_name] = (app_name, _ga.namespace, _ga.catalog_item_id, process_meta, process_extras)
                 meta_updated = True
             i += 1
             filtered_items.append(item)
-            # end while i < len(valid_items):
+        # end while i < len(valid_items):
 
         # setup and teardown of thread pool takes some time, so only do it when it makes sense.
         self.use_threads = len(fetch_list) > 5
         # self.use_threads = False  # test only
         if fetch_list:
             if gui_g.progress_window_ref is not None:
                 gui_g.progress_window_ref.reset(
@@ -744,21 +755,21 @@
         self.update_aliases(force=meta_updated)
 
         if gui_g.s.never_update_data_files:
             meta_updated = False
         if meta_updated:
             if gui_g.progress_window_ref is not None:
                 gui_g.progress_window_ref.reset(new_value=0, new_text="Updating metadata files...", new_max_value=len(_ret))
-            # delete old files
+            self.log.info(f'Updating metadata files...Could take a some time')
             self._prune_metadata()
             self._save_metadata(_ret)
         if meta_updated:
             if gui_g.progress_window_ref is not None:
                 gui_g.progress_window_ref.reset(new_value=0, new_text="Updating extras data files...", new_max_value=len(_ret))
-            # save new ones
+            self.log.info(f'Updating extras data files...Could take a some time')
             self._prune_extras_data(update_global_dict=False)
             self._save_extras_data(self.uevmlfs.assets_extras_data, update_global_dict=False)
         return _ret
 
     # end def get_asset_list(self, update_assets=True, platform='Windows', filter_category='') -> (List[App], Dict[str, List[App]]):
 
     def _prune_metadata(self) -> None:
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/downloader/mp/manager.py` & `UEVaultManager-1.6.7/UEVaultManager/downloader/mp/manager.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/downloader/mp/workers.py` & `UEVaultManager-1.6.7/UEVaultManager/downloader/mp/workers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/lfs/egl.py` & `UEVaultManager-1.6.7/UEVaultManager/lfs/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/lfs/eos.py` & `UEVaultManager-1.6.7/UEVaultManager/lfs/eos.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/lfs/uevmlfs.py` & `UEVaultManager-1.6.7/UEVaultManager/lfs/uevmlfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,15 @@
         """
         Delete all the metadata files that are not in the app_names_to_keep list
         """
         self.delete_folder(self.manifests_folder)
 
     def clean_logs_and_backups(self) -> None:
         """
-        Delete all the log and backup files
+        Delete all the log and backup files in the app folder
         """
         for f in os.listdir(self.path):
             file_name_no_ext, file_ext = os.path.splitext(f)
             if '.log' in file_ext or '.bak' in file_ext:
                 try:
                     os.remove(os.path.join(self.path, f))
                 except Exception as error:
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/lfs/utils.py` & `UEVaultManager-1.6.7/UEVaultManager/lfs/utils.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/lfs/windows_helpers.py` & `UEVaultManager-1.6.7/UEVaultManager/lfs/windows_helpers.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/app.py` & `UEVaultManager-1.6.7/UEVaultManager/models/app.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/chunk.py` & `UEVaultManager-1.6.7/UEVaultManager/models/chunk.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/config.py` & `UEVaultManager-1.6.7/UEVaultManager/models/config.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/csv.py` & `UEVaultManager-1.6.7/UEVaultManager/models/csv.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/downloading.py` & `UEVaultManager-1.6.7/UEVaultManager/models/downloading.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/egl.py` & `UEVaultManager-1.6.7/UEVaultManager/models/egl.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/json_manifest.py` & `UEVaultManager-1.6.7/UEVaultManager/models/json_manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/models/manifest.py` & `UEVaultManager-1.6.7/UEVaultManager/models/manifest.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/main.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             Set to False for running the GUI initialization only, useful if called from cli.py
     :return: the path to the csv file to use at startup. It's used when the window is opened from the cli.py script
     """
     app_icon_filename = gui_fn.path_from_relative_to_absolute(gui_g.s.app_icon_filename)
     csv_filename = gui_fn.path_from_relative_to_absolute(gui_g.s.csv_filename)
     rebuild = False
     if not os.path.isfile(csv_filename):
-        csv_filename = gui_fn.create_empty_file(csv_filename)
+        _, csv_filename = gui_fn.create_empty_file(csv_filename)
         rebuild = True
     if open_mainwindow:
         main_window = UEVMGui(
             title=gui_g.s.app_title,
             width=gui_g.s.app_width,
             height=gui_g.s.app_height,
             icon=app_icon_filename,
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/DisplayContentWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditCellWindowClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditCellWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditRowWindowClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditRowWindowClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/EditableTableClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/EditableTableClass.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,70 +93,82 @@
         #  'cubehelix', 'flag', 'gist_earth', 'gist_gray', 'gist_heat', 'gist_ncar', 'gist_rainbow', 'gist_stern', 'gist_yarg', 'gnuplot', 'gnuplot2',
         #  'gray', 'hot', 'hsv', 'jet', 'nipy_spectral', 'ocean', 'pink', 'prism', 'rainbow', 'seismic', 'spring', 'summer', 'tab10', 'tab20', 'tab20b',
         #  'tab20c', 'terrain', 'winter'
 
         if col_names is None:
             return
         df = self.data_filtered if self.data_filtered is not None else self.model.df
-        for colname in col_names:
-            x = df[colname]
+        for col_name in col_names:
+            try:
+                x = df[col_name]
+            except KeyError:
+                log_debug(f'gradient_color_cells: Column {col_name} not found in the table data.')
+                continue
             clrs = self.values_to_colors(x, cmap, alpha)
             clrs = pd.Series(clrs, index=df.index)
             rc = self.rowcolors
-            rc[colname] = clrs
+            rc[col_name] = clrs
 
     def color_cells_if(self, col_names=None, color='green', value_to_check='True') -> None:
         """
         Set the cell color for the specified columns and the cell with a given value.
         :param col_names: The names of the columns to create a gradient color for.
         :param color: The color to set the cell to.
         :param value_to_check: The value to check for.
         """
 
         if col_names is None:
             return
         df = self.data_filtered if self.data_filtered is not None else self.model.df
         for col_name in col_names:
-            if col_name not in df.columns:
+            try:
+                mask = df[col_name] == value_to_check
+            except KeyError:
+                log_debug(f'color_cells_if: Column {col_name} not found in the table data.')
                 continue
-            mask = df[col_name] == value_to_check
             self.setColorByMask(col=col_name, mask=mask, clr=color)
 
     def color_cells_if_not(self, col_names=None, color='grey', value_to_check='False') -> None:
         """
         Set the cell color for the specified columns and the cell with NOT a given value.
         :param col_names: The names of the columns to create a gradient color for.
         :param color: The color to set the cell to.
         :param value_to_check: The value to check for.
         """
         if col_names is None:
             return
         df = self.data_filtered if self.data_filtered is not None else self.model.df
         for col_name in col_names:
-            if col_name not in df.columns:
+            try:
+                mask = df[col_name] != value_to_check
+            except KeyError:
+                log_debug(f'color_cells_if_not: Column {col_name} not found in the table data.')
                 continue
-            mask = df[col_name] != value_to_check
             self.setColorByMask(col=col_name, mask=mask, clr=color)
 
     def color_rows_if(self, col_names=None, color='#55555', value_to_check='True') -> None:
         """
         Set the row color for the specified columns and the rows with a given value.
         :param col_names: The names of the columns to check for the value.
         :param color: The color to set the row to.
         :param value_to_check: The value to check for.
         """
         if col_names is None:
             return
         df = self.data_filtered if self.data_filtered is not None else self.model.df
 
         for col_name in col_names:
+            row_indices = []
             if col_name not in df.columns:
                 continue
-            row_indices = []
-            mask = df[col_name]
+            try:
+                mask = df[col_name]
+            except KeyError:
+                log_debug(f'color_rows_if: Column {col_name} not found in the table data.')
+                continue
             for i in range(min(self.rows_per_page, len(mask))):
                 try:
                     if str(mask[i]) == value_to_check:
                         row_indices.append(i)
                 except KeyError:
                     log_debug(f'KeyError for row {i} in color_rows_if')
             if len(row_indices) > 0:  # Check if there are any row indices
@@ -740,15 +752,15 @@
         :param row: The row index of the selected cell.
         :return: The image URL of the selected row.
         """
         if row is None:
             return ''
         try:
             return self.model.getValueAt(row, col=self.model.df.columns.get_loc('Image'))
-        except IndexError:
+        except (IndexError, KeyError):
             return ''
 
     def open_asset_url(self, url: str = None):
         """
         Opens the asset URL in a web browser.
         :param url: The URL to open.
         """
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/ExtendedWidgetClasses.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/GUISettingsClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/GUISettingsClass.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 
 from termcolor import colored
 
 import UEVaultManager.tkgui.modules.functions_no_deps as gui_fn
 from UEVaultManager.lfs.utils import clean_filename
 from UEVaultManager.models.config import AppConf
+from UEVaultManager import __name__, __version__, __codename__
 
 # NOTE : we can't import the following modules here because of circular dependencies
 # UEVaultManager.tkgui.modules.functions_no_deps
 
 
 def log(msg: str) -> None:
     """
@@ -65,15 +66,15 @@
 
         if self.config_vars['reopen_last_file'] and os.path.isfile((self.config_vars['last_opened_file'])):
             self.csv_filename = self.config_vars['last_opened_file']
         else:
             self.csv_filename = os.path.join(self.config_vars['results_folder'], 'list.csv')
 
         self.csv_filename = os.path.normpath(self.csv_filename)
-        self.app_title = 'UEVM Gui'
+        self.app_title = f'{__name__} Gui v{__version__} ({__codename__})'
         self.app_width = 1600
         self.app_height = 935
         self.app_monitor = 1
         self.csv_datetime_format = '%Y-%m-%d %H:%M:%S'
         self.data_filetypes = (('csv file', '*.csv'), ('tcsv file', '*.tcsv'), ('json file', '*.json'), ('text file', '*.txt'))
         self.preview_max_width = 150
         self.preview_max_height = 150
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/ProgressWindowsClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/ProgressWindowsClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/SaferDictClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/SaferDictClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/TaggedLabelFrameClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/UEVMGuiClass.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,30 +73,32 @@
         self.bind('<Key>', self.on_key_press)
         # Bind the table to the mouse motion event
         self.editable_table.bind('<Motion>', self.on_mouse_over_cell)
         self.editable_table.bind('<Leave>', self.on_mouse_leave_cell)
         self.editable_table.bind('<<CellSelectionChanged>>', self.on_selection_change)
         self.protocol('WM_DELETE_WINDOW', self.on_close)
 
-        if show_open_file_dialog:
-            if self.load_file() == '':
-                gui_f.log_error('This application could not run without a file to read data from')
-                self.quit()
-
-        # Quick edit the first row
-        self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=0)
-
-        if rebuild_data or self.editable_table.must_rebuild:
-            if gui_f.box_okcancel('Data are invalid or empty. They will be rebuilt from sources files. Do you want to continue ?'):
+        if not show_open_file_dialog and (rebuild_data or self.editable_table.must_rebuild):
+            if gui_f.box_yesno('Data file is invalid or empty. Do you want to rebuild data from sources files ?'):
                 if not self.editable_table.rebuild_data():
                     gui_f.log_error('Rebuild data error. This application could not run without a file to read from or some data to build from it')
                     self.destroy()  # self.quit() won't work here
                     return
+            elif gui_f.box_yesno('So, do you want to load another file ? If not, the application will be closed'):
+                show_open_file_dialog = True
             else:
                 self.destroy()  # self.quit() won't work here
+                gui_f.log_error('No valid file to read from. Application will be closed',)
+
+        if show_open_file_dialog:
+            if self.load_file() == '':
+                gui_f.log_error('This application could not run without a file to read data from')
+                self.quit()
+        # Quick edit the first row
+        self.editable_table.update_quick_edit(quick_edit_frame=self.control_frame.lbtf_quick_edit, row=0)
 
     class ToolbarFrame(ttk.Frame):
         """
         This class is used to create the toolbar frame
         :param container: The parent container
         """
 
@@ -149,16 +151,18 @@
             lblf_commands.pack(side=tk.LEFT, **lblf_def_options)
             btn_help = ttk.Button(lblf_commands, text='Help', command=lambda: container.run_cli_command('print_help'))
             btn_help.pack(**pack_def_options, side=tk.LEFT)
             btn_status = ttk.Button(lblf_commands, text='Status', command=lambda: container.run_cli_command('status'))
             btn_status.pack(**pack_def_options, side=tk.LEFT)
             btn_info = ttk.Button(lblf_commands, text='Info', command=lambda: container.run_cli_command('info'))
             btn_info.pack(**pack_def_options, side=tk.LEFT)
-            btn_info = ttk.Button(lblf_commands, text='List Files', command=lambda: container.run_cli_command('list_files'))
-            btn_info.pack(**pack_def_options, side=tk.LEFT)
+            btn_list_files = ttk.Button(lblf_commands, text='List Files', command=lambda: container.run_cli_command('list_files'))
+            btn_list_files.pack(**pack_def_options, side=tk.LEFT)
+            btn_cleanup = ttk.Button(lblf_commands, text='Cleanup', command=lambda: container.run_cli_command('cleanup'))
+            btn_cleanup.pack(**pack_def_options, side=tk.LEFT)
 
             lblf_actions = ttk.LabelFrame(self, text='Actions')
             lblf_actions.pack(side=tk.RIGHT, **lblf_def_options)
             # noinspection PyArgumentList
             btn_toggle_options = ttk.Button(lblf_actions, text='Show Options', command=container.toggle_options_pane, state=tk.DISABLED)
             btn_toggle_options.pack(**pack_def_options, side=tk.LEFT)
             # noinspection PyArgumentList
@@ -377,25 +381,40 @@
             force_refresh_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('force', False))
             force_refresh_var.trace_add('write', lambda name, index, mode: gui_g.set_args_force_refresh(force_refresh_var.get()))
             ck_force_refresh = ttk.Checkbutton(lblf_options, text='Force refresh', variable=force_refresh_var)
             ck_force_refresh.grid(row=cur_row, column=cur_col, **grid_fw_options)
             # row 1
             cur_row += 1
             cur_col = 0
-            offline_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('offli', False))
+            offline_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('offline', False))
             offline_var.trace_add('write', lambda name, index, mode: gui_g.set_args_offline(offline_var.get()))
             ck_offline = ttk.Checkbutton(lblf_options, text='Offline Mode', variable=offline_var)
             ck_offline.grid(row=cur_row, column=cur_col, **grid_fw_options)
             # row 2
             cur_row += 1
             cur_col = 0
             debug_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('debug', False))
             debug_var.trace_add('write', lambda name, index, mode: gui_g.set_args_debug(debug_var.get()))
             ck_debug = ttk.Checkbutton(lblf_options, text='Debug mode', variable=debug_var)
             ck_debug.grid(row=cur_row, column=cur_col, **grid_fw_options)
+            # row 3
+            # delete_extras_data'] = True
+            cur_row += 1
+            cur_col = 0
+            delete_metadata_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('delete_metadata', False))
+            delete_metadata_var.trace_add('write', lambda name, index, mode: gui_g.set_args_delete_metadata(delete_metadata_var.get()))
+            ck_delete_metadata = ttk.Checkbutton(lblf_options, text='Delete metadata (cleanup)', variable=delete_metadata_var)
+            ck_delete_metadata.grid(row=cur_row, column=cur_col, **grid_fw_options)
+            # row 4
+            cur_row += 1
+            cur_col = 0
+            delete_extras_data_var = tk.BooleanVar(value=gui_g.UEVM_cli_args.get('delete_extras_data', False))
+            delete_extras_data_var.trace_add('write', lambda name, index, mode: gui_g.set_args_delete_extras_data(delete_extras_data_var.get()))
+            ck_delete_extras_data = ttk.Checkbutton(lblf_options, text='Delete metadata (cleanup)', variable=delete_extras_data_var)
+            ck_delete_extras_data.grid(row=cur_row, column=cur_col, **grid_fw_options)
 
     def _open_file_dialog(self, save_mode=False, filename=None) -> str:
         """
         Open a file dialog to choose a file to save or load data to/from
         :param save_mode: if True, the dialog will be in saving mode, else in loading mode
         :param filename: the default filename to use
         :return: the chosen filename
@@ -787,21 +806,21 @@
         """
         Update the category variable with the current categories in the data
         :return: a dict with the new categories list as value and the key is the name of the variable.
         """
         try:
             # if the file is empty or absent or invalid when creating the class, the data is empty, so no categories
             categories = list(self.editable_table.data['Category'].cat.categories)
-        except (AttributeError, TypeError):
+        except (AttributeError, TypeError, KeyError):
             categories = []
         categories.insert(0, gui_g.s.default_category_for_all)
         try:
             # if the file is empty or absent or invalid when creating the class, the data is empty, so no categories
             grab_results = list(self.editable_table.data['Grab result'].cat.categories)
-        except (AttributeError, TypeError):
+        except (AttributeError, TypeError, KeyError):
             grab_results = []
         grab_results.insert(0, gui_g.s.default_category_for_all)
         return {'categories': categories, 'grab_results': grab_results}
 
     def reload_data(self) -> None:
         """
         Reload the data from the file
@@ -824,34 +843,39 @@
             if self.editable_table.rebuild_data():
                 gui_f.box_message(f'Data rebuilt from {self.editable_table.file}')
                 self.update_page_numbers()
                 self.update_category_var()
 
     def run_cli_command(self, command_name='') -> None:
         """
-        Execute the 'status' command and display the result in DisplayContentWindow
+        Execute a cli command and display the result in DisplayContentWindow
         :param command_name: the name of the command to execute
         """
         if command_name == '':
             return
         if gui_g.UEVM_cli_ref is None:
             gui_f.from_cli_only_message()
             return
         row = self.editable_table.getSelectedRow()
         col = self.editable_table.model.df.columns.get_loc('App name')
         app_name = self.editable_table.model.getValueAt(row, col)
-
-        # gui_g.UEVM_cli_args['offline'] = True  # speed up some commands
+        # gui_g.UEVM_cli_args['offline'] = True  # speed up some commands DEBUG ONLY
         # set default options for the cli command to execute
-        gui_g.UEVM_cli_args['gui'] = True
-        gui_g.UEVM_cli_args['full_help'] = True
+        gui_g.UEVM_cli_args['gui'] = True  # mandatory for displaying the result in the DisplayContentWindow
+        # arguments for various commands
         gui_g.UEVM_cli_args['csv'] = False  # mandatory for displaying the result in the DisplayContentWindow
         gui_g.UEVM_cli_args['tcsv'] = False  # mandatory for displaying the result in the DisplayContentWindow
         gui_g.UEVM_cli_args['json'] = False  # mandatory for displaying the result in the DisplayContentWindow
+        # arguments for cleanup command
+        # now set in command options
+        # gui_g.UEVM_cli_args['delete_extras_data'] = True
+        # gui_g.UEVM_cli_args['delete_metadata'] = True
 
+        # arguments for help command
+        gui_g.UEVM_cli_args['full_help'] = True
         if app_name != '':
             gui_g.UEVM_cli_args['app_name'] = app_name
 
         if gui_g.display_content_window_ref is None or not gui_g.display_content_window_ref.winfo_viewable():
             # we display the window only if it is not already displayed
             function_to_call = getattr(gui_g.UEVM_cli_ref, command_name)
             function_to_call(gui_g.UEVM_cli_args)
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/UEVMGuiHiddenRootClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/WebImageClass.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/WebImageClass.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,10 +264,10 @@
 def custom_print(text='', keep_mode=True) -> None:
     """
     Print the given text on the GUI if it's available, otherwise print it on the console²
     :param text: the text to print
     :param keep_mode: whether to keep the existing content when adding a new one
     """
     if gui_g.display_content_window_ref is not None:
-        gui_g.display_content_window_ref.display(content=text, keep_mode=keep_mode)
+        gui_g.display_content_window_ref.display(content=text + '\n', keep_mode=keep_mode)
     else:
         print(text)
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/functions_no_deps.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/functions_no_deps.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,50 +131,52 @@
             try:
                 tk_window.iconbitmap(icon)
             except Exception as error:
                 # in linux, the ico can exist but not be readable
                 print(f'Error while setting the icon: {error!r}')
 
 
-def create_empty_file(file_path: str) -> str:
+def create_empty_file(file_path: str) -> (bool, str):
     """
     Create an empty file
     :param file_path: the path of the file to create
-    :return: the path of the file
+    :return: (True if path was valid, the corrected path of the file)
     """
     path, file = os.path.split(file_path)
-    path = check_and_get_folder(os.path.dirname(path))
+    is_valid, path = check_and_get_folder(os.path.dirname(path))
     file_path = os.path.normpath(os.path.join(path, file))
     open(file_path, 'a').close()
-    return file_path
+    return is_valid, file_path
 
 
-def check_and_get_folder(folder_path: str) -> str:
+def check_and_get_folder(folder_path: str) -> (bool, str):
     """
     Check if the folder exists. If not, create it or use the default one
     :param folder_path: the path of the folder to check
-    :return: the path of the folder
+    :return: (True if path was valid, the corrected path of the folder)
     """
     path = folder_path
+    is_valid = True
     if not os.path.exists(path):
         try:
             os.makedirs(path)
         except (OSError, PermissionError) as e:
+            is_valid = False
             print(f'Error while creating the directory {path}: {e}')
             if home_dir := os.environ.get('XDG_CONFIG_HOME'):
                 path = os.path.join(home_dir, 'UEVaultManager')
             else:
                 path = os.path.expanduser('~/.config/UEVaultManager')
             if not os.path.exists(path):
                 os.makedirs(path)
                 path = os.path.normpath(path)
             print(f'The following folder {path} will be used as default')
 
     path = os.path.normpath(path)
-    return path
+    return is_valid, path
 
 
 def convert_to_bool(value) -> bool:
     """
     Convert a value to a boolean
     :param value: the value to convert. If the value is not a boolean, it will be converted to a string and then to a boolean.
     :return:
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/tkgui/modules/globals.py` & `UEVaultManager-1.6.7/UEVaultManager/tkgui/modules/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,23 @@
 
 def set_args_offline(value: bool) -> None:
     """
     Set the value of the argument offline. Mandadory fot the associated ttk.ckbutton to work
     :param value:  True or False
     """
     UEVM_cli_args['offline'] = value
+
+
+def set_args_delete_metadata(value: bool) -> None:
+    """
+    Set the value of the argument delete_metadata. Mandadory fot the associated ttk.ckbutton to work
+    :param value:  True or False
+    """
+    UEVM_cli_args['delete_metadata'] = value
+
+
+def set_args_delete_extras_data(value: bool) -> None:
+    """
+    Set the value of the argument delete_extras_data. Mandadory fot the associated ttk.ckbutton to work
+    :param value:  True or False
+    """
+    UEVM_cli_args['delete_extras_data'] = value
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/aliasing.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/aliasing.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/cli.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/cli.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/custom_parser.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/custom_parser.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/egl_crypt.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/egl_crypt.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/rolling_hash.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/rolling_hash.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager/utils/webview_login.py` & `UEVaultManager-1.6.7/UEVaultManager/utils/webview_login.py`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/UEVaultManager.egg-info/PKG-INFO` & `UEVaultManager-1.6.7/UEVaultManager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UEVaultManager
-Version: 1.6.6
+Version: 1.6.7
 Summary: Free and open-source replacement for the Epic Games Launcher application, mainly to manage the assets for Unreal Engine
 Home-page: https://github.com/LaurentOngaro/UEVaultManager
 Author: Laurent Ongaro
 Author-email: laurent@gameamea.com
 License: GPL-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.9
@@ -63,8 +63,8 @@
 * [Configuration](https://uevaultmanager.readthedocs.io/en/latest/configuration.html)
   * [Config folder](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-folder)
   * [Config file](https://uevaultmanager.readthedocs.io/en/latest/configuration.html#config-file)
 
 [More info](https://uevaultmanager.readthedocs.io/en/latest/intro.html "UEVaultManager")
 
 
- UEVaultManager ## version:1.6.6 ## codename: Virgo+6
+ UEVaultManager ## version:1.6.7 ## codename: Virgo+7
```

### Comparing `UEVaultManager-1.6.6/UEVaultManager.egg-info/SOURCES.txt` & `UEVaultManager-1.6.7/UEVaultManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UEVaultManager-1.6.6/setup.py` & `UEVaultManager-1.6.7/setup.py`

 * *Files identical despite different names*

