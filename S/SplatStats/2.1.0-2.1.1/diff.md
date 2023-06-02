# Comparing `tmp/SplatStats-2.1.0.tar.gz` & `tmp/SplatStats-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.1.0.tar", last modified: Thu Jun  1 03:38:26 2023, max compression
+gzip compressed data, was "SplatStats-2.1.1.tar", last modified: Fri Jun  2 04:01:57 2023, max compression
```

## Comparing `SplatStats-2.1.0.tar` & `SplatStats-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-01 03:38:26.414769 SplatStats-2.1.0/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.1.0/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-01 03:38:26.414596 SplatStats-2.1.0/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.1.0/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-01 03:38:26.413514 SplatStats-2.1.0/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.1.0/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.1.0/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10176 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.1.0/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.1.0/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.1.0/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-01 03:38:26.414371 SplatStats-2.1.0/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-06-01 03:38:26.000000 SplatStats-2.1.0/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-01 03:38:26.414815 SplatStats-2.1.0/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.1.0/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.820232 SplatStats-2.1.1/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.1.1/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-02 04:01:57.820075 SplatStats-2.1.1/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.1.1/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.818949 SplatStats-2.1.1/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.1.1/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.1.1/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10727 2023-06-02 03:50:03.000000 SplatStats-2.1.1/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.1.1/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.1.1/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.819868 SplatStats-2.1.1/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-02 04:01:57.820278 SplatStats-2.1.1/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.1.1/setup.py
```

### Comparing `SplatStats-2.1.0/LICENSE` & `SplatStats-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/PKG-INFO` & `SplatStats-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.1.0
+Version: 2.1.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.1.0/README.md` & `SplatStats-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/Battle.py` & `SplatStats-2.1.1/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/Player.py` & `SplatStats-2.1.1/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/StatInk.py` & `SplatStats-2.1.1/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/Team.py` & `SplatStats-2.1.1/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/__init__.py` & `SplatStats-2.1.1/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/auxiliary.py` & `SplatStats-2.1.1/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/colors.py` & `SplatStats-2.1.1/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/constants.py` & `SplatStats-2.1.1/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/files.py` & `SplatStats-2.1.1/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/parsers.py` & `SplatStats-2.1.1/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/plots.py` & `SplatStats-2.1.1/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/plotsAux.py` & `SplatStats-2.1.1/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/plotsTeam.py` & `SplatStats-2.1.1/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/statInkConstants.py` & `SplatStats-2.1.1/SplatStats/statInkConstants.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,46 +40,55 @@
   'prime': 'Splattershot Pro',
   'prime_collabo': 'Forge Splattershot Pro',
   'promodeler_mg': 'Aerospray MG',
   'promodeler_rg': 'Aerospray RG',
   'sharp': 'Splash-o-matic',
   'sharp_neo': 'Neo Splash-o-matic',
   'spaceshooter': 'Splattershot Nova',
+  'spaceshooter_collabo': 'Annaki Splattershot Nova',
   'sshooter': 'Splattershot',
   'sshooter_collabo': 'Tentatek Splattershot',
   'wakaba': 'Splattershot Jr.',
   'clashblaster': 'Clash Blaster',
   'clashblaster_neo': 'Clash Blaster Neo',
   'hotblaster': 'Blaster',
   'longblaster': 'Range Blaster',
   'nova': 'Luna Blaster',
   'nova_neo': 'Luna Blaster Neo',
   'rapid': 'Rapid Blaster',
   'rapid_deco': 'Rapid Blaster Deco',
   'rapid_elite': 'Rapid Blaster Pro',
+  'rapid_elite_deco': 'Rapid Blaster Pro Deco',
+  'sblast92': "S-BLAST '92",
   'h3reelgun': 'H-3 Nozzlenose',
+  'h3reelgun_d': 'H-3 Nozzlenose D',
   'l3reelgun': 'L-3 Nozzlenose',
   'l3reelgun_d': 'L-3 Nozzlenose D',
   'dualsweeper': 'Dualie Squelchers',
+  'dualsweeper_custom': 'Custom Dualie Squelchers',
   'kelvin525': 'Glooga Dualies',
   'maneuver': 'Splat Dualies',
   'quadhopper_black': 'Dark Tetra Dualies',
+  'quadhopper_white': 'Light Tetra Dualies',
   'sputtery': 'Dapple Dualies',
   'sputtery_hue': 'Dapple Dualies Nouveau',
   'carbon': 'Carbon Roller',
   'carbon_deco': 'Carbon Roller Deco',
   'dynamo': 'Dynamo Roller',
   'splatroller': 'Splat Roller',
   'splatroller_collabo': 'Krak-On Splat Roller',
   'variableroller': 'Flingza Roller',
   'wideroller': 'Big Swig Roller',
+  'wideroller_collabo': 'Big Swig Roller Express',
+  'fincent': 'Painbrush',
   'hokusai': 'Octobrush',
   'pablo': 'Inkbrush',
   'pablo_hue': 'Inkbrush Nouveau',
   'drivewiper': 'Splatana Wiper',
+  'drivewiper_deco': 'Splatana Wiper Deco',
   'jimuwiper': 'Splatana Stamper',
   'bamboo14mk1': 'Bamboozler 14 Mk I',
   'liter4k': 'E-liter 4K',
   'liter4k_scope': 'E-liter 4K Scope',
   'rpen_5h': 'Snipewriter 5H',
   'soytuber': 'Goo Tuber',
   'splatcharger': 'Splat Charger',
@@ -91,35 +100,38 @@
   'bucketslosher_deco': 'Slosher Deco',
   'explosher': 'Explosher',
   'furo': 'Bloblobber',
   'hissen': 'Tri-Slosher',
   'hissen_hue': 'Tri-Slosher Nouveau',
   'screwslosher': 'Sloshing Machine',
   'barrelspinner': 'Heavy Splatling',
+  'barrelspinner_deco': 'Heavy Splatling Deco',
   'hydra': 'Hydra Splatling',
   'kugelschreiber': 'Ballpoint Splatling',
   'nautilus47': 'Nautilus 47',
   'splatspinner': 'Mini Splatling',
   'splatspinner_collabo': 'Zink Mini Splatling',
   'campingshelter': 'Tenta Brella',
+  'campingshelter_sorella': 'Tenta Sorella Brella',
   'parashelter': 'Splat Brella',
   'spygadget': 'Undercover Brella',
   'lact450': 'REEF-LUX 450',
   'tristringer': 'Tri-Stringer'
 }
 
 STGS_DICT = {
   'yunohana': 'Scorch Gorge', 'gonzui': 'Eeltail Alley',
   'kinmedai': "Museum d'Alfonsino", 'mategai': 'Undertow Spillway',
   'namero': 'Mincemeat Metalworks', 'yagara': 'Hagglefish Market',
   'masaba': 'Hammerhead Bridge', 'mahimahi': 'Mahi-Mahi Resort',
   'zatou': 'MakoMart', 'chozame': 'Sturgeon Shipyard',
   'amabi': 'Inkblot Art Academy', 'sumeshi': 'Wahoo World',
   'hirame': 'Flounder Heights', 'kusaya': 'Brinewater Springs',
-  'manta': 'Manta Maria', 'nampla': "Um'ami Ruins"
+  'manta': 'Manta Maria', 'nampla': "Um'ami Ruins", 
+  'taraport':'Barnacle & Dime', 'kombu': 'Humpback Pump Track'
 }
 
 STATINK_DTYPES = {
   # Match information -------------------------------------------------------
   '# season': 'string',
   #'period': 'datetime64'
   'game-ver': 'string',
```

### Comparing `SplatStats-2.1.0/SplatStats/statInkPlots.py` & `SplatStats-2.1.1/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/statInkStats.py` & `SplatStats-2.1.1/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats/stats.py` & `SplatStats-2.1.1/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.1.1/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.1.0
+Version: 2.1.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.1.0/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.1.1/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.0/setup.py` & `SplatStats-2.1.1/setup.py`

 * *Files identical despite different names*

