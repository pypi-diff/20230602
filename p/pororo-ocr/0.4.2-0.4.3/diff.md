# Comparing `tmp/pororo_ocr-0.4.2-py3-none-any.whl.zip` & `tmp/pororo_ocr-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17095 bytes, number of entries: 7
--rw-r--r--  2.0 unx    11360 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    26965 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_library
--rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_model
--rw-r--r--  2.0 unx     8749 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 00:17 pororo_ocr-0.4.2.dist-info/RECORD
-7 files, 48750 bytes uncompressed, 15989 bytes compressed:  67.2%
+Zip file size: 17096 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    11360 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26965 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_library
+-rw-r--r--  2.0 unx      966 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_model
+-rw-r--r--  2.0 unx     8764 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      617 b- defN 23-Jun-02 00:27 pororo_ocr-0.4.3.dist-info/RECORD
+7 files, 48765 bytes uncompressed, 15990 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: pororo_ocr-0.4.2.dist-info/LICENSE
+Filename: pororo_ocr-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_library
+Filename: pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_library
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_model
+Filename: pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_model
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/METADATA
+Filename: pororo_ocr-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/WHEEL
+Filename: pororo_ocr-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/top_level.txt
+Filename: pororo_ocr-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pororo_ocr-0.4.2.dist-info/RECORD
+Filename: pororo_ocr-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pororo_ocr-0.4.2.dist-info/LICENSE` & `pororo_ocr-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_library` & `pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_library`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.2.dist-info/LICENSE.3rd_party_model` & `pororo_ocr-0.4.3.dist-info/LICENSE.3rd_party_model`

 * *Files identical despite different names*

## Comparing `pororo_ocr-0.4.2.dist-info/METADATA` & `pororo_ocr-0.4.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pororo-ocr
-Version: 0.4.2
+Version: 0.4.3
 Summary: Rebuilding only the OCR part of the pororo package for lightweight and fast operation.
 Home-page: https://github.com/stellarway/pororo-ocr
 Author: Wonhee Go
 Author-email: whgo.nlp@gmail.com
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -81,37 +81,37 @@
 
 ## Usage
 
 - `pororo` can be used as follows:
 - First, in order to import `pororo`, you must execute the following snippet
 
 ```python
->>> from pororo import Pororo
+>>> from pororoOCR import Pororo
 ```
 
 - After the import, you can check the tasks currently supported by the `pororo` through the following commands
 
 ```python
->>> from pororo import Pororo
+>>> from pororoOCR import Pororo
 >>> Pororo.available_tasks()
 "Available tasks are ['mrc', 'rc', 'qa', 'question_answering', 'machine_reading_comprehension', 'reading_comprehension', 'sentiment', 'sentiment_analysis', 'nli', 'natural_language_inference', 'inference', 'fill', 'fill_in_blank', 'fib', 'para', 'pi', 'cse', 'contextual_subword_embedding', 'similarity', 'sts', 'semantic_textual_similarity', 'sentence_similarity', 'sentvec', 'sentence_embedding', 'sentence_vector', 'se', 'inflection', 'morphological_inflection', 'g2p', 'grapheme_to_phoneme', 'grapheme_to_phoneme_conversion', 'w2v', 'wordvec', 'word2vec', 'word_vector', 'word_embedding', 'tokenize', 'tokenise', 'tokenization', 'tokenisation', 'tok', 'segmentation', 'seg', 'mt', 'machine_translation', 'translation', 'pos', 'tag', 'pos_tagging', 'tagging', 'const', 'constituency', 'constituency_parsing', 'cp', 'pg', 'collocation', 'collocate', 'col', 'word_translation', 'wt', 'summarization', 'summarisation', 'text_summarization', 'text_summarisation', 'summary', 'gec', 'review', 'review_scoring', 'lemmatization', 'lemmatisation', 'lemma', 'ner', 'named_entity_recognition', 'entity_recognition', 'zero-topic', 'dp', 'dep_parse', 'caption', 'captioning', 'asr', 'speech_recognition', 'st', 'speech_translation', 'ocr', 'srl', 'semantic_role_labeling', 'p2g', 'aes', 'essay', 'qg', 'question_generation', 'age_suitability']"
 ```
 
 - To check which models are supported by each task, you can go through the following process
 
 ```python
->>> from pororo import Pororo
+>>> from pororoOCR import Pororo
 >>> Pororo.available_models("collocation")
 'Available models for collocation are ([lang]: ko, [model]: kollocate), ([lang]: en, [model]: collocate.en), ([lang]: ja, [model]: collocate.ja), ([lang]: zh, [model]: collocate.zh)'
 ```
 
 - If you want to perform a specific task, you can put the task name in the `task` argument and the language name in the `lang` argument
 
 ```python
->>> from pororo import Pororo
+>>> from pororoOCR import Pororo
 >>> ner = Pororo(task="ner", lang="en")
 ```
 
 - After object construction, it can be used in a way that passes the input value as follows:
 
 ```python
 >>> ner("Michael Jeffrey Jordan (born February 17, 1963) is an American businessman and former professional basketball player.")
@@ -131,15 +131,15 @@
 >>> ner("麥可·傑佛瑞·喬丹是美國退役NBA職業籃球運動員，也是一名商人，現任夏洛特黃蜂董事長及主要股東")
 [('麥可·傑佛瑞·喬丹', 'PERSON'), ('是', 'O'), ('美國', 'GPE'), ('退', 'O'), ('役', 'O'), ('nba', 'ORG'), ('職', 'O'), ('業', 'O'), ('籃', 'O'), ('球', 'O'), ('運', 'O'), ('動', 'O'), ('員', 'O'), ('，', 'O'), ('也', 'O'), ('是', 'O'), ('一', 'O'), ('名', 'O'), ('商', 'O'), ('人', 'O'), ('，', 'O'), ('現', 'O'), ('任', 'O'), ('夏洛特黃蜂', 'ORG'), ('董', 'O'), ('事', 'O'), ('長', 'O'), ('及', 'O'), ('主', 'O'), ('要', 'O'), ('股', 'O'), ('東', 'O')]
 ```
 
 - If the task supports **multiple models**, you can change the `model` argument to use another model.
 
 ```python
->>> from pororo import Pororo
+>>> from pororoOCR import Pororo
 >>> mt = Pororo(task="mt", lang="multi", model="transformer.large.multi.mtpg")
 >>> fast_mt = Pororo(task="mt", lang="multi", model="transformer.large.multi.fast.mtpg")
 ```
 
 <br>
 
 ## Documentation
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pororo-ocr Version: 0.4.2 Summary: Rebuilding only
+Metadata-Version: 2.1 Name: pororo-ocr Version: 0.4.3 Summary: Rebuilding only
 the OCR part of the pororo package for lightweight and fast operation. Home-
 page: https://github.com/stellarway/pororo-ocr Author: Wonhee Go Author-email:
 whgo.nlp@gmail.com License: Apache-2.0 Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
@@ -26,19 +26,19 @@
 Recognition**, [_wav2letter_](https://github.com/facebookresearch/wav2letter)
 should be installed separately. For the installation, please run the [asr-
 install.sh](asr-install.sh) ```console bash asr-install.sh ``` - For the
 utilization of **Speech Synthesis**, please run the [tts-install.sh](tts-
 install.sh) ```console bash tts-install.sh ``` - **Speech Synthesis** samples
 can be found [here](https://pororo-tts.github.io/)
 ## Usage - `pororo` can be used as follows: - First, in order to import
-`pororo`, you must execute the following snippet ```python >>> from pororo
+`pororo`, you must execute the following snippet ```python >>> from pororoOCR
 import Pororo ``` - After the import, you can check the tasks currently
 supported by the `pororo` through the following commands ```python >>> from
-pororo import Pororo >>> Pororo.available_tasks() "Available tasks are ['mrc',
-'rc', 'qa', 'question_answering', 'machine_reading_comprehension',
+pororoOCR import Pororo >>> Pororo.available_tasks() "Available tasks are
+['mrc', 'rc', 'qa', 'question_answering', 'machine_reading_comprehension',
 'reading_comprehension', 'sentiment', 'sentiment_analysis', 'nli',
 'natural_language_inference', 'inference', 'fill', 'fill_in_blank', 'fib',
 'para', 'pi', 'cse', 'contextual_subword_embedding', 'similarity', 'sts',
 'semantic_textual_similarity', 'sentence_similarity', 'sentvec',
 'sentence_embedding', 'sentence_vector', 'se', 'inflection',
 'morphological_inflection', 'g2p', 'grapheme_to_phoneme',
 'grapheme_to_phoneme_conversion', 'w2v', 'wordvec', 'word2vec', 'word_vector',
@@ -50,20 +50,20 @@
 'text_summarization', 'text_summarisation', 'summary', 'gec', 'review',
 'review_scoring', 'lemmatization', 'lemmatisation', 'lemma', 'ner',
 'named_entity_recognition', 'entity_recognition', 'zero-topic', 'dp',
 'dep_parse', 'caption', 'captioning', 'asr', 'speech_recognition', 'st',
 'speech_translation', 'ocr', 'srl', 'semantic_role_labeling', 'p2g', 'aes',
 'essay', 'qg', 'question_generation', 'age_suitability']" ``` - To check which
 models are supported by each task, you can go through the following process
-```python >>> from pororo import Pororo >>> Pororo.available_models
+```python >>> from pororoOCR import Pororo >>> Pororo.available_models
 ("collocation") 'Available models for collocation are ([lang]: ko, [model]:
 kollocate), ([lang]: en, [model]: collocate.en), ([lang]: ja, [model]:
 collocate.ja), ([lang]: zh, [model]: collocate.zh)' ``` - If you want to
 perform a specific task, you can put the task name in the `task` argument and
-the language name in the `lang` argument ```python >>> from pororo import
+the language name in the `lang` argument ```python >>> from pororoOCR import
 Pororo >>> ner = Pororo(task="ner", lang="en") ``` - After object construction,
 it can be used in a way that passes the input value as follows: ```python >>>
 ner("Michael Jeffrey Jordan (born February 17, 1963) is an American businessman
 and former professional basketball player.") [('Michael Jeffrey Jordan',
 'PERSON'), ('(', 'O'), ('born', 'O'), ('February 17, 1963)', 'DATE'), ('is',
 'O'), ('an', 'O'), ('American', 'NORP'), ('businessman', 'O'), ('and', 'O'),
 ('former', 'O'), ('professional', 'O'), ('basketball', 'O'), ('player', 'O'),
@@ -87,15 +87,15 @@
 ('é', 'O'), ('å½¹', 'O'), ('nba', 'ORG'), ('è·', 'O'), ('æ¥­', 'O'), ('ç±',
 'O'), ('ç', 'O'), ('é', 'O'), ('å', 'O'), ('å¡', 'O'), ('ï¼', 'O'),
 ('ä¹', 'O'), ('æ¯', 'O'), ('ä¸', 'O'), ('å', 'O'), ('å', 'O'), ('äºº',
 'O'), ('ï¼', 'O'), ('ç¾', 'O'), ('ä»»', 'O'), ('å¤æ´ç¹é»è', 'ORG'),
 ('è£', 'O'), ('äº', 'O'), ('é·', 'O'), ('å', 'O'), ('ä¸»', 'O'), ('è¦',
 'O'), ('è¡', 'O'), ('æ±', 'O')] ``` - If the task supports **multiple
 models**, you can change the `model` argument to use another model. ```python
->>> from pororo import Pororo >>> mt = Pororo(task="mt", lang="multi",
+>>> from pororoOCR import Pororo >>> mt = Pororo(task="mt", lang="multi",
 model="transformer.large.multi.mtpg") >>> fast_mt = Pororo(task="mt",
 lang="multi", model="transformer.large.multi.fast.mtpg") ```
 ## Documentation For more detailed information, see [full documentation](https:
 //kakaobrain.github.io/pororo/) If you have any questions or requests, please
 report [the issue](https://github.com/kakaobrain/pororo/issues).
 ## Citation If you apply this library to any project and research, please cite
 our code: ``` @misc{pororo, author = {Heo, Hoon and Ko, Hyunwoong and Kim,
```

