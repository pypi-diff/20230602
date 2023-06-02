# Comparing `tmp/spacy_huggingface_pipelines-0.0.3.tar.gz` & `tmp/spacy_huggingface_pipelines-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy_huggingface_pipelines-0.0.3.tar", last modified: Thu May  4 15:26:45 2023, max compression
+gzip compressed data, was "spacy_huggingface_pipelines-0.0.4.tar", last modified: Fri Jun  2 18:10:12 2023, max compression
```

## Comparing `spacy_huggingface_pipelines-0.0.3.tar` & `spacy_huggingface_pipelines-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     8455 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1766 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.276632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.280632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/enable_gpu.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3028 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/test_pipeline_components.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3701 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/text_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6764 2023-05-04 15:26:29.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/token_classification.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-04 15:26:45.276632 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     9718 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-05-04 15:26:45.000000 spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-02 18:10:12.258628 spacy_huggingface_pipelines-0.0.4/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     9850 2023-06-02 18:10:12.258628 spacy_huggingface_pipelines-0.0.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     8587 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       88 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1766 2023-06-02 18:10:12.262628 spacy_huggingface_pipelines-0.0.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      171 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-02 18:10:12.258628 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)      143 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-02 18:10:12.258628 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/tests/enable_gpu.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3222 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/tests/test_pipeline_components.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3701 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/text_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6892 2023-06-02 18:10:01.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/token_classification.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-02 18:10:12.258628 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9850 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      720 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)       61 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       28 2023-06-02 18:10:12.000000 spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/top_level.txt
```

### Comparing `spacy_huggingface_pipelines-0.0.3/LICENSE` & `spacy_huggingface_pipelines-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.3/PKG-INFO` & `spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spacy_huggingface_pipelines
-Version: 0.0.3
+Name: spacy-huggingface-pipelines
+Version: 0.0.4
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
 Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
 Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
@@ -141,15 +141,16 @@
 nlp = spacy.blank("en")
 nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-base-NER"})
 doc = nlp("My name is Sarah and I live in London")
 print(doc.ents)
 # (Sarah, London)
 ```
 
-2. Save named entity annotation as `Doc.spans[spans_key]`:
+2. Save named entity annotation as `Doc.spans[spans_key]` and scores as
+   `Doc.spans[spans_key].attrs["scores"]`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "hf_token_pipe",
     config={
@@ -157,14 +158,16 @@
         "annotate": "spans",
         "annotate_spans_key": "bert-base-ner",
     },
 )
 doc = nlp("My name is Sarah and I live in London")
 print(doc.spans["bert-base-ner"])
 # [Sarah, London]
+print(doc.spans["bert-base-ner"].attrs["scores"])
+# [0.99854773, 0.9996215]
 ```
 
 3. Save fine-grained tags as `Token.tag`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.4 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
 github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
 email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
 https://github.com/explosion/spacy-huggingface-pipelines Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
@@ -76,47 +76,48 @@
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
 annotation is saved to the spaCy doc. You can save the output as `token.tag_`,
 `token.pos_` (only for UPOS tags), `doc.ents` or `doc.spans`. #### Examples 1.
 Save named entity annotation as `Doc.ents`: ```python import spacy nlp =
 spacy.blank("en") nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-
 base-NER"}) doc = nlp("My name is Sarah and I live in London") print(doc.ents)
-# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans
-[spans_key]`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "hf_token_pipe", config={ "model": "dslim/bert-base-NER", "annotate":
-"spans", "annotate_spans_key": "bert-base-ner", }, ) doc = nlp("My name is
-Sarah and I live in London") print(doc.spans["bert-base-ner"]) # [Sarah,
-London] ``` 3. Save fine-grained tags as `Token.tag`: ```python import spacy
-nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model": "QCRI/
-bert-base-multilingual-cased-pos-english", "annotate": "tag", }, ) doc = nlp
-("My name is Sarah and I live in London") print([t.tag_ for t in doc]) #
-['PRP$', 'NN', 'VBZ', 'NNP', 'CC', 'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save
-coarse-grained tags as `Token.pos`: ```python import spacy nlp = spacy.blank
-("en") nlp.add_pipe( "hf_token_pipe", config={"model": "vblagoje/bert-english-
-uncased-finetuned-pos", "annotate": "pos"}, ) doc = nlp("My name is Sarah and I
-live in London") print([t.pos_ for t in doc]) # ['PRON', 'NOUN', 'AUX',
-'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP', 'PROPN'] ``` ### Text classification
-Config settings for `hf_text_pipe`: ```ini [components.hf_text_pipe] factory =
-"hf_text_pipe" model = "distilbert-base-uncased-finetuned-sst-2-english" #
-Model name or path revision = "main" # Model revision kwargs = {} # Any
-additional arguments for # TextClassificationPipeline scorer = null # Optional
-scorer ``` The input texts are truncated according to the transformers model
-max length. #### `TextClassificationPipeline` settings - `model`: The model
-name or path. - `revision`: The model revision. For production use, a specific
-git commit is recommended instead of the default `main`. - `kwargs`: Any
-additional arguments to [`TextClassificationPipeline`](https://huggingface.co/
-docs/transformers/main_classes/
-pipelines#transformers.TextClassificationPipeline). #### Example ```python
-import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
-{"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
-is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
-0.00013048505934420973} ``` ### Batching and GPU Both token and text
-classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` If the component runs into an
-error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
-processing each text individually. If it runs into an error on an individual
-text, a warning is shown and the doc is returned without additional annotation.
-Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
-(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
-the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
-new thread on the [discussion board](https://github.com/explosion/spaCy/
-discussions) for other issues.
+# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans[spans_key]`
+and scores as `Doc.spans[spans_key].attrs["scores"]`: ```python import spacy
+nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model":
+"dslim/bert-base-NER", "annotate": "spans", "annotate_spans_key": "bert-base-
+ner", }, ) doc = nlp("My name is Sarah and I live in London") print(doc.spans
+["bert-base-ner"]) # [Sarah, London] print(doc.spans["bert-base-ner"].attrs
+["scores"]) # [0.99854773, 0.9996215] ``` 3. Save fine-grained tags as
+`Token.tag`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
+( "hf_token_pipe", config={ "model": "QCRI/bert-base-multilingual-cased-pos-
+english", "annotate": "tag", }, ) doc = nlp("My name is Sarah and I live in
+London") print([t.tag_ for t in doc]) # ['PRP$', 'NN', 'VBZ', 'NNP', 'CC',
+'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save coarse-grained tags as `Token.pos`:
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe",
+config={"model": "vblagoje/bert-english-uncased-finetuned-pos", "annotate":
+"pos"}, ) doc = nlp("My name is Sarah and I live in London") print([t.pos_ for
+t in doc]) # ['PRON', 'NOUN', 'AUX', 'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP',
+'PROPN'] ``` ### Text classification Config settings for `hf_text_pipe`: ```ini
+[components.hf_text_pipe] factory = "hf_text_pipe" model = "distilbert-base-
+uncased-finetuned-sst-2-english" # Model name or path revision = "main" # Model
+revision kwargs = {} # Any additional arguments for #
+TextClassificationPipeline scorer = null # Optional scorer ``` The input texts
+are truncated according to the transformers model max length. ####
+`TextClassificationPipeline` settings - `model`: The model name or path. -
+`revision`: The model revision. For production use, a specific git commit is
+recommended instead of the default `main`. - `kwargs`: Any additional arguments
+to [`TextClassificationPipeline`](https://huggingface.co/docs/transformers/
+main_classes/pipelines#transformers.TextClassificationPipeline). #### Example
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe",
+config={"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc =
+nlp("This is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419,
+'NEGATIVE': 0.00013048505934420973} ``` ### Batching and GPU Both token and
+text classification support batching with `nlp.pipe`: ```python for doc in
+nlp.pipe(texts, batch_size=256): do_something(doc) ``` If the component runs
+into an error processing a batch (e.g. on an empty text), `nlp.pipe` will back
+off to processing each text individually. If it runs into an error on an
+individual text, a warning is shown and the doc is returned without additional
+annotation. Switch to GPU: ```python import spacy spacy.require_gpu() for doc
+in nlp.pipe(texts): do_something(doc) ``` ## Bug reports and issues Please
+report bugs in the [spaCy issue tracker](https://github.com/explosion/spaCy/
+issues) or open a new thread on the [discussion board](https://github.com/
+explosion/spaCy/discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.3/README.md` & `spacy_huggingface_pipelines-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,16 @@
 nlp = spacy.blank("en")
 nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-base-NER"})
 doc = nlp("My name is Sarah and I live in London")
 print(doc.ents)
 # (Sarah, London)
 ```
 
-2. Save named entity annotation as `Doc.spans[spans_key]`:
+2. Save named entity annotation as `Doc.spans[spans_key]` and scores as
+   `Doc.spans[spans_key].attrs["scores"]`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "hf_token_pipe",
     config={
@@ -128,14 +129,16 @@
         "annotate": "spans",
         "annotate_spans_key": "bert-base-ner",
     },
 )
 doc = nlp("My name is Sarah and I live in London")
 print(doc.spans["bert-base-ner"])
 # [Sarah, London]
+print(doc.spans["bert-base-ner"].attrs["scores"])
+# [0.99854773, 0.9996215]
 ```
 
 3. Save fine-grained tags as `Token.tag`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
```

#### html2text {}

```diff
@@ -59,47 +59,48 @@
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
 annotation is saved to the spaCy doc. You can save the output as `token.tag_`,
 `token.pos_` (only for UPOS tags), `doc.ents` or `doc.spans`. #### Examples 1.
 Save named entity annotation as `Doc.ents`: ```python import spacy nlp =
 spacy.blank("en") nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-
 base-NER"}) doc = nlp("My name is Sarah and I live in London") print(doc.ents)
-# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans
-[spans_key]`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "hf_token_pipe", config={ "model": "dslim/bert-base-NER", "annotate":
-"spans", "annotate_spans_key": "bert-base-ner", }, ) doc = nlp("My name is
-Sarah and I live in London") print(doc.spans["bert-base-ner"]) # [Sarah,
-London] ``` 3. Save fine-grained tags as `Token.tag`: ```python import spacy
-nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model": "QCRI/
-bert-base-multilingual-cased-pos-english", "annotate": "tag", }, ) doc = nlp
-("My name is Sarah and I live in London") print([t.tag_ for t in doc]) #
-['PRP$', 'NN', 'VBZ', 'NNP', 'CC', 'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save
-coarse-grained tags as `Token.pos`: ```python import spacy nlp = spacy.blank
-("en") nlp.add_pipe( "hf_token_pipe", config={"model": "vblagoje/bert-english-
-uncased-finetuned-pos", "annotate": "pos"}, ) doc = nlp("My name is Sarah and I
-live in London") print([t.pos_ for t in doc]) # ['PRON', 'NOUN', 'AUX',
-'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP', 'PROPN'] ``` ### Text classification
-Config settings for `hf_text_pipe`: ```ini [components.hf_text_pipe] factory =
-"hf_text_pipe" model = "distilbert-base-uncased-finetuned-sst-2-english" #
-Model name or path revision = "main" # Model revision kwargs = {} # Any
-additional arguments for # TextClassificationPipeline scorer = null # Optional
-scorer ``` The input texts are truncated according to the transformers model
-max length. #### `TextClassificationPipeline` settings - `model`: The model
-name or path. - `revision`: The model revision. For production use, a specific
-git commit is recommended instead of the default `main`. - `kwargs`: Any
-additional arguments to [`TextClassificationPipeline`](https://huggingface.co/
-docs/transformers/main_classes/
-pipelines#transformers.TextClassificationPipeline). #### Example ```python
-import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
-{"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
-is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
-0.00013048505934420973} ``` ### Batching and GPU Both token and text
-classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` If the component runs into an
-error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
-processing each text individually. If it runs into an error on an individual
-text, a warning is shown and the doc is returned without additional annotation.
-Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
-(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
-the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
-new thread on the [discussion board](https://github.com/explosion/spaCy/
-discussions) for other issues.
+# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans[spans_key]`
+and scores as `Doc.spans[spans_key].attrs["scores"]`: ```python import spacy
+nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model":
+"dslim/bert-base-NER", "annotate": "spans", "annotate_spans_key": "bert-base-
+ner", }, ) doc = nlp("My name is Sarah and I live in London") print(doc.spans
+["bert-base-ner"]) # [Sarah, London] print(doc.spans["bert-base-ner"].attrs
+["scores"]) # [0.99854773, 0.9996215] ``` 3. Save fine-grained tags as
+`Token.tag`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
+( "hf_token_pipe", config={ "model": "QCRI/bert-base-multilingual-cased-pos-
+english", "annotate": "tag", }, ) doc = nlp("My name is Sarah and I live in
+London") print([t.tag_ for t in doc]) # ['PRP$', 'NN', 'VBZ', 'NNP', 'CC',
+'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save coarse-grained tags as `Token.pos`:
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe",
+config={"model": "vblagoje/bert-english-uncased-finetuned-pos", "annotate":
+"pos"}, ) doc = nlp("My name is Sarah and I live in London") print([t.pos_ for
+t in doc]) # ['PRON', 'NOUN', 'AUX', 'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP',
+'PROPN'] ``` ### Text classification Config settings for `hf_text_pipe`: ```ini
+[components.hf_text_pipe] factory = "hf_text_pipe" model = "distilbert-base-
+uncased-finetuned-sst-2-english" # Model name or path revision = "main" # Model
+revision kwargs = {} # Any additional arguments for #
+TextClassificationPipeline scorer = null # Optional scorer ``` The input texts
+are truncated according to the transformers model max length. ####
+`TextClassificationPipeline` settings - `model`: The model name or path. -
+`revision`: The model revision. For production use, a specific git commit is
+recommended instead of the default `main`. - `kwargs`: Any additional arguments
+to [`TextClassificationPipeline`](https://huggingface.co/docs/transformers/
+main_classes/pipelines#transformers.TextClassificationPipeline). #### Example
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe",
+config={"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc =
+nlp("This is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419,
+'NEGATIVE': 0.00013048505934420973} ``` ### Batching and GPU Both token and
+text classification support batching with `nlp.pipe`: ```python for doc in
+nlp.pipe(texts, batch_size=256): do_something(doc) ``` If the component runs
+into an error processing a batch (e.g. on an empty text), `nlp.pipe` will back
+off to processing each text individually. If it runs into an error on an
+individual text, a warning is shown and the doc is returned without additional
+annotation. Switch to GPU: ```python import spacy spacy.require_gpu() for doc
+in nlp.pipe(texts): do_something(doc) ``` ## Bug reports and issues Please
+report bugs in the [spaCy issue tracker](https://github.com/explosion/spaCy/
+issues) or open a new thread on the [discussion board](https://github.com/
+explosion/spaCy/discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.3/setup.cfg` & `spacy_huggingface_pipelines-0.0.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.0.3
+version = 0.0.4
 description = spaCy wrapper for Hugging Face Transformers pipelines
 url = https://github.com/explosion/spacy-huggingface-pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/tests/test_pipeline_components.py` & `spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/tests/test_pipeline_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 import torch
 from thinc.api import get_torch_default_device
 import spacy
 
 torch.set_num_threads(1)
 
+pytestmark = pytest.mark.filterwarnings(
+    "ignore:The 'warn' method is deprecated.*:DeprecationWarning"
+)
+
 
 @pytest.mark.parametrize("aggregation_strategy", ("simple", "first", "average", "max"))
 @pytest.mark.parametrize("annotate", ("ents", "spans", "tag"))
 @pytest.mark.parametrize("n_process", (1, 2))
 @pytest.mark.filterwarnings(
     "ignore:Unable to process, skipping annotation for doc ' ':UserWarning"
 )
@@ -59,14 +63,15 @@
                 token.tag_.startswith("LABEL_")
         elif annotate == "ents":
             assert len(doc.ents) > 0
             for ent in doc.ents:
                 assert ent.label_.startswith("LABEL_")
         elif annotate == "spans":
             assert len(doc.spans["tiny"]) > 0
+            assert len(doc.spans["tiny"]) == len(doc.spans["tiny"].attrs["scores"])
             for span in doc.spans["tiny"]:
                 assert span.label_.startswith("LABEL_")
 
 
 @pytest.mark.parametrize("n_process", (1, 2))
 def test_hf_text_pipe(n_process):
     if (
```

### Comparing `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/text_classification.py` & `spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/text_classification.py`

 * *Files identical despite different names*

### Comparing `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines/token_classification.py` & `spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines/token_classification.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Callable, Iterable, Iterator, List, Literal, Optional
 import warnings
 
 from thinc.api import get_torch_default_device
 from spacy.language import Language
 from spacy.pipeline import Pipe
-from spacy.tokens import Doc, Span
+from spacy.tokens import Doc, Span, SpanGroup
 from spacy import util
 
 from transformers import pipeline
 
 
 @Language.factory(
     "hf_token_pipe",
@@ -99,29 +99,30 @@
     def __call__(self, doc: Doc) -> Doc:
         return next(self.pipe([doc]))
 
     def pipe(self, stream: Iterable[Doc], *, batch_size: int = 128) -> Iterator[Doc]:
         for docs in util.minibatch(stream, size=batch_size):
             outputs = self._get_annotations(docs)
             for doc, output in zip(docs, outputs):
-                output_spans = []
+                output_spans = SpanGroup(doc, attrs={"scores": []})
                 prev_ann_end = 0
                 for ann in output:
                     if ann["start"] >= prev_ann_end:
                         output_span = doc.char_span(
                             ann["start"],
                             ann["end"],
                             label=ann["entity_group"],
                             alignment_mode=self.alignment_mode,
                         )
                         if (
                             output_span is not None
                             and output_span.start_char >= prev_ann_end
                         ):
                             output_spans.append(output_span)
+                            output_spans.attrs["scores"].append(ann["score"])
                             prev_ann_end = ann["end"]
                         else:
                             text_excerpt = (
                                 doc.text
                                 if len(doc.text) < 100
                                 else doc.text[:100] + "..."
                             )
@@ -160,17 +161,17 @@
                     )
                     warnings.warn(
                         f"Unable to process, skipping annotation for doc '{text_excerpt}'"
                     )
                     outputs.append([])
             return outputs
 
-    def _set_annotation_from_spans(self, doc: Doc, spans: List[Span]) -> Doc:
+    def _set_annotation_from_spans(self, doc: Doc, spans: SpanGroup) -> Doc:
         if self.annotate == "ents":
-            doc.set_ents(spans)
+            doc.set_ents(list(spans))
         elif self.annotate == "spans":
             doc.spans[self.annotate_spans_key] = spans
         elif self.annotate == "tag":
             for span in spans:
                 for token in span:
                     token.tag_ = span.label_
         elif self.annotate == "pos":
```

### Comparing `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/PKG-INFO` & `spacy_huggingface_pipelines-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spacy-huggingface-pipelines
-Version: 0.0.3
+Name: spacy_huggingface_pipelines
+Version: 0.0.4
 Summary: spaCy wrapper for Hugging Face Transformers pipelines
 Home-page: https://github.com/explosion/spacy-huggingface-pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-huggingface-pipelines/releases
 Project-URL: Source, https://github.com/explosion/spacy-huggingface-pipelines
@@ -141,15 +141,16 @@
 nlp = spacy.blank("en")
 nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-base-NER"})
 doc = nlp("My name is Sarah and I live in London")
 print(doc.ents)
 # (Sarah, London)
 ```
 
-2. Save named entity annotation as `Doc.spans[spans_key]`:
+2. Save named entity annotation as `Doc.spans[spans_key]` and scores as
+   `Doc.spans[spans_key].attrs["scores"]`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
 nlp.add_pipe(
     "hf_token_pipe",
     config={
@@ -157,14 +158,16 @@
         "annotate": "spans",
         "annotate_spans_key": "bert-base-ner",
     },
 )
 doc = nlp("My name is Sarah and I live in London")
 print(doc.spans["bert-base-ner"])
 # [Sarah, London]
+print(doc.spans["bert-base-ner"].attrs["scores"])
+# [0.99854773, 0.9996215]
 ```
 
 3. Save fine-grained tags as `Token.tag`:
 
 ```python
 import spacy
 nlp = spacy.blank("en")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-huggingface-pipelines Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: spacy_huggingface_pipelines Version: 0.0.4 Summary:
 spaCy wrapper for Hugging Face Transformers pipelines Home-page: https://
 github.com/explosion/spacy-huggingface-pipelines Author: Explosion Author-
 email: contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-huggingface-pipelines/releases Project-URL: Source,
 https://github.com/explosion/spacy-huggingface-pipelines Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
@@ -76,47 +76,48 @@
 token boundaries as described for [`Doc.char_span`](https://spacy.io/api/
 doc#char_span). - `annotate` and `annotate_spans_key` configure how the
 annotation is saved to the spaCy doc. You can save the output as `token.tag_`,
 `token.pos_` (only for UPOS tags), `doc.ents` or `doc.spans`. #### Examples 1.
 Save named entity annotation as `Doc.ents`: ```python import spacy nlp =
 spacy.blank("en") nlp.add_pipe("hf_token_pipe", config={"model": "dslim/bert-
 base-NER"}) doc = nlp("My name is Sarah and I live in London") print(doc.ents)
-# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans
-[spans_key]`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
-( "hf_token_pipe", config={ "model": "dslim/bert-base-NER", "annotate":
-"spans", "annotate_spans_key": "bert-base-ner", }, ) doc = nlp("My name is
-Sarah and I live in London") print(doc.spans["bert-base-ner"]) # [Sarah,
-London] ``` 3. Save fine-grained tags as `Token.tag`: ```python import spacy
-nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model": "QCRI/
-bert-base-multilingual-cased-pos-english", "annotate": "tag", }, ) doc = nlp
-("My name is Sarah and I live in London") print([t.tag_ for t in doc]) #
-['PRP$', 'NN', 'VBZ', 'NNP', 'CC', 'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save
-coarse-grained tags as `Token.pos`: ```python import spacy nlp = spacy.blank
-("en") nlp.add_pipe( "hf_token_pipe", config={"model": "vblagoje/bert-english-
-uncased-finetuned-pos", "annotate": "pos"}, ) doc = nlp("My name is Sarah and I
-live in London") print([t.pos_ for t in doc]) # ['PRON', 'NOUN', 'AUX',
-'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP', 'PROPN'] ``` ### Text classification
-Config settings for `hf_text_pipe`: ```ini [components.hf_text_pipe] factory =
-"hf_text_pipe" model = "distilbert-base-uncased-finetuned-sst-2-english" #
-Model name or path revision = "main" # Model revision kwargs = {} # Any
-additional arguments for # TextClassificationPipeline scorer = null # Optional
-scorer ``` The input texts are truncated according to the transformers model
-max length. #### `TextClassificationPipeline` settings - `model`: The model
-name or path. - `revision`: The model revision. For production use, a specific
-git commit is recommended instead of the default `main`. - `kwargs`: Any
-additional arguments to [`TextClassificationPipeline`](https://huggingface.co/
-docs/transformers/main_classes/
-pipelines#transformers.TextClassificationPipeline). #### Example ```python
-import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe", config=
-{"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc = nlp("This
-is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419, 'NEGATIVE':
-0.00013048505934420973} ``` ### Batching and GPU Both token and text
-classification support batching with `nlp.pipe`: ```python for doc in nlp.pipe
-(texts, batch_size=256): do_something(doc) ``` If the component runs into an
-error processing a batch (e.g. on an empty text), `nlp.pipe` will back off to
-processing each text individually. If it runs into an error on an individual
-text, a warning is shown and the doc is returned without additional annotation.
-Switch to GPU: ```python import spacy spacy.require_gpu() for doc in nlp.pipe
-(texts): do_something(doc) ``` ## Bug reports and issues Please report bugs in
-the [spaCy issue tracker](https://github.com/explosion/spaCy/issues) or open a
-new thread on the [discussion board](https://github.com/explosion/spaCy/
-discussions) for other issues.
+# (Sarah, London) ``` 2. Save named entity annotation as `Doc.spans[spans_key]`
+and scores as `Doc.spans[spans_key].attrs["scores"]`: ```python import spacy
+nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe", config={ "model":
+"dslim/bert-base-NER", "annotate": "spans", "annotate_spans_key": "bert-base-
+ner", }, ) doc = nlp("My name is Sarah and I live in London") print(doc.spans
+["bert-base-ner"]) # [Sarah, London] print(doc.spans["bert-base-ner"].attrs
+["scores"]) # [0.99854773, 0.9996215] ``` 3. Save fine-grained tags as
+`Token.tag`: ```python import spacy nlp = spacy.blank("en") nlp.add_pipe
+( "hf_token_pipe", config={ "model": "QCRI/bert-base-multilingual-cased-pos-
+english", "annotate": "tag", }, ) doc = nlp("My name is Sarah and I live in
+London") print([t.tag_ for t in doc]) # ['PRP$', 'NN', 'VBZ', 'NNP', 'CC',
+'PRP', 'VBP', 'IN', 'NNP'] ``` 4. Save coarse-grained tags as `Token.pos`:
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_token_pipe",
+config={"model": "vblagoje/bert-english-uncased-finetuned-pos", "annotate":
+"pos"}, ) doc = nlp("My name is Sarah and I live in London") print([t.pos_ for
+t in doc]) # ['PRON', 'NOUN', 'AUX', 'PROPN', 'CCONJ', 'PRON', 'VERB', 'ADP',
+'PROPN'] ``` ### Text classification Config settings for `hf_text_pipe`: ```ini
+[components.hf_text_pipe] factory = "hf_text_pipe" model = "distilbert-base-
+uncased-finetuned-sst-2-english" # Model name or path revision = "main" # Model
+revision kwargs = {} # Any additional arguments for #
+TextClassificationPipeline scorer = null # Optional scorer ``` The input texts
+are truncated according to the transformers model max length. ####
+`TextClassificationPipeline` settings - `model`: The model name or path. -
+`revision`: The model revision. For production use, a specific git commit is
+recommended instead of the default `main`. - `kwargs`: Any additional arguments
+to [`TextClassificationPipeline`](https://huggingface.co/docs/transformers/
+main_classes/pipelines#transformers.TextClassificationPipeline). #### Example
+```python import spacy nlp = spacy.blank("en") nlp.add_pipe( "hf_text_pipe",
+config={"model": "distilbert-base-uncased-finetuned-sst-2-english"}, ) doc =
+nlp("This is great!") print(doc.cats) # {'POSITIVE': 0.9998694658279419,
+'NEGATIVE': 0.00013048505934420973} ``` ### Batching and GPU Both token and
+text classification support batching with `nlp.pipe`: ```python for doc in
+nlp.pipe(texts, batch_size=256): do_something(doc) ``` If the component runs
+into an error processing a batch (e.g. on an empty text), `nlp.pipe` will back
+off to processing each text individually. If it runs into an error on an
+individual text, a warning is shown and the doc is returned without additional
+annotation. Switch to GPU: ```python import spacy spacy.require_gpu() for doc
+in nlp.pipe(texts): do_something(doc) ``` ## Bug reports and issues Please
+report bugs in the [spaCy issue tracker](https://github.com/explosion/spaCy/
+issues) or open a new thread on the [discussion board](https://github.com/
+explosion/spaCy/discussions) for other issues.
```

### Comparing `spacy_huggingface_pipelines-0.0.3/spacy_huggingface_pipelines.egg-info/SOURCES.txt` & `spacy_huggingface_pipelines-0.0.4/spacy_huggingface_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

