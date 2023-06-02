# Comparing `tmp/triangle_check-1.0.tar.gz` & `tmp/triangle_check-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triangle_check-1.0.tar", last modified: Fri Jun  2 07:17:58 2023, max compression
+gzip compressed data, was "triangle_check-1.1.tar", last modified: Fri Jun  2 14:29:04 2023, max compression
```

## Comparing `triangle_check-1.0.tar` & `triangle_check-1.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 07:17:58.143562 triangle_check-1.0/
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     6809 2023-06-02 07:17:09.000000 triangle_check-1.0/CLA.md
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     1079 2023-06-02 07:17:09.000000 triangle_check-1.0/License.txt
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     3576 2023-06-02 07:17:58.143562 triangle_check-1.0/PKG-INFO
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     2932 2023-06-02 07:17:09.000000 triangle_check-1.0/README.md
--rw-rw-r--   0 igosha    (1000) igosha    (1000)    60475 2023-06-02 07:17:09.000000 triangle_check-1.0/legal_notices.txt
--rw-rw-r--   0 igosha    (1000) igosha    (1000)      126 2023-06-02 07:17:09.000000 triangle_check-1.0/pyproject.toml
--rw-rw-r--   0 igosha    (1000) igosha    (1000)      853 2023-06-02 07:17:58.143562 triangle_check-1.0/setup.cfg
-drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 07:17:58.139562 triangle_check-1.0/triangle_check/
--rw-rw-r--   0 igosha    (1000) igosha    (1000)    14171 2023-06-02 07:17:09.000000 triangle_check-1.0/triangle_check/__init__.py
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     1846 2023-06-02 07:17:09.000000 triangle_check-1.0/triangle_check/__main__.py
-drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 07:17:58.143562 triangle_check-1.0/triangle_check.egg-info/
--rw-rw-r--   0 igosha    (1000) igosha    (1000)     3576 2023-06-02 07:17:58.000000 triangle_check-1.0/triangle_check.egg-info/PKG-INFO
--rw-rw-r--   0 igosha    (1000) igosha    (1000)      322 2023-06-02 07:17:58.000000 triangle_check-1.0/triangle_check.egg-info/SOURCES.txt
--rw-rw-r--   0 igosha    (1000) igosha    (1000)        1 2023-06-02 07:17:58.000000 triangle_check-1.0/triangle_check.egg-info/dependency_links.txt
--rw-rw-r--   0 igosha    (1000) igosha    (1000)       64 2023-06-02 07:17:58.000000 triangle_check-1.0/triangle_check.egg-info/entry_points.txt
--rw-rw-r--   0 igosha    (1000) igosha    (1000)       15 2023-06-02 07:17:58.000000 triangle_check-1.0/triangle_check.egg-info/top_level.txt
+drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 14:29:04.956286 triangle_check-1.1/
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     6809 2023-06-02 07:17:09.000000 triangle_check-1.1/CLA.md
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     1079 2023-06-02 07:17:09.000000 triangle_check-1.1/License.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     4016 2023-06-02 14:29:04.956286 triangle_check-1.1/PKG-INFO
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     3372 2023-06-02 11:43:42.000000 triangle_check-1.1/README.md
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)    60475 2023-06-02 07:17:09.000000 triangle_check-1.1/legal_notices.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)      126 2023-06-02 07:17:09.000000 triangle_check-1.1/pyproject.toml
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)      926 2023-06-02 14:29:04.956286 triangle_check-1.1/setup.cfg
+drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 14:29:04.952286 triangle_check-1.1/triangle_check/
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)    14171 2023-06-02 07:17:09.000000 triangle_check-1.1/triangle_check/__init__.py
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     1854 2023-06-02 11:43:42.000000 triangle_check-1.1/triangle_check/__main__.py
+drwxrwxr-x   0 igosha    (1000) igosha    (1000)        0 2023-06-02 14:29:04.956286 triangle_check-1.1/triangle_check.egg-info/
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)     4016 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/PKG-INFO
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)      359 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/SOURCES.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)        1 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/dependency_links.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)       64 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/entry_points.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)       50 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/requires.txt
+-rw-rw-r--   0 igosha    (1000) igosha    (1000)       15 2023-06-02 14:29:04.000000 triangle_check-1.1/triangle_check.egg-info/top_level.txt
```

### Comparing `triangle_check-1.0/CLA.md` & `triangle_check-1.1/CLA.md`

 * *Files identical despite different names*

### Comparing `triangle_check-1.0/License.txt` & `triangle_check-1.1/License.txt`

 * *Files identical despite different names*

### Comparing `triangle_check-1.0/PKG-INFO` & `triangle_check-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triangle_check
-Version: 1.0
+Version: 1.1
 Summary: Triangle Check: scan iTunes backups for traces of compromise by Operation Triangulation
 Home-page: https://github.com/KasperskyLab/triangle_check
 Author: Kaspersky Lab
 Author-email: triangulation@kaspersky.com
 Project-URL: Bug Tracker, https://github.com/KasperskyLab/triangle_check/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,33 +25,42 @@
 
 ## Prerequisites
 
 The script depends on: colorama (for pretty printing), pycryptodome
 
 ## Installation
 
+The triangle_check utility can be installed from [PyPI](https://pypi.org/project/triangle-check/) (recommended):
+
+```
+python -m pip install triangle_check
+```
+
 The script can be run as-is (the subdirectory *triangle_check* is required):
 
 ```
-python3 triangle_check.py 
+python -m pip install -r requirements.txt
+python triangle_check.py 
 ```
 
 It can also be built into a pip package:
 
 ```
-python3 -m build
-pip3 install dist/triangle_check-1.0-py3-none-any.whl
-
+git clone https://github.com/KasperskyLab/triangle_check
+cd triangle_check
+python -m build
+python -m pip install dist/triangle_check-1.0-py3-none-any.whl
 ```
 
+For Windows or Linux, alternatively use the [binary builds](https://github.com/KasperskyLab/triangle_check/releases) of the triangle_check utility.  
 
 ## Usage
 
 ```
-Usage: triangle_check.py /path/to/iTunes_backup [backup_password]
+Usage: python -m triangle_check /path/to/iTunes_backup [backup_password]
 ```
 
 ### iTunes backup location
 
 Locate the backup directory created by iTunes. The exact location depends on the OS and is described [here](https://support.apple.com/en-us/HT204215).
 The directory you are looking for should contain may subdirectories, and should include 'Manifest.db', 'Manifest.plist'. The backup may be encrypted
 with a password, if set up in iTunes. That password is required to decrypt password-protected backups.
```

### Comparing `triangle_check-1.0/README.md` & `triangle_check-1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,42 @@
 
 ## Prerequisites
 
 The script depends on: colorama (for pretty printing), pycryptodome
 
 ## Installation
 
+The triangle_check utility can be installed from [PyPI](https://pypi.org/project/triangle-check/) (recommended):
+
+```
+python -m pip install triangle_check
+```
+
 The script can be run as-is (the subdirectory *triangle_check* is required):
 
 ```
-python3 triangle_check.py 
+python -m pip install -r requirements.txt
+python triangle_check.py 
 ```
 
 It can also be built into a pip package:
 
 ```
-python3 -m build
-pip3 install dist/triangle_check-1.0-py3-none-any.whl
-
+git clone https://github.com/KasperskyLab/triangle_check
+cd triangle_check
+python -m build
+python -m pip install dist/triangle_check-1.0-py3-none-any.whl
 ```
 
+For Windows or Linux, alternatively use the [binary builds](https://github.com/KasperskyLab/triangle_check/releases) of the triangle_check utility.  
 
 ## Usage
 
 ```
-Usage: triangle_check.py /path/to/iTunes_backup [backup_password]
+Usage: python -m triangle_check /path/to/iTunes_backup [backup_password]
 ```
 
 ### iTunes backup location
 
 Locate the backup directory created by iTunes. The exact location depends on the OS and is described [here](https://support.apple.com/en-us/HT204215).
 The directory you are looking for should contain may subdirectories, and should include 'Manifest.db', 'Manifest.plist'. The backup may be encrypted
 with a password, if set up in iTunes. That password is required to decrypt password-protected backups.
```

### Comparing `triangle_check-1.0/legal_notices.txt` & `triangle_check-1.1/legal_notices.txt`

 * *Files identical despite different names*

### Comparing `triangle_check-1.0/setup.cfg` & `triangle_check-1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = triangle_check
-version = 1.0
+version = 1.1
 author = Kaspersky Lab
 author_email = triangulation@kaspersky.com
 description = Triangle Check: scan iTunes backups for traces of compromise by Operation Triangulation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KasperskyLab/triangle_check
 license_files = License.txt
@@ -18,14 +18,18 @@
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= .
 packages = find:
 python_requires = >=3.8
+install_requires = 
+	setuptools>=42
+	colorama==0.4.6
+	pycryptodome==3.17
 
 [options.packages.find]
 where = .
 
 [options.entry_points]
 console_scripts = 
 	triangle_check = triangle_check:__main__.main
```

### Comparing `triangle_check-1.0/triangle_check/__init__.py` & `triangle_check-1.1/triangle_check/__init__.py`

 * *Files identical despite different names*

### Comparing `triangle_check-1.0/triangle_check/__main__.py` & `triangle_check-1.1/triangle_check/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     dir = '.'
     password = None
     if len(sys.argv) == 1:
         print('Triangle Check: scan iTunes backups for traces of compromise by Operation Triangulation © 2023 AO Kaspersky Lab. All Rights Reserved.')
         print('\n  Contact: triangulation@kaspersky.com')
         print('  More info: https://securelist.ru/trng-2023/')
-        print('\nUsage: triangle_check.py /path/to/iTunes_backup [backup_password]')
+        print('\nUsage: python -m triangle_check /path/to/iTunes_backup [backup_password]')
         return
     if len(sys.argv) > 1:
         dir = sys.argv[1]
     if len(sys.argv) > 2:
         password = sys.argv[2].encode('utf-8')
 
     checker = IOSBackupChecker()
@@ -42,8 +42,8 @@
         sys.exit(2)
     else:
         print(Fore.GREEN + 'No traces of compromise were identified' + Fore.RESET)
         sys.exit(0)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `triangle_check-1.0/triangle_check.egg-info/PKG-INFO` & `triangle_check-1.1/triangle_check.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triangle-check
-Version: 1.0
+Version: 1.1
 Summary: Triangle Check: scan iTunes backups for traces of compromise by Operation Triangulation
 Home-page: https://github.com/KasperskyLab/triangle_check
 Author: Kaspersky Lab
 Author-email: triangulation@kaspersky.com
 Project-URL: Bug Tracker, https://github.com/KasperskyLab/triangle_check/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,33 +25,42 @@
 
 ## Prerequisites
 
 The script depends on: colorama (for pretty printing), pycryptodome
 
 ## Installation
 
+The triangle_check utility can be installed from [PyPI](https://pypi.org/project/triangle-check/) (recommended):
+
+```
+python -m pip install triangle_check
+```
+
 The script can be run as-is (the subdirectory *triangle_check* is required):
 
 ```
-python3 triangle_check.py 
+python -m pip install -r requirements.txt
+python triangle_check.py 
 ```
 
 It can also be built into a pip package:
 
 ```
-python3 -m build
-pip3 install dist/triangle_check-1.0-py3-none-any.whl
-
+git clone https://github.com/KasperskyLab/triangle_check
+cd triangle_check
+python -m build
+python -m pip install dist/triangle_check-1.0-py3-none-any.whl
 ```
 
+For Windows or Linux, alternatively use the [binary builds](https://github.com/KasperskyLab/triangle_check/releases) of the triangle_check utility.  
 
 ## Usage
 
 ```
-Usage: triangle_check.py /path/to/iTunes_backup [backup_password]
+Usage: python -m triangle_check /path/to/iTunes_backup [backup_password]
 ```
 
 ### iTunes backup location
 
 Locate the backup directory created by iTunes. The exact location depends on the OS and is described [here](https://support.apple.com/en-us/HT204215).
 The directory you are looking for should contain may subdirectories, and should include 'Manifest.db', 'Manifest.plist'. The backup may be encrypted
 with a password, if set up in iTunes. That password is required to decrypt password-protected backups.
```

