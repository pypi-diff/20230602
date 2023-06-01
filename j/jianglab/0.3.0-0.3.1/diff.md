# Comparing `tmp/jianglab-0.3.0.tar.gz` & `tmp/jianglab-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jianglab-0.3.0.tar", last modified: Thu Jun  1 23:04:00 2023, max compression
+gzip compressed data, was "jianglab-0.3.1.tar", last modified: Thu Jun  1 23:25:17 2023, max compression
```

## Comparing `jianglab-0.3.0.tar` & `jianglab-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:04:00.573712 jianglab-0.3.0/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 23:04:00.573212 jianglab-0.3.0/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.0/README.md
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:04:00.568491 jianglab-0.3.0/jianglab/
--rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.0/jianglab/__init__.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)    13324 2023-06-01 23:02:51.000000 jianglab-0.3.0/jianglab/common_functions.py
--rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.0/jianglab/params.py
-drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:04:00.572407 jianglab-0.3.0/jianglab.egg-info/
--rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 23:04:00.000000 jianglab-0.3.0/jianglab.egg-info/PKG-INFO
--rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 23:04:00.000000 jianglab-0.3.0/jianglab.egg-info/SOURCES.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 23:04:00.000000 jianglab-0.3.0/jianglab.egg-info/dependency_links.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 23:04:00.000000 jianglab-0.3.0/jianglab.egg-info/requires.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 23:04:00.000000 jianglab-0.3.0/jianglab.egg-info/top_level.txt
--rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 23:04:00.573928 jianglab-0.3.0/setup.cfg
--rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 23:03:57.000000 jianglab-0.3.0/setup.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:25:17.312898 jianglab-0.3.1/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 23:25:17.312248 jianglab-0.3.1/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)     1082 2023-04-13 14:33:05.000000 jianglab-0.3.1/README.md
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:25:17.308499 jianglab-0.3.1/jianglab/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       76 2023-05-30 15:41:31.000000 jianglab-0.3.1/jianglab/__init__.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)    13432 2023-06-01 23:24:59.000000 jianglab-0.3.1/jianglab/common_functions.py
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      400 2023-05-30 15:41:33.000000 jianglab-0.3.1/jianglab/params.py
+drwxr-xr-x   0 zhengjiang   (501) staff       (20)        0 2023-06-01 23:25:17.310951 jianglab-0.3.1/jianglab.egg-info/
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      593 2023-06-01 23:25:17.000000 jianglab-0.3.1/jianglab.egg-info/PKG-INFO
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      246 2023-06-01 23:25:17.000000 jianglab-0.3.1/jianglab.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        1 2023-06-01 23:25:17.000000 jianglab-0.3.1/jianglab.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       79 2023-06-01 23:25:17.000000 jianglab-0.3.1/jianglab.egg-info/requires.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)        9 2023-06-01 23:25:17.000000 jianglab-0.3.1/jianglab.egg-info/top_level.txt
+-rw-r--r--   0 zhengjiang   (501) staff       (20)       38 2023-06-01 23:25:17.313070 jianglab-0.3.1/setup.cfg
+-rw-r--r--   0 zhengjiang   (501) staff       (20)      924 2023-06-01 23:25:10.000000 jianglab-0.3.1/setup.py
```

### Comparing `jianglab-0.3.0/PKG-INFO` & `jianglab-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.0/README.md` & `jianglab-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `jianglab-0.3.0/jianglab/common_functions.py` & `jianglab-0.3.1/jianglab/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,17 @@
     return raw_data
 
 def get_acquisition_rate(filepath):
     raw_data = McsCMOSMEA.McsData(filepath)
     return 1/(float(raw_data.Acquisition.Sensor_Data.SensorMeta["Tick"])*1e-6) # in Hz
 
 def cmcr_to_nparray(filepath):
-    data = load_raw_data(filepath)
-    return data.Acquisition.Sensor_Data.SensorData_1_1
+    data = McsCMOSMEA.McsData(filepath)
+    data = np.array(data.Acquisition.Sensor_Data.SensorData_1_1)
+    return data
 
 def import_cmtr_firing_rate(filename, bin_size = 100): 
     """Import a .cmtr file and return a dictionary of units holding the timestamps and waveforms.
     :param filename: The path to the .cmtr file.
     :return: A dictionary of units holding the timestamps and waveforms.
 
     Note: 
@@ -230,25 +231,26 @@
 
 def resample_med(np_array, kernel_size = 101, resample_rate =10): # med filter through first axis
     counter = 0
     out_array = np.zeros_like(np_array)
     for i in tqdm(range(np_array.shape[1])):
         for j in range(np_array.shape[2]):
             counter += 1
-            if counter % 100 == 0:
-                print(counter, " out of 4225")
+            # if counter % 100 == 0:
+            #     print(counter, " out of 4225")
             out_array[:,i,j] = signal.medfilt(np_array[:,i,j], kernel_size=kernel_size)
     return out_array[::resample_rate]
 
-def get_lowpass_data(np_array, 
+def get_lowpass_data(raw_cmcr_data, 
                 pre_resample_rate = 100,
                 post_resample_rate = 10, 
                 kernel_size = 51):
         # total resample 1000 result in 20 Hz acq rate
         # 30 mins processing time for 10 mins data
+    np_array = raw_cmcr_data.Acquisition.Sensor_Data.SensorData_1_1
     images = np_array[::pre_resample_rate]
     images = resample_med(images, kernel_size= kernel_size, resample_rate = post_resample_rate) 
     return images
 
 
 def remove_bad_lanes(data, bad_lanes): # for low pass filtered data
     data = np.delete(data, [int(lane)-1 for lane in bad_lanes], axis= 2)
```

### Comparing `jianglab-0.3.0/jianglab.egg-info/PKG-INFO` & `jianglab-0.3.1/jianglab.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jianglab
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package for Jiang lab
 Home-page: https://github.com/jiang-lab-retina/jianglab.git
 Author: Jiang Zheng
 Author-email: zjiang314@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `jianglab-0.3.0/setup.py` & `jianglab-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jianglab',
-    version='0.3.0',
+    version='0.3.1',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "matplotlib",
         "treelib",
         "McsPyDataTools",
```

