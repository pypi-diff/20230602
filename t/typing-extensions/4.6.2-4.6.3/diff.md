# Comparing `tmp/typing_extensions-4.6.2.tar.gz` & `tmp/typing_extensions-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing_extensions-4.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "typing_extensions-4.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `typing_extensions-4.6.2.tar` & `typing_extensions-4.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10760 2023-05-25 13:13:20.271098 typing_extensions-4.6.2/CHANGELOG.md
--rw-r--r--   0        0        0    12787 2022-12-31 19:31:45.654412 typing_extensions-4.6.2/LICENSE
--rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.2/README.md
--rw-r--r--   0        0        0     1916 2023-05-25 13:13:20.271880 typing_extensions-4.6.2/pyproject.toml
--rw-r--r--   0        0        0      426 2022-12-31 19:31:45.655964 typing_extensions-4.6.2/src/_typed_dict_test_helper.py
--rw-r--r--   0        0        0   170054 2023-05-25 13:09:56.284393 typing_extensions-4.6.2/src/test_typing_extensions.py
--rw-r--r--   0        0        0   104592 2023-05-25 13:09:56.295773 typing_extensions-4.6.2/src/typing_extensions.py
--rw-r--r--   0        0        0      135 2023-05-22 00:37:39.060665 typing_extensions-4.6.2/tox.ini
--rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11557 2023-06-01 23:39:03.206669 typing_extensions-4.6.3/CHANGELOG.md
+-rw-r--r--   0        0        0    13936 2023-06-01 23:37:58.110406 typing_extensions-4.6.3/LICENSE
+-rw-r--r--   0        0        0     1290 2023-05-22 00:14:41.277524 typing_extensions-4.6.3/README.md
+-rw-r--r--   0        0        0     1916 2023-06-01 23:39:19.239989 typing_extensions-4.6.3/pyproject.toml
+-rw-r--r--   0        0        0      426 2023-05-27 00:24:46.431541 typing_extensions-4.6.3/src/_typed_dict_test_helper.py
+-rw-r--r--   0        0        0   174623 2023-06-01 23:37:58.216239 typing_extensions-4.6.3/src/test_typing_extensions.py
+-rw-r--r--   0        0        0   104335 2023-06-01 23:37:58.217871 typing_extensions-4.6.3/src/typing_extensions.py
+-rw-r--r--   0        0        0      135 2023-06-01 23:37:57.995967 typing_extensions-4.6.3/tox.ini
+-rw-r--r--   0        0        0     2786 1970-01-01 00:00:00.000000 typing_extensions-4.6.3/PKG-INFO
```

### Comparing `typing_extensions-4.6.2/CHANGELOG.md` & `typing_extensions-4.6.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+# Release 4.6.3 (June 1, 2023)
+
+- Fix a regression introduced in v4.6.0 in the implementation of
+  runtime-checkable protocols. The regression meant
+  that doing `class Foo(X, typing_extensions.Protocol)`, where `X` was a class that
+  had `abc.ABCMeta` as its metaclass, would then cause subsequent
+  `isinstance(1, X)` calls to erroneously raise `TypeError`. Patch by
+  Alex Waygood (backporting the CPython PR
+  https://github.com/python/cpython/pull/105152).
+- Sync the repository's LICENSE file with that of CPython.
+  `typing_extensions` is distributed under the same license as
+  CPython itself.
+- Skip a problematic test on Python 3.12.0b1. The test fails on 3.12.0b1 due to
+  a bug in CPython, which will be fixed in 3.12.0b2. The
+  `typing_extensions` test suite now passes on 3.12.0b1.
+
 # Release 4.6.2 (May 25, 2023)
 
 - Fix use of `@deprecated` on classes with `__new__` but no `__init__`.
   Patch by Jelle Zijlstra.
 - Fix regression in version 4.6.1 where comparing a generic class against a
   runtime-checkable protocol using `isinstance()` would cause `AttributeError`
   to be raised if using Python 3.7.
```

### Comparing `typing_extensions-4.6.2/LICENSE` & `typing_extensions-4.6.3/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 A. HISTORY OF THE SOFTWARE
 ==========================
 
 Python was created in the early 1990s by Guido van Rossum at Stichting
-Mathematisch Centrum (CWI, see http://www.cwi.nl) in the Netherlands
+Mathematisch Centrum (CWI, see https://www.cwi.nl) in the Netherlands
 as a successor of a language called ABC.  Guido remains Python's
 principal author, although it includes many contributions from others.
 
 In 1995, Guido continued his work on Python at the Corporation for
-National Research Initiatives (CNRI, see http://www.cnri.reston.va.us)
+National Research Initiatives (CNRI, see https://www.cnri.reston.va.us)
 in Reston, Virginia where he released several versions of the
 software.
 
 In May 2000, Guido and the Python core development team moved to
 BeOpen.com to form the BeOpen PythonLabs team.  In October of the same
 year, the PythonLabs team moved to Digital Creations, which became
 Zope Corporation.  In 2001, the Python Software Foundation (PSF, see
 https://www.python.org/psf/) was formed, a non-profit organization
 created specifically to own Python-related Intellectual Property.
 Zope Corporation was a sponsoring member of the PSF.
 
-All Python releases are Open Source (see http://www.opensource.org for
+All Python releases are Open Source (see https://opensource.org for
 the Open Source Definition).  Historically, most, but not all, Python
 releases have also been GPL-compatible; the table below summarizes
 the various releases.
 
     Release         Derived     Year        Owner       GPL-
                     from                                compatible? (1)
 
@@ -55,29 +55,40 @@
 Thanks to the many outside volunteers who have worked under Guido's
 direction to make these releases possible.
 
 
 B. TERMS AND CONDITIONS FOR ACCESSING OR OTHERWISE USING PYTHON
 ===============================================================
 
+Python software and documentation are licensed under the
+Python Software Foundation License Version 2.
+
+Starting with Python 3.8.6, examples, recipes, and other code in
+the documentation are dual licensed under the PSF License Version 2
+and the Zero-Clause BSD license.
+
+Some software incorporated into Python is under different licenses.
+The licenses are listed with code falling under that license.
+
+
 PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
 --------------------------------------------
 
 1. This LICENSE AGREEMENT is between the Python Software Foundation
 ("PSF"), and the Individual or Organization ("Licensee") accessing and
 otherwise using this software ("Python") in source or binary form and
 its associated documentation.
 
 2. Subject to the terms and conditions of this License Agreement, PSF hereby
 grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce,
 analyze, test, perform and/or display publicly, prepare derivative works,
 distribute, and otherwise use Python alone or in any derivative version,
 provided, however, that PSF's License Agreement and PSF's notice of copyright,
 i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
-2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022 Python Software Foundation;
+2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023 Python Software Foundation;
 All Rights Reserved" are retained in Python alone or in any derivative version
 prepared by Licensee.
 
 3. In the event Licensee prepares a derivative work that is based on
 or incorporates Python or any part thereof, and wants to make
 the derivative work available to others as provided herein, then
 Licensee hereby agrees to include in any such work a brief summary of
@@ -248,7 +259,21 @@
 STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO
 THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
 FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE
 FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
 OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+
+ZERO-CLAUSE BSD LICENSE FOR CODE IN THE PYTHON DOCUMENTATION
+----------------------------------------------------------------------
+
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
+AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `typing_extensions-4.6.2/README.md` & `typing_extensions-4.6.3/README.md`

 * *Files identical despite different names*

### Comparing `typing_extensions-4.6.2/pyproject.toml` & `typing_extensions-4.6.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["flit_core >=3.4,<4"]
 build-backend = "flit_core.buildapi"
 
 # Project metadata
 [project]
 name = "typing_extensions"
-version = "4.6.2"
+version = "4.6.3"
 description = "Backported and Experimental Type Hints for Python 3.7+"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = [
     "annotations",
     "backport",
```

### Comparing `typing_extensions-4.6.2/src/test_typing_extensions.py` & `typing_extensions-4.6.3/src/test_typing_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1692,14 +1692,20 @@
         return 0
 
 class NT(NamedTuple):
     x: int
     y: int
 
 
+skip_if_py312b1 = skipIf(
+    sys.version_info == (3, 12, 0, 'beta', 1),
+    "CPython had bugs in 3.12.0b1"
+)
+
+
 class ProtocolTests(BaseTestCase):
     def test_runtime_alias(self):
         self.assertIs(runtime, runtime_checkable)
 
     def test_basic_protocol(self):
         @runtime_checkable
         class P(Protocol):
@@ -1892,48 +1898,83 @@
         class BadPG(Protocol[T]):
             def x(self): ...
         class C:
             def x(self): ...
         self.assertIsSubclass(C, P)
         self.assertIsSubclass(C, PG)
         self.assertIsSubclass(BadP, PG)
-        with self.assertRaises(TypeError):
+
+        no_subscripted_generics = (
+            "Subscripted generics cannot be used with class and instance checks"
+        )
+
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             issubclass(C, PG[T])
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             issubclass(C, PG[C])
-        with self.assertRaises(TypeError):
+
+        only_runtime_checkable_protocols = (
+            "Instance and class checks can only be used with "
+            "@runtime_checkable protocols"
+        )
+
+        with self.assertRaisesRegex(TypeError, only_runtime_checkable_protocols):
             issubclass(C, BadP)
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, only_runtime_checkable_protocols):
             issubclass(C, BadPG)
-        with self.assertRaises(TypeError):
+
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             issubclass(P, PG[T])
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             issubclass(PG, PG[int])
 
+        only_classes_allowed = r"issubclass\(\) arg 1 must be a class"
+
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(1, P)
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(1, PG)
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(1, BadP)
+        with self.assertRaisesRegex(TypeError, only_classes_allowed):
+            issubclass(1, BadPG)
+
     def test_protocols_issubclass_non_callable(self):
         class C:
             x = 1
+
         @runtime_checkable
         class PNonCall(Protocol):
             x = 1
-        with self.assertRaises(TypeError):
+
+        non_callable_members_illegal = (
+            "Protocols with non-method members don't support issubclass()"
+        )
+
+        with self.assertRaisesRegex(TypeError, non_callable_members_illegal):
             issubclass(C, PNonCall)
+
         self.assertIsInstance(C(), PNonCall)
         PNonCall.register(C)
-        with self.assertRaises(TypeError):
+
+        with self.assertRaisesRegex(TypeError, non_callable_members_illegal):
             issubclass(C, PNonCall)
+
         self.assertIsInstance(C(), PNonCall)
+
         # check that non-protocol subclasses are not affected
         class D(PNonCall): ...
+
         self.assertNotIsSubclass(C, D)
         self.assertNotIsInstance(C(), D)
         D.register(C)
         self.assertIsSubclass(C, D)
         self.assertIsInstance(C(), D)
-        with self.assertRaises(TypeError):
+
+        with self.assertRaisesRegex(TypeError, non_callable_members_illegal):
             issubclass(D, PNonCall)
 
     def test_no_weird_caching_with_issubclass_after_isinstance(self):
         @runtime_checkable
         class Spam(Protocol):
             x: int
 
@@ -1944,15 +1985,18 @@
         self.assertIsInstance(Eggs(), Spam)
 
         # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
         # TypeError wouldn't be raised here,
         # as the cached result of the isinstance() check immediately above
         # would mean the issubclass() call would short-circuit
         # before we got to the "raise TypeError" line
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(
+            TypeError,
+            "Protocols with non-method members don't support issubclass()"
+        ):
             issubclass(Eggs, Spam)
 
     def test_no_weird_caching_with_issubclass_after_isinstance_2(self):
         @runtime_checkable
         class Spam(Protocol):
             x: int
 
@@ -1961,15 +2005,18 @@
         self.assertNotIsInstance(Eggs(), Spam)
 
         # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
         # TypeError wouldn't be raised here,
         # as the cached result of the isinstance() check immediately above
         # would mean the issubclass() call would short-circuit
         # before we got to the "raise TypeError" line
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(
+            TypeError,
+            "Protocols with non-method members don't support issubclass()"
+        ):
             issubclass(Eggs, Spam)
 
     def test_no_weird_caching_with_issubclass_after_isinstance_3(self):
         @runtime_checkable
         class Spam(Protocol):
             x: int
 
@@ -1982,15 +2029,18 @@
         self.assertNotIsInstance(Eggs(), Spam)
 
         # gh-104555: If we didn't override ABCMeta.__subclasscheck__ in _ProtocolMeta,
         # TypeError wouldn't be raised here,
         # as the cached result of the isinstance() check immediately above
         # would mean the issubclass() call would short-circuit
         # before we got to the "raise TypeError" line
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(
+            TypeError,
+            "Protocols with non-method members don't support issubclass()"
+        ):
             issubclass(Eggs, Spam)
 
     def test_protocols_isinstance(self):
         T = TypeVar('T')
         @runtime_checkable
         class P(Protocol):
             def meth(x): ...
@@ -2018,21 +2068,32 @@
         class C2:
             def __init__(self):
                 self.meth = lambda: None
         for klass in C, C2:
             for proto in P, PG, WeirdProto, WeirdProto2, WeirderProto:
                 with self.subTest(klass=klass.__name__, proto=proto.__name__):
                     self.assertIsInstance(klass(), proto)
-        with self.assertRaises(TypeError):
+
+        no_subscripted_generics = (
+            "Subscripted generics cannot be used with class and instance checks"
+        )
+
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             isinstance(C(), PG[T])
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, no_subscripted_generics):
             isinstance(C(), PG[C])
-        with self.assertRaises(TypeError):
+
+        only_runtime_checkable_msg = (
+            "Instance and class checks can only be used "
+            "with @runtime_checkable protocols"
+        )
+
+        with self.assertRaisesRegex(TypeError, only_runtime_checkable_msg):
             isinstance(C(), BadP)
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, only_runtime_checkable_msg):
             isinstance(C(), BadPG)
 
     def test_protocols_isinstance_properties_and_descriptors(self):
         class C:
             @property
             def attr(self):
                 return 42
@@ -2263,14 +2324,64 @@
         f = Foo()
         self.assertNotIsInstance(f, HasX)
         f.x = 42
         self.assertIsInstance(f, HasX)
         del f.x
         self.assertNotIsInstance(f, HasX)
 
+    @skip_if_py312b1
+    def test_runtime_checkable_generic_non_protocol(self):
+        # Make sure this doesn't raise AttributeError
+        with self.assertRaisesRegex(
+            TypeError,
+            "@runtime_checkable can be only applied to protocol classes",
+        ):
+            @runtime_checkable
+            class Foo(Generic[T]): ...
+
+    def test_runtime_checkable_generic(self):
+        @runtime_checkable
+        class Foo(Protocol[T]):
+            def meth(self) -> T: ...
+
+        class Impl:
+            def meth(self) -> int: ...
+
+        self.assertIsSubclass(Impl, Foo)
+
+        class NotImpl:
+            def method(self) -> int: ...
+
+        self.assertNotIsSubclass(NotImpl, Foo)
+
+    if sys.version_info >= (3, 12):
+        exec(textwrap.dedent(
+            """
+            @skip_if_py312b1
+            def test_pep695_generics_can_be_runtime_checkable(self):
+                @runtime_checkable
+                class HasX(Protocol):
+                    x: int
+
+                class Bar[T]:
+                    x: T
+                    def __init__(self, x):
+                        self.x = x
+
+                class Capybara[T]:
+                    y: str
+                    def __init__(self, y):
+                        self.y = y
+
+                self.assertIsInstance(Bar(1), HasX)
+                self.assertNotIsInstance(Capybara('a'), HasX)
+                """
+        ))
+
+    @skip_if_py312b1
     def test_protocols_isinstance_generic_classes(self):
         T = TypeVar("T")
 
         class Foo(Generic[T]):
             x: T
 
             def __init__(self, x):
@@ -2375,20 +2486,21 @@
             def __subclasshook__(cls, other):
                 return other.__name__.startswith("OK")
         self.assertIsInstance(OKClass(), C)
         self.assertNotIsInstance(BadClass(), C)
         self.assertIsSubclass(OKClass, C)
         self.assertNotIsSubclass(BadClass, C)
 
+    @skip_if_py312b1
     def test_issubclass_fails_correctly(self):
         @runtime_checkable
         class P(Protocol):
             x = 1
         class C: pass
-        with self.assertRaises(TypeError):
+        with self.assertRaisesRegex(TypeError, r"issubclass\(\) arg 1 must be a class"):
             issubclass(C(), P)
 
     def test_defining_generic_protocols(self):
         T = TypeVar('T')
         S = TypeVar('S')
         @runtime_checkable
         class PR(Protocol[T, S]):
@@ -2708,14 +2820,38 @@
         self.assertEqual(X.__parameters__, (T, T2))
         self.assertEqual(X.__args__, (int, T, T2))
 
         Y = X[bytes, memoryview]
         self.assertEqual(Y.__parameters__, ())
         self.assertEqual(Y.__args__, (int, bytes, memoryview))
 
+    @skip_if_py312b1
+    def test_interaction_with_isinstance_checks_on_superclasses_with_ABCMeta(self):
+        # Ensure the cache is empty, or this test won't work correctly
+        collections.abc.Sized._abc_registry_clear()
+
+        class Foo(collections.abc.Sized, Protocol): pass
+
+        # CPython gh-105144: this previously raised TypeError
+        # if a Protocol subclass of Sized had been created
+        # before any isinstance() checks against Sized
+        self.assertNotIsInstance(1, collections.abc.Sized)
+
+    @skip_if_py312b1
+    def test_interaction_with_isinstance_checks_on_superclasses_with_ABCMeta_2(self):
+        # Ensure the cache is empty, or this test won't work correctly
+        collections.abc.Sized._abc_registry_clear()
+
+        class Foo(typing.Sized, Protocol): pass
+
+        # CPython gh-105144: this previously raised TypeError
+        # if a Protocol subclass of Sized had been created
+        # before any isinstance() checks against Sized
+        self.assertNotIsInstance(1, typing.Sized)
+
 
 class Point2DGeneric(Generic[T], TypedDict):
     a: T
     b: T
 
 
 class Bar(Foo):
```

### Comparing `typing_extensions-4.6.2/src/typing_extensions.py` & `typing_extensions-4.6.3/src/typing_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -543,15 +543,15 @@
 
 # The performance of runtime-checkable protocols is significantly improved on Python 3.12,
 # so we backport the 3.12 version of Protocol to Python <=3.11
 if sys.version_info >= (3, 12):
     Protocol = typing.Protocol
     runtime_checkable = typing.runtime_checkable
 else:
-    def _allow_reckless_class_checks(depth=4):
+    def _allow_reckless_class_checks(depth=3):
         """Allow instance and class checks for special stdlib modules.
         The abc and functools modules indiscriminately call isinstance() and
         issubclass() on the whole MRO of a user class, which may contain protocols.
         """
         return _caller(depth) in {'abc', 'functools', None}
 
     def _no_init(self, *args, **kwargs):
@@ -568,34 +568,42 @@
                 # PEP 544 prohibits using issubclass()
                 # with protocols that have non-method members.
                 cls.__callable_proto_members_only__ = all(
                     callable(getattr(cls, attr, None)) for attr in cls.__protocol_attrs__
                 )
 
         def __subclasscheck__(cls, other):
+            if not isinstance(other, type):
+                # Same error message as for issubclass(1, int).
+                raise TypeError('issubclass() arg 1 must be a class')
             if (
                 getattr(cls, '_is_protocol', False)
-                and not cls.__callable_proto_members_only__
-                and not _allow_reckless_class_checks(depth=3)
+                and not _allow_reckless_class_checks()
             ):
-                raise TypeError(
-                    "Protocols with non-method members don't support issubclass()"
-                )
+                if not cls.__callable_proto_members_only__:
+                    raise TypeError(
+                        "Protocols with non-method members don't support issubclass()"
+                    )
+                if not getattr(cls, '_is_runtime_protocol', False):
+                    raise TypeError(
+                        "Instance and class checks can only be used with "
+                        "@runtime_checkable protocols"
+                    )
             return super().__subclasscheck__(other)
 
         def __instancecheck__(cls, instance):
             # We need this method for situations where attributes are
             # assigned in __init__.
             if not getattr(cls, "_is_protocol", False):
                 # i.e., it's a concrete subclass of a protocol
                 return super().__instancecheck__(instance)
 
             if (
                 not getattr(cls, '_is_runtime_protocol', False) and
-                not _allow_reckless_class_checks(depth=2)
+                not _allow_reckless_class_checks()
             ):
                 raise TypeError("Instance and class checks can only be used with"
                                 " @runtime_checkable protocols")
 
             if super().__instancecheck__(instance):
                 return True
 
@@ -628,42 +636,28 @@
             return type.__hash__(cls)
 
     @classmethod
     def _proto_hook(cls, other):
         if not cls.__dict__.get('_is_protocol', False):
             return NotImplemented
 
-        # First, perform various sanity checks.
-        if not getattr(cls, '_is_runtime_protocol', False):
-            if _allow_reckless_class_checks():
-                return NotImplemented
-            raise TypeError("Instance and class checks can only be used with"
-                            " @runtime_checkable protocols")
-
-        if not isinstance(other, type):
-            # Same error message as for issubclass(1, int).
-            raise TypeError('issubclass() arg 1 must be a class')
-
-        # Second, perform the actual structural compatibility check.
         for attr in cls.__protocol_attrs__:
             for base in other.__mro__:
                 # Check if the members appears in the class dictionary...
                 if attr in base.__dict__:
                     if base.__dict__[attr] is None:
                         return NotImplemented
                     break
 
                 # ...or in annotations, if it is a sub-protocol.
                 annotations = getattr(base, '__annotations__', {})
                 if (
                     isinstance(annotations, collections.abc.Mapping)
                     and attr in annotations
                     and issubclass(other, (typing.Generic, _ProtocolMeta))
-                    # All subclasses of Generic have an _is_proto attribute on 3.8+
-                    # But not on 3.7
                     and getattr(other, "_is_protocol", False)
                 ):
                     break
             else:
                 return NotImplemented
         return True
```

### Comparing `typing_extensions-4.6.2/PKG-INFO` & `typing_extensions-4.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing_extensions
-Version: 4.6.2
+Version: 4.6.3
 Summary: Backported and Experimental Type Hints for Python 3.7+
 Keywords: annotations,backport,checker,checking,function,hinting,hints,type,typechecking,typehinting,typehints,typing
 Author-email: "Guido van Rossum, Jukka Lehtosalo, Łukasz Langa, Michael Lee" <levkivskyi@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

