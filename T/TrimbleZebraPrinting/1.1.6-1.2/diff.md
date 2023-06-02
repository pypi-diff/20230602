# Comparing `tmp/TrimbleZebraPrinting-1.1.6.tar.gz` & `tmp/TrimbleZebraPrinting-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TrimbleZebraPrinting-1.1.6.tar", last modified: Fri Mar 31 23:05:47 2023, max compression
+gzip compressed data, was "TrimbleZebraPrinting-1.2.tar", last modified: Fri Jun  2 21:20:37 2023, max compression
```

## Comparing `TrimbleZebraPrinting-1.1.6.tar` & `TrimbleZebraPrinting-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 23:05:47.529703 TrimbleZebraPrinting-1.1.6/
--rw-rw-rw-   0        0        0     1092 2023-03-31 16:17:36.000000 TrimbleZebraPrinting-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     2232 2023-03-31 23:05:47.529703 TrimbleZebraPrinting-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1410 2023-03-31 20:57:38.000000 TrimbleZebraPrinting-1.1.6/README.md
--rw-rw-rw-   0        0        0      966 2023-03-31 23:05:29.000000 TrimbleZebraPrinting-1.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 23:05:47.529703 TrimbleZebraPrinting-1.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-31 23:05:47.498457 TrimbleZebraPrinting-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-03-31 23:05:47.514083 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/
--rw-rw-rw-   0        0        0      170 2023-03-31 20:39:25.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/__init__.py
--rw-rw-rw-   0        0        0    18529 2023-03-30 14:05:15.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/trimble_graphics_conversion.py
--rw-rw-rw-   0        0        0    10056 2023-03-31 23:03:07.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/trimble_zebra_printing.py
-drwxrwxrwx   0        0        0        0 2023-03-31 23:05:47.529703 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/
--rw-rw-rw-   0        0        0     2232 2023-03-31 23:05:47.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-03-31 23:05:47.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 23:05:47.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-03-31 23:05:47.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-03-31 23:05:47.000000 TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 21:20:37.456050 TrimbleZebraPrinting-1.2/
+-rw-rw-rw-   0        0        0     1092 2023-03-31 16:17:36.000000 TrimbleZebraPrinting-1.2/LICENSE
+-rw-rw-rw-   0        0        0     2574 2023-06-02 21:20:37.456050 TrimbleZebraPrinting-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1754 2023-06-02 21:13:42.000000 TrimbleZebraPrinting-1.2/README.md
+-rw-rw-rw-   0        0        0      964 2023-06-02 21:20:18.000000 TrimbleZebraPrinting-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 21:20:37.456050 TrimbleZebraPrinting-1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 21:20:37.440470 TrimbleZebraPrinting-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 21:20:37.456050 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/
+-rw-rw-rw-   0        0        0      170 2023-03-31 20:39:25.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/__init__.py
+-rw-rw-rw-   0        0        0    18529 2023-03-30 14:05:15.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/trimble_graphics_conversion.py
+-rw-rw-rw-   0        0        0    11268 2023-06-02 21:06:54.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/trimble_zebra_printing.py
+drwxrwxrwx   0        0        0        0 2023-06-02 21:20:37.456050 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/
+-rw-rw-rw-   0        0        0     2574 2023-06-02 21:20:37.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-06-02 21:20:37.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 21:20:37.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-02 21:20:37.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-02 21:20:37.000000 TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/top_level.txt
```

### Comparing `TrimbleZebraPrinting-1.1.6/LICENSE` & `TrimbleZebraPrinting-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TrimbleZebraPrinting-1.1.6/PKG-INFO` & `TrimbleZebraPrinting-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimbleZebraPrinting
-Version: 1.1.6
+Version: 1.2
 Summary: Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended.
 Author-email: Ryan Strasburg <ryan_strasburg@trimble.com>
 Project-URL: Homepage, https://github.com/ryan-strasburg/Trimble-Zebra-Printing
 Project-URL: Bug Tracker, https://github.com/ryan-strasburg/Trimble-Zebra-Printing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,19 +14,23 @@
 
 # Trimble Zebra Printing
 Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended.
 
 # class Zebra
 Class To Communicate & Print With (Zebra) Label Printers.
 
-## def print_label(commands, queue = None):
+## def print_label(commands, label_width = None, label_length = None, queue = None):
 Print Label Using ZPL Commands.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches) (required for printer scaling) (optional)
+
+:param label_length: label length (in inches) (required for printer scaling) (optional)
+
 :param queue: printer queue (string) (optional)
 
 ## def set_queue(queue):
 Set Printer Queue.
 
 :param queue: printer queue (string)
 
@@ -38,28 +42,32 @@
 ## def get_printer_dpi(queue = None):
 Get Printer DPI.
 
 :param queue: printer queue (string) (optional)
 
 :return: printer DPI (int)
 
-## def get_label_dpi(commands):
+## def get_label_dpi(commands, label_width, label_length):
 Get Label DPI.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches)
+
+:param label_length: label length (in inches)
+
 :return: label DPI (int)
 
-## def setup(label_height, label_width, direct_thermal = None):
+## def setup(label_width, label_height, direct_thermal = None):
 Setup Printer Parameters Manually.
 
-:param label_height: tuple (label height, label gap) (in dots)
-
 :param label_width: label width (in dots)
 
+:param label_height: tuple (label height, label gap) (in dots)
+
 :param direct_thermal: True if using direct thermal labels (bool) (optional)
 
 ## def autosense():
 Autosense Label Parameters.
 
 ## def reset():
 Reset Printer.
```

### Comparing `TrimbleZebraPrinting-1.1.6/README.md` & `TrimbleZebraPrinting-1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Trimble Zebra Printing
 Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended.
 
 # class Zebra
 Class To Communicate & Print With (Zebra) Label Printers.
 
-## def print_label(commands, queue = None):
+## def print_label(commands, label_width = None, label_length = None, queue = None):
 Print Label Using ZPL Commands.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches) (required for printer scaling) (optional)
+
+:param label_length: label length (in inches) (required for printer scaling) (optional)
+
 :param queue: printer queue (string) (optional)
 
 ## def set_queue(queue):
 Set Printer Queue.
 
 :param queue: printer queue (string)
 
@@ -24,28 +28,32 @@
 ## def get_printer_dpi(queue = None):
 Get Printer DPI.
 
 :param queue: printer queue (string) (optional)
 
 :return: printer DPI (int)
 
-## def get_label_dpi(commands):
+## def get_label_dpi(commands, label_width, label_length):
 Get Label DPI.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches)
+
+:param label_length: label length (in inches)
+
 :return: label DPI (int)
 
-## def setup(label_height, label_width, direct_thermal = None):
+## def setup(label_width, label_height, direct_thermal = None):
 Setup Printer Parameters Manually.
 
-:param label_height: tuple (label height, label gap) (in dots)
-
 :param label_width: label width (in dots)
 
+:param label_height: tuple (label height, label gap) (in dots)
+
 :param direct_thermal: True if using direct thermal labels (bool) (optional)
 
 ## def autosense():
 Autosense Label Parameters.
 
 ## def reset():
 Reset Printer.
```

### Comparing `TrimbleZebraPrinting-1.1.6/pyproject.toml` & `TrimbleZebraPrinting-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TrimbleZebraPrinting"
-version = "1.1.6"
+version = "1.2"
 authors = [
   { name="Ryan Strasburg", email="ryan_strasburg@trimble.com" },
 ]
 description = "Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/trimble_graphics_conversion.py` & `TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/trimble_graphics_conversion.py`

 * *Files identical despite different names*

### Comparing `TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting/trimble_zebra_printing.py` & `TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting/trimble_zebra_printing.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,28 +162,33 @@
                 win32print.WritePrinter(hPrinter, commands)
                 win32print.EndPagePrinter(hPrinter)
             finally:
                 win32print.EndDocPrinter(hPrinter)
         finally:
             win32print.ClosePrinter(hPrinter)
 
-    def print_label(self, commands, queue = None):
+    def print_label(self, commands, label_width = None, label_length = None, queue = None):
         """
         Print Label Using ZPL Commands.
         :param commands: ZPL command (string)
+        :param label_width: label width (in inches) (required for printer scaling) (optional)
+        :param label_length: label length (in inches) (required for printer scaling) (optional)
         :param queue: printer queue (string) (optional)
         """
         if queue is None:
             self.queue = win32print.GetDefaultPrinter()
         else:
             self.queue = queue
         printer_dpi = self.get_printer_dpi(self.queue)
-        label_dpi = self.get_label_dpi(commands)
-        if printer_dpi > 0 and label_dpi > 0 and label_dpi != printer_dpi:
-            self._output(self._rescale(commands, printer_dpi, label_dpi))
+        if label_width != None or label_length != None:
+            label_dpi = self.get_label_dpi(commands, label_width, label_length)
+            if printer_dpi > 0 and label_dpi > 0 and label_dpi != printer_dpi:
+                self._output(self._rescale(commands, printer_dpi, label_dpi))
+            else:
+                self._output(commands)
         else:
             self._output(commands)
 
     def set_queue(self, queue):
         """
         Set Printer Queue.
         :param queue: printer queue (string)
@@ -211,39 +216,50 @@
         for (_, _, name, _) in win32print.EnumPrinters(win32print.PRINTER_ENUM_LOCAL):
             if name == queue:
                 hPrinter = win32print.OpenPrinter(name)
                 port = win32print.GetPrinter(hPrinter, 2)['pPortName']
                 return win32print.DeviceCapabilities(name, port, 13)[0]['xdpi']
         return 0
 
-    def get_label_dpi(self, commands):
+    def get_label_dpi(self, commands, label_width, label_length):
         """
         Get Label DPI.
         :param commands: ZPL command (string)
+        :param label_width: label width (in inches)
+        :param label_length: label length (in inches)
         :return: label DPI (int)
         """
-        pattern = r'\^LL\d{3}'
-        if tgc.re.search(pattern, commands):
-            dpi = tgc.re.search(pattern, commands)
-            return int(dpi.group().strip('^LL'))
-        else:
-            return 0
+        width_pattern = r'\^PW\d+'
+        length_pattern = r'\^LL\d+'
+        if tgc.re.search(length_pattern, commands) and tgc.re.search(width_pattern, commands):
+            width = int(tgc.re.search(width_pattern, commands).group().strip('^PW'))
+            length = int(tgc.re.search(length_pattern, commands).group().strip('^LL'))
+            dpi_options = [203, 300, 600]
+            dpi_width = min(dpi_options, key = lambda x:abs(x - width / label_width))
+            dpi_length = min(dpi_options, key = lambda x:abs(x - length / label_length))
+            if dpi_width == dpi_length and dpi_width == dpi_options[0]:
+                return dpi_options[0]
+            elif dpi_width == dpi_length and dpi_width == dpi_options[1]:
+                return dpi_options[1]
+            elif dpi_width == dpi_length and dpi_width == dpi_options[2]:
+                return dpi_options[2]
+        return 0
 
-    def setup(self, label_height, label_width, direct_thermal = None):
+    def setup(self, label_width, label_length, direct_thermal = None):
         """
         Setup Printer Parameters Manually.
-        :param label_height: tuple (label height, label gap) (in dots)
         :param label_width: label width (in dots)
+        :param label_length: tuple (label length, label gap) (in dots)
         :param direct_thermal: True if using direct thermal labels (bool) (optional)
         """
         commands = '\n'
         if direct_thermal:
             commands += 'OD\n'
-        commands += 'Q%s,%s\n' % (label_height[0], label_height[1])
         commands += 'q%s\n' % label_width
+        commands += 'Q%s,%s\n' % (label_length[0], label_length[1])
         self._output(commands)
 
     def autosense(self):
          """
          Autosense Label Parameters.
          """
          self._output('\nxa\n')
@@ -267,11 +283,11 @@
     test_commands = ("""N\n"""
                      """A40,80,0,4,1,1,N,"Trimble Inc."\n"""
                      """A40,198,0,3,1,1,N,"ARFC Label Printing"\n"""
                      """A40,240,0,3,1,1,N,"Created On: March 31, 2023"\n"""
                      """A40,320,0,4,1,1,N,"With Trimble, Work Works Now."\n"""
                      """P1\n""")
     z = Zebra()
-    z.setup((406, 32), 812, True)
+    z.setup(609, (1015, 32), True)
     z.print_label(test_commands)
     print('~ Printer Commands ~' + '\n' + test_commands)
     print('Printer Queues:', z.get_queues(), '\n')
```

### Comparing `TrimbleZebraPrinting-1.1.6/src/TrimbleZebraPrinting.egg-info/PKG-INFO` & `TrimbleZebraPrinting-1.2/src/TrimbleZebraPrinting.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TrimbleZebraPrinting
-Version: 1.1.6
+Version: 1.2
 Summary: Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended.
 Author-email: Ryan Strasburg <ryan_strasburg@trimble.com>
 Project-URL: Homepage, https://github.com/ryan-strasburg/Trimble-Zebra-Printing
 Project-URL: Bug Tracker, https://github.com/ryan-strasburg/Trimble-Zebra-Printing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,19 +14,23 @@
 
 # Trimble Zebra Printing
 Trimble Zebra Printing was built to simplify and standardize ZPL printing in the Trimble Facilities. This includes features, such as DPI scaling, to improve printing automation. Upscaling DPI results in a loss of quality. Matching DPIs or downscaling is recommended.
 
 # class Zebra
 Class To Communicate & Print With (Zebra) Label Printers.
 
-## def print_label(commands, queue = None):
+## def print_label(commands, label_width = None, label_length = None, queue = None):
 Print Label Using ZPL Commands.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches) (required for printer scaling) (optional)
+
+:param label_length: label length (in inches) (required for printer scaling) (optional)
+
 :param queue: printer queue (string) (optional)
 
 ## def set_queue(queue):
 Set Printer Queue.
 
 :param queue: printer queue (string)
 
@@ -38,28 +42,32 @@
 ## def get_printer_dpi(queue = None):
 Get Printer DPI.
 
 :param queue: printer queue (string) (optional)
 
 :return: printer DPI (int)
 
-## def get_label_dpi(commands):
+## def get_label_dpi(commands, label_width, label_length):
 Get Label DPI.
 
 :param commands: ZPL command (string)
 
+:param label_width: label width (in inches)
+
+:param label_length: label length (in inches)
+
 :return: label DPI (int)
 
-## def setup(label_height, label_width, direct_thermal = None):
+## def setup(label_width, label_height, direct_thermal = None):
 Setup Printer Parameters Manually.
 
-:param label_height: tuple (label height, label gap) (in dots)
-
 :param label_width: label width (in dots)
 
+:param label_height: tuple (label height, label gap) (in dots)
+
 :param direct_thermal: True if using direct thermal labels (bool) (optional)
 
 ## def autosense():
 Autosense Label Parameters.
 
 ## def reset():
 Reset Printer.
```

