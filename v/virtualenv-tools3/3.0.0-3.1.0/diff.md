# Comparing `tmp/virtualenv_tools3-3.0.0.tar.gz` & `tmp/virtualenv_tools3-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virtualenv_tools3-3.0.0.tar", last modified: Tue May 23 00:31:13 2023, max compression
+gzip compressed data, was "virtualenv_tools3-3.1.0.tar", last modified: Fri Jun  2 02:51:49 2023, max compression
```

## Comparing `virtualenv_tools3-3.0.0.tar` & `virtualenv_tools3-3.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/
--rw-r--r--   0 ckuehl    (3119) users      (100)     1499 2017-07-22 21:16:14.000000 virtualenv_tools3-3.0.0/LICENSE
--rw-r--r--   0 ckuehl    (3119) users      (100)     3602 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/PKG-INFO
--rw-r--r--   0 ckuehl    (3119) users      (100)     2921 2017-10-19 21:09:54.000000 virtualenv_tools3-3.0.0/README.md
--rw-r--r--   0 ckuehl    (3119) users      (100)     1136 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/setup.cfg
--rw-r--r--   0 ckuehl    (3119) users      (100)       37 2023-05-23 00:30:18.000000 virtualenv_tools3-3.0.0/setup.py
--rw-r--r--   0 ckuehl    (3119) users      (100)    10527 2023-05-23 00:30:18.000000 virtualenv_tools3-3.0.0/virtualenv_tools.py
-drwxr-xr-x   0 ckuehl    (3119) users      (100)        0 2023-05-23 00:31:13.194668 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/
--rw-r--r--   0 ckuehl    (3119) users      (100)     3602 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/PKG-INFO
--rw-r--r--   0 ckuehl    (3119) users      (100)      264 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/SOURCES.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)        1 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/dependency_links.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       60 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/entry_points.txt
--rw-r--r--   0 ckuehl    (3119) users      (100)       17 2023-05-23 00:31:13.000000 virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/top_level.txt
+drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2023-06-02 02:51:49.190007 virtualenv_tools3-3.1.0/
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     1499 2023-06-02 02:51:19.000000 virtualenv_tools3-3.1.0/LICENSE
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     4327 2023-06-02 02:51:49.190007 virtualenv_tools3-3.1.0/PKG-INFO
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     2921 2023-06-02 02:51:19.000000 virtualenv_tools3-3.1.0/README.md
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     1136 2023-06-02 02:51:49.190007 virtualenv_tools3-3.1.0/setup.cfg
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       37 2023-06-02 02:51:19.000000 virtualenv_tools3-3.1.0/setup.py
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)    11141 2023-06-02 02:51:19.000000 virtualenv_tools3-3.1.0/virtualenv_tools.py
+drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2023-06-02 02:51:49.190007 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     4327 2023-06-02 02:51:49.000000 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/PKG-INFO
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      264 2023-06-02 02:51:49.000000 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)        1 2023-06-02 02:51:49.000000 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       60 2023-06-02 02:51:49.000000 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/entry_points.txt
+-rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       17 2023-06-02 02:51:49.000000 virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/top_level.txt
```

### Comparing `virtualenv_tools3-3.0.0/LICENSE` & `virtualenv_tools3-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualenv_tools3-3.0.0/PKG-INFO` & `virtualenv_tools3-3.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,110 @@
 Metadata-Version: 2.1
 Name: virtualenv_tools3
-Version: 3.0.0
+Version: 3.1.0
 Summary: A set of tools for virtualenv
 Home-page: http://github.com/Yelp/virtualenv-tools
 Author: Fireteam Ltd.; Yelp, Inc.
 Author-email: opensource@yelp.com
 License: UNKNOWN
+Description: [![Build Status](https://travis-ci.org/Yelp/virtualenv-tools.svg?branch=master)](https://travis-ci.org/Yelp/virtualenv-tools)
+        [![Coverage Status](https://img.shields.io/coveralls/Yelp/virtualenv-tools.svg?branch=master)](https://coveralls.io/r/Yelp/virtualenv-tools)
+        [![PyPI version](https://badge.fury.io/py/virtualenv-tools3.svg)](https://pypi.python.org/pypi/virtualenv-tools3)
+        
+        virtualenv-tools3
+        --------
+        
+        virtualenv-tools3 is a fork of [the original
+        virtualenv-tools](https://github.com/fireteam/virtualenv-tools) (now
+        unmaintained) which adds support for Python 3, among other things. Full patch
+        details are below.
+        
+        ##  yelp patches
+        
+        ### yelp4
+        
+        * Add python3 support
+        * Drop python2.6 support
+        * 100% test coverage
+        * Removes `$VENV/local` instead of fixing up symlinks
+        * Removed `--reinitialize`, instead run `virtualenv $VENV -p $PYTHON`
+        * Rewrite .pth files to relative paths
+        
+        
+        ### yelp3
+        
+        * default output much more concise, added a --verbose option
+        * improved fault tolerance, in the case of:
+            * corrupt pyc files
+            * broken symlinks
+            * unexpected directories
+        * no-changes-needed is a success case (idempotency exits 0)
+        
+        
+        ### yelp1
+        
+        * --update now works more generally and reliably (e.g. virtualenv --python=python2.7)
+        
+        
+        ## virtualenv-tools
+        
+        This repository contains scripts we're using at Fireteam for our
+        deployment of Python code.  We're using them in combination with
+        salt to build code on one server on a self contained virtualenv
+        and then move that over to the destination servers to run.
+        
+        ### Why not virtualenv --relocatable?
+        
+        For starters: because it does not work.  relocatable is very
+        limited in what it does and it works at runtime instead of
+        making the whole thing actually move to the new location.  We
+        ran into a ton of issues with it and it is currently in the
+        process of being phased out.
+        
+        ### Why would I want to use it?
+        
+        The main reason you want to use this is for build caching.  You
+        have one folder where one virtualenv exists, you install the
+        latest version of your codebase and all extensions in there, then
+        you can make the virtualenv relocate to a target location, put it
+        into a tarball, distribute it to all servers and done!
+        
+        ### Example flow:
+        
+        First time: create the build cache
+        
+        ```
+        $ mkdir /tmp/build-cache
+        $ virtualenv --distribute /tmp/build-cache
+        ```
+        
+        Now every time you build:
+        
+        ```
+        $ . /tmp/build-cache/bin/activate
+        $ pip install YourApplication
+        ```
+        
+        Build done, package up and copy to whatever location you want to have it.
+        
+        Once unpacked on the target server, use the virtualenv tools to
+        update the paths and make the virtualenv magically work in the new
+        location.  For instance we deploy things to a path with the
+        hash of the commit in:
+        
+        ```
+        $ virtualenv-tools --update-path /srv/your-application/<hash>
+        ```
+        
+        Compile once, deploy whereever.  Virtualenvs are completely self
+        contained.  In order to switch the current version all you need to
+        do is to relink the builds.
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/Yelp/virtualenv-tools.svg?branch=master)](https://travis-ci.org/Yelp/virtualenv-tools)
-[![Coverage Status](https://img.shields.io/coveralls/Yelp/virtualenv-tools.svg?branch=master)](https://coveralls.io/r/Yelp/virtualenv-tools)
-[![PyPI version](https://badge.fury.io/py/virtualenv-tools3.svg)](https://pypi.python.org/pypi/virtualenv-tools3)
-
-virtualenv-tools3
---------
-
-virtualenv-tools3 is a fork of [the original
-virtualenv-tools](https://github.com/fireteam/virtualenv-tools) (now
-unmaintained) which adds support for Python 3, among other things. Full patch
-details are below.
-
-##  yelp patches
-
-### yelp4
-
-* Add python3 support
-* Drop python2.6 support
-* 100% test coverage
-* Removes `$VENV/local` instead of fixing up symlinks
-* Removed `--reinitialize`, instead run `virtualenv $VENV -p $PYTHON`
-* Rewrite .pth files to relative paths
-
-
-### yelp3
-
-* default output much more concise, added a --verbose option
-* improved fault tolerance, in the case of:
-    * corrupt pyc files
-    * broken symlinks
-    * unexpected directories
-* no-changes-needed is a success case (idempotency exits 0)
-
-
-### yelp1
-
-* --update now works more generally and reliably (e.g. virtualenv --python=python2.7)
-
-
-## virtualenv-tools
-
-This repository contains scripts we're using at Fireteam for our
-deployment of Python code.  We're using them in combination with
-salt to build code on one server on a self contained virtualenv
-and then move that over to the destination servers to run.
-
-### Why not virtualenv --relocatable?
-
-For starters: because it does not work.  relocatable is very
-limited in what it does and it works at runtime instead of
-making the whole thing actually move to the new location.  We
-ran into a ton of issues with it and it is currently in the
-process of being phased out.
-
-### Why would I want to use it?
-
-The main reason you want to use this is for build caching.  You
-have one folder where one virtualenv exists, you install the
-latest version of your codebase and all extensions in there, then
-you can make the virtualenv relocate to a target location, put it
-into a tarball, distribute it to all servers and done!
-
-### Example flow:
-
-First time: create the build cache
-
-```
-$ mkdir /tmp/build-cache
-$ virtualenv --distribute /tmp/build-cache
-```
-
-Now every time you build:
-
-```
-$ . /tmp/build-cache/bin/activate
-$ pip install YourApplication
-```
-
-Build done, package up and copy to whatever location you want to have it.
-
-Once unpacked on the target server, use the virtualenv tools to
-update the paths and make the virtualenv magically work in the new
-location.  For instance we deploy things to a path with the
-hash of the commit in:
-
-```
-$ virtualenv-tools --update-path /srv/your-application/<hash>
-```
-
-Compile once, deploy whereever.  Virtualenvs are completely self
-contained.  In order to switch the current version all you need to
-do is to relink the builds.
-
-
```

### Comparing `virtualenv_tools3-3.0.0/README.md` & `virtualenv_tools3-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `virtualenv_tools3-3.0.0/setup.cfg` & `virtualenv_tools3-3.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = virtualenv_tools3
-version = 3.0.0
+version = 3.1.0
 description = A set of tools for virtualenv
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = http://github.com/Yelp/virtualenv-tools
 author = Fireteam Ltd.; Yelp, Inc.
 author_email = opensource@yelp.com
 license_file = LICENSE
```

### Comparing `virtualenv_tools3-3.0.0/virtualenv_tools.py` & `virtualenv_tools3-3.1.0/virtualenv_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,25 +87,50 @@
     new_path = new_path_s.encode(filesystem_encoding)
 
     with open(script_filename, 'rb') as f:
         if f.read(2) != b'#!':
             return
         f.seek(0)
         lines = list(f)
-    args = lines[0][2:].strip().split()
-    if not args:
-        return
 
-    if path_is_within(args[0], old_path):
-        new_bin = os.path.join(new_path, os.path.relpath(args[0], old_path))
+    # is this a python script being run under a bourne exec call
+    if (
+            len(lines) >= 2 and
+            lines[0] == b'#!/bin/sh\n' and
+            lines[1].startswith(b"'''exec' ")
+    ):
+        args = lines[1].strip().split()
+
+        if path_is_within(args[1], old_path):
+            new_bin = os.path.join(
+                new_path,
+                os.path.relpath(args[1], old_path)
+            )
+        else:
+            return
+
+        args[1] = new_bin
+        lines[1] = b' '.join(args) + b'\n'
     else:
-        return
+        args = lines[0][2:].strip().split()
+
+        if not args:
+            return
+
+        if path_is_within(args[0], old_path):
+            new_bin = os.path.join(
+                new_path,
+                os.path.relpath(args[0], old_path)
+            )
+        else:
+            return
+
+        args[0] = new_bin
+        lines[0] = b'#!' + b' '.join(args) + b'\n'
 
-    args[0] = new_bin
-    lines[0] = b'#!' + b' '.join(args) + b'\n'
     debug('S %s' % script_filename)
     with open(script_filename, 'wb') as f:
         f.writelines(lines)
 
 
 def update_scripts(
         bin_dir: str,
```

### Comparing `virtualenv_tools3-3.0.0/virtualenv_tools3.egg-info/PKG-INFO` & `virtualenv_tools3-3.1.0/virtualenv_tools3.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,110 @@
 Metadata-Version: 2.1
 Name: virtualenv-tools3
-Version: 3.0.0
+Version: 3.1.0
 Summary: A set of tools for virtualenv
 Home-page: http://github.com/Yelp/virtualenv-tools
 Author: Fireteam Ltd.; Yelp, Inc.
 Author-email: opensource@yelp.com
 License: UNKNOWN
+Description: [![Build Status](https://travis-ci.org/Yelp/virtualenv-tools.svg?branch=master)](https://travis-ci.org/Yelp/virtualenv-tools)
+        [![Coverage Status](https://img.shields.io/coveralls/Yelp/virtualenv-tools.svg?branch=master)](https://coveralls.io/r/Yelp/virtualenv-tools)
+        [![PyPI version](https://badge.fury.io/py/virtualenv-tools3.svg)](https://pypi.python.org/pypi/virtualenv-tools3)
+        
+        virtualenv-tools3
+        --------
+        
+        virtualenv-tools3 is a fork of [the original
+        virtualenv-tools](https://github.com/fireteam/virtualenv-tools) (now
+        unmaintained) which adds support for Python 3, among other things. Full patch
+        details are below.
+        
+        ##  yelp patches
+        
+        ### yelp4
+        
+        * Add python3 support
+        * Drop python2.6 support
+        * 100% test coverage
+        * Removes `$VENV/local` instead of fixing up symlinks
+        * Removed `--reinitialize`, instead run `virtualenv $VENV -p $PYTHON`
+        * Rewrite .pth files to relative paths
+        
+        
+        ### yelp3
+        
+        * default output much more concise, added a --verbose option
+        * improved fault tolerance, in the case of:
+            * corrupt pyc files
+            * broken symlinks
+            * unexpected directories
+        * no-changes-needed is a success case (idempotency exits 0)
+        
+        
+        ### yelp1
+        
+        * --update now works more generally and reliably (e.g. virtualenv --python=python2.7)
+        
+        
+        ## virtualenv-tools
+        
+        This repository contains scripts we're using at Fireteam for our
+        deployment of Python code.  We're using them in combination with
+        salt to build code on one server on a self contained virtualenv
+        and then move that over to the destination servers to run.
+        
+        ### Why not virtualenv --relocatable?
+        
+        For starters: because it does not work.  relocatable is very
+        limited in what it does and it works at runtime instead of
+        making the whole thing actually move to the new location.  We
+        ran into a ton of issues with it and it is currently in the
+        process of being phased out.
+        
+        ### Why would I want to use it?
+        
+        The main reason you want to use this is for build caching.  You
+        have one folder where one virtualenv exists, you install the
+        latest version of your codebase and all extensions in there, then
+        you can make the virtualenv relocate to a target location, put it
+        into a tarball, distribute it to all servers and done!
+        
+        ### Example flow:
+        
+        First time: create the build cache
+        
+        ```
+        $ mkdir /tmp/build-cache
+        $ virtualenv --distribute /tmp/build-cache
+        ```
+        
+        Now every time you build:
+        
+        ```
+        $ . /tmp/build-cache/bin/activate
+        $ pip install YourApplication
+        ```
+        
+        Build done, package up and copy to whatever location you want to have it.
+        
+        Once unpacked on the target server, use the virtualenv tools to
+        update the paths and make the virtualenv magically work in the new
+        location.  For instance we deploy things to a path with the
+        hash of the commit in:
+        
+        ```
+        $ virtualenv-tools --update-path /srv/your-application/<hash>
+        ```
+        
+        Compile once, deploy whereever.  Virtualenvs are completely self
+        contained.  In order to switch the current version all you need to
+        do is to relink the builds.
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Build Status](https://travis-ci.org/Yelp/virtualenv-tools.svg?branch=master)](https://travis-ci.org/Yelp/virtualenv-tools)
-[![Coverage Status](https://img.shields.io/coveralls/Yelp/virtualenv-tools.svg?branch=master)](https://coveralls.io/r/Yelp/virtualenv-tools)
-[![PyPI version](https://badge.fury.io/py/virtualenv-tools3.svg)](https://pypi.python.org/pypi/virtualenv-tools3)
-
-virtualenv-tools3
---------
-
-virtualenv-tools3 is a fork of [the original
-virtualenv-tools](https://github.com/fireteam/virtualenv-tools) (now
-unmaintained) which adds support for Python 3, among other things. Full patch
-details are below.
-
-##  yelp patches
-
-### yelp4
-
-* Add python3 support
-* Drop python2.6 support
-* 100% test coverage
-* Removes `$VENV/local` instead of fixing up symlinks
-* Removed `--reinitialize`, instead run `virtualenv $VENV -p $PYTHON`
-* Rewrite .pth files to relative paths
-
-
-### yelp3
-
-* default output much more concise, added a --verbose option
-* improved fault tolerance, in the case of:
-    * corrupt pyc files
-    * broken symlinks
-    * unexpected directories
-* no-changes-needed is a success case (idempotency exits 0)
-
-
-### yelp1
-
-* --update now works more generally and reliably (e.g. virtualenv --python=python2.7)
-
-
-## virtualenv-tools
-
-This repository contains scripts we're using at Fireteam for our
-deployment of Python code.  We're using them in combination with
-salt to build code on one server on a self contained virtualenv
-and then move that over to the destination servers to run.
-
-### Why not virtualenv --relocatable?
-
-For starters: because it does not work.  relocatable is very
-limited in what it does and it works at runtime instead of
-making the whole thing actually move to the new location.  We
-ran into a ton of issues with it and it is currently in the
-process of being phased out.
-
-### Why would I want to use it?
-
-The main reason you want to use this is for build caching.  You
-have one folder where one virtualenv exists, you install the
-latest version of your codebase and all extensions in there, then
-you can make the virtualenv relocate to a target location, put it
-into a tarball, distribute it to all servers and done!
-
-### Example flow:
-
-First time: create the build cache
-
-```
-$ mkdir /tmp/build-cache
-$ virtualenv --distribute /tmp/build-cache
-```
-
-Now every time you build:
-
-```
-$ . /tmp/build-cache/bin/activate
-$ pip install YourApplication
-```
-
-Build done, package up and copy to whatever location you want to have it.
-
-Once unpacked on the target server, use the virtualenv tools to
-update the paths and make the virtualenv magically work in the new
-location.  For instance we deploy things to a path with the
-hash of the commit in:
-
-```
-$ virtualenv-tools --update-path /srv/your-application/<hash>
-```
-
-Compile once, deploy whereever.  Virtualenvs are completely self
-contained.  In order to switch the current version all you need to
-do is to relink the builds.
-
-
```

