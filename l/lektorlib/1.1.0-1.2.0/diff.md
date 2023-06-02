# Comparing `tmp/lektorlib-1.1.0.tar.gz` & `tmp/lektorlib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektorlib-1.1.0.tar", last modified: Fri Apr 21 02:16:01 2023, max compression
+gzip compressed data, was "lektorlib-1.2.0.tar", last modified: Fri Jun  2 20:51:24 2023, max compression
```

## Comparing `lektorlib-1.1.0.tar` & `lektorlib-1.2.0.tar`

### file list

```diff
@@ -1,46 +1,27 @@
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      101 2022-01-28 23:09:49.000000 lektorlib-1.1.0/.gitignore
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      380 2023-04-21 02:13:38.000000 lektorlib-1.1.0/CHANGES.md
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1062 2020-05-05 17:14:03.000000 lektorlib-1.1.0/LICENSE
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       14 2023-04-20 22:36:48.000000 lektorlib-1.1.0/MANIFEST.in
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4649 2023-04-21 02:16:01.364485 lektorlib-1.1.0/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2071 2022-01-28 20:29:23.000000 lektorlib-1.1.0/README.md
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/lektorlib/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)        0 2020-04-26 00:52:06.000000 lektorlib-1.1.0/lektorlib/__init__.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      886 2023-04-20 22:36:48.000000 lektorlib-1.1.0/lektorlib/context.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     5087 2022-01-28 19:26:47.000000 lektorlib-1.1.0/lektorlib/query.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      756 2022-01-28 19:17:12.000000 lektorlib-1.1.0/lektorlib/recordcache.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      466 2022-01-28 19:27:18.000000 lektorlib-1.1.0/lektorlib/testing.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/lektorlib.egg-info/
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     4649 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/PKG-INFO
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)      798 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/SOURCES.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)        1 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/dependency_links.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       10 2023-04-21 02:16:01.000000 lektorlib-1.1.0/lektorlib.egg-info/top_level.txt
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1173 2023-04-20 22:36:48.000000 lektorlib-1.1.0/pyproject.toml
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)       38 2023-04-21 02:16:01.364485 lektorlib-1.1.0/setup.cfg
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)        0 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/__init__.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     1015 2022-01-28 19:27:52.000000 lektorlib-1.1.0/tests/conftest.py
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)       27 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/Test Site.lektorproject
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.360485 lektorlib-1.1.0/tests/test-site/assets/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/assets/static/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      538 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/assets/static/style.css
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/about/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      144 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/about/contents.lr
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      135 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/contents.lr
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/content/projects/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)       96 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/content/projects/contents.lr
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/models/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      133 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/models/page.ini
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/templates/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      804 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/layout.html
-drwxrwxr-x   0 dairiki   (1000) dairiki   (1000)        0 2023-04-21 02:16:01.364485 lektorlib-1.1.0/tests/test-site/templates/macros/
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      475 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/macros/pagination.html
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      154 2020-04-26 00:52:06.000000 lektorlib-1.1.0/tests/test-site/templates/page.html
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     2123 2023-04-20 22:36:48.000000 lektorlib-1.1.0/tests/test_context.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     8641 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_query.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)     2112 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_recordcache.py
--rw-r--r--   0 dairiki   (1000) dairiki   (1000)      729 2022-01-28 19:17:12.000000 lektorlib-1.1.0/tests/test_testing.py
--rw-rw-r--   0 dairiki   (1000) dairiki   (1000)     1002 2023-04-20 22:36:48.000000 lektorlib-1.1.0/tox.ini
+-rw-r--r--   0        0        0      567 2023-06-02 20:51:07.394074 lektorlib-1.2.0/CHANGES.md
+-rw-r--r--   0        0        0     1062 2023-06-02 20:51:07.394074 lektorlib-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2204 2023-06-02 20:51:07.394074 lektorlib-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/context.py
+-rw-r--r--   0        0        0        0 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/py.typed
+-rw-r--r--   0        0        0     6155 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/query.py
+-rw-r--r--   0        0        0     1056 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/recordcache.py
+-rw-r--r--   0        0        0      749 2023-06-02 20:51:07.394074 lektorlib-1.2.0/lektorlib/testing.py
+-rw-r--r--   0        0        0      753 2023-06-02 20:51:07.398074 lektorlib-1.2.0/pdm_build.py
+-rw-r--r--   0        0        0     4963 2023-06-02 20:51:24.386522 lektorlib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1014 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       27 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/Test Site.lektorproject
+-rw-r--r--   0        0        0      538 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/assets/static/style.css
+-rw-r--r--   0        0        0      144 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/about/contents.lr
+-rw-r--r--   0        0        0      135 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/contents.lr
+-rw-r--r--   0        0        0       96 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/content/projects/contents.lr
+-rw-r--r--   0        0        0      133 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/models/page.ini
+-rw-r--r--   0        0        0      804 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/layout.html
+-rw-r--r--   0        0        0      475 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/macros/pagination.html
+-rw-r--r--   0        0        0      154 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test-site/templates/page.html
+-rw-r--r--   0        0        0     2103 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_context.py
+-rw-r--r--   0        0        0     8876 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_query.py
+-rw-r--r--   0        0        0     2087 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_recordcache.py
+-rw-r--r--   0        0        0      727 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tests/test_testing.py
+-rw-r--r--   0        0        0     1178 2023-06-02 20:51:07.398074 lektorlib-1.2.0/tox.ini
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 lektorlib-1.2.0/PKG-INFO
```

### Comparing `lektorlib-1.1.0/LICENSE` & `lektorlib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lektorlib-1.1.0/PKG-INFO` & `lektorlib-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: lektorlib
-Version: 1.1.0
+Version: 1.2.0
 Summary: A few bits which are potentially useful to developers of Lektor plugins
-Author-email: Jeff Dairiki <dairiki@dairiki.org>
+Keywords: Lektor utilities
+Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: Copyright © 2020 Geoffrey T. Dairiki
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
         distribute, sublicense, and/or sell copies of the Software, and to
@@ -19,40 +20,38 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Home, https://github.com/dairiki/lektorlib
-Keywords: Lektor,utilities
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Lektor
 Classifier: Environment :: Plugins
 Classifier: Topic :: Software Development :: Libraries
+Project-URL: Home, https://github.com/dairiki/lektorlib
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Lektorlib
 
 [![PyPI version](https://img.shields.io/pypi/v/lektorlib.svg)](https://pypi.org/project/lektorlib/)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektorlib.svg)](https://pypi.python.org/pypi/lektorlib/)
 [![GitHub license](https://img.shields.io/github/license/dairiki/lektorlib)](https://github.com/dairiki/lektorlib/blob/master/LICENSE)
 [![GitHub Actions (Tests)](https://github.com/dairiki/lektorlib/workflows/Tests/badge.svg)](https://github.com/dairiki/lektorlib)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhaqecdxux7krt01vbsl)](https://trackgit.com)
 
 A few bits which may possibly be useful to developers of [Lektor][] plugins.
 
 ## Bits Included
 
 ### `lektorlib.query.PrecomputedQuery`
 
@@ -95,14 +94,21 @@
 
 Jeff Dairiki <dairiki@dairiki.org>
 
 [Lektor]: <https://www.getlektor.com/> "Lektor Static Content Management System"
 
 ## Changelog
 
+### Release 1.2.0 (2023-06-02)
+
+- Added type annotations
+- Use PDM instead of setuptools to build distribution
+- Configured pre-commit
+- Run black and reorder-python-imports on the code
+
 ### Release 1.1.0 (2023-04-20)
 
 Fixes for Lektor 3.4 (in pre-release).
 
 We now test under Lektor 3.3 and Lektor 3.4 (pre-release).
 
 ### Release 1.0 (2022-01-28)
```

### Comparing `lektorlib-1.1.0/README.md` & `lektorlib-1.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Lektorlib
 
 [![PyPI version](https://img.shields.io/pypi/v/lektorlib.svg)](https://pypi.org/project/lektorlib/)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektorlib.svg)](https://pypi.python.org/pypi/lektorlib/)
 [![GitHub license](https://img.shields.io/github/license/dairiki/lektorlib)](https://github.com/dairiki/lektorlib/blob/master/LICENSE)
 [![GitHub Actions (Tests)](https://github.com/dairiki/lektorlib/workflows/Tests/badge.svg)](https://github.com/dairiki/lektorlib)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhaqecdxux7krt01vbsl)](https://trackgit.com)
 
 A few bits which may possibly be useful to developers of [Lektor][] plugins.
 
 ## Bits Included
 
 ### `lektorlib.query.PrecomputedQuery`
```

### Comparing `lektorlib-1.1.0/lektorlib/query.py` & `lektorlib-1.2.0/lektorlib/query.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,40 @@
 """A Query-like object which can be used to access a precomputed
 sequence of sources.  This works for virtual sources, too.
 
 
 """
+from __future__ import annotations
+
+import sys
 from collections import OrderedDict
+from typing import Generator
+from typing import Iterable
+from typing import Sequence
+from typing import TYPE_CHECKING
 
+from lektor.db import Pad
 from lektor.db import Query
+from lektor.db import Record
 from lektor.environment import PRIMARY_ALT
+from lektor.sourceobj import VirtualSourceObject
+
+if sys.version_info >= (3, 10):
+    from types import EllipsisType
+elif TYPE_CHECKING:
+    from builtins import ellipsis as EllipsisType
 
 
-def get_source(pad, path, alt=PRIMARY_ALT, page_num=None, persist=True):
+def get_source(
+    pad: Pad,
+    path: str,
+    alt: str = PRIMARY_ALT,
+    page_num: int | None = None,
+    persist: bool = True,
+) -> Record | VirtualSourceObject:
     """Like Pad.get() but works for paginated virtual sources as well as
     concrete records.
 
     """
     # lektor.db.Pad.get does not support page_num on a virtual path.
     # This is mostly because there seems to be no official syntax for
     # contructing a virtual path with a page number.
@@ -25,15 +46,15 @@
     # This function will use the ``source.pagination.for_page()``
     # method exposed by the pagination API to get the paginated
     # version of the source.
     #
     # NB: The user will have to ensure that pagination.for_page
     # is properly implemented for their virtual sources.
 
-    if page_num is None or '@' not in path:
+    if page_num is None or "@" not in path:
         return pad.get(path, alt=alt, page_num=page_num, persist=persist)
 
     source = pad.get(path, persist=persist, alt=alt)
     if source is None:
         return None
     try:
         pagination = source.pagination
@@ -44,47 +65,65 @@
         return None
 
     paginated_source = pagination.for_page(page_num)
     pad.db.track_record_dependency(paginated_source)
     return paginated_source
 
 
-class PrecomputedQuery(Query):
+class PrecomputedQuery(Query):  # type: ignore[misc]
     """This is a Query which yields a pre-computed sequence of children.
 
     This is useful in (at least) two circumstances:
 
     First, when the children to be queried are virtual source objects,
     the standard ``lektor.db.Query`` will not work.  This version will.
 
     Second, when we would like to generate a query of a pre-computed
     subset of a resource's children, this prevents intruducing
     unnecessary build dependencies.  If we used a standard query with
     a filter applied, still iterates of all of the parent nodes
     children, registering dependencies on all of them.
 
     """
-    def __init__(self, path, pad, child_ids, alt=PRIMARY_ALT):
+
+    # Annotations for fields inherited from Query
+    _order_by: Sequence[str] | None
+    _page_num: int | None
+
+    def __init__(
+        self,
+        path: str,
+        pad: Pad,
+        child_ids: Iterable[str],
+        alt: str = PRIMARY_ALT,
+    ):
         super().__init__(path, pad, alt=alt)
         # We really just want an ordered set, but we'll use an OrderedDict
         # to avoid requiring another library.
         self.__child_ids = OrderedDict((id_, None) for id_ in child_ids)
         self.__assert_is_not_attachment_query()
 
-    def _get(self, id, persist=True, page_num=Ellipsis):
+    def _get(
+        self,
+        id: str,
+        persist: bool = True,
+        page_num: int | None | EllipsisType = Ellipsis,
+    ) -> Record | VirtualSourceObject:
         """Low level record access."""
         if id not in self.__child_ids:
-            return None         # not in our query set
-        if page_num is Ellipsis:
-            page_num = self._page_num
-        return get_source(self.pad,
-                          path=f'{self.path}/{id}',
-                          page_num=page_num, alt=self.alt, persist=persist)
+            return None  # not in our query set
+        return get_source(
+            self.pad,
+            path=f"{self.path}/{id}",
+            page_num=self._page_num if page_num is Ellipsis else page_num,
+            alt=self.alt,
+            persist=persist,
+        )
 
-    def _iterate(self):
+    def _iterate(self) -> Generator[Record | VirtualSourceObject, None, None]:
         self.__assert_is_not_attachment_query()
         # note dependencies
         self_record = self.pad.get(self.path, alt=self.alt)
         if self_record is not None:
             self.pad.db.track_record_dependency(self_record)
 
         for id in self.__child_ids:
@@ -93,40 +132,42 @@
                 if self._page_num is not None:
                     # Sanity check: ensure the unpaginated version exists
                     unpaginated = self._get(id, persist=False, page_num=None)
                     if unpaginated is not None:
                         # Requested explicit page_num, but source does not
                         # support pagination.  Punt and skip it.
                         continue
-                path = f'{self.path}/{id}'
+                path = f"{self.path}/{id}"
                 raise RuntimeError("could not load source for %r" % path)
 
-            is_page = not getattr(record, 'is_attachment', False)
+            is_page = not getattr(record, "is_attachment", False)
             if is_page and self._matches(record):
                 yield record
 
-    def get_order_by(self):
+    def get_order_by(self) -> Sequence[str] | None:
         # child_ids are already in default order, so unless an ordering
         # is explicitly applied, we do not need to sort the results
         return self._order_by
 
-    def __assert_is_not_attachment_query(self):
+    def __assert_is_not_attachment_query(self) -> None:
         if not self._include_pages or self._include_attachments:
-            raise AssertionError(
-                "Attachment queries are not currently supported")
+            raise AssertionError("Attachment queries are not currently supported")
 
-    def count(self):
+    def count(self) -> int:
         if self._pristine:
             # optimization
             return len(self.__child_ids)
-        return super().count()
+        return super().count()  # type: ignore[no-any-return]
 
-    def get(self, id, page_num=Ellipsis):
+    def get(
+        self, id: str, page_num: int | None | EllipsisType = Ellipsis
+    ) -> Record | VirtualSourceObject | None:
         # optimization
         if id in self.__child_ids:
             return self._get(id, page_num=page_num)
+        return None
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         if self._pristine:
             # optimization
             return len(self.__child_ids) > 0
-        return super().__bool__()
+        return super().__bool__()  # type: ignore[no-any-return]
```

### Comparing `lektorlib-1.1.0/tests/conftest.py` & `lektorlib-1.2.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from pathlib import Path
 
-import pytest
-
 import lektor.builder
 import lektor.context
 import lektor.datamodel
 import lektor.db
 import lektor.environment
 import lektor.pagination
 import lektor.project
+import pytest
 
 
 @pytest.fixture(scope="session")
 def site_path():
-    return Path(__file__).parent / 'test-site'
+    return Path(__file__).parent / "test-site"
 
 
 @pytest.fixture
 def lektor_project(site_path):
     return lektor.project.Project.from_path(str(site_path))
```

### Comparing `lektorlib-1.1.0/tests/test-site/assets/static/style.css` & `lektorlib-1.2.0/tests/test-site/assets/static/style.css`

 * *Files identical despite different names*

### Comparing `lektorlib-1.1.0/tests/test-site/templates/layout.html` & `lektorlib-1.2.0/tests/test-site/templates/layout.html`

 * *Files identical despite different names*

### Comparing `lektorlib-1.1.0/tests/test_context.py` & `lektorlib-1.2.0/tests/test_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 import pytest
+from lektor.context import Context
+from lektor.context import get_ctx
 
-from lektor.context import (
-    get_ctx,
-    Context,
-    )
-
-from lektorlib.context import (
-    disable_dependency_recording,
-    DependencyIgnoringContextProxy,
-    )
+from lektorlib.context import DependencyIgnoringContextProxy
+from lektorlib.context import disable_dependency_recording
 
 
 class Test_disable_dependency_recording:
-
-    @pytest.mark.usefixtures('lektor_context')
+    @pytest.mark.usefixtures("lektor_context")
     def test(self):
-        get_ctx().record_dependency('a')
+        get_ctx().record_dependency("a")
         with disable_dependency_recording():
-            get_ctx().record_dependency('b')
-        get_ctx().record_dependency('c')
-        assert get_ctx().referenced_dependencies == {'a', 'c'}
+            get_ctx().record_dependency("b")
+        get_ctx().record_dependency("c")
+        assert get_ctx().referenced_dependencies == {"a", "c"}
 
     def test_no_context(self):
         assert get_ctx() is None
         with disable_dependency_recording():
             assert get_ctx() is None
         assert get_ctx() is None
 
@@ -40,25 +34,24 @@
         assert get_ctx() is lektor_context
 
     def test_isinstance(self, proxy):
         assert isinstance(proxy, DependencyIgnoringContextProxy)
         assert isinstance(proxy, Context)
 
     def test_cache(self, proxy, lektor_context):
-        proxy.cache['test'] = 'value'
-        assert lektor_context.cache['test'] == 'value'
+        proxy.cache["test"] = "value"
+        assert lektor_context.cache["test"] == "value"
 
     def test_record_dependency(self, proxy, lektor_context):
-        lektor_context.record_dependency('a')
-        proxy.record_dependency('b')
-        assert proxy.referenced_dependencies == set('a')
+        lektor_context.record_dependency("a")
+        proxy.record_dependency("b")
+        assert proxy.referenced_dependencies == set("a")
 
     def test_record_dependency_accepts_affects_url(self, proxy):
-        proxy.record_dependency('b', affects_url=True)
+        proxy.record_dependency("b", affects_url=True)
         assert proxy.referenced_dependencies == set()
 
-    def test_record_virtual_dependency(self, proxy, lektor_context,
-                                       lektor_pad):
-        proxy.record_virtual_dependency(lektor_pad.get('/projects@1'))
+    def test_record_virtual_dependency(self, proxy, lektor_context, lektor_pad):
+        proxy.record_virtual_dependency(lektor_pad.get("/projects@1"))
         assert not proxy.referenced_virtual_dependencies
-        lektor_context.record_virtual_dependency(lektor_pad.get('/projects@2'))
+        lektor_context.record_virtual_dependency(lektor_pad.get("/projects@2"))
         assert proxy.referenced_virtual_dependencies
```

### Comparing `lektorlib-1.1.0/tests/test_query.py` & `lektorlib-1.2.0/tests/test_query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import inspect
 import re
 
 import pytest
-
-from lektor.environment import (
-    Expression,
-    PRIMARY_ALT,
-    )
+from lektor.environment import Expression
+from lektor.environment import PRIMARY_ALT
 from lektor.pluginsystem import Plugin
 from lektor.sourceobj import VirtualSourceObject
 
-from lektorlib.query import (
-    get_source,
-    PrecomputedQuery,
-    )
+from lektorlib.query import get_source
+from lektorlib.query import PrecomputedQuery
 
 
 class DummyVirtualSource(VirtualSourceObject):
-    virtual_path_prefix = 'dummy-virtual'
+    virtual_path_prefix = "dummy-virtual"
 
     def __init__(self, record, extra_path=None):
         VirtualSourceObject.__init__(self, record)
         self.extra_path = extra_path
 
     @property
     def path(self):
         fmt = "{0.record.path}@{0.virtual_path_prefix}"
         if self.extra_path:
             fmt += "/{0.extra_path}"
         return fmt.format(self)
 
 
 class PaginatedVirtualSource(DummyVirtualSource):
-    virtual_path_prefix = 'paginated-virtual'
+    virtual_path_prefix = "paginated-virtual"
 
     def __init__(self, record, extra_path=None, page_num=None):
         super().__init__(record, extra_path)
         self.page_num = page_num
 
     @property
     def path(self):
@@ -54,219 +49,241 @@
     def __init__(self, source):
         self.source = source
 
     def for_page(self, page_num):
         source = self.source
         if page_num == source.page_num:
             return source
-        return PaginatedVirtualSource(
-            source.record, source.extra_path, page_num)
+        return PaginatedVirtualSource(source.record, source.extra_path, page_num)
 
 
 class DummyPlugin(Plugin):
     def on_setup_env(self, **extra):
         env = self.env
 
-        @env.virtualpathresolver('dummy-virtual')
+        @env.virtualpathresolver("dummy-virtual")
         def resolve_virtual(record, pieces):
-            if 'missing' not in pieces:
-                return DummyVirtualSource(record, extra_path='/'.join(pieces))
+            if "missing" not in pieces:
+                return DummyVirtualSource(record, extra_path="/".join(pieces))
 
-        @env.virtualpathresolver('paginated-virtual')
+        @env.virtualpathresolver("paginated-virtual")
         def resolve_paginated(record, pieces):
-            if pieces and re.match(r'page=(\d+)\Z', pieces[-1]):
-                page_num = int(pieces[-1][len('page='):])
+            if pieces and re.match(r"page=(\d+)\Z", pieces[-1]):
+                page_num = int(pieces[-1][len("page=") :])
                 pieces = pieces[:-1]
             else:
                 page_num = None
-            if 'missing' not in pieces:
+            if "missing" not in pieces:
                 return PaginatedVirtualSource(
-                    record, extra_path='/'.join(pieces), page_num=page_num)
+                    record, extra_path="/".join(pieces), page_num=page_num
+                )
 
 
 @pytest.fixture
 def dummy_plugin(lektor_env):
     # Configure lektor_env with our dummy plugin
     plugin_controller = lektor_env.plugin_controller
-    plugin_controller.instanciate_plugin('dummy-plugin', DummyPlugin)
-    plugin_controller.emit('setup-env')
-    return lektor_env.plugins['dummy-plugin']
+    plugin_controller.instanciate_plugin("dummy-plugin", DummyPlugin)
+    plugin_controller.emit("setup-env")
+    return lektor_env.plugins["dummy-plugin"]
 
 
-@pytest.mark.usefixtures('dummy_plugin')
+@pytest.mark.usefixtures("dummy_plugin")
 class Test_get_source:
-    @pytest.mark.parametrize("path", [
-        "/",
-        "/about",
-        "/about@dummy-virtual",
-        "/projects@dummy-virtual/foo",
-        ])
+    @pytest.mark.parametrize(
+        "path",
+        [
+            "/",
+            "/about",
+            "/about@dummy-virtual",
+            "/projects@dummy-virtual/foo",
+        ],
+    )
     def test_get_unpaginated(self, lektor_pad, path):
         source = get_source(lektor_pad, path)
         assert source.path == path
-        assert getattr(source, 'page_num', None) is None
+        assert getattr(source, "page_num", None) is None
 
-    @pytest.mark.parametrize("path", [
-        "/projects",
-        "/projects@paginated-virtual",
-        "/@paginated-virtual/foo",
-        ])
+    @pytest.mark.parametrize(
+        "path",
+        [
+            "/projects",
+            "/projects@paginated-virtual",
+            "/@paginated-virtual/foo",
+        ],
+    )
     def test_get_paginated(self, lektor_pad, path):
         page_num = 1
         source = get_source(lektor_pad, path, page_num=page_num)
-        if '@' in path:
-            assert source.path == '%s/page=%d' % (path, page_num)
+        if "@" in path:
+            assert source.path == "%s/page=%d" % (path, page_num)
         else:
-            assert source.path == '%s@%d' % (path, page_num)
+            assert source.path == "%s@%d" % (path, page_num)
         assert source.page_num == page_num
 
-    @pytest.mark.parametrize("path", [
-        "/@dummy-virtual",
-        ])
+    @pytest.mark.parametrize(
+        "path",
+        [
+            "/@dummy-virtual",
+        ],
+    )
     def test_get_paginated_unsupported(self, lektor_pad, path):
         page_num = 1
         source = get_source(lektor_pad, path, page_num=page_num)
         assert source is None
 
-    @pytest.mark.parametrize("path", [
-        "/missing",
-        "/missing@dummy-virtual",
-        "/about@missing-virtual",
-        ])
+    @pytest.mark.parametrize(
+        "path",
+        [
+            "/missing",
+            "/missing@dummy-virtual",
+            "/about@missing-virtual",
+        ],
+    )
     def test_get_missing(self, lektor_pad, path):
         assert get_source(lektor_pad, path) is None
         assert get_source(lektor_pad, path, page_num=1) is None
 
 
-@pytest.mark.usefixtures('dummy_plugin')
+@pytest.mark.usefixtures("dummy_plugin")
 class QueryTestBase:
-
     @pytest.fixture
     def make_query(self, query_path, lektor_pad):
         def make_query(child_ids, **kw):
             return PrecomputedQuery(query_path, lektor_pad, child_ids, **kw)
+
         return make_query
 
     @pytest.fixture
     def jinja_eval(self, lektor_env, lektor_pad):
         def jinja_eval(expr, this=None, alt=None, **kw):
             frame = inspect.currentframe()
             try:
                 # Get locals from calling frame
                 locals = dict(frame.f_back.f_locals)
             finally:
                 del frame
             locals.update(kw)
             return Expression(lektor_env, expr).evaluate(
-                lektor_pad, this=this, values=locals, alt=alt)
+                lektor_pad, this=this, values=locals, alt=alt
+            )
+
         return jinja_eval
 
     @pytest.fixture
     def query(self, make_query, child_ids):
         return make_query(child_ids)
 
-    @pytest.mark.parametrize("extra_kw, expected_alt", [
-        ({}, PRIMARY_ALT),
-        ({'alt': 'xx'}, 'xx'),
-        ])
+    @pytest.mark.parametrize(
+        "extra_kw, expected_alt",
+        [
+            ({}, PRIMARY_ALT),
+            ({"alt": "xx"}, "xx"),
+        ],
+    )
     def test_with_alt(self, make_query, child_ids, extra_kw, expected_alt):
         query = make_query(child_ids, **extra_kw)
         assert query.first().alt == expected_alt
 
     def test_assert_is_not_attachment_query(self, query):
         query._include_attachments = True
-        with pytest.raises(AssertionError,
-                           match=r'(?i)attachment\b.* not\b.* supported'):
+        with pytest.raises(
+            AssertionError, match=r"(?i)attachment\b.* not\b.* supported"
+        ):
             query.first()
 
-    @pytest.mark.parametrize("child_ids", [('missing',)])
+    @pytest.mark.parametrize("child_ids", [("missing",)])
     def test_raises_on_missing_id(self, query):
         with pytest.raises(RuntimeError):
             query.first()
 
     def test__get_bad_id(self, query):
-        assert query._get('missing', persist=False) is None
+        assert query._get("missing", persist=False) is None
 
     def test_count(self, query, lektor_context):
         # .count() on a pristine PrecomputedQuery should not register deps
         n = query.count()
         assert not lektor_context.referenced_dependencies
         assert not lektor_context.referenced_virtual_dependencies
 
         # .on a non-pristine query, it does
         assert n == query.filter(lambda r: True).count()
-        assert lektor_context.referenced_dependencies \
+        assert (
+            lektor_context.referenced_dependencies
             or lektor_context.referenced_virtual_dependencies
+        )
 
     def test_bool(self, query, lektor_context):
         # .__bool__() on a pristine PrecomputedQuery should not register deps
         assert query
         assert not lektor_context.referenced_dependencies
         assert not lektor_context.referenced_virtual_dependencies
 
         # .on a non-pristine query, it does
         assert not query.filter(lambda r: False)
-        assert lektor_context.referenced_dependencies \
+        assert (
+            lektor_context.referenced_dependencies
             or lektor_context.referenced_virtual_dependencies
+        )
 
 
 class TestConcreteSourceQuery(QueryTestBase):
     @pytest.fixture
     def query_path(self):
-        return '/'
+        return "/"
 
     @pytest.fixture
     def child_ids(self):
-        return ('about', 'projects')
+        return ("about", "projects")
 
     def test_iter(self, query):
-        assert [obj.path for obj in query] == ['/about', '/projects']
+        assert [obj.path for obj in query] == ["/about", "/projects"]
 
-    @pytest.mark.parametrize("child_ids", [('about',)])
+    @pytest.mark.parametrize("child_ids", [("about",)])
     def test_get(self, query):
-        assert query.get('about')['_id'] == 'about'
-        assert query.get('projects') is None
+        assert query.get("about")["_id"] == "about"
+        assert query.get("projects") is None
 
     def test_filter(self, query, jinja_eval):
         assert jinja_eval("query.filter(F.title == 'Projects').count()") == 1
 
     def test_order_by(self, query, jinja_eval):
-        reversed = query.order_by('-title')
-        assert [obj['title'] for obj in reversed] == [
-            'Projects',
-            'About this Website',
-            ]
+        reversed = query.order_by("-title")
+        assert [obj["title"] for obj in reversed] == [
+            "Projects",
+            "About this Website",
+        ]
 
 
 class TestVirtualSourceQuery(QueryTestBase):
     virtual_path_prefix = DummyVirtualSource.virtual_path_prefix
 
     @pytest.fixture
     def query_path(self):
-        return f'/projects@{self.virtual_path_prefix}'
+        return f"/projects@{self.virtual_path_prefix}"
 
     @pytest.fixture
     def child_ids(self):
-        return ('a', 'b')
+        return ("a", "b")
 
     def test_iter(self, query):
         assert [obj.path for obj in query] == [
-            f'/projects@{self.virtual_path_prefix}/a',
-            f'/projects@{self.virtual_path_prefix}/b',
-            ]
+            f"/projects@{self.virtual_path_prefix}/a",
+            f"/projects@{self.virtual_path_prefix}/b",
+        ]
 
     def test_get(self, query):
-        assert query.get('a').extra_path == 'a'
-        assert query.get('x') is None
+        assert query.get("a").extra_path == "a"
+        assert query.get("x") is None
 
     def test_request_page(self, query):
         assert list(query.request_page(1)) == []
 
 
 class TestPaginatedVirtualSourceQuery(TestVirtualSourceQuery):
     virtual_path_prefix = PaginatedVirtualSource.virtual_path_prefix
 
     def test_request_page(self, query):
         assert [obj.path for obj in query.request_page(1)] == [
-            '/projects@paginated-virtual/a/page=1',
-            '/projects@paginated-virtual/b/page=1',
-            ]
+            "/projects@paginated-virtual/a/page=1",
+            "/projects@paginated-virtual/b/page=1",
+        ]
```

### Comparing `lektorlib-1.1.0/tests/test_recordcache.py` & `lektorlib-1.2.0/tests/test_recordcache.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 import pytest
-
 from lektor.sourceobj import VirtualSourceObject
 
 from lektorlib.recordcache import get_or_create_virtual
 
 
 class Test_get_or_create_virtual:
     @pytest.fixture
     def record(self, lektor_pad):
-        return lektor_pad.get('/about')
+        return lektor_pad.get("/about")
 
     @pytest.fixture
     def virtual_source(self, record):
-        return DummyVirtualSource(record, 'virtual/path')
+        return DummyVirtualSource(record, "virtual/path")
 
     def test_finds_cached_record(self, lektor_pad, record, virtual_source):
         lektor_pad.cache.remember(virtual_source)
 
         def creator():
             pytest.fail("should not be called")
-        rv = get_or_create_virtual(record, 'virtual/path', creator)
+
+        rv = get_or_create_virtual(record, "virtual/path", creator)
         assert rv is virtual_source
 
     def test_creates_record(self, record, virtual_source):
         def creator():
             creator.calls.append(())
             return virtual_source
+
         creator.calls = []
 
-        for n in range(2):
-            rv = get_or_create_virtual(record, 'virtual/path', creator)
+        for _n in range(2):
+            rv = get_or_create_virtual(record, "virtual/path", creator)
             assert rv is virtual_source
         assert creator.calls == [()]
 
-    @pytest.mark.parametrize('persist', [True, False])
+    @pytest.mark.parametrize("persist", [True, False])
     def test_persist(self, record, virtual_source, persist, lektor_pad):
         def creator():
             return virtual_source
-        get_or_create_virtual(record, 'virtual/path', creator,
-                              persist=persist)
+
+        get_or_create_virtual(record, "virtual/path", creator, persist=persist)
         if persist:
             assert virtual_source in lektor_pad.cache.persistent.values()
         else:
             assert virtual_source in lektor_pad.cache.ephemeral.values()
 
     def test_remembers_missing(self, record):
         def creator():
             creator.calls.append(())
             return None
+
         creator.calls = []
 
-        for n in range(2):
-            rv = get_or_create_virtual(record, 'virtual/path', creator)
+        for _n in range(2):
+            rv = get_or_create_virtual(record, "virtual/path", creator)
             assert rv is None
         assert creator.calls == [()]
 
 
 class DummyVirtualSource(VirtualSourceObject):
     def __init__(self, record, virtual_path):
         VirtualSourceObject.__init__(self, record)
```

### Comparing `lektorlib-1.1.0/tox.ini` & `lektorlib-1.2.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,62 @@
 [tox]
 minversion = 3.3
 isolated_build = true
-envlist = {py37,py38,py39,py310,py311}{,-lektor33},lint
+envlist =
+    py{37,38,39,310,311}{,-lektor33}
+    cover-{clean,report}
+    lint
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311, lint
 
 [testenv]
 deps =
+    coverage[toml]
     pytest
-    pytest-cov
     !lektor33: lektor>=3.4.0a1
     lektor33: lektor<3.4
-    
-setenv =
-    # Prevent parallel pytest-cov runs from clobbering each others .coverage file
-    COVERAGE_FILE = .coverage.{envname}
 commands =
-    pytest --cov=lektorlib --cov-report=term-missing --cov-report=html \
-        {posargs:--cov-fail-under=100 tests}
+    coverage run -m pytest {posargs:tests -ra}
+depends =
+    py{37,38,39,310,311}: cover-clean
+    cover-report: py{37,38,39,310,311}{,-lektor33}
 
 # workaround for pip cache contention under `tox p` with older pips
 download = true
 
 [testenv:lint]
 skip_install = True
 deps =
     build
-    flake8
     twine
 commands =
     python -m build --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
-    flake8 lektorlib tests
+
+[testenv:cover-clean]
+deps = coverage[toml]
+skip_install = true
+commands = coverage erase
+
+[testenv:cover-report]
+deps = coverage[toml]
+skip_install = true
+commands =
+    -coverage combine --append
+    coverage report --show-missing --fail-under=100
 
 [flake8]
+max-line-length = 88
+extend-ignore = E203
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs,
     # excludes other virtualenv lib and bin directories
     python*.*, bin
```

