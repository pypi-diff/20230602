# Comparing `tmp/pepver-1.0.3.tar.gz` & `tmp/pepver-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepver-1.0.3.tar", max compression
+gzip compressed data, was "pepver-1.1.0.tar", max compression
```

## Comparing `pepver-1.0.3.tar` & `pepver-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1072 2022-09-29 16:22:12.696108 pepver-1.0.3/LICENSE
--rw-r--r--   0        0        0    11946 2022-09-29 16:22:12.696108 pepver-1.0.3/pepver/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 16:22:12.696108 pepver-1.0.3/pepver/py.typed
--rw-r--r--   0        0        0      955 2022-09-29 16:22:12.696108 pepver-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1983 2022-09-29 16:22:12.696108 pepver-1.0.3/readme.md
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 pepver-1.0.3/setup.py
--rw-r--r--   0        0        0     2773 1970-01-01 00:00:00.000000 pepver-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-02 11:53:00.615630 pepver-1.1.0/LICENSE
+-rw-r--r--   0        0        0    12824 2023-06-02 11:53:00.615630 pepver-1.1.0/pepver/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:53:00.615630 pepver-1.1.0/pepver/py.typed
+-rw-r--r--   0        0        0      955 2023-06-02 11:53:00.615630 pepver-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1983 2023-06-02 11:53:00.615630 pepver-1.1.0/readme.md
+-rw-r--r--   0        0        0     2776 1970-01-01 00:00:00.000000 pepver-1.1.0/PKG-INFO
```

### Comparing `pepver-1.0.3/LICENSE` & `pepver-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pepver-1.0.3/pepver/__init__.py` & `pepver-1.1.0/pepver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,32 @@
                 *tuple(part for part, _ in zip_longest(self.release, range(idx), fillvalue=0)),
                 change,
             )
         else:
             release = *self.release[:idx], self.release[idx] + change
         return type(self)(epoch=self.epoch, release=release)
 
+    def truncate_release(self, keep: int = 0) -> "Version":
+        """
+        Remove trailing zeroes from the release part of the version.
+
+        str(Version.parse("1.0.0.0").truncate()) == "1"
+        str(Version.parse("1.0.0.0").truncate(3)) == "1.0.0"
+        str(Version.parse("1.0.0.1").truncate(3)) == "1.0.0.1"
+        """
+        if keep < 0:
+            raise ValueError("kept number of digits must be non-negative")
+        if keep == 0:
+            keep = 1
+
+        version = deepcopy(self)
+        version.release = _truncate(version.release, keep)
+        return version
+
+
     @property
     def major(self) -> int:
         """Major (first) segment of the release part."""
         return self.release[0]
 
     @major.setter
     def major(self, value: int) -> None:
@@ -350,7 +368,17 @@
             return None
         return True
     if right is None:
         return False
     if left == right:
         return None
     return left < right
+
+
+def _truncate(value: Tuple[int, ...], keep: int) -> Tuple[int, ...]:
+    if len(value) <= keep:
+        return value
+    last_non_zero = keep
+    for i, val in enumerate(value[keep:], start=keep+1):
+        if val:
+            last_non_zero = i
+    return tuple(value[:last_non_zero])
```

### Comparing `pepver-1.0.3/pyproject.toml` & `pepver-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pepver"
-version = "1.0.3"
+version = "1.1.0"
 description = "PEP-440 version parsing, interpretation and manipulation"
 authors = ["technomunk <thegriffones@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/technomunk/pepver"
 repository = "https://github.com/technomunk/pepver"
 keywords = ["version", "package"]
```

### Comparing `pepver-1.0.3/readme.md` & `pepver-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `pepver-1.0.3/setup.py` & `pepver-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,92 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pepver
+Version: 1.1.0
+Summary: PEP-440 version parsing, interpretation and manipulation
+Home-page: https://github.com/technomunk/pepver
+License: MIT
+Keywords: version,package
+Author: technomunk
+Author-email: thegriffones@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Project-URL: Repository, https://github.com/technomunk/pepver
+Description-Content-Type: text/markdown
 
-packages = \
-['pepver']
+# pepver
 
-package_data = \
-{'': ['*']}
+[![Python versions](https://img.shields.io/pypi/pyversions/pepver.svg)](https://pypi.org/project/pepver)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Unit tests](https://github.com/technomunk/pepver/actions/workflows/test.yml/badge.svg)](https://github.com/technomunk/pepver/actions/workflows/test.yml)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-setup_kwargs = {
-    'name': 'pepver',
-    'version': '1.0.3',
-    'description': 'PEP-440 version parsing, interpretation and manipulation',
-    'long_description': '# pepver\n\n[![Python versions](https://img.shields.io/pypi/pyversions/pepver.svg)](https://pypi.org/project/pepver)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Unit tests](https://github.com/technomunk/pepver/actions/workflows/test.yml/badge.svg)](https://github.com/technomunk/pepver/actions/workflows/test.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nPEP-440 version parsing, interpretation and manipulation.\n\n```py\n>>> from pepver import Version\n>>> version = Version.parse("0!1.2.3.4a5.post6.dev7+8.9")\n>>> version.epoch\n0\n>>> version.release\n(1, 2, 3, 4)\n>>> version.major\n1\n>>> version.minor\n2\n>>> version.micro\n3\n>>> version.pre\n(\'a\', 5)\n>>> version.post\n6\n>>> version.dev\n7\n>>> version.local\n\'8.9\'\n```\n\n## Usage\n\nThe main star of the library is the `Version` class, which encompasses the semantics of a version string.\nIt can be instantiated directly or be parsed from a string:\n```py\n>>> from pepver import Version\n>>> Version(1, 2, 3, 4)\nValue(release=(1,), pre=2, post=3, dev=4)\n>>> Version((0, 1, 2, 3), post=11, epoch=1)\nValue(epoch=1, release=(0, 1, 2, 3), post=11)\n>>> Version.parse("11.2")\nValue(release=(11, 2))\n```\n\nVersions can be updated to suit one\'s needs:\n```py\n>>> from pepver import Version\n>>> version = Version.parse("0!1.2.3.4a5.post6.dev7+8.9")\n>>> version.update("minor")\nValue(epoch=0, release=(1, 3))\n>>> version.update("post", -2)\nValue(epoch=0, release=(1, 2, 3, 4), pre=(\'a\', 5), post=4)\n>>> version.update("release")\nValue(epoch=0, release=(1, 2, 3, 5))\n>>> version.update("release").is_final()\nTrue\n```\n\nVersions correctly convert into strings. Note that the conversion is "normalized" ie\nstandard representation that is the same for the same version:\n\n```py\n>>> from pepver import Version\n>>> str(Version.parse("010.12-11"))\n\'10.12.post11\'\n>>> str(Version.parse("1.2.3preview11dev"))\n\'1.2.3rc11.dev0\'\n```\n',
-    'author': 'technomunk',
-    'author_email': 'thegriffones@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/technomunk/pepver',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+PEP-440 version parsing, interpretation and manipulation.
 
+```py
+>>> from pepver import Version
+>>> version = Version.parse("0!1.2.3.4a5.post6.dev7+8.9")
+>>> version.epoch
+0
+>>> version.release
+(1, 2, 3, 4)
+>>> version.major
+1
+>>> version.minor
+2
+>>> version.micro
+3
+>>> version.pre
+('a', 5)
+>>> version.post
+6
+>>> version.dev
+7
+>>> version.local
+'8.9'
+```
+
+## Usage
+
+The main star of the library is the `Version` class, which encompasses the semantics of a version string.
+It can be instantiated directly or be parsed from a string:
+```py
+>>> from pepver import Version
+>>> Version(1, 2, 3, 4)
+Value(release=(1,), pre=2, post=3, dev=4)
+>>> Version((0, 1, 2, 3), post=11, epoch=1)
+Value(epoch=1, release=(0, 1, 2, 3), post=11)
+>>> Version.parse("11.2")
+Value(release=(11, 2))
+```
+
+Versions can be updated to suit one's needs:
+```py
+>>> from pepver import Version
+>>> version = Version.parse("0!1.2.3.4a5.post6.dev7+8.9")
+>>> version.update("minor")
+Value(epoch=0, release=(1, 3))
+>>> version.update("post", -2)
+Value(epoch=0, release=(1, 2, 3, 4), pre=('a', 5), post=4)
+>>> version.update("release")
+Value(epoch=0, release=(1, 2, 3, 5))
+>>> version.update("release").is_final()
+True
+```
+
+Versions correctly convert into strings. Note that the conversion is "normalized" ie
+standard representation that is the same for the same version:
+
+```py
+>>> from pepver import Version
+>>> str(Version.parse("010.12-11"))
+'10.12.post11'
+>>> str(Version.parse("1.2.3preview11dev"))
+'1.2.3rc11.dev0'
+```
 
-setup(**setup_kwargs)
```

