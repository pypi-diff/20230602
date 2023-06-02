# Comparing `tmp/pyDictStore-1.0.0-1.tar.gz` & `tmp/pyDictStore-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDictStore-1.0.0.tar", last modified: Sat Aug  6 00:45:58 2022, max compression
+gzip compressed data, was "pyDictStore-1.0.1.tar", last modified: Fri Jun  2 19:34:49 2023, max compression
```

## Comparing `pyDictStore-1.0.0-1.tar` & `pyDictStore-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-06 00:45:58.190621 pyDictStore-1.0.0/
--rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4494 2022-08-06 00:45:58.189620 pyDictStore-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2022-08-06 00:45:58.191618 pyDictStore-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-06 00:45:58.157641 pyDictStore-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-06 00:45:58.166633 pyDictStore-1.0.0/src/pyDictStore/
--rw-rw-rw-   0        0        0     2780 2022-06-06 01:53:10.000000 pyDictStore-1.0.0/src/pyDictStore/__decorators__.py
--rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.0/src/pyDictStore/__events__.py
--rw-rw-rw-   0        0        0      545 2022-07-02 22:55:36.000000 pyDictStore-1.0.0/src/pyDictStore/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-06 00:45:58.187621 pyDictStore-1.0.0/src/pyDictStore.egg-info/
--rw-rw-rw-   0        0        0     4494 2022-08-06 00:45:57.000000 pyDictStore-1.0.0/src/pyDictStore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-08-06 00:45:57.000000 pyDictStore-1.0.0/src/pyDictStore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-06 00:45:57.000000 pyDictStore-1.0.0/src/pyDictStore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-08-06 00:45:57.000000 pyDictStore-1.0.0/src/pyDictStore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2157 2022-08-06 00:45:50.000000 pyDictStore-1.0.0/zsetup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.537985 pyDictStore-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2022-05-31 23:42:26.000000 pyDictStore-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4494 2023-06-02 19:34:49.537006 pyDictStore-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2022-08-06 00:15:10.000000 pyDictStore-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-02 19:34:49.538958 pyDictStore-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2158 2023-06-02 18:25:43.000000 pyDictStore-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.463784 pyDictStore-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.478429 pyDictStore-1.0.1/src/pyDictStore/
+-rw-rw-rw-   0        0        0     2780 2022-06-06 01:53:10.000000 pyDictStore-1.0.1/src/pyDictStore/__decorators__.py
+-rw-rw-rw-   0        0        0      974 2022-06-05 20:49:49.000000 pyDictStore-1.0.1/src/pyDictStore/__events__.py
+-rw-rw-rw-   0        0        0      545 2023-06-02 19:05:36.000000 pyDictStore-1.0.1/src/pyDictStore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 19:34:49.534081 pyDictStore-1.0.1/src/pyDictStore.egg-info/
+-rw-rw-rw-   0        0        0     4494 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 19:34:49.000000 pyDictStore-1.0.1/src/pyDictStore.egg-info/top_level.txt
```

### Comparing `pyDictStore-1.0.0/LICENSE` & `pyDictStore-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.0/PKG-INFO` & `pyDictStore-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.0
+Version: 1.0.1
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

### Comparing `pyDictStore-1.0.0/README.md` & `pyDictStore-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.0/src/pyDictStore/__decorators__.py` & `pyDictStore-1.0.1/src/pyDictStore/__decorators__.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.0/src/pyDictStore/__events__.py` & `pyDictStore-1.0.1/src/pyDictStore/__events__.py`

 * *Files identical despite different names*

### Comparing `pyDictStore-1.0.0/src/pyDictStore/__init__.py` & `pyDictStore-1.0.1/src/pyDictStore/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 .. include:: ../../README.md
 
 # Library functions
 '''
 
 __PROJECT__ = 'pyDictStore'
-__VERSION__ = '1.0.0'
+__VERSION__ = '1.0.1'
 
 from .__decorators__ import default, storageSetter, storage
 
 def isDefault(obj:object,prop:str) -> bool:
     '''
     Checks if an objects property is equal to its default value
     '''
```

### Comparing `pyDictStore-1.0.0/src/pyDictStore.egg-info/PKG-INFO` & `pyDictStore-1.0.1/src/pyDictStore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDictStore
-Version: 1.0.0
+Version: 1.0.1
 Summary: pyDictStore adds automated dictionary storage to properties eliminating the need for code bodies, property getters and setters. It also provides a property change event.
 Home-page: https://OpenWayside.org
 Author: Peter Varney, OpenWayside
 Author-email: pyDictStore@OpenWayside.org
 License: UNKNOWN
 Project-URL: Documentation, https://openwayside.org/rtm/pyDictStore/
 Project-URL: Source, https://github.com/OpenWayside/pyDictStore
```

### Comparing `pyDictStore-1.0.0/zsetup.py` & `pyDictStore-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 AUTHOR = 'Peter Varney, OpenWayside'
 AUTHOR_EMAIL = 'pyDictStore@OpenWayside.org'
 URL = 'https://OpenWayside.org'
 DESCRIPTION = "pyDictStore adds automated dictionary storage to properties" \
               " eliminating the need for code bodies, property getters and" \
               " setters. It also provides a property change event."
 
-def VERSION(project:str):
+def VERSION(project:str=PROJECT):
     init = join(dirname(__file__),'src',project,'__init__.py')
     if exists(init):
         with open(init, 'r', encoding="utf8") as f:
             return re.search(r"__VERSION__ = '(.*?)'"
                             , f.read()
                             ).group(1)
     return None
@@ -33,15 +33,15 @@
 if __name__ == '__main__':
     sys.argv.append('build')
     sys.argv.append('sdist')
     sys.argv.append('bdist_wheel')
     setup(
         install_requires=INSTALL_REQUIRES(),
         name=PROJECT,
-        version=VERSION(PROJECT),
+        version=VERSION(),
         author=AUTHOR,
         author_email=AUTHOR_EMAIL,
         description=DESCRIPTION,
         long_description=DESCRIPTION_LONG(),
         long_description_content_type="text/markdown",
         url=URL,
         project_urls={
```

