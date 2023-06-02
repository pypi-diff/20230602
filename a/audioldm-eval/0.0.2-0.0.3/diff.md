# Comparing `tmp/audioldm_eval-0.0.2.tar.gz` & `tmp/audioldm_eval-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioldm_eval-0.0.2.tar", last modified: Wed May 17 14:26:16 2023, max compression
+gzip compressed data, was "audioldm_eval-0.0.3.tar", last modified: Fri Jun  2 00:35:07 2023, max compression
```

## Comparing `audioldm_eval-0.0.2.tar` & `audioldm_eval-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.749132 audioldm_eval-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1071 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4082 2023-05-17 14:26:16.746697 audioldm_eval-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3407 2023-05-17 14:25:05.000000 audioldm_eval-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.466554 audioldm_eval-0.0.2/audioldm_eval/
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.522530 audioldm_eval-0.0.2/audioldm_eval/audio/
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/audio_processing.py
--rw-r--r--   0 root         (0) root         (0)     6248 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/stft.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/audio/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.539919 audioldm_eval-0.0.2/audioldm_eval/datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6454 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/load_mel.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/datasets/transforms.py
--rw-r--r--   0 root         (0) root         (0)    14540 2023-05-17 14:23:15.000000 audioldm_eval-0.0.2/audioldm_eval/eval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.562019 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20706 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/inception3.py
--rw-r--r--   0 root         (0) root         (0)     4622 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception.py
--rw-r--r--   0 root         (0) root         (0)     5305 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception_audioset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.626678 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7940 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/config.py
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/finetune_template.py
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/losses.py
--rw-r--r--   0 root         (0) root         (0)    14159 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/main.py
--rw-r--r--   0 root         (0) root         (0)   128914 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/models.py
--rw-r--r--   0 root         (0) root         (0)     8592 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/pytorch_utils.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.672083 audioldm_eval-0.0.2/audioldm_eval/metrics/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9023 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/fad.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/fid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.742370 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/
--rw-r--r--   0 root         (0) root         (0)       72 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2087 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/geom_score.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/top_utils.py
--rw-r--r--   0 root         (0) root         (0)     4758 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/gs/utils.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/isc.py
--rw-r--r--   0 root         (0) root         (0)     3094 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/kid.py
--rw-r--r--   0 root         (0) root         (0)     6224 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/kl.py
--rw-r--r--   0 root         (0) root         (0)    13472 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/ndb.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-04-29 15:38:50.000000 audioldm_eval-0.0.2/audioldm_eval/metrics/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 14:26:16.498973 audioldm_eval-0.0.2/audioldm_eval.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4082 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1542 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 14:26:16.000000 audioldm_eval-0.0.2/audioldm_eval.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 14:26:16.748697 audioldm_eval-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4286 2023-05-17 14:25:38.000000 audioldm_eval-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.962151 audioldm_eval-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-06-02 00:35:07.959635 audioldm_eval-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.683205 audioldm_eval-0.0.3/audioldm_eval/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.742763 audioldm_eval-0.0.3/audioldm_eval/audio/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/audio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/audio/audio_processing.py
+-rw-r--r--   0 root         (0) root         (0)     6248 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/audio/stft.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/audio/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.761902 audioldm_eval-0.0.3/audioldm_eval/datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-06-02 00:23:51.000000 audioldm_eval-0.0.3/audioldm_eval/datasets/load_mel.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/datasets/transforms.py
+-rw-r--r--   0 root         (0) root         (0)    14540 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/eval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.790098 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20706 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/inception3.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/melception.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/melception_audioset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.863066 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7940 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/config.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     4234 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/finetune_template.py
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/losses.py
+-rw-r--r--   0 root         (0) root         (0)    14159 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/main.py
+-rw-r--r--   0 root         (0) root         (0)   128914 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/models.py
+-rw-r--r--   0 root         (0) root         (0)     8592 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/pytorch_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.921594 audioldm_eval-0.0.3/audioldm_eval/metrics/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2023-06-02 00:22:00.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/fad.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/fid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.953284 audioldm_eval-0.0.3/audioldm_eval/metrics/gs/
+-rw-r--r--   0 root         (0) root         (0)       72 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/gs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2087 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/gs/geom_score.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/gs/top_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/gs/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/isc.py
+-rw-r--r--   0 root         (0) root         (0)     3094 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/kid.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/kl.py
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/ndb.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-02 00:18:11.000000 audioldm_eval-0.0.3/audioldm_eval/metrics/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 00:35:07.715958 audioldm_eval-0.0.3/audioldm_eval.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-06-02 00:35:07.000000 audioldm_eval-0.0.3/audioldm_eval.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-06-02 00:35:07.000000 audioldm_eval-0.0.3/audioldm_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 00:35:07.000000 audioldm_eval-0.0.3/audioldm_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-06-02 00:35:07.000000 audioldm_eval-0.0.3/audioldm_eval.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-02 00:35:07.000000 audioldm_eval-0.0.3/audioldm_eval.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 00:35:07.961634 audioldm_eval-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-06-02 00:24:37.000000 audioldm_eval-0.0.3/setup.py
```

### Comparing `audioldm_eval-0.0.2/LICENSE` & `audioldm_eval-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/PKG-INFO` & `audioldm_eval-0.0.3/audioldm_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: audioldm_eval
-Version: 0.0.2
+Name: audioldm-eval
+Version: 0.0.3
 Summary: This package is written for the evaluation of audio generation model.
 Home-page: https://github.com/haoheliu/audioldm_eval
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audioldm_eval-0.0.2/README.md` & `audioldm_eval-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/audio/audio_processing.py` & `audioldm_eval-0.0.3/audioldm_eval/audio/audio_processing.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/audio/stft.py` & `audioldm_eval-0.0.3/audioldm_eval/audio/stft.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/audio/tools.py` & `audioldm_eval-0.0.3/audioldm_eval/audio/tools.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/datasets/load_mel.py` & `audioldm_eval-0.0.3/audioldm_eval/datasets/load_mel.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,19 +155,21 @@
 
     def read_from_file(self, audio_file):
         audio, file_sr = torchaudio.load(audio_file)
         # Only use the first channel
         audio = audio[0:1,...]
         audio = audio - audio.mean()
 
-        if file_sr != self.sr and file_sr == 32000 and self.sr == 16000:
-            audio = audio[..., ::2]
-        if file_sr != self.sr and file_sr == 48000 and self.sr == 16000:
-            audio = audio[..., ::3]
-        elif file_sr != self.sr:
+        # if file_sr != self.sr and file_sr == 32000 and self.sr == 16000:
+        #     audio = audio[..., ::2]
+        # if file_sr != self.sr and file_sr == 48000 and self.sr == 16000:
+        #     audio = audio[..., ::3]
+        # el
+        
+        if file_sr != self.sr:
             audio = torchaudio.functional.resample(
                 audio, orig_freq=file_sr, new_freq=self.sr
             )
         audio = pad_short_audio(audio, min_samples=32000)
         return audio
```

### Comparing `audioldm_eval-0.0.2/audioldm_eval/datasets/transforms.py` & `audioldm_eval-0.0.3/audioldm_eval/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/eval.py` & `audioldm_eval-0.0.3/audioldm_eval/eval.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/inception3.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/inception3.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/melception.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/melception_audioset.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/melception_audioset.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/config.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/config.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/evaluate.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/evaluate.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/finetune_template.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/finetune_template.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/main.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/main.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/models.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/models.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/pytorch_utils.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/feature_extractors/panns/utilities.py` & `audioldm_eval-0.0.3/audioldm_eval/feature_extractors/panns/utilities.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/fad.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/fad.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,21 @@
     wav_data = wav_data / 32768.0  # Convert to [-1.0, +1.0]
 
     # Convert to mono
     if len(wav_data.shape) > 1:
         wav_data = np.mean(wav_data, axis=1)
 
     if sr != SAMPLE_RATE:
-        if SAMPLE_RATE == 16000 and sr == 32000:
-            wav_data = wav_data[::2]
-        else:
-            wav_data = resampy.resample(wav_data, sr, SAMPLE_RATE)
+        # if SAMPLE_RATE == 16000 and sr == 32000:
+        #     wav_data = wav_data[::2]
+        # else:
+        wav_data = resampy.resample(wav_data, sr, SAMPLE_RATE) # TODO try out different kinds of sampling rate here
 
     return wav_data, SAMPLE_RATE
 
-
 class FrechetAudioDistance:
     def __init__(
         self, use_pca=False, use_activation=False, verbose=False, audio_load_worker=8
     ):
         self.__get_model(use_pca=use_pca, use_activation=use_activation)
         self.verbose = verbose
         self.audio_load_worker = audio_load_worker
```

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/fid.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/fid.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/geom_score.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/gs/geom_score.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/top_utils.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/gs/top_utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/gs/utils.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/gs/utils.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/isc.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/isc.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/kid.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/kid.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/kl.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/kl.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/ndb.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/ndb.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval/metrics/validate.py` & `audioldm_eval-0.0.3/audioldm_eval/metrics/validate.py`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/audioldm_eval.egg-info/PKG-INFO` & `audioldm_eval-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: audioldm-eval
-Version: 0.0.2
+Name: audioldm_eval
+Version: 0.0.3
 Summary: This package is written for the evaluation of audio generation model.
 Home-page: https://github.com/haoheliu/audioldm_eval
 Author: Haohe Liu
 Author-email: haoheliu@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `audioldm_eval-0.0.2/audioldm_eval.egg-info/SOURCES.txt` & `audioldm_eval-0.0.3/audioldm_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audioldm_eval-0.0.2/setup.py` & `audioldm_eval-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # Package meta-data.
 NAME = "audioldm_eval"
 DESCRIPTION = "This package is written for the evaluation of audio generation model."
 URL = "https://github.com/haoheliu/audioldm_eval"
 EMAIL = "haoheliu@gmail.com"
 AUTHOR = "Haohe Liu"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "torch>=1.11.0",
     "torchaudio",
     "scikit-image",
     "torchlibrosa",
```

