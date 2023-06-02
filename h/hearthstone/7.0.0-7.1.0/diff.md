# Comparing `tmp/hearthstone-7.0.0.tar.gz` & `tmp/hearthstone-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hearthstone-7.0.0.tar", last modified: Thu Jun  1 16:23:46 2023, max compression
+gzip compressed data, was "hearthstone-7.1.0.tar", last modified: Fri Jun  2 18:48:02 2023, max compression
```

## Comparing `hearthstone-7.0.0.tar` & `hearthstone-7.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:23:46.538478 hearthstone-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-01 16:23:39.000000 hearthstone-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-01 16:23:46.538478 hearthstone-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-01 16:23:39.000000 hearthstone-7.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:23:46.538478 hearthstone-7.0.0/hearthstone/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/bountyxml.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/cardxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/dbf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/deckstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)    59267 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/mercenaryxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/stringsfile.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:23:46.538478 hearthstone-7.0.0/hearthstone/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-01 16:23:39.000000 hearthstone-7.0.0/hearthstone/xmlutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:23:46.538478 hearthstone-7.0.0/hearthstone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:23:46.000000 hearthstone-7.0.0/hearthstone.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 16:23:46.538478 hearthstone-7.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-01 16:23:39.000000 hearthstone-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.364363 hearthstone-7.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-02 18:47:56.000000 hearthstone-7.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 18:48:02.364363 hearthstone-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 18:47:56.000000 hearthstone-7.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.360362 hearthstone-7.1.0/hearthstone/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/bountyxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/cardxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/dbf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/deckstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60583 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/mercenaryxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/stringsfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.364363 hearthstone-7.1.0/hearthstone/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-02 18:47:56.000000 hearthstone-7.1.0/hearthstone/xmlutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:48:02.360362 hearthstone-7.1.0/hearthstone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:48:02.000000 hearthstone-7.1.0/hearthstone.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-02 18:48:02.364363 hearthstone-7.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-06-02 18:47:56.000000 hearthstone-7.1.0/setup.py
```

### Comparing `hearthstone-7.0.0/LICENSE` & `hearthstone-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/PKG-INFO` & `hearthstone-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.0.0
+Version: 7.1.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.0.0/README.md` & `hearthstone-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/bountyxml.py` & `hearthstone-7.1.0/hearthstone/bountyxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/cardxml.py` & `hearthstone-7.1.0/hearthstone/cardxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/dbf.py` & `hearthstone-7.1.0/hearthstone/dbf.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/deckstrings.py` & `hearthstone-7.1.0/hearthstone/deckstrings.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/entities.py` & `hearthstone-7.1.0/hearthstone/entities.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/enums.py` & `hearthstone-7.1.0/hearthstone/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1830,14 +1830,26 @@
 	DRUID_HUNTER = 8
 	DRUID_SHAMAN = 9
 	MAGE_SHAMAN = 10
 	MAGE_ROGUE = 11
 	ROGUE_WARRIOR = 12
 	PALADIN_WARRIOR = 13
 
+	MAGE_HUNTER = 28
+	HUNTER_DEATHKNIGHT = 29
+	DEATHKNIGHT_PALADIN = 30
+	PALADIN_SHAMAN = 31
+	SHAMAN_WARRIOR = 32
+	WARRIOR_DEMONHUNTER = 33
+	DEMONHUNTER_ROGUE = 34
+	ROGUE_PRIEST = 35
+	PRIEST_DRUID = 36
+	DRUID_WARLOCK = 37
+	WARLOCK_MAGE = 38
+
 	@property
 	def card_classes(self):
 		# Gadgetzan
 		if self == MultiClassGroup.GRIMY_GOONS:
 			return [CardClass.HUNTER, CardClass.WARRIOR, CardClass.PALADIN]
 		elif self == MultiClassGroup.JADE_LOTUS:
 			return [CardClass.ROGUE, CardClass.SHAMAN, CardClass.DRUID]
@@ -1862,14 +1874,38 @@
 		elif self == MultiClassGroup.MAGE_ROGUE:
 			return [CardClass.MAGE, CardClass.ROGUE]
 		elif self == MultiClassGroup.ROGUE_WARRIOR:
 			return [CardClass.ROGUE, CardClass.WARRIOR]
 		elif self == MultiClassGroup.PALADIN_WARRIOR:
 			return [CardClass.PALADIN, CardClass.WARRIOR]
 
+		# Audiopocalypse
+		if self == MultiClassGroup.MAGE_HUNTER:
+			return [CardClass.MAGE, CardClass.HUNTER]
+		elif self == MultiClassGroup.HUNTER_DEATHKNIGHT:
+			return [CardClass.HUNTER, CardClass.DEATHKNIGHT]
+		elif self == MultiClassGroup.DEATHKNIGHT_PALADIN:
+			return [CardClass.DEATHKNIGHT, CardClass.PALADIN]
+		elif self == MultiClassGroup.PALADIN_SHAMAN:
+			return [CardClass.PALADIN, CardClass.SHAMAN]
+		elif self == MultiClassGroup.SHAMAN_WARRIOR:
+			return [CardClass.SHAMAN, CardClass.WARRIOR]
+		elif self == MultiClassGroup.WARRIOR_DEMONHUNTER:
+			return [CardClass.WARRIOR, CardClass.DEMONHUNTER]
+		elif self == MultiClassGroup.DEMONHUNTER_ROGUE:
+			return [CardClass.DEMONHUNTER, CardClass.ROGUE]
+		elif self == MultiClassGroup.ROGUE_PRIEST:
+			return [CardClass.ROGUE, CardClass.PRIEST]
+		elif self == MultiClassGroup.PRIEST_DRUID:
+			return [CardClass.PRIEST, CardClass.DRUID]
+		elif self == MultiClassGroup.DRUID_WARLOCK:
+			return [CardClass.DRUID, CardClass.WARLOCK]
+		elif self == MultiClassGroup.WARLOCK_MAGE:
+			return [CardClass.WARLOCK, CardClass.MAGE]
+
 		return []
 
 
 class SpellSchool(IntEnum):
 	"""TAG_SPELL_SCHOOL"""
 
 	NONE = 0
```

### Comparing `hearthstone-7.0.0/hearthstone/mercenaryxml.py` & `hearthstone-7.1.0/hearthstone/mercenaryxml.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/stringsfile.py` & `hearthstone-7.1.0/hearthstone/stringsfile.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/utils/__init__.py` & `hearthstone-7.1.0/hearthstone/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone/xmlutils.py` & `hearthstone-7.1.0/hearthstone/xmlutils.py`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/hearthstone.egg-info/PKG-INFO` & `hearthstone-7.1.0/hearthstone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hearthstone
-Version: 7.0.0
+Version: 7.1.0
 Summary: CardDefs.xml parser and Hearthstone enums for Python
 Home-page: https://github.com/HearthSim/python-hearthstone/
 Download-URL: https://github.com/HearthSim/python-hearthstone/tarball/master
 Author: Jerome Leclanche
 Author-email: jerome@leclan.ch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `hearthstone-7.0.0/hearthstone.egg-info/SOURCES.txt` & `hearthstone-7.1.0/hearthstone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hearthstone-7.0.0/setup.cfg` & `hearthstone-7.1.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hearthstone
-version = 7.0.0
+version = 7.1.0
 description = CardDefs.xml parser and Hearthstone enums for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jerome Leclanche
 author_email = jerome@leclan.ch
 url = https://github.com/HearthSim/python-hearthstone/
 download_url = https://github.com/HearthSim/python-hearthstone/tarball/master
```

