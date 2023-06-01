# Comparing `tmp/whisper-clipboard-0.1.1.tar.gz` & `tmp/whisper-clipboard-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-clipboard-0.1.1.tar", last modified: Thu Jun  1 22:48:14 2023, max compression
+gzip compressed data, was "whisper-clipboard-0.1.2.tar", last modified: Thu Jun  1 23:02:12 2023, max compression
```

## Comparing `whisper-clipboard-0.1.1.tar` & `whisper-clipboard-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:48:14.009825 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/top_level.txt
```

### Comparing `whisper-clipboard-0.1.1/LICENSE` & `whisper-clipboard-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.1/PKG-INFO` & `whisper-clipboard-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.1
+Version: 0.1.2
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `whisper-clipboard-0.1.1/README.md` & `whisper-clipboard-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.1/setup.py` & `whisper-clipboard-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 from setuptools import setup
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
+
 setup(
     name="whisper-clipboard",
-    version="0.1.1",
+    version="0.1.2",
     description="A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Bent Mueller",
     author_email="bentmuller.ai@gmail.com",
     url="http://github.com/data-stepper/whisper-clipboard",
     py_modules=["transcribe"],
@@ -23,8 +26,9 @@
     },
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
+    install_requires=requirements,
 )
```

### Comparing `whisper-clipboard-0.1.1/transcribe.py` & `whisper-clipboard-0.1.2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.1/whisper_clipboard.egg-info/PKG-INFO` & `whisper-clipboard-0.1.2/whisper_clipboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.1
+Version: 0.1.2
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

