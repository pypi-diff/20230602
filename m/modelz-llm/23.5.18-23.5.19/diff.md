# Comparing `tmp/modelz-llm-23.5.18.tar.gz` & `tmp/modelz-llm-23.5.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.5.18.tar", last modified: Fri Jun  2 03:42:55 2023, max compression
+gzip compressed data, was "modelz-llm-23.5.19.tar", last modified: Fri Jun  2 03:52:58 2023, max compression
```

## Comparing `modelz-llm-23.5.18.tar` & `modelz-llm-23.5.19.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.5.18/.github/workflows/docker-publish.yml` & `modelz-llm-23.5.19/.github/workflows/docker-publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         image:
           - name: modelzai/llm-chatglm-6b-int4
             dockerfile: ./images/base/Dockerfile
           - name: modelzai/llm-chatglm-6b
             dockerfile: ./images/chatglm-6b/Dockerfile
           - name: modelzai/llm-llama-7b
             dockerfile: ./images/llama-7b/Dockerfile
-          # - name: modelzai/llm-fastchat-t5-3b
-          #   dockerfile: ./images/fastchat-t5-3b/Dockerfile
+          - name: modelzai/llm-fastchat-t5-3b
+            dockerfile: ./images/fastchat-t5-3b/Dockerfile
           - name: modelzai/llm-vicuna-7b
             dockerfile: ./images/vicuna-7b/Dockerfile
     runs-on: ubuntu-latest
     permissions:
       contents: read
       packages: write
```

### Comparing `modelz-llm-23.5.18/.github/workflows/gcr.yml` & `modelz-llm-23.5.19/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/.github/workflows/python-check.yml` & `modelz-llm-23.5.19/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/.github/workflows/python-publish.yml` & `modelz-llm-23.5.19/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/.gitignore` & `modelz-llm-23.5.19/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/PKG-INFO` & `modelz-llm-23.5.19/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.18
+Version: 23.5.19
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -48,30 +48,43 @@
 modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
 | Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
+|FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general)
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
 | Bloomz 560M | `bigscience/bloomz-560m` | |
 | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | |
 | Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
-<!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
 openai.api_key="any"
 
 # create a chat completion
 chat_completion = openai.ChatCompletion.create(model="any", messages=[{"role": "user", "content": "Hello world"}])
 ```
+
+## Supported APIs
+
+```py
+    app.add_route("/", Ping())
+    app.add_route("/completions", completion)
+    app.add_route("/chat/completions", chat_completion)
+    app.add_route("/embeddings", embeddings)
+    app.add_route("/engines/{engine}/embeddings", embeddings)
+    app.add_route("/v1/completions", completion)
+    app.add_route("/v1/chat/completions", chat_completion)
+    app.add_route("/v1/embeddings", embeddings)
+    app.add_route("/v1/engines/{engine}/embeddings", embeddings)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.18 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.19 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
@@ -18,22 +18,30 @@
 Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
 docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
 # or install from source pip install git+https://github.com/tensorchord/modelz-
 llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
 self-hosted API server by following the instructions: ```bash modelz-llm -
 m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
 Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
--------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+-------------- | |FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-
+fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-
+t5-3b/general) | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
 //hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
 560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
-7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+7b1` | | ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
-"content": "Hello world"}]) ```
+"content": "Hello world"}]) ``` ## Supported APIs ```py app.add_route("/", Ping
+()) app.add_route("/completions", completion) app.add_route("/chat/
+completions", chat_completion) app.add_route("/embeddings", embeddings)
+app.add_route("/engines/{engine}/embeddings", embeddings) app.add_route("/v1/
+completions", completion) app.add_route("/v1/chat/completions",
+chat_completion) app.add_route("/v1/embeddings", embeddings) app.add_route("/
+v1/engines/{engine}/embeddings", embeddings) ```
```

### Comparing `modelz-llm-23.5.18/README.md` & `modelz-llm-23.5.19/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -36,30 +36,43 @@
 modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
 | Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
+|FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general)
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
 | Bloomz 560M | `bigscience/bloomz-560m` | |
 | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | |
 | Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
-<!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
 openai.api_key="any"
 
 # create a chat completion
 chat_completion = openai.ChatCompletion.create(model="any", messages=[{"role": "user", "content": "Hello world"}])
 ```
+
+## Supported APIs
+
+```py
+    app.add_route("/", Ping())
+    app.add_route("/completions", completion)
+    app.add_route("/chat/completions", chat_completion)
+    app.add_route("/embeddings", embeddings)
+    app.add_route("/engines/{engine}/embeddings", embeddings)
+    app.add_route("/v1/completions", completion)
+    app.add_route("/v1/chat/completions", chat_completion)
+    app.add_route("/v1/embeddings", embeddings)
+    app.add_route("/v1/engines/{engine}/embeddings", embeddings)
+```
```

#### html2text {}

```diff
@@ -12,22 +12,30 @@
 Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
 docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
 # or install from source pip install git+https://github.com/tensorchord/modelz-
 llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
 self-hosted API server by following the instructions: ```bash modelz-llm -
 m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
 Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
--------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+-------------- | |FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-
+fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-
+t5-3b/general) | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
 //hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
 560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
-7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+7b1` | | ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
-"content": "Hello world"}]) ```
+"content": "Hello world"}]) ``` ## Supported APIs ```py app.add_route("/", Ping
+()) app.add_route("/completions", completion) app.add_route("/chat/
+completions", chat_completion) app.add_route("/embeddings", embeddings)
+app.add_route("/engines/{engine}/embeddings", embeddings) app.add_route("/v1/
+completions", completion) app.add_route("/v1/chat/completions",
+chat_completion) app.add_route("/v1/embeddings", embeddings) app.add_route("/
+v1/engines/{engine}/embeddings", embeddings) ```
```

### Comparing `modelz-llm-23.5.18/build.envd` & `modelz-llm-23.5.19/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/client.py` & `modelz-llm-23.5.19/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/images/base/Dockerfile` & `modelz-llm-23.5.19/images/base/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ENV MOSEC_PORT=${MOSEC_PORT}
 
 ARG CONDA_VERSION=py310_22.11.1-1
 
 RUN apt update && \
     apt install -y --no-install-recommends \
         wget \
+        git \
         build-essential \
         ca-certificates && \
     rm -rf /var/lib/apt/lists/*
 
 RUN set -x && \
     UNAME_M="$(uname -m)" && \
     if [ "${UNAME_M}" = "x86_64" ]; then \
```

### Comparing `modelz-llm-23.5.18/images/chatglm-6b/Dockerfile` & `modelz-llm-23.5.19/images/chatglm-6b/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ENV MOSEC_PORT=${MOSEC_PORT}
 
 ARG CONDA_VERSION=py310_22.11.1-1
 
 RUN apt update && \
     apt install -y --no-install-recommends \
         wget \
+        git \
         build-essential \
         ca-certificates && \
     rm -rf /var/lib/apt/lists/*
 
 RUN set -x && \
     UNAME_M="$(uname -m)" && \
     if [ "${UNAME_M}" = "x86_64" ]; then \
```

### Comparing `modelz-llm-23.5.18/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.5.19/images/fastchat-t5-3b/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ENV MOSEC_PORT=${MOSEC_PORT}
 
 ARG CONDA_VERSION=py310_22.11.1-1
 
 RUN apt update && \
     apt install -y --no-install-recommends \
         wget \
+        git \
         build-essential \
         ca-certificates && \
     rm -rf /var/lib/apt/lists/*
 
 RUN set -x && \
     UNAME_M="$(uname -m)" && \
     if [ "${UNAME_M}" = "x86_64" ]; then \
```

### Comparing `modelz-llm-23.5.18/images/llama-7b/Dockerfile` & `modelz-llm-23.5.19/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/images/vicuna-7b/Dockerfile` & `modelz-llm-23.5.19/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/pyproject.toml` & `modelz-llm-23.5.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/src/modelz_llm/cli.py` & `modelz-llm-23.5.19/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/src/modelz_llm/falcon_service.py` & `modelz-llm-23.5.19/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/src/modelz_llm/mosec_service.py` & `modelz-llm-23.5.19/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/src/modelz_llm/utils.py` & `modelz-llm-23.5.19/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.18/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.5.19/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.18
+Version: 23.5.19
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -48,30 +48,43 @@
 modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
 | Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
+|FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-t5-3b/general)
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
 | Bloomz 560M | `bigscience/bloomz-560m` | |
 | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | |
 | Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
-<!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
 openai.api_key="any"
 
 # create a chat completion
 chat_completion = openai.ChatCompletion.create(model="any", messages=[{"role": "user", "content": "Hello world"}])
 ```
+
+## Supported APIs
+
+```py
+    app.add_route("/", Ping())
+    app.add_route("/completions", completion)
+    app.add_route("/chat/completions", chat_completion)
+    app.add_route("/embeddings", embeddings)
+    app.add_route("/engines/{engine}/embeddings", embeddings)
+    app.add_route("/v1/completions", completion)
+    app.add_route("/v1/chat/completions", chat_completion)
+    app.add_route("/v1/embeddings", embeddings)
+    app.add_route("/v1/engines/{engine}/embeddings", embeddings)
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.18 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.19 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
@@ -18,22 +18,30 @@
 Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
 docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
 # or install from source pip install git+https://github.com/tensorchord/modelz-
 llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
 self-hosted API server by following the instructions: ```bash modelz-llm -
 m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
 Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
--------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+-------------- | |FastChat T5 | `lmsys/fastchat-t5-3b-v1.0` | [modelzai/llm-
+fastchat-t5-3b](https://hub.docker.com/repository/docker/modelzai/llm-fastchat-
+t5-3b/general) | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
 //hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
 560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
 | Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
-7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+7b1` | | ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
-"content": "Hello world"}]) ```
+"content": "Hello world"}]) ``` ## Supported APIs ```py app.add_route("/", Ping
+()) app.add_route("/completions", completion) app.add_route("/chat/
+completions", chat_completion) app.add_route("/embeddings", embeddings)
+app.add_route("/engines/{engine}/embeddings", embeddings) app.add_route("/v1/
+completions", completion) app.add_route("/v1/chat/completions",
+chat_completion) app.add_route("/v1/embeddings", embeddings) app.add_route("/
+v1/engines/{engine}/embeddings", embeddings) ```
```

### Comparing `modelz-llm-23.5.18/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.5.19/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

