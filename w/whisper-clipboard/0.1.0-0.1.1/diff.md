# Comparing `tmp/whisper-clipboard-0.1.0.tar.gz` & `tmp/whisper-clipboard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-clipboard-0.1.0.tar", last modified: Thu Jun  1 22:29:06 2023, max compression
+gzip compressed data, was "whisper-clipboard-0.1.1.tar", last modified: Thu Jun  1 22:48:14 2023, max compression
```

## Comparing `whisper-clipboard-0.1.0.tar` & `whisper-clipboard-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:29:06.980066 whisper-clipboard-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 22:28:57.000000 whisper-clipboard-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 22:29:06.980066 whisper-clipboard-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-01 22:28:57.000000 whisper-clipboard-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:29:06.980066 whisper-clipboard-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-01 22:28:57.000000 whisper-clipboard-0.1.0/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-01 22:28:57.000000 whisper-clipboard-0.1.0/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:29:06.980066 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 22:29:06.000000 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 22:29:06.000000 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:29:06.000000 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 22:29:06.000000 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 22:29:06.000000 whisper-clipboard-0.1.0/whisper_clipboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 22:48:14.013825 whisper-clipboard-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-01 22:48:05.000000 whisper-clipboard-0.1.1/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 22:48:14.009825 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 22:48:13.000000 whisper-clipboard-0.1.1/whisper_clipboard.egg-info/top_level.txt
```

### Comparing `whisper-clipboard-0.1.0/LICENSE` & `whisper-clipboard-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.0/README.md` & `whisper-clipboard-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,40 +4,48 @@
 command line application that allows you to record audio and transcribe it using one of the
 [Whisper ASR models by OpenAI](https://openai.com/research/whisper). It uses a terminal user interface, making it easy to use.
 
 ## Prerequisites
 * Python 3.10 or higher (probably works with lower versions, but not tested)
 * ffmpeg
 
-## Installation
+## Installation from PyPI
+
+```
+pip install whisper-clipboard
+```
+And then run `transcribe` and start transcribing.
+Please make sure you have `ffmpeg` installed properly on your system (this may vary between different operating systems).
+
+## Installation using the repo
 
 ### For NixOS Users:
 
 ```bash
 # Step 1: Clone the repository.
-git clone https://github.com/data-stepper/whisper-transcribe
+git clone https://github.com/data-stepper/whisper-clipboard
 
 # Step 2: cd into the cloned repository.
-cd whisper-transcribe
+cd whisper-clipboard
 
 # Step 3: Run Nix-shell to set up the environment and install all necessary packages.
 nix-shell
 
 # Step 4: Run the Whisper Transcribe program.
 python transcribe.py
 ```
 
 ### For Non-NixOS Users:
 
 ```bash
 # Step 1: Clone the repository.
-git clone https://github.com/data-stepper/whisper-transcribe
+git clone https://github.com/data-stepper/whisper-clipboard
 
 # Step 2: cd into the cloned repository.
-cd whisper-transcribe
+cd whisper-clipboard
 
 # Step 3: (Optional) Create a virtual environment and activate it.
 python -m venv venv
 source venv/bin/activate
 # On Windows, activate the virtual environment with 'venv\Scripts\activate'
 
 # Step 4: Install the required packages.
```

### Comparing `whisper-clipboard-0.1.0/setup.py` & `whisper-clipboard-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,21 @@
+from os import path
+
 from setuptools import setup
 
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
+    long_description = f.read()
+
 setup(
     name="whisper-clipboard",
-    version="0.1.0",
+    version="0.1.1",
     description="A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Bent Mueller",
     author_email="bentmuller.ai@gmail.com",
     url="http://github.com/data-stepper/whisper-clipboard",
     py_modules=["transcribe"],
     entry_points={
         "console_scripts": [
             "transcribe = transcribe:main",
```

### Comparing `whisper-clipboard-0.1.0/transcribe.py` & `whisper-clipboard-0.1.1/transcribe.py`

 * *Files identical despite different names*

