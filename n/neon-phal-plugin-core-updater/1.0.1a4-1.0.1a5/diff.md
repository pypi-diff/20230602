# Comparing `tmp/neon_phal_plugin_core_updater-1.0.1a4-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_core_updater-1.0.1a5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6641 bytes, number of entries: 7
--rw-r--r--  2.0 unx     8156 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater/__init__.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2333 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/WHEEL
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       30 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      726 b- defN 23-Jun-01 22:37 neon_phal_plugin_core_updater-1.0.1a4.dist-info/RECORD
-7 files, 13070 bytes uncompressed, 5313 bytes compressed:  59.3%
+Zip file size: 6655 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     8281 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater/__init__.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2333 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       30 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      726 b- defN 23-Jun-01 23:59 neon_phal_plugin_core_updater-1.0.1a5.dist-info/RECORD
+7 files, 13195 bytes uncompressed, 5327 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: neon_phal_plugin_core_updater/__init__.py
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/LICENSE.md
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/METADATA
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/WHEEL
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/entry_points.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/top_level.txt
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_core_updater-1.0.1a4.dist-info/RECORD
+Filename: neon_phal_plugin_core_updater-1.0.1a5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_core_updater/__init__.py

```diff
@@ -123,38 +123,41 @@
         """
         version = message.data.get("version", "")
         LOG.debug(f"Starting update to version: {version}")
         default_branch = "dev" if "a" in version else "master"
         patch_ver = version.split('a')[0] if version else "master"
         if self.patch_script:
             patch_script = self.patch_script.format(patch_ver)
-            LOG.info(f"Running patches from: {patch_script}")
             patch_script = requests.get(patch_script)
             if not patch_script.ok:
                 LOG.info(f"No branch for {patch_ver}, trying {default_branch}")
+                patch_ver = default_branch
                 patch_script = \
                     requests.get(self.patch_script.format(default_branch))
             if patch_script.ok:
+                LOG.info(f"Running patches from: {patch_script.url}")
                 ref, temp_path = mkstemp()
                 close(ref)
                 with open(temp_path, 'w+') as f:
                     f.write(patch_script.text)
                 try:
                     Popen(f"chmod ugo+x {temp_path}", shell=True).wait(10)
                     LOG.info(f"Running {temp_path}")
                     patch = Popen([temp_path, patch_ver])
+
                     LOG.info(f"Patch finished with code: "
                              f"{patch.wait(timeout=180)}")
                 except Exception as e:
                     LOG.error(e)
             else:
                 LOG.error(f"Error getting patch: {patch_script.status_code}")
                 LOG.error(patch_script.text)
         self.bus.wait_for_response(message.forward("neon.update_config",
                                                    {"skill_config": False,
+                                                    "apps_config": True,
                                                     "core_config": True,
                                                     "restart": False,
                                                     "version": patch_ver}),
                                    timeout=30)
         if self.update_command:
             branch_spec = version or 'master'
             LOG.info(f"Starting Core Update to version: {branch_spec}")
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a4.dist-info/LICENSE.md` & `neon_phal_plugin_core_updater-1.0.1a5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_core_updater-1.0.1a4.dist-info/METADATA` & `neon_phal_plugin_core_updater-1.0.1a5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-core-updater
-Version: 1.0.1a4
+Version: 1.0.1a5
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-core-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_phal_plugin_core_updater-1.0.1a4.dist-info/RECORD` & `neon_phal_plugin_core_updater-1.0.1a5.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-neon_phal_plugin_core_updater/__init__.py,sha256=ix_rYKJekpVXexCVgyxJMHKDWvfzRaha4q9IqTsIi7k,8156
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/METADATA,sha256=WQJ0v2Yj7SU_9zUxiOUrjnmcqoN2bNCdUBZ7igif4mQ,2333
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
-neon_phal_plugin_core_updater-1.0.1a4.dist-info/RECORD,,
+neon_phal_plugin_core_updater/__init__.py,sha256=H0JdwOl9E3abQJaWF8d2SA9FfxXTnr8C97_RP3h2xto,8281
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/METADATA,sha256=7_DbwWIh_pmd-GdnmnOB0PpB_lnoTmcbSmPYhWumKqc,2333
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/entry_points.txt,sha256=VNgr7F2h4e9YHmu7kYdA3YQRnayDrsBKBnaUMW_YkpM,99
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/top_level.txt,sha256=rNzTcvxgwp9uHhuqJeV4KI4DEs5IOXh4R08n3XCTQUI,30
+neon_phal_plugin_core_updater-1.0.1a5.dist-info/RECORD,,
```

