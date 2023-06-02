# Comparing `tmp/padacioso-0.2.1a5.tar.gz` & `tmp/padacioso-0.2.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padacioso-0.2.1a5.tar", last modified: Tue May 16 16:22:38 2023, max compression
+gzip compressed data, was "padacioso-0.2.1a6.tar", last modified: Fri Jun  2 21:45:22 2023, max compression
```

## Comparing `padacioso-0.2.1a5.tar` & `padacioso-0.2.1a6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/padacioso/
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso/bracket_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/padacioso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/padacioso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:22:38.937206 padacioso-0.2.1a5/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-16 16:22:38.000000 padacioso-0.2.1a5/test/test_padacioso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/padacioso/
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso/bracket_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/padacioso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/padacioso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:45:22.849091 padacioso-0.2.1a6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-02 21:45:22.000000 padacioso-0.2.1a6/test/test_padacioso.py
```

### Comparing `padacioso-0.2.1a5/LICENSE.md` & `padacioso-0.2.1a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a5/padacioso/__init__.py` & `padacioso-0.2.1a6/padacioso/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,14 @@
                             penalty += 0.1
                     yield {"entities": entities or {},
                            "conf": 1 - penalty,
                            "name": intent_name}
                     break
 
                 if self.fuzz:
-                    LOG.debug(f"Fallback to fuzzy match")
                     penalty += 0.25
                     for f in self._get_fuzzed(r):
                         entities = simplematch.match(f, query,
                                                      case_sensitive=False)
                         if entities is not None:
                             yield {"entities": entities or {},
                                    "conf": 1 - penalty,
```

### Comparing `padacioso-0.2.1a5/padacioso/bracket_expansion.py` & `padacioso-0.2.1a6/padacioso/bracket_expansion.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a5/setup.py` & `padacioso-0.2.1a6/setup.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.1a5/test/test_padacioso.py` & `padacioso-0.2.1a6/test/test_padacioso.py`

 * *Files identical despite different names*

