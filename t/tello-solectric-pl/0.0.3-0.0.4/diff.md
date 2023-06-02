# Comparing `tmp/tello_solectric_pl-0.0.3.tar.gz` & `tmp/tello_solectric_pl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello_solectric_pl-0.0.3.tar", last modified: Thu Jun  1 12:33:50 2023, max compression
+gzip compressed data, was "tello_solectric_pl-0.0.4.tar", last modified: Fri Jun  2 16:30:08 2023, max compression
```

## Comparing `tello_solectric_pl-0.0.3.tar` & `tello_solectric_pl-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.3/README.md
--rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/setup.cfg
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-01 12:31:52.000000 tello_solectric_pl-0.0.3/setup.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/tello_solectric_pl/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.3/tello_solectric_pl/__init__.py
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3044 2023-06-01 12:05:06.000000 tello_solectric_pl-0.0.3/tello_solectric_pl/tello_solectric_pl.py
-drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-01 12:33:50.805644 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/PKG-INFO
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/SOURCES.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/dependency_links.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/requires.txt
--rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-01 12:33:50.000000 tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/top_level.txt
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.770210 tello_solectric_pl-0.0.4/
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     2546 2023-04-08 09:49:02.000000 tello_solectric_pl-0.0.4/README.md
+-rw-rw-r--   0 adasiek   (1000) adasiek   (1000)       38 2023-06-02 16:30:08.770210 tello_solectric_pl-0.0.4/setup.cfg
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      890 2023-06-02 16:28:14.000000 tello_solectric_pl-0.0.4/setup.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/tello_solectric_pl/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      288 2023-04-08 09:32:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl/__init__.py
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3460 2023-06-02 16:25:16.000000 tello_solectric_pl-0.0.4/tello_solectric_pl/tello_solectric_pl.py
+drwxrwxr-x   0 adasiek   (1000) adasiek   (1000)        0 2023-06-02 16:30:08.768210 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)     3176 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/PKG-INFO
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)      299 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/SOURCES.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)        1 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/dependency_links.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       11 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/requires.txt
+-rw-r--r--   0 adasiek   (1000) adasiek   (1000)       19 2023-06-02 16:30:08.000000 tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/top_level.txt
```

### Comparing `tello_solectric_pl-0.0.3/PKG-INFO` & `tello_solectric_pl-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello_solectric_pl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

### Comparing `tello_solectric_pl-0.0.3/README.md` & `tello_solectric_pl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tello_solectric_pl-0.0.3/setup.py` & `tello_solectric_pl-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tello_solectric_pl",
-    version="0.0.3",
+    version="0.0.4",
     author="Adam Jurkiewicz",
     python_requires='>=3.8',
     author_email="adam@jurkiewicz.tech",
     description="Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://solectric.pl",
```

### Comparing `tello_solectric_pl-0.0.3/tello_solectric_pl/tello_solectric_pl.py` & `tello_solectric_pl-0.0.4/tello_solectric_pl/tello_solectric_pl.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,92 +9,106 @@
     """
 
     def __init__(self, info_all=False):
         if not info_all:
             Tello.LOGGER.setLevel(logging.CRITICAL)
         super().__init__()
 
-    def query_hardware(self):
+    def query_hardware(self) -> str:
         """
 
-        :return: "RMTT" if using the Controller on top of the RMTT, or "TELLO", if using a Tello or RMTT without
+        :return: "RMTT" if using the Controller on top of the RMTT, or "TelloEDU", if using a Tello or RMTT without
         the controller.
         :rtype:
         """
         try:
-            hardware = self.send_read_command('hardware?')
-            if hardware in ('ok', 'unknown command: hardware?'):
+            hardware = self.send_read_command("hardware?")
+            if hardware in ("ok", "unknown command: hardware?"):
                 hardware = "TelloEDU"
+            else:
+                print(f"Bład przy sprawdzeniu hardware: {hardware}")
         except Exception as exc:
             hardware = "TelloEDU"
 
         return hardware
 
     def get_speed(self) -> int:
         """Query speed setting (cm/s)
         This method is in the DroneBlocksTello class because the Tello class
         uses a different command that no longer seems supported.
         Returns:
             int: 1-100
         """
-        speed_value = self.send_read_command('speed?')
+        speed_value = self.send_read_command("speed?")
         try:
             speed_value = int(float(speed_value))
             self.last_speed_value = speed_value
         except:
             speed_value = self.last_speed_value
 
         return speed_value
 
+    def tello_connect(self, hardware_type, min_battery_level, wait_for_state) -> bool:
+        connection_success = False
+        hardware_ok = False
+        hardware_probe = "xxxx"
+
+        try:
+            super().connect(wait_for_state=wait_for_state)
+            connection_success = True
+        except Exception as e:
+            print(f"Błąd przy wywołaniu CONNECT: {e}")
+            return False
+
+        hardware_probe = self.query_hardware()
+        if hardware_type == hardware_probe:
+            hardware_ok = True
+            print(f"Połączono z dronem typu {hardware_type}")
+            battery_level = self.get_battery()
+            print(f"Poziom baterii == ({battery_level} %)")
+            if battery_level < min_battery_level:
+                print(
+                    f"Poziom baterii zbyt niski - wymagane minimum to {min_battery_level} %."
+                )
+                return False
+        else:
+            print(f"Otrzymano: {repr(hardware_probe)} -> nie pasuje do {hardware_type}")
+
+        return connection_success and hardware_ok
+
 
 class TelloEDU(TelloMain):
     """
 
     Klasa przeznaczona dla dronów Tello-EDU (czarny)
     W metodzie D.connect() sprawdza, czy to taki dron, czy poziom naładowania baterii jest wystarczający
     """
+
     hardware_type = "TelloEDU"
     min_battery_level = 25
 
     def __init__(self, info_all=False):
         """
 
         :param info_all: Czy ysyłać wszystkie informacje na ekran, True lub False (default)
         """
         super().__init__(info_all=info_all)
 
     def connect(self, wait_for_state=True) -> bool:
-        connection_success = False
-        hardware_ok = False
-        hardware_probe = "xxxx"
-
-
-        try:
-            super().connect(wait_for_state=wait_for_state)
-            connection_success = True
-        except Exception as e:
-            print(f"Błąd przy wywołaniu CONNECT: {e}")
-            return False
-
-        hardware_probe = self.query_hardware()
-        if self.hardware_type == hardware_probe:
-            hardware_ok = True
-            print(f"Połączono z dronem typu {self.hardware_type}")
-            battery_level = self.get_battery()
-	    print(f"Poziom baterii == ({battery_level} %)")
-            if battery_level < self.min_battery_level:
-                print(f"Poziom baterii zbyt niski - wymagane minimum to {self.min_battery_level} %.")
-                return False
-        else:
-            print(f"Otrzymano: {repr(hardware_probe)} -> nie pasuje do {self.hardware_type}")
 
-        return connection_success and hardware_ok
+        return super().tello_connect(
+            hardware_type=hardware_type,
+            min_battery_level=min_battery_level,
+            wait_for_state=wait_for_state,
+        )
 
 
 class RyzenTT(TelloMain):
     """
     Klasa przeznaczona dla dronów Ryzen-TT (czerwony)
     W metodzie D.connect() sprawdza, czy to taki dron
     W przyszłości pojawią się definicje metod
     """
+
     hardware_type = "RyzenTT"
+    min_battery_level = 25
     pass
```

### Comparing `tello_solectric_pl-0.0.3/tello_solectric_pl.egg-info/PKG-INFO` & `tello_solectric_pl-0.0.4/tello_solectric_pl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tello-solectric-pl
-Version: 0.0.3
+Version: 0.0.4
 Summary: Biblioteka dla wsparcia nauczycieli w Polsce dla dronów Tello-EDU oraz Ryzen TT (z wyświetlaczem LCD)
 Home-page: https://solectric.pl
 Author: Adam Jurkiewicz
 Author-email: adam@jurkiewicz.tech
 License: UNKNOWN
 Keywords: Dron Tello TelloEDU Ryzen RyzenTT DJI
 Platform: UNKNOWN
```

