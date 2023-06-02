# Comparing `tmp/dronefly_discord-0.1.0.tar.gz` & `tmp/dronefly_discord-0.1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronefly_discord-0.1.0.tar", max compression
+gzip compressed data, was "dronefly_discord-0.1.1.dev0.tar", max compression
```

## Comparing `dronefly_discord-0.1.0.tar` & `dronefly_discord-0.1.1.dev0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.0/LICENSE
--rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.0/dronefly/discord/__init__.py
--rw-r--r--   0        0        0     3278 2023-04-30 16:36:34.398098 dronefly_discord-0.1.0/dronefly/discord/embeds.py
--rw-r--r--   0        0        0      683 2023-05-06 10:38:14.043479 dronefly_discord-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1588 1970-01-01 00:00:00.000000 dronefly_discord-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    56697 2023-04-22 11:51:53.202527 dronefly_discord-0.1.1.dev0/LICENSE
+-rw-r--r--   0        0        0      916 2023-04-22 11:51:09.749659 dronefly_discord-0.1.1.dev0/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 12:15:11.202522 dronefly_discord-0.1.1.dev0/dronefly/discord/__init__.py
+-rw-r--r--   0        0        0     3430 2023-05-27 08:05:17.585923 dronefly_discord-0.1.1.dev0/dronefly/discord/embeds.py
+-rw-r--r--   0        0        0      688 2023-06-02 15:47:25.548696 dronefly_discord-0.1.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev0/setup.py
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 dronefly_discord-0.1.1.dev0/PKG-INFO
```

### Comparing `dronefly_discord-0.1.0/LICENSE` & `dronefly_discord-0.1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.0/README.md` & `dronefly_discord-0.1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `dronefly_discord-0.1.0/dronefly/discord/embeds.py` & `dronefly_discord-0.1.1.dev0/dronefly/discord/embeds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from functools import wraps
 
 import discord
 import inflect
 from pyinaturalist.models import IconPhoto, Taxon
 
+from dronefly.core import formatters
 from dronefly.core.formatters.constants import WWW_BASE_URL
 from dronefly.core.formatters.generic import (
     format_taxon_names,
     TaxonFormatter,
 )
 
+# This shows up better in Discord than \u{SPARKLE}:
+formatters.generic.MEANS_LABEL_EMOJI["endemic"] = ":sparkle:"
+
 EMBED_COLOR = 0x90EE90
 # From https://discordapp.com/developers/docs/resources/channel#embed-limits
 MAX_EMBED_TITLE_LEN = MAX_EMBED_NAME_LEN = 256
 MAX_EMBED_DESCRIPTION_LEN = 2048
 MAX_EMBED_FIELDS = 25
 MAX_EMBED_VALUE_LEN = 1024
 MAX_EMBED_FOOTER_LEN = 2048
```

### Comparing `dronefly_discord-0.1.0/pyproject.toml` & `dronefly_discord-0.1.1.dev0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 max-line-length = 100
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.poetry]
 name = "dronefly-discord"
-version = "0.1.0"
+version = "0.1.1.dev0"
 description = "Dronefly Discord library"
 authors = ["Ben Armstrong <synrg@debian.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
         { include = "dronefly/discord" },
 ]
```

### Comparing `dronefly_discord-0.1.0/PKG-INFO` & `dronefly_discord-0.1.1.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronefly-discord
-Version: 0.1.0
+Version: 0.1.1.dev0
 Summary: Dronefly Discord library
 License: AGPL-3.0-or-later
 Author: Ben Armstrong
 Author-email: synrg@debian.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

