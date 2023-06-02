# Comparing `tmp/easymms-0.1.4.tar.gz` & `tmp/easymms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.4.tar", last modified: Tue May 30 05:45:07 2023, max compression
+gzip compressed data, was "easymms-0.1.5.tar", last modified: Fri Jun  2 00:34:21 2023, max compression
```

## Comparing `easymms-0.1.4.tar` & `easymms-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.891826 easymms-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-30 05:44:59.000000 easymms-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-30 05:45:07.891826 easymms-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-30 05:44:59.000000 easymms-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/easymms/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/models/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-30 05:44:59.000000 easymms-0.1.4/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.891826 easymms-0.1.4/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 05:45:07.000000 easymms-0.1.4/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:45:07.891826 easymms-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 05:44:59.000000 easymms-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:45:07.887826 easymms-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 05:44:59.000000 easymms-0.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-30 05:44:59.000000 easymms-0.1.4/tests/test_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.154697 easymms-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-06-02 00:34:12.000000 easymms-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 00:34:21.150696 easymms-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-02 00:34:12.000000 easymms-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/models/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-02 00:34:12.000000 easymms-0.1.5/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:34:20.000000 easymms-0.1.5/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 00:34:21.000000 easymms-0.1.5/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:34:21.154697 easymms-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-02 00:34:12.000000 easymms-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:21.150696 easymms-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/test_asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 00:34:12.000000 easymms-0.1.5/tests/test_tts.py
```

### Comparing `easymms-0.1.4/LICENSE` & `easymms-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.4/PKG-INFO` & `easymms-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.4
+Version: 0.1.5
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
@@ -33,38 +33,41 @@
 * [API reference](#api-reference)
 * [License](#license)
 * [Disclaimer & Credits](#disclaimer--credits)
 <!-- TOC -->
 # Installation
 
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
+2. Install `easymms` from Pypi
+```bash
+pip install easymms
+```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
-2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
+3. If you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
 pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
-3. Install `easymms` from Pypi
-```bash
-pip install easymms
-```
-or from source 
-```bash
-pip install git+https://github.com/abdeladim-s/easymms
-```
+
 4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
 ```shell
 pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
 ```
 
 # Quickstart
+:warning: There is an [issue](https://github.com/abdeladim-s/easymms/issues/3) with `fairseq` when running the code in interactive environments like Jupyter notebooks.<br/>
+**Please use normal Python files** or use the colab notebook provided above. 
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
 
 
 ```python
 from easymms.models.asr import ASRModel
@@ -103,15 +106,21 @@
                                    lang='eng')
 for transcription in transcriptions:
     for segment in transcription:
         print(f"{segment['start_time']} -> {segment['end_time']}: {segment['text']}")
 ```
 
 ## TTS
-Coming Soon
+```python 
+from easymms.models.tts import TTSModel
+
+tts = TTSModel('eng')
+res = tts.synthesize("This is a simple example")
+tts.save(res)
+```
 
 ## LID 
 Coming Soon
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/easymms/) for more details.
```

### Comparing `easymms-0.1.4/README.md` & `easymms-0.1.5/easymms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: easymms
+Version: 0.1.5
+Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
+Author: Abdeladim Sadiki
+License: MIT
+Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
+Project-URL: Source, https://abdeladim-s.github.io/easymms/
+Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
 [![wheels](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml/badge.svg)](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml)
 <a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
@@ -20,38 +33,41 @@
 * [API reference](#api-reference)
 * [License](#license)
 * [Disclaimer & Credits](#disclaimer--credits)
 <!-- TOC -->
 # Installation
 
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
+2. Install `easymms` from Pypi
+```bash
+pip install easymms
+```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
-2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
+3. If you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
 pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
-3. Install `easymms` from Pypi
-```bash
-pip install easymms
-```
-or from source 
-```bash
-pip install git+https://github.com/abdeladim-s/easymms
-```
+
 4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
 ```shell
 pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
 ```
 
 # Quickstart
+:warning: There is an [issue](https://github.com/abdeladim-s/easymms/issues/3) with `fairseq` when running the code in interactive environments like Jupyter notebooks.<br/>
+**Please use normal Python files** or use the colab notebook provided above. 
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
 
 
 ```python
 from easymms.models.asr import ASRModel
@@ -90,15 +106,21 @@
                                    lang='eng')
 for transcription in transcriptions:
     for segment in transcription:
         print(f"{segment['start_time']} -> {segment['end_time']}: {segment['text']}")
 ```
 
 ## TTS
-Coming Soon
+```python 
+from easymms.models.tts import TTSModel
+
+tts = TTSModel('eng')
+res = tts.synthesize("This is a simple example")
+tts.save(res)
+```
 
 ## LID 
 Coming Soon
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/easymms/) for more details.
```

### Comparing `easymms-0.1.4/easymms/_logger.py` & `easymms-0.1.5/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.4/easymms/constants.py` & `easymms-0.1.5/easymms/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,26 @@
 import logging
 from pathlib import Path
 
 import numpy as np
 from platformdirs import *
 
 PACKAGE_NAME = 'easymms'
+LOGGING_LEVEL = logging.INFO
+
 PACKAGE_DATA_DIR = user_data_dir(PACKAGE_NAME)
 
-LOGGING_LEVEL = logging.INFO
+
+TTS_DIR = (Path(PACKAGE_DATA_DIR) / 'tts').resolve()
+TTS_MODELS_BASE_URL = "https://dl.fbaipublicfiles.com/mms/tts/"  # lang.tar.gz
+VITS_URL = "https://github.com/jaywalnut310/vits"
+VITS_DIR = TTS_DIR / 'vits'
+
+FAIRSEQ_URL = "https://github.com/facebookresearch/fairseq"
+FAIRSEQ_DIR = Path(PACKAGE_DATA_DIR) / 'fairseq'
 
 CFG = {
   '_name': None,
   'task': {
     '_name': 'audio_finetuning',
     'data': '',
     'labels': 'ltr'
@@ -193,11 +202,11 @@
 }
 
 HYPO_WORDS_FILE = 'hypo.word'
 
 ALIGNMENT_MODEL_URL = "https://dl.fbaipublicfiles.com/mms/torchaudio/ctc_alignment_mling_uroman/model.pt"
 ALIGNMENT_DICTIONARY_URL = "https://dl.fbaipublicfiles.com/mms/torchaudio/ctc_alignment_mling_uroman/dictionary.txt"
 
-UROMAN_URL = "https://github.com/isi-nlp/uroman/archive/refs/tags/v1.2.8.zip"
-UROMAN_DIR_NAME = 'uroman-1.2.8'
+UROMAN_URL = "https://github.com/isi-nlp/uroman"
+UROMAN_DIR = Path(PACKAGE_DATA_DIR) / 'uroman'
 
 MMS_LANGS_FILE = (Path(__file__).parent / 'data' / 'mms_langs.json').resolve()
```

### Comparing `easymms-0.1.4/easymms/models/alignment.py` & `easymms-0.1.5/easymms/models/alignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,29 @@
 import logging
 import shutil
 import sys
 from pathlib import Path
 from typing import List
 import torch
 # fix importing from fairseq.examples
+import site
+sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
 try:
     from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
     from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
     from fairseq.examples.mms.data_prep.text_normalization import text_normalize
 except ImportError:
-    try:
-        from examples.mms.data_prep.align_and_segment import get_alignments
-        from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
-        from examples.mms.data_prep.text_normalization import text_normalize
-    except ImportError:
-        import fairseq
-        sys.path.append(str(Path(fairseq.__file__).parent))
-        from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
-        from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
-        from fairseq.examples.mms.data_prep.text_normalization import text_normalize
+    from examples.mms.data_prep.align_and_segment import get_alignments
+    from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+    from examples.mms.data_prep.text_normalization import text_normalize
 
 from easymms import utils
 from easymms._logger import set_log_level
 from easymms.constants import PACKAGE_DATA_DIR, ALIGNMENT_MODEL_URL, ALIGNMENT_DICTIONARY_URL, UROMAN_URL, \
-    UROMAN_DIR_NAME
+    UROMAN_DIR
 
 
 
 from torchaudio.models import wav2vec2_model
 
 logger = logging.getLogger(__name__)
 
@@ -66,38 +61,28 @@
         set_log_level(log_level)
         assert shutil.which("perl") is not None, "To use the alignment algorithm you will need uroman " \
                                                  "<https://github.com/isi-nlp/uroman> which is written in perl " \
                                                  "please install perl first <https://www.perl.org/get.html>"
         if uroman_dir is not None:
             self.uroman_dir_path = Path(uroman_dir)
         else:
-            self._get_uroman()
+            self.uroman_dir_path = utils.get_uroman()
 
         if model is not None:
             self.model_path = Path(model)
         else:
             self.model_path = Path(PACKAGE_DATA_DIR) / "ctc_alignment_mling_uroman_model.pt"
 
         if dictionary is not None:
             self.dictionary_path = Path(dictionary)
         else:
             self.dictionary_path = Path(PACKAGE_DATA_DIR) / "ctc_alignment_mling_uroman_model.dict"
 
         self.model, self.dictionary = self._load_model_dict()
 
-    def _get_uroman(self):
-        logger.info("Searching uroman ...")
-        uroman_dir_path = Path(PACKAGE_DATA_DIR) / 'uroman' / UROMAN_DIR_NAME
-        if uroman_dir_path.exists():
-            logger.info(f"uroman exists at {uroman_dir_path}")
-        else:
-            logger.info(f"Downloading uroman from {UROMAN_URL} ...")
-            utils.download_and_unzip(UROMAN_URL, str(uroman_dir_path.parent.resolve()))
-        self.uroman_dir_path = uroman_dir_path / 'bin'
-
     def _load_model_dict(self):
         """
         Modified from <https://github.com/facebookresearch/fairseq/blob/main/examples/mms/data_prep/align_utils.py>
         to store the models in a consistent directory
 
         :return: None
         """
```

### Comparing `easymms-0.1.4/easymms/models/asr.py` & `easymms-0.1.5/easymms/models/asr.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 """
 This file contains a class definition to use the ASR models from [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms)
 """
 
 __author__ = "Abdeladim S."
 __copyright__ = "Copyright 2023,"
 
+
 import atexit
 import json
+import re
 import sys
 import tempfile
 import logging
 from pathlib import Path
 from typing import Union, List
-
 import torch
 from omegaconf import OmegaConf
 from pydub import AudioSegment
 from pydub.utils import mediainfo
 
 # fix importing from fairseq.examples
+import site
+sys.path.append(str(Path(site.getsitepackages()[0]) / 'fairseq'))
 try:
     from fairseq.examples.speech_recognition.new.infer import hydra_main
 except ImportError:
-    try:
-        from examples.speech_recognition.new.infer import hydra_main
-    except ImportError:
-        import fairseq
-        sys.path.append(str(Path(fairseq.__file__).parent))
-        from fairseq.examples.speech_recognition.new.infer import hydra_main
+    from examples.speech_recognition.new.infer import hydra_main
+
 
 from easymms import utils
 from easymms._logger import set_log_level
 from easymms.models.alignment import AlignmentModel
 from easymms.constants import CFG, HYPO_WORDS_FILE, MMS_LANGS_FILE
 
 logger = logging.getLogger(__name__)
@@ -125,15 +124,15 @@
                 res.append((str(save_file_at.resolve()), int(ds)))
         return res
 
     def transcribe(self,
                    media_files: List[str],
                    lang: str = 'eng',
                    device: str = None,
-                   align: bool = True,
+                   align: bool = False,
                    timestamps_type: str = 'segment',
                    max_segment_len: int = 27,
                    cfg: dict = None) -> Union[List[str], List[dict]]:
         """
         Transcribes a list of media files provided as inputs
 
         :param media_files: list of media files (video/audio), in whichever format supported by ffmpeg
@@ -159,25 +158,24 @@
                     device = 'cpu'
             if device == 'cuda':
                 pass  # default
             elif device == 'cpu':
                 self.cfg['common']['cpu'] = True
             if device == 'tpu':
                 self.cfg['common']['tpu'] = True
-            else:
-                logging.warning(f'Unknown device option {device}, Use one of (cuda, cpu, tpu)')
             cfg = OmegaConf.structured(self.cfg)
 
         self.wer = hydra_main(cfg)
         # get results: will just read from hypo.word as I don't want to change fairseq repo to get the hypo array
         hypo_file = self.tmp_dir_path / HYPO_WORDS_FILE
         res = []
         with open(hypo_file) as hw:
-            transcripts = [line.strip()[:-9] for line in hw.readlines()]
-            transcripts.reverse()
+            hypos = hw.readlines()
+            outputs = self._reorder_decode(hypos)
+            transcripts = [line[1].strip() for line in outputs]
         if align:
             align_model = AlignmentModel()
             for i in range(len(transcripts)):
                 media_file = processed_files[i][0]
                 transcript = utils.get_transcript_segments(transcripts[i], timestamps_type, max_segment_len=max_segment_len)
                 segments = align_model.align(media_file=media_file,
                                              transcript=transcript,
@@ -195,7 +193,23 @@
         Source <https://dl.fbaipublicfiles.com/mms/misc/language_coverage_mms.html>
         :return: list of supported languages
         """
         with open(MMS_LANGS_FILE) as f:
             data = json.load(f)
             return [key for key in data if data[key]['ASR']]
 
+    @staticmethod
+    def _reorder_decode(hypos):
+        """
+        Helper method to reorder the `hypos`, see @bekarys0504 comment in
+        [#5](https://github.com/abdeladim-s/easymms/issues/5)
+
+        :param hypos: hypos list
+        :return: ordered hypos
+        """
+        outputs = []
+        for hypo in hypos:
+            idx = int(re.findall("\(None-(\d+)\)$", hypo)[0])
+            hypo = re.sub("\(\S+\)$", "", hypo).strip()
+            outputs.append((idx, hypo))
+        outputs = sorted(outputs)
+        return outputs
```

### Comparing `easymms-0.1.4/easymms.egg-info/PKG-INFO` & `easymms-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: easymms
-Version: 0.1.4
-Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
-Author: Abdeladim Sadiki
-License: MIT
-Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
-Project-URL: Source, https://abdeladim-s.github.io/easymms/
-Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # EasyMMS
 
 A simple Python package to easily use [Meta's Massively Multilingual Speech (MMS) project](https://github.com/facebookresearch/fairseq/tree/main/examples/mms). 
 
 [![PyPi version](https://badgen.net/pypi/v/easymms)](https://pypi.org/project/easymms/)
 [![wheels](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml/badge.svg)](https://github.com/abdeladim-s/easymms/actions/workflows/wheels.yml)
 <a target="_blank" href="https://colab.research.google.com/github/abdeladim-s/easymms/blob/main/examples/EasyMMS.ipynb">
@@ -33,38 +20,41 @@
 * [API reference](#api-reference)
 * [License](#license)
 * [Disclaimer & Credits](#disclaimer--credits)
 <!-- TOC -->
 # Installation
 
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
+2. Install `easymms` from Pypi
+```bash
+pip install easymms
+```
+or from source 
+```bash
+pip install git+https://github.com/abdeladim-s/easymms
+```
 
-2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
+3. If you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
 pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
-3. Install `easymms` from Pypi
-```bash
-pip install easymms
-```
-or from source 
-```bash
-pip install git+https://github.com/abdeladim-s/easymms
-```
+
 4. `Fairseq` has not included the `MMS` project yet in the released PYPI version, so until the next release, you will need to install `fairseq` from source:
 ```shell
 pip uninstall fairseq && pip install git+https://github.com/facebookresearch/fairseq
 ```
 
 # Quickstart
+:warning: There is an [issue](https://github.com/abdeladim-s/easymms/issues/3) with `fairseq` when running the code in interactive environments like Jupyter notebooks.<br/>
+**Please use normal Python files** or use the colab notebook provided above. 
 
 ## ASR 
 You will need first to download the model weights, you can find and download all the supported models from [here](https://github.com/facebookresearch/fairseq/tree/main/examples/mms#asr).
 
 
 ```python
 from easymms.models.asr import ASRModel
@@ -103,15 +93,21 @@
                                    lang='eng')
 for transcription in transcriptions:
     for segment in transcription:
         print(f"{segment['start_time']} -> {segment['end_time']}: {segment['text']}")
 ```
 
 ## TTS
-Coming Soon
+```python 
+from easymms.models.tts import TTSModel
+
+tts = TTSModel('eng')
+res = tts.synthesize("This is a simple example")
+tts.save(res)
+```
 
 ## LID 
 Coming Soon
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/easymms/) for more details.
```

### Comparing `easymms-0.1.4/setup.py` & `easymms-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.4",
+    version="0.1.5",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
@@ -22,9 +22,19 @@
     long_description_content_type="text/markdown",
     license='MIT',
     project_urls={
         'Documentation': 'https://abdeladim-s.github.io/easymms/',
         'Source': 'https://abdeladim-s.github.io/easymms/',
         'Tracker': 'https://abdeladim-s.github.io/easymms/issues',
     },
-    install_requires=["fairseq~=0.12.2", "pydub~=0.25.1", "platformdirs==3.5.1", "editdistance", "sox", "dataclasses", "soundfile"],
+    install_requires=["fairseq~=0.12.2",
+                      "pydub~=0.25.1",
+                      "platformdirs==3.5.1",
+                      "editdistance",
+                      "sox",
+                      "dataclasses",
+                      "soundfile",
+                      "GitPython",
+                      "Unidecode==1.1.1",
+                      "phonemizer==2.2.1",
+                      "librosa==0.8.0"],
 )
```

### Comparing `easymms-0.1.4/tests/test_asr.py` & `easymms-0.1.5/tests/test_asr.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class TestASR(TestCase):
     asr = ASRModel('../models_dir/mms1b_fl102.pt')
     eng_files = ['../assets/eng_1.mp3', '../assets/eng_2.flac']
     ara_files = ['../assets/ara_1.ogg']
 
     def test_transcribe_eng(self):
-        res = self.asr.transcribe(self.eng_files, align=True, lang='eng')
+        res = self.asr.transcribe(self.eng_files, align=False, lang='eng')
         self.assertIsNotNone(res)
         self.assertIsInstance(res, list)
         self.assertEqual(len(self.eng_files), len(res))
 
     def test_transcribe_ara(self):
         """
         Just to try testing with another lang other than `eng`
```

