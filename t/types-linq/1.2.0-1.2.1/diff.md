# Comparing `tmp/types-linq-1.2.0.tar.gz` & `tmp/types-linq-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-linq-1.2.0.tar", last modified: Tue Mar  1 04:16:28 2022, max compression
+gzip compressed data, was "types-linq-1.2.1.tar", last modified: Fri Jun  2 20:40:52 2023, max compression
```

## Comparing `types-linq-1.2.0.tar` & `types-linq-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 04:16:28.374347 types-linq-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-03-01 04:16:14.000000 types-linq-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-03-01 04:16:28.370347 types-linq-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-03-01 04:16:14.000000 types-linq-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-01 04:16:28.374347 types-linq-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-03-01 04:16:14.000000 types-linq-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 04:16:28.370347 types-linq-1.2.0/types_linq/
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2653 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/cached_enumerable.py
--rw-r--r--   0 runner    (1001) docker     (121)    34275 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/enumerable.py
--rw-r--r--   0 runner    (1001) docker     (121)    63972 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/enumerable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/grouping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 04:16:28.370347 types-linq-1.2.0/types_linq/more/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5316 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more/extrema_enumerable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more/extrema_enumerable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11610 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more/more_enumerable.py
--rw-r--r--   0 runner    (1001) docker     (121)    19438 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more/more_enumerable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/more_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2999 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/ordered_enumerable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/ordered_enumerable.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/types_linq_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     4738 2022-03-01 04:16:14.000000 types-linq-1.2.0/types_linq/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 04:16:28.370347 types-linq-1.2.0/types_linq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-01 04:16:28.000000 types-linq-1.2.0/types_linq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:40:52.030966 types-linq-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-02 20:40:35.000000 types-linq-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-02 20:40:52.030966 types-linq-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-02 20:40:35.000000 types-linq-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 20:40:52.030966 types-linq-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-02 20:40:35.000000 types-linq-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:40:52.030966 types-linq-1.2.1/types_linq/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/cached_enumerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34275 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/enumerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62237 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/enumerable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:40:52.030966 types-linq-1.2.1/types_linq/more/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/extrema_enumerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/extrema_enumerable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/more_enumerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23105 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/more_enumerable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/more_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more/more_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/more_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/ordered_enumerable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/ordered_enumerable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/types_linq_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-02 20:40:35.000000 types-linq-1.2.1/types_linq/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 20:40:52.030966 types-linq-1.2.1/types_linq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-02 20:40:51.000000 types-linq-1.2.1/types_linq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-02 20:40:52.000000 types-linq-1.2.1/types_linq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:40:51.000000 types-linq-1.2.1/types_linq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 20:40:51.000000 types-linq-1.2.1/types_linq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 20:40:51.000000 types-linq-1.2.1/types_linq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 20:40:51.000000 types-linq-1.2.1/types_linq.egg-info/top_level.txt
```

### Comparing `types-linq-1.2.0/LICENSE` & `types-linq-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-linq-1.2.0/PKG-INFO` & `types-linq-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-linq
-Version: 1.2.0
+Version: 1.2.1
 Summary: Standard sequence helper methods with full typing support
 Home-page: https://github.com/cleoold/types-linq
 Author: cleoold
 License: BSD 2-Clause License
 Description: # types-linq
         
         ![Python](https://img.shields.io/badge/python-3.7%2B-blue.svg) [![pypi](https://img.shields.io/pypi/v/types-linq)](https://pypi.org/project/types-linq/) [![pytest](https://github.com/cleoold/types-linq/workflows/pytest/badge.svg)](https://github.com/cleoold/types-linq/actions?query=workflow%3Apytest) [![codecov](https://codecov.io/gh/cleoold/types-linq/branch/main/graph/badge.svg?token=HTUKZ0SQJ3)](https://codecov.io/gh/cleoold/types-linq) [![Documentation Status](https://readthedocs.org/projects/types-linq/badge/?version=latest)](https://types-linq.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `types-linq-1.2.0/README.md` & `types-linq-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `types-linq-1.2.0/setup.py` & `types-linq-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='types-linq',
-    version='v1.2.0',
+    version='v1.2.1',
     url='https://github.com/cleoold/types-linq',
     license='BSD 2-Clause License',
     author='cleoold',
     description='Standard sequence helper methods with full typing support',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['types_linq', 'types_linq.more'],
```

### Comparing `types-linq-1.2.0/types_linq/cached_enumerable.py` & `types-linq-1.2.1/types_linq/cached_enumerable.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from .more_typing import (
     TSource_co,
 )
 
 
 class CachedEnumerable(Enumerable[TSource_co]):
     '''
-    .. code-block:: python
-
-        from types_linq.cached_enumerable import CachedEnumerable
+    ```py
+    from types_linq.cached_enumerable import CachedEnumerable
+    ```
 
     Enumerable that stores the enumerated results which can be accessed repeatedly.
 
-    Users should not construct instances of this class directly. Use ``Enumerable.as_cached()`` instead.
+    Users should not construct instances of this class directly. Use `Enumerable.as_cached()` instead.
 
-    Revisions:
-        - v0.1.1: New.
+    Revisions
+        ~ v0.1.1: New.
     '''
 
     _iter: Iterator[TSource_co]
     _cache_capacity: Optional[int]
     _enumerated_values: Dict[int, TSource_co]
     _min_index: int
     _tracked: int
@@ -47,14 +47,17 @@
                 res = self._enumerated_values[i]
                 i += 1
                 yield res
             try:
                 res = next(self._iter)
             except StopIteration:
                 break
+            if self._cache_capacity == 0:
+                yield res
+                continue
             len_ = len(self._enumerated_values)
             if self._cache_capacity is not None and \
                 len_ > 0 and len_ == self._cache_capacity:
                 del self._enumerated_values[self._min_index]
                 self._min_index += 1
             self._enumerated_values[self._tracked] = res
             self._tracked += 1
```

### Comparing `types-linq-1.2.0/types_linq/enumerable.py` & `types-linq-1.2.1/types_linq/enumerable.py`

 * *Files identical despite different names*

### Comparing `types-linq-1.2.0/types_linq/enumerable.pyi` & `types-linq-1.2.1/types_linq/enumerable.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     TSupportsLessThan,
     TValue,
 )
 
 
 class Enumerable(Sequence[TSource_co], Generic[TSource_co]):
     '''
-    .. code-block:: python
-
-        from types_linq import Enumerable
+    ```py
+    from types_linq import Enumerable
+    ```
 
     Provides a set of helper methods for querying iterable objects.
     '''
 
     @overload
     def __init__(self, __iterable: Iterable[TSource_co]) -> None:
         '''
@@ -50,120 +50,125 @@
 
     def __contains__(self, value: object) -> bool:
         '''
         Tests whether the sequence contains the specified element. Prefers calling `__contains__()`
         on the wrapped iterable if available, otherwise, calls `self.contains()`.
 
         Example
-            >>> en = Enumerable([1, 10, 100])
-            >>> 1000 in en
-            False
+        ```py
+        >>> en = Enumerable([1, 10, 100])
+        >>> 1000 in en
+        False
+        ```
         '''
 
     @overload
     def __getitem__(self, index: int) -> TSource_co:
         '''
         Returns the element at specified index in the sequence. Prefers calling `__getitem__()` on the
         wrapped iterable if available, otherwise, calls `self.element_at()`.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen())[1]
-                10
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen())[1]
+        10
+        ```
         '''
 
     @overload
     def __getitem__(self, __index_and_default: Tuple[int, TDefault]) -> Union[TSource_co, TDefault]:
         '''
         Returns the element at specified index in the sequence or returns the default value if it does not
         exist. Prefers calling `__getitem__()` on the wrapped iterable if available, otherwise, calls
         `self.element_at()`.
 
         Example
-            .. code-block:: python
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen())[3, 1000]
+        1000
+        ```
 
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen())[3, 1000]
-                1000
-
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     @overload
     def __getitem__(self, index: slice) -> Enumerable[TSource_co]:
         '''
         Produces a subsequence defined by the given slice notation. Prefers calling `__getitem__()` on the
         wrapped iterable if available, otherwise, calls `self.elements_in()`.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
-
-                >>> Enumerable(gen())[1:3].to_list()
-                [10, 100]
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
+
+        >>> Enumerable(gen())[1:3].to_list()
+        [10, 100]
+        ```
         '''
 
     def __iter__(self) -> Iterator[TSource_co]:
         '''
         Returns an iterator that enumerates the values in the sequence.
 
         Example
-
-        .. code-block:: python
-
-            def gen():
-                print('working...')
-                yield 1; yield 10; yield 100
-
-            query = Enumerable(gen()).select(lambda e: e * 1000)
-            print('go!')
-            for e in query:
-                print(e)
-
-            # output:
-            # go!
-            # working...
-            # 1000
-            # 10000
-            # 100000
+        ```py
+        def gen():
+            print('working...')
+            yield 1; yield 10; yield 100
+
+        query = Enumerable(gen()).select(lambda e: e * 1000)
+        print('go!')
+        for e in query:
+            print(e)
+
+        # output:
+        # go!
+        # working...
+        # 1000
+        # 10000
+        # 100000
+        ```
         '''
 
     def __len__(self) -> int:
         '''
         Returns the number of elements in the sequence. Prefers calling `__len__()` on the wrapped iterable
         if available, otherwise, calls `self.count()`.
 
         Example
-            >>> en = Enumerable([1, 10, 100])
-            >>> len(en)
-            3
+        ```py
+        >>> en = Enumerable([1, 10, 100])
+        >>> len(en)
+        3
+        ```
         '''
 
     def __reversed__(self) -> Iterator[TSource_co]:
         '''
         Inverts the order of the elements in the sequence. Prefers calling `__reversed__()` on the wrapped
         iterable if available, otherwise, calls `self.reverse()`.
 
         Example
-            >>> ints = [1, 10, 100]
-            >>> en = Enumerable(ints)
-            >>> for e in reversed(en):
-            ...     print(e)
-            100
-            10
-            1
+        ```py
+        >>> ints = [1, 10, 100]
+        >>> en = Enumerable(ints)
+        >>> for e in reversed(en):
+        ...     print(e)
+        100
+        10
+        1
+        ```
         '''
 
     @staticmethod
     def _raise_empty_sequence() -> NoReturn: ...  # internal
 
     @overload
     def aggregate(self,
@@ -172,377 +177,400 @@
         __result_selector: Callable[[TAccumulate], TResult],
     ) -> TResult:
         '''
         Applies an accumulator function over the sequence. The seed is used as the initial
         accumulator value, and the result_selector is used to select the result value.
 
         Example
-            >>> fruits = ['apple', 'mango', 'orange', 'passionfruit', 'grape']
-            >>> Enumerable(fruits).aggregate('banana', lambda acc, e: e if len(e) > len(acc) else acc, str.upper)
-            'PASSIONFRUIT'
+        ```py
+        >>> fruits = ['apple', 'mango', 'orange', 'passionfruit', 'grape']
+        >>> Enumerable(fruits).aggregate('banana', lambda acc, e: e if len(e) > len(acc) else acc, str.upper)
+        'PASSIONFRUIT'
+        ```
         '''
 
     @overload
     def aggregate(self,
         __seed: TAccumulate,
         __func: Callable[[TAccumulate, TSource_co], TAccumulate],
     ) -> TAccumulate:
         '''
         Applies an accumulator function over the sequence. The seed is used as the initial
-        accumulator value
+        accumulator value.
 
         Example
-            >>> words = 'the quick brown fox jumps over the lazy dog'.split(' ')
-            >>> Enumerable(words).aggregate('end', lambda acc, e: f'{e} {acc}')
-            'dog lazy the over jumps fox brown quick the end'
+        ```py
+        >>> words = 'the quick brown fox jumps over the lazy dog'.split(' ')
+        >>> Enumerable(words).aggregate('end', lambda acc, e: f'{e} {acc}')
+        'dog lazy the over jumps fox brown quick the end'
+        ```
         '''
 
     @overload
     def aggregate(self,
         __func: Callable[[TSource_co, TSource_co], TSource_co],
     ) -> TSource_co:
         '''
         Applies an accumulator function over the sequence. Raises `InvalidOperationError` if
         there is no value in the sequence.
 
         Example
-            >>> words = 'the quick brown fox jumps over the lazy dog'.split(' ')
-            >>> Enumerable(words).aggregate(lambda acc, e: f'{e} {acc}')
-            'dog lazy the over jumps fox brown quick the'
+        ```py
+        >>> words = 'the quick brown fox jumps over the lazy dog'.split(' ')
+        >>> Enumerable(words).aggregate(lambda acc, e: f'{e} {acc}')
+        'dog lazy the over jumps fox brown quick the'
+        ```
 
         Example
-            >>> Enumerable.range(1, 10).aggregate(lambda acc, e: acc * e)
-            3628800
+        ```py
+        >>> Enumerable.range(1, 10).aggregate(lambda acc, e: acc * e)
+        3628800
+        ```
 
-        Revisions:
-            - v1.2.0: Fixed annotation for __func.
+        Revisions
+            ~ v1.2.0: Fixed annotation for __func.
         '''
 
     def all(self, predicate: Callable[[TSource_co], bool]) -> bool:
         '''
         Tests whether all elements of the sequence satisfy a condition.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).all(lambda e: e % 2 == 1)
-            True
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).all(lambda e: e % 2 == 1)
+        True
+        ```
         '''
 
     @overload
     def any(self) -> bool:
         '''
         Tests whether the sequence has any elements.
 
         Example
-            >>> Enumerable([]).any()
-            False
-            >>> Enumerable([1]).any()
-            True
+        ```py
+        >>> Enumerable([]).any()
+        False
+        >>> Enumerable([1]).any()
+        True
+        ```
         '''
 
     @overload
     def any(self, __predicate: Callable[[TSource_co], bool]) -> bool:
         '''
         Tests whether any element of the sequence satisfy a condition.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).any(lambda e: e % 2 == 0)
-            False
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).any(lambda e: e % 2 == 0)
+        False
+        ```
         '''
 
     def append(self, element: TSource_co) -> Enumerable[TSource_co]:  # type: ignore
         '''
         Appends a value to the end of the sequence. Again, this does not affect the original wrapped
         object.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).append(11).to_list()
-            [1, 3, 5, 7, 9, 11]
-            >>> ints
-            [1, 3, 5, 7, 9]
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).append(11).to_list()
+        [1, 3, 5, 7, 9, 11]
+        >>> ints
+        [1, 3, 5, 7, 9]
+        ```
         '''
 
     def as_cached(self, *, cache_capacity: Optional[int] = None) -> CachedEnumerable[TSource_co]:
         '''
         Returns a CachedEnumerable to cache the enumerated results in this query so that if the wrapped
         iterable is not repeatable (e.g. generator object), it will be repeatable.
 
-        By default, ``Enumerable`` s constructed from nonrepeatable sources cannot be enumerated multiple
+        By default, `Enumerable`s constructed from nonrepeatable sources cannot be enumerated multiple
         times, for example
 
-        .. code-block:: python
+        ```py
+        def gen():
+            yield 1
+            yield 0
+            yield 3
+
+        query = Enumerable(gen())
+        print(query.count())
+        print(query.where(lambda x: x > 0).to_list())
+        ```
 
-            def gen():
-                yield 1
-                yield 0
-                yield 3
-
-            query = Enumerable(gen())
-            print(query.count())
-            print(query.where(lambda x: x > 0).to_list())
-
-        prints ``3`` followed by an empty list ``[]``. This is because the ``.count()`` exhausts the
+        prints `3` followed by an empty list `[]`. This is because the `.count()` exhausts the
         contents in the generator before the second query is run.
 
         To avoid the issue, use this method which saves the results along the way.
     
-        .. code-block:: python
-
-            query = Enumerable(gen()).as_cached()
-            print(query.count())
-            print(query.take(2).to_list())
-            print(query.where(lambda x: x > 0).to_list())
-
+        ```py
+        query = Enumerable(gen()).as_cached()
+        print(query.count())
+        print(query.take(2).to_list())
+        print(query.where(lambda x: x > 0).to_list())
+        ```
 
-        printing ``3``, ``[1, 0]`` and ``[1, 3]``.
+        printing `3`, `[1, 0]` and `[1, 3]`.
 
         This is an alternative way to deal with non-repeatable sources other than passing function
-        (``query = Enumerable(gen)``) or solidifying the source in advance
-        (``query = Enumerable(list(gen))``).
+        (`query = Enumerable(gen)`) or solidifying the source in advance
+        (`query = Enumerable(list(gen))`).
         This method is useless if you have constructed an Enumerable from a repeatable source such as
-        a builtin list, an iterable factory mentioned above, or other ``Enumerable``'s query methods.
+        a builtin list, an iterable factory mentioned above, or other `Enumerable`'s query methods.
 
         If cache_capacity is None, it is infinite.
 
         Raises `InvalidOperationError` if cache_capacity is negative.
 
-        The behavior of this method differs from that of ``CachedEnumerable``.
+        The behavior of this method differs from that of `CachedEnumerable`.
 
-        Revisions:
-            - v0.1.1: New.
+        Revisions
+            ~ v0.1.1: New.
         '''
 
     def as_more(self) -> MoreEnumerable[TSource_co]:
         '''
         Returns a MoreEnumerable that has more non-standard query methods available.
 
         Example
-            >>> Enumerable([1, 2, 3]).as_more()
+        ```py
+        >>> Enumerable([1, 2, 3]).as_more()
+        ```
 
-        Revisions:
-            - v0.2.0: New.
+        Revisions
+            ~ v0.2.0: New.
         '''
 
     @overload
     def average(self: Enumerable[SupportsAverage[TResult]]) -> TResult:
         '''
         Computes the average value of the sequence. Raises `InvalidOperationError` if there
         is no value.
 
-        The returned type is the type of the expression
-        `(elem1 + elem2 + ...) / cast(int, ...)`.
-
         Example
-            >>> ints = [1, 3, 5, 9, 11]
-            >>> Enumerable(ints).average()
-            5.8
+        ```py
+        >>> ints = [1, 3, 5, 9, 11]
+        >>> Enumerable(ints).average()
+        5.8
+        ```
         '''
 
     @overload
     def average(self, __selector: Callable[[TSource_co], SupportsAverage[TResult]]) -> TResult:
         '''
         Computes the average value of the sequence using the selector. Raises
         `InvalidOperationError` if there is no value.
 
-        The returned type is the type of the expression
-        `(selector(elem1) + selector(elem2) + ...) / cast(int, ...)`.
-
         Example
-            >>> strs = ['1', '3', '5', '9', '11']
-            >>> Enumerable(strs).average(lambda e: int(e) * 1000)
-            5800.0
+        ```py
+        >>> strs = ['1', '3', '5', '9', '11']
+        >>> Enumerable(strs).average(lambda e: int(e) * 1000)
+        5800.0
+        ```
         '''
 
     @overload
     def average2(self: Enumerable[SupportsAverage[TResult]],
         __default: TDefault,
     ) -> Union[TResult, TDefault]:
         '''
         Computes the average value of the sequence. Returns `default` if there is no value.
 
-        The returned type is the type of the expression
-        `(elem1 + elem2 + ...) / cast(int, ...)` or `TDefault`.
-
         Example
-            >>> Enumerable([1, 2]).average2(0)
-            1.5
-            >>> Enumerable([]).average2(0)
-            0
+        ```py
+        >>> Enumerable([1, 2]).average2(0)
+        1.5
+        >>> Enumerable([]).average2(0)
+        0
+        ```
         '''
 
     @overload
     def average2(self,
         __selector: Callable[[TSource_co], SupportsAverage[TResult]],
         __default: TDefault,
     ) -> Union[TResult, TDefault]:
         '''
         Computes the average value of the sequence using the selector. Returns `default` if there
         is no value.
 
-        The returned type is the type of the expression
-        `(selector(elem1) + selector(elem2) + ...) / cast(int, ...)` or `TDefault`.
-
         Example
-            >>> Enumerable([]).average2(lambda e: int(e) * 1000, 0)
-            0
+        ```py
+        >>> Enumerable([]).average2(lambda e: int(e) * 1000, 0)
+        0
+        ```
         '''
 
     def cast(self, __t_result: Type[TResult]) -> Enumerable[TResult]:
         '''
         Casts the elements to the specified type.
         
         This method does not change anything. It returns the original Enumerable reference unchanged.
 
         Example
-            .. code-block:: python
-
-                query: Enumerable[object] = ...
-                same_query: Enumerable[int] = query.cast(int)
+        ```py
+        query: Enumerable[object] = ...
+        same_query: Enumerable[int] = query.cast(int)
+        ```
         '''
 
     # nonstanard: .NET returns fix-size arrays as elements instead
     def chunk(self, size: int) -> Enumerable[MutableSequence[TSource_co]]:
         '''
         Splits the elements of a sequence into chunks of size at most the provided size. Raises
         `InvalidOperationError` if `size` is less than 1.
 
         Example
-            .. code-block:: python
-
-                >>> def source(i):
-                ...     while True:
-                ...         yield i
-                ...         i *= 3
-
-                >>> en = Enumerable(source(1)).chunk(4).take(3)
-                >>> for chunk in en:
-                ...     print(chunk)
-                [1, 3, 9, 27]
-                [81, 243, 729, 2187]
-                [6561, 19683, 59049, 177147]
+        ```py
+        >>> def source(i):
+        ...     while True:
+        ...         yield i
+        ...         i *= 3
+
+        >>> en = Enumerable(source(1)).chunk(4).take(3)
+        >>> for chunk in en:
+        ...     print(chunk)
+        [1, 3, 9, 27]
+        [81, 243, 729, 2187]
+        [6561, 19683, 59049, 177147]
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def concat(self, second: Iterable[TSource_co]) -> Enumerable[TSource_co]:
         '''
         Concatenates two sequences.
 
         Example
-            >>> en1 = Enumerable([1, 2, 3])
-            >>> en2 = Enumerable([1, 2, 4])
-            >>> en1.concat(en2).to_list()
-            [1, 2, 3, 1, 2, 4]
+        ```py
+        >>> en1 = Enumerable([1, 2, 3])
+        >>> en2 = Enumerable([1, 2, 4])
+        >>> en1.concat(en2).to_list()
+        [1, 2, 3, 1, 2, 4]
+        ```
         '''
 
     @overload
     def contains(self, value: object) -> bool:
         '''
         Tests whether the sequence contains the specified element using `==`.
 
         This method always uses a generic element-finding method (O(n)) regardless the implementation
         of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).contains(11)
-                False
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).contains(11)
+        False
+        ```
         '''
 
     @overload
     def contains(self, value: TOther, __comparer: Callable[[TSource_co, TOther], bool]) -> bool:
         '''
         Tests whether the sequence contains the specified element using the provided comparer that
         returns True if two values are equal.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).contains('9', lambda x, y: str(x) == y)
-            True
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).contains('9', lambda x, y: str(x) == y)
+        True
+        ```
         '''
 
     @overload
     def count(self) -> int:
         '''
         Returns the number of elements in the sequence.
 
         This method always uses a generic length-finding method (O(n)) regardless the implementation
         of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).count()
-                3
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).count()
+        3
+        ```
         '''
 
     @overload
     def count(self, __predicate: Callable[[TSource_co], bool]) -> int:
         '''
         Returns the number of elements that satisfy the condition.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).count(lambda e: e % 10 == 0)
-                2
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).count(lambda e: e % 10 == 0)
+        2
+        ```
         '''
 
     def default_if_empty(self,
         default: TDefault,
     ) -> Union[Enumerable[TSource_co], Enumerable[TDefault]]:
         '''
         Returns the elements of the sequence or the provided value in a singleton collection if
         the sequence is empty.
 
         Example
-            >>> Enumerable([]).default_if_empty(0).to_list()
-            [0]
-            >>> Enumerable([44, 45, 56]).default_if_empty(0).to_list()
-            [44, 45, 56]
+        ```py
+        >>> Enumerable([]).default_if_empty(0).to_list()
+        [0]
+        >>> Enumerable([44, 45, 56]).default_if_empty(0).to_list()
+        [44, 45, 56]
+        ```
         '''
 
     def distinct(self) -> Enumerable[TSource_co]:
         '''
         Returns distinct elements from the sequence.
 
         Example
-            >>> ints = [1, 4, 5, 6, 4, 3, 1, 99]
-            >>> Enumerable(ints).distinct().to_list()
-            [1, 4, 5, 6, 3, 99]
+        ```py
+        >>> ints = [1, 4, 5, 6, 4, 3, 1, 99]
+        >>> Enumerable(ints).distinct().to_list()
+        [1, 4, 5, 6, 3, 99]
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable values.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable values.
         '''
 
     def distinct_by(self, key_selector: Callable[[TSource_co], object]) -> Enumerable[TSource_co]:
         '''
         Returns distinct elements from the sequence where "distinctness" is determined by the value
         returned by the selector.
 
         Example
-            >>> ints = [1, 4, 5, 6, 4, 3, 1, 99]
-            >>> Enumerable(ints).distinct_by(lambda x: x // 2).to_list()
-            [1, 4, 6, 3, 99]
+        ```py
+        >>> ints = [1, 4, 5, 6, 4, 3, 1, 99]
+        >>> Enumerable(ints).distinct_by(lambda x: x // 2).to_list()
+        [1, 4, 6, 3, 99]
+        ```
 
-        Revisions:
-            - v1.0.0: New. The method with same name (but different return type) in MoreEnumerable class
+        Revisions
+            ~ v1.0.0: New. The method with same name (but different return type) in MoreEnumerable class
               was removed.
         '''
 
     @overload
     def element_at(self, index: int) -> TSource_co:
         '''
         Returns the element at specified index in the sequence. `IndexOutOfRangeError` is raised if
@@ -550,280 +578,290 @@
 
         If the index is negative, it means counting from the end.
 
         This method always uses a generic list element-finding method (O(n)) regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).element_at(1)
-                10
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).element_at(1)
+        10
+
+        >>> Enumerable(gen()).element_at(-1)
+        100
+        ```
 
-                >>> Enumerable(gen()).element_at(-1)
-                100
-
-        Revisions:
-            - v1.0.0: Added support for negative index.
+        Revisions
+            ~ v1.0.0: Added support for negative index.
         '''
 
     @overload
     def element_at(self, index: int, __default: TDefault) -> Union[TSource_co, TDefault]:
         '''
         Returns the element at specified index in the sequence. Default value is returned if no
         such element exists.
 
         If the index is negative, it means counting from the end.
 
         This method always uses a generic list element-finding method (O(n)) regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).element_at(3, 0)
+        0
+        ```
 
-                >>> Enumerable(gen()).element_at(3, 0)
-                0
-
-        Revisions:
-            - v1.0.0: Added support for negative index.
+        Revisions
+            ~ v1.0.0: Added support for negative index.
         '''
 
     @staticmethod
     def empty() -> Enumerable[TSource_co]:
         '''
         Returns an empty enumerable.
 
         Example
-            >>> en := Enumerable.empty()
-            <types_linq.enumerable.Enumerable at 0x00000000000>
-            >>> en.to_list()
-            []
+        ```py
+        >>> en := Enumerable.empty()
+        <types_linq.enumerable.Enumerable at 0x00000000000>
+        >>> en.to_list()
+        []
+        ```
         '''
 
     def except1(self, second: Iterable[TSource_co]) -> Enumerable[TSource_co]:
         '''
         Produces the set difference of two sequences: self - second.
 
-        Note ``except`` is a keyword in Python.
+        Note `except` is a keyword in Python.
 
         Example
-            >>> ints = [1, 2, 3, 4, 5]
-            >>> Enumerable(ints).except1([1, 3, 5, 7, 9]).to_list()
-            [2, 4]
+        ```py
+        >>> ints = [1, 2, 3, 4, 5]
+        >>> Enumerable(ints).except1([1, 3, 5, 7, 9]).to_list()
+        [2, 4]
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable values.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable values.
         '''
 
     def except_by(self,
         second: Iterable[TKey],
         key_selector: Callable[[TSource_co], TKey],
     ) -> Enumerable[TSource_co]:
         '''
         Produces the set difference of two sequences: self - second, according to a key selector that
         determines "distinctness".
 
         Example
-            >>> first = [(16, 'x'), (9, 'y'), (12, 'd'), (16, 't')]
-            >>> second = ['y', 'd']
-            >>> Enumerable(first).except_by(second, lambda x: x[1]).to_list()
-            [(16, 'x'), (16, 't')]
-
-        Revisions:
-            - v1.0.0: New. The method with same name (but different usage) in MoreEnumerable class was
-              renamed as ``except_by2()`` to accommodate this.
+        ```py
+        >>> first = [(16, 'x'), (9, 'y'), (12, 'd'), (16, 't')]
+        >>> second = ['y', 'd']
+        >>> Enumerable(first).except_by(second, lambda x: x[1]).to_list()
+        [(16, 'x'), (16, 't')]
+        ```
+
+        Revisions
+            ~ v1.0.0: New. The method with same name (but different usage) in MoreEnumerable class was
+              renamed as `except_by2()` to accommodate this.
         '''
 
     @overload
     def first(self) -> TSource_co:
         '''
         Returns the first element of the sequence. Raises `InvalidOperationError` if there is no
         first element.
 
         This method always uses a generic method to enumerate the first element regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).first()
-                1
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).first()
+        1
+        ```
         '''
 
     @overload
     def first(self, __predicate: Callable[[TSource_co], bool]) -> TSource_co:
         '''
         Returns the first element of the sequence that satisfies the condition. Raises
         `InvalidOperationError` if no such element exists.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9, 11, 13]
-            >>> Enumerable(ints).first(lambda e: e > 10)
-            11
+        ```py
+        >>> ints = [1, 3, 5, 7, 9, 11, 13]
+        >>> Enumerable(ints).first(lambda e: e > 10)
+        11
+        ```
         '''
 
     @overload
     def first2(self, __default: TDefault) -> Union[TSource_co, TDefault]:
         '''
         Returns the first element of the sequence or a default value if there is no such
         element.
 
         This method always uses a generic method to enumerate the first element regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen(ok: bool):
-                ...     if ok:
-                ...         yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen(True)).first2(0)
-                1
-                >>> Enumerable(gen(False)).first2(0)
-                0
+        ```py
+        >>> def gen(ok: bool):
+        ...     if ok:
+        ...         yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen(True)).first2(0)
+        1
+        >>> Enumerable(gen(False)).first2(0)
+        0
+        ```
         '''
 
     @overload
     def first2(self,
         __predicate: Callable[[TSource_co], bool],
         __default: TDefault,
     ) -> Union[TSource_co, TDefault]:
         '''
         Returns the first element of the sequence that satisfies the condition or a default value if
         no such element exists.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9, 11, 13]
-            >>> Enumerable(ints).first2(lambda e: e > 100, 100)
-            100
+        ```py
+        >>> ints = [1, 3, 5, 7, 9, 11, 13]
+        >>> Enumerable(ints).first2(lambda e: e > 100, 100)
+        100
+        ```
         '''
 
     @overload
     def group_by(self,
         key_selector: Callable[[TSource_co], TKey],
         value_selector: Callable[[TSource_co], TValue],
         __result_selector: Callable[[TKey, Enumerable[TValue]], TResult],
     ) -> Enumerable[TResult]:
         '''
         Groups the elements of the sequence according to specified key selector and value selector. Then
         it returns the result value using each grouping and its key.
 
         Example
-            .. code-block:: python
+        ```py
+        >>> pets_list = [
+        ...     ('Barley', 8.3), ('Boots', 4.9), ('Whiskers', 1.5), ('Daisy', 4.3),
+        ...     ('Roman', 8.6), ('Fangus', 8.6), ('Roam', 2.2), ('Roll', 1.4),
+        ... ]
+
+        >>> en = Enumerable(pets_list).group_by(
+        ...     lambda pet: math.floor(pet[1]),
+        ...     lambda pet: pet[0],
+        ...     lambda age_floored, names: (age_floored, names.to_set()),
+        ... )
+
+        >>> for obj in en:
+        ...     print(obj)
+        (8, {'Fangus', 'Roman', 'Barley'})
+        (4, {'Boots', 'Daisy'})
+        (1, {'Roll', 'Whiskers'})
+        (2, {'Roam'})
+        ```
 
-                >>> pets_list = [
-                ...     ('Barley', 8.3), ('Boots', 4.9), ('Whiskers', 1.5), ('Daisy', 4.3),
-                ...     ('Roman', 8.6), ('Fangus', 8.6), ('Roam', 2.2), ('Roll', 1.4),
-                ... ]
-
-                >>> en = Enumerable(pets_list).group_by(
-                ...     lambda pet: math.floor(pet[1]),
-                ...     lambda pet: pet[0],
-                ...     lambda age_floored, names: (age_floored, names.to_set()),
-                ... )
-
-                >>> for obj in en:
-                ...     print(obj)
-                (8, {'Fangus', 'Roman', 'Barley'})
-                (4, {'Boots', 'Daisy'})
-                (1, {'Roll', 'Whiskers'})
-                (2, {'Roam'})
-
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def group_by(self,
         key_selector: Callable[[TSource_co], TKey],
         value_selector: Callable[[TSource_co], TValue],
     ) -> Enumerable[Grouping[TKey, TValue]]:
         '''
         Groups the elements of the sequence according to specified key selector and value selector.
 
         Example
-            .. code-block:: python
-
-                >>> en = Enumerable(pets_list).group_by(
-                ...     lambda pet: math.floor(pet[1]),
-                ...     lambda pet: pet[0],
-                ... )
-
-                >>> for grouping in en:
-                ...     print(grouping.key, grouping.to_set())
-                8 {'Fangus', 'Roman', 'Barley'}
-                4 {'Boots', 'Daisy'}
-                1 {'Roll', 'Whiskers'}
-                2 {'Roam'}
+        ```py
+        >>> en = Enumerable(pets_list).group_by(
+        ...     lambda pet: math.floor(pet[1]),
+        ...     lambda pet: pet[0],
+        ... )
+
+        >>> for grouping in en:
+        ...     print(grouping.key, grouping.to_set())
+        8 {'Fangus', 'Roman', 'Barley'}
+        4 {'Boots', 'Daisy'}
+        1 {'Roll', 'Whiskers'}
+        2 {'Roam'}
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def group_by2(self,
         key_selector: Callable[[TSource_co], TKey],
         __result_selector: Callable[[TKey, Enumerable[TSource_co]], TResult],
     ) -> Enumerable[TResult]:
         '''
         Groups the elements of the sequence according to a specified key selector function and creates a
         result value using each grouping and its key.
 
         Example
-            .. code-block:: python
-
-                >>> en = Enumerable(pets_list).group_by2(
-                ...     lambda pet: math.floor(pet[1]),
-                ...     lambda age_floored, pets: (age_floored, pets.to_list()),
-                ... )
-
-                >>> for obj in en:
-                ...     print(obj)
-                (8, [('Barley', 8.3), ('Roman', 8.6), ('Fangus', 8.6)])
-                (4, [('Boots', 4.9), ('Daisy', 4.3)])
-                (1, [('Whiskers', 1.5), ('Roll', 1.4)])
-                (2, [('Roam', 2.2)])
+        ```py
+        >>> en = Enumerable(pets_list).group_by2(
+        ...     lambda pet: math.floor(pet[1]),
+        ...     lambda age_floored, pets: (age_floored, pets.to_list()),
+        ... )
+
+        >>> for obj in en:
+        ...     print(obj)
+        (8, [('Barley', 8.3), ('Roman', 8.6), ('Fangus', 8.6)])
+        (4, [('Boots', 4.9), ('Daisy', 4.3)])
+        (1, [('Whiskers', 1.5), ('Roll', 1.4)])
+        (2, [('Roam', 2.2)])
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def group_by2(self,
         key_selector: Callable[[TSource_co], TKey],
     ) -> Enumerable[Grouping[TKey, TSource_co]]:
         '''
         Groups the elements of the sequence according to a specified key selector function.
 
         Example
-            .. code-block:: python
+        ```py
+        >>> en = Enumerable(pets_list).group_by2(
+        ...     lambda pet: math.floor(pet[1]),
+        ... )
+
+        >>> for grouping in en:
+        ...     print(grouping.key, grouping.to_list())
+        8 [('Barley', 8.3), ('Roman', 8.6), ('Fangus', 8.6)]
+        4 [('Boots', 4.9), ('Daisy', 4.3)]
+        1 [('Whiskers', 1.5), ('Roll', 1.4)]
+        2 [('Roam', 2.2)]
+        ```
 
-                >>> en = Enumerable(pets_list).group_by2(
-                ...     lambda pet: math.floor(pet[1]),
-                ... )
-
-                >>> for grouping in en:
-                ...     print(grouping.key, grouping.to_list())
-                8 [('Barley', 8.3), ('Roman', 8.6), ('Fangus', 8.6)]
-                4 [('Boots', 4.9), ('Daisy', 4.3)]
-                1 [('Whiskers', 1.5), ('Roll', 1.4)]
-                2 [('Roam', 2.2)]
-
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     def group_join(self,
         inner: Iterable[TInner],
         outer_key_selector: Callable[[TSource_co], TKey],
         inner_key_selector: Callable[[TInner], TKey],
         result_selector: Callable[[TSource_co, Enumerable[TInner]], TResult],
@@ -835,84 +873,88 @@
         In normal cases, the iteration preserves order of elements in self (outer), and for each element in
         self, the order of matching elements from inner.
         
         Unhashable keys are supported (where hashibility is determined by checking `typing.Hashable`). If any
         keys formed by key selectors involve such types, the order is unspecified.
 
         Example
-            .. code-block:: python
-
-                >>> class Person(NamedTuple):
-                ...     name: str
-                >>> class Pet(NamedTuple):
-                ...     name: str
-                ...     owner: Person
-
-                >>> magnus = Person('Hedlund, Magnus')
-                >>> terry = Person('Adams, Terry')
-                >>> charlotte = Person('Weiss, Charlotte')
-                >>> poor = Person('Animal, No')
-                >>> barley = Pet('Barley', owner=terry)
-                >>> boots = Pet('Boots', owner=terry)
-                >>> whiskers = Pet('Whiskers', owner=charlotte)
-                >>> daisy = Pet('Daisy', owner=magnus)
-                >>> roman = Pet('Roman', owner=terry)
-
-                >>> people = [magnus, terry, charlotte, poor]
-                >>> pets = [barley, boots, whiskers, daisy, roman]
-
-                >>> en = Enumerable(people).group_join(
-                ...     pets,
-                ...     lambda person: person,
-                ...     lambda pet: pet.owner,
-                ...     lambda person, pet_collection: (
-                ...         person.name,
-                ...         pet_collection.select(lambda pet: pet.name).to_set(),
-                ...     ),
-                ... )
-
-                >>> for obj in en:
-                ...     print(obj)
-                ('Hedlund, Magnus', {'Daisy'})
-                ('Adams, Terry', {'Boots', 'Roman', 'Barley'})
-                ('Weiss, Charlotte', {'Whiskers'})
-                ('Animal, No', set())
+        ```py
+        >>> class Person(NamedTuple):
+        ...     name: str
+        >>> class Pet(NamedTuple):
+        ...     name: str
+        ...     owner: Person
+
+        >>> magnus = Person('Hedlund, Magnus')
+        >>> terry = Person('Adams, Terry')
+        >>> charlotte = Person('Weiss, Charlotte')
+        >>> poor = Person('Animal, No')
+        >>> barley = Pet('Barley', owner=terry)
+        >>> boots = Pet('Boots', owner=terry)
+        >>> whiskers = Pet('Whiskers', owner=charlotte)
+        >>> daisy = Pet('Daisy', owner=magnus)
+        >>> roman = Pet('Roman', owner=terry)
+
+        >>> people = [magnus, terry, charlotte, poor]
+        >>> pets = [barley, boots, whiskers, daisy, roman]
+
+        >>> en = Enumerable(people).group_join(
+        ...     pets,
+        ...     lambda person: person,
+        ...     lambda pet: pet.owner,
+        ...     lambda person, pet_collection: (
+        ...         person.name,
+        ...         pet_collection.select(lambda pet: pet.name).to_set(),
+        ...     ),
+        ... )
+
+        >>> for obj in en:
+        ...     print(obj)
+        ('Hedlund, Magnus', {'Daisy'})
+        ('Adams, Terry', {'Boots', 'Roman', 'Barley'})
+        ('Weiss, Charlotte', {'Whiskers'})
+        ('Animal, No', set())
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     def intersect(self, second: Iterable[TSource_co]) -> Enumerable[TSource_co]:
         '''
-        Produces the set intersection of two sequences: self * second.
+        Produces the set intersection of two sequences: self & second.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9, 11]
-            >>> Enumerable(ints).intersect([1, 2, 3, 4, 5]).to_list()
-            [1, 3, 5]
+        ```py
+        >>> ints = [1, 3, 5, 7, 9, 11]
+        >>> Enumerable(ints).intersect([1, 2, 3, 4, 5]).to_list()
+        [1, 3, 5]
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable values.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable values.
         '''
 
     def intersect_by(self,
         second: Iterable[TKey],
         key_selector: Callable[[TSource_co], TKey],
     ) -> Enumerable[TSource_co]:
         '''
-        Produces the set intersection of two sequences: self * second according to a
+        Produces the set intersection of two sequences: self & second according to a
         specified key selector.
 
         Example
-            >>> strs = ['+1', '-3', '+5', '-7', '+9', '-11']
-            >>> Enumerable(strs).intersect_by([1, 2, 3, 5, 9], lambda x: abs(int(x))).to_list()
-            ['+1', '-3', '+5', '+9']
+        ```py
+        >>> strs = ['+1', '-3', '+5', '-7', '+9', '-11']
+        >>> Enumerable(strs).intersect_by([1, 2, 3, 5, 9], lambda x: abs(int(x))).to_list()
+        ['+1', '-3', '+5', '+9']
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def join(self,
         inner: Iterable[TInner],
         outer_key_selector: Callable[[TSource_co], TKey],
         inner_key_selector: Callable[[TInner], TKey],
         result_selector: Callable[[TSource_co, TInner], TResult],
@@ -923,185 +965,199 @@
         In normal cases, the iteration preserves order of elements in self (outer), and for each element in
         self, the order of matching elements from inner.
         
         Unhashable keys are supported (where hashibility is determined by checking `typing.Hashable`). If any
         keys formed by key selectors involve such types, the order is unspecified.
 
         Example
-            .. code-block:: python
-
-                # Please refer to group_join() for definition of people and pets
+        ```py
+        # Please refer to group_join() for definition of people and pets
 
-                >>> en = Enumerable(people).join(
-                ...     pets,
-                ...     lambda person: person,
-                ...     lambda pet: pet.owner,
-                ...     lambda person, pet: (person.name, pet.name),
-                ... )
-
-                >>> for obj in en:
-                ...     print(obj)
-                ('Hedlund, Magnus', 'Daisy')
-                ('Adams, Terry', 'Barley')
-                ('Adams, Terry', 'Boots')
-                ('Adams, Terry', 'Roman')
-                ('Weiss, Charlotte', 'Whiskers')
+        >>> en = Enumerable(people).join(
+        ...     pets,
+        ...     lambda person: person,
+        ...     lambda pet: pet.owner,
+        ...     lambda person, pet: (person.name, pet.name),
+        ... )
+
+        >>> for obj in en:
+        ...     print(obj)
+        ('Hedlund, Magnus', 'Daisy')
+        ('Adams, Terry', 'Barley')
+        ('Adams, Terry', 'Boots')
+        ('Adams, Terry', 'Roman')
+        ('Weiss, Charlotte', 'Whiskers')
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def last(self) -> TSource_co:
         '''
         Returns the last element of the sequence. Raises `InvalidOperationError` if there is no first
         element.
 
         This method always uses a generic method to enumerate the last element (O(n)) regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).last()
-                100
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).last()
+        100
+        ```
         '''
 
     @overload
     def last(self, __predicate: Callable[[TSource_co], bool]) -> TSource_co:
         '''
         Returns the last element of the sequence that satisfies the condition. Raises
         `InvalidOperationError` if no such element exists.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9, 11, 13]
-            >>> Enumerable(ints).last(lambda e: e < 10)
-            9
+        ```py
+        >>> ints = [1, 3, 5, 7, 9, 11, 13]
+        >>> Enumerable(ints).last(lambda e: e < 10)
+        9
+        ```
         '''
 
     @overload
     def last2(self, __default: TDefault) -> Union[TSource_co, TDefault]:
         '''
         Returns the last element of the sequence or a default value if there is no such
         element.
 
         This method always uses a generic method to enumerate the last element (O(n)) regardless the
         implementation of the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen(ok: bool):
-                ...     if ok:
-                ...         yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen(True)).last2(9999)
-                100
-                >>> Enumerable(gen(False)).last2(9999)
-                9999
+        ```py
+        >>> def gen(ok: bool):
+        ...     if ok:
+        ...         yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen(True)).last2(9999)
+        100
+        >>> Enumerable(gen(False)).last2(9999)
+        9999
+        ```
         '''
 
     @overload
     def last2(self,
         __predicate: Callable[[TSource_co], bool],
         __default: TDefault,
     ) -> Union[TSource_co, TDefault]:
         '''
         Returns the last element of the sequence that satisfies the condition or a default value if
         no such element exists.
 
         Example
-            >>> ints = [13, 11, 9, 7, 5, 3, 1]
-            >>> Enumerable(ints).last2(lambda e: e < 0, 9999)
-            9999
+        ```py
+        >>> ints = [13, 11, 9, 7, 5, 3, 1]
+        >>> Enumerable(ints).last2(lambda e: e < 0, 9999)
+        9999
+        ```
         '''
 
     @overload
     def max(self: Enumerable[TSupportsLessThan]) -> TSupportsLessThan:
         '''
         Returns the maximum value in the sequence. Raises `InvalidOperationError` if there is no value.
 
         Example
-            >>> nums = [1, 5, 2.2, 5, 1, 2]
-            >>> Enumerable(nums).max()
-            5
+        ```py
+        >>> nums = [1, 5, 2.2, 5, 1, 2]
+        >>> Enumerable(nums).max()
+        5
+        ```
         '''
 
     @overload
     def max(self, __result_selector: Callable[[TSource_co], TSupportsLessThan]) -> TSupportsLessThan:
         '''
         Invokes a transform function on each element of the sequence and returns the maximum of the
         resulting values. Raises `InvalidOperationError` if there is no value.
 
         Example
-            >>> strs = ['aaa', 'bb', 'c', 'dddd']
-            >>> Enumerable(strs).max(len)
-            4
+        ```py
+        >>> strs = ['aaa', 'bb', 'c', 'dddd']
+        >>> Enumerable(strs).max(len)
+        4
+        ```
         '''
 
     @overload
     def max2(self: Enumerable[TSupportsLessThan],
         __default: TDefault,
     ) -> Union[TSupportsLessThan, TDefault]:
         '''
         Returns the maximum value in the sequence, or the default one if there is no value.
 
         Example
-            >>> Enumerable([]).max2(0)
-            0
+        ```py
+        >>> Enumerable([]).max2(0)
+        0
+        ```
         '''
 
     @overload
     def max2(self,
         __result_selector: Callable[[TSource_co], TSupportsLessThan],
         __default: TDefault,
     ) -> Union[TSupportsLessThan, TDefault]:
         '''
         Invokes a transform function on each element of the sequence and returns the maximum of the
         resulting values. Returns the default one if there is no value.
 
         Example
-            >>> Enumerable([]).max2(len, 0)
-            0
-            >>> Enumerable(['a']).max2(len, 0)
-            1
+        ```py
+        >>> Enumerable([]).max2(len, 0)
+        0
+        >>> Enumerable(['a']).max2(len, 0)
+        1
+        ```
         '''
 
     @overload
     def max_by(self, key_selector: Callable[[TSource_co], TSupportsLessThan]) -> TSource_co:
         '''
         Returns the maximal element of the sequence based on the given key selector. Raises
         `InvalidOperationError` if there is no value.
 
         Example
-            >>> strs = ['aaa', 'bb', 'c', 'dddd']
-            >>> Enumerable(strs).max_by(len)
-            'dddd'
+        ```py
+        >>> strs = ['aaa', 'bb', 'c', 'dddd']
+        >>> Enumerable(strs).max_by(len)
+        'dddd'
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     @overload
     def max_by(self,
         key_selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
     ) -> TSource_co:
         '''
         Returns the maximal element of the sequence based on the given key selector and the comparer.
         Raises `InvalidOperationError` if there is no value.
 
         Such comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal.
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     @overload
     def min(self: Enumerable[TSupportsLessThan]) -> TSupportsLessThan:
         '''
         Returns the minimum value in the sequence. Raises `InvalidOperationError` if there is no value.
         '''
@@ -1133,104 +1189,112 @@
 
     @overload
     def min_by(self, key_selector: Callable[[TSource_co], TSupportsLessThan]) -> TSource_co:
         '''
         Returns the minimal element of the sequence based on the given key selector. Raises
         `InvalidOperationError` if there is no value.
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     @overload
     def min_by(self,
         key_selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
     ) -> TSource_co:
         '''
         Returns the minimal element of the sequence based on the given key selector and the comparer.
         Raises `InvalidOperationError` if there is no value.
 
         Such comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal.
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def of_type(self, t_result: Type[TResult]) -> Enumerable[TResult]:
         '''
         Filters elements based on the specified type.
 
         Builtin `isinstance()` is used.
 
         Example
-            >>> lst = [1, 14, object(), True, []]
-            >>> Enumerable(lst).of_type(int).to_list()
-            [1, 14, True]
+        ```py
+        >>> lst = [1, 14, object(), True, []]
+        >>> Enumerable(lst).of_type(int).to_list()
+        [1, 14, True]
+        ```
         '''
 
     @overload
     def order_by(self,
         key_selector: Callable[[TSource_co], TSupportsLessThan],
     ) -> OrderedEnumerable[TSource_co, TSupportsLessThan]:
         '''
         Sorts the elements of the sequence in ascending order according to a key.
 
         Example
-            >>> ints = [8, 4, 5, 2]
-            >>> Enumerable(ints).order_by(lambda e: e).to_list()
-            [2, 4, 5, 8]
+        ```py
+        >>> ints = [8, 4, 5, 2]
+        >>> Enumerable(ints).order_by(lambda e: e).to_list()
+        [2, 4, 5, 8]
+        ```
+
+        Example
+        ```py
+        >>> class Pet(NamedTuple):
+        ...     name: str
+        ...     age: int
+
+        >>> pets = [Pet('Barley', 8), Pet('Boots', 4), Pet('Roman', 5)]
+        >>> Enumerable(pets).order_by(lambda p: p.age) \\
+        ...     .select(lambda p: p.name)              \\
+        ...     .to_list()
+        ['Boots', 'Roman', 'Barley']
+        ```
 
-        Example
-            .. code-block:: python
-
-                >>> class Pet(NamedTuple):
-                ...     name: str
-                ...     age: int
-
-                >>> pets = [Pet('Barley', 8), Pet('Boots', 4), Pet('Roman', 5)]
-                >>> Enumerable(pets).order_by(lambda p: p.age) \\
-                ...     .select(lambda p: p.name)              \\
-                ...     .to_list()
-                ['Boots', 'Roman', 'Barley']
-
-        Subsequent ordering is supported. See ``OrderedEnumerable``.
+        Subsequent ordering is supported. See `OrderedEnumerable`.
         '''
 
     @overload
     def order_by(self,
         key_selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
     ) -> OrderedEnumerable[TSource_co, TKey]:
         '''
         Sorts the elements of the sequence in ascending order by using a specified comparer.
 
         Such comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal. In fact, this overload should not be used
-        (see `Sorting HOW TO <https://docs.python.org/3/howto/sorting.html#the-old-way-using-the-cmp-parameter>`_).
+        (see [Sorting HOW TO](https://docs.python.org/3/howto/sorting.html#the-old-way-using-the-cmp-parameter>)).
 
         Example
-            >>> Enumerable(pets).order_by(lambda p: p, lambda pl, pr: pl.age - pr.age) \\
-            ...     .select(lambda p: p.name)                                          \\
-            ...     .to_list()
-            ['Boots', 'Roman', 'Barley']
+        ```py
+        >>> Enumerable(pets).order_by(lambda p: p, lambda pl, pr: pl.age - pr.age) \\
+        ...     .select(lambda p: p.name)                                          \\
+        ...     .to_list()
+        ['Boots', 'Roman', 'Barley']
+        ```
         '''
 
     @overload
     def order_by_descending(self,
         key_selector: Callable[[TSource_co], TSupportsLessThan],
     ) -> OrderedEnumerable[TSource_co, TSupportsLessThan]:
         '''
         Sorts the elements of the sequence in descending order according to a key.
 
         Example
-            >>> ints = [8, 4, 5, 2]
-            >>> Enumerable(ints).order_by_descending(lambda e: e).to_list()
-            [8, 5, 4, 2]
+        ```py
+        >>> ints = [8, 4, 5, 2]
+        >>> Enumerable(ints).order_by_descending(lambda e: e).to_list()
+        [8, 5, 4, 2]
+        ```
         '''
 
     @overload
     def order_by_descending(self,
         key_selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
     ) -> OrderedEnumerable[TSource_co, TKey]:
@@ -1243,127 +1307,139 @@
 
     def prepend(self, element: TSource_co) -> Enumerable[TSource_co]:  # type: ignore
         '''
         Adds a value to the beginning of the sequence. Again, this does not affect the original
         wrapped object.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).prepend(-1).to_list()
-            [-1, 1, 3, 5, 7, 9]
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).prepend(-1).to_list()
+        [-1, 1, 3, 5, 7, 9]
+        ```
         '''
 
     # count: Optional[int] is nonstandard behavior
     @staticmethod
     def range(start: int, count: Optional[int]) -> Enumerable[int]:
         '''
         Generates a sequence of `count` integral numbers from `start`, incrementing each by one.
 
         If `count` is `None`, the sequence is infinite. Raises `InvalidOperationError` if `count`
         is negative.
 
         Example
-            >>> Enumerable.range(-5, 6).to_list()
-            [-5, -4, -3, -2, -1, 0]
+        ```py
+        >>> Enumerable.range(-5, 6).to_list()
+        [-5, -4, -3, -2, -1, 0]
+        ```
         '''
 
     # count: Optional[int] is nonstandard behavior
     @staticmethod
     def repeat(value: TResult, count: Optional[int] = None) -> Enumerable[TResult]:
         '''
         Generates a sequence that contains one repeated value.
 
         If `count` is `None`, the sequence is infinite. Raises `InvalidOperationError` if `count`
         is negative.
 
         Example
-            >>> Enumerable.repeat(0, 6).to_list()
-            [0, 0, 0, 0, 0, 0]
+        ```py
+        >>> Enumerable.repeat(0, 6).to_list()
+        [0, 0, 0, 0, 0, 0]
+        ```
         '''
 
     def reverse(self) -> Enumerable[TSource_co]:
         '''
         Inverts the order of the elements in the sequence.
 
         This method always uses a generic reverse traversal method regardless the implementation of
         the wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-
-                >>> Enumerable(gen()).reverse().to_list()
-                [100, 10, 1]
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+
+        >>> Enumerable(gen()).reverse().to_list()
+        [100, 10, 1]
+        ```
         '''
 
     def select(self, selector: Callable[[TSource_co], TResult]) -> Enumerable[TResult]:
         '''
         Projects each element of the sequence into a new form.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).select(lambda e: '*' * e).to_list()
-            ['*', '***', '*****', '*******', '*********']
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).select(lambda e: '*' * e).to_list()
+        ['*', '***', '*****', '*******', '*********']
+        ```
         '''
 
     def select2(self, selector: Callable[[TSource_co, int], TResult]) -> Enumerable[TResult]:
         '''
         Projects each element of the sequence into a new form by incorporating the indices.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> Enumerable(ints).select2(lambda e, i: e * (i + 1)).to_list()
-            [1, 6, 15, 28, 45]
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> Enumerable(ints).select2(lambda e, i: e * (i + 1)).to_list()
+        [1, 6, 15, 28, 45]
+        ```
         '''
 
     @overload
     def select_many(self,
         collection_selector: Callable[[TSource_co], Iterable[TCollection]],
         __result_selector: Callable[[TSource_co, TCollection], TResult],
     ) -> Enumerable[TResult]:
         '''
         Projects each element of the sequence into an iterable, flattens the resulting sequence
         into one sequence, then calls result_selector on each element therein.
 
         Example
-            .. code-block:: python
-
-                >>> pet_owners = [
-                ...     {'name': 'Higa', 'pets': ['Scruffy', 'Sam']},
-                ...     {'name': 'Ashkenazi', 'pets': ['Walker', 'Sugar']},
-                ...     {'name': 'Hines',  'pets': ['Dusty']},
-                ... ]
-
-                >>> en = Enumerable(pet_owners).select_many(
-                ...     lambda owner: owner['pets'],
-                ...     lambda owner, name: (name, owner['name']),
-                ... )
-
-                >>> for tup in en:
-                ...     print(tup)
-                ('Scruffy', 'Higa')
-                ('Sam', 'Higa')
-                ('Walker', 'Ashkenazi')
-                ('Sugar', 'Ashkenazi')
-                ('Dusty', 'Hines')
+        ```py
+        >>> pet_owners = [
+        ...     {'name': 'Higa', 'pets': ['Scruffy', 'Sam']},
+        ...     {'name': 'Ashkenazi', 'pets': ['Walker', 'Sugar']},
+        ...     {'name': 'Hines',  'pets': ['Dusty']},
+        ... ]
+
+        >>> en = Enumerable(pet_owners).select_many(
+        ...     lambda owner: owner['pets'],
+        ...     lambda owner, name: (name, owner['name']),
+        ... )
+
+        >>> for tup in en:
+        ...     print(tup)
+        ('Scruffy', 'Higa')
+        ('Sam', 'Higa')
+        ('Walker', 'Ashkenazi')
+        ('Sugar', 'Ashkenazi')
+        ('Dusty', 'Hines')
+        ```
         '''
 
     @overload
     def select_many(self,
         __selector: Callable[[TSource_co], Iterable[TResult]],
     ) -> Enumerable[TResult]:
         '''
         Projects each element of the sequence to an iterable and flattens the resultant sequences.
 
         Example
-            >>> sentences = ['i select things', 'i do many times']
-            >>> Enumerable(sentences).select_many(str.split).to_list()
-            ['i', 'select', 'things', 'i', 'do', 'many', 'times']
+        ```py
+        >>> sentences = ['i select things', 'i do many times']
+        >>> Enumerable(sentences).select_many(str.split).to_list()
+        ['i', 'select', 'things', 'i', 'do', 'many', 'times']
+        ```
         '''
 
     @overload
     def select_many2(self,
         collection_selector: Callable[[TSource_co, int], Iterable[TCollection]],
         __result_selector: Callable[[TSource_co, TCollection], TResult],
     ) -> Enumerable[TResult]:
@@ -1378,274 +1454,310 @@
         __selector: Callable[[TSource_co, int], Iterable[TResult]],
     ) -> Enumerable[TResult]:
         '''
         Projects each element of the sequence to an iterable and flattens the resultant sequences.
         The indices of source elements are used.
 
         Example
-            >>> dinner = ['Ramen with Egg and Beef', 'Gyoza', 'Fried Chicken']
-            >>> en = Enumerable(dinner).select_many2(
-            ...     lambda e, i: Enumerable(e.split(' '))
-            ...         .where(lambda w: w[0].isupper())
-            ...         .select(lambda w: f'Table {i}: {w}'),
-            ... )
-            >>> for s in en:
-            ...     print(s)
-            Table 0: Ramen
-            Table 0: Egg  
-            Table 0: Beef 
-            Table 1: Gyoza
-            Table 2: Fried
-            Table 2: Chicken
+        ```py
+        >>> dinner = ['Ramen with Egg and Beef', 'Gyoza', 'Fried Chicken']
+        >>> en = Enumerable(dinner).select_many2(
+        ...     lambda e, i: Enumerable(e.split(' '))
+        ...         .where(lambda w: w[0].isupper())
+        ...         .select(lambda w: f'Table {i}: {w}'),
+        ... )
+        >>> for s in en:
+        ...     print(s)
+        Table 0: Ramen
+        Table 0: Egg  
+        Table 0: Beef 
+        Table 1: Gyoza
+        Table 2: Fried
+        Table 2: Chicken
+        ```
         '''
 
     @overload
     def sequence_equal(self, second: Iterable[TSource_co]) -> bool:
         '''
         Determines whether two sequences are equal using `==` on each element.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100
-                >>> lst = [1, 10, 100]
-
-                >>> Enumerable(gen()).sequence_equal(lst)
-                True
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100
+        >>> lst = [1, 10, 100]
+
+        >>> Enumerable(gen()).sequence_equal(lst)
+        True
+        ```
         '''
 
     @overload
     def sequence_equal(self,
         second: Iterable[TOther],
         __comparer: Callable[[TSource_co, TOther], bool],
     ) -> bool:
         '''
         Determines whether two sequences are equal using a comparer that returns True if two values
         are equal, on each element.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9]
-            >>> strs = ['1', '3', '5', '7', '9']
-            >>> Enumerable(ints).sequence_equal(strs, lambda x, y: str(x) == y)
-            True
+        ```py
+        >>> ints = [1, 3, 5, 7, 9]
+        >>> strs = ['1', '3', '5', '7', '9']
+        >>> Enumerable(ints).sequence_equal(strs, lambda x, y: str(x) == y)
+        True
+        ```
 
-        Revisions:
-            - v0.1.2: New.
+        Revisions
+            ~ v0.1.2: New.
         '''
 
     @overload
     def single(self) -> TSource_co:
         '''
         Returns the only element in the sequence. Raises `InvalidOperationError` if the sequence does not
         contain exactly one element.
 
         Example
-            >>> Enumerable([5]).single()
-            5
+        ```py
+        >>> Enumerable([5]).single()
+        5
+        ```
 
         Example
-            >>> lst = [5, 6]
-            >>> try:
-            ...     print(Enumerable(lst).single())
-            ... except InvalidOperationError:
-            ...     print('Collection does not contain exactly one element. Sorry.')
-            Collection does not contain exactly one element. Sorry.
+        ```py
+        >>> lst = [5, 6]
+        >>> try:
+        ...     print(Enumerable(lst).single())
+        ... except InvalidOperationError:
+        ...     print('Collection does not contain exactly one element. Sorry.')
+        Collection does not contain exactly one element. Sorry.
+        ```
         '''
 
     @overload
     def single(self, __predicate: Callable[[TSource_co], bool]) -> TSource_co:
         '''
         Returns the only element in the sequence that satisfies the condition. Raises `InvalidOperationError`
         if no element satisfies the condition, or more than one do.
 
         Example
-            >>> ints = [1, 3, 5, 7, 9, 11, 9]
-            >>> Enumerable(ints).single(lambda e: e > 10)
-            11
-            >>> try:
-            ...     Enumerable(ints).single(lambda e: e == 9)
-            ... except InvalidOperationError:
-            ...     print('Too many nines!')
-            Too many nines!
+        ```py
+        >>> ints = [1, 3, 5, 7, 9, 11, 9]
+        >>> Enumerable(ints).single(lambda e: e > 10)
+        11
+        >>> try:
+        ...     Enumerable(ints).single(lambda e: e == 9)
+        ... except InvalidOperationError:
+        ...     print('Too many nines!')
+        Too many nines!
+        ```
         '''
 
     @overload
     def single2(self, __default: TDefault) -> Union[TSource_co, TDefault]:
         '''
         Returns the only element in the sequence or the default value if the sequence is empty. Raises
         `InvalidOperationError` if there are more than one elements in the sequence.
 
         Example
-            >>> Enumerable([]).single2(0)
-            0
+        ```py
+        >>> Enumerable([]).single2(0)
+        0
+        ```
         '''
 
     @overload
     def single2(self,
         __predicate: Callable[[TSource_co], bool],
         __default: TDefault,
     ) -> Union[TSource_co, TDefault]:
         '''
         Returns the only element in the sequence that satisfies the condition, or the default value if there is
         no such element. Raises `InvalidOperationError` if there are more than one elements satisfying the
         condition.
 
         Example
-            >>> fruits = ['apple', 'banana', 'mango']
-            >>> Enumerable(fruits).single2(lambda e: len(e) > 10, 'sorry')
-            'sorry'
+        ```py
+        >>> fruits = ['apple', 'banana', 'mango']
+        >>> Enumerable(fruits).single2(lambda e: len(e) > 10, 'sorry')
+        'sorry'
+        ```
         '''
 
     def skip(self, count: int) -> Enumerable[TSource_co]:
         '''
         Bypasses a specified number of elements in the sequence and then returns the remaining.
 
         Example
-            >>> grades = [59, 82, 70, 56, 92, 98, 85]
-            >>> Enumerable(grades).order_by_descending(lambda g: g).skip(3).to_list()
-            [82, 70, 59, 56]
+        ```py
+        >>> grades = [59, 82, 70, 56, 92, 98, 85]
+        >>> Enumerable(grades).order_by_descending(lambda g: g).skip(3).to_list()
+        [82, 70, 59, 56]
+        ```
         '''
 
     def skip_last(self, count: int) -> Enumerable[TSource_co]:
         '''
         Returns a new sequence that contains the elements of the current sequence with last `count` elements
         omitted.
 
         Example
-            >>> grades = [59, 82, 70, 56, 92, 98, 85]
-            >>> Enumerable(grades).order_by_descending(lambda g: g).skip_last(3).to_list()
-            [98, 92, 85, 82]
+        ```py
+        >>> grades = [59, 82, 70, 56, 92, 98, 85]
+        >>> Enumerable(grades).order_by_descending(lambda g: g).skip_last(3).to_list()
+        [98, 92, 85, 82]
+        ```
         '''
 
     def skip_while(self, predicate: Callable[[TSource_co], bool]) -> Enumerable[TSource_co]:
         '''
         Bypasses elements in the sequence as long as the condition is true and then returns the remaining
         elements.
 
         Example
-            >>> grades = [59, 82, 70, 56, 92, 98, 85]
-            >>> Enumerable(grades).order_by_descending(lambda g: g) \\
-            ...     .skip_while(lambda g: g >= 80)                  \\
-            ...     .to_list()
-            [70, 59, 56]
+        ```py
+        >>> grades = [59, 82, 70, 56, 92, 98, 85]
+        >>> Enumerable(grades).order_by_descending(lambda g: g) \\
+        ...     .skip_while(lambda g: g >= 80)                  \\
+        ...     .to_list()
+        [70, 59, 56]
+        ```
         '''
 
     def skip_while2(self, predicate: Callable[[TSource_co, int], bool]) -> Enumerable[TSource_co]:
         '''
         Bypasses elements in the sequence as long as the condition is true and then returns the remaining
         elements. The element's index is used in the predicate function.
 
         Example
-            >>> amounts = [500, 250, 900, 800, 650, 400, 150, 550]
-            >>> Enumerable(amounts).skip_while2(lambda a, i: a > i * 100).to_list()
-            [400, 150, 550]
+        ```py
+        >>> amounts = [500, 250, 900, 800, 650, 400, 150, 550]
+        >>> Enumerable(amounts).skip_while2(lambda a, i: a > i * 100).to_list()
+        [400, 150, 550]
+        ```
         '''
 
     # returning 0 conforms the builtin sum() function
     @overload
     def sum(self: Enumerable[TSupportsAdd]) -> Union[TSupportsAdd, int]:
         '''
         Computes the sum of the sequence, or `0` if the sequence is empty.
 
         Example
-            >>> floats = [.1, .3, .5, .9, 1.1]
-            >>> Enumerable(floats).sum()
-            2.9000000000000004
+        ```py
+        >>> floats = [.1, .3, .5, .9, 1.1]
+        >>> Enumerable(floats).sum()
+        2.9000000000000004
+        ```
         '''
 
     # returning 0 conforms the builtin sum() function
     @overload
     def sum(self, __selector: Callable[[TSource_co], TSupportsAdd]) -> Union[TSupportsAdd, int]:
         '''
         Computes the sum of the sequence using the selector. Returns `0` if the sequence is empty.
 
         Example
-            >>> floats = [.1, .3, .5, .9, 1.1]
-            >>> Enumerable(floats).sum(lambda e: int(e * 1000))
-            2900
+        ```py
+        >>> floats = [.1, .3, .5, .9, 1.1]
+        >>> Enumerable(floats).sum(lambda e: int(e * 1000))
+        2900
+        ```
         '''
 
     @overload
     def sum2(self: Enumerable[TSupportsAdd],
         __default: TDefault,
     ) -> Union[TSupportsAdd, TDefault]:
         '''
         Computes the sum of the sequence. Returns the default value if it is empty.
 
         Example
-            >>> Enumerable([]).sum2(880)
-            880
+        ```py
+        >>> Enumerable([]).sum2(880)
+        880
+        ```
         '''
 
     @overload
     def sum2(self,
         __selector: Callable[[TSource_co], TSupportsAdd],
         __default: TDefault,
     ) -> Union[TSupportsAdd, TDefault]:
         '''
         Computes the sum of the sequence using the selector. Returns the default value if it is empty.
 
         Example
-            >>> Enumerable([]).sum2(lambda e: int(e * 1000), 880)
-            880
+        ```py
+        >>> Enumerable([]).sum2(lambda e: int(e * 1000), 880)
+        880
+        ```
         '''
 
     @overload
     def take(self, count: int) -> Enumerable[TSource_co]:
         '''
         Returns a specified number of contiguous elements from the start of the sequence.
 
         Example
-            >>> grades = [98, 92, 85, 82, 70, 59, 56]
-            >>> Enumerable(grades).take(3).to_list()
-            [98, 92, 85]
+        ```py
+        >>> grades = [98, 92, 85, 82, 70, 59, 56]
+        >>> Enumerable(grades).take(3).to_list()
+        [98, 92, 85]
+        ```
         '''
 
     @overload
     def take(self, __index: slice) -> Enumerable[TSource_co]:
         '''
         Produces a subsequence defined by the given slice notation.
 
         This method always uses a generic list slicing method regardless the implementation of the
         wrapped iterable.
 
         This method currently is identical to `elements_in()` when it takes a slice.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
-
-                >>> Enumerable(gen()).take(slice(1, 3)).to_list()
-                [10, 100]
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
+
+        >>> Enumerable(gen()).take(slice(1, 3)).to_list()
+        [10, 100]
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def take_last(self, count: int) -> Enumerable[TSource_co]:
         '''
         Returns a new sequence that contains the last `count` elements.
 
         Example
-            >>> grades = [98, 92, 85, 82, 70, 59, 56]
-            >>> Enumerable(grades).take_last(3).to_list()
-            [70, 59, 56]
+        ```py
+        >>> grades = [98, 92, 85, 82, 70, 59, 56]
+        >>> Enumerable(grades).take_last(3).to_list()
+        [70, 59, 56]
+        ```
         '''
 
     def take_while(self, predicate: Callable[[TSource_co], bool]) -> Enumerable[TSource_co]:
         '''
         Returns elements from the sequence as long as the condition is true and skips the remaining.
 
         Example
-            >>> strs = ['1', '3', '5', '7', '', '1', '4', '5']
-            >>> Enumerable(strs).take_while(lambda g: g).to_list()
-            ['1', '3', '5', '7']
+        ```py
+        >>> strs = ['1', '3', '5', '7', '', '1', '4', '5']
+        >>> Enumerable(strs).take_while(lambda g: g).to_list()
+        ['1', '3', '5', '7']
+        ```
         '''
 
     def take_while2(self, predicate: Callable[[TSource_co, int], bool]) -> Enumerable[TSource_co]:
         '''
         Returns elements from the sequence as long as the condition is true and skips the remaining. The
         element's index is used in the predicate function.
         '''
@@ -1686,219 +1798,233 @@
     ) -> Lookup[TKey, TValue]:
         '''
         Enumerates all values and returns a lookup containing them according to specified key
         selector and value selector. The values within each group are in the same order as in
         self.
 
         Example
-            >>> food = [
-            ...     ('main', 'ramen'), ('main', 'noodles'), ('side', 'chicken'),
-            ...     ('main', 'spaghetti'), ('snack', 'popcorns'), ('side', 'apples'),
-            ...     ('side', 'orange'), ('drink', 'coke'), ('main', 'birthdaycake'),
-            ... ]
-            >>> lookup = Enumerable(food).to_lookup(lambda e: e[0], lambda e: e[1])
-            >>> lookup.select(lambda grouping: grouping.key).to_list()
-            ['main', 'side', 'snack', 'drink']
-            >>> if 'side' in lookup:
-            ...     print(lookup['side'].to_list())
-            ['chicken', 'apples', 'orange']
+        ```py
+        >>> food = [
+        ...     ('main', 'ramen'), ('main', 'noodles'), ('side', 'chicken'),
+        ...     ('main', 'spaghetti'), ('snack', 'popcorns'), ('side', 'apples'),
+        ...     ('side', 'orange'), ('drink', 'coke'), ('main', 'birthdaycake'),
+        ... ]
+        >>> lookup = Enumerable(food).to_lookup(lambda e: e[0], lambda e: e[1])
+        >>> lookup.select(lambda grouping: grouping.key).to_list()
+        ['main', 'side', 'snack', 'drink']
+        >>> if 'side' in lookup:
+        ...     print(lookup['side'].to_list())
+        ['chicken', 'apples', 'orange']
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def to_lookup(self,
         key_selector: Callable[[TSource_co], TKey],
     ) -> Lookup[TKey, TSource_co]:
         '''
         Enumerates all values and returns a lookup containing them according to the specified
         key selector. The values within each group are in the same order as in self.
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable keys.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     def union(self, second: Iterable[TSource_co]) -> Enumerable[TSource_co]:
         '''
         Produces the set union of two sequences: self + second.
 
         Example
-            >>> gen = (i for i in range(5))
-            >>> lst = [5, 3, 9, 7, 5, 9, 3, 7]
-            >>> Enumerable(gen).union(lst).to_list()
-            [0, 1, 2, 3, 4, 5, 9, 7]
+        ```py
+        >>> gen = (i for i in range(5))
+        >>> lst = [5, 3, 9, 7, 5, 9, 3, 7]
+        >>> Enumerable(gen).union(lst).to_list()
+        [0, 1, 2, 3, 4, 5, 9, 7]
+        ```
 
-        Revisions:
-            - v0.2.1: Added preliminary support for unhashable values.
+        Revisions
+            ~ v0.2.1: Added preliminary support for unhashable values.
         '''
 
     def union_by(self,
         second: Iterable[TSource_co],
         key_selector: Callable[[TSource_co], object],
     ) -> Enumerable[TSource_co]:
         '''
         Produces the set union of two sequences: self + second according to a specified key
         selector.
 
         Example
-            >>> en = Enumerable([1, 9, -2, -7, 14])
-            >>> en.union_by([15, 2, -26, -7], abs).to_list()
-            [1, 9, -2, -7, 14, 15, -26]  # abs(-2) == abs(2)
+        ```py
+        >>> en = Enumerable([1, 9, -2, -7, 14])
+        >>> en.union_by([15, 2, -26, -7], abs).to_list()
+        [1, 9, -2, -7, 14, 15, -26]  # abs(-2) == abs(2)
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def where(self, predicate: Callable[[TSource_co], bool]) -> Enumerable[TSource_co]:
         '''
         Filters the sequence of values based on a predicate.
 
         Example
-            >>> strs = ['apple', 'orange', 'Apple', 'xx', 'Grapes']
-            >>> Enumerable(strs).where(str.istitle).to_list()
-            ['Apple', 'Grapes']
+        ```py
+        >>> strs = ['apple', 'orange', 'Apple', 'xx', 'Grapes']
+        >>> Enumerable(strs).where(str.istitle).to_list()
+        ['Apple', 'Grapes']
+        ```
         '''
 
     def where2(self, predicate: Callable[[TSource_co, int], bool]) -> Enumerable[TSource_co]:
         '''
         Filters the sequence of values based on a predicate. Each element's index is used in the
         predicate logic.
 
         Example
-            >>> ints = [0, 30, 20, 15, 90, 85, 40, 75]
-            >>> Enumerable(ints).where2(lambda e, i: e <= i * 10).to_list()
-            [0, 20, 15, 40]
+        ```py
+        >>> ints = [0, 30, 20, 15, 90, 85, 40, 75]
+        >>> Enumerable(ints).where2(lambda e, i: e <= i * 10).to_list()
+        [0, 20, 15, 40]
+        ```
         '''
 
     @overload
     def zip(self,
         __second: Iterable[TOther],
     ) -> Enumerable[Tuple[TSource_co, TOther]]:
         '''
         Produces a sequence of 2-element tuples from the two sequences.
 
         Example
-            >>> ints = [1, 2, 3, 4]
-            >>> dims = ['x', 'y', 'z', 't', 'u', 'v']
-            >>> Enumerable(ints).zip(dims).to_list()
-            [(1, 'x'), (2, 'y'), (3, 'z'), (4, 't')]
+        ```py
+        >>> ints = [1, 2, 3, 4]
+        >>> dims = ['x', 'y', 'z', 't', 'u', 'v']
+        >>> Enumerable(ints).zip(dims).to_list()
+        [(1, 'x'), (2, 'y'), (3, 'z'), (4, 't')]
+        ```
         '''
 
     @overload
     def zip(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
     ) -> Enumerable[Tuple[TSource_co, TOther, TOther2]]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
         __fourth: Iterable[TOther3],
     ) -> Enumerable[Tuple[TSource_co, TOther, TOther2, TOther3]]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
         __fourth: Iterable[TOther3],
         __fifth: Iterable[TOther4],
     ) -> Enumerable[Tuple[TSource_co, TOther, TOther2, TOther3, TOther4]]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip(self,
         __second: Iterable[Any],
         __third: Iterable[Any],
         __fourth: Iterable[Any],
         __fifth: Iterable[Any],
         __sixth: Iterable[Any],
         *iters: Iterable[Any],
     ) -> Enumerable[Tuple[Any, ...]]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip2(self,
         __second: Iterable[TOther],
         __result_selector: Callable[[TSource_co, TOther], TResult],
     ) -> Enumerable[TResult]:
         '''
         Applies a specified function to the corresponding elements of two sequences, producing a
         sequence of the results.
 
         Example
-            >>> ints = [1, 2, 3, 4]
-            >>> dims = ['x', 'y', 'z', 't', 'u', 'v']
-            >>> Enumerable(ints).zip2(dims, lambda i, d: f'{i}.{d}').to_list()
-            ['1.x', '2.y', '3.z', '4.t']
+        ```py
+        >>> ints = [1, 2, 3, 4]
+        >>> dims = ['x', 'y', 'z', 't', 'u', 'v']
+        >>> Enumerable(ints).zip2(dims, lambda i, d: f'{i}.{d}').to_list()
+        ['1.x', '2.y', '3.z', '4.t']
+        ```
         '''
 
     @overload
     def zip2(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
         __result_selector: Callable[[TSource_co, TOther, TOther2], TResult],
     ) -> Enumerable[TResult]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip2(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
         __fourth: Iterable[TOther3],
         __result_selector: Callable[[TSource_co, TOther, TOther2, TOther3], TResult],
     ) -> Enumerable[TResult]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip2(self,
         __second: Iterable[TOther],
         __third: Iterable[TOther2],
         __fourth: Iterable[TOther3],
         __fifth: Iterable[TOther4],
         __result_selector: Callable[[TSource_co, TOther, TOther2, TOther3, TOther4], TResult],
     ) -> Enumerable[TResult]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     @overload
     def zip2(self,
         __second: Iterable[Any],
         __third: Iterable[Any],
         __fourth: Iterable[Any],
         __fifth: Iterable[Any],
         __sixth: Iterable[Any],
         *iters_and_result_selector: Union[Iterable[Any], Callable[..., Any]],
     ) -> Enumerable[Any]:
         '''
         Revisions
-            - v0.1.1: New.
+            ~ v0.1.1: New.
         '''
 
     # Methods below are non-standard. They do not have .NET builtin equivalence and are here just
     # for convenience.
 
     @overload
     def elements_in(self, __index: slice) -> Enumerable[TSource_co]:
@@ -1907,41 +2033,41 @@
 
         This method always uses a generic list slicing method regardless the implementation of the
         wrapped iterable.
 
         This method currently is identical to `take()` when it takes a slice.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
-
-                >>> Enumerable(gen()).elements_in(slice(1, 3)).to_list()
-                [10, 100]
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
+
+        >>> Enumerable(gen()).elements_in(slice(1, 3)).to_list()
+        [10, 100]
+        ```
         '''
 
     @overload
     def elements_in(self, __start: int, __stop: int, __step: int = 1) -> Enumerable[TSource_co]:
         '''
         Produces a subsequence with indices that define a slice.
 
         This method always uses a generic list slicing method regardless the implementation of the
         wrapped iterable.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
-
-                >>> Enumerable(gen()).elements_in(1, 3).to_list()
-                [10, 100]
+        ```py
+        >>> def gen():
+        ...     yield 1; yield 10; yield 100; yield 1000; yield 10000
+
+        >>> Enumerable(gen()).elements_in(1, 3).to_list()
+        [10, 100]
+        ```
         '''
 
     def to_tuple(self) -> Tuple[TSource_co, ...]:
         '''
         Enumerates all values and returns a tuple containing them.
 
-        Revisions:
-            - v0.1.2: New.
+        Revisions
+            ~ v0.1.2: New.
         '''
```

### Comparing `types-linq-1.2.0/types_linq/grouping.py` & `types-linq-1.2.1/types_linq/grouping.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 )
 
 
 # kind of respect IGrouping's covariant type parameters if the method _append()
 # is really treated as an internal method
 class Grouping(Enumerable[TValue_co], Generic[TKey_co, TValue_co]):
     '''
-    .. code-block:: python
-
-        from types_linq.grouping import Grouping
+    ```py
+    from types_linq.grouping import Grouping
+    ```
 
     Represents a collection of objects that have a common key.
 
-    Users should not construct instances of this class directly. Use ``Enumerable.group_by()`` instead.
+    Users should not construct instances of this class directly. Use `Enumerable.group_by()` instead.
     '''
 
     _key: TKey_co
     _values: List[TValue_co]
 
     def __init__(self, key: TKey_co):  # type: ignore
         self._values = []
```

### Comparing `types-linq-1.2.0/types_linq/lookup.py` & `types-linq-1.2.1/types_linq/lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 )
 
 
 # TODO: Wish to support Mapping[TKey, TValue], but its default mixin methods are doing something
 # weird.
 class Lookup(Enumerable[Grouping[TKey_co, TValue_co]]):
     '''
-    .. code-block:: python
-
-        from types_linq.lookup import Lookup
+    ```py
+    from types_linq.lookup import Lookup
+    ```
 
     A lookup is a one-to-many dictionary. It maps keys to Enumerable sequences of values.
 
-    Users should not construct instances of this class directly. Use ``Enumerable.to_lookup()``
+    Users should not construct instances of this class directly. Use `Enumerable.to_lookup()`
     instead.
     '''
 
     _groupings: ComposeMap[TKey_co, Grouping[TKey_co, TValue_co]]
 
     def __init__(self,
         source: Iterable[TSource],
```

### Comparing `types-linq-1.2.0/types_linq/more/extrema_enumerable.py` & `types-linq-1.2.1/types_linq/more/extrema_enumerable.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # count elems only store that number of elems in the buffer
     def _get_iterable(self) -> Iterable[TSource_co]:
         it = super()._get_iterable()
         getter = lambda: _FirstExtrema(None)
         return _extrema_by(it, getter, self._selector, self._comparer, self._for_min)
 
     # please maintain same overloads
-    def first(self, *args):  # pyright: reportIncompatibleMethodOverride=false
+    def first(self, *args):  # pyright: ignore[reportIncompatibleMethodOverride]
         if len(args) == 0:
             return MoreEnumerable.first(self.take(1))
         else:  # len(args) == 1
             return super().first(*args)
 
     # please maintain same overloads
     def first2(self, *args):
```

### Comparing `types-linq-1.2.0/types_linq/more/extrema_enumerable.pyi` & `types-linq-1.2.1/types_linq/more/extrema_enumerable.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -6,25 +6,25 @@
     TKey,
     TSource_co,
 )
 
 
 class ExtremaEnumerable(MoreEnumerable[TSource_co], Generic[TSource_co, TKey]):
     '''
-    .. code-block:: python
-
-        from types_linq.more.extrema_enumerable import ExtremaEnumerable
+    ```py
+    from types_linq.more.extrema_enumerable import ExtremaEnumerable
+    ```
 
     Specialization for manipulating extrema.
 
-    Users should not construct instances of this class directly. Use ``MoreEnumerable.maxima_by()``
+    Users should not construct instances of this class directly. Use `MoreEnumerable.maxima_by()`
     instead.
 
-    Revisions:
-        - v0.2.0: New.
+    Revisions
+        ~ v0.2.0: New.
     '''
 
     def __init__(self,
         source: Iterable[TSource_co],
         selector: Callable[[TSource_co], TKey],
         comparer: Optional[Callable[[TKey, TKey], int]],
         for_min: bool,
@@ -37,15 +37,15 @@
         '''
 
     @overload
     def take(self, __index: slice) -> Enumerable[TSource_co]:
         '''
         Identical to parent.
 
-        Revisions:
-            - v1.1.0: Fixed incorrect override of Enumerable.take() when it takes a slice.
+        Revisions
+            ~ v1.1.0: Fixed incorrect override of `Enumerable.take()` when it takes a slice.
         '''
 
     def take_last(self, count: int) -> MoreEnumerable[TSource_co]:
         '''
         Returns a new sequence that contains the last `count` elements.
         '''
```

### Comparing `types-linq-1.2.0/types_linq/more/more_enumerable.py` & `types-linq-1.2.1/types_linq/more/more_enumerable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 from typing import Any, Callable, Deque, Iterable, Iterator, List, Optional, TYPE_CHECKING, Tuple
 
 if TYPE_CHECKING:
     from .extrema_enumerable import ExtremaEnumerable
 
+from .more_enums import RankMethods
+from .more_error import DirectedGraphNotAcyclicError
 from ..enumerable import Enumerable
 from ..util import (
     ComposeMap,
     ComposeSet,
     default_equal,
     identity,
 )
@@ -36,15 +38,15 @@
             except StopIteration:
                 self._raise_empty_sequence()
 
         for elem in it:
             seed = func(elem, seed)
         return result_selector(seed)
 
-    def as_more(self) -> MoreEnumerable[TSource_co]:  # pyright: reportIncompatibleMethodOverride=false
+    def as_more(self) -> MoreEnumerable[TSource_co]:  # pyright: ignore[reportIncompatibleMethodOverride]
         return self
 
     def consume(self) -> None:
         for _ in self:
             ...
 
     def cycle(self, count: Optional[int] = None) -> MoreEnumerable[TSource_co]:
@@ -176,47 +178,55 @@
             yield identity
             for elem in it:
                 aggregator = transformation(aggregator, past)
                 yield aggregator
                 past = elem
         return MoreEnumerable(inner)
 
-    def rank(self, *args: Callable[[TSource_co, TSource_co], int]) -> MoreEnumerable[int]:
-        return self.rank_by(identity, *args)
+    def rank(self,
+        *args: Callable[[TSource_co, TSource_co], int],
+        method: RankMethods = RankMethods.dense,
+    ) -> MoreEnumerable[int]:
+        return self.rank_by(identity, *args, method=method)
 
     def rank_by(self,
         key_selector: Callable[[TSource_co], TKey],
-        *args: Callable[[TKey, TKey], int]) -> MoreEnumerable[int]:
+        *args: Callable[[TKey, TKey], int],
+        method: RankMethods = RankMethods.dense,
+     ) -> MoreEnumerable[int]:
         if len(args) == 0:
-            comparer = None
+            # it is sufficient to have only equality
+            comparer = lambda l, r: 0 if l == r else 1
         else:  # len(args) == 1
             comparer = args[0]
 
         def inner():
             # avoid enumerating twice
-            copy = MoreEnumerable(self.select(key_selector).to_list())
-            ordered = copy.distinct() \
-                .order_by_descending(identity, *args)
-            if comparer is None:
-                # replaces .enumerate()
-                rank_map = ComposeMap(ordered.select2(lambda x, i: (x, i + 1)))
-            else:
-                # this is different from morelinq
-                ordered = ordered.to_list()
-                if not ordered:
-                    return
-                rank_map = ComposeMap()
-                rank_map[ordered[0]] = 1
-                rank = 1
-                for i in range(1, len(ordered)):
-                    if comparer(ordered[i - 1], ordered[i]) != 0:
-                        rank += 1
-                    rank_map[ordered[i]] = rank
-            for key in copy:
-                yield rank_map[key]
+            copy = self.select(key_selector).to_list()
+            if not copy:
+                return
+            l = len(copy)
+            ordered = MoreEnumerable(range(l)) \
+                .order_by_descending(lambda i: copy[i], *args).to_list()
+            rank_map = [0] * l
+            rank_map[ordered[0]] = 1
+            rank = 1
+            consec = 1
+            for i in range(1, l):
+                if method == RankMethods.ordinal:
+                    rank += 1
+                elif comparer(copy[ordered[i - 1]], copy[ordered[i]]) != 0:
+                    rank += consec
+                    consec = 1
+                elif method == RankMethods.competitive:
+                    consec += 1
+                rank_map[ordered[i]] = rank
+            del ordered
+            for i in rank_map:
+                yield i
         return MoreEnumerable(inner)
 
     def run_length_encode(self,
         *args: Callable[[TSource_co, TSource_co], bool],
     ) -> MoreEnumerable[Tuple[TSource_co, int]]:
         if len(args) == 0:
             comparer = default_equal
@@ -335,10 +345,49 @@
     ) -> MoreEnumerable[TSource]:
         def inner():
             stack = [root]
             while stack:
                 elem = stack.pop()
                 yield elem
                 children = [*children_selector(elem)]
-                for children in reversed(children):
-                    stack.append(children)
+                for child in reversed(children):
+                    stack.append(child)
+        return MoreEnumerable(inner)
+
+    def traverse_topological(self,
+        children_selector: Callable[[TSource_co], Iterable[TSource_co]],
+    ) -> MoreEnumerable[TSource_co]:
+        return self.traverse_topological2(children_selector, identity)
+
+    def traverse_topological2(self,
+        children_selector: Callable[[TSource_co], Iterable[TSource_co]],
+        key_selector: Callable[[TSource_co], object],
+    ) -> MoreEnumerable[TSource_co]:
+        def inner():
+            stack: List[Tuple[TSource_co, bool]] = []
+            visited = ComposeMap()
+            result: List[TSource_co] = []  # post order
+            result_keys = ComposeSet()
+            # NOTE: a copy of the sequence is made in this call because it falls back
+            for root in self.reverse():
+                if not visited.get(key_selector(root)):
+                    stack.append((root, False))
+                while stack:
+                    node, done = stack.pop()
+                    if done:
+                        # detect cycle. normally edges from node will go to nodes in the
+                        # result list. otherwise we found cycle
+                        for child in children_selector(node):
+                            if key_selector(child) not in result_keys:
+                                raise DirectedGraphNotAcyclicError((node, child))
+                        # good
+                        result.append(node)
+                        result_keys.add(key_selector(node))
+                        continue
+                    visited[key_selector(node)] = True
+                    stack.append((node, True))
+                    for child in children_selector(node):
+                        if not visited.get(key_selector(child)):
+                            stack.append((child, False))
+            while result:
+                yield result.pop()
         return MoreEnumerable(inner)
```

### Comparing `types-linq-1.2.0/types_linq/more/more_enumerable.pyi` & `types-linq-1.2.1/types_linq/more/more_enumerable.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,162 +1,175 @@
 from typing import Any, Callable, Iterable, Optional, Tuple, overload
 
 from ..enumerable import Enumerable
 from .extrema_enumerable import ExtremaEnumerable
+from .more_enums import RankMethods
 from ..more_typing import (
     TAccumulate,
     TKey,
     TResult,
     TSource,
     TSource_co,
     TSupportsLessThan,
 )
 
 
 class MoreEnumerable(Enumerable[TSource_co]):
     '''
-    .. code-block:: python
-
-        from types_linq.more import MoreEnumerable
+    ```py
+    from types_linq.more import MoreEnumerable
+    ```
 
     MoreEnumerable provides more query methods. Instances of this class can be created by directly
-    constructing, using as_more(), or invoking MoreEnumerable methods that return MoreEnumerable
+    constructing, using `as_more()`, or invoking MoreEnumerable methods that return MoreEnumerable
     instead of Enumerable.
 
     These APIs may have breaking changes more frequently than those in Enumerable class because updates
     in .NET are happening and sometimes ones of these APIs could be moved to Enumerable with modification,
     or changed to accommodate changes to Enumerable.
 
-    Revisions:
-        - v0.2.0: New.
+    Revisions
+        ~ v0.2.0: New.
     '''
 
     @overload
     def aggregate_right(self,
         __seed: TAccumulate,
         __func: Callable[[TSource_co, TAccumulate], TAccumulate],
         __result_selector: Callable[[TAccumulate], TResult],
     ) -> TResult:
         '''
         Applies a right-associative accumulator function over the sequence. The seed is used as
         the initial accumulator value, and the result_selector is used to select the result value.
 
-        Revisions:
-            - v1.2.0: Fixed annotation for __func.
+        Revisions
+            ~ v1.2.0: Fixed annotation for __func.
         '''
 
     @overload
     def aggregate_right(self,
         __seed: TAccumulate,
         __func: Callable[[TSource_co, TAccumulate], TAccumulate],
     ) -> TAccumulate:
         '''
         Applies a right-associative accumulator function over the sequence. The seed is used as the
         initial accumulator value.
 
-        Example:
-            >>> values = [9, 4, 2]
-            >>> MoreEnumerable(values).aggregate_right('null', lambda e, rr: f'(cons {e} {rr})')
-            '(cons 9 (cons 4 (cons 2 null)))'
+        Example
+        ```py
+        >>> values = [9, 4, 2]
+        >>> MoreEnumerable(values).aggregate_right('null', lambda e, rr: f'(cons {e} {rr})')
+        '(cons 9 (cons 4 (cons 2 null)))'
+        ```
 
-        Revisions:
-            - v1.2.0: Fixed annotation for __func.
+        Revisions
+            ~ v1.2.0: Fixed annotation for __func.
         '''
 
     @overload
     def aggregate_right(self,
         __func: Callable[[TSource_co, TSource_co], TSource_co],
     ) -> TSource_co:
         '''
         Applies a right-associative accumulator function over the sequence. Raises `InvalidOperationError`
         if there is no value in the sequence.
 
         Example
-            >>> values = ['9', '4', '2', '5']
-            >>> MoreEnumerable(values).aggregate_right(lambda e, rr: f'({e}+{rr})')
-            '(9+(4+(2+5)))'
+        ```py
+        >>> values = ['9', '4', '2', '5']
+        >>> MoreEnumerable(values).aggregate_right(lambda e, rr: f'({e}+{rr})')
+        '(9+(4+(2+5)))'
+        ```
 
-        Revisions:
-            - v1.2.0: Fixed annotation for __func.
+        Revisions
+            ~ v1.2.0: Fixed annotation for __func.
         '''
 
     def as_more(self) -> MoreEnumerable[TSource_co]:
         '''
         Returns the original MoreEnumerable reference.
         '''
 
     def consume(self) -> None:
         '''
         Consumes the sequence completely. This method iterates the sequence immediately and does not save
         any intermediate data.
 
-        Revisions:
-            - v1.1.0: New.
+        Revisions
+            ~ v1.1.0: New.
         '''
 
     def cycle(self, count: Optional[int] = None) -> MoreEnumerable[TSource_co]:
         '''
         Repeats the sequence `count` times.
 
         If `count` is `None`, the sequence is infinite. Raises `InvalidOperationError` if `count`
         is negative.
 
         Example
-            >>> MoreEnumerable([1, 2, 3]).cycle(3).to_list()
-            [1, 2, 3, 1, 2, 3, 1, 2, 3]
+        ```py
+        >>> MoreEnumerable([1, 2, 3]).cycle(3).to_list()
+        [1, 2, 3, 1, 2, 3, 1, 2, 3]
+        ```
 
-        Revisions:
-            - v1.1.0: New.
+        Revisions
+            ~ v1.1.0: New.
         '''
 
     def enumerate(self, start: int = 0) -> MoreEnumerable[Tuple[int, TSource_co]]:
         '''
         Returns a sequence of tuples containing the index and the value from the source sequence. `start`
         is used to specify the starting index.
 
         Example
-            >>> ints = [2, 4, 6]
-            >>> MoreEnumerable(ints).enumerate().to_list()
-            [(0, 2), (1, 4), (2, 6)]
+        ```py
+        >>> ints = [2, 4, 6]
+        >>> MoreEnumerable(ints).enumerate().to_list()
+        [(0, 2), (1, 4), (2, 6)]
+        ```
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.0.0: New.
         '''
 
     def except_by2(self,
         second: Iterable[TSource_co],
         key_selector: Callable[[TSource_co], object],
     ) -> MoreEnumerable[TSource_co]:
         '''
         Produces the set difference of two sequences: self - second, according to a key selector that
         determines "distinctness". Note the second iterable is homogenous to self.
 
         Example
-            >>> first = [(16, 'x'), (9, 'y'), (12, 'd'), (16, 't')]
-            >>> second = [(24, 'd'), (77, 'y')]
-            >>> MoreEnumerable(first).except_by2(second, lambda x: x[1]).to_list()
-            [(16, 'x'), (16, 't')]
-
-        Revisions:
-            - v1.0.0: Renamed from ``except_by()`` to this name to accommodate the update to Enumerable class.
-            - v0.2.1: Added preliminary support for unhashable keys.
+        ```py
+        >>> first = [(16, 'x'), (9, 'y'), (12, 'd'), (16, 't')]
+        >>> second = [(24, 'd'), (77, 'y')]
+        >>> MoreEnumerable(first).except_by2(second, lambda x: x[1]).to_list()
+        [(16, 'x'), (16, 't')]
+        ```
+
+        Revisions
+            ~ v1.0.0: Renamed from `except_by()` to this name to accommodate an update to Enumerable class.
+            ~ v0.2.1: Added preliminary support for unhashable keys.
         '''
 
     @overload
     def flatten(self) -> MoreEnumerable[Any]:
         '''
         Flattens the sequence containing arbitrarily-nested subsequences.
 
         Note: the nested objects must be Iterable to be flatten.
         Instances of `str` or `bytes` are not flattened.
 
         Example
-            >>> lst = ['apple', ['orange', ['juice', 'mango'], 'delta function']]
-            >>> MoreEnumerable(lst).flatten().to_list()
-            ['apple', 'orange', 'juice', 'mango', 'delta function']
+        ```py
+        >>> lst = ['apple', ['orange', ['juice', 'mango'], 'delta function']]
+        >>> MoreEnumerable(lst).flatten().to_list()
+        ['apple', 'orange', 'juice', 'mango', 'delta function']
+        ```
         '''
 
     @overload
     def flatten(self, __predicate: Callable[[Iterable[Any]], bool]) -> MoreEnumerable[Any]:
         '''
         Flattens the sequence containing arbitrarily-nested subsequences. A predicate function determines
         whether a nested iterable should be flattened or not.
@@ -172,53 +185,57 @@
         '''
 
     def for_each(self, action: Callable[[TSource_co], object]) -> None:
         '''
         Executes the given function on each element in the source sequence. The return values are discarded.
 
         Example
-            .. code-block:: python
-
-                >>> def gen():
-                ...     yield 116; yield 35; yield -9
-
-                >>> Enumerable(gen()).where(lambda x: x > 0).as_more().for_each(print)
-                116
-                35
+        ```py
+        >>> def gen():
+        ...     yield 116; yield 35; yield -9
+
+        >>> Enumerable(gen()).where(lambda x: x > 0).as_more().for_each(print)
+        116
+        35
+        ```
         '''
 
     def for_each2(self, action: Callable[[TSource_co, int], object]) -> None:
         '''
         Executes the given function on each element in the source sequence. Each element's index is used in
         the logic of the function. The return values are discarded.
         '''
 
     def interleave(self, *iters: Iterable[TSource_co]) -> MoreEnumerable[TSource_co]:
         '''
         Interleaves the elements of two or more sequences into a single sequence, skipping sequences if they
         are consumed.
 
         Example
-            >>> MoreEnumerable(['1', '2']).interleave(['4', '5', '6'], ['7', '8', '9']).to_list()
-            ['1', '4', '7', '2', '5', '8', '6', '9']
+        ```py
+        >>> MoreEnumerable(['1', '2']).interleave(['4', '5', '6'], ['7', '8', '9']).to_list()
+        ['1', '4', '7', '2', '5', '8', '6', '9']
+        ```
         '''
 
     @overload
     def maxima_by(self,
         selector: Callable[[TSource_co], TSupportsLessThan],
     ) -> ExtremaEnumerable[TSource_co, TSupportsLessThan]:
         '''
         Returns the maximal elements of the sequence based on the given selector.
 
         Example
-            >>> strings = ['foo', 'bar', 'cheese', 'orange', 'baz', 'spam', 'egg', 'toasts', 'dish']
-            >>> MoreEnumerable(strings).maxima_by(len).to_list()
-            ['cheese', 'orange', 'toasts']
-            >>> MoreEnumerable(strings).maxima_by(lambda x: x.count('e')).first()
-            'cheese'
+        ```py
+        >>> strings = ['foo', 'bar', 'cheese', 'orange', 'baz', 'spam', 'egg', 'toasts', 'dish']
+        >>> MoreEnumerable(strings).maxima_by(len).to_list()
+        ['cheese', 'orange', 'toasts']
+        >>> MoreEnumerable(strings).maxima_by(lambda x: x.count('e')).first()
+        'cheese'
+        ```
         '''
 
     @overload
     def maxima_by(self,
         selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
     ) -> ExtremaEnumerable[TSource_co, TKey]:
@@ -251,293 +268,412 @@
 
     def pipe(self, action: Callable[[TSource_co], object]) -> MoreEnumerable[TSource_co]:
         '''
         Executes the given action on each element in the sequence and yields it. Return values of
         action are discarded.
 
         Example
-            >>> store = set()
-            >>> MoreEnumerable([1, 2, 2, 1]).pipe(store.add).where(lambda x: x % 2 == 0).to_list()
-            [2, 2]
-            >>> store
-            {1, 2}
+        ```py
+        >>> store = set()
+        >>> MoreEnumerable([1, 2, 2, 1]).pipe(store.add).where(lambda x: x % 2 == 0).to_list()
+        [2, 2]
+        >>> store
+        {1, 2}
+        ```
 
-        Revisions:
-            - v0.2.1: New.
+        Revisions
+            ~ v0.2.1: New.
         '''
 
     # note: diffrent from morelinq: identity is first parameter
     def pre_scan(self,
         identity: TAccumulate,
         transformation: Callable[[TAccumulate, TSource_co], TAccumulate],
     ) -> MoreEnumerable[TAccumulate]:
         '''
         Performs a pre-scan (exclusive prefix sum) over the sequence. Such scan returns an
         equal-length sequence where the first element is the identity, and i-th element (i>1) is
         the sum of the first i-1 (and identity) elements in the original sequence.
 
         Example
-            >>> values = [9, 4, 2, 5, 7]
-            >>> MoreEnumerable(values).pre_scan(0, lambda acc, e: acc + e).to_list()
-            [0, 9, 13, 15, 20]
-            >>> MoreEnumerable([]).pre_scan(0, lambda acc, e: acc + e).to_list()
-            []
-
-        Revisions:
-            - v1.2.0: New.
+        ```py
+        >>> values = [9, 4, 2, 5, 7]
+        >>> MoreEnumerable(values).pre_scan(0, lambda acc, e: acc + e).to_list()
+        [0, 9, 13, 15, 20]
+        >>> MoreEnumerable([]).pre_scan(0, lambda acc, e: acc + e).to_list()
+        []
+        ```
+
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     @overload
-    def rank(self: MoreEnumerable[TSupportsLessThan]) -> MoreEnumerable[int]:
+    def rank(self: MoreEnumerable[TSupportsLessThan],
+        *,
+        method: RankMethods = RankMethods.dense,
+    ) -> MoreEnumerable[int]:
         '''
-        Ranks each item in the sequence in descending order.
+        Ranks each item in the sequence in descending order using the method provided.
 
         Example
-            >>> scores = [1, 4, 77, 23, 23, 4, 9, 0, -7, 101, 23]
-            >>> MoreEnumerable(scores).rank().to_list()
-            [6, 5, 2, 3, 3, 5, 4, 7, 8, 1, 3]  # 101 is largest, so has rank of 1
+        ```py
+        >>> scores = [1, 4, 77, 23, 23, 4, 9, 0, -7, 101, 23]
+        >>> MoreEnumerable(scores).rank().to_list()
+        [6, 5, 2, 3, 3, 5, 4, 7, 8, 1, 3]  # 101 is largest, so has rank of 1
+
+        >>> MoreEnumerable(scores).rank(method=RankMethods.competitive).to_list()
+        [9, 7, 2, 3, 3, 7, 6, 10, 11, 1, 3]  # there are no 4th or 5th since there
+                                             # are three 3rd's
 
-        Revisions:
-            - v1.0.0: New.
+        >>> MoreEnumerable(scores).rank(method=RankMethods.ordinal).to_list()
+        [9, 7, 2, 3, 4, 8, 6, 10, 11, 1, 5]  # as in sorting
+        ```
+
+        Revisions
+            ~ v1.2.1: Added method parameter to support more ranking methods.
+            ~ v1.0.0: New.
         '''
 
     @overload
-    def rank(self, __comparer: Callable[[TSource_co, TSource_co], int]) -> MoreEnumerable[int]:
+    def rank(self,
+        __comparer: Callable[[TSource_co, TSource_co], int],
+        *,
+        method: RankMethods = RankMethods.dense,
+    ) -> MoreEnumerable[int]:
         '''
-        Ranks each item in the sequence in descending order using the given comparer.
+        Ranks each item in the sequence in descending order using the given comparer and the
+        method.
 
         Such comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal.
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.2.1: Added method parameter to support more ranking methods.
+            ~ v1.0.0: New.
         '''
 
     @overload
-    def rank_by(self, key_selector: Callable[[TSource_co], TSupportsLessThan]) -> MoreEnumerable[int]:
+    def rank_by(self,
+        key_selector: Callable[[TSource_co], TSupportsLessThan],
+        *,
+        method: RankMethods = RankMethods.dense,
+    ) -> MoreEnumerable[int]:
         '''
-        Ranks each item in the sequence in descending order using the given selector.
+        Ranks each item in the sequence in descending order using the given selector and the
+        method.
 
         Example
-            .. code-block:: python
-
-                >>> scores = [
-                ...     {'name': 'Frank', 'score': 75},
-                ...     {'name': 'Alica', 'score': 90},
-                ...     {'name': 'Erika', 'score': 99},
-                ...     {'name': 'Rogers', 'score': 90},
-                ... ]
-
-                >>> MoreEnumerable(scores).rank_by(lambda x: x['score']) \\
-                ...     .zip(scores) \\
-                ...     .group_by(lambda t: t[0], lambda t: t[1]['name']) \\
-                ...     .to_dict(lambda g: g.key, lambda g: g.to_list())
-                {3: ['Frank'], 2: ['Alica', 'Rogers'], 1: ['Erika']}
-
-        Revisions:
-            - v1.0.0: New.
+        ```py
+        >>> scores = [
+        ...     {'name': 'Frank', 'score': 75},
+        ...     {'name': 'Alica', 'score': 90},
+        ...     {'name': 'Erika', 'score': 99},
+        ...     {'name': 'Rogers', 'score': 90},
+        ... ]
+
+        >>> MoreEnumerable(scores).rank_by(lambda x: x['score']) \\
+        ...     .zip(scores) \\
+        ...     .group_by(lambda t: t[0], lambda t: t[1]['name']) \\
+        ...     .to_dict(lambda g: g.key, lambda g: g.to_list())
+        {3: ['Frank'], 2: ['Alica', 'Rogers'], 1: ['Erika']}
+        ```
+
+        Revisions
+            ~ v1.2.1: Added method parameter to support more ranking methods.
+            ~ v1.0.0: New.
         '''
 
     @overload
     def rank_by(self,
         key_selector: Callable[[TSource_co], TKey],
         __comparer: Callable[[TKey, TKey], int],
+        *,
+        method: RankMethods = RankMethods.dense,
     ) -> MoreEnumerable[int]:
         '''
-        Ranks each item in the sequence in descending order using the given selector and comparer.
+        Ranks each item in the sequence in descending order using the given selector, comparer
+        and the method.
 
         Such comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal.
 
-        Revisions:
-            - v1.0.0: New.
+        Revisions
+            ~ v1.2.1: Added method parameter to support more ranking methods.
+            ~ v1.0.0: New.
         '''
 
     @overload
     def run_length_encode(self) -> MoreEnumerable[Tuple[TSource_co, int]]:
         '''
         Run-length encodes the sequence into a sequence of tuples where each tuple contains an
         (the first) element and its number of contingent occurrences, where equality is based on
         `==`.
 
         Example
-            >>> MoreEnumerable('abbcaeeeaa').run_length_encode().to_list()
-            [('a', 1), ('b', 2), ('c', 1), ('a', 1), ('e', 3), ('a', 2)]
+        ```py
+        >>> MoreEnumerable('abbcaeeeaa').run_length_encode().to_list()
+        [('a', 1), ('b', 2), ('c', 1), ('a', 1), ('e', 3), ('a', 2)]
+        ```
 
-        Revisions:
-            - v1.1.0: New.
+        Revisions
+            ~ v1.1.0: New.
         '''
 
     @overload
     def run_length_encode(self,
         __comparer: Callable[[TSource_co, TSource_co], bool],
     ) -> MoreEnumerable[Tuple[TSource_co, int]]:
         '''
         Run-length encodes the sequence into a sequence of tuples where each tuple contains an
         (the first) element and its number of contingent occurrences, where equality is determined by
         the comparer.
 
         Example
-            >>> MoreEnumerable('abBBbcaEeeff') \\
-            >>>     .run_length_encode(lambda x, y: x.lower() == y.lower()).to_list()
-            [('a', 1), ('b', 4), ('c', 1), ('a', 1), ('E', 3), ('f', 2)]
+        ```py
+        >>> MoreEnumerable('abBBbcaEeeff') \\
+        >>>     .run_length_encode(lambda x, y: x.lower() == y.lower()).to_list()
+        [('a', 1), ('b', 4), ('c', 1), ('a', 1), ('E', 3), ('f', 2)]
+        ```
 
-        Revisions:
-            - v1.1.0: New.
+        Revisions
+            ~ v1.1.0: New.
         '''
 
     @overload
     def scan(self,
         __transformation: Callable[[TSource_co, TSource_co], TSource_co],
     ) -> MoreEnumerable[TSource_co]:
         '''
         Performs a inclusive prefix sum over the sequence. Such scan returns an equal-length sequence
         where the i-th element is the sum of the first i elements in the original sequence.
 
         Example
-            >>> values = [9, 4, 2, 5, 7]
-            >>> MoreEnumerable(values).scan(lambda acc, e: acc + e).to_list()
-            [9, 13, 15, 20, 27]
-            >>> MoreEnumerable([]).scan(lambda acc, e: acc + e).to_list()
-            []
-
-        Example
-            >>> # running max
-            >>> fruits = ['apple', 'mango', 'orange', 'passionfruit', 'grape']
-            >>> MoreEnumerable(fruits).scan(lambda acc, e: e if len(e) > len(acc) else acc).to_list()
-            ['apple', 'apple', 'orange', 'passionfruit', 'passionfruit']
+        ```py
+        >>> values = [9, 4, 2, 5, 7]
+        >>> MoreEnumerable(values).scan(lambda acc, e: acc + e).to_list()
+        [9, 13, 15, 20, 27]
+        >>> MoreEnumerable([]).scan(lambda acc, e: acc + e).to_list()
+        []
+        ```
+
+        Example
+        ```py
+        >>> # running max
+        >>> fruits = ['apple', 'mango', 'orange', 'passionfruit', 'grape']
+        >>> MoreEnumerable(fruits).scan(lambda acc, e: e if len(e) > len(acc) else acc).to_list()
+        ['apple', 'apple', 'orange', 'passionfruit', 'passionfruit']
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     @overload
     def scan(self,
         __seed: TAccumulate,
         __transformation: Callable[[TAccumulate, TSource_co], TAccumulate],
     ) -> MoreEnumerable[TAccumulate]:
         '''
         Like Enumerable.aggregate(seed, transformation) except that the intermediate results are
         included in the result sequence.
 
         Example
-            >>> Enumerable.range(1, 5).as_more().scan(-1, lambda acc, e: acc * e).to_list()
-            [-1, -1, -2, -6, -24, -120]
+        ```py
+        >>> Enumerable.range(1, 5).as_more().scan(-1, lambda acc, e: acc * e).to_list()
+        [-1, -1, -2, -6, -24, -120]
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     @overload
     def scan_right(self,
         __func: Callable[[TSource_co, TSource_co], TSource_co],
     ) -> MoreEnumerable[TSource_co]:
         '''
         Performs a right-associative inclusive prefix sum over the sequence. This is the
         right-associative version of MoreEnumerable.scan(func).
 
         Example
-            >>> values = ['9', '4', '2', '5']
-            >>> MoreEnumerable(values).scan_right(lambda e, rr: f'({e}+{rr})').to_list()
-            ['(9+(4+(2+5)))', '(4+(2+5))', '(2+5)', '5']
-            >>> MoreEnumerable([]).scan_right(lambda e, rr: e + rr).to_list()
-            []
+        ```py
+        >>> values = ['9', '4', '2', '5']
+        >>> MoreEnumerable(values).scan_right(lambda e, rr: f'({e}+{rr})').to_list()
+        ['(9+(4+(2+5)))', '(4+(2+5))', '(2+5)', '5']
+        >>> MoreEnumerable([]).scan_right(lambda e, rr: e + rr).to_list()
+        []
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     @overload
     def scan_right(self,
         __seed: TAccumulate,
         __func: Callable[[TSource_co, TAccumulate], TAccumulate],
     ) -> MoreEnumerable[TAccumulate]:
         '''
         The right-associative version of MoreEnumerable.scan(seed, func).
 
         Example
-            >>> values = [9, 4, 2]
-            >>> MoreEnumerable(values).scan_right('null', lambda e, rr: f'(cons {e} {rr})').to_list()
-            ['(cons 9 (cons 4 (cons 2 null)))', '(cons 4 (cons 2 null))', '(cons 2 null)', 'null']
+        ```py
+        >>> values = [9, 4, 2]
+        >>> MoreEnumerable(values).scan_right('null', lambda e, rr: f'(cons {e} {rr})').to_list()
+        ['(cons 9 (cons 4 (cons 2 null)))', '(cons 4 (cons 2 null))', '(cons 2 null)', 'null']
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     def segment(self,
         new_segment_predicate: Callable[[TSource_co], bool],
     ) -> MoreEnumerable[MoreEnumerable[TSource_co]]:
         '''
         Splits the sequence into segments by using a detector function that returns True to signal a
         new segment.
 
         Example
-            >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
-            >>> MoreEnumerable(values).segment(lambda x: x < 0).select(lambda x: x.to_list()).to_list()
-            [[0, 1, 2, 4], [-4], [-2, 6, 2], [-2]]
+        ```py
+        >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
+        >>> MoreEnumerable(values).segment(lambda x: x < 0).select(lambda x: x.to_list()).to_list()
+        [[0, 1, 2, 4], [-4], [-2, 6, 2], [-2]]
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     def segment2(self,
         new_segment_predicate: Callable[[TSource_co, int], bool],
     ) -> MoreEnumerable[MoreEnumerable[TSource_co]]:
         '''
         Splits the sequence into segments by using a detector function that returns True to signal a
         new segment. The element's index is used in the detector function.
 
         Example
-            >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
-            >>> MoreEnumerable(values).segment2(lambda x, i: x < 0 or i % 3 == 0) \\
-            ...     .select(lambda x: x.to_list()) \\
-            ...     .to_list()
-            [[0, 1, 2], [4], [-4], [-2], [6, 2], [-2]]
+        ```py
+        >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
+        >>> MoreEnumerable(values).segment2(lambda x, i: x < 0 or i % 3 == 0) \\
+        ...     .select(lambda x: x.to_list()) \\
+        ...     .to_list()
+        [[0, 1, 2], [4], [-4], [-2], [6, 2], [-2]]
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     def segment3(self,
         new_segment_predicate: Callable[[TSource_co, TSource_co, int], bool],
     ) -> MoreEnumerable[MoreEnumerable[TSource_co]]:
         '''
         Splits the sequence into segments by using a detector function that returns True to signal a
         new segment. The last element and the current element's index are used in the detector
         function.
 
         Example
-            >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
-            >>> MoreEnumerable(values).segment3(lambda curr, prev, i: curr * prev < 0) \\
-            ...     .select(lambda x: x.to_list()) \\
-            ...     .to_list()
-            [[0, 1, 2, 4], [-4, -2], [6, 2], [-2]]
+        ```py
+        >>> values = [0, 1, 2, 4, -4, -2, 6, 2, -2]
+        >>> MoreEnumerable(values).segment3(lambda curr, prev, i: curr * prev < 0) \\
+        ...     .select(lambda x: x.to_list()) \\
+        ...     .to_list()
+        [[0, 1, 2, 4], [-4, -2], [6, 2], [-2]]
+        ```
 
-        Revisions:
-            - v1.2.0: New.
+        Revisions
+            ~ v1.2.0: New.
         '''
 
     @staticmethod
     def traverse_breath_first(
         root: TSource,
         children_selector: Callable[[TSource], Iterable[TSource]],
     ) -> MoreEnumerable[TSource]:
         '''
         Traverses the tree (graph) from the root node in a breath-first fashion. A selector is used to
         select children of each node.
 
-        Graphs are not checked for cycles. If the resulting sequence needs to be finite then it is the
-        responsibility of children_selector to ensure that duplicate nodes are not visited.
+        Graphs are not checked for cycles or duplicates visits. If the resulting sequence needs to be
+        finite then it is the responsibility of children_selector to ensure that duplicate nodes are not
+        visited.
+
+        Example
+        ```py
+        >>> tree = { 3: [1, 4], 1: [0, 2], 4: [5] }
+        >>> MoreEnumerable.traverse_breath_first(3, lambda x: tree.get(x, [])) \\
+        >>>     .to_list()
+        [3, 1, 4, 0, 2, 5]
+        ```
         '''
 
     @staticmethod
     def traverse_depth_first(
         root: TSource,
         children_selector: Callable[[TSource], Iterable[TSource]],
     ) -> MoreEnumerable[TSource]:
         '''
         Traverses the tree (graph) from the root node in a depth-first fashion. A selector is used to
         select children of each node.
 
-        Graphs are not checked for cycles. If the resulting sequence needs to be finite then it is the
-        responsibility of children_selector to ensure that duplicate nodes are not visited.
+        Graphs are not checked for cycles or duplicates visits. If the resulting sequence needs to be
+        finite then it is the responsibility of children_selector to ensure that duplicate nodes are not
+        visited.
+
+        Example
+        ```py
+        >>> tree = { 3: [1, 4], 1: [0, 2], 4: [5] }
+        >>> MoreEnumerable.traverse_depth_first(3, lambda x: tree.get(x, [])) \\
+        >>>     .to_list()
+        [3, 1, 0, 2, 4, 5]
+        ```
+        '''
+
+    # NOTE: leave room for comparer overloads
+    # TODO: when hasher support is done
+    def traverse_topological(self,
+        children_selector: Callable[[TSource_co], Iterable[TSource_co]],
+    ) -> MoreEnumerable[TSource_co]:
+        '''
+        Traverses the graph in topological order, A selector is used to select children of each
+        node. The ordering created from this method is a variant of depth-first traversal and ensures
+        duplicate nodes are output once.
+
+        To invoke this method, the self sequence contains nodes with zero in-degrees to start the
+        iteration. Passing a list of all nodes is allowed although not required.
+
+        Raises `DirectedGraphNotAcyclicError` if the directed graph contains a cycle and the
+        topological ordering cannot be produced.
+
+        Example
+        ```py
+        >>> adj = { 5: [2, 0], 4: [0, 1], 2: [3], 3: [1] }
+        >>> MoreEnumerable([5, 4]).traverse_topological(lambda x: adj.get(x, [])) \\
+        >>>     .to_list()
+        [5, 2, 3, 4, 0, 1]
+        ```
+
+        Revisions
+            ~ v1.2.1: New.
+        '''
+
+    def traverse_topological2(self,
+        children_selector: Callable[[TSource_co], Iterable[TSource_co]],
+        key_selector: Callable[[TSource_co], object],
+    ) -> MoreEnumerable[TSource_co]:
+        '''
+        Traverses the graph in topological order, A selector is used to select children of each
+        node. The ordering created from this method is a variant of depth-first traversal and
+        ensures duplicate nodes are output once. A key selector is used to determine equality
+        between nodes.
+
+        To invoke this method, the self sequence contains nodes with zero in-degrees to start the
+        iteration. Passing a list of all nodes is allowed although not required.
+
+        Raises `DirectedGraphNotAcyclicError` if the directed graph contains a cycle and the
+        topological ordering cannot be produced.
+
+        Revisions
+            ~ v1.2.1: New.
         '''
```

### Comparing `types-linq-1.2.0/types_linq/ordered_enumerable.py` & `types-linq-1.2.1/types_linq/ordered_enumerable.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             else:
                 selector = curr._key_selector
                 class key:
                     def __init__(self, elem):
                         self.elem = elem
                     def __lt__(self, __o: key):
                         return comparer(selector(self.elem), selector(__o.elem)) < 0  # type: ignore
+                    # it is OK to omit __eq__() because python sort only uses __lt__()
             lst.sort(key=key, reverse=curr._descending)
             curr = curr._parent
         yield from lst
 
     def create_ordered_enumerable(self,
         key_selector: Callable[[TSource_co], TKey2],
         comparer: Optional[Callable[[TKey2, TKey2], int]],
```

### Comparing `types-linq-1.2.0/types_linq/ordered_enumerable.pyi` & `types-linq-1.2.1/types_linq/ordered_enumerable.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
     TKey2,
     TSupportsLessThan,
 )
 
 
 class OrderedEnumerable(Enumerable[TSource_co], Generic[TSource_co, TKey]):
     '''
-    .. code-block:: python
-
-        from types_linq.ordered_enumerable import OrderedEnumerable
+    ```py
+    from types_linq.ordered_enumerable import OrderedEnumerable
+    ```
 
     Represents a sorted Enumerable sequence that is sorted by some key.
 
-    Users should not construct instances of this class directly. Use ``Enumerable.order_by()`` instead.
+    Users should not construct instances of this class directly. Use `Enumerable.order_by()` instead.
     '''
 
     def __init__(self, *args): ...
 
     def create_ordered_enumerable(self,
         key_selector: Callable[[TSource_co], TKey2],
         comparer: Optional[Callable[[TKey2, TKey2], int]],
@@ -30,38 +30,38 @@
     ) -> OrderedEnumerable[TSource_co, TKey2]:
         '''
         Performs a subsequent ordering on the elements of the sequence according to a key.
 
         Comparer takes two values and return positive ints when lhs > rhs, negative ints
         if lhs < rhs, and 0 if they are equal.
 
-        Revisions:
-            - v0.1.2: Fixed incorrect parameter type of comparer.
+        Revisions
+            ~ v0.1.2: Fixed incorrect parameter type of comparer.
         '''
 
     @overload
     def then_by(self,
         key_selector: Callable[[TSource_co], TSupportsLessThan],
     ) -> OrderedEnumerable[TSource_co, TSupportsLessThan]:
         '''
         Performs a subsequent ordering of the elements in ascending order according to key.
 
         Example
-            .. code-block:: python
-
-                >>> class Pet(NamedTuple):
-                ...     name: str
-                ...     age: int
-
-                >>> pets = [Pet('Barley', 8), Pet('Boots', 4), Pet('Roman', 5), Pet('Daisy', 4)]
-                >>> Enumerable(pets).order_by(lambda p: p.age) \\
-                ...     .then_by(lambda p: p.name)             \\
-                ...     .select(lambda p: p.name)              \\
-                ...     .to_list()
-                ['Boots', 'Daisy', 'Roman', 'Barley']
+        ```py
+        >>> class Pet(NamedTuple):
+        ...     name: str
+        ...     age: int
+
+        >>> pets = [Pet('Barley', 8), Pet('Boots', 4), Pet('Roman', 5), Pet('Daisy', 4)]
+        >>> Enumerable(pets).order_by(lambda p: p.age) \\
+        ...     .then_by(lambda p: p.name)             \\
+        ...     .select(lambda p: p.name)              \\
+        ...     .to_list()
+        ['Boots', 'Daisy', 'Roman', 'Barley']
+        ```
         '''
 
     @overload
     def then_by(self,
         key_selector: Callable[[TSource_co], TKey2],
         __comparer: Callable[[TKey2, TKey2], int],
     ) -> OrderedEnumerable[TSource_co, TKey2]:
```

### Comparing `types-linq-1.2.0/types_linq/util.py` & `types-linq-1.2.1/types_linq/util.py`

 * *Files identical despite different names*

### Comparing `types-linq-1.2.0/types_linq.egg-info/PKG-INFO` & `types-linq-1.2.1/types_linq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-linq
-Version: 1.2.0
+Version: 1.2.1
 Summary: Standard sequence helper methods with full typing support
 Home-page: https://github.com/cleoold/types-linq
 Author: cleoold
 License: BSD 2-Clause License
 Description: # types-linq
         
         ![Python](https://img.shields.io/badge/python-3.7%2B-blue.svg) [![pypi](https://img.shields.io/pypi/v/types-linq)](https://pypi.org/project/types-linq/) [![pytest](https://github.com/cleoold/types-linq/workflows/pytest/badge.svg)](https://github.com/cleoold/types-linq/actions?query=workflow%3Apytest) [![codecov](https://codecov.io/gh/cleoold/types-linq/branch/main/graph/badge.svg?token=HTUKZ0SQJ3)](https://codecov.io/gh/cleoold/types-linq) [![Documentation Status](https://readthedocs.org/projects/types-linq/badge/?version=latest)](https://types-linq.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `types-linq-1.2.0/types_linq.egg-info/SOURCES.txt` & `types-linq-1.2.1/types_linq.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 types_linq.egg-info/not-zip-safe
 types_linq.egg-info/requires.txt
 types_linq.egg-info/top_level.txt
 types_linq/more/__init__.py
 types_linq/more/extrema_enumerable.py
 types_linq/more/extrema_enumerable.pyi
 types_linq/more/more_enumerable.py
-types_linq/more/more_enumerable.pyi
+types_linq/more/more_enumerable.pyi
+types_linq/more/more_enums.py
+types_linq/more/more_error.py
```

