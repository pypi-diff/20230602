# Comparing `tmp/jianglab-0.2.8.tar.gz` & `tmp/jianglab-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.2.8.tar", last modified: Thu Jun  1 17:42:31 2023, max compression
+gzip compressed data, was "jianglab-0.2.9.tar", last modified: Thu Jun  1 22:17:09 2023, max compression
```

## Comparing `jianglab-0.2.8.tar` & `jianglab-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.703123 jianglab-0.2.8/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 17:42:31.702810 jianglab-0.2.8/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.8/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.700202 jianglab-0.2.8/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.8/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    12878 2023-06-01 17:42:22.000000 jianglab-0.2.8/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.8/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 17:42:31.702317 jianglab-0.2.8/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 17:42:31.000000 jianglab-0.2.8/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 17:42:31.703247 jianglab-0.2.8/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 17:42:26.000000 jianglab-0.2.8/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 22:17:09.047085 jianglab-0.2.9/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 22:17:09.046756 jianglab-0.2.9/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.2.9/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 22:17:09.043812 jianglab-0.2.9/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.2.9/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    13308 2023-06-01 22:16:58.000000 jianglab-0.2.9/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.2.9/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 22:17:09.046193 jianglab-0.2.9/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 22:17:08.000000 jianglab-0.2.9/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 22:17:08.000000 jianglab-0.2.9/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 22:17:08.000000 jianglab-0.2.9/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 22:17:08.000000 jianglab-0.2.9/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 22:17:08.000000 jianglab-0.2.9/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 22:17:09.047198 jianglab-0.2.9/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 22:17:04.000000 jianglab-0.2.9/setup.py
```

### Comparing `jianglab-0.2.8/PKG-INFO` & `jianglab-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.8/README.md` & `jianglab-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.2.8/jianglab/common_functions.py` & `jianglab-0.2.9/jianglab/common_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from scipy.signal import find_peaks
 import matplotlib.pyplot as plt
 import gspread
 import pandas as pd
 from oauth2client.service_account import ServiceAccountCredentials
 import scipy.signal as signal
 from tqdm import tqdm
+import pickle
+
 
 def frame_ref_to_onset(frame_ref, first_onset_index = 184, visualize_window = (250_000,350_000), stimulus_interval = 60, on_duration = 30, sampling_rate = 20000,overlay_split_num = 5):
     '''
         Convert frame_ref to onset_index
         input:
             frame_ref: 2d array, first row is the light, second row is the frame
             first_onset_index: the index of the first onset, it needs to be manually adjusted
@@ -221,25 +223,35 @@
     creds_obj = ServiceAccountCredentials.from_json_keyfile_name(cred, scope)
     client = gspread.authorize(creds_obj)
     sheet = client.open(sheet_name).sheet1.get_all_records()
     df = pd.DataFrame.from_dict(sheet)
     df.to_csv("../gsheet_table.csv", index = False)
     return df
 
-def resample_med(np_array, kernel_size = 100, resample_rate =10): # med filter through first axis
+def resample_med(np_array, kernel_size = 101, resample_rate =10): # med filter through first axis
     counter = 0
     out_array = np.zeros_like(np_array)
     for i in tqdm(range(np_array.shape[1])):
         for j in range(np_array.shape[2]):
             counter += 1
             if counter % 100 == 0:
                 print(counter, " out of 4225")
             out_array[:,i,j] = signal.medfilt(np_array[:,i,j], kernel_size=kernel_size)
     return out_array[::resample_rate]
 
+def get_lowpass_data(np_array, 
+                pre_resample_rate = 100,
+                post_resample_rate = 10, 
+                kernel_size = 51):
+        # total resample 1000 result in 20 Hz acq rate
+        # 30 mins processing time for 10 mins data
+    images = np_array[::pre_resample_rate]
+    images = resample_med(images, kernel_size= kernel_size, resample_rate = post_resample_rate) 
+    return images
+
 
 def remove_bad_lanes(data, bad_lanes): # for low pass filtered data
     data = np.delete(data, [int(lane)-1 for lane in bad_lanes], axis= 2)
     return data
 
 def save_instance(filename, instance):
     with open(filename, "wb") as file_:
```

### Comparing `jianglab-0.2.8/jianglab.egg-info/PKG-INFO` & `jianglab-0.2.9/jianglab.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.2.8/setup.py` & `jianglab-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.2.8',
+    version='0.2.9',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

