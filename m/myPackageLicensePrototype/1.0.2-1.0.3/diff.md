# Comparing `tmp/myPackageLicensePrototype-1.0.2.tar.gz` & `tmp/myPackageLicensePrototype-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myPackageLicensePrototype-1.0.2.tar", last modified: Fri Jun  2 09:23:52 2023, max compression
+gzip compressed data, was "myPackageLicensePrototype-1.0.3.tar", last modified: Fri Jun  2 10:02:23 2023, max compression
```

## Comparing `myPackageLicensePrototype-1.0.2.tar` & `myPackageLicensePrototype-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 09:23:52.702969 myPackageLicensePrototype-1.0.2/
--rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      133 2023-06-02 09:23:52.702969 myPackageLicensePrototype-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      110 2023-06-02 09:22:58.000000 myPackageLicensePrototype-1.0.2/PackageContent.py
--rw-rw-rw-   0        0        0       25 2023-06-01 20:38:54.000000 myPackageLicensePrototype-1.0.2/README.md
--rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.2/local_environment_installation_guide.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 09:23:52.701400 myPackageLicensePrototype-1.0.2/myPackageLicensePrototype.egg-info/
--rw-rw-rw-   0        0        0      133 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.2/myPackageLicensePrototype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.2/myPackageLicensePrototype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.2/myPackageLicensePrototype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.2/myPackageLicensePrototype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      555 2023-06-01 20:50:12.000000 myPackageLicensePrototype-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 09:23:52.703977 myPackageLicensePrototype-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1035 2023-06-02 09:23:42.000000 myPackageLicensePrototype-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:02:23.172165 myPackageLicensePrototype-1.0.3/
+-rw-rw-rw-   0        0        0      971 2023-06-02 09:58:42.000000 myPackageLicensePrototype-1.0.3/Implementation.ipynb
+-rw-rw-rw-   0        0        0     1085 2022-11-15 06:56:28.000000 myPackageLicensePrototype-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      133 2023-06-02 10:02:23.170672 myPackageLicensePrototype-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-06-02 09:58:42.000000 myPackageLicensePrototype-1.0.3/PackageContent.py
+-rw-rw-rw-   0        0        0      176 2023-06-02 09:27:14.000000 myPackageLicensePrototype-1.0.3/README.md
+-rw-rw-rw-   0        0        0        0 2023-06-02 09:18:16.000000 myPackageLicensePrototype-1.0.3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:02:23.123113 myPackageLicensePrototype-1.0.3/dist/
+-rw-rw-rw-   0        0        0     3154 2023-06-02 09:23:52.000000 myPackageLicensePrototype-1.0.3/dist/myPackageLicensePrototype-1.0.2.tar.gz
+-rw-rw-rw-   0        0        0     1503 2023-03-03 16:35:30.000000 myPackageLicensePrototype-1.0.3/local_environment_installation_guide.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 10:02:23.168666 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/
+-rw-rw-rw-   0        0        0      133 2023-06-02 10:02:22.000000 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      423 2023-06-02 10:02:22.000000 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:02:22.000000 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 10:02:22.000000 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-02 10:02:22.000000 myPackageLicensePrototype-1.0.3/myPackageLicensePrototype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       13 2023-06-02 09:59:14.000000 myPackageLicensePrototype-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:02:23.172165 myPackageLicensePrototype-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-06-02 10:02:20.000000 myPackageLicensePrototype-1.0.3/setup.py
```

### Comparing `myPackageLicensePrototype-1.0.2/LICENSE` & `myPackageLicensePrototype-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.2/local_environment_installation_guide.txt` & `myPackageLicensePrototype-1.0.3/local_environment_installation_guide.txt`

 * *Files identical despite different names*

### Comparing `myPackageLicensePrototype-1.0.2/setup.py` & `myPackageLicensePrototype-1.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 from setuptools import setup
 
+import codecs
+import chardet
+
+def get_encoding(file):
+    with open(file, 'rb') as f:
+        return chardet.detect(f.read())['encoding']
+
+encoding = get_encoding('requirements.txt')
+install_requires = codecs.open('requirements.txt', 'r', encoding=encoding).read().splitlines()
+ 
 setup(
     name='myPackageLicensePrototype',
-    version='1.0.2',
+    version='1.0.3',
     description='Description of your package',
+    install_requires=install_requires,
     ppackage_data={'': ['src/*.py']}
 )
 
 
 # from setuptools import setup, find_packages
 
 #from myPackageLicensePrototype import __version__
```

