# Comparing `tmp/danielutils-0.8.6.tar.gz` & `tmp/danielutils-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danielutils-0.8.6.tar", last modified: Sat Apr 29 22:22:51 2023, max compression
+gzip compressed data, was "danielutils-0.8.7.tar", last modified: Fri Jun  2 10:05:08 2023, max compression
```

## Comparing `danielutils-0.8.6.tar` & `danielutils-0.8.7.tar`

### file list

```diff
@@ -1,74 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.977510 danielutils-0.8.6/
--rw-rw-rw-   0        0        0     1967 2023-04-29 22:22:51.977510 danielutils-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     1259 2023-04-29 22:22:51.000000 danielutils-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.915449 danielutils-0.8.6/danielutils/
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.941274 danielutils-0.8.6/danielutils/Classes/
--rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.6/danielutils/Classes/Convenience.py
--rw-rw-rw-   0        0        0     4612 2023-04-21 07:35:02.000000 danielutils-0.8.6/danielutils/Classes/TypedBuiltins.py
--rw-rw-rw-   0        0        0      107 2023-04-20 18:11:11.000000 danielutils-0.8.6/danielutils/Classes/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-04-20 20:24:10.000000 danielutils-0.8.6/danielutils/Classes/frange.py
--rw-rw-rw-   0        0        0     3992 2023-04-29 17:53:23.000000 danielutils-0.8.6/danielutils/Colors.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.943279 danielutils-0.8.6/danielutils/Conversions/
--rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.6/danielutils/Conversions/MainConversions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.946339 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/
--rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/__init__.py
--rw-rw-rw-   0        0        0      476 2023-04-20 20:15:32.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/to_hex.py
--rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.6/danielutils/Conversions/SpecializedConversions/to_int.py
--rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.6/danielutils/Conversions/__init__.py
--rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.6/danielutils/Data.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.951878 danielutils-0.8.6/danielutils/DataStructures/
--rw-rw-rw-   0        0        0     1569 2023-04-20 20:36:21.000000 danielutils-0.8.6/danielutils/DataStructures/Comparer.py
--rw-rw-rw-   0        0        0     3299 2023-04-20 20:00:10.000000 danielutils-0.8.6/danielutils/DataStructures/Heap.py
--rw-rw-rw-   0        0        0      412 2023-04-20 20:11:14.000000 danielutils-0.8.6/danielutils/DataStructures/Node.py
--rw-rw-rw-   0        0        0     4428 2023-04-27 14:48:46.000000 danielutils-0.8.6/danielutils/DataStructures/Queue.py
--rw-rw-rw-   0        0        0       89 2023-04-29 16:43:01.000000 danielutils-0.8.6/danielutils/DataStructures/__init__.py
--rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.6/danielutils/DataStructures/functions.py
--rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.8.6/danielutils/DateTime.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.964499 danielutils-0.8.6/danielutils/Decorators/
--rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.8.6/danielutils/Decorators/PartiallyImplemented.py
--rw-rw-rw-   0        0        0      335 2023-04-29 21:26:25.000000 danielutils-0.8.6/danielutils/Decorators/__init__.py
--rw-rw-rw-   0        0        0      601 2023-04-29 17:43:40.000000 danielutils-0.8.6/danielutils/Decorators/atomic.py
--rw-rw-rw-   0        0        0     1195 2023-04-29 17:44:07.000000 danielutils-0.8.6/danielutils/Decorators/attach.py
--rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.8.6/danielutils/Decorators/chain_decorators.py
--rw-rw-rw-   0        0        0      845 2023-04-29 17:44:22.000000 danielutils-0.8.6/danielutils/Decorators/decorate_conditionally.py
--rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.8.6/danielutils/Decorators/delay_call.py
--rw-rw-rw-   0        0        0     1479 2023-04-29 17:44:59.000000 danielutils-0.8.6/danielutils/Decorators/limit_recursion.py
--rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.8.6/danielutils/Decorators/memo.py
--rw-rw-rw-   0        0        0     3991 2023-04-29 17:46:01.000000 danielutils-0.8.6/danielutils/Decorators/overload.py
--rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.8.6/danielutils/Decorators/threadify.py
--rw-rw-rw-   0        0        0     1736 2023-04-29 21:25:16.000000 danielutils-0.8.6/danielutils/Decorators/timeout.py
--rw-rw-rw-   0        0        0     9732 2023-04-29 17:50:06.000000 danielutils-0.8.6/danielutils/Decorators/validate.py
--rw-rw-rw-   0        0        0     2127 2023-04-20 19:47:46.000000 danielutils-0.8.6/danielutils/Exceptions.py
--rw-rw-rw-   0        0        0     5564 2023-04-21 15:43:35.000000 danielutils-0.8.6/danielutils/Functions.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.967499 danielutils-0.8.6/danielutils/Generators/
--rw-rw-rw-   0        0        0       32 2023-04-29 22:08:49.000000 danielutils-0.8.6/danielutils/Generators/__init__.py
--rw-rw-rw-   0        0        0     1025 2023-04-29 22:18:06.000000 danielutils-0.8.6/danielutils/Generators/join_generators.py
--rw-rw-rw-   0        0        0     9257 2023-04-26 09:21:09.000000 danielutils-0.8.6/danielutils/IO.py
--rw-rw-rw-   0        0        0     1846 2023-04-29 17:47:59.000000 danielutils-0.8.6/danielutils/Internet.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.973533 danielutils-0.8.6/danielutils/Math/
--rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.6/danielutils/Math/Constants.py
--rw-rw-rw-   0        0        0      347 2023-04-20 20:10:18.000000 danielutils-0.8.6/danielutils/Math/Functions.py
--rw-rw-rw-   0        0        0     1045 2023-04-20 18:34:15.000000 danielutils-0.8.6/danielutils/Math/MathPrint.py
--rw-rw-rw-   0        0        0     3779 2023-04-20 17:25:45.000000 danielutils-0.8.6/danielutils/Math/MathSymbols.py
--rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.6/danielutils/Math/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.976510 danielutils-0.8.6/danielutils/MetaClasses/
--rw-rw-rw-   0        0        0      742 2023-04-29 17:55:43.000000 danielutils-0.8.6/danielutils/MetaClasses/AtomicClassMeta.py
--rw-rw-rw-   0        0        0    10395 2023-04-29 17:55:35.000000 danielutils-0.8.6/danielutils/MetaClasses/Interface.py
--rw-rw-rw-   0        0        0       58 2023-04-29 16:46:20.000000 danielutils-0.8.6/danielutils/MetaClasses/__init__.py
--rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.6/danielutils/Path.py
--rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.6/danielutils/Print.py
--rw-rw-rw-   0        0        0     4529 2023-04-29 15:46:45.000000 danielutils-0.8.6/danielutils/Reflection.py
--rw-rw-rw-   0        0        0     6089 2023-04-20 19:51:00.000000 danielutils-0.8.6/danielutils/System.py
--rw-rw-rw-   0        0        0     4213 2023-04-29 18:00:25.000000 danielutils-0.8.6/danielutils/Text.py
--rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.6/danielutils/Time.py
--rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.8.6/danielutils/Windows.py
--rw-rw-rw-   0        0        0      664 2023-04-29 22:08:58.000000 danielutils-0.8.6/danielutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 22:22:51.935927 danielutils-0.8.6/danielutils.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1986 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 22:22:51.000000 danielutils-0.8.6/danielutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      728 2023-04-29 22:22:51.000000 danielutils-0.8.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 22:22:51.978839 danielutils-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0     1389 2023-04-29 22:22:51.000000 danielutils-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.395799 danielutils-0.8.7/
+-rw-rw-rw-   0        0        0     1967 2023-06-02 10:05:08.395799 danielutils-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1259 2023-06-02 10:05:07.000000 danielutils-0.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.345655 danielutils-0.8.7/danielutils/
+-rw-rw-rw-   0        0        0     4362 2023-06-02 08:57:30.000000 danielutils-0.8.7/danielutils/Aliases.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.354355 danielutils-0.8.7/danielutils/Classes/
+-rw-rw-rw-   0        0        0      210 2023-04-20 17:59:42.000000 danielutils-0.8.7/danielutils/Classes/Convenience.py
+-rw-rw-rw-   0        0        0     1144 2023-06-01 23:36:28.000000 danielutils-0.8.7/danielutils/Classes/Counter.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.359391 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/
+-rw-rw-rw-   0        0        0       96 2023-06-02 09:15:33.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/__init__.py
+-rw-rw-rw-   0        0        0      477 2023-05-01 13:03:04.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tbase.py
+-rw-rw-rw-   0        0        0     2042 2023-06-01 21:38:07.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tdict.py
+-rw-rw-rw-   0        0        0     1824 2023-06-01 23:26:15.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tlist.py
+-rw-rw-rw-   0        0        0      818 2023-05-01 13:01:21.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/tset.py
+-rw-rw-rw-   0        0        0      137 2023-06-02 09:13:53.000000 danielutils-0.8.7/danielutils/Classes/TypedBuiltins/ttuple.py
+-rw-rw-rw-   0        0        0      126 2023-05-01 13:01:32.000000 danielutils-0.8.7/danielutils/Classes/__init__.py
+-rw-rw-rw-   0        0        0     1047 2023-06-01 21:36:49.000000 danielutils-0.8.7/danielutils/Classes/frange.py
+-rw-rw-rw-   0        0        0     4763 2023-06-01 23:17:25.000000 danielutils-0.8.7/danielutils/Colors.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.360462 danielutils-0.8.7/danielutils/Conversions/
+-rw-rw-rw-   0        0        0     2227 2023-04-20 19:56:42.000000 danielutils-0.8.7/danielutils/Conversions/MainConversions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.363055 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/
+-rw-rw-rw-   0        0        0       46 2022-10-14 16:36:49.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-06-02 09:23:12.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/to_hex.py
+-rw-rw-rw-   0        0        0      407 2023-04-20 17:57:46.000000 danielutils-0.8.7/danielutils/Conversions/SpecializedConversions/to_int.py
+-rw-rw-rw-   0        0        0       71 2022-10-14 16:31:17.000000 danielutils-0.8.7/danielutils/Conversions/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-04-20 17:15:00.000000 danielutils-0.8.7/danielutils/Data.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.370063 danielutils-0.8.7/danielutils/DataStructures/
+-rw-rw-rw-   0        0        0     1056 2023-06-02 08:41:44.000000 danielutils-0.8.7/danielutils/DataStructures/Comparer.py
+-rw-rw-rw-   0        0        0     2264 2023-06-02 09:00:59.000000 danielutils-0.8.7/danielutils/DataStructures/Graph.py
+-rw-rw-rw-   0        0        0     3372 2023-06-02 08:43:49.000000 danielutils-0.8.7/danielutils/DataStructures/Heap.py
+-rw-rw-rw-   0        0        0     2620 2023-06-02 08:58:56.000000 danielutils-0.8.7/danielutils/DataStructures/Node.py
+-rw-rw-rw-   0        0        0     5065 2023-06-02 08:59:09.000000 danielutils-0.8.7/danielutils/DataStructures/Queue.py
+-rw-rw-rw-   0        0        0     1507 2023-06-01 23:41:53.000000 danielutils-0.8.7/danielutils/DataStructures/Stack.py
+-rw-rw-rw-   0        0        0      133 2023-05-10 19:33:24.000000 danielutils-0.8.7/danielutils/DataStructures/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-04-20 20:07:14.000000 danielutils-0.8.7/danielutils/DataStructures/functions.py
+-rw-rw-rw-   0        0        0      135 2023-04-21 22:43:20.000000 danielutils-0.8.7/danielutils/DateTime.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.379999 danielutils-0.8.7/danielutils/Decorators/
+-rw-rw-rw-   0        0        0      696 2023-04-29 17:38:05.000000 danielutils-0.8.7/danielutils/Decorators/PartiallyImplemented.py
+-rw-rw-rw-   0        0        0      361 2023-06-01 10:32:05.000000 danielutils-0.8.7/danielutils/Decorators/__init__.py
+-rw-rw-rw-   0        0        0      613 2023-06-01 23:35:30.000000 danielutils-0.8.7/danielutils/Decorators/atomic.py
+-rw-rw-rw-   0        0        0     1213 2023-06-01 22:03:38.000000 danielutils-0.8.7/danielutils/Decorators/attach.py
+-rw-rw-rw-   0        0        0      730 2023-04-29 17:58:20.000000 danielutils-0.8.7/danielutils/Decorators/chain_decorators.py
+-rw-rw-rw-   0        0        0      853 2023-06-01 23:23:43.000000 danielutils-0.8.7/danielutils/Decorators/decorate_conditionally.py
+-rw-rw-rw-   0        0        0      817 2023-04-29 18:02:16.000000 danielutils-0.8.7/danielutils/Decorators/delay_call.py
+-rw-rw-rw-   0        0        0      587 2023-06-01 10:37:25.000000 danielutils-0.8.7/danielutils/Decorators/deprecate.py
+-rw-rw-rw-   0        0        0     1479 2023-04-29 17:44:59.000000 danielutils-0.8.7/danielutils/Decorators/limit_recursion.py
+-rw-rw-rw-   0        0        0      622 2023-04-29 17:38:26.000000 danielutils-0.8.7/danielutils/Decorators/memo.py
+-rw-rw-rw-   0        0        0    10169 2023-06-02 09:22:26.000000 danielutils-0.8.7/danielutils/Decorators/overload.py
+-rw-rw-rw-   0        0        0      661 2023-05-21 20:38:07.000000 danielutils-0.8.7/danielutils/Decorators/property.py
+-rw-rw-rw-   0        0        0      595 2023-04-29 17:59:44.000000 danielutils-0.8.7/danielutils/Decorators/threadify.py
+-rw-rw-rw-   0        0        0     1730 2023-06-01 23:20:48.000000 danielutils-0.8.7/danielutils/Decorators/timeout.py
+-rw-rw-rw-   0        0        0     9642 2023-06-01 23:37:04.000000 danielutils-0.8.7/danielutils/Decorators/validate.py
+-rw-rw-rw-   0        0        0     2130 2023-04-30 19:46:55.000000 danielutils-0.8.7/danielutils/Exceptions.py
+-rw-rw-rw-   0        0        0     8761 2023-06-02 09:04:00.000000 danielutils-0.8.7/danielutils/Functions.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.383389 danielutils-0.8.7/danielutils/Generators/
+-rw-rw-rw-   0        0        0       70 2023-06-01 11:44:02.000000 danielutils-0.8.7/danielutils/Generators/__init__.py
+-rw-rw-rw-   0        0        0      450 2023-06-01 12:22:56.000000 danielutils-0.8.7/danielutils/Generators/generator_from_stream.py
+-rw-rw-rw-   0        0        0     2638 2023-06-01 23:35:56.000000 danielutils-0.8.7/danielutils/Generators/join_generators.py
+-rw-rw-rw-   0        0        0     9424 2023-06-01 22:39:00.000000 danielutils-0.8.7/danielutils/IO.py
+-rw-rw-rw-   0        0        0     1851 2023-06-01 22:39:25.000000 danielutils-0.8.7/danielutils/Internet.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.388073 danielutils-0.8.7/danielutils/Math/
+-rw-rw-rw-   0        0        0     7682 2023-04-20 20:14:55.000000 danielutils-0.8.7/danielutils/Math/Constants.py
+-rw-rw-rw-   0        0        0      341 2023-06-01 22:46:15.000000 danielutils-0.8.7/danielutils/Math/Functions.py
+-rw-rw-rw-   0        0        0     1061 2023-06-01 23:34:42.000000 danielutils-0.8.7/danielutils/Math/MathPrint.py
+-rw-rw-rw-   0        0        0     3815 2023-06-01 22:45:35.000000 danielutils-0.8.7/danielutils/Math/MathSymbols.py
+-rw-rw-rw-   0        0        0       80 2023-04-03 18:56:40.000000 danielutils-0.8.7/danielutils/Math/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.391847 danielutils-0.8.7/danielutils/MetaClasses/
+-rw-rw-rw-   0        0        0      724 2023-06-01 23:27:38.000000 danielutils-0.8.7/danielutils/MetaClasses/AtomicClassMeta.py
+-rw-rw-rw-   0        0        0     1950 2023-06-01 23:27:26.000000 danielutils-0.8.7/danielutils/MetaClasses/ImplicitDataDeleterMeta.py
+-rw-rw-rw-   0        0        0     1499 2023-05-01 12:50:48.000000 danielutils-0.8.7/danielutils/MetaClasses/InstanceCacheMeta.py
+-rw-rw-rw-   0        0        0    10521 2023-06-02 08:37:49.000000 danielutils-0.8.7/danielutils/MetaClasses/Interface.py
+-rw-rw-rw-   0        0        0       98 2023-04-30 22:02:36.000000 danielutils-0.8.7/danielutils/MetaClasses/__init__.py
+-rw-rw-rw-   0        0        0     1006 2023-01-12 01:01:37.000000 danielutils-0.8.7/danielutils/Path.py
+-rw-rw-rw-   0        0        0     2686 2023-04-11 13:05:54.000000 danielutils-0.8.7/danielutils/Print.py
+-rw-rw-rw-   0        0        0     5412 2023-06-01 22:35:02.000000 danielutils-0.8.7/danielutils/Reflection.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.394288 danielutils-0.8.7/danielutils/Snippets/
+-rw-rw-rw-   0        0        0       24 2023-06-01 14:01:33.000000 danielutils-0.8.7/danielutils/Snippets/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-06-01 14:01:26.000000 danielutils-0.8.7/danielutils/Snippets/try_get.py
+-rw-rw-rw-   0        0        0     6444 2023-06-01 22:24:03.000000 danielutils-0.8.7/danielutils/System.py
+-rw-rw-rw-   0        0        0     4213 2023-04-29 18:00:25.000000 danielutils-0.8.7/danielutils/Text.py
+-rw-rw-rw-   0        0        0      426 2023-04-11 21:07:07.000000 danielutils-0.8.7/danielutils/Time.py
+-rw-rw-rw-   0        0        0     2254 2023-04-21 15:17:41.000000 danielutils-0.8.7/danielutils/Windows.py
+-rw-rw-rw-   0        0        0      688 2023-06-01 17:00:29.000000 danielutils-0.8.7/danielutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 10:05:08.351697 danielutils-0.8.7/danielutils.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2616 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-02 10:05:08.000000 danielutils-0.8.7/danielutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      728 2023-06-02 10:05:07.000000 danielutils-0.8.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 10:05:08.395799 danielutils-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0     1389 2023-06-02 10:05:07.000000 danielutils-0.8.7/setup.py
```

### Comparing `danielutils-0.8.6/PKG-INFO` & `danielutils-0.8.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.6
+Version: 0.8.7
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.8.6
+# danielutils v=0.8.7
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 ## Further reading
 check out [READMES/readme.md](./READMES/readme.md) to check out some of the stuff this library can do
```

### Comparing `danielutils-0.8.6/README.md` & `danielutils-0.8.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.8.6
+# danielutils v=0.8.7
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 ## Further reading
 check out [READMES/readme.md](./READMES/readme.md) to check out some of the stuff this library can do
```

### Comparing `danielutils-0.8.6/danielutils/Classes/frange.py` & `danielutils-0.8.7/danielutils/Classes/frange.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """frange class"""
-from typing import Iterable, Callable
+from typing import Iterable, Callable, Optional
 
 
 class frange:
     """this class is the same like builtin range but with float values
     """
 
-    def __init__(self, start: float, stop: float = None,
+    def __init__(self, start: float, stop: Optional[float] = None,
                  step: float = 1, round_method: Callable[[float], float] = lambda f: round(f, 3)):
         if stop is None:
             stop = start
             start = 0
         self.start = start
         self.stop = stop
         self.step = step
```

### Comparing `danielutils-0.8.6/danielutils/Colors.py` & `danielutils-0.8.7/danielutils/Colors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from .Decorators.validate import validate
 
 
 class ColoredText:
     """static utility class with static functions:\n
         from_rgb,
         green,
@@ -25,15 +26,15 @@
 
         Returns:
             str: The given text with an RGB color applied to it.
         """
         return f"\033[38;2;{red};{green};{blue}m{text}\033[38;2;255;255;255m"
 
     @staticmethod
-    def green(text: str):
+    def green(text: str) -> str:
         """Applies green color to the given text.
 
         Args:
             text (str): The text to apply the green color to.
 
         Returns:
             str: The given text with green color applied to it.
@@ -73,14 +74,26 @@
 
         Returns:
             str: The given text with yellow color applied to it.
         """
         return ColoredText.from_rgb(255, 255, 0, text)
 
     @staticmethod
+    def orange(text: str):
+        """Applies yellow color to the given text.
+
+        Args:
+            text (str): The text to apply the yellow color to.
+
+        Returns:
+            str: The given text with yellow color applied to it.
+        """
+        return ColoredText.from_rgb(255, 165, 0, text)
+
+    @staticmethod
     def white(text: str):
         """Applies white color to the given text.
 
         Args:
             text (str): The text to apply the white color to.
 
         Returns:
@@ -97,48 +110,59 @@
 
         Returns:
             str: The given text with black color applied to it.
         """
         return ColoredText.from_rgb(0, 0, 0, text)
 
 
-def __special_print(*args, sep=" ", end="\n", start_with=None):
+def __special_print(*args, sep: str = " ", end: str = "\n", start_with: Optional[str] = None):
     """inner helper function"""
     if start_with:
         if "\n" not in sep:
             print(f"{start_with}: ", end="")
             print(sep.join([str(arg) for arg in args]), sep="", end=end)
         else:
             print(
                 sep.join([f"{start_with}: {str(arg)}" for arg in args]), sep="", end=end)
     else:
         print(*args, sep=sep, end=end)
 
 
-def warning(*args, sep=" ", end="\n"):
+def warning(*args, sep: str = " ", end: str = "\n"):
     """print a warning message
 
     Args:
         sep (str, optional): print separator. Defaults to " ".
         end (str, optional): print endline. Defaults to "\\n".
     """
 
     __special_print(*args, sep=sep, end=end,
-                    start_with=ColoredText.yellow("WARNING"))
+                    start_with=ColoredText.orange("WARNING"))
 
 
-def error(*args, sep=" ", end="\n"):
+def error(*args, sep: str = " ", end: str = "\n"):
     """print an error message
 
     Args:
         sep (str, optional): print separator. Defaults to " ".
         end (str, optional): print endline. Defaults to "\\n".
     """
     __special_print(*args, sep=sep, end=end,
                     start_with=ColoredText.red("ERROR"))
 
 
+def info(*args, sep: str = " ", end: str = "\n"):
+    """print an error message
+
+    Args:
+        sep (str, optional): print separator. Defaults to " ".
+        end (str, optional): print endline. Defaults to "\\n".
+    """
+    __special_print(*args, sep=sep, end=end,
+                    start_with=ColoredText.red("INFO"))
+
+
 __all__ = [
     "ColoredText",
     "warning",
     "error"
 ]
```

### Comparing `danielutils-0.8.6/danielutils/Conversions/MainConversions.py` & `danielutils-0.8.7/danielutils/Conversions/MainConversions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Data.py` & `danielutils-0.8.7/danielutils/Data.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/DataStructures/Comparer.py` & `danielutils-0.8.7/danielutils/DataStructures/Comparer.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,56 +2,36 @@
 from typing import Callable, Any
 from .functions import default_weight_function
 
 
 class Comparer():
     """a Comparer class to be used when comparing two objects
     """
-    class _Comparer:
-        """inner implementation
-        """
 
-        def __init__(self, func: Callable[[Any, Any], int]):
-            self.func = func
+    def __init__(self, func: Callable[[Any, Any], int | float]):
+        self.func = func
 
-        def compare(self, v1: Any, v2: Any) -> int:
-            """compares two objects
-
-            Args:
-                v1 (Any): first object
-                v2 (Any): second object
-
-            Returns:
-                int: a number specifying the order of the objects
-            """
-            return self.func(v1, v2)
-
-        def __call__(self, v1: Any, v2: Any) -> int:
-            return self.compare(v1, v2)
-
-    GREATER = _Comparer(lambda a, b: default_weight_function(
-        a)-default_weight_function(b))
-    SMALLER = _Comparer(lambda a, b: default_weight_function(
-        b)-default_weight_function(a))
-
-    def __init__(self, func: Callable[[Any, Any], int]):
-        self.__comp = Comparer._Comparer(func)
-
-    def compare(self, v1: Any, v2: Any) -> int:
+    def compare(self, v1: Any, v2: Any) -> int | float:
         """compares two objects
 
             Args:
                 v1 (Any): first object
                 v2 (Any): second object
 
             Returns:
                 int: a number specifying the order of the objects
             """
-        return self.__comp(v1, v2)
+        return self.func(v1, v2)
 
-    def __call__(self, v1: Any, v2: Any) -> int:
+    def __call__(self, v1: Any, v2: Any) -> int | float:
         return self.compare(v1, v2)
 
 
+CompareGreater = Comparer(lambda a, b: default_weight_function(a) -
+                          default_weight_function(b))
+CompareSmaller = Comparer(lambda a, b: default_weight_function(b) -
+                          default_weight_function(a))
 __all__ = [
-    "Comparer"
+    "Comparer",
+    "CompareGreater",
+    "CompareSmaller"
 ]
```

### Comparing `danielutils-0.8.6/danielutils/DataStructures/Heap.py` & `danielutils-0.8.7/danielutils/DataStructures/Heap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from typing import Any
-from .Comparer import Comparer
+from .Comparer import Comparer, CompareGreater, CompareSmaller
 
 
 class Heap:
     """a Heap class which will do the sorting according to the supplied comparer object
     """
 
-    def __init__(self, comparer: Comparer):
-        self.arr = []
+    def __init__(self, comparer: Comparer) -> None:
+        self.arr: list = []
         self.comparer = comparer
 
     def push(self, val: Any) -> None:
         """will add a new object to the heap
 
         Args:
             val (Any): the object to add to the heap
         """
-        res = -1
+        res: int | float = -1
         curr_index = len(self)
         self.arr.append(val)
         parent_index = curr_index//2 - (1 - curr_index % 2)
         while res < 0 and parent_index >= 0:
-            res = self.comparer.compare(self[parent_index], self[curr_index])
+            res = self.comparer.compare(
+                self[parent_index], self[curr_index])
             if res < 0:
                 self.arr[parent_index], self.arr[curr_index] = self[curr_index], self[parent_index]
                 curr_index = parent_index
                 parent_index = curr_index//2 - (1 - curr_index % 2)
 
     def __len__(self):
         return len(self.arr)
@@ -88,23 +89,23 @@
 
 
 class MaxHeap(Heap):
     """classic MaxHeap implementation
     """
 
     def __init__(self):
-        super().__init__(Comparer.GREATER)
+        super().__init__(CompareGreater)
 
 
 class MinHeap(Heap):
     """classic MinHeap implementation
     """
 
     def __init__(self):
-        super().__init__(Comparer.SMALLER)
+        super().__init__(CompareSmaller)
 
 
 __all__ = [
     "Heap",
     "MaxHeap",
     "MinHeap",
 ]
```

### Comparing `danielutils-0.8.6/danielutils/DataStructures/Queue.py` & `danielutils-0.8.7/danielutils/DataStructures/Queue.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from typing import Callable, Any
 from .Heap import Heap
-from .Comparer import Comparer
+from .Comparer import Comparer, CompareGreater
 from .functions import default_weight_function
+from ..MetaClasses import AtomicClassMeta
 
 
 class Queue:
     """classic Queue data structure"""
 
-    def __init__(self):
-        self.data = []
+    def __init__(self) -> None:
+        self.data: list = []
 
     def pop(self) -> Any:
         """return the oldest element while removing it from the queue
 
         Returns:
             Any: result
         """
@@ -45,16 +46,34 @@
             bool: result
         """
         return len(self) == 0
 
     def __str__(self) -> str:
         return str(self.data)
 
+    def __iter__(self):
+        while not self.is_empty():
+            yield self.pop()
 
-class PriorityQueue:
+    def push_many(self, arr: list):
+        """will push many objects to the Queue
+
+        Args:
+            arr (list): the objects to push
+        """
+        for v in arr:
+            self.push(v)
+
+
+class AtomicQueue(Queue, metaclass=AtomicClassMeta):
+    """Same as Queue but atomic
+    """
+
+
+class PriorityQueue(Queue):
     """
     A priority queue implementation based on a binary heap.
 
     Args:
         weight_func (Callable[[T], int | float], optional): A function to calculate the weight of items added
             to the queue. Defaults to default_weight_function.
         comparer (Comparer, optional): The comparer to use when comparing weights of items in the queue.
@@ -73,37 +92,39 @@
             (i.e., the lowest weight value) from the queue without removing it.
         __str__() -> str:
             Returns a string representation of the queue.
 
     Example:
         >>> pq = PriorityQueue()
         >>> pq.push(5)
-        >>> pq.push(3)
         >>> pq.push(10)
+        >>> pq.push(3)
         >>> pq.pop()
-        3
+        10
     """
 
-    def __init__(self, weight_func: Callable[[Any], int | float] = default_weight_function,
-                 comparer: Comparer = Comparer.GREATER):
-        self.heap = Heap(comparer)
+    def __init__(self, weight_func: Callable[[Any], int | float] = default_weight_function):
+        super().__init__()
+        comparer = CompareGreater if weight_func is default_weight_function else Comparer(
+            lambda a, b: weight_func(a)-weight_func(b))
+        self.data: Heap = Heap(comparer)
         self.weight_func = weight_func
-        self.dct = {}
+        self.dct: dict = {}
 
     def pop(self) -> Any:
         """
         Removes and returns the item with the highest priority (i.e., the lowest weight value) from the queue.
 
         Returns:
             T: The item with the highest priority in the queue.
 
         Raises:
             KeyError: Raised if the queue is empty.
         """
-        item_weight = self.heap.pop()
+        item_weight = self.data.pop()
         res = self.dct[item_weight]
         del self.dct[item_weight]
         return res
 
     def push(self, value: Any):
         """
         Adds a new item to the queue with the specified value and weight.
@@ -117,36 +138,37 @@
         Raises:
             ValueError: Raised if an item with the same weight value is added more than once.
         """
         item_weight = self.weight_func(value)
         if item_weight in self.dct:
             raise ValueError(
                 "Can't have same weight value more than once in current implementation")
-        self.heap.push(item_weight)
+        self.data.push(item_weight)
         self.dct[item_weight] = value
 
     def peek(self) -> Any:
         """
         Returns the item with the highest priority (i.e., the lowest weight value) from the queue without removing it.
 
         Returns:
             T: The item with the highest priority in the queue.
 
         Raises:
             KeyError: Raised if the queue is empty.
         """
-        return self.dct[self.heap.peek()]
+        return self.dct[self.data.peek()]
 
     def __str__(self) -> str:
         """
         Returns a string representation of the queue.
 
         Returns:
             str: A string representation of the queue.
         """
-        return str([str(self.dct[w]) for w in [self.heap[i] for i in range(len(self.heap))]])
+        return str([str(self.dct[w]) for w in [self.data[i] for i in range(len(self.data))]])
 
 
 __all__ = [
     "Queue",
+    "AtomicQueue",
     "PriorityQueue"
 ]
```

### Comparing `danielutils-0.8.6/danielutils/DataStructures/functions.py` & `danielutils-0.8.7/danielutils/DataStructures/functions.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/PartiallyImplemented.py` & `danielutils-0.8.7/danielutils/Decorators/PartiallyImplemented.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/atomic.py` & `danielutils-0.8.7/danielutils/Decorators/atomic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-from typing import Callable
+from typing import Callable, Any
 import threading
 from .validate import validate
 
 
 @validate
 def atomic(func: Callable) -> Callable:
     """will make function thread safe by making it
@@ -14,15 +14,15 @@
 
     Returns:
         Callable: the thread safe function
     """
     lock = threading.Lock()
 
     @ functools.wraps(func)
-    def wrapper(*args, **kwargs):
+    def wrapper(*args, **kwargs) -> Any:
         with lock:
             return func(*args, **kwargs)
     return wrapper
 
 
 __all__ = [
     "atomic"
```

### Comparing `danielutils-0.8.6/danielutils/Decorators/attach.py` & `danielutils-0.8.7/danielutils/Decorators/attach.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
-from typing import Callable
+from typing import Callable, Optional
 from .validate import validate
 
 
 @validate(strict=False)
-def attach(before: Callable = None, after: Callable = None) -> Callable:
+def attach(before: Optional[Callable] = None, after: Optional[Callable] = None) -> Callable:
     """attaching functions to a function
 
     Args:
         before (Callable, optional): function to call before. Defaults to None.
         after (Callable, optional): function to call after. Defaults to None.
 
     Raises:
@@ -18,15 +18,15 @@
     Returns:
         Callable: the decorated result
     """
     if before is None and after is None:
         raise ValueError("You must supply at least one function")
 
     def attach_deco(func: Callable):
-        if not isinstance(func, Callable):
+        if not callable(func):
             raise ValueError("attach must decorate a function")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             if before is not None:
                 before()
             res = func(*args, **kwargs)
```

### Comparing `danielutils-0.8.6/danielutils/Decorators/chain_decorators.py` & `danielutils-0.8.7/danielutils/Decorators/chain_decorators.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/decorate_conditionally.py` & `danielutils-0.8.7/danielutils/Decorators/decorate_conditionally.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import functools
-from typing import Callable
+from typing import Callable, Optional
 from .validate import validate
 
 
 @validate(strict=False)
-def decorate_conditionally(decorator: Callable, predicate: bool | Callable[[], bool], args: list = None):
+def decorate_conditionally(decorator: Callable, predicate: bool | Callable[[], bool], args: Optional[list] = None):
     """will decorate a function iff the predicate is True or returns True
 
     Args:
         decorator (Callable): the decorator to use
         predicate (bool | Callable[[], bool]): the predicate
     """
 
     def deco(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
-        if (predicate() if isinstance(predicate, Callable) else predicate):
+        if (predicate() if callable(predicate) else predicate):
             if args is None:
                 return decorator(func)
             return decorator(*args)(func)
         return wrapper
     return deco
```

### Comparing `danielutils-0.8.6/danielutils/Decorators/delay_call.py` & `danielutils-0.8.7/danielutils/Decorators/delay_call.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/limit_recursion.py` & `danielutils-0.8.7/danielutils/Decorators/limit_recursion.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/memo.py` & `danielutils-0.8.7/danielutils/Decorators/memo.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/threadify.py` & `danielutils-0.8.7/danielutils/Decorators/threadify.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Decorators/timeout.py` & `danielutils-0.8.7/danielutils/Decorators/timeout.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         Exception: any exception from within the function
 
     Returns:
         Callable: the result decorated function
     """
     # https://stackoverflow.com/a/21861599/6416556
     def timeout_deco(func: Callable) -> Callable:
-        if not isinstance(func, Callable):
+        if not callable(func):
             raise ValueError("timeout must decorate a function")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
-            res = [
+            res: list = [
                 TimeoutError(f'{func.__module__}.{func.__qualname__} timed out after {duration} seconds!')]
 
             def timeout_wrapper() -> None:
                 try:
                     res[0] = func(*args, **kwargs)
                 except Exception as function_error:
                     res[0] = function_error
```

### Comparing `danielutils-0.8.6/danielutils/Decorators/validate.py` & `danielutils-0.8.7/danielutils/Decorators/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import functools
 import inspect
-from typing import Callable,  get_type_hints
-from ..Functions import isoftype
+from typing import Callable, get_type_hints, cast
+from ..Functions import isoftype, get_function_return_type
 from ..Exceptions import EmptyAnnotationException,\
     InvalidDefaultValueException, ValidationException, InvalidReturnValueException
 
 
 def validate(strict: Callable | bool = True) -> Callable:
     """A decorator that validates the annotations and types of the arguments and return
     value of a function.
 
         * 'None' is allowed as default value for everything
-        * Because of their use in classes, the generally accepted keywords 'self' and 'cls'
-        are not validated to not break intellisense when using 'Any'
+        * Because of their wide known use, generally accepted keywords 'self', 'cls', 'args', 'kwargs'
+        are not validated.
 
     Args:
         func (Callable): The function to be decorated.
 
     Raises:
         TypeError: if the decorated object is nto a Callable
         EmptyAnnotationException: If an argument is not annotated.
@@ -27,18 +27,18 @@
     Returns:
         Callable: A wrapper function that performs the validation and calls the original function.
     """
     if not isoftype(strict, bool | Callable):
         raise TypeError(
             "the argument for validate must be a Callable or a boolean to mark strict use")
 
-    def deco(func):
-        nonlocal strict
-        SKIP_SET = {"self", "cls"}
-        if not isinstance(func, Callable):
+    def deco(func: Callable):
+
+        SKIP_SET = {"self", "cls", "args", "kwargs"}
+        if not callable(func):
             raise TypeError(
                 "The validate decorator must only decorate a function")
         func_name = f"{func.__module__}.{func.__qualname__}"
         # get the signature of the function
         signature = inspect.signature(func)
         for arg_name, arg_param in signature.parameters.items():
             if arg_name not in SKIP_SET:
@@ -60,14 +60,16 @@
                         f"In {func_name}, argument '{arg_name}'s default value is annotated \
                         as {arg_type} but got '{default_value}' which is {type(default_value)}")
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             """wrapper function for the type validating - will run on each call independently
             """
+            nonlocal strict
+            strict = cast(bool, strict)
             hints = None
             # check all arguments
             bound = signature.bind(*args, **kwargs)
             for variable_name, variable_value in bound.arguments.items():
                 if variable_name in SKIP_SET:
                     continue
                 expected_type = func.__annotations__[variable_name]
@@ -83,26 +85,25 @@
                         f"In {func_name}, argument '{variable_name}' is annotated as "
                         f"{expected_type} but got '{variable_value}' which is {type(variable_value)}")
 
             # call the function
             result = func(*args, **kwargs)
 
             # check the return type
-            return_type = type(None) if ("inspect._empty" in str(signature.return_annotation)
-                                         or signature.return_annotation is None) else signature.return_annotation
+            return_type = get_function_return_type(func, signature)
             if isinstance(return_type, str):
                 # why does this even happen?
                 return_type = get_type_hints(func)["return"]
             if return_type is not type(None) and not isoftype(result, return_type):
                 raise InvalidReturnValueException(
                     f"In function {func_name}, the return type is annotated as "
                     f"{return_type} but got '{result}' which is {type(result)}")
             return result
         return wrapper
-    if isinstance(strict, Callable):
+    if callable(strict):
         func = strict
         strict = True
         return deco(func)
     return deco
 
 
 # def validate(func: Callable) -> Callable:
```

### Comparing `danielutils-0.8.6/danielutils/Exceptions.py` & `danielutils-0.8.7/danielutils/Exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 class InvalidReturnValueException(ValidationException):
     """exception for validate decorator to be used if a function has
     an annotated return value but the actual return value doesn't conform to it
     """
 
 
-class PrintCatch:
+class PrintCatchOne:
     """a utility class to be used with a "with" block to print 
     any exception that happens inside of it rather than exiting the program
     """
 
     def __enter__(self):
         return self
```

### Comparing `danielutils-0.8.6/danielutils/IO.py` & `danielutils-0.8.7/danielutils/IO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import subprocess
-from typing import IO, Iterator, Generator
+from typing import IO, Iterator, Generator, Optional, cast
 import shutil
 from pathlib import Path
 import os
 from .Decorators import validate
 
 
 @validate
@@ -54,15 +54,15 @@
         path (str): path of file
     """
     if file_exists(path):
         os.remove(path)
 
 
 @validate
-def read_file(path: str, read_bytes: bool = False) -> list[str]:
+def read_file(path: str, read_bytes: bool = False) -> list[str] | list[bytes]:
     """read all lines from a file
 
     Args:
         path (str): the path to the file
 
     Returns:
         list[str]: a list of all the lines in the file
@@ -72,16 +72,16 @@
             with open(path, "rb") as f:
                 return f.readlines()
         else:
             with open(path, "r", encoding="mbcs") as f:
                 return f.readlines()
     except Exception as e:
         if isinstance(e, UnicodeDecodeError):
-            raise UnicodeDecodeError(
-                "Can't read byte in file.\nTo use with bytes use: read_bytes = True ") from e
+            raise UnicodeDecodeError(e.encoding, e.object, e.start, e.end,
+                                     "Can't read byte in file.\nTo use with bytes use: read_bytes = True ") from e
         raise e
 
 
 @validate
 def is_file(path: str) -> bool:
     """return whether a path represents a file
 
@@ -292,17 +292,17 @@
         also, the output_stream must be set whether by the first argument io super().__init__(...)
         or by set_stream() explicitly somewhere else.
 
         this class will not function properly is the output_stream is not set!
 
     """
 
-    def __init__(self, output_stream: IO = None, indent_value: str = "\t"):
+    def __init__(self, output_stream: Optional[IO] = None, indent_value: str = "\t"):
         self.indent_level = 0
-        self.output_stream: IO = output_stream
+        self.output_stream: Optional[IO] = output_stream
         self.indent_value = indent_value
 
     def write(self, *args, sep=" ", end="\n"):
         """writes the supplied arguments to the output_stream
 
         Args:
             sep (str, optional): the str to use as a separator between arguments. Defaults to " ".
@@ -320,14 +320,15 @@
     def set_stream(self, stream: IO):
         """explicitly sets the stream
 
         Args:
             stream (IO): stream
         """
         self.output_stream = stream
+        self.output_stream = cast(IO, self.output_stream)
 
     def indent(self) -> None:
         """indents the preceding output with write() by one quantity more
         """
         self.indent_level += 1
 
     def undent(self) -> None:
```

### Comparing `danielutils-0.8.6/danielutils/Internet.py` & `danielutils-0.8.7/danielutils/Internet.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     req = urllib.request.Request(url, headers=headers)
     html = urllib.request.urlopen(req).read().decode('UTF-8')
     # return bs4(html, 'html.parser').prettify()
     return html
 
 
 @validate
-def get_url_details(url: str) -> tuple[str, str, str, str, str]:
+def get_url_details(url: str) -> tuple[str, str, str, str, str, str]:
     """returns details about a url
 
     Args:
         url (str): url
 
     Returns:
         tuple[str, str, str, str, str]: scheme, nteloc, path, params, query, fragment
```

### Comparing `danielutils-0.8.6/danielutils/Math/Constants.py` & `danielutils-0.8.7/danielutils/Math/Constants.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Math/MathPrint.py` & `danielutils-0.8.7/danielutils/Math/MathPrint.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Args:
         s (str): the string to parse with math symbols
 
     Returns:
         str: the result
     """
 
-    def inner(res, index, dct):
+    def inner(res: str, index: int, dct: dict):
         start = index
         while index < len(s) and s[index] not in {' ', '*', '+', '-', '/', '_', '^'}:
             index += 1
         end = index
         for char in s[start:end]:
             if char in dct:
                 res += dct[char]
```

### Comparing `danielutils-0.8.6/danielutils/Math/MathSymbols.py` & `danielutils-0.8.7/danielutils/Math/MathSymbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # superscript_big_case_v = 'ⁱ'
 # superscript_big_case_w = 'ⁱ'
 # superscript_big_case_x = 'ⁱ'
 # superscript_big_case_y = 'ⁱ'
 # superscript_big_case_z = 'ⁱ'
 
 
-superscript_dict = {}
+superscript_dict :dict[str|int,str]= {}
 superscript_dict.update(
     {chr(i+ord('a')): SUPERSCRIPT_SMALL_LETTERS[i] for i in range(26)}
 )
 superscript_digits = ["⁰", "¹", "²", "³",
                       "⁴", "⁵", "⁶", "⁷", "⁸", "⁹"]
 superscript_dict.update(
     {i: superscript_digits[i] for i in range(len(superscript_digits))}
@@ -93,15 +93,15 @@
 # subscript_big_case_t = 'ⁱ'
 # subscript_big_case_u = 'ⁱ'
 # subscript_big_case_v = 'ⁱ'
 # subscript_big_case_w = 'ⁱ'
 # subscript_big_case_x = 'ⁱ'
 # subscript_big_case_y = 'ⁱ'
 # subscript_big_case_z = 'ⁱ'
-subscript_dict = {}
+subscript_dict:dict[str|int,str] = {}
 subscript_dict.update(
     {chr(i+ord('a')): SUBSCRIPT_SMALL_LETTERS[i]
      for i in range(len(SUBSCRIPT_SMALL_LETTERS))}
 )
 
 subscript_digits = ["\u2080", "\u2081", "\u2082", "\u2083",
                     "\u2084", "\u2085", "\u2086", "\u2087", "\u2088", "\u2089"]
```

### Comparing `danielutils-0.8.6/danielutils/MetaClasses/AtomicClassMeta.py` & `danielutils-0.8.7/danielutils/MetaClasses/AtomicClassMeta.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 
 class AtomicClassMeta(type):
     """will make all of the class's function atomic
     """
     def __new__(mcs, name, bases, namespace):
         for k, v in namespace.items():
-            if isinstance(v, Callable):
+            if callable(v):
                 namespace[k] = atomic(v)
         for base in bases:
             for k, v in base.__dict__.items():
-                if isinstance(v, Callable):
+                if callable(v):
                     if k not in namespace:
                         namespace[k] = atomic(v)
-                    else:
-                        breakpoint()
-                        pass
+                    # else:
+                    #     breakpoint()
+                    #     pass
         return super().__new__(mcs, name, bases, namespace)
 
 
 __all__ = [
     "AtomicClassMeta"
 ]
```

### Comparing `danielutils-0.8.6/danielutils/MetaClasses/Interface.py` & `danielutils-0.8.7/danielutils/MetaClasses/Interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Iterable, Any, Generator
+from typing import Callable, Iterable, Any, Generator, Optional, cast
 import inspect
 import re
 import traceback
 import functools
 # from ..Decorators.decorate_conditionally import decorate_conditionally
 
 
@@ -86,15 +86,15 @@
         src = inspect.getsource(cls).splitlines()
         for line in src:
             if re.match(r".*def \w+\(.*\).*:", line):
                 func_name = re.findall(r".*def (\w+)\(.*", line)[0]
                 yield func_name
 
     @staticmethod
-    def create_init_handler(cls_name, missing: list[str] = None, original: Callable = None):
+    def create_init_handler(cls_name, missing: Optional[list[str] | set[str]] = None, original: Optional[Callable] = None):
         """this function will create the default interface __init__ function with the wanted behavior"""
         # @decorate_conditionally(functools.wraps, original is not None, [original])  # TODO implement this decorator
         def __interface_init__(*args, **kwargs):
             instance = args[0]
             caller_frame = traceback.format_stack()[-2]
             is_super_call = bool(re.match(
                 fr"\s+File \".*\", line \d+, in __init__\n\s+(?:super\(\)|{cls_name})\.__init__\(.*\)\n", caller_frame))
@@ -145,34 +145,36 @@
 
     @staticmethod
     def abstractmethod(func):
         """will explicitly mark a method as an abstract method"""
         setattr(func, Interface.FUNC_KEY, True)
         return func
 
-    def __new__(mcs, name: str, bases: tuple, namespace: dict):
+    def __new__(mcs: type['Interface'], name: str, bases: tuple, namespace: dict):
         if len(bases) == 0:
             return mcs._handle_new_interface(mcs, name, bases, namespace)
         return mcs._handle_new_subclass(mcs, name, bases, namespace)
 
-    def _handle_new_interface(cls, name: str, bases: tuple, namespace: dict[str, Any]):
+    @staticmethod
+    def _handle_new_interface(mcs, name: str, bases: tuple, namespace: dict[str, Any]) -> type:
         namespace[InterfaceHelper.ORIGINAL_INIT] = None
         if "__init__" in namespace:
             namespace[InterfaceHelper.ORIGINAL_INIT] = namespace["__init__"]
         namespace["__init__"] = InterfaceHelper.create_init_handler(
             name, original=namespace[InterfaceHelper.ORIGINAL_INIT])
         for k, v in namespace.items():
-            if isinstance(v, Callable) and not k == "__init__":
+            if callable(v) and not k == "__init__":
                 if not InterfaceHelper.is_func_implemented(v):
                     namespace[k] = InterfaceHelper.create_generic_handler(k, v)
         namespace[Interface.KEY] = True
-        return super().__new__(cls, name, bases, namespace)
+        return type.__new__(mcs, name, bases, namespace)
 
-    def _handle_new_subclass(cls, name: str, bases: tuple, namespace: dict[str, Any]):
-        need_to_be_implemented = set()
+    @staticmethod
+    def _handle_new_subclass(mcs: type['Interface'], name: str, bases: tuple, namespace: dict[str, Any]) -> type:
+        need_to_be_implemented: set = set()
         ancestry = set()
         for base in bases:
             cls_tree = inspect.getclasstree([base], unique=True)
             ancestry.update(InterfaceHelper.flatten_iterables(cls_tree))
             for item in cls_tree:
                 if isinstance(item, tuple):
                     derived, parent = item
@@ -239,15 +241,15 @@
             namespace["__init__"] = InterfaceHelper.create_init_handler(
                 name, missing)
         else:
             namespace[Interface.KEY] = False
             if "__init__" not in namespace:
                 namespace["__init__"] = object.__init__
 
-        return super().__new__(cls, name, bases, namespace)
+        return type.__new__(mcs, name, bases, namespace)
 
     @staticmethod
     def is_cls_interface(cls_to_check: type) -> bool:
         """will check if a class is an interface
 
         Args:
             cls_to_check (type): the class to check
```

### Comparing `danielutils-0.8.6/danielutils/Path.py` & `danielutils-0.8.7/danielutils/Path.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Print.py` & `danielutils-0.8.7/danielutils/Print.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Reflection.py` & `danielutils-0.8.7/danielutils/Reflection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 import inspect
 import traceback
 import platform
 import sys
 import importlib
 from enum import Enum
-from typing import Any, Callable
+from typing import Any, cast, Optional
+from types import FrameType
 
 
-def get_caller_name(steps_back: int = 0) -> str:
+def __get_prev_frame(frame: Optional[FrameType]) -> Optional[FrameType]:
+    if frame is None:
+        return None
+    if not isinstance(frame, FrameType):
+        return None
+    frame = cast(FrameType, frame)
+    return frame.f_back
+
+
+def get_caller_name(steps_back: int = 0) -> Optional[str]:
     """returns the name caller of the function
 
     Returns:
         str: name of caller
     """
     if not isinstance(steps_back, int):
         raise TypeError("steps_back must be an int")
@@ -30,17 +40,23 @@
 
     # current_frame = inspect.currentframe()
     # callee_frame = current_frame.f_back
     # # callee_name = callee_frame.f_code.co_name
     # caller_frame = callee_frame.f_back
     # caller_name = caller_frame.f_code.co_name
     # return caller_name
-    frame = inspect.currentframe().f_back.f_back
+    frame = __get_prev_frame(__get_prev_frame(inspect.currentframe()))
+    if frame is None:
+        return None
+    frame = cast(FrameType, frame)
     while steps_back > 0:
-        frame = frame.f_back
+        frame = __get_prev_frame(frame)
+        if frame is None:
+            return None
+        frame = cast(FrameType, frame)
         steps_back -= 1
     return frame.f_code.co_name
 
 
 def dynamically_load(module_name: str, obj_name: str) -> Any:
     """dynammically loads the module and returns the object from this file
 
@@ -58,15 +74,15 @@
 #     """dynammically loads the module and returns the class from this file
 
 #     Args:
 #         module_name (str): name of python module, (typically a file name without extention)
 #         class_name (str): the name of the wanted class
 
 #     Returns:
-#         type: The class
+#         type (type): The class
 #     """
 #     return dynamically_load(module_name, class_name)
 
 
 # def get_function(module_name: str, func_name: str) -> Callable:
 #     """dynammically loads the module and returns the function from this file
 
@@ -77,42 +93,52 @@
 #     Returns:
 #         Callable: the function
 #     """
 #     return dynamically_load(module_name, func_name)
 
 
 # def get_current_function() -> Callable:
-    """return the function that is calling this file
+#     """return the function that is calling this file
 
-    Returns:
-        Callable: function
-    """
-    return get_caller()
+#     Returns:
+#         Callable: function
+#     """
+#     return get_caller()
+
+def get_filename() -> Optional[str]:
+    frame = __get_prev_frame(inspect.currentframe())
+    if frame is None:
+        return None
+    frame = cast(FrameType, frame)
+    return frame.f_code.co_filename
 
 
-def get_caller_file() -> str:
+def get_caller_filename() -> Optional[str]:
     """return the name of the file that the caller of the 
     function that's using this function is in
 
     Returns:
         str: name of file
     """
-    frame = inspect.currentframe().f_back.f_back
+    frame = __get_prev_frame(__get_prev_frame(inspect.currentframe()))
+    if frame is None:
+        return None
+    frame = cast(FrameType, frame)
     return frame.f_code.co_filename
 
 
 # def get_caller() -> Callable:
-    """returns the caller of the function thats using this function
+#     """returns the caller of the function thats using this function
 
-    Returns:
-        Callable: caller
-    """
-    name = get_caller_name(1)
-    module = get_caller_file().removesuffix(".py")
-    return get_function(module, name)
+#     Returns:
+#         Callable: caller
+#     """
+#     name = get_caller_name(1)
+#     module = get_caller_filename().removesuffix(".py")
+#     return get_function(module, name)
 
 
 def get_traceback() -> list[str]:
     """returns the traceback of the stack until current frame
 
     Returns:
         list[str]: list of frames as strings
@@ -156,14 +182,15 @@
 
 __all__ = [
     "get_caller_name",
     "dynamically_load",
     # "get_class",
     # "get_function",
     # "get_current_function",
-    "get_caller_file",
+    "get_filename",
+    "get_caller_filename",
     # "get_caller",
     "get_traceback",
     "OSType",
     "get_os",
     "get_python_version"
 ]
```

### Comparing `danielutils-0.8.6/danielutils/System.py` & `danielutils-0.8.7/danielutils/System.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Generator
-from typing import IO
+from typing import IO, Optional, cast
 from pathlib import Path
 import subprocess
 import time
 from .Decorators import timeout, validate
 from .Conversions import str_to_bytes
+from .Generators import join_generators, generator_from_stream
 
 
 def cm(*args, shell: bool = True) -> tuple[int, bytes, bytes]:
     """Execute windows shell command and return output
 
     Args:
         command or args:\n
@@ -22,15 +23,16 @@
     Returns:
         Tuple[int, bytes, bytes]: return code, stdout, stderr
     """
     if not isinstance(shell, bool):
         raise TypeError(
             "In function 'cm' param 'shell' must be of type bool")
     for i, arg in enumerate(args):
-        if Path(args[i]).is_file() or Path(args[i]).is_dir():
+        path_obj = Path(args[i])
+        if path_obj.is_file() or path_obj.is_dir():
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
     res = subprocess.run(" ".join(args), shell=shell,
                          capture_output=True, check=False)
     return res.returncode, res.stdout, res.stderr
 
 
 @validate
@@ -43,24 +45,24 @@
     Returns:
         None
     """
     time.sleep(seconds)
 
 
 def __acm_write(*args, p: subprocess.Popen, sep=" ", end="\n") -> None:
+    p.stdin = cast(IO[bytes], p.stdin)
     b_args = str_to_bytes(sep).join(str_to_bytes(v) for v in args)
     b_end = str_to_bytes(end)
     p.stdin.write(b_args+b_end)
     p.stdin.flush()
 
 
 @validate
-def acm(command: str, inputs: list[str] = None, i_timeout: float = 0.01,
-        shell: bool = False, use_write_helper: bool = True, cwd: str = None,
-        env: str = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
+def acm(command: str, inputs: Optional[list[str]] = None, i_timeout: float = 0.01,
+        shell: bool = False, use_write_helper: bool = True, cwd: Optional[str] = None) -> tuple[int, list[bytes] | None, list[bytes] | None]:
     """Advanced command
 
     Args:
         command (str): The command to execute\n
         inputs (list[str]): the inputs to give to the program from the command. Defaults to None.\n
         i_timeout (float, optional): An individual timeout for every step of the execution. Defaults to 0.01.\n
         cwd (?, optional): Current working directory. Defaults to None.\n
@@ -75,19 +77,23 @@
 
     Returns:
         tuple[int, list[bytes] | None, list[bytes] | None]: return code, stdout, stderr
     """
 
     if inputs is None:
         inputs = []
+
     p = None
     try:
         # TODO with ... as p:
         p = subprocess.Popen(command, stdout=subprocess.PIPE,
-                             stdin=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd, env=env, shell=shell)
+                             stdin=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=cwd, shell=shell)
+        p.stdin = cast(IO[bytes], p.stdin)
+        p.stdout = cast(IO[bytes], p.stdout)
+        p.stderr = cast(IO[bytes], p.stderr)
 
         @timeout(i_timeout)
         def readlines(s: IO, l: list):
             l.extend(s.readlines())
 
         def extend_from_stream(stream: IO[bytes], list_to_extend_to: list):
             if stream is not None and stream.readable():
@@ -127,43 +133,48 @@
                 p.stdin.close()
             if p.stderr is not None:
                 p.stderr.close()
             if p.stdout is not None:
                 p.stdout.close()
 
 
-def cmrt(*args, shell: bool = True) -> Generator[bytes, None, None]:
+def cmrt(*args, shell: bool = True) -> Generator[tuple[int, bytes], None, None]:
     """Executes a command and yields stdout and stderr in real-time.
 
     Args:
-        *args: A sequence of strings representing the command and its arguments.
         shell (bool, optional): If True, the command is executed through the shell. Defaults to True.
 
     Raises:
-        TypeError: If `shell` argument is not a boolean.
+        TypeError: if 'shell' is not boolean
 
     Yields:
-        An iterator that yields bytes for stdout and stderr lines in real-time.
+        Generator[tuple[int, bytes], None, None]: the tuple yielded will contain the 'stream identifier'
+            0 - stdout,
+            1 - stderr
+        and the actual value from the stream
     """
     if not isinstance(shell, bool):
         raise TypeError("The 'shell' parameter must be of type bool.")
 
     # Quote the arguments that represent file or directory paths.
     for i, arg in enumerate(args):
-        if Path(args[i]).is_file() or Path(args[i]).is_dir():
+        path_obj = Path(args[i])
+        if path_obj.is_file() or path_obj.is_dir():
             args = (*args[:i], f"\"{arg}\"", *args[i+1:])
 
     # Join the arguments into a command string and execute the command.
     cmd = " ".join(args)
-    with subprocess.Popen(
-            cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as process:
-        # Yield stdout and stderr in real-time.
-        while process.poll() is None:
-            yield from process.stderr
-            yield from process.stdout
+
+    with subprocess.Popen(cmd, shell=shell, stdout=subprocess.PIPE, stderr=subprocess.PIPE) as process:
+        combined = join_generators(
+            generator_from_stream(process.stdout),
+            generator_from_stream(process.stderr)
+        )
+        for tup in combined:
+            yield tup
 
 
 __all__ = [
     "cm",
     "acm",
     "sleep",
     "cmrt"
```

### Comparing `danielutils-0.8.6/danielutils/Text.py` & `danielutils-0.8.7/danielutils/Text.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/Windows.py` & `danielutils-0.8.7/danielutils/Windows.py`

 * *Files identical despite different names*

### Comparing `danielutils-0.8.6/danielutils/__init__.py` & `danielutils-0.8.7/danielutils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 from .Decorators import *
 from .IO import *
 from .System import *
 from .Text import *
 from .Conversions import *
 from .Classes import *
 from .Time import *
-# from .Threading import *
 from .Colors import *
 from .Data import *
 from .DataStructures import *
 from .Math import *
 from .Path import *
 from .Windows import *
 from .Print import *
-from .Exceptions import PrintCatch
+from .Exceptions import PrintCatchOne
 from .Reflection import *
 from .DateTime import *
 from .MetaClasses import *
 from .Generators import *
+from .Snippets import *
+from .Aliases import *
```

### Comparing `danielutils-0.8.6/danielutils.egg-info/PKG-INFO` & `danielutils-0.8.7/danielutils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danielutils
-Version: 0.8.6
+Version: 0.8.7
 Summary: A python utils library for things I find useful
 Home-page: https://github.com/danielnachumdev/danielutils
 Author: danielnachumdev
 Author-email: danielnachumdev <danielnachumdev@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/danielnachumdev/danielutils
 Project-URL: Bug Tracker, https://github.com/danielnachumdev/danielutils/issues
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 [![Python package](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/python-package.yml)
 [![Pylint](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/pylint.yml)
 [![Python 3.10.11](https://img.shields.io/badge/python-3.10.11-blue.svg)](https://www.python.org/downloads/release/python-31011/)
 [![gitleaks](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/gitleaks.yml)
 [![CodeQL](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/danielnachumdev/danielutils/actions/workflows/github-code-scanning/codeql)
-# danielutils v=0.8.6
+# danielutils v=0.8.7
 A utils library for things that I find useful for my coding workflow.\
 Feel free to use and / or contribute / improve my code :)
 
 THIS PACKAGE IS IN DEVELOPMENT AND SUBJECT TO CHANGE, USE AT YOUR OWN RISK!
 
 ## Further reading
 check out [READMES/readme.md](./READMES/readme.md) to check out some of the stuff this library can do
```

### Comparing `danielutils-0.8.6/danielutils.egg-info/SOURCES.txt` & `danielutils-0.8.7/danielutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 setup.py
+danielutils/Aliases.py
 danielutils/Colors.py
 danielutils/Data.py
 danielutils/DateTime.py
 danielutils/Exceptions.py
 danielutils/Functions.py
 danielutils/IO.py
 danielutils/Internet.py
@@ -18,44 +19,59 @@
 danielutils/__init__.py
 danielutils.egg-info/PKG-INFO
 danielutils.egg-info/SOURCES.txt
 danielutils.egg-info/dependency_links.txt
 danielutils.egg-info/requires.txt
 danielutils.egg-info/top_level.txt
 danielutils/Classes/Convenience.py
-danielutils/Classes/TypedBuiltins.py
+danielutils/Classes/Counter.py
 danielutils/Classes/__init__.py
 danielutils/Classes/frange.py
+danielutils/Classes/TypedBuiltins/__init__.py
+danielutils/Classes/TypedBuiltins/tbase.py
+danielutils/Classes/TypedBuiltins/tdict.py
+danielutils/Classes/TypedBuiltins/tlist.py
+danielutils/Classes/TypedBuiltins/tset.py
+danielutils/Classes/TypedBuiltins/ttuple.py
 danielutils/Conversions/MainConversions.py
 danielutils/Conversions/__init__.py
 danielutils/Conversions/SpecializedConversions/__init__.py
 danielutils/Conversions/SpecializedConversions/to_hex.py
 danielutils/Conversions/SpecializedConversions/to_int.py
 danielutils/DataStructures/Comparer.py
+danielutils/DataStructures/Graph.py
 danielutils/DataStructures/Heap.py
 danielutils/DataStructures/Node.py
 danielutils/DataStructures/Queue.py
+danielutils/DataStructures/Stack.py
 danielutils/DataStructures/__init__.py
 danielutils/DataStructures/functions.py
 danielutils/Decorators/PartiallyImplemented.py
 danielutils/Decorators/__init__.py
 danielutils/Decorators/atomic.py
 danielutils/Decorators/attach.py
 danielutils/Decorators/chain_decorators.py
 danielutils/Decorators/decorate_conditionally.py
 danielutils/Decorators/delay_call.py
+danielutils/Decorators/deprecate.py
 danielutils/Decorators/limit_recursion.py
 danielutils/Decorators/memo.py
 danielutils/Decorators/overload.py
+danielutils/Decorators/property.py
 danielutils/Decorators/threadify.py
 danielutils/Decorators/timeout.py
 danielutils/Decorators/validate.py
 danielutils/Generators/__init__.py
+danielutils/Generators/generator_from_stream.py
 danielutils/Generators/join_generators.py
 danielutils/Math/Constants.py
 danielutils/Math/Functions.py
 danielutils/Math/MathPrint.py
 danielutils/Math/MathSymbols.py
 danielutils/Math/__init__.py
 danielutils/MetaClasses/AtomicClassMeta.py
+danielutils/MetaClasses/ImplicitDataDeleterMeta.py
+danielutils/MetaClasses/InstanceCacheMeta.py
 danielutils/MetaClasses/Interface.py
-danielutils/MetaClasses/__init__.py
+danielutils/MetaClasses/__init__.py
+danielutils/Snippets/__init__.py
+danielutils/Snippets/try_get.py
```

### Comparing `danielutils-0.8.6/pyproject.toml` & `danielutils-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "danielutils"
-version = "0.8.6"
+version = "0.8.7"
 authors = [
   { name="danielnachumdev", email="danielnachumdev@gmail.com" },
 ]
 description = "A python utils library for things I find useful"
 readme = "README.md"
 requires-python = ">=3.10.5"
 classifiers = [
```

### Comparing `danielutils-0.8.6/setup.py` & `danielutils-0.8.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 def read_file(path: str) -> "list[str]":
     with codecs.open(path, 'r', 'utf-8') as f:
         return [l.strip() for l in f.readlines()]
 
 
 README_PATH = 'README.md'
 DESCRIPTION = 'A python utils library for things I find useful'
-VERSION = "0.8.6"
+VERSION = "0.8.7"
 LONG_DESCRIPTION = '\n'.join(read_file(README_PATH))
 setup(
     name="danielutils",
     version=VERSION,
     author="danielnachumdev",
     author_email="<danielnachumdev@gmail.com>",
     description=DESCRIPTION,
```

