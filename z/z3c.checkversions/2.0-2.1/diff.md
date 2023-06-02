# Comparing `tmp/z3c.checkversions-2.0.tar.gz` & `tmp/z3c.checkversions-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.checkversions-2.0.tar", last modified: Tue Feb 14 08:00:29 2023, max compression
+gzip compressed data, was "z3c.checkversions-2.1.tar", last modified: Fri Jun  2 14:31:53 2023, max compression
```

## Comparing `z3c.checkversions-2.0.tar` & `z3c.checkversions-2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.646124 z3c.checkversions-2.0/
--rw-r--r--   0 mac        (513) staff       (20)     2286 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/COPYRIGHT.rst
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/LICENSE.rst
--rw-r--r--   0 mac        (513) staff       (20)      273 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     7288 2023-02-14 08:00:29.646302 z3c.checkversions-2.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     3651 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      208 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/TODO.rst
--rw-r--r--   0 mac        (513) staff       (20)      423 2023-02-14 08:00:29.646995 z3c.checkversions-2.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2549 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.631148 z3c.checkversions-2.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.637619 z3c.checkversions-2.0/src/z3c/
--rw-r--r--   0 mac        (513) staff       (20)       75 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.644379 z3c.checkversions-2.0/src/z3c/checkversions/
--rw-r--r--   0 mac        (513) staff       (20)      213 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/README.txt
--rw-r--r--   0 mac        (513) staff       (20)        0 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     5174 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/base.py
--rw-r--r--   0 mac        (513) staff       (20)     1661 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/buildout.py
--rw-r--r--   0 mac        (513) staff       (20)     5200 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/buildout.txt
--rw-r--r--   0 mac        (513) staff       (20)     1002 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/installed.py
--rw-r--r--   0 mac        (513) staff       (20)      364 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/installed.txt
--rw-r--r--   0 mac        (513) staff       (20)     3238 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/main.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.632066 z3c.checkversions-2.0/src/z3c/checkversions/testindex/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.644772 z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.component/
--rw-r--r--   0 mac        (513) staff       (20)     2699 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.component/index.html
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.645109 z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.interface/
--rw-r--r--   0 mac        (513) staff       (20)     1955 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.interface/index.html
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.632696 z3c.checkversions-2.0/src/z3c/checkversions/testindex2/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.645459 z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.component/
--rw-r--r--   0 mac        (513) staff       (20)     2585 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.component/index.html
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.645833 z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.interface/
--rw-r--r--   0 mac        (513) staff       (20)     2068 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.interface/index.html
--rw-r--r--   0 mac        (513) staff       (20)     1718 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/src/z3c/checkversions/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-02-14 08:00:29.640926 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     7288 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1034 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)       62 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/entry_points.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       63 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2023-02-14 08:00:29.000000 z3c.checkversions-2.0/src/z3c.checkversions.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1470 2023-02-14 08:00:28.000000 z3c.checkversions-2.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.486253 z3c.checkversions-2.1/
+-rw-r--r--   0 jens       (501) staff       (20)     2469 2023-06-02 14:29:48.000000 z3c.checkversions-2.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/COPYRIGHT.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/LICENSE.rst
+-rw-r--r--   0 jens       (501) staff       (20)      273 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)     7471 2023-06-02 14:31:53.486312 z3c.checkversions-2.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3651 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      208 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/TODO.rst
+-rw-r--r--   0 jens       (501) staff       (20)      423 2023-06-02 14:31:53.486543 z3c.checkversions-2.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2543 2023-06-02 14:29:59.000000 z3c.checkversions-2.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.480938 z3c.checkversions-2.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.483303 z3c.checkversions-2.1/src/z3c/
+-rw-r--r--   0 jens       (501) staff       (20)       75 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.485563 z3c.checkversions-2.1/src/z3c/checkversions/
+-rw-r--r--   0 jens       (501) staff       (20)      213 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)        0 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     5558 2023-05-25 07:32:42.000000 z3c.checkversions-2.1/src/z3c/checkversions/base.py
+-rw-r--r--   0 jens       (501) staff       (20)     1661 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/buildout.py
+-rw-r--r--   0 jens       (501) staff       (20)     5200 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/buildout.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1002 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/installed.py
+-rw-r--r--   0 jens       (501) staff       (20)      364 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/installed.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3238 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/main.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.481301 z3c.checkversions-2.1/src/z3c/checkversions/testindex/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.485702 z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.component/
+-rw-r--r--   0 jens       (501) staff       (20)     2699 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.component/index.html
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.485858 z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.interface/
+-rw-r--r--   0 jens       (501) staff       (20)     1955 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.interface/index.html
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.481531 z3c.checkversions-2.1/src/z3c/checkversions/testindex2/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.485991 z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.component/
+-rw-r--r--   0 jens       (501) staff       (20)     2585 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.component/index.html
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.486117 z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.interface/
+-rw-r--r--   0 jens       (501) staff       (20)     2068 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.interface/index.html
+-rw-r--r--   0 jens       (501) staff       (20)     1718 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/src/z3c/checkversions/tests.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-06-02 14:31:53.484382 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)     7471 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1034 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       62 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        4 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-05-25 05:28:07.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)       59 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        4 2023-06-02 14:31:53.000000 z3c.checkversions-2.1/src/z3c.checkversions.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1470 2023-05-25 05:27:24.000000 z3c.checkversions-2.1/tox.ini
```

### Comparing `z3c.checkversions-2.0/CHANGES.rst` & `z3c.checkversions-2.1/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.1 (2023-02-06)
+----------------
+
+- Fix parsing of versions that are really requirements specifications.
+  (`#24 <https://github.com/zopefoundation/z3c.checkversions/issues/24>`_)
+
+
 2.0 (2023-02-14)
 ----------------
 
 - Add support for Python 3.10, 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.checkversions-2.0/CONTRIBUTING.md` & `z3c.checkversions-2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/LICENSE.rst` & `z3c.checkversions-2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/PKG-INFO` & `z3c.checkversions-2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.checkversions
-Version: 2.0
+Version: 2.1
 Summary: Find newer package versions on PyPI
 Home-page: https://github.com/zopefoundation/z3c.checkversions
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: version,buildout,packages,upgrade,zope,ztk
 Classifier: Development Status :: 5 - Production/Stable
@@ -164,14 +164,21 @@
     $ virtualenv .
     $ bin/pip install tox
     $ tox
 
 Changelog
 =========
 
+2.1 (2023-02-06)
+----------------
+
+- Fix parsing of versions that are really requirements specifications.
+  (`#24 <https://github.com/zopefoundation/z3c.checkversions/issues/24>`_)
+
+
 2.0 (2023-02-14)
 ----------------
 
 - Add support for Python 3.10, 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.checkversions-2.0/README.rst` & `z3c.checkversions-2.1/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/setup.py` & `z3c.checkversions-2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='z3c.checkversions',
-    version='2.0',
+    version='2.1',
     description="Find newer package versions on PyPI",
     long_description=(open("README.rst").read() + "\n" +
                       open("CHANGES.rst").read()),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
@@ -50,15 +50,15 @@
     license='ZPL 2.1',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['z3c'],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        'setuptools >= 8, < 66',
+        'setuptools >= 8',
     ],
     python_requires='>=3.7',
     extras_require={
         'buildout': ['zc.buildout'],
         'test': ['zope.testing'],
     },
     entry_points="""
```

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/base.py` & `z3c.checkversions-2.1/src/z3c/checkversions/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,25 @@
         versions = self.get_versions()
 
         for name, version in sorted(versions.items()):
             if self.incremental == 'stop':
                 # skip subsequent scans
                 print("{}={}".format(name, version))
                 continue
-            parsed_version = parse_version(version)
+
+            try:
+                parsed_version = parse_version(version)
+            except ValueError:
+                # This could be a requirements specification instead
+                # of a straight version number
+                req = Requirement(f'{name}{version}')
+                for spec in req.specifier:
+                    parsed_version = parse_version(spec.version)
+                    break  # Just use the first one
+
             req = Requirement.parse(name)
             self.pi.find_packages(req)
             new_dist = None
             # loop all index versions until we find the 1st newer version
             # that keeps the major versions (below level)
             # and is a final version
             # and is not in the blacklist
```

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/buildout.py` & `z3c.checkversions-2.1/src/z3c/checkversions/buildout.py`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/buildout.txt` & `z3c.checkversions-2.1/src/z3c/checkversions/buildout.txt`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/installed.py` & `z3c.checkversions-2.1/src/z3c/checkversions/installed.py`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/main.py` & `z3c.checkversions-2.1/src/z3c/checkversions/main.py`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.component/index.html` & `z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.component/index.html`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/testindex/zope.interface/index.html` & `z3c.checkversions-2.1/src/z3c/checkversions/testindex/zope.interface/index.html`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.component/index.html` & `z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.component/index.html`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/testindex2/zope.interface/index.html` & `z3c.checkversions-2.1/src/z3c/checkversions/testindex2/zope.interface/index.html`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c/checkversions/tests.py` & `z3c.checkversions-2.1/src/z3c/checkversions/tests.py`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/src/z3c.checkversions.egg-info/PKG-INFO` & `z3c.checkversions-2.1/src/z3c.checkversions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.checkversions
-Version: 2.0
+Version: 2.1
 Summary: Find newer package versions on PyPI
 Home-page: https://github.com/zopefoundation/z3c.checkversions
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: version,buildout,packages,upgrade,zope,ztk
 Classifier: Development Status :: 5 - Production/Stable
@@ -164,14 +164,21 @@
     $ virtualenv .
     $ bin/pip install tox
     $ tox
 
 Changelog
 =========
 
+2.1 (2023-02-06)
+----------------
+
+- Fix parsing of versions that are really requirements specifications.
+  (`#24 <https://github.com/zopefoundation/z3c.checkversions/issues/24>`_)
+
+
 2.0 (2023-02-14)
 ----------------
 
 - Add support for Python 3.10, 3.11.
 
 - Drop support for Python 2.7, 3.5, 3.6.
```

### Comparing `z3c.checkversions-2.0/src/z3c.checkversions.egg-info/SOURCES.txt` & `z3c.checkversions-2.1/src/z3c.checkversions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.checkversions-2.0/tox.ini` & `z3c.checkversions-2.1/tox.ini`

 * *Files identical despite different names*

