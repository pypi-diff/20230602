# Comparing `tmp/modelz-llm-23.5.12.tar.gz` & `tmp/modelz-llm-23.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.5.12.tar", last modified: Thu May 25 11:48:15 2023, max compression
+gzip compressed data, was "modelz-llm-23.5.18.tar", last modified: Fri Jun  2 03:42:55 2023, max compression
```

## Comparing `modelz-llm-23.5.12.tar` & `modelz-llm-23.5.18.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.155868 modelz-llm-23.5.12/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.147868 modelz-llm-23.5.12/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.147868 modelz-llm-23.5.12/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:48:15.155868 modelz-llm-23.5.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.147868 modelz-llm-23.5.12/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-25 11:48:02.000000 modelz-llm-23.5.12/src/modelz_llm/mosec_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:48:15.151868 modelz-llm-23.5.12/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 11:48:15.000000 modelz-llm-23.5.12/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.533335 modelz-llm-23.5.18/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 03:42:44.000000 modelz-llm-23.5.18/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:42:55.537335 modelz-llm-23.5.18/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 03:42:55.000000 modelz-llm-23.5.18/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.5.12/.github/workflows/docker-publish.yml` & `modelz-llm-23.5.18/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/.github/workflows/gcr.yml` & `modelz-llm-23.5.18/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/.github/workflows/python-check.yml` & `modelz-llm-23.5.18/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/.github/workflows/python-publish.yml` & `modelz-llm-23.5.18/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/.gitignore` & `modelz-llm-23.5.18/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/PKG-INFO` & `modelz-llm-23.5.18/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.12
+Version: 23.5.18
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: gpu
 
 <div align="center">
 
 # Modelz LLM
 
 </div>
 
@@ -23,48 +24,49 @@
 Modelz LLM is an inference server that facilitates the utilization of open source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on either **local or cloud-based** environments with **OpenAI compatible API**.
 
 ## Features
 
 - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK to interact with the model.
 - **Self-hosted**: Modelz LLM can be easily deployed on either local or cloud-based environments.
 - **Open source LLMs**: Modelz LLM supports open source LLMs, such as FastChat, LLaMA, and ChatGLM.
-- **Modelz integration**: Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai), which is a serverless inference platform for LLMs and other foundation models.
+- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://docs.modelz.ai))
 
 ## Quick Start
 
 ### Install
 
 ```bash
-pip install modelz-llm
+pip install modelz-llm[gpu]
 # or install from source
-pip install git+https://github.com/tensorchord/modelz-llm.git
+pip install git+https://github.com/tensorchord/modelz-llm.git[gpu]
 ```
 
 ### Run the self-hosted API server
 
 Please first start the self-hosted API server by following the instructions:
 
 ```bash
-export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL
+modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
-| Model Name | Model (`MODELZ_MODEL`) | Docker Image |
+| Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
+| Bloomz 560M | `bigscience/bloomz-560m` | |
+| Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | |
+| Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
 <!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
 
-You could set the `MODELZ_MODEL` environment variables to specify the model and tokenizer.
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
```

#### html2text {}

```diff
@@ -1,38 +1,39 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.12 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.18 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
 Modelz LLM is an inference server that facilitates the utilization of open
 source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on
 either **local or cloud-based** environments with **OpenAI compatible API**. ##
 Features - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible
 API for LLMs, which means you can use the OpenAI python SDK to interact with
 the model. - **Self-hosted**: Modelz LLM can be easily deployed on either local
 or cloud-based environments. - **Open source LLMs**: Modelz LLM supports open
-source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Modelz integration**:
-Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai),
-which is a serverless inference platform for LLMs and other foundation models.
-## Quick Start ### Install ```bash pip install modelz-llm # or install from
-source pip install git+https://github.com/tensorchord/modelz-llm.git ``` ###
-Run the self-hosted API server Please first start the self-hosted API server by
-following the instructions: ```bash export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL ``` Currently, we support the following models: |
-Model Name | Model (`MODELZ_MODEL`) | Docker Image | | ---------- | ----------
-- | ---------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud native**: We
+provide docker images for different LLMs, which can be easily deployed on
+Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
+docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
+# or install from source pip install git+https://github.com/tensorchord/modelz-
+llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
+self-hosted API server by following the instructions: ```bash modelz-llm -
+m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
+Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
+-------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
-//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |  You
-could set the `MODELZ_MODEL` environment variables to specify the model and
-tokenizer. ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
+560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
+7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
 "content": "Hello world"}]) ```
```

### Comparing `modelz-llm-23.5.12/README.md` & `modelz-llm-23.5.18/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: modelz-llm
+Version: 23.5.18
+Summary: LLM unified service
+Author-email: TensorChord <modelz@tensorchord.ai>
+Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+
 <div align="center">
 
 # Modelz LLM
 
 </div>
 
 <p align=center>
@@ -12,48 +24,49 @@
 Modelz LLM is an inference server that facilitates the utilization of open source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on either **local or cloud-based** environments with **OpenAI compatible API**.
 
 ## Features
 
 - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK to interact with the model.
 - **Self-hosted**: Modelz LLM can be easily deployed on either local or cloud-based environments.
 - **Open source LLMs**: Modelz LLM supports open source LLMs, such as FastChat, LLaMA, and ChatGLM.
-- **Modelz integration**: Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai), which is a serverless inference platform for LLMs and other foundation models.
+- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://docs.modelz.ai))
 
 ## Quick Start
 
 ### Install
 
 ```bash
-pip install modelz-llm
+pip install modelz-llm[gpu]
 # or install from source
-pip install git+https://github.com/tensorchord/modelz-llm.git
+pip install git+https://github.com/tensorchord/modelz-llm.git[gpu]
 ```
 
 ### Run the self-hosted API server
 
 Please first start the self-hosted API server by following the instructions:
 
 ```bash
-export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL
+modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
-| Model Name | Model (`MODELZ_MODEL`) | Docker Image |
+| Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
+| Bloomz 560M | `bigscience/bloomz-560m` | |
+| Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | |
+| Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
 <!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
 
-You could set the `MODELZ_MODEL` environment variables to specify the model and tokenizer.
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
```

#### html2text {}

```diff
@@ -1,32 +1,39 @@
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.18 Summary: LLM unified
+service Author-email: TensorChord
+tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
+llm Classifier: Intended Audience :: Developers Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
+Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
 Modelz LLM is an inference server that facilitates the utilization of open
 source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on
 either **local or cloud-based** environments with **OpenAI compatible API**. ##
 Features - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible
 API for LLMs, which means you can use the OpenAI python SDK to interact with
 the model. - **Self-hosted**: Modelz LLM can be easily deployed on either local
 or cloud-based environments. - **Open source LLMs**: Modelz LLM supports open
-source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Modelz integration**:
-Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai),
-which is a serverless inference platform for LLMs and other foundation models.
-## Quick Start ### Install ```bash pip install modelz-llm # or install from
-source pip install git+https://github.com/tensorchord/modelz-llm.git ``` ###
-Run the self-hosted API server Please first start the self-hosted API server by
-following the instructions: ```bash export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL ``` Currently, we support the following models: |
-Model Name | Model (`MODELZ_MODEL`) | Docker Image | | ---------- | ----------
-- | ---------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud native**: We
+provide docker images for different LLMs, which can be easily deployed on
+Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
+docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
+# or install from source pip install git+https://github.com/tensorchord/modelz-
+llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
+self-hosted API server by following the instructions: ```bash modelz-llm -
+m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
+Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
+-------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
-//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |  You
-could set the `MODELZ_MODEL` environment variables to specify the model and
-tokenizer. ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
+560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
+7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
 "content": "Hello world"}]) ```
```

### Comparing `modelz-llm-23.5.12/build.envd` & `modelz-llm-23.5.18/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/images/base/Dockerfile` & `modelz-llm-23.5.18/images/base/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,16 @@
 COPY requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
-RUN pip install -e .
-
 WORKDIR /workspace
+RUN pip install -e .[gpu]
 
 RUN modelz-llm --dry-run
 
 # disable huggingface update check (could be very slow)
 ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.5.12/images/chatglm-6b/Dockerfile` & `modelz-llm-23.5.18/images/chatglm-6b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,16 @@
 COPY requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
-RUN pip install -e .
-
 WORKDIR /workspace
+RUN pip install -e .[gpu]
 
 # RUN modelz-llm --dry-run --model THUDM/chatglm-6b
 
 # # disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.5.12/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.5.18/images/fastchat-t5-3b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,16 @@
 COPY ./images/llama-7b/requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
-RUN pip install -e .
-
 WORKDIR /workspace
+RUN pip install -e .[gpu]
 
 RUN modelz-llm --dry-run --model lmsys/fastchat-t5-3b-v1.0
 
 # disable huggingface update check (could be very slow)
 ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.5.12/images/llama-7b/Dockerfile` & `modelz-llm-23.5.18/images/llama-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,16 @@
 COPY ./images/llama-7b/requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
-RUN pip install -e .
-
 WORKDIR /workspace
+RUN pip install -e .[gpu]
 
 # RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
 
 # # disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.5.12/images/vicuna-7b/Dockerfile` & `modelz-llm-23.5.18/images/vicuna-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,16 @@
 COPY ./images/llama-7b/requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
-RUN pip install -e .
-
 WORKDIR /workspace
+RUN pip install -e .[gpu]
 
 # RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
 
 # # disable huggingface update check (could be very slow)
 # ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
```

### Comparing `modelz-llm-23.5.12/pyproject.toml` & `modelz-llm-23.5.18/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -6,19 +6,27 @@
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
-    "llmspec>=0.3.3",
+    "llmspec",
     "falcon>=3",
     "uvicorn>=0.22",
     "mosec>0.6",
 ]
+[project.optional-dependencies]
+gpu = [
+    "torch",  # CUDA 11.7, ref https://pytorch.org/get-started/locally/
+    "transformers",
+    "sentencepiece",
+    "accelerate",
+    "cpm_kernels",
+]
 [project.urls]
 "Homepage" = "https://github.com/tensorchord/modelz-llm"
 [project.scripts]
 modelz-llm = "modelz_llm.cli:main"
 
 [build-system]
 requires = ["setuptools", "setuptools_scm>=7.0"]
@@ -27,10 +35,13 @@
 [tool.setuptools_scm]
 write_to = "src/modelz_llm/_version.py"
 
 [tool.ruff]
 target-version = "py38"
 line-length = 88
 select = ["E", "F", "B", "I", "SIM", "TID", "PL"]
+[tool.ruff.pylint]
+max-branches = 35
+max-statements = 100
 
 [tool.black]
 line-length = 88
```

### Comparing `modelz-llm-23.5.12/src/modelz_llm/cli.py` & `modelz-llm-23.5.18/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/src/modelz_llm/mosec_service.py` & `modelz-llm-23.5.18/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.12/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.5.18/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: modelz-llm
-Version: 23.5.12
-Summary: LLM unified service
-Author-email: TensorChord <modelz@tensorchord.ai>
-Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 <div align="center">
 
 # Modelz LLM
 
 </div>
 
 <p align=center>
@@ -23,48 +12,49 @@
 Modelz LLM is an inference server that facilitates the utilization of open source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on either **local or cloud-based** environments with **OpenAI compatible API**.
 
 ## Features
 
 - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible API for LLMs, which means you can use the OpenAI python SDK to interact with the model.
 - **Self-hosted**: Modelz LLM can be easily deployed on either local or cloud-based environments.
 - **Open source LLMs**: Modelz LLM supports open source LLMs, such as FastChat, LLaMA, and ChatGLM.
-- **Modelz integration**: Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai), which is a serverless inference platform for LLMs and other foundation models.
+- **Cloud native**: We provide docker images for different LLMs, which can be easily deployed on Kubernetes, or other cloud-based environments (e.g. [Modelz](https://docs.modelz.ai))
 
 ## Quick Start
 
 ### Install
 
 ```bash
-pip install modelz-llm
+pip install modelz-llm[gpu]
 # or install from source
-pip install git+https://github.com/tensorchord/modelz-llm.git
+pip install git+https://github.com/tensorchord/modelz-llm.git[gpu]
 ```
 
 ### Run the self-hosted API server
 
 Please first start the self-hosted API server by following the instructions:
 
 ```bash
-export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL
+modelz-llm -m "THUDM/chatglm-6b-int4"
 ```
 
 Currently, we support the following models:
 
-| Model Name | Model (`MODELZ_MODEL`) | Docker Image |
+| Model Name | Huggingface Model | Docker Image |
 | ---------- | ----------- | ---------------- |
 | Vicuna 7B Delta V1.1  | `lmsys/vicuna-7b-delta-v1.1` | [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-vicuna-7b/general) |
 | LLaMA 7B    | `decapoda-research/llama-7b-hf` | [modelzai/llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/general) |
 | ChatGLM 6B INT4    | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/general) |
 | ChatGLM 6B  | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |
+| Bloomz 560M | `bigscience/bloomz-560m` | |
+| Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | |
+| Bloomz 7.1B | `bigscience/bloomz-7b1` | |
 
 <!-- | FastChat T5 3B V1.0  | `lmsys/fastchat-t5-3b-v1.0` | `lmsys/fastchat-t5-3b-v1.0` | -->
 
-You could set the `MODELZ_MODEL` environment variables to specify the model and tokenizer.
-
 ### Use OpenAI python SDK
 
 Then you can use the OpenAI python SDK to interact with the model:
 
 ```python
 import openai
 openai.api_base="http://localhost:8000"
```

#### html2text {}

```diff
@@ -1,38 +1,33 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.12 Summary: LLM unified
-service Author-email: TensorChord
-tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
-llm Classifier: Intended Audience :: Developers Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
-Description-Content-Type: text/markdown
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
 Modelz LLM is an inference server that facilitates the utilization of open
 source large language models (LLMs), such as FastChat, LLaMA, and ChatGLM, on
 either **local or cloud-based** environments with **OpenAI compatible API**. ##
 Features - **OpenAI compatible API**: Modelz LLM provides an OpenAI compatible
 API for LLMs, which means you can use the OpenAI python SDK to interact with
 the model. - **Self-hosted**: Modelz LLM can be easily deployed on either local
 or cloud-based environments. - **Open source LLMs**: Modelz LLM supports open
-source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Modelz integration**:
-Modelz LLM can be easily integrated with [Modelz](https://docs.modelz.ai),
-which is a serverless inference platform for LLMs and other foundation models.
-## Quick Start ### Install ```bash pip install modelz-llm # or install from
-source pip install git+https://github.com/tensorchord/modelz-llm.git ``` ###
-Run the self-hosted API server Please first start the self-hosted API server by
-following the instructions: ```bash export MODELZ_MODEL="THUDM/chatglm-6b-int4"
-modelz-llm -m MODELZ_MODEL ``` Currently, we support the following models: |
-Model Name | Model (`MODELZ_MODEL`) | Docker Image | | ---------- | ----------
-- | ---------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
+source LLMs, such as FastChat, LLaMA, and ChatGLM. - **Cloud native**: We
+provide docker images for different LLMs, which can be easily deployed on
+Kubernetes, or other cloud-based environments (e.g. [Modelz](https://
+docs.modelz.ai)) ## Quick Start ### Install ```bash pip install modelz-llm[gpu]
+# or install from source pip install git+https://github.com/tensorchord/modelz-
+llm.git[gpu] ``` ### Run the self-hosted API server Please first start the
+self-hosted API server by following the instructions: ```bash modelz-llm -
+m "THUDM/chatglm-6b-int4" ``` Currently, we support the following models: |
+Model Name | Huggingface Model | Docker Image | | ---------- | ----------- | --
+-------------- | | Vicuna 7B Delta V1.1 | `lmsys/vicuna-7b-delta-v1.1` |
 [modelzai/llm-vicuna-7b](https://hub.docker.com/repository/docker/modelzai/llm-
 vicuna-7b/general) | | LLaMA 7B | `decapoda-research/llama-7b-hf` | [modelzai/
 llm-llama-7b](https://hub.docker.com/repository/docker/modelzai/llm-llama-7b/
 general) | | ChatGLM 6B INT4 | `THUDM/chatglm-6b-int4` | [modelzai/llm-chatglm-
 6b-int4](https://hub.docker.com/repository/docker/modelzai/llm-chatglm-6b-int4/
 general) | | ChatGLM 6B | `THUDM/chatglm-6b` | [modelzai/llm-chatglm-6b](https:
-//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) |  You
-could set the `MODELZ_MODEL` environment variables to specify the model and
-tokenizer. ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
+//hub.docker.com/repository/docker/modelzai/llm-chatglm-6b/general) | | Bloomz
+560M | `bigscience/bloomz-560m` | | | Bloomz 1.7B | `bigscience/bloomz-1b7` | |
+| Bloomz 3B | `bigscience/bloomz-3b` | | | Bloomz 7.1B | `bigscience/bloomz-
+7b1` | |  ### Use OpenAI python SDK Then you can use the OpenAI python SDK to
 interact with the model: ```python import openai openai.api_base="http://
 localhost:8000" openai.api_key="any" # create a chat completion chat_completion
 = openai.ChatCompletion.create(model="any", messages=[{"role": "user",
 "content": "Hello world"}]) ```
```

### Comparing `modelz-llm-23.5.12/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.5.18/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,13 +18,14 @@
 images/llama-7b/requirements.txt
 images/vicuna-7b/Dockerfile
 src/modelz_llm/__init__.py
 src/modelz_llm/_version.py
 src/modelz_llm/cli.py
 src/modelz_llm/falcon_service.py
 src/modelz_llm/mosec_service.py
+src/modelz_llm/utils.py
 src/modelz_llm.egg-info/PKG-INFO
 src/modelz_llm.egg-info/SOURCES.txt
 src/modelz_llm.egg-info/dependency_links.txt
 src/modelz_llm.egg-info/entry_points.txt
 src/modelz_llm.egg-info/requires.txt
 src/modelz_llm.egg-info/top_level.txt
```

