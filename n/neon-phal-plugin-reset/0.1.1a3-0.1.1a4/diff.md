# Comparing `tmp/neon_phal_plugin_reset-0.1.1a3-py3-none-any.whl.zip` & `tmp/neon_phal_plugin_reset-0.1.1a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11276 bytes, number of entries: 10
--rw-r--r--  2.0 unx    11560 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/__init__.py
--rw-r--r--  2.0 unx     2687 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/config.py
--rw-r--r--  2.0 unx     3873 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/create_media.py
--rw-r--r--  2.0 unx     1856 b- defN 23-Jun-01 00:16 neon_phal_plugin_reset/version.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1197 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       85 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      952 b- defN 23-Jun-01 00:17 neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD
-10 files, 23959 bytes uncompressed, 9612 bytes compressed:  59.9%
+Zip file size: 11306 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    12157 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset/__init__.py
+-rw-r--r--  2.0 unx     2687 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset/config.py
+-rw-r--r--  2.0 unx     3873 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset/create_media.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset/version.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       85 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      952 b- defN 23-Jun-01 23:55 neon_phal_plugin_reset-0.1.1a4.dist-info/RECORD
+10 files, 24556 bytes uncompressed, 9642 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: neon_phal_plugin_reset/create_media.py
 Comment: 
 
 Filename: neon_phal_plugin_reset/version.py
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/METADATA
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/WHEEL
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/WHEEL
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/entry_points.txt
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/top_level.txt
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD
+Filename: neon_phal_plugin_reset-0.1.1a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_phal_plugin_reset/__init__.py

```diff
@@ -90,26 +90,27 @@
         try:
             download_url = f"https://github.com/neongeckocom/" \
                            f"neon-image-recipe/archive/{version}.zip"
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
         except BadZipFile:
-            LOG.warning(f"No branch for version: {version}. Trying default")
+            LOG.debug(f"No branch for version: {version}. "
+                      f"Trying default {default_branch}")
             download_url = default_dl_url
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
         except Exception as e:
             LOG.exception(e)
             download_url = default_dl_url
             LOG.debug(f"Downloading from {download_url}")
             download_extract_zip(download_url, "/tmp/neon/",
                                  skill_folder_name="neon-image-recipe")
-
+        LOG.info(f"Downloaded default config from {download_url}")
         # Contents are now at /tmp/neon/neon-image-recipe
         try:
             if message.data.get('skill_config'):
                 LOG.debug("Updating skill config from default")
                 Popen(["/usr/bin/cp", "-r",
                        "/tmp/neon/neon-image-recipe/05_neon_core"
                        "/overlay/home/neon/.config/neon/skills",
@@ -117,14 +118,22 @@
                 if isdir("/tmp/neon/neon-image-recipe/05_neon_core/overlay/"
                          "home/neon/.config/neon/apps"):
                     Popen(["/usr/bin/cp", "-r",
                            "/tmp/neon/neon-image-recipe/05_neon_core"
                            "/overlay/home/neon/.config/neon/apps",
                            "/home/neon/.config/neon/"])
                 Popen("chown -R neon:neon /home/neon", shell=True)
+            if message.data.get('apps_config'):
+                if isdir("/tmp/neon/neon-image-recipe/05_neon_core/overlay/"
+                         "home/neon/.config/neon/apps"):
+                    Popen(["/usr/bin/cp", "-r",
+                           "/tmp/neon/neon-image-recipe/05_neon_core"
+                           "/overlay/home/neon/.config/neon/apps",
+                           "/home/neon/.config/neon/"])
+                Popen("chown -R neon:neon /home/neon", shell=True)
             if message.data.get('core_config'):
                 LOG.debug("Updating system config from default")
                 move("/tmp/neon/neon-image-recipe/05_neon_core/overlay"
                      "/etc/neon/neon.yaml", "/etc/neon/neon.yaml")
             LOG.info(f"Restored default configuration")
             rmtree("/tmp/neon/neon-image-recipe")
         except Exception as e:
```

## neon_phal_plugin_reset/version.py

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a3"
+__version__ = "0.1.1a4"
```

## Comparing `neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md` & `neon_phal_plugin_reset-0.1.1a4.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA` & `neon_phal_plugin_reset-0.1.1a4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-reset
-Version: 0.1.1a3
+Version: 0.1.1a4
 Summary: Device Reset Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-reset
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

## Comparing `neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD` & `neon_phal_plugin_reset-0.1.1a4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-neon_phal_plugin_reset/__init__.py,sha256=YyD_pNztg08YPbmVsKpmqUsUKuocWtCYLL3TR1m00Tg,11560
+neon_phal_plugin_reset/__init__.py,sha256=VmpiAThfceS28IZV3iFR9TeXvkVxNNc-en-zQ8WCQ_s,12157
 neon_phal_plugin_reset/config.py,sha256=nuf5EMlYXd1UN5sUey1uVO-V5G5ENMEj8BTs7Efctys,2687
 neon_phal_plugin_reset/create_media.py,sha256=v6IFDU1nM2Q4-EgVUTzNoXGPZVl3dvS9bO1WldwkTrE,3873
-neon_phal_plugin_reset/version.py,sha256=TcR4_ZtHShUvYmq1B5NewavbaSNQN9I2JsqCd4GEWJw,1856
-neon_phal_plugin_reset-0.1.1a3.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_phal_plugin_reset-0.1.1a3.dist-info/METADATA,sha256=QILbYXJio3PqP0g4sg5D3q4GGFv2T0AdrW7L3svGY8c,1197
-neon_phal_plugin_reset-0.1.1a3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_phal_plugin_reset-0.1.1a3.dist-info/entry_points.txt,sha256=uEmgDx1-r9Hr4K2GPMExL_oPpRdCxgtElxnqLhfLBRw,85
-neon_phal_plugin_reset-0.1.1a3.dist-info/top_level.txt,sha256=0qp8KO5XNgKsWYzWK0MmltqOKmQUbKNDHhQggPMr32s,23
-neon_phal_plugin_reset-0.1.1a3.dist-info/RECORD,,
+neon_phal_plugin_reset/version.py,sha256=Txaxe_eR4WP2J3zbaMKOLRuHpfDH1qJBGc_t0M1uY60,1856
+neon_phal_plugin_reset-0.1.1a4.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_phal_plugin_reset-0.1.1a4.dist-info/METADATA,sha256=pJH8I2LA9CFnktSkHOjvlozPPhI08os4XrFJv9bmXVs,1197
+neon_phal_plugin_reset-0.1.1a4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_phal_plugin_reset-0.1.1a4.dist-info/entry_points.txt,sha256=uEmgDx1-r9Hr4K2GPMExL_oPpRdCxgtElxnqLhfLBRw,85
+neon_phal_plugin_reset-0.1.1a4.dist-info/top_level.txt,sha256=0qp8KO5XNgKsWYzWK0MmltqOKmQUbKNDHhQggPMr32s,23
+neon_phal_plugin_reset-0.1.1a4.dist-info/RECORD,,
```

