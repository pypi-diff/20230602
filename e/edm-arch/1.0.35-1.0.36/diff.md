# Comparing `tmp/edm-arch-1.0.35.tar.gz` & `tmp/edm-arch-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edm-arch-1.0.35.tar", last modified: Wed May 24 07:57:28 2023, max compression
+gzip compressed data, was "edm-arch-1.0.36.tar", last modified: Fri Jun  2 15:19:21 2023, max compression
```

## Comparing `edm-arch-1.0.35.tar` & `edm-arch-1.0.36.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.558853 edm-arch-1.0.35/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.35/LICENSE
--rw-rw-rw-   0        0        0    17591 2023-05-24 07:57:28.559853 edm-arch-1.0.35/PKG-INFO
--rw-rw-rw-   0        0        0    16697 2023-05-24 07:51:33.000000 edm-arch-1.0.35/README.md
--rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm-arch-1.0.35/pyproject.toml
--rw-rw-rw-   0        0        0     1255 2023-05-24 07:57:28.560890 edm-arch-1.0.35/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.35/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.521871 edm-arch-1.0.35/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.536855 edm-arch-1.0.35/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0    17591 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.35/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      162 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 07:57:28.000000 edm-arch-1.0.35/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.549852 edm-arch-1.0.35/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.35/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.35/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    28427 2023-05-16 12:08:43.000000 edm-arch-1.0.35/src/edmpy/cfg.py
--rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.35/src/edmpy/constants.py
--rw-rw-rw-   0        0        0     5450 2023-05-22 10:08:25.000000 edm-arch-1.0.35/src/edmpy/db.py
--rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   126492 2023-05-24 07:51:36.000000 edm-arch-1.0.35/src/edmpy/edm.py
--rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/geo.py
--rw-rw-rw-   0        0        0     2508 2023-05-11 11:24:10.000000 edm-arch-1.0.35/src/edmpy/ini.py
-drwxrwxrwx   0        0        0        0 2023-05-24 07:57:28.558853 edm-arch-1.0.35/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.35/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4220 2023-05-11 11:23:24.000000 edm-arch-1.0.35/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4338 2023-05-11 11:23:24.000000 edm-arch-1.0.35/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/lib/constants.py
--rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.35/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   177497 2023-05-23 07:50:54.000000 edm-arch-1.0.35/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.35/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.35/src/edmpy/py.typed
--rw-rw-rw-   0        0        0    44664 2023-05-16 12:03:19.000000 edm-arch-1.0.35/src/edmpy/totalstation.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:19:21.299911 edm-arch-1.0.36/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm-arch-1.0.36/LICENSE
+-rw-rw-rw-   0        0        0    17657 2023-06-02 15:19:21.299911 edm-arch-1.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0    16763 2023-05-24 08:10:46.000000 edm-arch-1.0.36/README.md
+-rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm-arch-1.0.36/pyproject.toml
+-rw-rw-rw-   0        0        0     1255 2023-06-02 15:19:21.300816 edm-arch-1.0.36/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm-arch-1.0.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:19:21.262445 edm-arch-1.0.36/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 15:19:21.277630 edm-arch-1.0.36/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    17657 2023-06-02 15:19:21.000000 edm-arch-1.0.36/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-06-02 15:19:21.000000 edm-arch-1.0.36/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 15:19:21.000000 edm-arch-1.0.36/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm-arch-1.0.36/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      162 2023-06-02 15:19:21.000000 edm-arch-1.0.36/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-02 15:19:21.000000 edm-arch-1.0.36/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 15:19:21.289460 edm-arch-1.0.36/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.36/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm-arch-1.0.36/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28470 2023-06-02 12:38:17.000000 edm-arch-1.0.36/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0       18 2023-03-08 09:12:03.000000 edm-arch-1.0.36/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5450 2023-05-22 10:08:25.000000 edm-arch-1.0.36/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13461 2023-05-08 09:53:16.000000 edm-arch-1.0.36/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   126791 2023-06-02 14:53:35.000000 edm-arch-1.0.36/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5691 2023-05-08 09:53:16.000000 edm-arch-1.0.36/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2508 2023-05-11 11:24:10.000000 edm-arch-1.0.36/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2023-06-02 15:19:21.298260 edm-arch-1.0.36/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm-arch-1.0.36/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4220 2023-05-11 11:23:24.000000 edm-arch-1.0.36/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4338 2023-05-11 11:23:24.000000 edm-arch-1.0.36/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     2334 2023-05-08 09:53:16.000000 edm-arch-1.0.36/src/edmpy/lib/constants.py
+-rw-rw-rw-   0        0        0     4035 2023-03-08 08:56:31.000000 edm-arch-1.0.36/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   178831 2023-06-02 14:48:48.000000 edm-arch-1.0.36/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1792 2023-05-08 09:53:16.000000 edm-arch-1.0.36/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm-arch-1.0.36/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0    44664 2023-05-16 12:03:19.000000 edm-arch-1.0.36/src/edmpy/totalstation.py
```

### Comparing `edm-arch-1.0.35/LICENSE` & `edm-arch-1.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/PKG-INFO` & `edm-arch-1.0.36/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.35
+Version: 1.0.36
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -108,46 +108,46 @@
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Changes for Version 1.0.35 (May 24, 2023)
-  Bug in file import fixed
-  Bug in CFG when no field type is specified fixed as well
-  Bug in Filter records that crashed program is fixed
-  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
-  Saving a point is now faster when record count is high
-  Reworked a number of features because JSON files are not in doc_id order
-  Add a "SIMULATION mode on" warning to maing screen when simulating points
-  Suffix values on import csv are retained as integers
-  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
-  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
-  Error trap continuation shot on an empty data file
+1.   Bug in file import fixed
+2.   Bug in CFG when no field type is specified fixed as well
+3.   Bug in Filter records that crashed program is fixed
+4.   Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+5.   Saving a point is now faster when record count is high
+6.   Reworked a number of features because JSON files are not in doc_id order
+7.   Add a "SIMULATION mode on" warning to maing screen when simulating points
+8.   Suffix values on import csv are retained as integers
+9.   Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+10.  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+11.  Error trap continuation shot on an empty data file
 
 ##### Changes for Version 1.0.34
-  Yet more fixes for Windows/PyPi installations
+1.   Yet more fixes for Windows/PyPi installations
 
 ##### Changes for Version 1.0.33
-  Fixed installation issues
+1.   Fixed installation issues
 
 ##### Changes for Version 1.0.32
-  Fixing issues with GeoCom and station setup
+1.   Fixing issues with GeoCom and station setup
 
 ##### Changes for Version 1.0.31
-  Fixed issue with numeric values saved as text in JSON after initial save
-  Added Help JSON to view raw data in JSON file
+1.   Fixed issue with numeric values saved as text in JSON after initial save
+2.   Added Help JSON to view raw data in JSON file
 
 ##### Changes for Version 1.0.31
-  BlueTooth tested with Leica GeoCom stations
-  UI fixes
-  Tested with 1000 records in DB
-  Made JSON files better formatted so that they are more human readable
-  Made geoJSON files work with QGIS (points and lines are separate layers)
-  Substantial refactoring of Python classes and file structure
+1.   BlueTooth tested with Leica GeoCom stations
+2.   UI fixes
+3.   Tested with 1000 records in DB
+4.   Made JSON files better formatted so that they are more human readable
+5.   Made geoJSON files work with QGIS (points and lines are separate layers)
+6.   Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.35/README.md` & `edm-arch-1.0.36/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -81,46 +81,46 @@
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Changes for Version 1.0.35 (May 24, 2023)
-  Bug in file import fixed
-  Bug in CFG when no field type is specified fixed as well
-  Bug in Filter records that crashed program is fixed
-  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
-  Saving a point is now faster when record count is high
-  Reworked a number of features because JSON files are not in doc_id order
-  Add a "SIMULATION mode on" warning to maing screen when simulating points
-  Suffix values on import csv are retained as integers
-  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
-  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
-  Error trap continuation shot on an empty data file
+1.   Bug in file import fixed
+2.   Bug in CFG when no field type is specified fixed as well
+3.   Bug in Filter records that crashed program is fixed
+4.   Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+5.   Saving a point is now faster when record count is high
+6.   Reworked a number of features because JSON files are not in doc_id order
+7.   Add a "SIMULATION mode on" warning to maing screen when simulating points
+8.   Suffix values on import csv are retained as integers
+9.   Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+10.  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+11.  Error trap continuation shot on an empty data file
 
 ##### Changes for Version 1.0.34
-  Yet more fixes for Windows/PyPi installations
+1.   Yet more fixes for Windows/PyPi installations
 
 ##### Changes for Version 1.0.33
-  Fixed installation issues
+1.   Fixed installation issues
 
 ##### Changes for Version 1.0.32
-  Fixing issues with GeoCom and station setup
+1.   Fixing issues with GeoCom and station setup
 
 ##### Changes for Version 1.0.31
-  Fixed issue with numeric values saved as text in JSON after initial save
-  Added Help JSON to view raw data in JSON file
+1.   Fixed issue with numeric values saved as text in JSON after initial save
+2.   Added Help JSON to view raw data in JSON file
 
 ##### Changes for Version 1.0.31
-  BlueTooth tested with Leica GeoCom stations
-  UI fixes
-  Tested with 1000 records in DB
-  Made JSON files better formatted so that they are more human readable
-  Made geoJSON files work with QGIS (points and lines are separate layers)
-  Substantial refactoring of Python classes and file structure
+1.   BlueTooth tested with Leica GeoCom stations
+2.   UI fixes
+3.   Tested with 1000 records in DB
+4.   Made JSON files better formatted so that they are more human readable
+5.   Made geoJSON files work with QGIS (points and lines are separate layers)
+6.   Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.35/pyproject.toml` & `edm-arch-1.0.36/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/setup.cfg` & `edm-arch-1.0.36/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3335 0d0a  rsion = 1.0.35..
+00000050: 7273 696f 6e20 3d20 312e 302e 3336 0d0a  rsion = 1.0.36..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
```

### Comparing `edm-arch-1.0.35/src/edm_arch.egg-info/PKG-INFO` & `edm-arch-1.0.36/src/edm_arch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.35
+Version: 1.0.36
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -108,46 +108,46 @@
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
 ##### Changes for Version 1.0.35 (May 24, 2023)
-  Bug in file import fixed
-  Bug in CFG when no field type is specified fixed as well
-  Bug in Filter records that crashed program is fixed
-  Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
-  Saving a point is now faster when record count is high
-  Reworked a number of features because JSON files are not in doc_id order
-  Add a "SIMULATION mode on" warning to maing screen when simulating points
-  Suffix values on import csv are retained as integers
-  Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
-  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
-  Error trap continuation shot on an empty data file
+1.   Bug in file import fixed
+2.   Bug in CFG when no field type is specified fixed as well
+3.   Bug in Filter records that crashed program is fixed
+4.   Importing CSV now takes seconds rather than many many minutes (tested on import of 3996 records)
+5.   Saving a point is now faster when record count is high
+6.   Reworked a number of features because JSON files are not in doc_id order
+7.   Add a "SIMULATION mode on" warning to maing screen when simulating points
+8.   Suffix values on import csv are retained as integers
+9.   Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
+10.  Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
+11.  Error trap continuation shot on an empty data file
 
 ##### Changes for Version 1.0.34
-  Yet more fixes for Windows/PyPi installations
+1.   Yet more fixes for Windows/PyPi installations
 
 ##### Changes for Version 1.0.33
-  Fixed installation issues
+1.   Fixed installation issues
 
 ##### Changes for Version 1.0.32
-  Fixing issues with GeoCom and station setup
+1.   Fixing issues with GeoCom and station setup
 
 ##### Changes for Version 1.0.31
-  Fixed issue with numeric values saved as text in JSON after initial save
-  Added Help JSON to view raw data in JSON file
+1.   Fixed issue with numeric values saved as text in JSON after initial save
+2.   Added Help JSON to view raw data in JSON file
 
 ##### Changes for Version 1.0.31
-  BlueTooth tested with Leica GeoCom stations
-  UI fixes
-  Tested with 1000 records in DB
-  Made JSON files better formatted so that they are more human readable
-  Made geoJSON files work with QGIS (points and lines are separate layers)
-  Substantial refactoring of Python classes and file structure
+1.   BlueTooth tested with Leica GeoCom stations
+2.   UI fixes
+3.   Tested with 1000 records in DB
+4.   Made JSON files better formatted so that they are more human readable
+5.   Made geoJSON files work with QGIS (points and lines are separate layers)
+6.   Substantial refactoring of Python classes and file structure
 
 ##### Update (March 2, 2023)
 1.   Added and debugged Topcon stations
 2.   Added and debugged Leica and Leica GeoCom stations
 3.   Stopped program from exiting when escape is pressed
 4.   Fixed default locations for ini, log, and data
 5.   Program remembers last size and location of the screen
```

### Comparing `edm-arch-1.0.35/src/edm_arch.egg-info/SOURCES.txt` & `edm-arch-1.0.36/src/edm_arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/cfg.py` & `edm-arch-1.0.36/src/edmpy/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,16 @@
         self.link_fields = []
         bad_characters = r' !@#$%^&*()?/\{}<.,.|+=~`-'
 
         # This is a legacy issue.  Linked fields are now listed with each field.
         unit_fields = self.get_value('EDM', 'UNITFIELDS')
         if unit_fields:
             unit_fields = unit_fields.upper().split(',')
-            unit_fields.remove('UNIT')
+            if 'UNIT' in unit_fields:
+                unit_fields.remove('UNIT')
             unit_fields = ','.join(unit_fields)
             self.update_value('UNIT', 'LINKED', unit_fields)
             self.delete_key('EDM', 'UNITFIELDS')
 
         table_name = self.get_value('EDM', 'TABLE')
         if table_name:
             if any((c in set(bad_characters)) for c in table_name):
```

### Comparing `edm-arch-1.0.35/src/edmpy/db.py` & `edm-arch-1.0.36/src/edmpy/db.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/edm.kv` & `edm-arch-1.0.36/src/edmpy/edm.kv`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/edm.py` & `edm-arch-1.0.36/src/edmpy/edm.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,18 @@
   Reworked a number of features because JSON files are not in doc_id order
   Add a "SIMULATION mode on" warning to maing screen when simulating points
   Suffix values on import csv are retained as integers
   Tried to improve open CFG so that if a non-EDM CFG is opened, it is not also trashed
   Fixed important bugs in station setup when using Manual XYZ or Manual VHD options
   Error trap continuation shot on an empty data file
 
+Changes for Vesion 1.0.36
+  Redid font sizing for buttons and text
+  Trapped a bug with units when switching CFGs
+
 Bugs/To Do
   could make menus work better with keyboard (at least with tab)
   there is no error checking on duplicates in datagrid edits
   Do unitchecking after doing an offset shot on suffix 0 points
   Good way to get random hash IDs
   Offer to change Z when prism changes in datagrid edit cases
   Thoroughly test unit checking
@@ -152,16 +156,16 @@
 """
 try:
     import win32timezone
     win32timezone.TimeZoneInfo.local()
 except ModuleNotFoundError:
     pass
 
-VERSION = '1.0.35'
-PRODUCTION_DATE = 'May, 2023'
+VERSION = '1.0.36'
+PRODUCTION_DATE = 'June, 2023'
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __BUTTONS__ = 13
 __LASTCOMPORT__ = 16
 MAX_SCREEN_WIDTH = 400
 
 
 class MainScreen(e5_MainScreen):
@@ -1122,22 +1126,23 @@
                                     size_hint_max_x = MAX_SCREEN_WIDTH,
                                     size_hint_y = 1,
                                     pos_hint = {'center_x': .5, 'center_y': .5})
         self.add_widget(self.layout)
         self.build_screen()
 
     def build_screen(self):
-        prism = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
+        prism = GridLayout(cols = 2, size_hint_y = None, spacing = 5, padding = 5)
         prism.add_widget(e5_label('Prompt for prism height after each point', colors = self.colors))
         prism_switch = Switch(active = self.station.prism_prompt)
         prism_switch.bind(active = self.prism_prompt)
         prism.add_widget(prism_switch)
+        prism.height = 100
         self.layout.add_widget(prism)
 
-        self.back_button = e5_button('Back', selected = True,
+        self.back_button = e5_button('Back', selected = True, 
                                              call_back = self.go_back,
                                              colors = self.colors)
         self.layout.add_widget(self.back_button)
 
     def prism_prompt(self, instance, value):
         self.station.prism_prompt = value
 
@@ -1193,17 +1198,17 @@
         self.current_settings = e5_label(self.current_settings_pretty(), colors = self.colors)
         self.settings.add_widget(self.current_settings)
         self.change_settings = e5_button("Change Settings", call_back = self.settings_change, colors = self.colors)
         self.settings.add_widget(self.change_settings)
         self.layout.add_widget(self.settings)
 
         self.horizontal_angle = GridLayout(cols = 2, spacing = 5, padding = 5, size_hint = (.2, None))
-        self.leftside = GridLayout(cols = 1, spacing = 5, padding = 5)
+        self.leftside = GridLayout(cols = 1, spacing = 2, padding =0)
         self.leftside.add_widget(e5_label('Enter angle as ddd.mmss', colors = self.colors))
-        self.hangle_input = e5_textinput(write_tab = False)
+        self.hangle_input = e5_textinput(write_tab = False, colors=self.colors)
         self.hangle_input.bind(minimum_height = self.hangle_input.setter('height'))
         self.leftside.add_widget(self.hangle_input)
         self.horizontal_angle.add_widget(self.leftside)
         self.set_angle = e5_button("Set H-angle", call_back = self.set_hangle, colors = self.colors)
         self.horizontal_angle.add_widget(self.set_angle)
         self.layout.add_widget(self.horizontal_angle)
 
@@ -1270,17 +1275,17 @@
                                     pos_hint = {'center_x': .5},
                                     padding = 5,
                                     spacing = 20)
         self.add_widget(self.content)
 
         self.content.add_widget(e5_label('Provide a name and notes (optional), then record and save.', colors = self.colors))
 
-        self.datum_name = DataGridLabelAndField('Name', colors = self.colors)
+        self.datum_name = DataGridLabelAndField('Name : ', colors=self.colors)
         self.content.add_widget(self.datum_name)
-        self.datum_notes = DataGridLabelAndField('Notes', colors = self.colors)
+        self.datum_notes = DataGridLabelAndField('Notes : ', colors=self.colors, note_field=True)
         self.content.add_widget(self.datum_notes)
 
         self.recorder = datum_recorder('Record datum', station = self.station,
                                         colors = self.colors, setup_type = 'record_new', data = self.data)
         self.content.add_widget(self.recorder)
 
         self.results = e5_label('', colors = self.colors)
@@ -1522,15 +1527,16 @@
                                         menu_list = prism_names,
                                         menu_selected = self.default_prism.name if self.default_prism.name else '',
                                         call_back = self.have_shot)
         else:
             return DataGridTextBox(title = 'Enter a Prism Height',
                                         text = str(self.default_prism.height) if self.default_prism.height else '',
                                         call_back = self.have_shot,
-                                        button_text = ['Back', 'Next'])
+                                        button_text = ['Back', 'Next'],
+                                        colors=self.colors)
 
     def microscribe(self, instance):
         result = self.popup.result
         self.popup.dismiss()
         p = self.station.text_to_point(result)
         if not p:
             self.popup = e5_MessageBox(title = 'Error',
@@ -1887,46 +1893,47 @@
         self.station = station
         self.data = data
         self.ini = ini
 
         lastsetup_type = self.ini.get_value('SETUPS', 'LASTSETUP_TYPE')
         self.setup = lastsetup_type if lastsetup_type else 'Horizontal Angle Only'
 
-        self.content = BoxLayout(orientation = 'vertical',
-                                    size_hint_y = 1,
-                                    size_hint_max_x = MAX_SCREEN_WIDTH,
-                                    pos_hint = {'center_x': .5, 'center_y': .5},
-                                    padding = 5,
-                                    spacing = 5)
+        self.content = BoxLayout(orientation='vertical',
+                                    size_hint_y=1,
+                                    size_hint_max_x=MAX_SCREEN_WIDTH,
+                                    pos_hint={'center_x': .5, 'center_y': .5},
+                                    padding=5,
+                                    spacing=5)
         self.add_widget(self.content)
 
-        setup_type_box = GridLayout(cols = 2,
-                                    size_hint_y = None,
-                                    pos_hint = {'center_x': .5, 'center_y': .5})
+        setup_type_box = GridLayout(cols=1, padding=2, spacing=2, size_hint_y=None)
+
+        setup_type_label = e5_label('Select a setup type from this dropdown', colors=self.colors)
+        setup_type_box.add_widget(setup_type_label)
 
         spinner_dropdown_button = SpinnerOptions
         spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
         spinner_dropdown_button.background_color = (0, 0, 0, 1)
 
-        self.setup_type = Spinner(text = self.setup,
+        self.setup_type = Spinner(text=self.setup,
                                     values=["Horizontal Angle Only",
                                             "Over a datum",
                                             "Over a datum + Record a datum",
                                             "Record two datums",
                                             "Three datum shift"],
-                                    option_cls = spinner_dropdown_button)
+                                    option_cls=spinner_dropdown_button)
         if colors.button_font_size:
             self.setup_type.font_size = colors.button_font_size
         setup_type_box.add_widget(self.setup_type)
         self.setup_type.bind(text = self.rebuild)
         self.content.add_widget(setup_type_box)
 
-        self.scroll_content = BoxLayout(orientation = 'vertical',
-                                        size_hint = (1, .9),
-                                        spacing = 5, padding = 5)
+        self.scroll_content = BoxLayout(orientation='vertical',
+                                        size_hint=(1, .9),
+                                        spacing=5, padding=5)
 
         self.content.add_widget(self.scroll_content)
 
         self.setup_widgets = setups(self.setup_type.text,
                                     data = self.data,
                                     ini = self.ini,
                                     station = self.station,
@@ -2199,15 +2206,15 @@
         super(station_setting, self).__init__(**kwargs)
 
         self.station = station
         self.id = id
         self.cols = 2
         self.pos_hint = {'center_x': .5},
         self.colors = colors
-        self.label = e5_label(text = label_text, colors = colors)
+        self.label = e5_label(text=label_text + ' : ', colors=colors, halign='right')
         self.add_widget(self.label)
 
         # Create a default dropdown button and then modify its properties
         # For some reason, the usual font size specification doesn't work here and sp has to be removed
         spinner_dropdown_button = SpinnerOptions
         spinner_dropdown_button.font_size = colors.button_font_size.replace("sp", '') if colors.button_font_size else None
         spinner_dropdown_button.background_color = (0, 0, 0, 1)
```

### Comparing `edm-arch-1.0.35/src/edmpy/geo.py` & `edm-arch-1.0.36/src/edmpy/geo.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/ini.py` & `edm-arch-1.0.36/src/edmpy/ini.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/lib/blockdata.py` & `edm-arch-1.0.36/src/edmpy/lib/blockdata.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/lib/colorscheme.py` & `edm-arch-1.0.36/src/edmpy/lib/colorscheme.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/lib/constants.py` & `edm-arch-1.0.36/src/edmpy/lib/constants.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/lib/dbs.py` & `edm-arch-1.0.36/src/edmpy/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/lib/e5_widgets.py` & `edm-arch-1.0.36/src/edmpy/lib/e5_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from kivy.properties import ObjectProperty, NumericProperty, StringProperty, BooleanProperty
 from kivy.uix.floatlayout import FloatLayout
 from kivy.uix.switch import Switch
 from kivy.uix.slider import Slider
 from kivy.uix.behaviors.focus import FocusBehavior
 from kivy.uix.spinner import Spinner, SpinnerOption
 from kivy.uix.progressbar import ProgressBar
+from kivy.core.text import Text
+
+from kivy.graphics import Color, Rectangle
 
 from decimal import DivisionByZero
 
 import ntpath
 import os
 from shutil import copyfile
 from datetime import datetime
@@ -134,44 +137,44 @@
         self.content = pop_content
         self.title = 'Filter dataset'
         self.size_hint = (.9, .38)
 
 
 class edm_manual(Popup):
 
-    def __init__(self, type = "Manual XYZ", call_back = None, colors = None, **kwargs):
+    def __init__(self, type="Manual XYZ", call_back=None, colors=None, **kwargs):
         super(edm_manual, self).__init__(**kwargs)
 
-        pop_content = GridLayout(cols = 1, spacing = 5, padding = 5)
+        pop_content = GridLayout(cols=1, spacing=5, padding=5)
         if type == "Manual XYZ":
-            input = DataGridLabelAndField(col = 'X', colors = colors, popup = True)
+            input = DataGridLabelAndField(col='X', colors=colors, popup=True)
             input.txt.bind(on_text_validate = self.next_field)
             self.xcoord = input.txt
             pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Y', colors = colors, popup = True)
+            input = DataGridLabelAndField(col='Y', colors=colors, popup=True)
             input.txt.bind(on_text_validate = self.next_field)
             self.ycoord = input.txt
             pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Z', colors = colors, popup = True)
-            input.txt.bind(on_text_validate = self.next_field)
+            input = DataGridLabelAndField(col='Z', colors=colors, popup=True)
+            input.txt.bind(on_text_validate=self.next_field)
             self.zcoord = input.txt
             pop_content.add_widget(input)
             self.hangle = None
             self.vangle = None
             self.sloped = None
         else:
-            input = DataGridLabelAndField(col = 'Horizontal angle', colors = colors, popup = True)
+            input = DataGridLabelAndField(col='Horizontal angle', colors=colors, popup=True)
             input.txt.bind(on_text_validate = self.next_field)
             self.hangle = input.txt
             pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Vertical angle', colors = colors, popup = True)
+            input = DataGridLabelAndField(col='Vertical angle', colors=colors, popup=True)
             input.txt.bind(on_text_validate = self.next_field)
             self.vangle = input.txt
             pop_content.add_widget(input)
-            input = DataGridLabelAndField(col = 'Slope distance', colors = colors, popup = True)
+            input = DataGridLabelAndField(col='Slope distance', colors=colors, popup=True)
             input.txt.bind(on_text_validate = self.next_field)
             self.sloped = input.txt
             pop_content.add_widget(input)
             self.xcoord = None
             self.ycoord = None
             self.zcoord = None
         buttons = e5_side_by_side_buttons(text = ['Cancel', 'Next'],
@@ -213,23 +216,33 @@
         instance.get_focus_next().focus = True
 
 
 class e5_textinput_without_clear(TextInput):
     id = ObjectProperty('')
     text_length = ObjectProperty(0)
 
-    def __init__(self, **kwargs):
-        super(e5_textinput_without_clear, self).__init__(**kwargs)
+    def __init__(self, colors=None, multiline=False, **kwargs):
+        super(e5_textinput_without_clear, self).__init__()
+        self.size_hint_y = None
+        if colors is not None:
+            self.font_size = colors.text_font_size
         if 'id' in kwargs:
             self.id = kwargs.get('id')
             if self.id in ['X', 'Y', 'Z', 'PRISM', 'SLOPED', 'STATIONX', 'STATIONY', 'STATIONZ', 'LOCALX', 'LOCALY', 'LOCALZ'] and APP_NAME == 'EDM':
                 self.bind(on_text_validate = self.do_coordinate_math)
         if 'text_length' in kwargs:
             self.text_length = kwargs.get('text_length')
 
+        instance = Text(text = 'Shannon', font_size = self.font_size)
+        width, height = instance.render()
+        if multiline:
+            self.height = (height * 4 + self.border[0] + self.border[2]) * 1.2
+        else:
+            self.height = (height + self.border[0] + self.border[2]) * 1.2
+
     def do_coordinate_math(self, instance):
         if instance.text:
             try:
                 self.text = str(eval(instance.text))
             except (DivisionByZero, NameError, SyntaxError):
                 pass
 
@@ -239,29 +252,34 @@
         else:
             s = substring
         return super().insert_text(s, from_undo = from_undo)
 
 
 class e5_textinput(GridLayout):
 
-    def __init__(self, **kwargs):
+    def __init__(self, colors=None, multiline=False, **kwargs):
         super(e5_textinput, self).__init__()
 
         self.cols = 2
         self.spacing = 0
         self.size_hint = (1, None)
-        self.height = TEXTBOX_HEIGHT
+        # self.height = TEXTBOX_HEIGHT - june 1
 
-        self.textbox = e5_textinput_without_clear(**kwargs, height = 30)
+        self.textbox = e5_textinput_without_clear(colors=colors, multiline=multiline, **kwargs)
         # self.textbox.bind(text = self.update_text)
         # self.text = self.textbox.text
         self.add_widget(self.textbox)
 
-        self.clear_button = Button(text = 'X', width = TEXTBOX_HEIGHT,
-                                    size_hint=(None, None), height = TEXTBOX_HEIGHT,
+        if multiline:
+            button_height = (self.textbox.height - self.textbox.border[0] - self.textbox.border[2]) / 1.2
+            button_height = (button_height / 4 + self.textbox.border[0] + self.textbox.border[2]) * 1.2
+        else:
+            button_height = self.textbox.height
+        self.clear_button = Button(text = 'X', width = button_height,
+                                    size_hint=(None, None), height = button_height,
                                     background_normal = '',
                                     background_color = (.2, .2, .2, 1),
                                     on_press = self.clear_text_box)
         self.add_widget(self.clear_button)
 
     # def update_text(self, instance, value):
     #     self.text = instance.text
@@ -276,20 +294,21 @@
     def __init__(self, text, popup = False, colors = None, label_height = None, **kwargs):
         super(e5_label, self).__init__(**kwargs)
         self.text = text
         self.color = set_color(popup, colors)
         if colors:
             if colors.text_font_size:
                 self.font_size = colors.text_font_size
-        if label_height is None:
-            self.bind(size = self.setter('text_size'))
+        # if label_height is None:
+        self.bind(size = self.setter('text_size'))
         # else:
         #     self.height = label_height
-        self.height = 30 if label_height is None else label_height
-        self.valign = 'center'
+        # self.height = 30 if label_height is None else label_height
+        # self.halign = 'center'
+        self.valign = 'top'
 
 
 class e5_label_wrapped(e5_label):
     def __init__(self, text, popup = False, colors = None, **kwargs):
         super(e5_label_wrapped, self).__init__(text, popup = False, colors = None, **kwargs)
         self.size_hint = (1, None)
         self.bind(width = lambda *x: self.setter('text_size')(self, (self.width, None)),
@@ -978,34 +997,34 @@
         backups_switch = Switch(active = self.ini.incremental_backups)
         backups_switch.bind(active = self.incremental_backups)
         backups.add_widget(backups_switch)
         layout.add_widget(backups)
 
         text_font_size = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
         text_font_size_value = int(self.colors.text_font_size.replace("sp", '')) if self.colors.text_font_size else 12
-        self.text_font_size_label = e5_label('Text font size is %s' % text_font_size_value,
+        self.text_font_size_label = e5_label('Text font\nsize is %s' % text_font_size_value,
                                                 id = 'label_font_size',
                                                 colors = self.colors)
         self.labels.append(self.text_font_size_label)
         text_font_size.add_widget(self.text_font_size_label)
-        text_font_slide = Slider(min = 12, max = 26, step = 1, value = text_font_size_value,
+        text_font_slide = Slider(min = 8, max = 20, step = 1, value = text_font_size_value,
                                     orientation = 'horizontal',
                                     value_track = True, value_track_color = self.colors.button_background)
         text_font_size.add_widget(text_font_slide)
         text_font_slide.bind(value = self.update_text_font_size)
         layout.add_widget(text_font_size)
 
         button_font_size = GridLayout(cols = 2, size_hint_y = .1, spacing = 5, padding = 5)
         button_font_size_value = int(self.colors.button_font_size.replace("sp", '')) if self.colors.button_font_size else 12
-        self.button_font_size_label = e5_label('Button font size is %s' % button_font_size_value,
+        self.button_font_size_label = e5_label('Button font\nsize is %s' % button_font_size_value,
                                                 id = 'label_font_size',
                                                 colors = self.colors)
         self.labels.append(self.button_font_size_label)
         button_font_size.add_widget(self.button_font_size_label)
-        button_font_slide = Slider(min = 12, max = 26, step = 1, value = button_font_size_value,
+        button_font_slide = Slider(min = 8, max = 20, step = 1, value = button_font_size_value,
                                     orientation = 'horizontal',
                                     value_track = True, value_track_color = self.colors.button_background)
         button_font_size.add_widget(button_font_slide)
         button_font_slide.bind(value = self.update_button_font_size)
         layout.add_widget(button_font_size)
 
         settings_layout = GridLayout(cols = 1,
@@ -1254,14 +1273,15 @@
     def __init__(self, data = None,
                         doc_id = None,
                         e5_cfg = None,
                         colors = None,
                         one_record_only = False,
                         **kwargs):
         super(e5_RecordEditScreen, self).__init__(**kwargs)
+
         self.colors = colors if colors is not None else ColorScheme()
         self.e5_cfg = e5_cfg
         self.data = data
         self.doc_id = doc_id
         self.one_record_only = one_record_only
         self.can_update_data_table = False
         self.layout = GridLayout(cols = 1,
@@ -1324,15 +1344,14 @@
     def on_leave(self):
         # This helps insure that saving on lost focus works properly
         # There is an issue this addresses with building the screens
         # at startup.
         self.loading = True
 
     def reset_doc_ids(self):
-        print('reset ids')
         self.doc_ids = sorted([r.doc_id for r in self.data.db.table(self.data.table).all()] if self.data.db is not None else [])
 
     def filter(self, instance):
         if instance.text == 'Clear Filter':
             instance.text = 'Filter'
             self.reset_doc_ids()
             self.last_record(None)
@@ -1381,17 +1400,18 @@
         self.first_field_widget = None
         if fields:
             first_field = True
             for col in fields:
                 field_type = self.e5_cfg.get_value(col, 'TYPE')
                 field_length = self.e5_cfg.get_value(col, 'LENGTH')
                 field_length = int(field_length) if self.is_numeric(field_length) else 0
-                widget = DataGridLabelAndField(col = col, prompt = self.e5_cfg.get_value(col, 'PROMPT'),
-                                                colors = self.colors, note_field = (field_type == 'NOTE'),
-                                                text_length = field_length)
+                widget = DataGridLabelAndField(col=col, prompt=self.e5_cfg.get_value(col, 'PROMPT'),
+                                                colors=self.colors,
+                                                note_field=(field_type == 'NOTE'),
+                                                text_length=field_length)
                 self.data_fields.add_widget(widget)
                 if first_field:
                     if field_type not in ['MENU', 'BOOLEAN']:
                         self.first_field_widget = widget.txt
                     first_field = False
 
     def leave_record_without_save(self, instance):
@@ -1970,37 +1990,37 @@
         instructions += 'If you select overwrite, all data for existing matching records in the '
         instructions += 'online repository will be overwritten with the data here.  Normally you '
         instructions += 'do not want to do this, but if you are making changes here to already '
         instructions += 'uploaded data, you may want to select this option. '
         instructions += 'A local backup of your JSON datafile is made before the upload.  '
         instructions += 'Select Delete to remove the data here after the upload (this is good practice).'
         self.scroll_grid.add_widget(e5_label_wrapped(text = instructions, colors = self.colors))
-        self.url = DataGridLabelAndField(col = 'URL', colors = self.colors)
+        self.url = DataGridLabelAndField(col='URL', colors=self.colors)
         if url:
             self.url.txt.text = url
         self.scroll_grid.add_widget(self.url)
-        self.username = DataGridLabelAndField(col = 'Username', colors = self.colors)
+        self.username = DataGridLabelAndField(col='Username', colors=self.colors)
         if username:
             self.username.txt.text = username
         self.scroll_grid.add_widget(self.username)
-        self.password = DataGridLabelAndField(col = 'Password', colors = self.colors)
+        self.password = DataGridLabelAndField(col='Password', colors=self.colors)
         password = ''
         if password:
             self.password.txt.text = password
         self.password.txt.password = True
         self.scroll_grid.add_widget(self.password)
-        self.dbname = DataGridLabelAndField(col = 'Database name', colors = self.colors)
+        self.dbname = DataGridLabelAndField(col='Database name', colors=self.colors)
         self.scroll_grid.add_widget(self.dbname)
-        self.tablename = DataGridLabelAndField(col = 'Table name', colors = self.colors)
+        self.tablename = DataGridLabelAndField(col='Table name', colors=self.colors)
         self.scroll_grid.add_widget(self.tablename)
-        self.overwrite = DataGridLabelAndToggle(col = 'Overwrite existing records?')
+        self.overwrite = DataGridLabelAndToggle(col='Overwrite existing records?')
         self.scroll_grid.add_widget(self.overwrite)
-        self.deleteafter = DataGridLabelAndToggle(col = 'Delete uploaded/updated?')
+        self.deleteafter = DataGridLabelAndToggle(col='Delete uploaded/updated?')
         self.scroll_grid.add_widget(self.deleteafter)
-        self.progress = DataGridLabelAndProgressBar(col = 'Progress\n')
+        self.progress = DataGridLabelAndProgressBar(col='Progress\n')
         self.scroll_grid.add_widget(self.progress)
         self.scroll_grid.add_widget(e5_side_by_side_buttons(text = ['Back', 'Test', 'Upload'],
                                                             id = ['back', 'test', 'upload'],
                                                             call_back = [self.back, self.test, self. upload],
                                                             selected = [False, False, False],
                                                             colors = self.colors))
         self.scroll.add_widget(self.scroll_grid)
@@ -2813,15 +2833,15 @@
         Window.unbind(on_key_down = self._on_keyboard_down)
 
 
 class DataGridTextInput(e5_textinput):
 
     id = ObjectProperty(None)
 
-    def __init__(self, call_back = None, **kwargs):
+    def __init__(self, call_back=None, **kwargs):
         super(DataGridTextInput, self).__init__(**kwargs)
         self.call_back = call_back
 
     def keyboard_on_key_up(self, window, keycode):
         # print(keycode)
         return super(DataGridTextInput, self).keyboard_on_key_up(window, keycode)
 
@@ -2836,24 +2856,25 @@
         super(DataGridTextBox, self).__init__(**kwargs)
         self.colors = colors if colors else ColorScheme()
         content = GridLayout(cols = 1, spacing = 5, padding = 10)
         if label:
             # e5_label(text = col, id = '__label', colors = colors)
             # content.add_widget(Label(text = label, text_size = (None, 30)))
             content.add_widget(e5_label(text = label, colors = self.colors, popup = True))
-        self.txt = DataGridTextInput(text = text, size_hint_y = None,
-                                        text_length = text_length,
+        self.txt = DataGridTextInput(text=text, size_hint_y=None,
+                                        text_length=text_length,
+                                        colors=self.colors,
                                         # height = 30 if not multiline else 90,
-                                        multiline = multiline, id = 'new_item')
-        if self.colors:
-            if self.colors.text_font_size:
-                self.txt.font_size = self.colors.text_font_size
-            if not multiline:
-                if self.colors.text_font_size:
-                    self.txt.height = int(self.colors.text_font_size.replace('sp', '')) * 1.8
+                                        multiline=multiline, id='new_item')
+        # if self.colors:
+            # if self.colors.text_font_size:
+            #     self.txt.textbox.font_size = self.colors.text_font_size
+            # if not multiline:
+            #     if self.colors.text_font_size:
+            #         self.txt.height = int(self.colors.text_font_size.replace('sp', '')) * 1.8
         self.result = text
         self.txt.textbox.bind(text = self.update)
         self.txt.textbox.bind(on_text_validate = self.accept_value)
         content.add_widget(self.txt)
         buttons = e5_side_by_side_buttons(button_text,
                                             button_height = None,
                                             id = [title, 'add_button'],
@@ -3145,15 +3166,15 @@
 
     def populate(self, data, fields, colors = None, call_back = None, revert = None):
         if data is not None and fields is not None:
             self.colors = colors if colors else ColorScheme()
             self.edit_list.bind(minimum_height = self.edit_list.setter('height'))
             self.edit_list.clear_widgets()
             for col in fields.fields():
-                label_and_text = DataGridLabelAndField(col = col, prompt = fields.get(col).prompt, colors = self.colors)
+                label_and_text = DataGridLabelAndField(col=col, prompt=fields.get(col).prompt, colors=self.colors)
                 label_and_text.txt.textbox.bind(on_text_validate = self.next_field)
                 self.edit_list.add_widget(label_and_text)
                 label_and_text.txt.textbox.bind(text = self.changes)
             self.add_widget(e5_side_by_side_buttons(text = ['Revert', 'Save'],
                                                     call_back = [revert, call_back],
                                                     colors = self.colors))
         self.changed = False
@@ -3193,46 +3214,56 @@
         label.bind(texture_size = label.setter('size'))
         self.check = Switch(active = active, size_hint = (0.75, None))
         self.check.height = 30
         self.add_widget(label)
         self.add_widget(self.check)
 
 
-class DataGridLabelAndField(BoxLayout):
+class DataGridLabelAndField(GridLayout):
 
     popup = ObjectProperty(None)
     sorted_result = None
 
-    def __init__(self, col, colors, prompt = '', note_field = False, popup = False, text_length = 0, height = None, **kwargs):
+    def __init__(self, col, colors, prompt='', note_field=False, popup=False, text_length=0, height=None, **kwargs):
         super(DataGridLabelAndField, self).__init__(**kwargs)
         self.update_db = False
         self.widget_type = 'data'
-        if not note_field:
-            if colors:
-                if colors.text_font_size:
-                    self.height = int(colors.text_font_size.replace('sp', '')) * 1.9
+        self.cols = 2
+        # if not note_field:
+        #     if colors:
+        #         if colors.text_font_size:
+        #             self.height = int(colors.text_font_size.replace('sp', '')) * 1.9
         self.size_hint = (0.9, None)
-        self.bind(minimum_height = self.setter('height'))
-        self.spacing = 10
-        label = e5_label(text = prompt if prompt else col, id = '__label',
-                            colors = colors, popup = popup, size_hint_y = None,
-                            halign = 'right', label_height = height)
-        label.bind(texture_size = label.setter('size'))
-        self.txt = e5_textinput(multiline = note_field,
-                                size_hint = (0.75, None),
-                                id = col,
-                                # size_hint_y = 1,
-                                text_length = text_length,
-                                write_tab = False)
-        self.txt.bind(minimum_height = self.txt.setter('height'))
-        if colors:
-            if colors.text_font_size:
-                self.txt.font_size = colors.text_font_size
-        self.add_widget(label)
+        self.spacing = 1
+        self.label = e5_label(text=prompt if prompt else col, id='__label',
+                                colors=colors,
+                                popup=popup,
+                                size_hint_y=None,
+                                halign='right')
+        # self.label.bind(text_size = self.label.setter('size'))
+        # self.label.bind(texture_size = self.fix_height)
+        self.txt = e5_textinput(multiline=note_field,
+                                size_hint=(0.75, None),
+                                id=col,
+                                size_hint_y=None,
+                                text_length=text_length,
+                                write_tab=False,
+                                colors=colors)
+        # if colors:
+        #     if colors.text_font_size:
+        #         self.txt.font_size = colors.text_font_size
+        # self.txt.height = 10
+        self.add_widget(self.label)
         self.add_widget(self.txt)
+        # self.label.height = 20
+        # self.txt.textbox.height = self.label.height
+        # self.label.height = self.txt.textbox.height
+        self.height = self.txt.textbox.height
+        self.label.padding = [10, self.txt.textbox.border[2] * 2]
+        # self.bind(minimum_height = self.txt.textbox.setter('height'))
 
 
 class DataGridDeletePanel(GridLayout):
 
     def populate(self, message = None, call_back = None, colors = None):
         self.colors = colors if colors else ColorScheme()
         self.clear_widgets()
@@ -3256,15 +3287,15 @@
         if data is not None and fields is not None:
             self.colors = colors if colors else ColorScheme()
             self.cols = 1
             if addnew:
                 self.addnew_list.bind(minimum_height = self.addnew_list.setter('height'))
                 self.addnew_list.clear_widgets()
                 for col in fields.fields():
-                    label_and_text = DataGridLabelAndField(col = col, colors = self.colors)
+                    label_and_text = DataGridLabelAndField(col=col, colors=self.colors)
                     label_and_text.txt.bind(on_text_validate = self.next_field)
                     self.addnew_list.add_widget(label_and_text)
                 self.button = e5_button('Add record',
                                             id = 'addnew',
                                             selected = False,
                                             call_back = call_back, colors = self.colors)
                 self.add_widget(self.button)
```

### Comparing `edm-arch-1.0.35/src/edmpy/lib/misc.py` & `edm-arch-1.0.36/src/edmpy/lib/misc.py`

 * *Files identical despite different names*

### Comparing `edm-arch-1.0.35/src/edmpy/totalstation.py` & `edm-arch-1.0.36/src/edmpy/totalstation.py`

 * *Files identical despite different names*

