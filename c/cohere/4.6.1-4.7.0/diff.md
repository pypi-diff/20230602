# Comparing `tmp/cohere-4.6.1.tar.gz` & `tmp/cohere-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-4.6.1.tar", max compression
+gzip compressed data, was "cohere-4.7.0.tar", max compression
```

## Comparing `cohere-4.6.1.tar` & `cohere-4.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:14:58.099289 cohere-4.6.1/LICENSE
--rw-r--r--   0        0        0     4480 2023-06-01 11:14:58.099289 cohere-4.6.1/README.md
--rw-r--r--   0        0        0      771 2023-06-01 11:14:58.099289 cohere-4.6.1/cohere/__init__.py
--rw-r--r--   0        0        0    37633 2023-06-01 11:14:58.099289 cohere-4.6.1/cohere/client.py
--rw-r--r--   0        0        0    28050 2023-06-01 11:14:58.099289 cohere-4.6.1/cohere/client_async.py
--rw-r--r--   0        0        0     1187 2023-06-01 11:14:58.099289 cohere-4.6.1/cohere/error.py
--rw-r--r--   0        0        0      529 2023-06-01 11:14:58.099289 cohere-4.6.1/cohere/logging.py
--rw-r--r--   0        0        0      839 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/base.py
--rw-r--r--   0        0        0     3438 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/bulk_embed.py
--rw-r--r--   0        0        0     4309 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/chat.py
--rw-r--r--   0        0        0     1461 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/classify.py
--rw-r--r--   0        0        0     4826 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/cluster.py
--rw-r--r--   0        0        0      436 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/codebook.py
--rw-r--r--   0        0        0      552 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/detectlang.py
--rw-r--r--   0        0        0      587 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/embeddings.py
--rw-r--r--   0        0        0      342 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/feedback.py
--rw-r--r--   0        0        0     5990 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/generation.py
--rw-r--r--   0        0        0     2057 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/rerank.py
--rw-r--r--   0        0        0      667 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/summarize.py
--rw-r--r--   0        0        0     1221 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/responses/tokenize.py
--rw-r--r--   0        0        0     3283 2023-06-01 11:14:58.103289 cohere-4.6.1/cohere/utils.py
--rw-r--r--   0        0        0      653 2023-06-01 11:14:58.103289 cohere-4.6.1/pyproject.toml
--rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.6.1/setup.py
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-02 17:04:01.524493 cohere-4.7.0/LICENSE
+-rw-r--r--   0        0        0     4480 2023-06-02 17:04:01.524493 cohere-4.7.0/README.md
+-rw-r--r--   0        0        0      771 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/__init__.py
+-rw-r--r--   0        0        0    38178 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/client.py
+-rw-r--r--   0        0        0    28216 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/client_async.py
+-rw-r--r--   0        0        0     1187 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/error.py
+-rw-r--r--   0        0        0      529 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/logging.py
+-rw-r--r--   0        0        0      839 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/base.py
+-rw-r--r--   0        0        0     3438 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/bulk_embed.py
+-rw-r--r--   0        0        0     4309 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/chat.py
+-rw-r--r--   0        0        0     1461 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/classify.py
+-rw-r--r--   0        0        0     4826 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/cluster.py
+-rw-r--r--   0        0        0      436 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/codebook.py
+-rw-r--r--   0        0        0      552 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/detectlang.py
+-rw-r--r--   0        0        0      587 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/embeddings.py
+-rw-r--r--   0        0        0      342 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/feedback.py
+-rw-r--r--   0        0        0     5990 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/generation.py
+-rw-r--r--   0        0        0     2057 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/rerank.py
+-rw-r--r--   0        0        0      667 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/summarize.py
+-rw-r--r--   0        0        0     1221 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/responses/tokenize.py
+-rw-r--r--   0        0        0     3283 2023-06-02 17:04:01.524493 cohere-4.7.0/cohere/utils.py
+-rw-r--r--   0        0        0      653 2023-06-02 17:04:01.528493 cohere-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 cohere-4.7.0/setup.py
+-rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 cohere-4.7.0/PKG-INFO
```

### Comparing `cohere-4.6.1/LICENSE` & `cohere-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/README.md` & `cohere-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/__init__.py` & `cohere-4.7.0/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/client.py` & `cohere-4.7.0/cohere/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -428,61 +428,65 @@
         }
         # remove None values from the dict
         json_body = {k: v for k, v in json_body.items() if v is not None}
         response = self._request(cohere.SUMMARIZE_URL, json=json_body)
 
         return SummarizeResponse(id=response["id"], summary=response["summary"], meta=response["meta"])
 
-    def batch_tokenize(self, texts: List[str], return_exceptions=False) -> List[Union[Tokens, Exception]]:
+    def batch_tokenize(self, texts: List[str], return_exceptions=False, **kwargs) -> List[Union[Tokens, Exception]]:
         """A batched version of tokenize.
 
         Args:
             texts: list of texts
             return_exceptions (bool): Return exceptions as list items rather than raise them. Ensures your entire batch is not lost on one of the items failing.
+            kwargs: other arguments to `tokenize`
         """
         return threadpool_map(
             self.tokenize,
-            [dict(text=text) for text in texts],
+            [dict(text=text, **kwargs) for text in texts],
             num_workers=self.num_workers,
             return_exceptions=return_exceptions,
         )
 
-    def tokenize(self, text: str) -> Tokens:
+    def tokenize(self, text: str, model: Optional[str] = None) -> Tokens:
         """Returns a Tokens object of the provided text, see https://docs.cohere.ai/reference/tokenize for advanced usage.
 
         Args:
             text (str): Text to summarize.
+            model (str): An optional model name that will ensure that the tokenization uses the tokenizer used by that model, which can be critical for counting tokens properly.
         """
-        json_body = {"text": text}
+        json_body = {"text": text, "model": model}
         res = self._request(cohere.TOKENIZE_URL, json=json_body)
         return Tokens(tokens=res["tokens"], token_strings=res["token_strings"], meta=res.get("meta"))
 
     def batch_detokenize(
-        self, list_of_tokens: List[List[int]], return_exceptions=False
+        self, list_of_tokens: List[List[int]], return_exceptions=False, **kwargs
     ) -> List[Union[Detokenization, Exception]]:
         """A batched version of detokenize.
 
         Args:
             list_of_tokens: list of list of tokens
             return_exceptions (bool): Return exceptions as list items rather than raise them. Ensures your entire batch is not lost on one of the items failing.
+            kwargs: other arguments to `detokenize`
         """
         return threadpool_map(
             self.detokenize,
-            [dict(tokens=tokens) for tokens in list_of_tokens],
+            [dict(tokens=tokens, **kwargs) for tokens in list_of_tokens],
             num_workers=self.num_workers,
             return_exceptions=return_exceptions,
         )
 
-    def detokenize(self, tokens: List[int]) -> Detokenization:
+    def detokenize(self, tokens: List[int], model: Optional[str] = None) -> Detokenization:
         """Returns a Detokenization object of the provided tokens, see https://docs.cohere.ai/reference/detokenize for advanced usage.
 
         Args:
             tokens (List[int]): A list of tokens to convert to strings
+            model (str): An optional model name. This will ensure that the detokenization is done by the tokenizer used by that model.
         """
-        json_body = {"tokens": tokens}
+        json_body = {"tokens": tokens, "model": model}
         res = self._request(cohere.DETOKENIZE_URL, json=json_body)
         return Detokenization(text=res["text"], meta=res.get("meta"))
 
     def detect_language(self, texts: List[str]) -> DetectLanguageResponse:
         """Returns a DetectLanguageResponse object of the provided texts, see https://docs.cohere.ai/reference/detect-language-1 for advanced usage.
 
         Args:
```

### Comparing `cohere-4.6.1/cohere/client_async.py` & `cohere-4.7.0/cohere/client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -317,29 +317,33 @@
             "extractiveness": extractiveness,
         }
         # remove None values from the dict
         json_body = {k: v for k, v in json_body.items() if v is not None}
         response = await self._request(cohere.SUMMARIZE_URL, json=json_body)
         return SummarizeResponse(id=response["id"], summary=response["summary"], meta=response["meta"])
 
-    async def batch_tokenize(self, texts: List[str], return_exceptions=False) -> List[Union[Tokens, Exception]]:
-        return await asyncio.gather(*[self.tokenize(t) for t in texts], return_exceptions=return_exceptions)
+    async def batch_tokenize(
+        self, texts: List[str], return_exceptions=False, **kwargs
+    ) -> List[Union[Tokens, Exception]]:
+        return await asyncio.gather(*[self.tokenize(t, **kwargs) for t in texts], return_exceptions=return_exceptions)
 
-    async def tokenize(self, text: str) -> Tokens:
-        json_body = {"text": text}
+    async def tokenize(self, text: str, model: Optional[str] = None) -> Tokens:
+        json_body = {"text": text, "model": model}
         res = await self._request(cohere.TOKENIZE_URL, json_body)
         return Tokens(tokens=res["tokens"], token_strings=res["token_strings"], meta=res["meta"])
 
     async def batch_detokenize(
-        self, list_of_tokens: List[List[int]], return_exceptions=False
+        self, list_of_tokens: List[List[int]], return_exceptions=False, **kwargs
     ) -> List[Union[Detokenization, Exception]]:
-        return await asyncio.gather(*[self.detokenize(t) for t in list_of_tokens], return_exceptions=return_exceptions)
+        return await asyncio.gather(
+            *[self.detokenize(t, **kwargs) for t in list_of_tokens], return_exceptions=return_exceptions
+        )
 
-    async def detokenize(self, tokens: List[int]) -> Detokenization:
-        json_body = {"tokens": tokens}
+    async def detokenize(self, tokens: List[int], model: Optional[str] = None) -> Detokenization:
+        json_body = {"tokens": tokens, "model": model}
         res = await self._request(cohere.DETOKENIZE_URL, json_body)
         return Detokenization(text=res["text"], meta=res["meta"])
 
     async def detect_language(self, texts: List[str]) -> DetectLanguageResponse:
         json_body = {
             "texts": texts,
         }
```

### Comparing `cohere-4.6.1/cohere/error.py` & `cohere-4.7.0/cohere/error.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/logging.py` & `cohere-4.7.0/cohere/logging.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/__init__.py` & `cohere-4.7.0/cohere/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/base.py` & `cohere-4.7.0/cohere/responses/base.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/bulk_embed.py` & `cohere-4.7.0/cohere/responses/bulk_embed.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/chat.py` & `cohere-4.7.0/cohere/responses/chat.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/classify.py` & `cohere-4.7.0/cohere/responses/classify.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/cluster.py` & `cohere-4.7.0/cohere/responses/cluster.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/detectlang.py` & `cohere-4.7.0/cohere/responses/detectlang.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/embeddings.py` & `cohere-4.7.0/cohere/responses/embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/generation.py` & `cohere-4.7.0/cohere/responses/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/rerank.py` & `cohere-4.7.0/cohere/responses/rerank.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/summarize.py` & `cohere-4.7.0/cohere/responses/summarize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/responses/tokenize.py` & `cohere-4.7.0/cohere/responses/tokenize.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/cohere/utils.py` & `cohere-4.7.0/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-4.6.1/pyproject.toml` & `cohere-4.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cohere"
-version = "4.6.1"
+version = "4.7.0"
 description = ""
 authors = ["Cohere"]
 readme = "README.md"
 
 [tool.black]
 line-length = 120
 target_version = ['py38']
```

### Comparing `cohere-4.6.1/setup.py` & `cohere-4.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.0,<4.0', 'backoff>=2.0,<3.0', 'requests>=2.0,<3.0']
 
 setup_kwargs = {
     'name': 'cohere',
-    'version': '4.6.1',
+    'version': '4.7.0',
     'description': '',
     'long_description': '![ci badge](https://github.com/cohere-ai/cohere-python/actions/workflows/test.yaml/badge.svg)\n![version badge](https://img.shields.io/pypi/v/cohere)\n![license badge](https://img.shields.io/github/license/cohere-ai/cohere-python)\n\n# Cohere Python SDK\n\nThis package provides functionality developed to simplify interfacing with the [Cohere API](https://docs.cohere.ai/) in Python 3.\n\n## Documentation\n\n* SDK Documentation is hosted on [Read the docs](https://cohere-sdk.readthedocs.io/en/latest/).\n  * You can build SDK documentation locally using `cd docs; make clean html`.\n* For more details on advanced parameters, you can also consult the [API documentation](https://docs.cohere.ai/reference/about).\n* See the [examples](examples/) directory for examples, including  some additional functionality for visualizations in Jupyter notebooks.\n\n## Installation\n\nThe package can be installed with `pip`:\n\n```bash\npip install --upgrade cohere\n```\n\nInstall from source:\n\n```bash\npip install .\n```\n\n### Requirements\n\n- Python 3.7+\n\n## Quick Start\n\nTo use this library, you must have an API key and specify it as a string when creating the `cohere.Client` object. API keys can be created through the [platform](https://os.cohere.ai). This is a basic example of the creating the client and using the `generate` endpoint.\n\n```python\nimport cohere\n\n# initialize the Cohere Client with an API Key\nco = cohere.Client(\'YOUR_API_KEY\')\n\n# generate a prediction for a prompt\nprediction = co.generate(\n            model=\'large\',\n            prompt=\'co:here\',\n            max_tokens=10)\n\n# print the predicted text\nprint(\'prediction: {}\'.format(prediction.generations[0].text))\n```\n\nThere is also an asyncio compatible client called `cohere.AsyncClient` with an equivalent interface. Consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) for more details.\n\n## Versioning\n\nEach SDK release is only compatible with the latest version of the Cohere API at the time of release. To use the SDK with an older API version, you need to download a version of the SDK tied to the API version you want. Look at the [Changelog](https://github.com/cohere-ai/cohere-python/blob/main/CHANGELOG.md) to see which SDK version to download.\n\n\n## Endpoints\n\nFor a full breakdown of endpoints and arguments, please consult the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere API Docs](https://docs.cohere.ai/).\n\n| Cohere Endpoint  | Function             |\n| ---------------- | -------------------- |\n| /generate        | co.generate()        |\n| /embed           | co.embed()           |\n| /classify        | co.classify()        |\n| /tokenize        | co.tokenize()        |\n| /detokenize      | co.detokenize()      |\n| /detect-language | co.detect_language() |\n\n## Models\n\nWhen you call Cohere\'s APIs we decide on a good default model for your use-case behind the scenes. The default model is great to get you started, but in production environments we recommend that you specify the model size yourself via the `model` parameter. Learn more about the available models here(https://os.cohere.ai)\n\n## Responses\n\nAll of the endpoint functions will return a Cohere object corresponding to the endpoint (e.g. for generation, it would be `Generation`). The responses can be found as instance variables of the object (e.g. generation would be `Generation.text`). The names of these instance variables and a detailed breakdown of the response body can be found in the [SDK Docs](https://cohere-sdk.readthedocs.io/en/latest/) and [Cohere Docs](https://docs.cohere.ai/). Printing the Cohere response object itself will display an organized view of the instance variables.\n\n## Exceptions\n\nUnsuccessful API calls from the SDK will raise an exception. Please see the documentation\'s page on [errors](https://docs.cohere.ai/errors-reference) for more information about what the errors mean.\n\n## Contributing\n\nTo set up a development environment, run:\n\n```\npoetry shell    # any time you want to run code or tests\npoetry install  # install and update dependencies in your environment, the first time\n```\n\nIn addition, to ensure your code is formatted correctly, install pre-commit hooks using:\n\n```bash\npre-commit install\n```\n\nYou can run tests locally using:\n```\npython -m pytest\n```\n\nYou can configure a different base url with:\n```bash\nCO_API_URL="https://localhost:8050" python3 foo.py\n```\nor\n```python\ncohere.COHERE_API_URL = "https://localhost:8050" # Place before client initilization\n```\n',
     'author': 'Cohere',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cohere-4.6.1/PKG-INFO` & `cohere-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 4.6.1
+Version: 4.7.0
 Summary: 
 Author: Cohere
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

