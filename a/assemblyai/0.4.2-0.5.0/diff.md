# Comparing `tmp/assemblyai-0.4.2.tar.gz` & `tmp/assemblyai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.4.2.tar", last modified: Wed May 31 20:09:39 2023, max compression
+gzip compressed data, was "assemblyai-0.5.0.tar", last modified: Fri Jun  2 10:53:50 2023, max compression
```

## Comparing `assemblyai-0.4.2.tar` & `assemblyai-0.5.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.404760 assemblyai-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 20:09:30.000000 assemblyai-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 20:09:39.404760 assemblyai-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-31 20:09:30.000000 assemblyai-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    44904 2023-05-31 20:09:30.000000 assemblyai-0.4.2/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 20:09:39.000000 assemblyai-0.4.2/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:09:39.404760 assemblyai-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 20:09:30.000000 assemblyai-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.400760 assemblyai-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:39.404760 assemblyai-0.4.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-31 20:09:30.000000 assemblyai-0.4.2/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.867332 assemblyai-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-02 10:53:30.000000 assemblyai-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 10:53:50.863332 assemblyai-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-06-02 10:53:30.000000 assemblyai-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45979 2023-06-02 10:53:30.000000 assemblyai-0.5.0/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 10:53:50.000000 assemblyai-0.5.0/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 10:53:50.867332 assemblyai-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-02 10:53:30.000000 assemblyai-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:50.863332 assemblyai-0.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-06-02 10:53:30.000000 assemblyai-0.5.0/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.4.2/LICENSE` & `assemblyai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/PKG-INFO` & `assemblyai-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.2
+Version: 0.5.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.2/README.md` & `assemblyai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/__init__.py` & `assemblyai-0.5.0/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/api.py` & `assemblyai-0.5.0/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/client.py` & `assemblyai-0.5.0/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/lemur.py` & `assemblyai-0.5.0/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/transcriber.py` & `assemblyai-0.5.0/assemblyai/transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/assemblyai/types.py` & `assemblyai-0.5.0/assemblyai/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -332,14 +332,17 @@
     "The list of PII Redaction policies to enable."
     redact_pii_sub: Optional[PIISubstitutionPolicy]
     "The replacement logic for detected PII."
 
     speaker_labels: Optional[bool]
     "Enable Speaker Diarization."
 
+    speakers_expected: Optional[int]
+    "The number of speakers you expect to be in your audio file."
+
     # content_safety: bool = False
     # "Enable Content Safety Detection."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
     custom_spelling: Optional[List[Dict[str, List[str]]]]
@@ -402,14 +405,15 @@
         boost_param: Optional[WordBoost] = None,
         filter_profanity: Optional[bool] = None,
         redact_pii: Optional[bool] = None,
         redact_pii_audio: Optional[bool] = None,
         redact_pii_policies: Optional[PIIRedactionPolicy] = None,
         redact_pii_sub: Optional[PIISubstitutionPolicy] = None,
         speaker_labels: Optional[bool] = None,
+        speakers_expected: Optional[int] = None,
         # content_safety: bool = False,
         # iab_categories: bool = False,
         custom_spelling: Optional[Dict[str, Union[str, Sequence[str]]]] = None,
         disfluencies: Optional[bool] = None,
         # sentiment_analysis: bool = False,
         # auto_chapters: bool = False,
         # entity_detection: bool = False,
@@ -435,14 +439,15 @@
             boost_param: The weight to apply to words/phrases in the word_boost array.
             filter_profanity: Filter profanity from the transcribed text.
             redact_pii: Redact PII from the transcribed text.
             redact_pii_audio: Generate a copy of the original media file with spoken PII 'beeped' out.
             redact_pii_policies: The list of PII Redaction policies to enable.
             redact_pii_sub: The replacement logic for detected PII.
             speaker_labels: Enable Speaker Diarization.
+            speakers_expected: The number of speakers you expect to hear in your audio file. Up to 10 speakers are supported.
             content_safety: Enable Content Safety Detection.
             iab_categories: Enable Topic Detection.
             custom_spelling: Customize how words are spelled and formatted using to and from values.
             disfluencies: Transcribe Filler Words, like 'umm', in your media file.
             sentiment_analysis: Enable Sentiment Analysis.
             auto_chapters: Enable Auto Chapters.
             entity_detection: Enable Entity Detection.
@@ -476,15 +481,15 @@
         self.filter_profanity = filter_profanity
         self.set_redact_pii(
             redact_pii,
             redact_pii_audio,
             redact_pii_policies,
             redact_pii_sub,
         )
-        self.speaker_labels = speaker_labels
+        self.set_speaker_diarization(speaker_labels, speakers_expected)
         # self.content_safety = content_safety
         # self.iab_categories = iab_categories
         self.set_custom_spelling(custom_spelling, override=True)
         self.disfluencies = disfluencies
         # self.sentiment_analysis = sentiment_analysis
         # self.auto_chapters = auto_chapters
         # self.entity_detection = entity_detection
@@ -629,19 +634,19 @@
 
     @property
     def speaker_labels(self) -> Optional[bool]:
         "Returns the status of the Speaker Diarization feature."
 
         return self._raw_transcription_config.speaker_labels
 
-    @speaker_labels.setter
-    def speaker_labels(self, enable: Optional[bool]) -> None:
-        "Enable Speaker Diarization feature."
+    @property
+    def speakers_expected(self) -> Optional[int]:
+        "Returns the number of speakers expected to be in the audio file. Used in combination with the `speaker_labels` parameter."
 
-        self._raw_transcription_config.speaker_labels = enable
+        return self._raw_transcription_config.speakers_expected
 
     # @property
     # def content_safety(self) -> bool:
     #     "Returns the status of the Content Safety feature."
 
     #     return self._raw_transcription_config.content_safety
 
@@ -795,14 +800,36 @@
             enable: Enable Automatic Punctuation and Text Formatting
         """
         self._raw_transcription_config.punctuate = enable
         self._raw_transcription_config.format_text = enable
 
         return self
 
+    def set_speaker_diarization(
+        self,
+        enable: bool = True,
+        speakers_expected: Optional[int] = None,
+    ) -> Self:
+        """
+        Whether to enable Speaker Diarization on the transcript.
+
+        Args:
+            `enable`: Enable Speaker Diarization
+            `speakers_expected`: The number of speakers in the audio file.
+        """
+
+        if not enable:
+            self._raw_transcription_config.speaker_labels = None
+            self._raw_transcription_config.speakers_expected = None
+        else:
+            self._raw_transcription_config.speaker_labels = True
+            self._raw_transcription_config.speakers_expected = speakers_expected
+
+        return self
+
     def set_webhook(
         self,
         url: Optional[str],
         auth_header_name: Optional[str] = None,
         auth_header_value: Optional[str] = None,
     ) -> Self:
         """
```

### Comparing `assemblyai-0.4.2/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.5.0/assemblyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.2
+Version: 0.5.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.2/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.5.0/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/setup.py` & `assemblyai-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.4.2",
+    version="0.5.0",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.4.2/tests/unit/factories.py` & `assemblyai-0.5.0/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/tests/unit/test_domains.py` & `assemblyai-0.5.0/tests/unit/test_domains.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         "set_custom_spelling",  # custom_spelling
         "raw",  # access to the underlying raw config
         "set_word_boost",  # word boost setter
         "set_casing_and_formatting",  # punctuation, formatting setter
         "set_redact_pii",  # PII redaction
         "set_summarize",  # summarization
         "set_webhook",  # webhook
+        "set_speaker_diarization",  # speaker diarization
     }
 
     # get all members
     non_raw_members = inspect.getmembers(aai.TranscriptionConfig)
 
     # just retrieve the names
     raw_member_names = set(aai.RawTranscriptionConfig.__fields__.keys())
```

### Comparing `assemblyai-0.4.2/tests/unit/test_lemur.py` & `assemblyai-0.5.0/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/tests/unit/test_transcriber.py` & `assemblyai-0.5.0/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.2/tests/unit/test_transcript.py` & `assemblyai-0.5.0/tests/unit/test_transcript.py`

 * *Files identical despite different names*

