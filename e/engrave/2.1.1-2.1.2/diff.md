# Comparing `tmp/engrave-2.1.1.tar.gz` & `tmp/engrave-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engrave-2.1.1.tar", last modified: Fri Jan 27 07:04:35 2023, max compression
+gzip compressed data, was "engrave-2.1.2.tar", last modified: Fri Jun  2 16:19:26 2023, max compression
```

## Comparing `engrave-2.1.1.tar` & `engrave-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-01-27 07:04:35.018747 engrave-2.1.1/
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)     1071 2023-01-24 13:45:30.000000 engrave-2.1.1/LICENSE
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)     2396 2023-01-27 07:04:35.018747 engrave-2.1.1/PKG-INFO
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)      994 2023-01-27 07:04:12.000000 engrave-2.1.1/README.md
-drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-01-27 07:04:35.017747 engrave-2.1.1/bin/
--rwxr-xr-x   0 nitipit   (1000) nitipit   (1000)       83 2023-01-25 06:52:00.000000 engrave-2.1.1/bin/engrave
-drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-01-27 07:04:35.017747 engrave-2.1.1/engrave/
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)     7974 2023-01-27 07:04:12.000000 engrave-2.1.1/engrave/__init__.py
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)       61 2023-01-25 06:52:05.000000 engrave-2.1.1/engrave/__main__.py
-drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-01-27 07:04:35.018747 engrave-2.1.1/engrave.egg-info/
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)     2396 2023-01-27 07:04:35.000000 engrave-2.1.1/engrave.egg-info/PKG-INFO
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)      257 2023-01-27 07:04:35.000000 engrave-2.1.1/engrave.egg-info/SOURCES.txt
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)        1 2023-01-27 07:04:35.000000 engrave-2.1.1/engrave.egg-info/dependency_links.txt
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)       70 2023-01-27 07:04:35.000000 engrave-2.1.1/engrave.egg-info/requires.txt
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)        8 2023-01-27 07:04:35.000000 engrave-2.1.1/engrave.egg-info/top_level.txt
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)      103 2023-01-24 02:16:44.000000 engrave-2.1.1/pyproject.toml
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)      588 2023-01-27 07:04:35.018747 engrave-2.1.1/setup.cfg
--rw-r--r--   0 nitipit   (1000) nitipit   (1000)       37 2023-01-24 02:16:44.000000 engrave-2.1.1/setup.py
+drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-06-02 16:19:26.845620 engrave-2.1.2/
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)     1071 2023-06-02 14:06:35.000000 engrave-2.1.2/LICENSE
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)     2396 2023-06-02 16:19:26.845620 engrave-2.1.2/PKG-INFO
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)      994 2023-06-02 14:06:35.000000 engrave-2.1.2/README.md
+drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-06-02 16:19:26.844620 engrave-2.1.2/bin/
+-rwxr-xr-x   0 nitipit   (1000) nitipit   (1000)       83 2023-06-02 14:06:35.000000 engrave-2.1.2/bin/engrave
+drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-06-02 16:19:26.844620 engrave-2.1.2/engrave/
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)     8007 2023-06-02 14:32:32.000000 engrave-2.1.2/engrave/__init__.py
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)       61 2023-06-02 14:06:35.000000 engrave-2.1.2/engrave/__main__.py
+drwxr-xr-x   0 nitipit   (1000) nitipit   (1000)        0 2023-06-02 16:19:26.845620 engrave-2.1.2/engrave.egg-info/
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)     2396 2023-06-02 16:19:26.000000 engrave-2.1.2/engrave.egg-info/PKG-INFO
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)      248 2023-06-02 16:19:26.000000 engrave-2.1.2/engrave.egg-info/SOURCES.txt
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)        1 2023-06-02 16:19:26.000000 engrave-2.1.2/engrave.egg-info/dependency_links.txt
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)       70 2023-06-02 16:19:26.000000 engrave-2.1.2/engrave.egg-info/requires.txt
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)        8 2023-06-02 16:19:26.000000 engrave-2.1.2/engrave.egg-info/top_level.txt
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)      103 2023-06-02 14:06:35.000000 engrave-2.1.2/pyproject.toml
+-rw-r--r--   0 nitipit   (1000) nitipit   (1000)      588 2023-06-02 16:19:26.846620 engrave-2.1.2/setup.cfg
```

### Comparing `engrave-2.1.1/LICENSE` & `engrave-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `engrave-2.1.1/PKG-INFO` & `engrave-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engrave
-Version: 2.1.1
+Version: 2.1.2
 Summary: Engrave is a static website framework
 License: MIT
 Keywords: static web framework
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `engrave-2.1.1/README.md` & `engrave-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `engrave-2.1.1/engrave/__init__.py` & `engrave-2.1.2/engrave/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,16 +200,16 @@
 
     def _add_asset_option(self, parser):
         parser.add_argument(
             '--asset',
             nargs='?',
             const='.*.('+\
                 'apng|avif|gif|jpg|png|svg|webp|ttf|otf|woff|woff2|eot|' +\
-                'mp4|webm|3gp|ogg'
-            ')',
+                'mp4|webm|3gp|ogg)' +\
+                '|sitemap*.xml$|robot*.txt$',
             metavar='RegExp',
             default=None,
             help="Regular expression string to match asset files",        
         )
 
     def make_build_parser(self):
         parser = self.sub_parser.add_parser('build', help='Build html')
```

### Comparing `engrave-2.1.1/engrave.egg-info/PKG-INFO` & `engrave-2.1.2/engrave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: engrave
-Version: 2.1.1
+Version: 2.1.2
 Summary: Engrave is a static website framework
 License: MIT
 Keywords: static web framework
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `engrave-2.1.1/setup.cfg` & `engrave-2.1.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = engrave
-version = 2.1.1
+version = 2.1.2
 description = Engrave is a static website framework
 long_description = file: README.md, CHANGELOG.md, LICENSE
 long_description_content_type = text/markdown
 keywords = static web framework
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

