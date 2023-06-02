# Comparing `tmp/tello_solectric_pl-0.0.4.tar.gz` & `tmp/tello_solectric_pl-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_solectric_pl-0.0.4.tar", last modified: Fri Jun  2 16:30:08 2023, max compression
+gzip compressed data, was "tello_solectric_pl-0.0.5.tar", last modified: Fri Jun  2 16:46:07 2023, max compression
```

## Comparing `tello_solectric_pl-0.0.4.tar` & `tello_solectric_pl-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.770210 tello_solectric_pl-0.0.4/
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.4/README.md
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-02 16:30:08.770210 tello_solectric_pl-0.0.4/setup.cfg
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-02 16:28:14.000000 tello_solectric_pl-0.0.4/setup.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/tello_solectric_pl/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl/__init__.py
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3460 2023-06-02 16:25:16.000000 tello_solectric_pl-0.0.4/tello_solectric_pl/tello_solectric_pl.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/SOURCES.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/dependency_links.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/requires.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/top_level.txt
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:46:07.940209 tello_solectric_pl-0.0.5/
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:46:07.940209 tello_solectric_pl-0.0.5/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.5/README.md
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-02 16:46:07.940209 tello_solectric_pl-0.0.5/setup.cfg
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-02 16:46:02.000000 tello_solectric_pl-0.0.5/setup.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:46:07.938209 tello_solectric_pl-0.0.5/tello_solectric_pl/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.5/tello_solectric_pl/__init__.py
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3383 2023-06-02 16:44:47.000000 tello_solectric_pl-0.0.5/tello_solectric_pl/tello_solectric_pl.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:46:07.940209 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:46:07.000000 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-02 16:46:07.000000 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-02 16:46:07.000000 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-02 16:46:07.000000 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/requires.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-02 16:46:07.000000 tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/top_level.txt
```

### Comparing `tello_solectric_pl-0.0.4/PKG-INFO` & `tello_solectric_pl-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello_solectric_pl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

### Comparing `tello_solectric_pl-0.0.4/README.md` & `tello_solectric_pl-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.4/setup.py` & `tello_solectric_pl-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tello_solectric_pl",
-    version="0.0.4",
+    version="0.0.5",
     author="Adam Jurkiewicz",
     python_requires='>=3.8',
     author_email="adam@jurkiewicz.tech",
     description="Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://solectric.pl",
```

### Comparing `tello_solectric_pl-0.0.4/tello_solectric_pl/tello_solectric_pl.py` & `tello_solectric_pl-0.0.5/tello_solectric_pl/tello_solectric_pl.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,29 +79,26 @@
 class TelloEDU(TelloMain):
     """
 
     Klasa przeznaczona dla dronów Tello-EDU (czarny)
     W metodzie D.connect() sprawdza, czy to taki dron, czy poziom naładowania baterii jest wystarczający
     """
 
-    hardware_type = "TelloEDU"
-    min_battery_level = 25
-
     def __init__(self, info_all=False):
         """
 
         :param info_all: Czy ysyłać wszystkie informacje na ekran, True lub False (default)
         """
         super().__init__(info_all=info_all)
 
     def connect(self, wait_for_state=True) -> bool:
 
         return super().tello_connect(
-            hardware_type=hardware_type,
-            min_battery_level=min_battery_level,
+            hardware_type="TelloEDU",
+            min_battery_level=25,
             wait_for_state=wait_for_state,
         )
 
 
 class RyzenTT(TelloMain):
     """
     Klasa przeznaczona dla dronów Ryzen-TT (czerwony)
```

### Comparing `tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/PKG-INFO` & `tello_solectric_pl-0.0.5/tello_solectric_pl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello-solectric-pl
-Version: 0.0.4
+Version: 0.0.5
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

