# Comparing `tmp/whisper-clipboard-0.1.2.tar.gz` & `tmp/whisper-clipboard-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-clipboard-0.1.2.tar", last modified: Thu Jun  1 23:02:12 2023, max compression
+gzip compressed data, was "whisper-clipboard-0.1.3.tar", last modified: Thu Jun  1 23:20:32 2023, max compression
```

## Comparing `whisper-clipboard-0.1.2.tar` & `whisper-clipboard-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-01 23:02:02.000000 whisper-clipboard-0.1.2/transcribe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:02:12.528835 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 23:02:12.000000 whisper-clipboard-0.1.2/whisper_clipboard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2954 2023-06-01 23:20:24.000000 whisper-clipboard-0.1.3/transcribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 23:20:32.234173 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 23:20:32.000000 whisper-clipboard-0.1.3/whisper_clipboard.egg-info/top_level.txt
```

### Comparing `whisper-clipboard-0.1.2/LICENSE` & `whisper-clipboard-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.2/PKG-INFO` & `whisper-clipboard-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.2
+Version: 0.1.3
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `whisper-clipboard-0.1.2/README.md` & `whisper-clipboard-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `whisper-clipboard-0.1.2/setup.py` & `whisper-clipboard-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="whisper-clipboard",
-    version="0.1.2",
+    version="0.1.3",
     description="A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Bent Mueller",
     author_email="bentmuller.ai@gmail.com",
     url="http://github.com/data-stepper/whisper-clipboard",
     py_modules=["transcribe"],
```

### Comparing `whisper-clipboard-0.1.2/transcribe.py` & `whisper-clipboard-0.1.3/transcribe.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,18 +86,22 @@
             try:
                 _ = session.prompt("> ")
 
             except KeyboardInterrupt:
                 break
 
 
-if __name__ == "__main__":
+def main():
     print("Welcome to whisper-transcribe! \n")
     print("Instructions:")
     print("Press 'Space' to start / stop recording.")
     print("Press 'Q', Ctrl+D or Ctrl+C to quit the application.")
     print("Transcriptions are automatically copied to clipboard.")
     print()
 
     with tempfile.NamedTemporaryFile(suffix=".wav") as temp:
         recorder = Recorder(filename=temp.name)
         recorder.record_audio()
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `whisper-clipboard-0.1.2/whisper_clipboard.egg-info/PKG-INFO` & `whisper-clipboard-0.1.3/whisper_clipboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-clipboard
-Version: 0.1.2
+Version: 0.1.3
 Summary: A basic TUI for transcribing audio to your clipboard using OpenAI's whisper models.
 Home-page: http://github.com/data-stepper/whisper-clipboard
 Author: Bent Mueller
 Author-email: bentmuller.ai@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

