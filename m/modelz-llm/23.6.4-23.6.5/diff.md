# Comparing `tmp/modelz-llm-23.6.4.tar.gz` & `tmp/modelz-llm-23.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.4.tar", last modified: Fri Jun  2 08:32:34 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.5.tar", last modified: Fri Jun  2 08:42:08 2023, max compression
```

## Comparing `modelz-llm-23.6.4.tar` & `modelz-llm-23.6.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.069005 modelz-llm-23.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.061005 modelz-llm-23.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:32:34.069005 modelz-llm-23.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:32:34.069005 modelz-llm-23.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.065005 modelz-llm-23.6.4/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:32:33.000000 modelz-llm-23.6.4/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:32:08.000000 modelz-llm-23.6.4/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:32:34.069005 modelz-llm-23.6.4/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:32:34.000000 modelz-llm-23.6.4/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.712989 modelz-llm-23.6.5/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.708989 modelz-llm-23.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:41:49.000000 modelz-llm-23.6.5/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:42:08.716989 modelz-llm-23.6.5/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:42:08.000000 modelz-llm-23.6.5/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.4/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.5/.github/workflows/docker-publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -38,24 +38,14 @@
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
-      - name: Maximize build space
-        uses: easimon/maximize-build-space@master
-        with:
-          root-reserve-mb: 512
-          swap-size-mb: 1024
-          remove-dotnet: 'true'
-          remove-haskell: 'true'
-          remove-codeql: 'true'
-          remove-android: 'true'
-
       - name: Docker Login
         uses: docker/login-action@v2
         with:
           username: ${{ secrets.DOCKERIO_MODELZ_USERNAME }}
           password: ${{ secrets.DOCKERIO_MODELZ_TOKEN }}
 
       - name: Set up Docker Buildx
```

### Comparing `modelz-llm-23.6.4/.github/workflows/gcr.yml` & `modelz-llm-23.6.5/.github/workflows/gcr.yml`

 * *Files 10% similar despite different names*

```diff
@@ -38,24 +38,14 @@
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
-      - name: Maximize build space
-        uses: easimon/maximize-build-space@master
-        with:
-          root-reserve-mb: 512
-          swap-size-mb: 1024
-          remove-dotnet: 'true'
-          remove-haskell: 'true'
-          remove-codeql: 'true'
-          remove-android: 'true'
-
       - name: Docker Login
         uses: docker/login-action@v2
         with:
           registry: us-central1-docker.pkg.dev
           username: ${{ secrets.GCR_USERNAME }}
           password: ${{ secrets.GCR_TOKEN }}
```

### Comparing `modelz-llm-23.6.4/.github/workflows/python-check.yml` & `modelz-llm-23.6.5/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/.github/workflows/python-publish.yml` & `modelz-llm-23.6.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/.gitignore` & `modelz-llm-23.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/PKG-INFO` & `modelz-llm-23.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.4
+Version: 23.6.5
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.4 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.5 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.4/README.md` & `modelz-llm-23.6.5/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/build.envd` & `modelz-llm-23.6.5/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/client.py` & `modelz-llm-23.6.5/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/images/base/Dockerfile` & `modelz-llm-23.6.5/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.5/images/chatglm-6b/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run --model THUDM/chatglm-6b
+# RUN modelz-llm --dry-run --model THUDM/chatglm-6b
 
-# disable huggingface update check (could be very slow)
-ENV HF_HUB_OFFLINE=true
+# # disable huggingface update check (could be very slow)
+# ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b" ]
```

### Comparing `modelz-llm-23.6.4/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.5/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/images/llama-7b/Dockerfile` & `modelz-llm-23.6.5/images/llama-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
+# RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
 
-# disable huggingface update check (could be very slow)
-ENV HF_HUB_OFFLINE=true
+# # disable huggingface update check (could be very slow)
+# ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "decapoda-research/llama-7b-hf" ]
```

### Comparing `modelz-llm-23.6.4/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.5/images/vicuna-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
+# RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
 
-# disable huggingface update check (could be very slow)
-ENV HF_HUB_OFFLINE=true
+# # disable huggingface update check (could be very slow)
+# ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "lmsys/vicuna-7b-delta-v1.1" ]
```

### Comparing `modelz-llm-23.6.4/pyproject.toml` & `modelz-llm-23.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/src/modelz_llm/cli.py` & `modelz-llm-23.6.5/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.5/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.5/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/src/modelz_llm/utils.py` & `modelz-llm-23.6.5/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.4/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.5/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.4
+Version: 23.6.5
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.4 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.5 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.4/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.5/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

