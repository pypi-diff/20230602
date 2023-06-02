# Comparing `tmp/teaching-toolshed-0.1.9.tar.gz` & `tmp/teaching-toolshed-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teaching-toolshed-0.1.9.tar", max compression
+gzip compressed data, was "teaching-toolshed-0.2.0.tar", max compression
```

## Comparing `teaching-toolshed-0.1.9.tar` & `teaching-toolshed-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2021-12-29 18:48:12.748860 teaching-toolshed-0.1.9/LICENSE
--rw-r--r--   0        0        0      618 2022-10-08 02:56:12.775030 teaching-toolshed-0.1.9/README.md
--rw-r--r--   0        0        0      410 2023-06-02 19:48:53.638725 teaching-toolshed-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      132 2023-03-21 03:10:15.106159 teaching-toolshed-0.1.9/teachingtoolshed/__init__.py
--rw-r--r--   0        0        0       21 2021-12-29 18:48:12.749403 teaching-toolshed-0.1.9/teachingtoolshed/api/__init__.py
--rw-r--r--   0        0        0    20959 2023-06-02 19:47:43.544654 teaching-toolshed-0.1.9/teachingtoolshed/api/edstem.py
--rw-r--r--   0        0        0       94 2021-12-29 18:48:12.749634 teaching-toolshed-0.1.9/teachingtoolshed/gradebook/__init__.py
--rw-r--r--   0        0        0     7356 2022-12-20 03:05:41.303371 teaching-toolshed-0.1.9/teachingtoolshed/gradebook/canvas.py
--rw-r--r--   0        0        0     4190 2022-12-19 22:54:51.051819 teaching-toolshed-0.1.9/teachingtoolshed/gradebook/csv_readers.py
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 teaching-toolshed-0.1.9/setup.py
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 teaching-toolshed-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-12-29 18:48:12.748860 teaching-toolshed-0.2.0/LICENSE
+-rw-r--r--   0        0        0      618 2022-10-08 02:56:12.775030 teaching-toolshed-0.2.0/README.md
+-rw-r--r--   0        0        0      410 2023-06-02 19:59:25.639895 teaching-toolshed-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-03-21 03:10:15.106159 teaching-toolshed-0.2.0/teachingtoolshed/__init__.py
+-rw-r--r--   0        0        0       21 2021-12-29 18:48:12.749403 teaching-toolshed-0.2.0/teachingtoolshed/api/__init__.py
+-rw-r--r--   0        0        0    20954 2023-06-02 19:58:39.357431 teaching-toolshed-0.2.0/teachingtoolshed/api/edstem.py
+-rw-r--r--   0        0        0       94 2021-12-29 18:48:12.749634 teaching-toolshed-0.2.0/teachingtoolshed/gradebook/__init__.py
+-rw-r--r--   0        0        0     7356 2022-12-20 03:05:41.303371 teaching-toolshed-0.2.0/teachingtoolshed/gradebook/canvas.py
+-rw-r--r--   0        0        0     4190 2022-12-19 22:54:51.051819 teaching-toolshed-0.2.0/teachingtoolshed/gradebook/csv_readers.py
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.0/setup.py
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 teaching-toolshed-0.2.0/PKG-INFO
```

### Comparing `teaching-toolshed-0.1.9/LICENSE` & `teaching-toolshed-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.1.9/README.md` & `teaching-toolshed-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.1.9/teachingtoolshed/api/edstem.py` & `teaching-toolshed-0.2.0/teachingtoolshed/api/edstem.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,15 +472,15 @@
             no_attempt: Check; "Show empty attempts: Create a row for the user in the results even if the user has not attempted the quiz"
 
         Returns:
             Bytes content of the result file. Usually will be used to save to a file.
 
         """
         quiz_path = urljoin(
-                EdStemAPI.API_URL, "lessons/slides", quiz_id, "que:quizstions/results"
+                EdStemAPI.API_URL, "lessons/slides", quiz_id, "questions/results"
         )
         result = self._ed_post_request(
             quiz_path,
             {
                 "students": students,
                 "noAttempt": no_attempt,
             },
```

### Comparing `teaching-toolshed-0.1.9/teachingtoolshed/gradebook/canvas.py` & `teaching-toolshed-0.2.0/teachingtoolshed/gradebook/canvas.py`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.1.9/teachingtoolshed/gradebook/csv_readers.py` & `teaching-toolshed-0.2.0/teachingtoolshed/gradebook/csv_readers.py`

 * *Files identical despite different names*

### Comparing `teaching-toolshed-0.1.9/setup.py` & `teaching-toolshed-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=1.5.0,<2.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'teaching-toolshed',
-    'version': '0.1.9',
+    'version': '0.2.0',
     'description': 'Helpful libraries for running classes',
     'long_description': '# Teaching Toolshed\n\nA library of useful classes for writing scripts related to managing classes. Has helper classes for talking to various teaching APIs and for compiling gradebooks in Python. \n\nSee [Teaching Toolshed Examples](https://github.com/hschafer/teaching-toolshed-examples) to see example scripts of how these libraries are used in my classes.\n\nAny questions or comments can be handled here on GitHub or you can email me at [hschafer@cs.washington.edu](mailto:hschafer@cs.washington.edu).\n\n## Publish New Version\n\nSee [here](https://realpython.com/pypi-publish-python-package/#publish-your-package-to-pypi)\n',
     'author': 'Hunter Schafer',
     'author_email': 'hschafer@uw.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `teaching-toolshed-0.1.9/PKG-INFO` & `teaching-toolshed-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teaching-toolshed
-Version: 0.1.9
+Version: 0.2.0
 Summary: Helpful libraries for running classes
 License: MIT
 Author: Hunter Schafer
 Author-email: hschafer@uw.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

