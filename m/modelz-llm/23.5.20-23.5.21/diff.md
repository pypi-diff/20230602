# Comparing `tmp/modelz-llm-23.5.20.tar.gz` & `tmp/modelz-llm-23.5.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.5.20.tar", last modified: Fri Jun  2 04:16:33 2023, max compression
+gzip compressed data, was "modelz-llm-23.5.21.tar", last modified: Fri Jun  2 04:26:44 2023, max compression
```

## Comparing `modelz-llm-23.5.20.tar` & `modelz-llm-23.5.21.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.030529 modelz-llm-23.5.20/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.034529 modelz-llm-23.5.20/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.034529 modelz-llm-23.5.20/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 04:16:32.000000 modelz-llm-23.5.20/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.880175 modelz-llm-23.5.21/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:26:44.880175 modelz-llm-23.5.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:26:44.880175 modelz-llm-23.5.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.876175 modelz-llm-23.5.21/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.880175 modelz-llm-23.5.21/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 04:26:33.000000 modelz-llm-23.5.21/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:26:44.880175 modelz-llm-23.5.21/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 04:26:44.000000 modelz-llm-23.5.21/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.5.20/.github/workflows/docker-publish.yml` & `modelz-llm-23.5.21/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/.github/workflows/gcr.yml` & `modelz-llm-23.5.21/.github/workflows/gcr.yml`

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

### Comparing `modelz-llm-23.5.20/.github/workflows/python-check.yml` & `modelz-llm-23.5.21/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/.github/workflows/python-publish.yml` & `modelz-llm-23.5.21/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/.gitignore` & `modelz-llm-23.5.21/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/PKG-INFO` & `modelz-llm-23.5.21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.20
+Version: 23.5.21
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.20 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.21 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.5.20/README.md` & `modelz-llm-23.5.21/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/build.envd` & `modelz-llm-23.5.21/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/client.py` & `modelz-llm-23.5.21/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/images/base/Dockerfile` & `modelz-llm-23.5.21/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/images/chatglm-6b/Dockerfile` & `modelz-llm-23.5.21/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.5.21/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/images/llama-7b/Dockerfile` & `modelz-llm-23.5.21/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/images/vicuna-7b/Dockerfile` & `modelz-llm-23.5.21/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/pyproject.toml` & `modelz-llm-23.5.21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/src/modelz_llm/cli.py` & `modelz-llm-23.5.21/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/src/modelz_llm/falcon_service.py` & `modelz-llm-23.5.21/src/modelz_llm/falcon_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,18 +49,18 @@
     def __init__(self, model_name: str, device: str, dry_run: bool) -> None:
         self.model_name = model_name
         self.model_spec = LanguageModels.find(model_name).value
         tokenizer_cls = getattr(transformers, self.model_spec.tokenizer_cls)
         model_cls = getattr(transformers, self.model_spec.transformer_model_cls)
         if device == "auto":
             self.model = model_cls.from_pretrained(
-                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto"
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto", offload_folder="/tmp/model-offload"
             )
             self.tokenizer = tokenizer_cls.from_pretrained(
-                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto"
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto", offload_folder="/tmp/tokenizer-offload"
             )
             self.device = (
                 torch.cuda.current_device() if torch.cuda.is_available() else "cpu"
             )
         else:
             self.model = model_cls.from_pretrained(
                 model_name, trust_remote_code=True, low_cpu_mem_usage=True
```

### Comparing `modelz-llm-23.5.20/src/modelz_llm/mosec_service.py` & `modelz-llm-23.5.21/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/src/modelz_llm/utils.py` & `modelz-llm-23.5.21/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.20/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.5.21/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.20
+Version: 23.5.21
 Summary: LLM unified service
 Author-email: TensorChord <modelz@tensorchord.ai>
 Project-URL: Homepage, https://github.com/tensorchord/modelz-llm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.20 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.21 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.5.20/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.5.21/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

