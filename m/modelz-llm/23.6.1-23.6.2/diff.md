# Comparing `tmp/modelz-llm-23.6.1.tar.gz` & `tmp/modelz-llm-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.1.tar", last modified: Fri Jun  2 07:37:49 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.2.tar", last modified: Fri Jun  2 08:02:45 2023, max compression
```

## Comparing `modelz-llm-23.6.1.tar` & `modelz-llm-23.6.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.938464 modelz-llm-23.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.938464 modelz-llm-23.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.938464 modelz-llm-23.6.1/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.938464 modelz-llm-23.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 07:37:38.000000 modelz-llm-23.6.1/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:37:49.942464 modelz-llm-23.6.1/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 07:37:49.000000 modelz-llm-23.6.1/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.1/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.2/.github/workflows/docker-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/.github/workflows/gcr.yml` & `modelz-llm-23.6.2/.github/workflows/gcr.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/.github/workflows/python-check.yml` & `modelz-llm-23.6.2/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/.github/workflows/python-publish.yml` & `modelz-llm-23.6.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/.gitignore` & `modelz-llm-23.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/PKG-INFO` & `modelz-llm-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.1
+Version: 23.6.2
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.1 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.2 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.1/README.md` & `modelz-llm-23.6.2/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/build.envd` & `modelz-llm-23.6.2/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/client.py` & `modelz-llm-23.6.2/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/images/base/Dockerfile` & `modelz-llm-23.6.2/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.2/images/chatglm-6b/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model THUDM/chatglm-6b
+RUN modelz-llm --dry-run --model THUDM/chatglm-6b
 
-# # disable huggingface update check (could be very slow)
-# ENV HF_HUB_OFFLINE=true
+# disable huggingface update check (could be very slow)
+ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "THUDM/chatglm-6b" ]
```

### Comparing `modelz-llm-23.6.1/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.2/images/fastchat-t5-3b/Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ENV ENVD_PREFIX=/opt/conda/envs/envd/bin
 
 RUN update-alternatives --install /usr/bin/python python ${ENVD_PREFIX}/python 1 && \
     update-alternatives --install /usr/bin/python3 python3 ${ENVD_PREFIX}/python3 1 && \
     update-alternatives --install /usr/bin/pip pip ${ENVD_PREFIX}/pip 1 && \
     update-alternatives --install /usr/bin/pip3 pip3 ${ENVD_PREFIX}/pip3 1
 
-COPY ./images/llama-7b/requirements.txt /
+COPY /requirements.txt /
 
 RUN pip install -r requirements.txt
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
```

### Comparing `modelz-llm-23.6.1/images/llama-7b/Dockerfile` & `modelz-llm-23.6.2/images/llama-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
+RUN modelz-llm --dry-run --model decapoda-research/llama-7b-hf
 
-# # disable huggingface update check (could be very slow)
-# ENV HF_HUB_OFFLINE=true
+# disable huggingface update check (could be very slow)
+ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "decapoda-research/llama-7b-hf" ]
```

### Comparing `modelz-llm-23.6.1/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.2/images/vicuna-7b/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,14 @@
 
 RUN mkdir -p /workspace
 
 COPY . workspace/
 WORKDIR /workspace
 RUN pip install -e .[gpu]
 
-# RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
+RUN modelz-llm --dry-run --model lmsys/vicuna-7b-delta-v1.1
 
-# # disable huggingface update check (could be very slow)
-# ENV HF_HUB_OFFLINE=true
+# disable huggingface update check (could be very slow)
+ENV HF_HUB_OFFLINE=true
 
 ENTRYPOINT [ "modelz-llm" ]
 CMD [ "--port", "8080", "--model", "lmsys/vicuna-7b-delta-v1.1" ]
```

### Comparing `modelz-llm-23.6.1/pyproject.toml` & `modelz-llm-23.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/src/modelz_llm/cli.py` & `modelz-llm-23.6.2/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.2/src/modelz_llm/falcon_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
         resp.data = embedding_resp.to_json()
 
 
 def build_falcon_app(args: argparse.Namespace):
     if args.dry_run:
         snapshot_download(repo_id=args.model)
         return
-    llm = LLM(args.model, args.device, args.dry_run)
+    llm = LLM(args.model, args.device)
     embeddings = Embeddings(args.emb_model, args.device)
     completion = Completions(llm)
     chat_completion = ChatCompletions(llm)
     app = App()
     app.add_route("/", Ping())
     app.add_route("/completions", completion)
     app.add_route("/chat/completions", chat_completion)
```

### Comparing `modelz-llm-23.6.1/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.2/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/src/modelz_llm/utils.py` & `modelz-llm-23.6.2/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.1/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.2/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.1
+Version: 23.6.2
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.1 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.2 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.1/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.2/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

