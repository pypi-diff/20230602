# Comparing `tmp/ab-test-simulator-0.0.6.tar.gz` & `tmp/ab-test-simulator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-simulator-0.0.6.tar", last modified: Fri Jun  2 12:56:48 2023, max compression
+gzip compressed data, was "ab-test-simulator-0.0.7.tar", last modified: Fri Jun  2 13:13:27 2023, max compression
```

## Comparing `ab-test-simulator-0.0.6.tar` & `ab-test-simulator-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.584619 ab-test-simulator-0.0.6/
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.6/LICENSE
--rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.6/MANIFEST.in
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 12:56:48.584507 ab-test-simulator-0.0.6/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.6/README.md
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.583135 ab-test-simulator-0.0.6/ab_test_simulator/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/__init__.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     4224 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/_modidx.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     3080 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/generator.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     5848 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/plotting.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/power.py
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      525 2023-06-02 12:56:32.000000 ab-test-simulator-0.0.6/ab_test_simulator/wrappers.py
-drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 12:56:48.584329 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/PKG-INFO
--rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/entry_points.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/not-zip-safe
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/requires.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-02 12:56:48.000000 ab-test-simulator-0.0.6/ab_test_simulator.egg-info/top_level.txt
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-02 12:56:21.000000 ab-test-simulator-0.0.6/settings.ini
--rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-02 12:56:48.584655 ab-test-simulator-0.0.6/setup.cfg
--rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.6/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 13:13:27.584826 ab-test-simulator-0.0.7/
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.7/LICENSE
+-rw-rw-r--   0 koljakleineberg   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ab-test-simulator-0.0.7/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 13:13:27.584726 ab-test-simulator-0.0.7/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5020 2023-06-01 14:37:46.000000 ab-test-simulator-0.0.7/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 13:13:27.583597 ab-test-simulator-0.0.7/ab_test_simulator/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     4224 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     3099 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5848 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7904 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      525 2023-06-02 13:11:20.000000 ab-test-simulator-0.0.7/ab_test_simulator/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-02 13:13:27.584553 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7419 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      516 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       77 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-05-31 12:40:20.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       18 2023-06-02 13:13:27.000000 ab-test-simulator-0.0.7/ab_test_simulator.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1054 2023-06-02 13:09:21.000000 ab-test-simulator-0.0.7/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-02 13:13:27.584861 ab-test-simulator-0.0.7/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-01 06:53:26.000000 ab-test-simulator-0.0.7/setup.py
```

### Comparing `ab-test-simulator-0.0.6/LICENSE` & `ab-test-simulator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/PKG-INFO` & `ab-test-simulator-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.6/README.md` & `ab-test-simulator-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator/_modidx.py` & `ab-test-simulator-0.0.7/ab_test_simulator/_modidx.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator/generator.py` & `ab-test-simulator-0.0.7/ab_test_simulator/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,8 +79,8 @@
     c0 = binom.rvs(n0, cr0, loc=0, size=1)[0]
     c1 = binom.rvs(n1, cr1, loc=0, size=1)[0]
     df_result = pd.DataFrame(
         {"group": [0, 1], "users": [n0, n1], "converted": [c0, c1]}
     )
     df_result["not_converted"] = df_result["users"] - df_result["converted"]
     df_result["cvr"] = df_result["converted"] / df_result["users"]
-    return df_result
+    return df_result.set_index('group')
```

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator/plotting.py` & `ab-test-simulator-0.0.7/ab_test_simulator/plotting.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator/power.py` & `ab-test-simulator-0.0.7/ab_test_simulator/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator/wrappers.py` & `ab-test-simulator-0.0.7/ab_test_simulator/wrappers.py`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator.egg-info/PKG-INFO` & `ab-test-simulator-0.0.7/ab_test_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ab-test-simulator
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple library to simulate AB tests.
 Home-page: https://github.com/k111git/ab-test-simulator
 Author: Kolja
 Author-email: 
 License: Apache Software License 2.0
 Description: # ab-test-simulator
```

### Comparing `ab-test-simulator-0.0.6/ab_test_simulator.egg-info/SOURCES.txt` & `ab-test-simulator-0.0.7/ab_test_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ab-test-simulator-0.0.6/settings.ini` & `ab-test-simulator-0.0.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-simulator
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_simulator
```

### Comparing `ab-test-simulator-0.0.6/setup.py` & `ab-test-simulator-0.0.7/setup.py`

 * *Files identical despite different names*

