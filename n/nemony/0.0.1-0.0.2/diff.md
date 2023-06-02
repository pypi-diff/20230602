# Comparing `tmp/nemony-0.0.1.tar.gz` & `tmp/nemony-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemony-0.0.1.tar", last modified: Tue May 16 12:21:08 2023, max compression
+gzip compressed data, was "nemony-0.0.2.tar", last modified: Fri Jun  2 09:53:16 2023, max compression
```

## Comparing `nemony-0.0.1.tar` & `nemony-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:21:08.847878 nemony-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 12:20:57.000000 nemony-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-16 12:21:08.847878 nemony-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-16 12:20:57.000000 nemony-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:21:08.843877 nemony-0.0.1/nemony/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 12:20:57.000000 nemony-0.0.1/nemony/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-16 12:20:57.000000 nemony-0.0.1/nemony/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-05-16 12:20:57.000000 nemony-0.0.1/nemony/nemony.py
--rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-05-16 12:20:57.000000 nemony-0.0.1/nemony/words.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:21:08.847878 nemony-0.0.1/nemony.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:21:08.000000 nemony-0.0.1/nemony.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-16 12:20:57.000000 nemony-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:21:08.847878 nemony-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:21:08.847878 nemony-0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-16 12:20:57.000000 nemony-0.0.1/test/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:53:16.538455 nemony-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 09:52:58.000000 nemony-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-02 09:53:16.538455 nemony-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-02 09:52:58.000000 nemony-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:53:16.538455 nemony-0.0.2/nemony/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 09:52:58.000000 nemony-0.0.2/nemony/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-02 09:52:58.000000 nemony-0.0.2/nemony/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-06-02 09:52:58.000000 nemony-0.0.2/nemony/nemony.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30324 2023-06-02 09:52:58.000000 nemony-0.0.2/nemony/words.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:53:16.538455 nemony-0.0.2/nemony.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 09:53:16.000000 nemony-0.0.2/nemony.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 09:52:58.000000 nemony-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:53:16.538455 nemony-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:53:16.538455 nemony-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-02 09:52:58.000000 nemony-0.0.2/test/tests.py
```

### Comparing `nemony-0.0.1/LICENSE` & `nemony-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nemony-0.0.1/PKG-INFO` & `nemony-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: nemony
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert text to adjective-noun mnemonics.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 Project-URL: Homepage, https://github.com/scbirlab/nemony
 Project-URL: Bug Tracker, https://github.com/scbirlab/nemony/issues
 Keywords: mnemonic,hash,programming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🧠 nemony
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/nemony/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nemony)
+![PyPI](https://img.shields.io/pypi/v/nemony)
+
 Deterministically encode text as mnemonic adjective-noun pairs.
 
 The same text should be identically encoded across systems. While
 there are currently more than 800,000 combinations of adjective and noun,
 collisions (two texts having the same mnemonic) can happen.
 
 ## Installation
@@ -115,15 +121,15 @@
 options:
   -h, --help            show this help message and exit
   --interactive, -i     Run interactively.
   --output [OUTPUT], -o [OUTPUT]
                         Output file. Default STDOUT.
 ```
 
-### Python package
+### Python API
 
 You can import **nemony** and use it to encode Python objects, as
 long as they can be converted to strings.
 
 ```python
 >>> import nemony as nm
 >>> nm.encode('world', sep='-')
@@ -136,18 +142,18 @@
 'receding_cheese'
 ```
 
 As a convenience, you can also use the SHA-256 hashing functions 
 (which use Python standard library `hashlib`).
 
 ```python
->>> hash('world')
+>>> nm.hash('world')
 '486ea46224d1bb4fb680f34f7c9ad96a8f24ec88be73ea8e5a6c65260e9cb8a7'
->>> hash('world', n=8)
+>>> nm.hash('world', n=8)
 '486ea462'
->>> hash(5., n=8)
+>>> nm.hash(5., n=8)
 'a19a1584'
 ```
 
 #### Documentation
 
-Check the Python API [here](https://nemony.readthedocs.io/).
+Check the Python API at [ReadTheDocs](https://nemony.readthedocs.io/).
```

### Comparing `nemony-0.0.1/README.md` & `nemony-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # 🧠 nemony
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/nemony/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nemony)
+![PyPI](https://img.shields.io/pypi/v/nemony)
+
 Deterministically encode text as mnemonic adjective-noun pairs.
 
 The same text should be identically encoded across systems. While
 there are currently more than 800,000 combinations of adjective and noun,
 collisions (two texts having the same mnemonic) can happen.
 
 ## Installation
@@ -96,15 +100,15 @@
 options:
   -h, --help            show this help message and exit
   --interactive, -i     Run interactively.
   --output [OUTPUT], -o [OUTPUT]
                         Output file. Default STDOUT.
 ```
 
-### Python package
+### Python API
 
 You can import **nemony** and use it to encode Python objects, as
 long as they can be converted to strings.
 
 ```python
 >>> import nemony as nm
 >>> nm.encode('world', sep='-')
@@ -117,18 +121,18 @@
 'receding_cheese'
 ```
 
 As a convenience, you can also use the SHA-256 hashing functions 
 (which use Python standard library `hashlib`).
 
 ```python
->>> hash('world')
+>>> nm.hash('world')
 '486ea46224d1bb4fb680f34f7c9ad96a8f24ec88be73ea8e5a6c65260e9cb8a7'
->>> hash('world', n=8)
+>>> nm.hash('world', n=8)
 '486ea462'
->>> hash(5., n=8)
+>>> nm.hash(5., n=8)
 'a19a1584'
 ```
 
 #### Documentation
 
-Check the Python API [here](https://nemony.readthedocs.io/).
+Check the Python API at [ReadTheDocs](https://nemony.readthedocs.io/).
```

### Comparing `nemony-0.0.1/nemony/cli.py` & `nemony-0.0.2/nemony/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Command line interface for nemony."""
 
 import argparse
 import sys
 
-from .nemony import encode, _get_corpus
+from .nemony import _check_version, _get_wordlist, encode 
 
 def _interactive_session() -> None:
 
-    print("\n(Ctrl-C to exit.)\nWhat would you like to encode?\n",
-          file=sys.stderr)
+    print("", "(Ctrl-C to exit.)", "What would you like to encode?",
+          sep='\n',
+          file=sys.stderr, flush=True)
 
     while True:
 
         try:
+
             x = input("?> ")
+        
+        except KeyboardInterrupt or EOFError:
 
-            print(encode(x))
+            break
 
-        except KeyboardInterrupt:
+        else:
 
-            break
+            if len(x) > 0:
+                print(encode(x), flush=True)
 
     return None
 
 
 def main() -> None:
 
     parser = argparse.ArgumentParser(description='''
@@ -41,19 +46,20 @@
                         type=argparse.FileType('w'),
                         default=sys.stdout,
                         nargs='?',
                         help='Output file. Default STDOUT.')
     
     args = parser.parse_args()
 
-    adjectives, nouns = _get_corpus()
+    adjectives, nouns = _get_wordlist()
+    version_name = _check_version()
 
     print('\n## MNEMO: Generate adjective-noun mnemonics',
           file=sys.stderr)
-    print(f'Word list version: {encode(adjectives + nouns)}\n',
+    print(f'Word list version: {version_name}\n',
           f'- Number of adjectives: {len(adjectives)}\n',
           f'- Number of nouns: {len(nouns)}\n',
           f'- Combinations: {len(adjectives) * len(nouns)}\n',
           file=sys.stderr)
     
     if args.interactive:
```

### Comparing `nemony-0.0.1/nemony/nemony.py` & `nemony-0.0.2/nemony/nemony.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 """Encoding Python objects as mnemonic adjective-noun pairs.
 
 Currently supports strings, iterables, floats and ints.
 
 """
 
+from __future__ import annotations
+
 from typing import Union
 from collections.abc import Sequence, Iterable
 
 from functools import singledispatch
 import hashlib
 import os
 import sys
 
 import yaml
 
+def _get_data_path():
+
+    return os.path.join(os.path.dirname(__file__), 'words.yml')
 
-def _get_corpus() -> Sequence[Sequence[str]]:
 
-    _data_path = os.path.join(os.path.dirname(__file__), 
-                              'words.yml')
+def _load_corpus():
+
+    _data_path = _get_data_path()
 
     with open(_data_path, 'r') as f:
         _words = yaml.safe_load(f)
 
+    return _words
+
+
+def _get_wordlist(full: bool = False) -> Sequence[Sequence[str]]:
+
+    _words = _load_corpus()
+
     versions = _words['versions']
     word_lists = _words['word lists']
     latest_version = versions[0]
 
     adjectives = list(set(word_lists[latest_version]['adjectives']))
     adjectives.sort()
     nouns = list(set(word_lists[latest_version]['nouns']))
     nouns.sort()
 
-    version_name = encode(adjectives + nouns,
-                          wordlist=(adjectives, nouns))
+    if full:
+        return adjectives, nouns, latest_version, _words
+    else:
+        return adjectives, nouns
     
-    if version_name != latest_version:
-
-        print(f'INFO: Word list has changed compared to {latest_version}. '
-              f'Saving new list as {version_name}.',
-              file=sys.stderr)
-        _words['versions'] = [version_name] + _words['versions'][1:]
-        del  _words['word lists'][latest_version]
-        _words['word lists'][version_name] = dict(adjectives=adjectives, 
-                                                  nouns=nouns)
-
-        with open(_data_path, 'w') as f:
-            yaml.safe_dump(_words, f, 
-                    default_flow_style=False, 
-                    width=80, indent=1)
-            
-        return _get_corpus()
-
-    return adjectives, nouns
-
 
 @singledispatch
 def hash(x, *args, **kwargs) -> str:
 
     """Hash an object using SHA-256 and take the first `n` hexadecimal digits.
 
     Parameters
@@ -172,18 +167,49 @@
     >>> encode(5.)
     'live_drum'
     >>> encode(['hello', 'world']) == encode(('hello', 'world'))
     True
 
     """
 
-    adjectives, nouns = wordlist or _get_corpus()
+    adjectives, nouns = wordlist or _DEFAULT_WORDLIST
 
     # Take the first n characters of the hash and convert to an integer
     integer = int(hash(x, n=n), base=16)
 
     # Generate the two-word mnemonic from the hashed integer
     adjective = adjectives[integer % len(adjectives)]
     noun = nouns[(integer // len(adjectives)) % len(nouns)]
     mnemonic = sep.join((adjective, noun))
 
     return mnemonic
+
+
+def _check_version() -> None:
+
+    adjectives, nouns, latest_version, _words = _get_wordlist(full=True)
+
+    versions = _words['versions']
+    latest_version = versions[0]
+
+    version_name = encode(adjectives + nouns,
+                          wordlist=(adjectives, nouns))
+    
+    if version_name != latest_version:
+
+        print(f'INFO: Word list has changed compared to {latest_version}. '
+              f'Saving new list as {version_name}.',
+              file=sys.stderr)
+        _words['versions'] = [version_name] + _words['versions'][1:]
+        del  _words['word lists'][latest_version]
+        _words['word lists'][version_name] = dict(adjectives=adjectives, 
+                                                  nouns=nouns)
+
+        with open(_get_data_path(), 'w') as f:
+            yaml.safe_dump(_words, f, 
+                    default_flow_style=False, 
+                    width=80, indent=1)
+            
+    return version_name
+
+_check_version()
+_DEFAULT_WORDLIST = _get_wordlist()
```

### Comparing `nemony-0.0.1/nemony/words.yml` & `nemony-0.0.2/nemony/words.yml`

 * *Files identical despite different names*

### Comparing `nemony-0.0.1/nemony.egg-info/PKG-INFO` & `nemony-0.0.2/nemony.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: nemony
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert text to adjective-noun mnemonics.
 Author-email: Eachan Johnson <eachan.johnson@crick.ac.uk>
 Project-URL: Homepage, https://github.com/scbirlab/nemony
 Project-URL: Bug Tracker, https://github.com/scbirlab/nemony/issues
 Keywords: mnemonic,hash,programming
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🧠 nemony
 
+![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/scbirlab/nemony/python-publish.yml)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/nemony)
+![PyPI](https://img.shields.io/pypi/v/nemony)
+
 Deterministically encode text as mnemonic adjective-noun pairs.
 
 The same text should be identically encoded across systems. While
 there are currently more than 800,000 combinations of adjective and noun,
 collisions (two texts having the same mnemonic) can happen.
 
 ## Installation
@@ -115,15 +121,15 @@
 options:
   -h, --help            show this help message and exit
   --interactive, -i     Run interactively.
   --output [OUTPUT], -o [OUTPUT]
                         Output file. Default STDOUT.
 ```
 
-### Python package
+### Python API
 
 You can import **nemony** and use it to encode Python objects, as
 long as they can be converted to strings.
 
 ```python
 >>> import nemony as nm
 >>> nm.encode('world', sep='-')
@@ -136,18 +142,18 @@
 'receding_cheese'
 ```
 
 As a convenience, you can also use the SHA-256 hashing functions 
 (which use Python standard library `hashlib`).
 
 ```python
->>> hash('world')
+>>> nm.hash('world')
 '486ea46224d1bb4fb680f34f7c9ad96a8f24ec88be73ea8e5a6c65260e9cb8a7'
->>> hash('world', n=8)
+>>> nm.hash('world', n=8)
 '486ea462'
->>> hash(5., n=8)
+>>> nm.hash(5., n=8)
 'a19a1584'
 ```
 
 #### Documentation
 
-Check the Python API [here](https://nemony.readthedocs.io/).
+Check the Python API at [ReadTheDocs](https://nemony.readthedocs.io/).
```

### Comparing `nemony-0.0.1/pyproject.toml` & `nemony-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [project]
 name = "nemony"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Eachan Johnson", email="eachan.johnson@crick.ac.uk" },
 ]
 description = "Convert text to adjective-noun mnemonics."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["mnemonic", "hash", "programming"]
 
 classifiers = [  
   
   "Development Status :: 3 - Alpha",
 
   # Indicate who your project is intended for
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Bio-Informatics",
 
   "License :: OSI Approved :: MIT License",
 
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [ 
   "pyyaml"
```

