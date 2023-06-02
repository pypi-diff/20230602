# Comparing `tmp/django-stubs-ext-4.2.0.tar.gz` & `tmp/django-stubs-ext-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stubs-ext-4.2.0.tar", last modified: Thu Apr 27 12:47:35 2023, max compression
+gzip compressed data, was "django-stubs-ext-4.2.1.tar", last modified: Fri Jun  2 14:11:07 2023, max compression
```

## Comparing `django-stubs-ext-4.2.0.tar` & `django-stubs-ext-4.2.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/
--rw-r--r--   0 marti     (1000) marti      (121)     3658 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/README.md
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/django_stubs_ext/
--rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/__init__.py
--rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/annotations.py
--rw-r--r--   0 marti     (1000) marti      (121)     3660 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/patch.py
--rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/py.typed
--rw-r--r--   0 marti     (1000) marti      (121)      266 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/django_stubs_ext/types.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/
--rw-r--r--   0 marti     (1000) marti      (121)     3658 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/PKG-INFO
--rw-r--r--   0 marti     (1000) marti      (121)      460 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/SOURCES.txt
--rw-r--r--   0 marti     (1000) marti      (121)        1 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/dependency_links.txt
--rw-r--r--   0 marti     (1000) marti      (121)       25 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/requires.txt
--rw-r--r--   0 marti     (1000) marti      (121)       17 2023-04-27 12:47:35.000000 django-stubs-ext-4.2.0/django_stubs_ext.egg-info/top_level.txt
--rw-r--r--   0 marti     (1000) marti      (121)       80 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/setup.cfg
--rw-r--r--   0 marti     (1000) marti      (121)     1808 2023-04-27 12:45:58.000000 django-stubs-ext-4.2.0/setup.py
-drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-04-27 12:47:35.943416 django-stubs-ext-4.2.0/tests/
--rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/tests/test_aliases.py
--rw-r--r--   0 marti     (1000) marti      (121)     3957 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.0/tests/test_monkeypatching.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/
+-rw-r--r--   0 marti     (1000) marti      (121)     1075 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/LICENSE.md
+-rw-r--r--   0 marti     (1000) marti      (121)     3565 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)     2496 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/README.md
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.161298 django-stubs-ext-4.2.1/django_stubs_ext/
+-rw-r--r--   0 marti     (1000) marti      (121)      535 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)      620 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)      693 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/annotations.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/django_stubs_ext/db/
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/db/__init__.py
+-rw-r--r--   0 marti     (1000) marti      (121)     1886 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/db/models.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3660 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/patch.py
+-rw-r--r--   0 marti     (1000) marti      (121)        0 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/django_stubs_ext/py.typed
+-rw-r--r--   0 marti     (1000) marti      (121)      236 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/django_stubs_ext/types.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/
+-rw-r--r--   0 marti     (1000) marti      (121)     3565 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/PKG-INFO
+-rw-r--r--   0 marti     (1000) marti      (121)      508 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 marti     (1000) marti      (121)        1 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       25 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/requires.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       17 2023-06-02 14:11:07.000000 django-stubs-ext-4.2.1/django_stubs_ext.egg-info/top_level.txt
+-rw-r--r--   0 marti     (1000) marti      (121)       38 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/setup.cfg
+-rwxr-xr-x   0 marti     (1000) marti      (121)     1777 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/setup.py
+drwxr-xr-x   0 marti     (1000) marti      (121)        0 2023-06-02 14:11:07.164631 django-stubs-ext-4.2.1/tests/
+-rw-r--r--   0 marti     (1000) marti      (121)      169 2023-03-15 16:53:32.000000 django-stubs-ext-4.2.1/tests/test_aliases.py
+-rw-r--r--   0 marti     (1000) marti      (121)     3928 2023-06-02 14:08:54.000000 django-stubs-ext-4.2.1/tests/test_monkeypatching.py
```

### Comparing `django-stubs-ext-4.2.0/PKG-INFO` & `django-stubs-ext-4.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.0
+Version: 4.2.1
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: ../LICENSE.txt
+License-File: LICENSE.md
 
 # Extensions and monkey-patching for django-stubs
 
 [![Build Status](https://travis-ci.com/typeddjango/django-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/django-stubs)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
```

### Comparing `django-stubs-ext-4.2.0/README.md` & `django-stubs-ext-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.0/django_stubs_ext/__init__.py` & `django-stubs-ext-4.2.1/django_stubs_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.0/django_stubs_ext/aliases.py` & `django-stubs-ext-4.2.1/django_stubs_ext/aliases.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.0/django_stubs_ext/annotations.py` & `django-stubs-ext-4.2.1/django_stubs_ext/annotations.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.0/django_stubs_ext/patch.py` & `django-stubs-ext-4.2.1/django_stubs_ext/patch.py`

 * *Files identical despite different names*

### Comparing `django-stubs-ext-4.2.0/django_stubs_ext.egg-info/PKG-INFO` & `django-stubs-ext-4.2.1/django_stubs_ext.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: django-stubs-ext
-Version: 4.2.0
+Version: 4.2.1
 Summary: Monkey-patching and extensions for django-stubs
 Home-page: https://github.com/typeddjango/django-stubs
 Author: Simula Proxy
 Author-email: 3nki.nam.shub@gmail.com
 Maintainer: Marti Raudsepp
 Maintainer-email: marti@juffo.org
 License: MIT
 Project-URL: Release notes, https://github.com/typeddjango/django-stubs/releases
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: ../LICENSE.txt
+License-File: LICENSE.md
 
 # Extensions and monkey-patching for django-stubs
 
 [![Build Status](https://travis-ci.com/typeddjango/django-stubs.svg?branch=master)](https://travis-ci.com/typeddjango/django-stubs)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Gitter](https://badges.gitter.im/mypy-django/Lobby.svg)](https://gitter.im/mypy-django/Lobby)
```

### Comparing `django-stubs-ext-4.2.0/setup.py` & `django-stubs-ext-4.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python
 from distutils.core import setup
 
 from setuptools import find_packages
 
 with open("README.md") as f:
     readme = f.read()
 
@@ -10,44 +11,43 @@
     "typing-extensions",
 ]
 
 # NB! For clarity, keep version major.minor.patch in sync with django-stubs.
 # It's fine to skip django-stubs-ext releases, but when doing a release, update this to newest django-stubs version.
 setup(
     name="django-stubs-ext",
-    version="4.2.0",
+    version="4.2.1",
     description="Monkey-patching and extensions for django-stubs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
+    license_files=["LICENSE.md"],
     url="https://github.com/typeddjango/django-stubs",
     author="Simula Proxy",
     author_email="3nki.nam.shub@gmail.com",
     maintainer="Marti Raudsepp",
     maintainer_email="marti@juffo.org",
     py_modules=[],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     install_requires=dependencies,
     packages=["django_stubs_ext", *find_packages(exclude=["scripts"])],
     package_data={"django_stubs_ext": ["py.typed"]},
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Framework :: Django",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
         "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
         "Framework :: Django :: 4.2",
     ],
     project_urls={
         "Release notes": "https://github.com/typeddjango/django-stubs/releases",
     },
 )
```

### Comparing `django-stubs-ext-4.2.0/tests/test_monkeypatching.py` & `django-stubs-ext-4.2.1/tests/test_monkeypatching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import builtins
 from contextlib import suppress
-from typing import Iterable, List, Optional
+from typing import Iterable, List, Optional, Protocol
 
 import pytest
 from _pytest.fixtures import FixtureRequest
 from _pytest.monkeypatch import MonkeyPatch
 from django.db.models import Model
 from django.forms.models import ModelForm
-from typing_extensions import Protocol
 
 import django_stubs_ext
 from django_stubs_ext import patch
 from django_stubs_ext.patch import _need_generic, _VersionSpec
 
 
 class _MakeGenericClasses(Protocol):
```

