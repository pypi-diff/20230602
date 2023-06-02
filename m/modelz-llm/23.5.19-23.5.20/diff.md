# Comparing `tmp/modelz-llm-23.5.19.tar.gz` & `tmp/modelz-llm-23.5.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.5.19.tar", last modified: Fri Jun  2 03:52:58 2023, max compression
+gzip compressed data, was "modelz-llm-23.5.20.tar", last modified: Fri Jun  2 04:16:33 2023, max compression
```

## Comparing `modelz-llm-23.5.19.tar` & `modelz-llm-23.5.20.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.901058 modelz-llm-23.5.19/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 03:52:44.000000 modelz-llm-23.5.19/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 03:52:58.905058 modelz-llm-23.5.19/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 03:52:58.000000 modelz-llm-23.5.19/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.030529 modelz-llm-23.5.20/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.034529 modelz-llm-23.5.20/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.034529 modelz-llm-23.5.20/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.038529 modelz-llm-23.5.20/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-02 04:16:32.000000 modelz-llm-23.5.20/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15982 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 04:16:21.000000 modelz-llm-23.5.20/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:16:33.042529 modelz-llm-23.5.20/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 04:16:33.000000 modelz-llm-23.5.20/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.5.19/.github/workflows/docker-publish.yml` & `modelz-llm-23.5.20/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/.github/workflows/gcr.yml` & `modelz-llm-23.5.20/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/.github/workflows/python-check.yml` & `modelz-llm-23.5.20/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/.github/workflows/python-publish.yml` & `modelz-llm-23.5.20/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/.gitignore` & `modelz-llm-23.5.20/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/PKG-INFO` & `modelz-llm-23.5.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.19
+Version: 23.5.20
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.19 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.20 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.5.19/README.md` & `modelz-llm-23.5.20/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/build.envd` & `modelz-llm-23.5.20/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/client.py` & `modelz-llm-23.5.20/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/images/base/Dockerfile` & `modelz-llm-23.5.20/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/images/chatglm-6b/Dockerfile` & `modelz-llm-23.5.20/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.5.20/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/images/llama-7b/Dockerfile` & `modelz-llm-23.5.20/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/images/vicuna-7b/Dockerfile` & `modelz-llm-23.5.20/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/pyproject.toml` & `modelz-llm-23.5.20/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/src/modelz_llm/cli.py` & `modelz-llm-23.5.20/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/src/modelz_llm/falcon_service.py` & `modelz-llm-23.5.20/src/modelz_llm/falcon_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,33 +42,41 @@
 logger.addHandler(sh)
 
 
 CONTEXT_LEN = 2048
 
 
 class LLM:
-    def __init__(self, model_name: str, device: str) -> None:
+    def __init__(self, model_name: str, device: str, dry_run: bool) -> None:
         self.model_name = model_name
         self.model_spec = LanguageModels.find(model_name).value
         tokenizer_cls = getattr(transformers, self.model_spec.tokenizer_cls)
-        self.tokenizer = tokenizer_cls.from_pretrained(
-            model_name, trust_remote_code=True, low_cpu_mem_usage=True
-        )
         model_cls = getattr(transformers, self.model_spec.transformer_model_cls)
-        self.model = model_cls.from_pretrained(
-            model_name, trust_remote_code=True, low_cpu_mem_usage=True
-        )
         if device == "auto":
+            self.model = model_cls.from_pretrained(
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto"
+            )
+            self.tokenizer = tokenizer_cls.from_pretrained(
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True, device_map="auto"
+            )
             self.device = (
                 torch.cuda.current_device() if torch.cuda.is_available() else "cpu"
             )
         else:
+            self.model = model_cls.from_pretrained(
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True
+            )
+            self.tokenizer = tokenizer_cls.from_pretrained(
+                model_name, trust_remote_code=True, low_cpu_mem_usage=True
+            )
             self.device = device
-        self.model = self.model.to(self.device)
-        self.model.eval()
+        
+        if not dry_run:
+            self.model = self.model.to(self.device)
+            self.model.eval()
 
     def __str__(self) -> str:
         return f"LLM(model={self.model}, tokenizer={self.tokenizer})"
 
     def token_encode(self, text: str):
         """Encode with tokenizer."""
         tokens = self.tokenizer(text, return_tensors="pt")
@@ -399,15 +407,15 @@
                 total_tokens=token_count,
             ),
         )
         resp.data = embedding_resp.to_json()
 
 
 def build_falcon_app(args: argparse.Namespace):
-    llm = LLM(args.model, args.device)
+    llm = LLM(args.model, args.device, args.dry_run)
     embeddings = Embeddings(args.emb_model, args.device)
     completion = Completions(llm)
     chat_completion = ChatCompletions(llm)
 
     if args.dry_run:
         return
```

### Comparing `modelz-llm-23.5.19/src/modelz_llm/mosec_service.py` & `modelz-llm-23.5.20/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/src/modelz_llm/utils.py` & `modelz-llm-23.5.20/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.5.19/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.5.20/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.5.19
+Version: 23.5.20
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.19 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.5.20 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.5.19/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.5.20/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

