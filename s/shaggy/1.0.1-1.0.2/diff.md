# Comparing `tmp/shaggy-1.0.1.tar.gz` & `tmp/shaggy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaggy-1.0.1.tar", last modified: Fri Jun  2 13:28:46 2023, max compression
+gzip compressed data, was "shaggy-1.0.2.tar", last modified: Fri Jun  2 16:55:46 2023, max compression
```

## Comparing `shaggy-1.0.1.tar` & `shaggy-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 13:28:46.896774 shaggy-1.0.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-05-31 11:30:02.000000 shaggy-1.0.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 13:28:46.896774 shaggy-1.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2264 2023-06-02 12:57:10.000000 shaggy-1.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-02 13:28:46.896774 shaggy-1.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      693 2023-06-02 13:07:02.000000 shaggy-1.0.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 13:28:46.896774 shaggy-1.0.1/shaggy.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 13:28:46.000000 shaggy-1.0.1/shaggy.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-06-02 13:28:46.000000 shaggy-1.0.1/shaggy.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 13:28:46.000000 shaggy-1.0.1/shaggy.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-06-02 13:28:46.000000 shaggy-1.0.1/shaggy.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 13:28:46.000000 shaggy-1.0.1/shaggy.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 16:55:46.317046 shaggy-1.0.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-05-31 11:30:02.000000 shaggy-1.0.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 16:55:46.317046 shaggy-1.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2264 2023-06-02 12:57:10.000000 shaggy-1.0.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-02 16:55:46.317046 shaggy-1.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      693 2023-06-02 16:55:31.000000 shaggy-1.0.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-02 16:55:46.313046 shaggy-1.0.2/shaggy.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2655 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       48 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-02 16:55:46.000000 shaggy-1.0.2/shaggy.egg-info/top_level.txt
```

### Comparing `shaggy-1.0.1/LICENSE` & `shaggy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.1/PKG-INFO` & `shaggy-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `shaggy-1.0.1/README.md` & `shaggy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `shaggy-1.0.1/setup.py` & `shaggy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='shaggy',
-    version='1.0.1',
+    version='1.0.2',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Mauro Baladés',
     author_email='mauro.balades@tutanota.com',
     description='Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.',
     url='https://github.com/mauro-balades/shaggy',
     packages=find_packages(),
```

### Comparing `shaggy-1.0.1/shaggy.egg-info/PKG-INFO` & `shaggy-1.0.2/shaggy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaggy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Discover and connect with social media accounts across multiple platforms using just a username with SocialTrackr, the ultimate account hunting software.
 Home-page: https://github.com/mauro-balades/shaggy
 Author: Mauro Baladés
 Author-email: mauro.balades@tutanota.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

