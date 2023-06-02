# Comparing `tmp/readlog-1.1.5.tar.gz` & `tmp/readlog-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.5.tar", last modified: Fri Jun  2 08:51:46 2023, max compression
+gzip compressed data, was "readlog-1.1.6.tar", last modified: Fri Jun  2 09:20:10 2023, max compression
```

## Comparing `readlog-1.1.5.tar` & `readlog-1.1.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.863226 readlog-1.1.5/
--rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      745 2023-06-02 08:51:46.862226 readlog-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-06-02 08:50:15.000000 readlog-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.818194 readlog-1.1.5/demo/
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.820178 readlog-1.1.5/demo/__pycache__/
--rw-rw-rw-   0        0        0     5361 2023-06-02 08:42:26.000000 readlog-1.1.5/demo/__pycache__/readlog.cpython-311.pyc
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.822178 readlog-1.1.5/demo/imgs/
--rw-rw-rw-   0        0        0   220194 2023-06-02 08:49:13.000000 readlog-1.1.5/demo/imgs/PotEng.png
--rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.5/demo/log.lammps
--rw-rw-rw-   0        0        0    76031 2023-06-02 08:50:50.000000 readlog-1.1.5/demo/log_incomplete.lammps
--rw-rw-rw-   0        0        0     1235 2023-06-02 08:51:24.000000 readlog-1.1.5/demo/plot_themo.py
--rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 08:51:46.863226 readlog-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-06-02 08:43:18.000000 readlog-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.825177 readlog-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-02 08:51:46.859223 readlog-1.1.5/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      745 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 08:51:46.000000 readlog-1.1.5/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3000 2023-06-02 08:51:40.000000 readlog-1.1.5/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.349255 readlog-1.1.6/
+-rw-rw-rw-   0        0        0      128 2023-06-02 08:43:49.000000 readlog-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      759 2023-06-02 09:20:10.348256 readlog-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-06-02 09:15:04.000000 readlog-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.320907 readlog-1.1.6/demo/
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.322905 readlog-1.1.6/demo/__pycache__/
+-rw-rw-rw-   0        0        0     5361 2023-06-02 08:42:26.000000 readlog-1.1.6/demo/__pycache__/readlog.cpython-311.pyc
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.328214 readlog-1.1.6/demo/imgs/
+-rw-rw-rw-   0        0        0   220194 2023-06-02 08:49:13.000000 readlog-1.1.6/demo/imgs/PotEng.png
+-rw-rw-rw-   0        0        0   219866 2023-06-02 08:52:03.000000 readlog-1.1.6/demo/imgs/PotEng_incomplete.png
+-rw-rw-rw-   0        0        0    80925 2023-06-02 08:38:09.000000 readlog-1.1.6/demo/log.lammps
+-rw-rw-rw-   0        0        0    76031 2023-06-02 08:50:50.000000 readlog-1.1.6/demo/log_incomplete.lammps
+-rw-rw-rw-   0        0        0     1235 2023-06-02 08:51:24.000000 readlog-1.1.6/demo/plot_themo.py
+-rw-rw-rw-   0        0        0       49 2023-05-30 13:49:56.000000 readlog-1.1.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:20:10.349255 readlog-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-02 09:19:57.000000 readlog-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.331206 readlog-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 09:20:10.345277 readlog-1.1.6/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      759 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-02 09:20:10.000000 readlog-1.1.6/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3000 2023-06-02 08:51:40.000000 readlog-1.1.6/src/readlog.py
```

### Comparing `readlog-1.1.5/PKG-INFO` & `readlog-1.1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.5
+Version: 1.1.6
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
 
 - A python code to read thermo info from lammps log file 
 
 ### Installation 
 
 ```bash
-git clone https://github.com/eastsheng/ReadLog.git
-cd ReadLog
-python setup.py sdist
+git clone https://github.com/eastsheng/readlog.git
+cd readlog
 pip install .
+# or
+pip install readlog
 ```
 
 ### Requirements
 
 - numpy
 - pandas
 - matplotlib
@@ -31,15 +32,17 @@
 - run `plot_themo.py` in `demo` folder:
 
   ```bash
   python plot_thermo.py
   ```
 
 - out:
-- ![](README/_img/PotEng.png)
+- ![](./demo/imgs/PotEng.png)
 
 
 
 ### Fixed
 
-- Can adapt to incomplete thermo information
+- [x] Adapting to incomplete thermo information.
+
+
```

### Comparing `readlog-1.1.5/demo/__pycache__/readlog.cpython-311.pyc` & `readlog-1.1.6/demo/__pycache__/readlog.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `readlog-1.1.5/demo/imgs/PotEng.png` & `readlog-1.1.6/demo/imgs/PotEng.png`

 * *Files identical despite different names*

### Comparing `readlog-1.1.5/demo/log.lammps` & `readlog-1.1.6/demo/log.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.5/demo/log_incomplete.lammps` & `readlog-1.1.6/demo/log_incomplete.lammps`

 * *Files identical despite different names*

### Comparing `readlog-1.1.5/demo/plot_themo.py` & `readlog-1.1.6/demo/plot_themo.py`

 * *Files identical despite different names*

### Comparing `readlog-1.1.5/setup.py` & `readlog-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.5',
+version      = '1.1.6',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.5/src/readlog.egg-info/PKG-INFO` & `readlog-1.1.6/src/readlog.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.5
+Version: 1.1.6
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
 
 - A python code to read thermo info from lammps log file 
 
 ### Installation 
 
 ```bash
-git clone https://github.com/eastsheng/ReadLog.git
-cd ReadLog
-python setup.py sdist
+git clone https://github.com/eastsheng/readlog.git
+cd readlog
 pip install .
+# or
+pip install readlog
 ```
 
 ### Requirements
 
 - numpy
 - pandas
 - matplotlib
@@ -31,15 +32,17 @@
 - run `plot_themo.py` in `demo` folder:
 
   ```bash
   python plot_thermo.py
   ```
 
 - out:
-- ![](README/_img/PotEng.png)
+- ![](./demo/imgs/PotEng.png)
 
 
 
 ### Fixed
 
-- Can adapt to incomplete thermo information
+- [x] Adapting to incomplete thermo information.
+
+
```

### Comparing `readlog-1.1.5/src/readlog.py` & `readlog-1.1.6/src/readlog.py`

 * *Files identical despite different names*

