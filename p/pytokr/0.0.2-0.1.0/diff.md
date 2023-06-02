# Comparing `tmp/pytokr-0.0.2.tar.gz` & `tmp/pytokr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/balqui/Escritorio/RemoteBackups/github/hg/pytokr/dist/tmpnno7nhyk/pytokr-0.0.2.tar", last modified: Tue Apr  5 16:29:01 2022, max compression
+gzip compressed data, was "pytokr-0.1.0.tar", last modified: Fri Jun  2 06:22:08 2023, max compression
```

## Comparing `pytokr-0.0.2.tar` & `pytokr-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 balqui    (1000) balqui    (1000)        0 2022-04-05 16:29:01.000000 pytokr-0.0.2/
--rw-r--r--   0 balqui    (1000) balqui    (1000)      640 2022-04-05 16:29:01.000000 pytokr-0.0.2/setup.cfg
--rw-rw-r--   0 balqui    (1000) balqui    (1000)     1063 2022-03-23 12:22:12.000000 pytokr-0.0.2/LICENSE
--rw-rw-r--   0 balqui    (1000) balqui    (1000)     3758 2022-04-05 16:29:01.000000 pytokr-0.0.2/PKG-INFO
--rw-rw-r--   0 balqui    (1000) balqui    (1000)     3206 2022-04-05 16:20:35.000000 pytokr-0.0.2/README.md
-drwxrwxr-x   0 balqui    (1000) balqui    (1000)        0 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/
-drwxrwxr-x   0 balqui    (1000) balqui    (1000)        0 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr/
--rw-rw-r--   0 balqui    (1000) balqui    (1000)     2262 2022-04-05 16:20:10.000000 pytokr-0.0.2/src/pytokr/__init__.py
-drwxrwxr-x   0 balqui    (1000) balqui    (1000)        0 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr.egg-info/
--rw-rw-r--   0 balqui    (1000) balqui    (1000)        7 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr.egg-info/top_level.txt
--rw-rw-r--   0 balqui    (1000) balqui    (1000)     3758 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr.egg-info/PKG-INFO
--rw-rw-r--   0 balqui    (1000) balqui    (1000)        1 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr.egg-info/dependency_links.txt
--rw-rw-r--   0 balqui    (1000) balqui    (1000)      201 2022-04-05 16:29:01.000000 pytokr-0.0.2/src/pytokr.egg-info/SOURCES.txt
--rw-r--r--   0 balqui    (1000) balqui    (1000)       85 2022-03-23 12:28:01.000000 pytokr-0.0.2/pyproject.toml
+drwxrwxr-x   0 balqui    (1001) balqui    (1001)        0 2023-06-02 06:22:08.207288 pytokr-0.1.0/
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)     1063 2023-05-23 10:14:48.000000 pytokr-0.1.0/LICENSE
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)     5535 2023-06-02 06:22:08.207288 pytokr-0.1.0/PKG-INFO
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)     5014 2023-05-27 11:27:28.000000 pytokr-0.1.0/README.md
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)      600 2023-06-02 06:21:55.000000 pytokr-0.1.0/pyproject.toml
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)       38 2023-06-02 06:22:08.207288 pytokr-0.1.0/setup.cfg
+drwxrwxr-x   0 balqui    (1001) balqui    (1001)        0 2023-06-02 06:22:08.203288 pytokr-0.1.0/src/
+drwxrwxr-x   0 balqui    (1001) balqui    (1001)        0 2023-06-02 06:22:08.207288 pytokr-0.1.0/src/pytokr/
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)     6031 2023-05-27 10:56:38.000000 pytokr-0.1.0/src/pytokr/__init__.py
+drwxrwxr-x   0 balqui    (1001) balqui    (1001)        0 2023-06-02 06:22:08.207288 pytokr-0.1.0/src/pytokr.egg-info/
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)     5535 2023-06-02 06:22:08.000000 pytokr-0.1.0/src/pytokr.egg-info/PKG-INFO
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)      191 2023-06-02 06:22:08.000000 pytokr-0.1.0/src/pytokr.egg-info/SOURCES.txt
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)        1 2023-06-02 06:22:08.000000 pytokr-0.1.0/src/pytokr.egg-info/dependency_links.txt
+-rw-rw-r--   0 balqui    (1001) balqui    (1001)        7 2023-06-02 06:22:08.000000 pytokr-0.1.0/src/pytokr.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytokr-0.0.2/LICENSE` & `pytokr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytokr-0.0.2/PKG-INFO` & `pytokr-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,147 @@
-Metadata-Version: 2.1
-Name: pytokr
-Version: 0.0.2
-Summary: Very simple tokenizer for teaching purposes
-Home-page: https://github.com/balqui/pytokr
-Author: José Luis Balcázar
-Author-email: jose.luis.balcazar@upc.edu
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/balqui/pytokr/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pytokr
 
 Very simple, somewhat stoned tokenizer for teaching purposes.
 
+Current pip-installable version is 0.0.2 but the current status
+of the repository is version 0.1.0.
+
 Behaviorally inspired by the early versions of the 
 [easyinput module](https://github.com/jutge-org/easyinput); 
 shares with it some similar aims, but not the aim of 
-conceptual consistency with C/C++. Actually easyinput 
-has grown in ways I find inappropriate for many of my 
-students and I want to try now a different road.
+conceptual consistency with C/C++. 
 
-## Install
+<!--- Actually easyinput 
+has grown in ways I find somewhat inappropriate for 
+many of my current (non-CS) students and I want to 
+try now a different road. --->
+
+A separate, different evolution of `easyinput` is 
+[yogi](https://github.com/jutge-org/yogi).
 
-Current version is 0.0.2.
+## Install
 
-Trying to get it pip-ready these days. If that does not
-work, download or clone the repo, then put the pytokr
-folder where Python can see it from wherever you want 
-to use it.
+The usual incantation should work: pip install pytokr
+(maybe with either "sudo" or "--user" or within a 
+virtual environment).
+
+If that does not work, download or clone the repo, then 
+put the pytokr folder where Python can see it from 
+wherever you want to use it.
 
-## Simplest usage
+## Simplest usage since version 0.1.0
 
 Finds items (simple tokens white-space separated) in a 
 string-based iterable such as stdin (default). Ends of 
 line are counted as white space but are otherwise ignored. Usage:
 
-`from pytokr import item, items`
+`from pytokr import pytokr`
 
-(or only one of them as convenient). Then `item()` will provide
-the next item in `stdin` and `for w in items()` will iterate on
-whatever remains there. Calling `item()` at end of file will
-raise an exception StopIteration. Note that, as white-space is 
-ignored, in case only white-space remains then the program *is* 
-at end of file.
+then call pytokr to obtain the tokenizer function; give it 
+whatever name you see fit, say, `item`:
+
+`item = pytokr()`
+
+Then, successive calls to `item()` will provide you with
+successive tokens from `stdin`. In case no items remain,
+an EndOfDataError exception will be raised. Note that, 
+as white-space is ignored, in case only white-space remains 
+then the program *is* at end of data.
+
+If a different source of items is desired, say `source` 
+(e.g. a `file` just `open`'ed or a list of strings), 
+simply pass it on:
+
+`item = pytokr(source)`
+
+In either case, a second output can be requested, namely, an
+iterator over the items, say you want to name it `items`:
+
+`item, items = pytokr(iter = True)`
 
-Both calls combine naturally: it is valid to call `item()` 
+(such call would accept as well a `source` as first parameter).
+Then you can run `for itm in items():` or make up a `ls = list(items())`
+and, with some care, avoid the dependence on the EndOfDataError
+exception.
+
+Both combine naturally: the individual item function can be called 
+inside a for loop on the iterator, provided there is still 
+at least one item not yet read. That call will advance the 
+items; so, the next item at the loop will be the current one after 
+the local advances. Briefly: both advance *the same* iterator.
+
+<!--- Both calls combine naturally: it is valid to call `item()` 
 within a `for w in items()` loop provided there is still 
 at least one item not yet read. The reading will advance 
 on and the next item in the loop will correspond to the 
-advance. Briefly: both advance *the same* iterator.
+advance. 
+
+Token items are returned as strings; the user should cast them as
+int or float or whatever when appropriate. --->
 
 All items provided are of type `str` and will not contain 
 white space; casting into `int` or `float` or whatever, if
-convenient, falls upon the caller.
+convenient, falls upon the caller. 
 
 ## Example
 
 Based on [Jutge problem P29448](https://jutge.org/problems/P29448_en)
 Correct Dates (and removing spoilers):
 
-    from pytokr import items, item
+    from pytokr import pytokr
+    item, items = pytokr(f, iter = True)
     for d in items():
         m, y = item(), item()
         if correct_date(int(d), int(m), int(y)):
             print("Correct Date")
         else:
             print("Incorrect Date")
 
-## Usage on other string-based iterables
+## Deprecated usage of versions 0.0.*
+
+These versions were employed in a different manner. Version
+0.1.0 can still be employed in the same way for some
+backwards compatibility, but will print a deprecation
+message to `stderr`. This old usage was:
+
+`from pytokr import item, items`
+
+(or only one of them as convenient). Then `item()` will provide
+the next item in `stdin` and `for w in items()` will iterate on
+whatever remains there. Calling `item()` at end of file will
+raise an exception EndOfDataError. 
+
+### Old, deprecated usage on other string-based iterables
+
+Again, this still works on 0.1.0 but will print a deprecation
+message on `stderr`:
 
 `from pytokr import make_tokr`
 
 Then, if `g` is an iterable of strings such as an open
 file or a list of strings, the call
 
-`item, items = make_tokr(g)`
+`items, item = make_tokr(g)`
 
 will provide adapted versions of `item` and `items` that
 will read them in from `g` instead of from `stdin`.
 
-## To do: 
+<!--- ## To do: 
 
 - As said, call to `item()` raises `StopIteration` on 
 end of file; it will be a common error when mixing it 
 with `items()`. Consider catching it and raising instead 
 an exception more understandable by beginners.
 
-- Automatize a process that generates a jutge-testable 
-source even if jutge does not have pytokr (or, alternatively,
-get it to have pytokr).
-
 - Sources in the 'deprecated/jutge-like' folder use 
 obsolete identifiers; keep updating them and moving
 them to 'jutge_like'.
 
 - I called initially the items 'toks' (for very simple 
 'tokens') but that sounded a bit inappropriate to me, 
 first, because of the simplicity of the case and, 
 second, due to the early programming level of my 
 target students. Calling them 'items' seems suboptimal 
 though, since we are going to study `dict`'s later on 
 and then risk confusions. But I settled on 'items' for 
 the time being anyway; alternative suggestions welcome.
-
-
+--->
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

