# Comparing `tmp/myPackageLicensePrototype-1.0.0.tar.gz` & `tmp/myPackageLicensePrototype-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.0.0.tar", last modified: Fri Jun  2 08:57:54 2023, max compression
+gzip compressed data, was "myPackageLicensePrototype-1.0.1.tar", last modified: Fri Jun  2 09:18:33 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.0.0.tar` & `myPackageLicensePrototype-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:57:54.380848 myPackageLicensePrototype-1.0.0/
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-02 08:57:54.380848 myPackageLicensePrototype-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-06-01 20:38:54.000000 myPackageLicensePrototype-1.0.0/README.md
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.0/local_environment_installation_guide.txt
--rw-rw-rw-   0        0        0      555 2023-06-01 20:50:12.000000 myPackageLicensePrototype-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 08:57:54.380848 myPackageLicensePrototype-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-06-02 08:57:50.000000 myPackageLicensePrototype-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:57:54.360758 myPackageLicensePrototype-1.0.0/src/
--rw-rw-rw-   0        0        0      936 2023-06-01 20:50:44.000000 myPackageLicensePrototype-1.0.0/src/Implementation.ipynb
--rw-rw-rw-   0        0        0      104 2023-06-02 08:55:03.000000 myPackageLicensePrototype-1.0.0/src/Implementation.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:57:54.379853 myPackageLicensePrototype-1.0.0/src/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-02 08:57:54.000000 myPackageLicensePrototype-1.0.0/src/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-06-02 08:57:54.000000 myPackageLicensePrototype-1.0.0/src/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 08:57:54.000000 myPackageLicensePrototype-1.0.0/src/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 08:57:54.000000 myPackageLicensePrototype-1.0.0/src/myPackageLicensePrototype.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 09:18:33.175579 myPackageLicensePrototype-1.0.1/
+-rw-rw-rw-   0        0        0      104 2023-06-02 08:55:03.000000 myPackageLicensePrototype-1.0.1/Implementation.py
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-02 09:18:33.174307 myPackageLicensePrototype-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-06-01 20:38:54.000000 myPackageLicensePrototype-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.1/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 09:18:33.173403 myPackageLicensePrototype-1.0.1/myPackageLicensePrototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-02 09:18:32.000000 myPackageLicensePrototype-1.0.1/myPackageLicensePrototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-02 09:18:33.000000 myPackageLicensePrototype-1.0.1/myPackageLicensePrototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 09:18:32.000000 myPackageLicensePrototype-1.0.1/myPackageLicensePrototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 09:18:32.000000 myPackageLicensePrototype-1.0.1/myPackageLicensePrototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      555 2023-06-01 20:50:12.000000 myPackageLicensePrototype-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 09:18:33.175579 myPackageLicensePrototype-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1035 2023-06-02 09:18:26.000000 myPackageLicensePrototype-1.0.1/setup.py
```

### Comparing `myPackageLicensePrototype-1.0.0/LICENSE` & `myPackageLicensePrototype-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.0/local_environment_installation_guide.txt` & `myPackageLicensePrototype-1.0.1/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.0/requirements.txt` & `myPackageLicensePrototype-1.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.0/setup.py` & `myPackageLicensePrototype-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='myPackageLicensePrototype',
-    version='1.0.0',
+    version='1.0.1',
     description='Description of your package',
     ppackage_data={'': ['src/*.py']}
 )
 
 
 # from setuptools import setup, find_packages
```

