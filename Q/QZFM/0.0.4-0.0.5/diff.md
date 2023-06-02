# Comparing `tmp/QZFM-0.0.4.tar.gz` & `tmp/QZFM-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QZFM-0.0.4.tar", last modified: Wed May 31 17:14:47 2023, max compression
+gzip compressed data, was "QZFM-0.0.5.tar", last modified: Fri Jun  2 15:50:11 2023, max compression
```

## Comparing `QZFM-0.0.4.tar` & `QZFM-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-05-31 17:14:47.619172 QZFM-0.0.4/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.4/LICENSE
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     2933 2023-05-31 17:14:47.619172 QZFM-0.0.4/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     2347 2023-05-31 17:12:55.000000 QZFM-0.0.4/README.md
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-05-31 17:13:17.000000 QZFM-0.0.4/pyproject.toml
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-05-31 17:14:47.619172 QZFM-0.0.4/setup.cfg
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-05-31 17:14:47.619172 QZFM-0.0.4/src/
-drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-05-31 17:14:47.619172 QZFM-0.0.4/src/QZFM.egg-info/
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     2933 2023-05-31 17:14:47.000000 QZFM-0.0.4/src/QZFM.egg-info/PKG-INFO
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-05-31 17:14:47.000000 QZFM-0.0.4/src/QZFM.egg-info/SOURCES.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-05-31 17:14:47.000000 QZFM-0.0.4/src/QZFM.egg-info/dependency_links.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-05-31 17:14:47.000000 QZFM-0.0.4/src/QZFM.egg-info/requires.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-05-31 17:14:47.000000 QZFM-0.0.4/src/QZFM.egg-info/top_level.txt
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33687 2023-05-31 17:13:44.000000 QZFM-0.0.4/src/QZFM.py
--rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.4/src/__init__.py
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     1067 2023-03-09 20:08:42.000000 QZFM-0.0.5/LICENSE
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-02 15:50:11.089205 QZFM-0.0.5/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9333 2023-05-31 19:47:23.000000 QZFM-0.0.5/README.md
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      799 2023-06-02 15:49:52.000000 QZFM-0.0.5/pyproject.toml
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       38 2023-06-02 15:50:11.089205 QZFM-0.0.5/setup.cfg
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/src/
+drwxrwxr-x   0 dfujimoto  (1000) dfujimoto  (1000)        0 2023-06-02 15:50:11.089205 QZFM-0.0.5/src/QZFM.egg-info/
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)     9919 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/PKG-INFO
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)      219 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/SOURCES.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)        1 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/dependency_links.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       47 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/requires.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       14 2023-06-02 15:50:11.000000 QZFM-0.0.5/src/QZFM.egg-info/top_level.txt
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)    33775 2023-06-02 15:49:42.000000 QZFM-0.0.5/src/QZFM.py
+-rw-rw-r--   0 dfujimoto  (1000) dfujimoto  (1000)       43 2023-03-16 18:47:16.000000 QZFM-0.0.5/src/__init__.py
```

### Comparing `QZFM-0.0.4/LICENSE` & `QZFM-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `QZFM-0.0.4/pyproject.toml` & `QZFM-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QZFM"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Derek Fujimoto", email="dfujimoto@triumf.ca" },
 ]
 description = "Python class for serial communication with QuSpin Zero Field Magnetometer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `QZFM-0.0.4/src/QZFM.py` & `QZFM-0.0.5/src/QZFM.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,17 @@
             # get current setting
             self.update_status()
             Bz_now = self.sensor_par['Bz field (pT)']
             By_now = self.sensor_par['By field (pT)']
             B0_now = self.sensor_par['B0 field (pT)']
             T_now = self.sensor_par['cell temp error']
 
+            if show:
+                print('\n'*5)
+
             try:
                 while True:
 
                     # track
                     Bz_last = Bz_now
                     By_last = By_now
                     B0_last = B0_now
@@ -353,19 +356,19 @@
                     Bz_now = self.sensor_par['Bz field (pT)']
                     By_now = self.sensor_par['By field (pT)']
                     B0_now = self.sensor_par['B0 field (pT)']
                     T_now = self.sensor_par['cell temp error']
 
                     # print
                     if show:
-                        lines = [f'Bz = {Bz_now:.4f} pT, dBz = {abs(Bz_now-Bz_last):.4f} pT',
-                                 f'By = {By_now:.4f} pT, dBy = {abs(By_now-By_last):.4f} pT',
-                                 f'B0 = {B0_now:.4f} pT, dB0 = {abs(B0_now-B0_last):.4f} pT',
+                        lines = [f'Bz = {Bz_now:.4f} pT, dBz = {abs(Bz_now-Bz_last):.4f} pT' + ' '*10,
+                                 f'By = {By_now:.4f} pT, dBy = {abs(By_now-By_last):.4f} pT' + ' '*10,
+                                 f'B0 = {B0_now:.4f} pT, dB0 = {abs(B0_now-B0_last):.4f} pT' + ' '*10,
                                  '',
-                                 f'T error = {T_now:.4f}',
+                                 f'T error = {T_now:.4f}' + ' '*10,
                                 ]
                         print("\033[F"*5 + '\n'.join(lines))
             except KeyboardInterrupt:
                 print()
 
             self.update_status()
```

