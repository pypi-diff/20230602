# Comparing `tmp/gpyutils-0.8.4.tar.gz` & `tmp/gpyutils-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpyutils-0.8.4.tar", last modified: Fri Feb  3 16:46:23 2023, max compression
+gzip compressed data, was "gpyutils-0.9.tar", last modified: Sun Apr  9 11:36:27 2023, max compression
```

## Comparing `gpyutils-0.8.4.tar` & `gpyutils-0.9.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1300 2020-12-11 08:04:49.749509 gpyutils-0.8.4/COPYING
--rw-r--r--   0        0        0     4114 2022-05-28 05:56:30.051290 gpyutils-0.8.4/README.rst
--rw-r--r--   0        0        0       76 2023-02-03 16:44:31.441133 gpyutils-0.8.4/gpyutils/__init__.py
--rw-r--r--   0        0        0      382 2021-05-23 08:57:58.057850 gpyutils-0.8.4/gpyutils/ansi.py
--rw-r--r--   0        0        0      436 2022-05-16 17:25:01.563997 gpyutils-0.8.4/gpyutils/eclasses.py
--rw-r--r--   0        0        0     2858 2022-05-16 17:43:00.223567 gpyutils-0.8.4/gpyutils/implementations.py
--rw-r--r--   0        0        0     1924 2022-05-16 17:41:24.168198 gpyutils-0.8.4/gpyutils/packages.py
--rw-r--r--   0        0        0    15140 2022-05-16 17:46:21.221159 gpyutils-0.8.4/gpyutils/pycompat.py
--rw-r--r--   0        0        0        0 2022-05-16 18:00:30.395843 gpyutils-0.8.4/gpyutils/scripts/__init__.py
--rwxr-xr-x   0        0        0     7525 2022-05-16 18:11:25.099721 gpyutils-0.8.4/gpyutils/scripts/depgraph.py
--rwxr-xr-x   0        0        0     3414 2022-05-16 18:24:53.876841 gpyutils-0.8.4/gpyutils/scripts/drop_dead_impls.py
--rwxr-xr-x   0        0        0     1349 2022-05-16 18:23:30.158414 gpyutils-0.8.4/gpyutils/scripts/impl.py
--rwxr-xr-x   0        0        0     2853 2023-02-01 19:32:54.801134 gpyutils-0.8.4/gpyutils/scripts/list_pkg_impls.py
--rwxr-xr-x   0        0        0     3515 2022-05-16 18:28:10.087639 gpyutils-0.8.4/gpyutils/scripts/showimpls.py
--rwxr-xr-x   0        0        0     8746 2022-05-16 18:28:47.471761 gpyutils-0.8.4/gpyutils/scripts/upgrade_impl.py
--rwxr-xr-x   0        0        0     8644 2023-02-03 16:42:14.923435 gpyutils-0.8.4/gpyutils/scripts/verify_deps.py
--rw-r--r--   0        0        0     1389 2022-05-27 18:04:24.921863 gpyutils-0.8.4/pyproject.toml
--rw-r--r--   0        0        0      542 2022-05-17 06:45:37.537598 gpyutils-0.8.4/tox.ini
--rw-r--r--   0        0        0     4947 1970-01-01 00:00:00.000000 gpyutils-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1300 2020-12-11 08:04:49.749509 gpyutils-0.9/COPYING
+-rw-r--r--   0        0        0     4114 2022-05-28 05:56:30.051290 gpyutils-0.9/README.rst
+-rw-r--r--   0        0        0       74 2023-04-09 11:33:40.508231 gpyutils-0.9/gpyutils/__init__.py
+-rw-r--r--   0        0        0      382 2021-05-23 08:57:58.057850 gpyutils-0.9/gpyutils/ansi.py
+-rw-r--r--   0        0        0      436 2022-05-16 17:25:01.563997 gpyutils-0.9/gpyutils/eclasses.py
+-rw-r--r--   0        0        0     2858 2022-05-16 17:43:00.223567 gpyutils-0.9/gpyutils/implementations.py
+-rw-r--r--   0        0        0     1924 2022-05-16 17:41:24.168198 gpyutils-0.9/gpyutils/packages.py
+-rw-r--r--   0        0        0    15138 2023-04-09 11:27:51.944059 gpyutils-0.9/gpyutils/pycompat.py
+-rw-r--r--   0        0        0        0 2022-05-16 18:00:30.395843 gpyutils-0.9/gpyutils/scripts/__init__.py
+-rwxr-xr-x   0        0        0     7525 2022-05-16 18:11:25.099721 gpyutils-0.9/gpyutils/scripts/depgraph.py
+-rwxr-xr-x   0        0        0     3413 2023-04-09 11:28:08.577772 gpyutils-0.9/gpyutils/scripts/drop_dead_impls.py
+-rwxr-xr-x   0        0        0     1349 2022-05-16 18:23:30.158414 gpyutils-0.9/gpyutils/scripts/impl.py
+-rwxr-xr-x   0        0        0     2853 2023-02-01 19:32:54.801134 gpyutils-0.9/gpyutils/scripts/list_pkg_impls.py
+-rwxr-xr-x   0        0        0     1052 2023-03-16 17:56:03.082075 gpyutils-0.9/gpyutils/scripts/pkgs_with_newest_stable.py
+-rwxr-xr-x   0        0        0     3682 2023-04-09 11:33:02.187410 gpyutils-0.9/gpyutils/scripts/release_feed_opml.py
+-rwxr-xr-x   0        0        0     3515 2022-05-16 18:28:10.087639 gpyutils-0.9/gpyutils/scripts/showimpls.py
+-rwxr-xr-x   0        0        0     4543 2023-04-09 11:28:48.841988 gpyutils-0.9/gpyutils/scripts/to_pypi_eclass.py
+-rwxr-xr-x   0        0        0     8746 2022-05-16 18:28:47.471761 gpyutils-0.9/gpyutils/scripts/upgrade_impl.py
+-rwxr-xr-x   0        0        0     8629 2023-04-09 11:29:24.596078 gpyutils-0.9/gpyutils/scripts/verify_deps.py
+-rw-r--r--   0        0        0     1679 2023-04-09 11:26:51.582537 gpyutils-0.9/pyproject.toml
+-rw-r--r--   0        0        0      548 2023-04-09 11:25:24.014254 gpyutils-0.9/tox.ini
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 gpyutils-0.9/PKG-INFO
```

### Comparing `gpyutils-0.8.4/COPYING` & `gpyutils-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/README.rst` & `gpyutils-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/implementations.py` & `gpyutils-0.9/gpyutils/implementations.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/packages.py` & `gpyutils-0.9/gpyutils/packages.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/pycompat.py` & `gpyutils-0.9/gpyutils/pycompat.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return 'Value(full_name=%s, local_name=%s, removed=%s)' % (
             self.full_name,
             self.local_name,
             self.removed,
         )
 
     def __str__(self):
-        assert(not self.removed)
+        assert not self.removed
         return self.local_name
 
 
 def get_previous_val_index(values, v):
     """
     Return index of value in list values that lexically precedes v,
     or -1 if no value precedes it.
@@ -106,15 +106,15 @@
 
 
 range_re = re.compile(r'^(\d+)\.\.(\d+)$')
 
 
 class Range(Group):
     def __init__(self, f_prefix, l_prefix, values):
-        assert(len(values) == 1)
+        assert len(values) == 1
         m = range_re.match(values[0].local_name)
         if m is None:
             raise ValueError("Invalid range: %s" % values[0].local_name)
         Group.__init__(self, f_prefix, l_prefix,
                        [Value(''.join((f_prefix, str(x))), str(x))
                         for x in range(int(m.group(1)), int(m.group(2))+1)])
```

### Comparing `gpyutils-0.8.4/gpyutils/scripts/depgraph.py` & `gpyutils-0.9/gpyutils/scripts/depgraph.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/scripts/drop_dead_impls.py` & `gpyutils-0.9/gpyutils/scripts/drop_dead_impls.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 continue
 
             print(p)
             try:
                 impls = get_python_impls(p, need_dead=True)
             except (gentoopm.exceptions.InvalidBashCodeError, OSError):
                 continue
-            assert(impls is not None)
+            assert impls is not None
 
             found_one = True
 
             if any([i in impls for i in dead_impls]):
                 found_upd = True
 
                 if fix:
```

### Comparing `gpyutils-0.8.4/gpyutils/scripts/impl.py` & `gpyutils-0.9/gpyutils/scripts/impl.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/scripts/list_pkg_impls.py` & `gpyutils-0.9/gpyutils/scripts/list_pkg_impls.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/scripts/showimpls.py` & `gpyutils-0.9/gpyutils/scripts/showimpls.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/scripts/upgrade_impl.py` & `gpyutils-0.9/gpyutils/scripts/upgrade_impl.py`

 * *Files identical despite different names*

### Comparing `gpyutils-0.8.4/gpyutils/scripts/verify_deps.py` & `gpyutils-0.9/gpyutils/scripts/verify_deps.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 # Released under the terms of the 2-clause BSD license.
 
 from gentoopm import get_package_manager
 from gentoopm.basepm.atom import PMAtom
 
 from gpyutils.ansi import ANSI
 
-import argparse
 import collections
 import importlib.metadata
 import itertools
 import json
 import os.path
 import subprocess
 import sys
@@ -153,14 +152,15 @@
             matched_pkg = dist_name_map[dep_name].get(pyver, None)
             if matched_pkg is None:
                 missing_dists[dist.name][dep_name].add(pyver)
                 continue
             expected_deps.add(str(matched_pkg.key))
 
         expected_usedeps = set(expected_deps)
+
         def process_deps(dep):
             if not isinstance(dep, PMAtom):
                 for x in dep:
                     process_deps(x)
             else:
                 _, _, usedep = str(dep).partition("[")
                 flags = usedep.rstrip("]").split(",")
```

### Comparing `gpyutils-0.8.4/pyproject.toml` & `gpyutils-0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -22,27 +22,35 @@
     "Topic :: System :: Installation/Setup",
 ]
 
 [project.optional-dependencies]
 depgraph-nx = [
     "networkx",
 ]
+release-feed-opml = [
+    "lxml",
+]
 test = [
+    "lxml",
+    "packaging",
     "pytest",
 ]
 verify-deps = [
     "packaging",
 ]
 
 [project.scripts]
 gpy-depgraph = "gpyutils.scripts.depgraph:entry_point"
 gpy-drop-dead-impls = "gpyutils.scripts.drop_dead_impls:entry_point"
 gpy-impl = "gpyutils.scripts.impl:entry_point"
 gpy-list-pkg-impls = "gpyutils.scripts.list_pkg_impls:entry_point"
+gpy-pkgs-with-newest-stable = "gpyutils.scripts.pkgs_with_newest_stable:entry_point"
+gpy-release-feed-opml = "gpyutils.scripts.release_feed_opml:entry_point"
 gpy-showimpls = "gpyutils.scripts.showimpls:entry_point"
+gpy-to-pypi-eclass = "gpyutils.scripts.to_pypi_eclass:entry_point"
 gpy-upgrade-impl = "gpyutils.scripts.upgrade_impl:entry_point"
 gpy-verify-deps = "gpyutils.scripts.verify_deps:entry_point"
 
 [project.urls]
 Homepage = "https://github.com/mgorny/gpyutils/"
 
 [tool.flit.sdist]
```

### Comparing `gpyutils-0.8.4/tox.ini` & `gpyutils-0.9/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = qa,py38,py39,py310
+envlist = qa,py38,py39,py310,py311
 isolated_build = True
 skip_missing_interpreters = True
 
 [testenv]
 deps =
 # (currently tests do not use any gentoopm bits)
 #	pkgcore
```

### Comparing `gpyutils-0.8.4/PKG-INFO` & `gpyutils-0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: gpyutils
-Version: 0.8.4
+Version: 0.9
 Summary: Maintenance scripts for Gentoo Python packages
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Topic :: System :: Installation/Setup
 Requires-Dist: gentoopm
 Requires-Dist: networkx ; extra == "depgraph-nx"
+Requires-Dist: lxml ; extra == "release-feed-opml"
+Requires-Dist: lxml ; extra == "test"
+Requires-Dist: packaging ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: packaging ; extra == "verify-deps"
 Project-URL: Homepage, https://github.com/mgorny/gpyutils/
 Provides-Extra: depgraph-nx
+Provides-Extra: release-feed-opml
 Provides-Extra: test
 Provides-Extra: verify-deps
 
 ========
 gpyutils
 ========
```

