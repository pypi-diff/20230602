# Comparing `tmp/neon_phal_plugin_core_updater-1.1.1-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.1.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6626 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8281 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2325 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      714 b- defN 23-Jun-02 01:49 neon_phal_plugin_core_updater-1.1.1.dist-info/RECORD
-7 files, 13174 bytes uncompressed, 5322 bytes compressed:  59.6%
+Zip file size: 6654 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8281 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2333 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-Jun-02 01:37 neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD
+7 files, 13195 bytes uncompressed, 5326 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.1.1.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neon_phal_plugin_core_updater-1.1.1.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.1.1.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.1.1
+Version: 1.1.1a1
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 Requires-Dist: requests
 Requires-Dist: neon-utils (~=1.1)
 Requires-Dist: ovos-plugin-manager (~=0.0.20)
 
 # Core Updater Plugin
 Exposes a messagebus API to check for and initiate core module updates. Update
 checks use GitHub releases or PyPI indices, depending on plugin configuration.
@@ -66,8 +66,7 @@
 msg_type: neon.core_updater.start_update
 data:
   version: <new_version>
 ```
 will start the configured update command in a shell with `version` passed as the
 first and only argument. If `version` is omitted, the configured update command
 will be called with no commands.
-
```

## Comparing `neon_phal_plugin_core_updater-1.1.1.dist-info/RECORD` & `neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 neon_phal_plugin_core_updater/__init__.py,sha256=H0JdwOl9E3abQJaWF8d2SA9FfxXTnr8C97_RP3h2xto,8281
-neon_phal_plugin_core_updater-1.1.1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_core_updater-1.1.1.dist-info/METADATA,sha256=KP0Q61AyM-kR-f4w6ZlW0C-j5n98Uy4TSo6J9f9rQz4,2325
-neon_phal_plugin_core_updater-1.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_core_updater-1.1.1.dist-info/entry_points.txt,sha256=3UhJ0b7cF_TxJwAPWiEGnlMncHuI8nOvh9dzyeokMf0,98
-neon_phal_plugin_core_updater-1.1.1.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
-neon_phal_plugin_core_updater-1.1.1.dist-info/RECORD,,
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/METADATA,sha256=TkVlgH7kHW4ni1793i0-v8KiAM8brcnCYpGkyLX8pNs,2333
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
+neon_phal_plugin_core_updater-1.1.1a1.dist-info/RECORD,,
```

