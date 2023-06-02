# Comparing `tmp/generalimport-0.3.1.tar.gz` & `tmp/generalimport-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generalimport-0.3.1.tar", last modified: Thu Oct 27 14:21:55 2022, max compression
+gzip compressed data, was "generalimport-0.5.0.tar", last modified: Fri Jun  2 21:27:33 2023, max compression
```

## Comparing `generalimport-0.3.1.tar` & `generalimport-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.927629 generalimport-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-10-27 14:21:34.000000 generalimport-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-27 14:21:34.000000 generalimport-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11570 2022-10-27 14:21:55.927629 generalimport-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-10-27 14:21:35.000000 generalimport-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.923628 generalimport-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-10-27 14:19:43.000000 generalimport-0.3.1/examples/1minimal_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-10-27 14:19:43.000000 generalimport-0.3.1/examples/2tests_showcase.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-27 14:19:43.000000 generalimport-0.3.1/examples/3recommended_setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-10-27 14:19:43.000000 generalimport-0.3.1/examples/4how_it_works.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.923628 generalimport-0.3.1/generalimport/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      569 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/fake_module.py
--rw-r--r--   0 runner    (1001) docker     (121)     3224 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/general_importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/generalimport_bottom.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/import_catcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/min.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.923628 generalimport-0.3.1/generalimport/test/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/funcs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6447 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_generalimport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.927629 generalimport-0.3.1/generalimport/test/test_usage/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1591 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_callable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_cast.py
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_iterable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_logic.py
--rw-r--r--   0 runner    (1001) docker     (121)      876 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)     5858 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_math.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_string.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/test/test_usage/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-10-27 14:19:43.000000 generalimport-0.3.1/generalimport/top.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 14:21:55.923628 generalimport-0.3.1/generalimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11570 2022-10-27 14:21:55.000000 generalimport-0.3.1/generalimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-10-27 14:21:55.000000 generalimport-0.3.1/generalimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 14:21:55.000000 generalimport-0.3.1/generalimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-10-27 14:21:55.000000 generalimport-0.3.1/generalimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-10-27 14:21:34.000000 generalimport-0.3.1/metadata.json
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 14:21:55.927629 generalimport-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-10-27 14:21:35.000000 generalimport-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.632518 generalimport-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 21:27:04.000000 generalimport-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 21:27:04.000000 generalimport-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-02 21:27:33.632518 generalimport-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-02 21:27:06.000000 generalimport-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/1minimal_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/2tests_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/3recommended_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 21:25:00.000000 generalimport-0.5.0/examples/4how_it_works.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/dunders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/fake_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/general_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/generalimport_bottom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/import_catcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/min.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_generalimport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.632518 generalimport-0.5.0/generalimport/test/test_usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_callable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/test/test_usage/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-02 21:25:00.000000 generalimport-0.5.0/generalimport/top.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:27:33.628518 generalimport-0.5.0/generalimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 21:27:33.000000 generalimport-0.5.0/generalimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-02 21:27:04.000000 generalimport-0.5.0/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:27:33.632518 generalimport-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-02 21:27:06.000000 generalimport-0.5.0/setup.py
```

### Comparing `generalimport-0.3.1/PKG-INFO` & `generalimport-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,225 +1,233 @@
 Metadata-Version: 2.1
 Name: generalimport
-Version: 0.3.1
+Version: 0.5.0
 Summary: Handle all your optional dependencies with a single call!
 Home-page: https://github.com/ManderaGeneral/generalimport
 Author: Rickard "Mandera" Abraham
 Author-email: rickard.abraham@gmail.com
 License: mit
-Description: <details open>
-        <summary><h1>generalimport</h1></summary>
-        
-        Handle all your optional dependencies with a single call!
-        
-        <details>
-        <summary><h2>Table of Contents</h2></summary>
-        
-        <pre>
-        <a href='#generalimport'>generalimport</a>
-        ├─ <a href='#Dependency-Diagram-for-ManderaGeneral'>Dependency Diagram for ManderaGeneral</a>
-        ├─ <a href='#Installation-showing-dependencies'>Installation showing dependencies</a>
-        ├─ <a href='#Information'>Information</a>
-        ├─ <a href='#Examples'>Examples</a>
-        │  ├─ <a href='#Minimal-Example'>Minimal Example</a>
-        │  ├─ <a href='#Tests-Showcase'>Tests Showcase</a>
-        │  ├─ <a href='#Recommended-Setup'>Recommended Setup</a>
-        │  └─ <a href='#How-It-Works'>How It Works</a>
-        ├─ <a href='#Attributes'>Attributes</a>
-        └─ <a href='#Contributions'>Contributions</a>
-        </pre>
-        </details>
-        
-        
-        <details open>
-        <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
-        
-        ```mermaid
-        flowchart LR
-        1([library]) --> 4([packager])
-        2([file]) --> 4([packager])
-        1([library]) --> 2([file])
-        0([import]) --> 1([library])
-        0([import]) --> 2([file])
-        1([library]) --> 3([vector])
-        click 0 "https://github.com/ManderaGeneral/generalimport"
-        click 1 "https://github.com/ManderaGeneral/generallibrary"
-        click 2 "https://github.com/ManderaGeneral/generalfile"
-        click 3 "https://github.com/ManderaGeneral/generalvector"
-        click 4 "https://github.com/ManderaGeneral/generalpackager"
-        style 0 fill:#482
-        ```
-        </details>
-        
-        
-        <details open>
-        <summary><h2>Installation showing dependencies</h2></summary>
-        
-        | `pip install`     | `generalimport`   |
-        |:------------------|:------------------|
-        | *No dependencies* | ✔️                |
-        </details>
-        
-        
-        <details open>
-        <summary><h2>Information</h2></summary>
-        
-        | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
-        |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-        | [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.3.1](https://pypi.org/project/generalimport/) | 2022-10-27 16:21 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 98.4 %  |
-        </details>
-        
-        
-        <details open>
-        <summary><h2>Examples</h2></summary>
-        
-        
-        <details open>
-        <summary><h3>Minimal Example</h3></summary>
-        
-        
-        Call `generalimport` before importing any optional dependencies.
-        
-        ```python
-        from generalimport import generalimport
-        generalimport("notinstalled")
-        
-        from notinstalled import missing_func  # No error
-        
-        missing_func()  # Error occurs here
-        ```
-        
-        
-        ```
-        MissingOptionalDependency: Optional dependency 'notinstalled' was used but it isn't installed.
-        ```
-        
-        Imports fail when they are **used**, *not* imported.
-        
-        This means you don't need to keep checking if the package is installed before importing it.
-        Simply import your optional package and use it like you would any package and let it fail wherever it fails, with a nice error message.
-        </details>
-        
-        
-        <details>
-        <summary><h3>Tests Showcase</h3></summary>
-        
-        
-        The beauty of this package is that the error raised isn't just any exception.
-        It has two base classes: `unittest.case.SkipTest` and `_pytest.outcomes.Skipped` (If available).
-        
-        This means that if a test method uses an uninstalled optional package then that test is automatically skipped.
-        This means no more manual skip decorators for optional dependencies!
-        
-        ```python
-        from generalimport import generalimport
-        generalimport("optional_uninstalled_package")
-        
-        from optional_uninstalled_package import missing_func
-        
-        from unittest import TestCase
-        
-        class MyTest(TestCase):
-            def test_missing_func(self):
-                self.assertEqual(3, missing_func(1, 2))
-        ```
-        
-        
-        ```
-        Ran 1 test in 0.002s
-        
-        OK (skipped=1)
-        
-        Skipped: Optional dependency 'optional_uninstalled_package' was used but it isn't installed.
-        ```
-        </details>
-        
-        
-        <details>
-        <summary><h3>Recommended Setup</h3></summary>
-        
-        
-        Put this in your `__init__.py` file to affect *all* imports inside the folder `__init__.py` resides in.
-        
-        ```python
-        from generalimport import generalimport
-        generalimport("your", "optional", "dependencies")
-        ```
-        
-        
-        `generalimport("*")` makes it handle **all** names (If missing of course)
-        
-        :warning: `generalimport("*")._scope = None` disables the scope
-        - Makes it handle missing imports anywhere
-        - For example it will override `pandas` internal custom optional dependency handling
-        </details>
-        
-        
-        <details>
-        <summary><h3>How It Works</h3></summary>
-        
-        
-        
-        - When `generalimport` is instantiated it creates a new importer for `sys.meta_path`.
-        - This importer will return 'fake' modules for matching names and scope.
-        - The scope ensures only your own imports are faked.
-        - The fake module will recursively return itself when asked for an attribute.
-        - When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingOptionalDependency`.
-        - This exception has the 'skip-exceptions' from `unittest` and `pytest` as bases, which means that tests will automatically be skipped.
-        </details>
-        
-        </details>
-        
-        
-        <details>
-        <summary><h2>Attributes</h2></summary>
-        
-        <pre>
-        <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/__init__.py#L1'>Module: generalimport</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/fake_module.py#L4'>Class: FakeModule</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/fake_module.py#L17'>Method: error_func</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L8'>Class: GeneralImporter</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L23'>Method: catch</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L47'>Method: create_module</a>
-        │  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L50'>Method: exec_module</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L31'>Method: find_spec</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/import_catcher.py#L6'>Class: ImportCatcher</a>
-        │  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/import_catcher.py#L20'>Method: handle</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/exception.py#L13'>Class: MissingOptionalDependency</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L62'>Function: fake_module_check</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L14'>Function: generalimport</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L10'>Function: get_importer</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L7'>Function: get_installed_modules_names</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L41'>Function: get_spec</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L28'>Function: import_module</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L13'>Function: module_is_installed</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L47'>Function: module_is_namespace</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L51'>Function: module_name_is_namespace</a>
-        ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L36'>Function: reset_generalimport</a>
-        └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L44'>Function: spec_is_namespace</a>
-        </pre>
-        </details>
-        
-        
-        <details open>
-        <summary><h2>Contributions</h2></summary>
-        
-        Issue-creation, discussions and pull requests are most welcome!
-        </details>
-        
-        
-        
-        <sup>
-        Generated 2022-10-27 16:21 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/ee21333a'>ee21333a</a>.
-        </sup>
-        </details>
-        
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<details open>
+<summary><h1>generalimport</h1></summary>
+
+Handle all your optional dependencies with a single call!
+
+<details>
+<summary><h2>Table of Contents</h2></summary>
+
+<pre>
+<a href='#generalimport'>generalimport</a>
+├─ <a href='#Dependency-Diagram-for-ManderaGeneral'>Dependency Diagram for ManderaGeneral</a>
+├─ <a href='#Installation-showing-dependencies'>Installation showing dependencies</a>
+├─ <a href='#Information'>Information</a>
+├─ <a href='#Examples'>Examples</a>
+│  ├─ <a href='#Minimal-Example'>Minimal Example</a>
+│  ├─ <a href='#Tests-Showcase'>Tests Showcase</a>
+│  ├─ <a href='#Recommended-Setup'>Recommended Setup</a>
+│  └─ <a href='#How-It-Works'>How It Works</a>
+├─ <a href='#Attributes'>Attributes</a>
+└─ <a href='#Contributions'>Contributions</a>
+</pre>
+</details>
+
+
+<details open>
+<summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
+
+```mermaid
+flowchart LR
+2([library]) --> 5([packager])
+2([library]) --> 4([vector])
+3([file]) --> 5([packager])
+0([import]) --> 3([file])
+1([tool]) --> 2([library])
+0([import]) --> 2([library])
+2([library]) --> 3([file])
+click 0 "https://github.com/ManderaGeneral/generalimport"
+click 1 "https://github.com/ManderaGeneral/generaltool"
+click 2 "https://github.com/ManderaGeneral/generallibrary"
+click 3 "https://github.com/ManderaGeneral/generalfile"
+click 4 "https://github.com/ManderaGeneral/generalvector"
+click 5 "https://github.com/ManderaGeneral/generalpackager"
+style 0 fill:#482
+```
+</details>
+
+
+<details open>
+<summary><h2>Installation showing dependencies</h2></summary>
+
+| `pip install`     | `generalimport`   |
+|:------------------|:------------------|
+| *No dependencies* | ✔️                |
+</details>
+
+
+<details open>
+<summary><h2>Information</h2></summary>
+
+| Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
+|:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
+| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.0](https://pypi.org/project/generalimport/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.0 %  |
+</details>
+
+
+<details open>
+<summary><h2>Examples</h2></summary>
+
+
+<details open>
+<summary><h3>Minimal Example</h3></summary>
+
+
+Call `generalimport` before importing any optional dependencies.
+
+```python
+from generalimport import generalimport
+generalimport("notinstalled")
+
+from notinstalled import missing_func  # No error
+
+missing_func()  # Error occurs here
+```
+
+
+```
+MissingDependencyException: Optional dependency 'notinstalled' was used but it isn't installed.
+```
+
+Imports fail when they are **used**, *not* imported.
+
+This means you don't need to keep checking if the package is installed before importing it.
+Simply import your optional package and use it like you would any package and let it fail wherever it fails, with a nice error message.
+</details>
+
+
+<details>
+<summary><h3>Tests Showcase</h3></summary>
+
+
+The beauty of this package is that the error raised isn't just any exception.
+It has two base classes: `unittest.case.SkipTest` and `_pytest.outcomes.Skipped` (If available).
+
+This means that if a test method uses an uninstalled optional package then that test is automatically skipped.
+This means no more manual skip decorators for optional dependencies!
+
+```python
+from generalimport import generalimport
+generalimport("optional_uninstalled_package")
+
+from optional_uninstalled_package import missing_func
+
+from unittest import TestCase
+
+class MyTest(TestCase):
+    def test_missing_func(self):
+        self.assertEqual(3, missing_func(1, 2))
+```
+
+
+```
+Ran 1 test in 0.002s
+
+OK (skipped=1)
+
+Skipped: Optional dependency 'optional_uninstalled_package' was used but it isn't installed.
+```
+</details>
+
+
+<details>
+<summary><h3>Recommended Setup</h3></summary>
+
+
+Put this in your `__init__.py` file to affect *all* imports inside the folder `__init__.py` resides in.
+
+```python
+from generalimport import generalimport
+generalimport("your", "optional", "dependencies")
+```
+
+
+`generalimport("*")` makes it handle **all** names (If missing of course)
+
+:warning: `generalimport("*")._scope = None` disables the scope
+- Makes it handle missing imports anywhere
+- For example it will override `pandas` internal custom optional dependency handling
+</details>
+
+
+<details>
+<summary><h3>How It Works</h3></summary>
+
+
+
+- When `generalimport` is instantiated it creates a new importer for `sys.meta_path`.
+- This importer will return 'fake' modules for matching names and scope.
+- The scope ensures only your own imports are faked.
+- The fake module will recursively return a FakeModule instance when asked for an attribute.
+- When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingDependencyException`.
+- This exception has the 'skip-exceptions' from `unittest` and `pytest` as bases, which means that tests will automatically be skipped.
+</details>
+
+</details>
+
+
+<details>
+<summary><h2>Attributes</h2></summary>
+
+<pre>
+<a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/__init__.py#L1'>Module: generalimport</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L7'>Class: DynamicDunder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L20'>Method: result</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L19'>Method: trigger</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L14'>Class: FakeModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L67'>Method: error_func</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L72'>Method: error_func_class</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L9'>Class: GeneralImporter</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L25'>Method: catch</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L49'>Method: create_module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L52'>Method: exec_module</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L33'>Method: find_spec</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L8'>Class: ImportCatcher</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L24'>Method: handle</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L30'>Class: MissingDependencyException</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Function: MissingOptionalDependency</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L63'>Function: fake_module_check</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L16'>Function: generalimport</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L12'>Function: get_importer</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L8'>Function: get_installed_modules_names</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L42'>Function: get_spec</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L29'>Function: import_module</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L43'>Function: is_imported</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L14'>Function: module_is_installed</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L48'>Function: module_is_namespace</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L52'>Function: module_name_is_namespace</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L38'>Function: reset_generalimport</a>
+└─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L45'>Function: spec_is_namespace</a>
+</pre>
+</details>
+
+
+<details open>
+<summary><h2>Contributions</h2></summary>
+
+Issue-creation, discussions and pull requests are most welcome!
+</details>
+
+
+
+<sup>
+Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
+</sup>
+</details>
+
```

### Comparing `generalimport-0.3.1/README.md` & `generalimport-0.5.0/generalimport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: generalimport
+Version: 0.5.0
+Summary: Handle all your optional dependencies with a single call!
+Home-page: https://github.com/ManderaGeneral/generalimport
+Author: Rickard "Mandera" Abraham
+Author-email: rickard.abraham@gmail.com
+License: mit
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <details open>
 <summary><h1>generalimport</h1></summary>
 
 Handle all your optional dependencies with a single call!
 
 <details>
 <summary><h2>Table of Contents</h2></summary>
@@ -23,25 +41,27 @@
 
 
 <details open>
 <summary><h2>Dependency Diagram for ManderaGeneral</h2></summary>
 
 ```mermaid
 flowchart LR
-1([library]) --> 4([packager])
-2([file]) --> 4([packager])
-1([library]) --> 2([file])
-0([import]) --> 1([library])
-0([import]) --> 2([file])
-1([library]) --> 3([vector])
+2([library]) --> 5([packager])
+2([library]) --> 4([vector])
+3([file]) --> 5([packager])
+0([import]) --> 3([file])
+1([tool]) --> 2([library])
+0([import]) --> 2([library])
+2([library]) --> 3([file])
 click 0 "https://github.com/ManderaGeneral/generalimport"
-click 1 "https://github.com/ManderaGeneral/generallibrary"
-click 2 "https://github.com/ManderaGeneral/generalfile"
-click 3 "https://github.com/ManderaGeneral/generalvector"
-click 4 "https://github.com/ManderaGeneral/generalpackager"
+click 1 "https://github.com/ManderaGeneral/generaltool"
+click 2 "https://github.com/ManderaGeneral/generallibrary"
+click 3 "https://github.com/ManderaGeneral/generalfile"
+click 4 "https://github.com/ManderaGeneral/generalvector"
+click 5 "https://github.com/ManderaGeneral/generalpackager"
 style 0 fill:#482
 ```
 </details>
 
 
 <details open>
 <summary><h2>Installation showing dependencies</h2></summary>
@@ -53,15 +73,15 @@
 
 
 <details open>
 <summary><h2>Information</h2></summary>
 
 | Package                                                          | Ver                                              | Latest Release        | Python                                                                                                                                                                                                                                                 | Platform        | Cover   |
 |:-----------------------------------------------------------------|:-------------------------------------------------|:----------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:--------|
-| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.3.1](https://pypi.org/project/generalimport/) | 2022-10-27 16:21 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 98.4 %  |
+| [generalimport](https://github.com/ManderaGeneral/generalimport) | [0.5.0](https://pypi.org/project/generalimport/) | 2023-06-02 23:27 CEST | [3.8](https://www.python.org/downloads/release/python-380/), [3.9](https://www.python.org/downloads/release/python-390/), [3.10](https://www.python.org/downloads/release/python-3100/), [3.11](https://www.python.org/downloads/release/python-3110/) | Windows, Ubuntu | 97.0 %  |
 </details>
 
 
 <details open>
 <summary><h2>Examples</h2></summary>
 
 
@@ -78,15 +98,15 @@
 from notinstalled import missing_func  # No error
 
 missing_func()  # Error occurs here
 ```
 
 
 ```
-MissingOptionalDependency: Optional dependency 'notinstalled' was used but it isn't installed.
+MissingDependencyException: Optional dependency 'notinstalled' was used but it isn't installed.
 ```
 
 Imports fail when they are **used**, *not* imported.
 
 This means you don't need to keep checking if the package is installed before importing it.
 Simply import your optional package and use it like you would any package and let it fail wherever it fails, with a nice error message.
 </details>
@@ -150,58 +170,64 @@
 <summary><h3>How It Works</h3></summary>
 
 
 
 - When `generalimport` is instantiated it creates a new importer for `sys.meta_path`.
 - This importer will return 'fake' modules for matching names and scope.
 - The scope ensures only your own imports are faked.
-- The fake module will recursively return itself when asked for an attribute.
-- When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingOptionalDependency`.
+- The fake module will recursively return a FakeModule instance when asked for an attribute.
+- When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingDependencyException`.
 - This exception has the 'skip-exceptions' from `unittest` and `pytest` as bases, which means that tests will automatically be skipped.
 </details>
 
 </details>
 
 
 <details>
 <summary><h2>Attributes</h2></summary>
 
 <pre>
-<a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/__init__.py#L1'>Module: generalimport</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/fake_module.py#L4'>Class: FakeModule</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/fake_module.py#L17'>Method: error_func</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L8'>Class: GeneralImporter</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L23'>Method: catch</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L47'>Method: create_module</a>
-│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L50'>Method: exec_module</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/general_importer.py#L31'>Method: find_spec</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/import_catcher.py#L6'>Class: ImportCatcher</a>
-│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/import_catcher.py#L20'>Method: handle</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/exception.py#L13'>Class: MissingOptionalDependency</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L62'>Function: fake_module_check</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L14'>Function: generalimport</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L10'>Function: get_importer</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L7'>Function: get_installed_modules_names</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L41'>Function: get_spec</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L28'>Function: import_module</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L13'>Function: module_is_installed</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L47'>Function: module_is_namespace</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L51'>Function: module_name_is_namespace</a>
-├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport/top.py#L36'>Function: reset_generalimport</a>
-└─ <a href='https://github.com/ManderaGeneral/generalimport/blob/ee21333a/generalimport_bottom.py#L44'>Function: spec_is_namespace</a>
+<a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/__init__.py#L1'>Module: generalimport</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L7'>Class: DynamicDunder</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L20'>Method: result</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/dunders.py#L19'>Method: trigger</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L14'>Class: FakeModule</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L67'>Method: error_func</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/fake_module.py#L72'>Method: error_func_class</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L9'>Class: GeneralImporter</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L25'>Method: catch</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L49'>Method: create_module</a>
+│  ├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L52'>Method: exec_module</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/general_importer.py#L33'>Method: find_spec</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L8'>Class: ImportCatcher</a>
+│  └─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/import_catcher.py#L24'>Method: handle</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L30'>Class: MissingDependencyException</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/exception.py#L34'>Function: MissingOptionalDependency</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L63'>Function: fake_module_check</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L16'>Function: generalimport</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L12'>Function: get_importer</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L8'>Function: get_installed_modules_names</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L42'>Function: get_spec</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L29'>Function: import_module</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L43'>Function: is_imported</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L14'>Function: module_is_installed</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L48'>Function: module_is_namespace</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L52'>Function: module_name_is_namespace</a>
+├─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport/top.py#L38'>Function: reset_generalimport</a>
+└─ <a href='https://github.com/ManderaGeneral/generalimport/blob/master/generalimport_bottom.py#L45'>Function: spec_is_namespace</a>
 </pre>
 </details>
 
 
 <details open>
 <summary><h2>Contributions</h2></summary>
 
 Issue-creation, discussions and pull requests are most welcome!
 </details>
 
 
 
 <sup>
-Generated 2022-10-27 16:21 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/ee21333a'>ee21333a</a>.
+Generated 2023-06-02 23:27 CEST for commit <a href='https://github.com/ManderaGeneral/generalimport/commit/master'>master</a>.
 </sup>
 </details>
```

### Comparing `generalimport-0.3.1/examples/1minimal_example.py` & `generalimport-0.5.0/examples/1minimal_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 
 from notinstalled import missing_func  # No error
 
 missing_func()  # Error occurs here
 
 """
 ```
-MissingOptionalDependency: Optional dependency 'notinstalled' was used but it isn't installed.
+MissingDependencyException: Optional dependency 'notinstalled' was used but it isn't installed.
 ```
 
 Imports fail when they are **used**, *not* imported. 
 
 This means you don't need to keep checking if the package is installed before importing it.
 Simply import your optional package and use it like you would any package and let it fail wherever it fails, with a nice error message. """
```

### Comparing `generalimport-0.3.1/examples/2tests_showcase.py` & `generalimport-0.5.0/examples/2tests_showcase.py`

 * *Files identical despite different names*

### Comparing `generalimport-0.3.1/examples/4how_it_works.py` & `generalimport-0.5.0/examples/4how_it_works.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 """
  - When `generalimport` is instantiated it creates a new importer for `sys.meta_path`.
  - This importer will return 'fake' modules for matching names and scope.
  - The scope ensures only your own imports are faked.
- - The fake module will recursively return itself when asked for an attribute.
- - When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingOptionalDependency`.
+ - The fake module will recursively return a FakeModule instance when asked for an attribute.
+ - When used in any way (\_\_call\_\_, \_\_add\_\_, \_\_str\_\_ etc) it raises `generalimport.MissingDependencyException`.
  - This exception has the 'skip-exceptions' from `unittest` and `pytest` as bases, which means that tests will automatically be skipped.
 """
```

### Comparing `generalimport-0.3.1/generalimport/general_importer.py` & `generalimport-0.5.0/generalimport/general_importer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import importlib
 import sys
 from logging import getLogger
 
-from generalimport import FakeModule, spec_is_namespace, _get_top_name, get_spec, fake_module_check, module_is_namespace
+from generalimport.fake_module import FakeModule
+from generalimport.generalimport_bottom import spec_is_namespace, _get_top_name, get_spec, fake_module_check, module_is_namespace
 
 
 class GeneralImporter:
     """ Creates fake packages if they don't exist.
         These fake packages' attrs are always a function that raises a ModuleNotFoundError when used.
         This lets you write a single line to handle all your optional dependencies.
         If wildcard (default "*") is provided then this will work on any missing package. """
 
     singleton_instance = None
 
     def __init__(self):
         self.catchers = []
+        self.latest_catcher = None
 
         self._singleton()
         self._skip_fullname = None
         sys.meta_path.insert(0, self)
 
     def catch(self, fullname):
         """ Return first catcher that handles given fullname and filename.
@@ -41,15 +43,15 @@
 
         if spec_is_namespace(spec=spec):
             return self._handle_handle(fullname=fullname, reason="Namespace package")
 
         return self._handle_relay(fullname=fullname, spec=spec)
 
     def create_module(self, spec):
-        return FakeModule(spec=spec)
+        return FakeModule(spec=spec, catcher=self.latest_catcher)
 
     def exec_module(self, module):
         pass
 
 
 
     def _singleton(self):
@@ -73,19 +75,19 @@
             return False
 
     def _handle_ignore(self, fullname, reason):
         getLogger(__name__).debug(f"Ignoring '{fullname}' - {reason}")
         return None
 
     def _handle_handle(self, fullname, reason):
-        catcher = self.catch(fullname=fullname)
-        if not catcher:
+        self.latest_catcher = self.catch(fullname=fullname)
+        if not self.latest_catcher:
             return self._handle_ignore(fullname=fullname, reason="Unhandled")
 
-        getLogger(__name__).info(f"{catcher} is handling '{fullname}' - {reason}")
+        getLogger(__name__).info(f"{self.latest_catcher} is handling '{fullname}' - {reason}")
 
         sys.modules.pop(fullname, None)  # Remove possible namespace
 
         return importlib.util.spec_from_loader(fullname, self)
 
     def _handle_relay(self, fullname, spec):
         getLogger(__name__).debug(f"'{fullname}' exists, returning it's spec '{spec}'")
```

### Comparing `generalimport-0.3.1/generalimport/generalimport_bottom.py` & `generalimport-0.5.0/generalimport/generalimport_bottom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib
 import pkgutil
 import sys
+from inspect import getmodule
 from pathlib import Path
 
 
 def get_installed_modules_names():
     """ https://stackoverflow.com/a/73958089/3936044 """
     iter_modules = {module.name for module in pkgutil.iter_modules()}
     builtin = sys.builtin_module_names
@@ -59,32 +60,39 @@
 
     return is_namespace
 
 def fake_module_check(obj, error=True):
     """ Simple assertion to trigger error_func earlier if module isn't installed. """
     if type(obj).__name__ == "FakeModule":
         if error:
-            obj.error_func()
+            obj.error_func("fake_module_check")
         else:
             return True
     else:
         return False
 
 
-
 def _get_previous_frame_filename(depth):
     frame = sys._getframe(depth)
     files = ("importlib", "generalimport_bottom.py")
 
     while frame:
         filename = frame.f_code.co_filename
         frame_is_origin = all(file not in filename for file in files)
         if frame_is_origin:
             return filename
         frame = frame.f_back
 
+def _module_in_stack(module):
+    frame = sys._getframe(0)
+    while frame:
+        if getmodule(frame) is module:
+            return True
+        frame = frame.f_back
+    return False
+
 def _get_scope_from_filename(filename):
     last_part = Path(filename).parts[-1]
     return filename[0:filename.index(last_part)]
 
 def _get_top_name(fullname):
     return fullname.split(".")[0]
```

### Comparing `generalimport-0.3.1/generalimport/import_catcher.py` & `generalimport-0.5.0/generalimport/import_catcher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import dataclasses
 from logging import getLogger
+from typing import Optional, Union
 
-from generalimport import _get_previous_frame_filename, _get_top_name, _get_scope_from_filename
+from generalimport.generalimport_bottom import _get_previous_frame_filename, _get_top_name, _get_scope_from_filename
 
 
 class ImportCatcher:
     WILDCARD = "*"
 
-    def __init__(self, *names):
+    def __init__(self, *names, message=None):
         self.names = set(names)
+        self.message = message
+
         self.added_names = set()
         self.added_fullnames = set()
         self.enabled = True
         self._scope = self._get_scope()
 
         getLogger(__name__).info(f"Created Catcher with names {self.names} and scope {self._scope}")
 
@@ -48,7 +52,17 @@
 
     def _handle_scope(self):
         if self._scope is None:
             return True
         filename = _get_previous_frame_filename(depth=6)
         self.latest_scope_filename = filename
         return filename.startswith(self._scope)
+
+
+@dataclasses.dataclass
+class ErrorPars:
+    name: Optional[str]
+    trigger: Optional[str]
+    caller: str
+    catcher: Optional[ImportCatcher]
+    args: Union[list, tuple]
+    kwargs: dict
```

### Comparing `generalimport-0.3.1/generalimport/min.py` & `generalimport-0.5.0/generalimport/min.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+""" Standalone minimal example """
+
 import sys
 import importlib
 from unittest.case import SkipTest
 from _pytest.outcomes import Skipped
 
-class MissingOptionalDependency(SkipTest, Skipped):
+class MissingDependencyException(SkipTest, Skipped):
     def __init__(self, msg=None):
         self.msg = msg
     def __repr__(self):
-        return f"MissingOptionalDependency: {self.msg}" if self.msg else f"MissingOptionalDependency"
+        return f"MissingDependencyException: {self.msg}" if self.msg else f"MissingDependencyException"
 
 class GeneralImporter:
     def __init__(self, *names):
         self.names = names
         sys.meta_path.insert(0, self)
     def find_spec(self, fullname, path=None, target=None):
         if fullname in self.names:
@@ -21,13 +23,13 @@
     def exec_module(self, module):
         pass
 
 class FakeModule:
     def __init__(self, name):
         self.name = name
     def __call__(self, *args, **kwargs):
-        raise MissingOptionalDependency(f"Optional dependency '{self.name}' was used but it isn't installed.")
+        raise MissingDependencyException(f"Optional dependency '{self.name}' was used but it isn't installed.")
 
 GeneralImporter("notinstalled")
 import notinstalled  # No error
 print(notinstalled)  # <__main__.FakeModule object at 0x0000014B7F6D9E80>
-notinstalled()  # MissingOptionalDependency: Optional dependency 'notinstalled' was used but it isn't installed.
+notinstalled()  # MissingDependencyException: Optional dependency 'notinstalled' was used but it isn't installed.
```

### Comparing `generalimport-0.3.1/generalimport/test/test_generalimport.py` & `generalimport-0.5.0/generalimport/test/test_generalimport.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,39 +14,43 @@
         self.assertIn("mmap", get_installed_modules_names())  # built-in
         self.assertNotIn("doesntexist", get_installed_modules_names())
 
     def test_package_is_installed(self):
         self.assertEqual(True, module_is_installed("generalimport"))
         self.assertEqual(True, module_is_installed("setuptools"))
         self.assertEqual(False, module_is_installed("doesntexist"))
+    
+    def test_package_is_imported(self):
+        self.assertEqual(True, is_imported("generalimport"))
+        self.assertEqual(False, is_imported("setuptools"))
+        self.assertEqual(False, is_imported("doesntexist"))
+
+    def test_MissingDependencyException(self):
+        self.assertEqual("foo", MissingDependencyException("foo").msg)
+        self.assertIn("foo", repr(MissingDependencyException("foo")))
+        self.assertIn("foo", str(MissingDependencyException("foo")))
 
-    def test_MissingOptionalDependency(self):
-        self.assertEqual("foo", MissingOptionalDependency("foo").msg)
-        self.assertIn("foo", repr(MissingOptionalDependency("foo")))
-        self.assertIn("foo", str(MissingOptionalDependency("foo")))
-
-        self.assertEqual(None, MissingOptionalDependency().msg)
-        self.assertIn("MissingOptionalDependency", repr(MissingOptionalDependency()))
-        self.assertIn("MissingOptionalDependency", str(MissingOptionalDependency()))
+        self.assertIn("MissingDependencyException", repr(MissingDependencyException()))
+        self.assertEqual(str(AttributeError()), str(MissingDependencyException()))
 
     def test_GeneralImporter(self):
         generalimport("packagethatdoesntexist")
 
         self.assertIn(get_importer(), sys.meta_path)
 
         self.assertRaises(AssertionError, GeneralImporter)  # Singleton
 
         import packagethatdoesntexist
-        self.assertRaises(MissingOptionalDependency, packagethatdoesntexist)
+        self.assertRaises(MissingDependencyException, packagethatdoesntexist)
 
         from packagethatdoesntexist.module import fakefunc
-        self.assertRaises(MissingOptionalDependency, fakefunc)
+        self.assertRaises(MissingDependencyException, fakefunc)
 
         import packagethatdoesntexist.module.fakefunc2
-        self.assertRaises(MissingOptionalDependency, packagethatdoesntexist.module.fakefunc2)
+        self.assertRaises(MissingDependencyException, packagethatdoesntexist.module.fakefunc2)
 
         with self.assertRaises(ImportError):
             import notexisting
 
         with self.assertRaises(ImportError):
             from notexisting import hi
 
@@ -63,32 +67,32 @@
         import pkg_resources
         fake_module_check(pkg_resources)
 
     def test_wildcard(self):
         generalimport("*")
 
         from whateverz import this
-        self.assertRaises(MissingOptionalDependency, this)
+        self.assertRaises(MissingDependencyException, this)
 
         from whateverz.hi import that
-        self.assertRaises(MissingOptionalDependency, that)
+        self.assertRaises(MissingDependencyException, that)
 
         import hiii
-        self.assertRaises(MissingOptionalDependency, hiii)
+        self.assertRaises(MissingDependencyException, hiii)
 
         import heyyyy.foo
-        self.assertRaises(MissingOptionalDependency, heyyyy.foo)
+        self.assertRaises(MissingDependencyException, heyyyy.foo)
 
     def test_import_module(self):
         self.assertRaises(ModuleNotFoundError, import_module, "thisdoesntexist")
 
         generalimport("thisdoesntexist")
         thisdoesntexist = import_module("thisdoesntexist")
 
-        self.assertRaises(MissingOptionalDependency, thisdoesntexist)
+        self.assertRaises(MissingDependencyException, thisdoesntexist)
 
         self.assertIs(import_module("generalimport"), gi)
         import_module("generalimport")
 
     def test_import_module_namespace(self):
         self.assertIs(None, import_module("namespace", error=False))
         self.assertRaises(ModuleNotFoundError, import_module, "namespace")
@@ -97,15 +101,15 @@
         self.assertEqual(True, module_name_is_namespace("namespace"))
         self.assertEqual(True, module_name_is_namespace("namespace"))
 
         generalimport("namespace")
 
         from namespace.mod import func
 
-        self.assertRaises(MissingOptionalDependency, func)
+        self.assertRaises(MissingDependencyException, func)
 
     def test_generalimport(self):
         self.assertEqual(True, module_name_is_namespace("namespace"))
         self.assertEqual(True, module_name_is_namespace("namespace"))
 
         catcher = generalimport("namespace", "missing_dep")
         self.assertEqual(2, len(catcher.names))
@@ -113,23 +117,23 @@
         catcher2 = generalimport("another_missing")
         self.assertEqual(1, len(catcher2.names))
 
         import namespace
         import missing_dep
         import another_missing
 
-        self.assertRaises(MissingOptionalDependency, namespace.func)
-        self.assertRaises(MissingOptionalDependency, missing_dep.func)
-        self.assertRaises(MissingOptionalDependency, another_missing.func)
+        self.assertRaises(MissingDependencyException, namespace.func)
+        self.assertRaises(MissingDependencyException, missing_dep.func)
+        self.assertRaises(MissingDependencyException, another_missing.func)
 
     def test_fake_module_check(self):
         generalimport("fakepackage")
         import fakepackage
 
-        self.assertRaises(MissingOptionalDependency, fake_module_check, fakepackage)
+        self.assertRaises(MissingDependencyException, fake_module_check, fakepackage)
         self.assertIs(True, fake_module_check(fakepackage, error=False))
 
         fake_module_check(sys)
         self.assertIs(False, fake_module_check(sys, error=False))
 
     def test_import_catcher_scope(self):
         catcher = generalimport("hi")
@@ -173,17 +177,86 @@
     def test_latest_scope_filename_importlib(self):
         catcher = generalimport("hi")
 
         hi = importlib.import_module("hi")
         self.assertIs(True, fake_module_check(hi, error=False))
         self.assertIn("test_generalimport.py", catcher.latest_scope_filename)
 
+    def test_correct_message(self):
+        from generalimport import generalimport
+        generalimport("missing_dep")
+
+    def test_logging_message(self):
+        generalimport("nonexisting", "missing_dep")
+        import nonexisting
+
+        with self.assertLogs('generalimport', level='DEBUG') as cm:
+            with self.assertRaises(MissingDependencyException):
+                nonexisting.func()
+
+        self.assertIn("nonexisting", cm.output[0])
+        self.assertIn("__call__", cm.output[0])
+
+        from missing_dep import foo
+        from missing_dep import bar
+
+        try:
+            foo()
+        except MissingDependencyException as e:
+            self.assertIn("foo", str(e))
+        else:
+            self.fail("Error not raised")
+
+        try:
+            bar()
+        except MissingDependencyException as e:
+            self.assertIn("bar", str(e))
+        else:
+            self.fail("Error not raised")
+
+    def test_message(self):
+        generalimport("nonexisting", message="FooBar")
+        import nonexisting
+
+        try:
+            nonexisting()
+        except MissingDependencyException as e:
+            self.assertIn("FooBar", str(e))
+        else:
+            self.fail("Error not raised")
+
+    def test_catcher_relay_single(self):
+        catcher = generalimport("nonexisting")
+        import nonexisting
+
+        self.assertIs(nonexisting.catcher, catcher)
+
+    def test_catcher_relay_two(self):
+        catcher = generalimport("foo", "bar")
+        import foo
+        import bar
+
+        self.assertIs(foo.catcher, catcher)
+        self.assertIs(bar.catcher, catcher)
+
+    def test_catcher_relay_double(self):
+        catcher = generalimport("foo")
+        from foo import bar
+
+        self.assertIs(bar.catcher, catcher)
+
+    def test_catcher_relay_double_and_two(self):
+        foobar_catcher = generalimport("foo")
+        hiii_catcher = generalimport("hiii")
 
+        from foo import bar
+        import hiii
 
-
+        self.assertIs(bar.catcher, foobar_catcher)
+        self.assertIs(hiii.catcher, hiii_catcher)
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_binary.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_iterable.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,56 +3,55 @@
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
 class Test(ImportTestCase):
-    def test_ilshift(self):
+    def test_len(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage <<= 5
 
-    def test_irshift(self):
-        generalimport("fakepackage")
-        import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage >>= 5
+        with self.assertRaises(MissingDependencyException):
+            len(fakepackage)
 
-    def test_invert(self):
+    def test_next(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            ~fakepackage
 
-    def test_ixor(self):
+        with self.assertRaises(MissingDependencyException):
+            next(fakepackage)
+
+    def test_reversed(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage ^= 5
 
-    def test_lshift(self):
+        with self.assertRaises(MissingDependencyException):
+            reversed(fakepackage)
+
+    def test_contains(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage << 5
 
-    def test_rlshift(self):
+        with self.assertRaises(MissingDependencyException):
+            5 in fakepackage
+
+    def test_getitem(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            5 << fakepackage
 
-    def test_rrshift(self):
+        with self.assertRaises(MissingDependencyException):
+            fakepackage[0]
+
+    def test_index(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            5 >> fakepackage
 
-    def test_rshift(self):
+        with self.assertRaises(MissingDependencyException):
+            fakepackage.__index__()
+
+    def test_setitem(self):
         generalimport("fakepackage")
         import fakepackage
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage >> 5
-
 
+        with self.assertRaises(MissingDependencyException):
+            fakepackage[5] = "foo"
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_callable.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_callable.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,52 +4,52 @@
 
 
 class Test(ImportTestCase):
     def test_annotations(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__annotations__
 
     def test_call(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage()
 
     def test_closure(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__closure__
 
     def test_code(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__code__
 
     def test_defaults(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__defaults__
 
     def test_globals(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__globals__
 
     def test_kwdefaults(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage.__kwdefaults__
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_cast.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_cast.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,51 +7,51 @@
 
 
 class Test(ImportTestCase):
     def test_bool(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             bool(fakepackage)
 
     def test_bytes(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             bytes(fakepackage)
 
     def test_complex(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             complex(fakepackage)
 
     def test_float(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             float(fakepackage)
 
     def test_int(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             int(fakepackage)
 
     def test_iter(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             iter(fakepackage)
 
     def test_hash(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             hash(fakepackage)
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_compare.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_compare.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,63 +8,63 @@
 
 
 class Test(ImportTestCase):
     def test_eq(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage == 2
 
     def test_ge(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage >= 2
 
     def test_gt(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage > 2
 
     # https://github.com/ManderaGeneral/generalimport/issues/4
     @skip("Cannot cover `raise X` unless `isinstance(X, Y)` is covered.")
     def test_instancecheck(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             isinstance(fakepackage, int)
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             raise fakepackage  # This should work if we solve isinstance()
 
     def test_le(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage <= 2
 
     def test_lt(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage < 2
 
     def test_ne(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage != 2
 
     def test_subclasscheck(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             issubclass(int, fakepackage)
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_context.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_lookup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,39 @@
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
 class Test(ImportTestCase):
-    def test_enter(self):
+    def test_class_getitem(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            with fakepackage:
-                pass
+        with self.assertRaises(MissingDependencyException):
+            type(fakepackage)[5]
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage.__enter__()
+    def test_dir(self):
+        generalimport("fakepackage")
+        import fakepackage
+
+        with self.assertRaises(MissingDependencyException):
+            dir(fakepackage)
 
-    def test_exit(self):
+    # https://github.com/ManderaGeneral/generalimport/issues/8
+    @skip("Cannot cover __setattr__ as it won't allow `import foo.bar`.")
+    def test_setattr(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage.__exit__()
+        with self.assertRaises(MissingDependencyException):
+            fakepackage.x = 5
+
+
+
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_delete.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_delete.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 
 class Test(ImportTestCase):
     def test_delattr(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             del fakepackage.foo
 
     def test_delitem(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             del fakepackage[5]
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_info.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,34 @@
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
 class Test(ImportTestCase):
-    def test_sizeof(self):
+    def test_imatmul(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            sys.getsizeof(fakepackage)
+        with self.assertRaises(MissingDependencyException):
+            fakepackage @= 5
 
-    def test_subclasses(self):
+    def test_matmul(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage.__subclasses__()
+        with self.assertRaises(MissingDependencyException):
+            fakepackage @ 2
+
+    def test_rmatmul(self):
+        generalimport("fakepackage")
+        import fakepackage
+
+        with self.assertRaises(MissingDependencyException):
+            2 @ fakepackage
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_logic.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,69 +4,31 @@
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
 class Test(ImportTestCase):
-    def test_and(self):
+    def test_enter(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage & "foo"
+        with self.assertRaises(MissingDependencyException):
+            with fakepackage:
+                pass
 
-    def test_iand(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage &= "foo"
-
-    def test_ior(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage |= "foo"
-
-    def test_or(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage | "foo"
-
-    def test_rand(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            "foo" & fakepackage
-
-    def test_ror(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            "foo" | fakepackage
-
-    def test_rxor(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            "foo" ^ fakepackage
+        with self.assertRaises(MissingDependencyException):
+            fakepackage.__enter__()
 
-    def test_xor(self):
+    def test_exit(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage ^ "foo"
+        with self.assertRaises(MissingDependencyException):
+            fakepackage.__exit__()
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_lookup.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import sys
-from unittest import skip
+from unittest import skip, IsolatedAsyncioTestCase
 
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
-class Test(ImportTestCase):
-    def test_class_getitem(self):
+class Test(IsolatedAsyncioTestCase, ImportTestCase):
+    async def test_aenter(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            type(fakepackage)[5]
+        with self.assertRaises(MissingDependencyException):
+            async with fakepackage():
+                pass
 
-    def test_dir(self):
+    async def test_aiter(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            dir(fakepackage)
+        with self.assertRaises(MissingDependencyException):
+            async for x in fakepackage:
+                pass
 
-    # https://github.com/ManderaGeneral/generalimport/issues/8
-    @skip("Cannot cover __setattr__ as it won't allow `import foo.bar`.")
-    def test_setattr(self):
+    async def test_await(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage.x = 5
-
-
-
+        with self.assertRaises(MissingDependencyException):
+            await fakepackage
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_math.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_math.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,225 +9,225 @@
 
 
 class Test(ImportTestCase):
     def test_abs(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             abs(fakepackage)
 
     def test_add(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage + 3
 
     def test_ceil(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             math.ceil(fakepackage)
 
     def test_divmod(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             divmod(fakepackage, 5)
 
     def test_floor(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             math.floor(fakepackage)
 
     def test_floordiv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage // 2
 
     def test_iadd(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage += 2
 
     def test_ifloordiv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage //= 3
 
     def test_imod(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage %= 2
 
     def test_imul(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage *= 2
 
     def test_ipow(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage **= 5
 
     def test_isub(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage -= 3
 
     def test_itruediv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage /= 2
 
     def test_mod(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage % 2
 
     def test_mul(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage * 2
 
     def test_neg(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             -fakepackage
 
     def test_pos(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             +fakepackage
 
     def test_pow(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             math.pow(fakepackage, 2)
 
     def test_radd(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() + fakepackage
 
     def test_rdiv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() / fakepackage
 
     def test_rdivmod(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             divmod(object(), fakepackage)
 
     def test_rfloordiv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() // fakepackage
 
     def test_rmod(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() % fakepackage
 
     def test_rmul(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() * fakepackage
 
     def test_round(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             round(fakepackage)
 
     def test_rpow(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             math.pow(5, fakepackage)
 
     def test_rsub(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() - fakepackage
 
     def test_rtruediv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             object() / fakepackage
 
     def test_sub(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage - 5
 
     def test_truediv(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             fakepackage / 5
 
     def test_trunc(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             math.trunc(fakepackage)
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_matrix.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,34 +4,27 @@
 import generalimport as gi
 from generalimport import *
 
 from generalimport.test.funcs import ImportTestCase
 
 
 class Test(ImportTestCase):
-    def test_imatmul(self):
+    def test_sizeof(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage @= 5
+        with self.assertRaises(MissingDependencyException):
+            sys.getsizeof(fakepackage)
 
-    def test_matmul(self):
+    def test_subclasses(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
-            fakepackage @ 2
-
-    def test_rmatmul(self):
-        generalimport("fakepackage")
-        import fakepackage
-
-        with self.assertRaises(MissingOptionalDependency):
-            2 @ fakepackage
+        with self.assertRaises(MissingDependencyException):
+            fakepackage.__subclasses__()
```

### Comparing `generalimport-0.3.1/generalimport/test/test_usage/test_string.py` & `generalimport-0.5.0/generalimport/test/test_usage/test_string.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,39 +9,39 @@
 
 
 class Test(ImportTestCase):
     def test_format(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             format(fakepackage)
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             "{}".format(fakepackage)
 
     def test_fspath(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             os.fspath(fakepackage)
 
     def test_repr(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             repr(fakepackage)
 
     def test_str(self):
         generalimport("fakepackage")
         import fakepackage
 
-        with self.assertRaises(MissingOptionalDependency):
+        with self.assertRaises(MissingDependencyException):
             str(fakepackage)
```

### Comparing `generalimport-0.3.1/generalimport.egg-info/SOURCES.txt` & `generalimport-0.5.0/generalimport.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 metadata.json
 setup.py
 examples/1minimal_example.py
 examples/2tests_showcase.py
 examples/3recommended_setup.py
 examples/4how_it_works.py
 generalimport/__init__.py
+generalimport/dunders.py
 generalimport/exception.py
 generalimport/fake_module.py
 generalimport/general_importer.py
 generalimport/generalimport_bottom.py
 generalimport/import_catcher.py
 generalimport/min.py
 generalimport/top.py
@@ -32,9 +33,11 @@
 generalimport/test/test_usage/test_iterable.py
 generalimport/test/test_usage/test_logic.py
 generalimport/test/test_usage/test_lookup.py
 generalimport/test/test_usage/test_math.py
 generalimport/test/test_usage/test_matrix.py
 generalimport/test/test_usage/test_object.py
 generalimport/test/test_usage/test_pickle.py
+generalimport/test/test_usage/test_raise.py
 generalimport/test/test_usage/test_string.py
-generalimport/test/test_usage/test_thread.py
+generalimport/test/test_usage/test_thread.py
+generalimport/test/test_usage/test_typing.py
```

### Comparing `generalimport-0.3.1/setup.py` & `generalimport-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 except FileNotFoundError:
     long_description = 'Readme missing'
 
 setup(
     name="generalimport",
     author='Rickard "Mandera" Abraham',
     author_email="rickard.abraham@gmail.com",
-    version="0.3.1",
+    version="0.5.0",
     description="Handle all your optional dependencies with a single call!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/ManderaGeneral/generalimport",
     license="mit",
     packages=find_namespace_packages(exclude=("build*", "dist*")),
```

