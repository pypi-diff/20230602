# Comparing `tmp/robotransforms-0.5.2.tar.gz` & `tmp/robotransforms-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotransforms-0.5.2.tar", last modified: Thu May  4 21:54:38 2023, max compression
+gzip compressed data, was "robotransforms-0.5.3.tar", last modified: Thu Jun  1 22:33:19 2023, max compression
```

## Comparing `robotransforms-0.5.2.tar` & `robotransforms-0.5.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.2/LICENSE
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.2/MANIFEST.in
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-04 21:54:38.364235 robotransforms-0.5.2/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.2/README.md
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.2/pyproject.toml
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.352235 robotransforms-0.5.2/robotransforms/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-05-04 21:53:50.000000 robotransforms-0.5.2/robotransforms/_version.py
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.360235 robotransforms-0.5.2/robotransforms/dead_reckon/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/dead_reckon/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8894 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/dead_reckon/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/dead_reckon/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6652 2023-05-04 21:53:40.000000 robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.2/robotransforms/dead_reckon/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/robotransforms/euclidean/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/euclidean/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/euclidean.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.2/robotransforms/euclidean/euclidean_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.2/robotransforms/euclidean/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.364235 robotransforms-0.5.2/robotransforms/utils/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/__init__.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.2/robotransforms/utils/base.cpp
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/base.h
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/utils.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/utils_pure.py
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.2/robotransforms/utils/wrapper.cpp
-drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-05-04 21:54:38.360235 robotransforms-0.5.2/robotransforms.egg-info/
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-05-04 21:54:38.000000 robotransforms-0.5.2/robotransforms.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-05-04 21:54:38.364235 robotransforms-0.5.2/setup.cfg
--rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.2/setup.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1076 2022-12-01 23:55:43.000000 robotransforms-0.5.3/LICENSE
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       37 2022-12-02 15:43:21.000000 robotransforms-0.5.3/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-01 22:33:19.342161 robotransforms-0.5.3/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      347 2023-05-03 23:31:19.000000 robotransforms-0.5.3/README.md
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       60 2023-05-03 23:34:03.000000 robotransforms-0.5.3/pyproject.toml
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.330161 robotransforms-0.5.3/robotransforms/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      148 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       22 2023-06-01 22:30:33.000000 robotransforms-0.5.3/robotransforms/_version.py
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.338161 robotransforms-0.5.3/robotransforms/dead_reckon/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/dead_reckon/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    10020 2023-06-01 22:30:33.000000 robotransforms-0.5.3/robotransforms/dead_reckon/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      732 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/dead_reckon/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     2811 2023-03-07 00:07:47.000000 robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     7588 2023-06-01 22:30:47.000000 robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    15825 2023-03-07 00:44:08.000000 robotransforms-0.5.3/robotransforms/dead_reckon/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/robotransforms/euclidean/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      120 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/euclidean/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     8310 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1566 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    11585 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/euclidean.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)    14307 2023-05-04 15:04:49.000000 robotransforms-0.5.3/robotransforms/euclidean/euclidean_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6960 2023-05-03 23:28:26.000000 robotransforms-0.5.3/robotransforms/euclidean/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.342161 robotransforms-0.5.3/robotransforms/utils/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       55 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/__init__.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     3680 2022-12-02 19:58:46.000000 robotransforms-0.5.3/robotransforms/utils/base.cpp
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      351 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/base.h
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      545 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/utils.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1055 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/utils_pure.py
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     6290 2022-12-02 15:43:21.000000 robotransforms-0.5.3/robotransforms/utils/wrapper.cpp
+drwxrwxr-x   0 jonathan  (1001) jonathan  (1001)        0 2023-06-01 22:33:19.338161 robotransforms-0.5.3/robotransforms.egg-info/
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      670 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)      943 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)        1 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       12 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       67 2023-06-01 22:33:19.000000 robotransforms-0.5.3/robotransforms.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)       38 2023-06-01 22:33:19.342161 robotransforms-0.5.3/setup.cfg
+-rw-rw-r--   0 jonathan  (1001) jonathan  (1001)     1907 2022-12-02 17:09:02.000000 robotransforms-0.5.3/setup.py
```

### Comparing `robotransforms-0.5.2/LICENSE` & `robotransforms-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/PKG-INFO` & `robotransforms-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.2
+Version: 0.5.3
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.2/robotransforms/dead_reckon/base.h` & `robotransforms-0.5.3/robotransforms/dead_reckon/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon.py` & `robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/dead_reckon/dead_reckon_pure.py` & `robotransforms-0.5.3/robotransforms/dead_reckon/dead_reckon_pure.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,28 +51,36 @@
     if ( np.abs(vdiff) >= 1e-3 ) :
         rho = np.abs(np.tanh( vave / vdiff ))
 
     #  [ var_dl, cov_dldr, var_dr, var_b, var_c, var_d ]
     return [ ddl*ddl + 1e-8, rho*ddl*ddr, ddr*ddr + 1e-8 ] # TODO : these are estimates, based on gps's 1Hz
 
 def dead_reckon_apply(x_hat, P_hat, step):
+    SS = 7 # Full state size
+    SM = 6 # Manifold state size
 
-    # No-op if we didn't move
     if (step[1] == 0 and step[2] == 0):
-        return x_hat, P_hat
+        # If the tracks didn't move, then just update the quaternion-part. There are two reasons dl=dr=0:
+        #   1) The tracks didn't quite accrue a tick. In this case, the quaternion part might still have a
+        #      bit of rotation, that we don't want to loose. However, the error accrual is SUPER small, and
+        #      this should only happen 'infrequently' so the loss of error is probably negilible. Fun fact,
+        #      since the tick is gross, it turns out droping the quaternion correction builds up, so you loose
+        #      something like 20degs over a 180deg turn. Wild, dude.
+        #   2) The tracks really haven't been moving. In this case, the IMU is probably not moving either --
+        #      except for drift (which we are handling elsewhere in the KF), so we are fine to just accrue
+        #      the IMU corrections.
+        return np.hstack([x_hat[:3], t.compose_quat(x_hat[3:SS], step[3:SS])]), P_hat.copy()
 
     # Build up extended state vector
-    SS = 7
     z = np.zeros((SS+2))
     z[:SS] = x_hat[:]
     z[SS+0] = step[1]
     z[SS+1] = step[2]
 
     # Build up extended covariance on manifold
-    SM = 6
     P_z = np.zeros((SM+2,SM+2))
     P_z[:SM,:SM] = P_hat[:SM,:SM]
     e = dead_reckon_step_errors( step[1], step[2], step[7], step[8] )
     P_z[0+SM][0+SM] = e[0] # var_dl
     P_z[0+SM][1+SM] = e[1] # cov_dldr
     P_z[1+SM][0+SM] = e[1] # cov_dldr
     P_z[1+SM][1+SM] = e[2] # var_dr
```

### Comparing `robotransforms-0.5.2/robotransforms/dead_reckon/wrapper.cpp` & `robotransforms-0.5.3/robotransforms/dead_reckon/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/euclidean/base.cpp` & `robotransforms-0.5.3/robotransforms/euclidean/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/euclidean/base.h` & `robotransforms-0.5.3/robotransforms/euclidean/base.h`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/euclidean/euclidean.py` & `robotransforms-0.5.3/robotransforms/euclidean/euclidean.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/euclidean/euclidean_pure.py` & `robotransforms-0.5.3/robotransforms/euclidean/euclidean_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/euclidean/wrapper.cpp` & `robotransforms-0.5.3/robotransforms/euclidean/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/utils/base.cpp` & `robotransforms-0.5.3/robotransforms/utils/base.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/utils/utils.py` & `robotransforms-0.5.3/robotransforms/utils/utils.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/utils/utils_pure.py` & `robotransforms-0.5.3/robotransforms/utils/utils_pure.py`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms/utils/wrapper.cpp` & `robotransforms-0.5.3/robotransforms/utils/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/robotransforms.egg-info/PKG-INFO` & `robotransforms-0.5.3/robotransforms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotransforms
-Version: 0.5.2
+Version: 0.5.3
 Summary: A transformation library for robot motion
 Home-page: https://github.com/Nova-Dynamics/transforms-python
 Author: Jonathan D. B. Van Schenck
 Author-email: jvschenck@novadynamics.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `robotransforms-0.5.2/robotransforms.egg-info/SOURCES.txt` & `robotransforms-0.5.3/robotransforms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotransforms-0.5.2/setup.py` & `robotransforms-0.5.3/setup.py`

 * *Files identical despite different names*

