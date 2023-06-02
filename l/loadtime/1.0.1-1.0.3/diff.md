# Comparing `tmp/loadtime-1.0.1.tar.gz` & `tmp/loadtime-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadtime-1.0.1.tar", last modified: Fri Jun  2 01:28:46 2023, max compression
+gzip compressed data, was "loadtime-1.0.3.tar", last modified: Fri Jun  2 02:44:27 2023, max compression
```

## Comparing `loadtime-1.0.1.tar` & `loadtime-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.095141 loadtime-1.0.1/
--rw-rw-rw-   0        0        0    11364 2023-06-01 10:17:46.000000 loadtime-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       27 2023-06-01 13:30:18.000000 loadtime-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3815 2023-06-02 01:28:46.095141 loadtime-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3088 2023-06-02 01:27:09.000000 loadtime-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.082141 loadtime-1.0.1/loadtime/
--rw-rw-rw-   0        0        0       31 2023-06-01 10:27:06.000000 loadtime-1.0.1/loadtime/__init__.py
--rw-rw-rw-   0        0        0     8125 2023-06-02 01:27:09.000000 loadtime-1.0.1/loadtime/load_time.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.094141 loadtime-1.0.1/loadtime.egg-info/
--rw-rw-rw-   0        0        0     3815 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       98 2023-06-01 13:22:49.000000 loadtime-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      665 2023-06-02 01:28:46.096141 loadtime-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-02 01:27:09.000000 loadtime-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:44:27.655490 loadtime-1.0.3/
+-rw-rw-rw-   0        0        0    11364 2023-06-01 10:17:46.000000 loadtime-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-06-01 13:30:18.000000 loadtime-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-06-02 02:44:27.655490 loadtime-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-06-02 01:27:09.000000 loadtime-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 02:44:27.643077 loadtime-1.0.3/loadtime/
+-rw-rw-rw-   0        0        0       31 2023-06-01 10:27:06.000000 loadtime-1.0.3/loadtime/__init__.py
+-rw-rw-rw-   0        0        0     8826 2023-06-02 02:35:02.000000 loadtime-1.0.3/loadtime/load_time.py
+drwxrwxrwx   0        0        0        0 2023-06-02 02:44:27.654076 loadtime-1.0.3/loadtime.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-06-02 02:44:27.000000 loadtime-1.0.3/loadtime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-02 02:44:27.000000 loadtime-1.0.3/loadtime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 02:44:27.000000 loadtime-1.0.3/loadtime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 02:44:27.000000 loadtime-1.0.3/loadtime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:22:49.000000 loadtime-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      665 2023-06-02 02:44:27.656229 loadtime-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-02 02:44:08.000000 loadtime-1.0.3/setup.py
```

### Comparing `loadtime-1.0.1/LICENSE` & `loadtime-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loadtime-1.0.1/PKG-INFO` & `loadtime-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadtime
-Version: 1.0.1
+Version: 1.0.3
 Summary: Package to display a progress bar for long processes with uncertain end times
 Home-page: https://github.com/riversun/LoadTime
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `loadtime-1.0.1/README.md` & `loadtime-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `loadtime-1.0.1/loadtime/load_time.py` & `loadtime-1.0.3/loadtime/load_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 import threading
 from datetime import timedelta
 import os
 import json
-
+import traceback
+import sys
 
 class LoadTime:
     def __init__(self, name="", message=None, pbar=True, dirname="loadtime", hf=False, fn=None, fn_print=None):
         """
         Initialize the LoadTime class
 
         :param name: Name of the long-term process. For loading HuggingFace models, specify the model name.
@@ -24,30 +25,32 @@
         self.thread = None
         self.stop_event = threading.Event()  # Event to signal the thread to stop
         self.fn = fn
         self.dirname = dirname
         self.show_percentage = pbar
         self._load_data()  # Load cached data if exists
         self.last_message = None
+        self.last_message_fin = None
         self.elapsed_time = -1
         self.fn_print = None
         self.hf = hf
+        self.is_model_cached=self.is_model_cached(self.name)
 
         # If a print function is provided, use it, else print to the console
         if fn_print is not None:
             self.fn_print = fn_print
         else:
             def console_print_func(str):
                 print(f'{str}', end='', flush=True)
 
             self.fn_print = console_print_func
 
         # If this is for a HuggingFace model and the model is not cached yet, suppress the output
 
-        if self.hf is True and self.is_model_cached(self.name) is False:
+        if self.hf is True and self.is_model_cached is False:
             self.fn_print = None
 
         if self.fn is None:
             raise TypeError('fn not set')
 
     def clear_stored_data(self):
         """Clears stored time data from previous runs"""
@@ -100,15 +103,16 @@
     def _display_time(self):
         """
         Runs in a separate thread to display the elapsed time, estimated total time, and progress bar if enabled.
         """
         while not self.stop_event.is_set():
             self.elapsed_time = time.time() - self.start_time
             formatted_time = self._get_formatted_time(self.elapsed_time)
-            total_time_disp = f"{formatted_time}"
+            total_time_disp = f"{formatted_time} (Now recording loading time)"
+            total_time_disp_fin = f"{formatted_time}/{formatted_time}"
             total_time_in_sec = self.stored_data.get('total_time', None)
 
             progress_disp = ""
 
             if total_time_in_sec is not None and int(total_time_in_sec) != 0:
                 total_time_disp = f"{formatted_time}/{self._get_formatted_time(total_time_in_sec)}"
 
@@ -117,16 +121,19 @@
                     if percentage > 1:
                         percentage = 1
 
                     progress_disp = self._create_percentage_disp(percentage)
 
             if self.message is not None:
                 self.last_message = f'\r{self.message}{total_time_disp}'
+                self.last_message_fin = f'\r{self.message}{total_time_disp_fin}'
+
             else:
                 self.last_message = f'\rLoading "{self.name}" ... {total_time_disp}'
+                self.last_message_fin = f'\rLoading "{self.name}" ... {total_time_disp_fin}'
 
             if self.fn_print is not None:
                 self.fn_print(f'\r{self.last_message}{progress_disp}')
 
             time.sleep(0.5)  # update every 0.5 seconds
 
     def _create_percentage_disp(self, percentage):
@@ -160,35 +167,44 @@
         Starts the timer and the execution of the function, displaying the time tracking.
         """
         ret = None
         if self.thread is None:
             self.start_time = time.time()
             self.thread = threading.Thread(target=self._display_time)
             self.thread.start()
-            ret = self.fn()
-            self.fn = None
-            self._stop()
+
+            try:
+                ret = self.fn()
+            except Exception as e:
+                tb = traceback.format_exc()
+                sys.stderr.write(tb)
+            finally:
+                self.fn = None
+                self._stop()
         return ret
 
     def _stop(self):
         """
         Stops the timer and the thread, saves the elapsed time for future reference.
         """
         if self.thread is not None:
             if self.stored_data.get("total_time", None) is not None:
-                self.fn_print(f'\r{self.last_message}{self._create_percentage_disp(1)}\n')
+                if self.fn_print is not None:
+                    self.fn_print(f'\r{self.last_message}{self._create_percentage_disp(1)}\n')
             else:
-                self.fn_print(f'\r{self.last_message}\n')
+                if self.fn_print is not None:
+                    self.fn_print(f'\r{self.last_message_fin}\n')
 
             self.stop_event.set()
             self.thread.join()
             self.thread = None
             self.stop_event.clear()
             self.stored_data["total_time"] = self.elapsed_time
-            self.save_dict_to_json(self.stored_data)
+            if self.is_model_cached:
+                self.save_dict_to_json(self.stored_data)
         return self
 
     def save_dict_to_json(self, data_dict):
         """
         Save a dictionary of data to a json file, named after the operation
 
         """
```

### Comparing `loadtime-1.0.1/loadtime.egg-info/PKG-INFO` & `loadtime-1.0.3/loadtime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadtime
-Version: 1.0.1
+Version: 1.0.3
 Summary: Package to display a progress bar for long processes with uncertain end times
 Home-page: https://github.com/riversun/LoadTime
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `loadtime-1.0.1/setup.cfg` & `loadtime-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `loadtime-1.0.1/setup.py` & `loadtime-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="loadtime",
-    version="1.0.1",
+    version="1.0.3",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="Package to display a progress bar for long processes with uncertain end times",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/LoadTime",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
```

