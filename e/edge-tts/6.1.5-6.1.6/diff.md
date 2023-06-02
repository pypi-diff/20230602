# Comparing `tmp/edge-tts-6.1.5.tar.gz` & `tmp/edge-tts-6.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-tts-6.1.5.tar", last modified: Sun Apr 30 20:57:05 2023, max compression
+gzip compressed data, was "edge-tts-6.1.6.tar", last modified: Fri Jun  2 17:06:26 2023, max compression
```

## Comparing `edge-tts-6.1.5.tar` & `edge-tts-6.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/.github/
--rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.5/.github/dependabot.yml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/.github/workflows/
--rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.5/.github/workflows/code-quality.yml
--rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.5/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.5/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.5/.isort.cfg
--rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.5/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-04-30 20:57:05.573858 edge-tts-6.1.5/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-04-30 20:56:25.000000 edge-tts-6.1.5/README.md
--rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.5/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      957 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/basic_audio_streaming.py
--rw-rw-r--   0 user      (1000) user      (1000)      444 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/basic_generation.py
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/dynamic_voice_selection.py
--rw-rw-r--   0 user      (1000) user      (1000)     1022 2023-04-26 22:07:39.000000 edge-tts-6.1.5/examples/streaming_with_subtitles.py
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.5/format.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.5/lint.sh
--rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.5/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.5/pylintrc
--rw-rw-r--   0 user      (1000) user      (1000)      834 2023-04-30 20:57:05.573858 edge-tts-6.1.5/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.5/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_playback/
--rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.5/src/edge_playback/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.5/src/edge_playback/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.5/src/edge_playback/py.typed
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_tts/
--rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.5/src/edge_tts/__init__.py
--rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.5/src/edge_tts/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    17073 2023-04-30 20:46:32.000000 edge-tts-6.1.5/src/edge_tts/communicate.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.5/src/edge_tts/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.5/src/edge_tts/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.5/src/edge_tts/list_voices.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.5/src/edge_tts/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.5/src/edge_tts/submaker.py
--rw-rw-r--   0 user      (1000) user      (1000)     4343 2023-04-30 20:40:58.000000 edge-tts-6.1.5/src/edge_tts/util.py
--rw-rw-r--   0 user      (1000) user      (1000)      128 2023-04-30 20:56:50.000000 edge-tts-6.1.5/src/edge_tts/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-30 20:57:05.573858 edge-tts-6.1.5/src/edge_tts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-04-30 20:57:05.000000 edge-tts-6.1.5/src/edge_tts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.119232 edge-tts-6.1.6/.github/
+-rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.6/.github/dependabot.yml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/.github/workflows/
+-rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.6/.github/workflows/code-quality.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.6/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.6/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.6/.isort.cfg
+-rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.6/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-02 17:06:26.123232 edge-tts-6.1.6/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-04-30 20:56:25.000000 edge-tts-6.1.6/README.md
+-rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.6/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-02 17:04:37.000000 edge-tts-6.1.6/examples/basic_audio_streaming.py
+-rw-rw-r--   0 user      (1000) user      (1000)      492 2023-06-02 17:04:44.000000 edge-tts-6.1.6/examples/basic_generation.py
+-rw-rw-r--   0 user      (1000) user      (1000)      754 2023-06-02 17:04:50.000000 edge-tts-6.1.6/examples/dynamic_voice_selection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-02 17:04:56.000000 edge-tts-6.1.6/examples/streaming_with_subtitles.py
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.6/format.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.6/lint.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.6/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.6/pylintrc
+-rw-rw-r--   0 user      (1000) user      (1000)      834 2023-06-02 17:06:26.123232 edge-tts-6.1.6/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.6/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.119232 edge-tts-6.1.6/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_playback/
+-rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.6/src/edge_playback/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.6/src/edge_playback/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.6/src/edge_playback/py.typed
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_tts/
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.6/src/edge_tts/__init__.py
+-rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.6/src/edge_tts/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16836 2023-05-03 19:21:45.000000 edge-tts-6.1.6/src/edge_tts/communicate.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.6/src/edge_tts/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.6/src/edge_tts/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.6/src/edge_tts/list_voices.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.6/src/edge_tts/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.6/src/edge_tts/submaker.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4385 2023-06-02 17:05:35.000000 edge-tts-6.1.6/src/edge_tts/util.py
+-rw-rw-r--   0 user      (1000) user      (1000)      128 2023-06-02 17:06:07.000000 edge-tts-6.1.6/src/edge_tts/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_tts.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/top_level.txt
```

### Comparing `edge-tts-6.1.5/.github/workflows/code-quality.yml` & `edge-tts-6.1.6/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/.github/workflows/codeql-analysis.yml` & `edge-tts-6.1.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/.gitignore` & `edge-tts-6.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/LICENSE` & `edge-tts-6.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/PKG-INFO` & `edge-tts-6.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.5
+Version: 6.1.6
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.5/README.md` & `edge-tts-6.1.6/README.md`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/examples/basic_audio_streaming.py` & `edge-tts-6.1.6/examples/basic_audio_streaming.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 import edge_tts
 
 TEXT = "Hello World!"
 VOICE = "en-GB-SoniaNeural"
 OUTPUT_FILE = "test.mp3"
 
 
-async def _main() -> None:
+async def amain() -> None:
+    """Main function"""
     communicate = edge_tts.Communicate(TEXT, VOICE)
     with open(OUTPUT_FILE, "wb") as file:
         async for chunk in communicate.stream():
             if chunk["type"] == "audio":
                 file.write(chunk["data"])
             elif chunk["type"] == "WordBoundary":
                 print(f"WordBoundary: {chunk}")
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
+    loop = asyncio.get_event_loop_policy().get_event_loop()
     try:
-        loop.run_until_complete(_main())
+        loop.run_until_complete(amain())
     finally:
         loop.close()
```

### Comparing `edge-tts-6.1.5/examples/dynamic_voice_selection.py` & `edge-tts-6.1.6/examples/dynamic_voice_selection.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 import edge_tts
 from edge_tts import VoicesManager
 
 TEXT = "Hoy es un buen día."
 OUTPUT_FILE = "spanish.mp3"
 
 
-async def _main() -> None:
+async def amain() -> None:
+    """Main function"""
     voices = await VoicesManager.create()
     voice = voices.find(Gender="Male", Language="es")
     # Also supports Locales
     # voice = voices.find(Gender="Female", Locale="es-AR")
 
     communicate = edge_tts.Communicate(TEXT, random.choice(voice)["Name"])
     await communicate.save(OUTPUT_FILE)
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
+    loop = asyncio.get_event_loop_policy().get_event_loop()
     try:
-        loop.run_until_complete(_main())
+        loop.run_until_complete(amain())
     finally:
         loop.close()
```

### Comparing `edge-tts-6.1.5/examples/streaming_with_subtitles.py` & `edge-tts-6.1.6/examples/streaming_with_subtitles.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 
 TEXT = "Hello World!"
 VOICE = "en-GB-SoniaNeural"
 OUTPUT_FILE = "test.mp3"
 WEBVTT_FILE = "test.vtt"
 
 
-async def _main() -> None:
+async def amain() -> None:
+    """Main function"""
     communicate = edge_tts.Communicate(TEXT, VOICE)
     submaker = edge_tts.SubMaker()
     with open(OUTPUT_FILE, "wb") as file:
         async for chunk in communicate.stream():
             if chunk["type"] == "audio":
                 file.write(chunk["data"])
             elif chunk["type"] == "WordBoundary":
                 submaker.create_sub((chunk["offset"], chunk["duration"]), chunk["text"])
 
     with open(WEBVTT_FILE, "w", encoding="utf-8") as file:
         file.write(submaker.generate_subs())
 
 
 if __name__ == "__main__":
-    loop = asyncio.get_event_loop()
+    loop = asyncio.get_event_loop_policy().get_event_loop()
     try:
-        loop.run_until_complete(_main())
+        loop.run_until_complete(amain())
     finally:
         loop.close()
```

### Comparing `edge-tts-6.1.5/mypy.ini` & `edge-tts-6.1.6/mypy.ini`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/pylintrc` & `edge-tts-6.1.6/pylintrc`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/setup.cfg` & `edge-tts-6.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/src/edge_playback/__main__.py` & `edge-tts-6.1.6/src/edge_playback/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/src/edge_tts/communicate.py` & `edge-tts-6.1.6/src/edge_tts/communicate.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,29 +445,22 @@
         self,
         audio_fname: Union[str, bytes],
         metadata_fname: Optional[Union[str, bytes]] = None,
     ) -> None:
         """
         Save the audio and metadata to the specified files.
         """
-        written_audio: bool = False
         metadata: Union[TextIOWrapper, ContextManager[None]] = (
             open(metadata_fname, "w", encoding="utf-8")
             if metadata_fname is not None
             else nullcontext()
         )
         with metadata, open(audio_fname, "wb") as audio:
             async for message in self.stream():
                 if message["type"] == "audio":
                     audio.write(message["data"])
-                    written_audio = True
                 elif (
                     isinstance(metadata, TextIOWrapper)
                     and message["type"] == "WordBoundary"
                 ):
                     json.dump(message, metadata)
                     metadata.write("\n")
-
-        if not written_audio:
-            raise NoAudioReceived(
-                "No audio was received from the service, so the file is empty."
-            )
```

### Comparing `edge-tts-6.1.5/src/edge_tts/exceptions.py` & `edge-tts-6.1.6/src/edge_tts/exceptions.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/src/edge_tts/list_voices.py` & `edge-tts-6.1.6/src/edge_tts/list_voices.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/src/edge_tts/submaker.py` & `edge-tts-6.1.6/src/edge_tts/submaker.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.5/src/edge_tts/util.py` & `edge-tts-6.1.6/src/edge_tts/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
         if args.write_subtitles
         else sys.stderr
     )
     with sub_file:
         sub_file.write(subs.generate_subs(args.words_in_cue))
 
 
-async def _async_main() -> None:
+async def amain() -> None:
+    """Async main function"""
     parser = argparse.ArgumentParser(description="Microsoft Edge TTS")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("-t", "--text", help="what TTS will say")
     group.add_argument("-f", "--file", help="same as --text but read from file")
     parser.add_argument(
         "-v",
         "--voice",
@@ -127,16 +128,16 @@
 
     if args.text is not None:
         await _run_tts(args)
 
 
 def main() -> None:
     """Run the main function using asyncio."""
-    loop = asyncio.get_event_loop()
+    loop = asyncio.get_event_loop_policy().get_event_loop()
     try:
-        loop.run_until_complete(_async_main())
+        loop.run_until_complete(amain())
     finally:
         loop.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `edge-tts-6.1.5/src/edge_tts.egg-info/PKG-INFO` & `edge-tts-6.1.6/src/edge_tts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.5
+Version: 6.1.6
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.5/src/edge_tts.egg-info/SOURCES.txt` & `edge-tts-6.1.6/src/edge_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

