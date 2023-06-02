# Comparing `tmp/loadtime-1.0.0.tar.gz` & `tmp/loadtime-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadtime-1.0.0.tar", last modified: Thu Jun  1 13:14:36 2023, max compression
+gzip compressed data, was "loadtime-1.0.1.tar", last modified: Fri Jun  2 01:28:46 2023, max compression
```

## Comparing `loadtime-1.0.0.tar` & `loadtime-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 13:14:36.235660 loadtime-1.0.0/
--rw-rw-rw-   0        0        0    11364 2023-06-01 10:17:46.000000 loadtime-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3797 2023-06-01 13:14:36.235660 loadtime-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3072 2023-06-01 13:11:40.000000 loadtime-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 13:14:36.213352 loadtime-1.0.0/loadtime/
--rw-rw-rw-   0        0        0       31 2023-06-01 10:27:06.000000 loadtime-1.0.0/loadtime/__init__.py
--rw-rw-rw-   0        0        0     8078 2023-06-01 09:20:07.000000 loadtime-1.0.0/loadtime/load_time.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:14:36.225417 loadtime-1.0.0/loadtime.egg-info/
--rw-rw-rw-   0        0        0     3797 2023-06-01 13:14:36.000000 loadtime-1.0.0/loadtime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-06-01 13:14:36.000000 loadtime-1.0.0/loadtime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 13:14:36.000000 loadtime-1.0.0/loadtime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 13:14:36.000000 loadtime-1.0.0/loadtime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 13:14:36.235660 loadtime-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-06-01 12:39:50.000000 loadtime-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 13:14:36.226418 loadtime-1.0.0/tests/
--rw-rw-rw-   0        0        0     3326 2023-06-01 09:03:47.000000 loadtime-1.0.0/tests/test_load_time.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.095141 loadtime-1.0.1/
+-rw-rw-rw-   0        0        0    11364 2023-06-01 10:17:46.000000 loadtime-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-06-01 13:30:18.000000 loadtime-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3815 2023-06-02 01:28:46.095141 loadtime-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3088 2023-06-02 01:27:09.000000 loadtime-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.082141 loadtime-1.0.1/loadtime/
+-rw-rw-rw-   0        0        0       31 2023-06-01 10:27:06.000000 loadtime-1.0.1/loadtime/__init__.py
+-rw-rw-rw-   0        0        0     8125 2023-06-02 01:27:09.000000 loadtime-1.0.1/loadtime/load_time.py
+drwxrwxrwx   0        0        0        0 2023-06-02 01:28:46.094141 loadtime-1.0.1/loadtime.egg-info/
+-rw-rw-rw-   0        0        0     3815 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 01:28:46.000000 loadtime-1.0.1/loadtime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       98 2023-06-01 13:22:49.000000 loadtime-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      665 2023-06-02 01:28:46.096141 loadtime-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-06-02 01:27:09.000000 loadtime-1.0.1/setup.py
```

### Comparing `loadtime-1.0.0/LICENSE` & `loadtime-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loadtime-1.0.0/PKG-INFO` & `loadtime-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadtime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to display a progress bar for long processes with uncertain end times
 Home-page: https://github.com/riversun/LoadTime
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -67,29 +67,31 @@
 ```python
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 from loadtime import LoadTime
 
 model_path = "togethercomputer/RedPajama-INCITE-Chat-3B-v1"
 
-tokenizer = AutoTokenizer.from_pretrained(model_path)
 model = LoadTime(name=model_path,
                  fn=lambda: AutoModelForCausalLM.from_pretrained(model_path, torch_dtype=torch.float16))()
+
+tokenizer = AutoTokenizer.from_pretrained(model_path) # important: load tokenizer after loading model
+
 ```
 
 
 ## Initial Parameters
 
-  | Parameter | Description |
-    |-----------|-------------|
-    | name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
-    | message   | Specify the message to be displayed. If omitted, the default message is used. |
-    | pbar      | Set to True to display the progress bar and percentage. |
-    | dirname   | Directory name for cache storage. |
-    | hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
-    | fn        | Function to execute the long-term process. |
-    | fn_print  | Function to perform the display. If omitted, it will be output to the console. |
+| Parameter | Description |
+|-----------|-------------|
+| name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
+| message   | Specify the message to be displayed. If omitted, the default message is used. |
+| pbar      | Set to True to display the progress bar and percentage. |
+| dirname   | Directory name for cache storage. |
+| hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
+| fn        | Function to execute the long-term process. |
+| fn_print  | Function to perform the display. If omitted, it will be output to the console. |
 
 
 Take control of your loading times with LoadTime!
```

### Comparing `loadtime-1.0.0/README.md` & `loadtime-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -50,29 +50,31 @@
 ```python
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 from loadtime import LoadTime
 
 model_path = "togethercomputer/RedPajama-INCITE-Chat-3B-v1"
 
-tokenizer = AutoTokenizer.from_pretrained(model_path)
 model = LoadTime(name=model_path,
                  fn=lambda: AutoModelForCausalLM.from_pretrained(model_path, torch_dtype=torch.float16))()
+
+tokenizer = AutoTokenizer.from_pretrained(model_path) # important: load tokenizer after loading model
+
 ```
 
 
 ## Initial Parameters
 
-  | Parameter | Description |
-    |-----------|-------------|
-    | name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
-    | message   | Specify the message to be displayed. If omitted, the default message is used. |
-    | pbar      | Set to True to display the progress bar and percentage. |
-    | dirname   | Directory name for cache storage. |
-    | hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
-    | fn        | Function to execute the long-term process. |
-    | fn_print  | Function to perform the display. If omitted, it will be output to the console. |
+| Parameter | Description |
+|-----------|-------------|
+| name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
+| message   | Specify the message to be displayed. If omitted, the default message is used. |
+| pbar      | Set to True to display the progress bar and percentage. |
+| dirname   | Directory name for cache storage. |
+| hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
+| fn        | Function to execute the long-term process. |
+| fn_print  | Function to perform the display. If omitted, it will be output to the console. |
 
 
 Take control of your loading times with LoadTime!
```

### Comparing `loadtime-1.0.0/loadtime/load_time.py` & `loadtime-1.0.1/loadtime/load_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         else:
             def console_print_func(str):
                 print(f'{str}', end='', flush=True)
 
             self.fn_print = console_print_func
 
         # If this is for a HuggingFace model and the model is not cached yet, suppress the output
+
         if self.hf is True and self.is_model_cached(self.name) is False:
             self.fn_print = None
 
         if self.fn is None:
             raise TypeError('fn not set')
 
     def clear_stored_data(self):
@@ -119,15 +120,16 @@
                     progress_disp = self._create_percentage_disp(percentage)
 
             if self.message is not None:
                 self.last_message = f'\r{self.message}{total_time_disp}'
             else:
                 self.last_message = f'\rLoading "{self.name}" ... {total_time_disp}'
 
-            self.fn_print(f'\r{self.last_message}{progress_disp}')
+            if self.fn_print is not None:
+                self.fn_print(f'\r{self.last_message}{progress_disp}')
 
             time.sleep(0.5)  # update every 0.5 seconds
 
     def _create_percentage_disp(self, percentage):
         """
         Creates a progress bar display string with the given completion percentage.
         """
```

### Comparing `loadtime-1.0.0/loadtime.egg-info/PKG-INFO` & `loadtime-1.0.1/loadtime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadtime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package to display a progress bar for long processes with uncertain end times
 Home-page: https://github.com/riversun/LoadTime
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -67,29 +67,31 @@
 ```python
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM
 from loadtime import LoadTime
 
 model_path = "togethercomputer/RedPajama-INCITE-Chat-3B-v1"
 
-tokenizer = AutoTokenizer.from_pretrained(model_path)
 model = LoadTime(name=model_path,
                  fn=lambda: AutoModelForCausalLM.from_pretrained(model_path, torch_dtype=torch.float16))()
+
+tokenizer = AutoTokenizer.from_pretrained(model_path) # important: load tokenizer after loading model
+
 ```
 
 
 ## Initial Parameters
 
-  | Parameter | Description |
-    |-----------|-------------|
-    | name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
-    | message   | Specify the message to be displayed. If omitted, the default message is used. |
-    | pbar      | Set to True to display the progress bar and percentage. |
-    | dirname   | Directory name for cache storage. |
-    | hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
-    | fn        | Function to execute the long-term process. |
-    | fn_print  | Function to perform the display. If omitted, it will be output to the console. |
+| Parameter | Description |
+|-----------|-------------|
+| name      | Name of the long-term process. For loading HuggingFace models, specify the model name. |
+| message   | Specify the message to be displayed. If omitted, the default message is used. |
+| pbar      | Set to True to display the progress bar and percentage. |
+| dirname   | Directory name for cache storage. |
+| hf        | Set to True to use for time display for loading HuggingFace models. If the model data has not yet been downloaded to the disk, HuggingFace's loader displays the download progress, so this library does not display it. |
+| fn        | Function to execute the long-term process. |
+| fn_print  | Function to perform the display. If omitted, it will be output to the console. |
 
 
 Take control of your loading times with LoadTime!
```

### Comparing `loadtime-1.0.0/setup.py` & `loadtime-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="loadtime",
-    version="1.0.0",
+    version="1.0.1",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="Package to display a progress bar for long processes with uncertain end times",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/LoadTime",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
```

