# Comparing `tmp/apertium2ud-0.0.2.tar.gz` & `tmp/apertium2ud-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apertium2ud-0.0.2.tar", last modified: Thu May 25 10:33:59 2023, max compression
+gzip compressed data, was "apertium2ud-0.0.3.tar", last modified: Fri Jun  2 03:59:03 2023, max compression
```

## Comparing `apertium2ud-0.0.2.tar` & `apertium2ud-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:59.144171 apertium2ud-0.0.2/
--rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.2/LICENSE
--rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.2/MANIFEST.in
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2509 2023-05-25 10:33:59.139121 apertium2ud-0.0.2/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1995 2023-05-25 10:30:51.000000 apertium2ud-0.0.2/README.md
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:58.696427 apertium2ud-0.0.2/apertium2ud/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1874 2023-05-25 10:05:00.000000 apertium2ud-0.0.2/apertium2ud/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)     1818 2023-05-25 10:21:43.000000 apertium2ud-0.0.2/apertium2ud/_map_processing.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      955 2023-05-25 10:24:17.000000 apertium2ud-0.0.2/apertium2ud/convert.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-05-25 07:20:31.000000 apertium2ud-0.0.2/apertium2ud/meta.py
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:59.085735 apertium2ud-0.0.2/apertium2ud/resources/
--rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.2/apertium2ud/resources/__init__.py
--rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.2/apertium2ud/resources/tags_map.json
-drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-05-25 10:33:58.985730 apertium2ud-0.0.2/apertium2ud.egg-info/
--rwxrwxrwx   0 aam       (1000) aam       (1000)     2509 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/PKG-INFO
--rwxrwxrwx   0 aam       (1000) aam       (1000)      380 2023-05-25 10:33:58.000000 apertium2ud-0.0.2/apertium2ud.egg-info/SOURCES.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/dependency_links.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-05-25 10:33:56.000000 apertium2ud-0.0.2/apertium2ud.egg-info/not-zip-safe
--rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-05-25 10:33:57.000000 apertium2ud-0.0.2/apertium2ud.egg-info/top_level.txt
--rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-05-25 10:33:59.147143 apertium2ud-0.0.2/setup.cfg
--rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-05-25 07:20:31.000000 apertium2ud-0.0.2/setup.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.731982 apertium2ud-0.0.3/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    35823 2023-05-19 10:05:32.000000 apertium2ud-0.0.3/LICENSE
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       50 2023-05-20 12:30:15.000000 apertium2ud-0.0.3/MANIFEST.in
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 03:59:03.725988 apertium2ud-0.0.3/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2095 2023-05-26 10:57:10.000000 apertium2ud-0.0.3/README.md
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.329879 apertium2ud-0.0.3/apertium2ud/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1884 2023-06-01 16:50:15.000000 apertium2ud-0.0.3/apertium2ud/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1818 2023-05-25 10:21:43.000000 apertium2ud-0.0.3/apertium2ud/_map_processing.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     1129 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/apertium2ud/convert.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      234 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/apertium2ud/meta.py
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.680919 apertium2ud-0.0.3/apertium2ud/resources/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       25 2023-05-20 12:26:36.000000 apertium2ud-0.0.3/apertium2ud/resources/__init__.py
+-rwxrwxrwx   0 aam       (1000) aam       (1000)    20114 2023-05-25 09:30:37.000000 apertium2ud-0.0.3/apertium2ud/resources/tags_map.json
+drwxrwxrwx   0 aam       (1000) aam       (1000)        0 2023-06-02 03:59:03.586528 apertium2ud-0.0.3/apertium2ud.egg-info/
+-rwxrwxrwx   0 aam       (1000) aam       (1000)     2608 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/PKG-INFO
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      380 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)        1 2023-06-02 03:59:01.000000 apertium2ud-0.0.3/apertium2ud.egg-info/not-zip-safe
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       12 2023-06-02 03:59:02.000000 apertium2ud-0.0.3/apertium2ud.egg-info/top_level.txt
+-rwxrwxrwx   0 aam       (1000) aam       (1000)       38 2023-06-02 03:59:03.733986 apertium2ud-0.0.3/setup.cfg
+-rwxrwxrwx   0 aam       (1000) aam       (1000)      951 2023-06-01 16:57:32.000000 apertium2ud-0.0.3/setup.py
```

### Comparing `apertium2ud-0.0.2/LICENSE` & `apertium2ud-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.2/PKG-INFO` & `apertium2ud-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -59,14 +59,15 @@
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
+* Add the possibility to add the rules based on a `.udx` file, which usually describes custom tags
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
 @misc{apertium2ud2023alekseev,
```

### Comparing `apertium2ud-0.0.2/README.md` & `apertium2ud-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
+* Add the possibility to add the rules based on a `.udx` file, which usually describes custom tags
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
 @misc{apertium2ud2023alekseev,
```

### Comparing `apertium2ud-0.0.2/apertium2ud/__init__.py` & `apertium2ud-0.0.3/apertium2ud/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 from . import resources
 
 with pkg_resources.path(resources, "tags_map.json") as filepath:
     raw_text = open(filepath, "r+", encoding="utf-8").read().strip()
     RAW_WIKI_MAP = json.loads(raw_text)
     del raw_text
 
-UNDOCUMENTED_APERTIUM_SYMBOLS = {'recip', 'gpr_unac', 'mod_ind', 'gna_after', 'prc_plan', 'pcond', 'sim', 'mod_ass',
-                                 'prc_pcond', 'prc_cond', 'unk', 'opt', 'ger_unac', 'pih', 'prc_vol', 'gpr_pot2', 'equ',
-                                 'mod_dub', 'evid', 'unac', "coop", "qst", "emph", "subst", "gpr_pot", "ger_ppot",
-                                 "gpr_ppot", "advl", "prc_irre", "mod_tru", "gna_cond"}
+# UNDOCUMENTED_APERTIUM_SYMBOLS = {'recip', 'gpr_unac', 'mod_ind', 'gna_after', 'prc_plan', 'pcond', 'sim', 'mod_ass',
+#                                  'prc_pcond', 'prc_cond', 'unk', 'opt', 'ger_unac', 'pih', 'prc_vol', 'gpr_pot2', 'equ',
+#                                  'mod_dub', 'evid', 'unac', "coop", "qst", "emph", "subst", "gpr_pot", "ger_ppot",
+#                                  "gpr_ppot", "advl", "prc_irre", "mod_tru", "gna_cond"}
 
 UD2APERTIUM_RULES, APERTIUM2UD_RULES = _map_to_rules(RAW_WIKI_MAP)
-for s in UNDOCUMENTED_APERTIUM_SYMBOLS: APERTIUM2UD_RULES[s] = []
+# for s in UNDOCUMENTED_APERTIUM_SYMBOLS: APERTIUM2UD_RULES[s] = []
 
 POS_TAGS_LIST = sorted(list(set(RAW_WIKI_MAP["POS"].keys())
                             .difference({"punkt"})
                             .union(RAW_WIKI_MAP["POS"]["punkt"].keys())))
 
 OTHER_TAGS_LIST = sorted(list(set([t for k, v in UD2APERTIUM_RULES for t in v if not t in POS_TAGS_LIST])))
```

### Comparing `apertium2ud-0.0.2/apertium2ud/_map_processing.py` & `apertium2ud-0.0.3/apertium2ud/_map_processing.py`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.2/apertium2ud/convert.py` & `apertium2ud-0.0.3/apertium2ud/convert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 
+import sys
+
 from typing import List, Set, Collection
 
 from apertium2ud import UD2APERTIUM_RULES, APERTIUM2UD_RULES
 
 
 def ud2a(upos: str, feats: Set[str]) -> List[str]:
     pool = {upos}.union(feats)
@@ -24,15 +26,21 @@
 
 
 def a2ud(tags: Collection[str]):
 
     result_tags, result_feats = [], []
 
     for tag in tags:
+
+        if tag not in APERTIUM2UD_RULES:
+            print(f"Apertium tag <{tag}> is not documented, skipping.", file=sys.stderr)
+            continue
+
         rules = APERTIUM2UD_RULES[tag]
+
         for rule in rules:
             if "tag" in rule:
                 result_tags.extend(rule["tag"])
             if "feats" in rule:
                 result_feats.extend(rule["feats"])
 
     return result_tags, result_feats
```

### Comparing `apertium2ud-0.0.2/apertium2ud/resources/tags_map.json` & `apertium2ud-0.0.3/apertium2ud/resources/tags_map.json`

 * *Files identical despite different names*

### Comparing `apertium2ud-0.0.2/apertium2ud.egg-info/PKG-INFO` & `apertium2ud-0.0.3/apertium2ud.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apertium2ud
-Version: 0.0.2
+Version: 0.0.3
 Summary: Converting universal tags to Apertium tags.
 Home-page: https://github.com/alexeyev/apertium2ud
 Author: Anton Alekseev
 Author-email: anton.m.alexeye@gmail.com
 Keywords: natural language processing,apertium,morphology
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -59,14 +59,15 @@
 <sent?apos?percent?clb?punct?> 
 ```
 
 ## TODO
 
 * Should sections `chunks` and [XML tags](https://wiki.apertium.org/w/index.php?title=List_of_symbols#XML_tags) be added? [No](https://github.com/apertium/apertium/issues/185).
 * Tests: Apertium -> UD -> Apertium, UD -> Apertium -> UD (sometimes losses are inevitable)
+* Add the possibility to add the rules based on a `.udx` file, which usually describes custom tags
 
 ## How to cite
 
 Greatly appreciated, if you use this work.
 
 ```
 @misc{apertium2ud2023alekseev,
```

### Comparing `apertium2ud-0.0.2/setup.py` & `apertium2ud-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apertium2ud",
     packages=setuptools.find_packages(),
-    version="0.0.2",
+    version="0.0.3",
     description="Converting universal tags to Apertium tags.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Anton Alekseev",
     author_email="anton.m.alexeye@gmail.com",
     url="https://github.com/alexeyev/apertium2ud",
     keywords=["natural language processing", "apertium", "morphology"],
```

