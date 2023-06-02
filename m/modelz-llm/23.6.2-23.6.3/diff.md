# Comparing `tmp/modelz-llm-23.6.2.tar.gz` & `tmp/modelz-llm-23.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelz-llm-23.6.2.tar", last modified: Fri Jun  2 08:02:45 2023, max compression
+gzip compressed data, was "modelz-llm-23.6.3.tar", last modified: Fri Jun  2 08:26:44 2023, max compression
```

## Comparing `modelz-llm-23.6.2.tar` & `modelz-llm-23.6.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/docker-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/gcr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/python-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/build.envd
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/base/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/base/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/chatglm-6b/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/chatglm-6b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/fastchat-t5-3b/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/fastchat-t5-3b/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/llama-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/llama-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/llama-7b/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.608945 modelz-llm-23.6.2/images/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/images/vicuna-7b/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/requirements-cpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.600945 modelz-llm-23.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/src/modelz_llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/falcon_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/mosec_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:02:30.000000 modelz-llm-23.6.2/src/modelz_llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:02:45.612945 modelz-llm-23.6.2/src/modelz_llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:02:45.000000 modelz-llm-23.6.2/src/modelz_llm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/.github/workflows/docker-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/.github/workflows/gcr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/.github/workflows/python-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/build.envd
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/images/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/base/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/images/chatglm-6b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/chatglm-6b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/images/fastchat-t5-3b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/fastchat-t5-3b/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/images/llama-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/llama-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/llama-7b/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/images/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/images/vicuna-7b/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/requirements-cpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.958179 modelz-llm-23.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/src/modelz_llm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/src/modelz_llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/src/modelz_llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15650 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/src/modelz_llm/falcon_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/src/modelz_llm/mosec_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-02 08:26:28.000000 modelz-llm-23.6.3/src/modelz_llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:26:44.962180 modelz-llm-23.6.3/src/modelz_llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 08:26:44.000000 modelz-llm-23.6.3/src/modelz_llm.egg-info/top_level.txt
```

### Comparing `modelz-llm-23.6.2/.github/workflows/docker-publish.yml` & `modelz-llm-23.6.3/.github/workflows/docker-publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,25 @@
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
+      - name: Maximize build space
+        uses: easimon/maximize-build-space@master
+        with:
+          root-reserve-mb: 512
+          swap-size-mb: 1024
+          remove-dotnet: 'true'
+          remove-haskell: 'true'
+          remove-codeql: 'true'
+          remove-docker-images: 'true'
+          remove-android: 'true'
+
       - name: Docker Login
         uses: docker/login-action@v2
         with:
           username: ${{ secrets.DOCKERIO_MODELZ_USERNAME }}
           password: ${{ secrets.DOCKERIO_MODELZ_TOKEN }}
 
       - name: Set up Docker Buildx
```

### Comparing `modelz-llm-23.6.2/.github/workflows/gcr.yml` & `modelz-llm-23.6.3/.github/workflows/gcr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,25 @@
       contents: read
       packages: write
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
+      - name: Maximize build space
+        uses: easimon/maximize-build-space@master
+        with:
+          root-reserve-mb: 512
+          swap-size-mb: 1024
+          remove-dotnet: 'true'
+          remove-haskell: 'true'
+          remove-codeql: 'true'
+          remove-docker-images: 'true'
+          remove-android: 'true'
+
       - name: Docker Login
         uses: docker/login-action@v2
         with:
           registry: us-central1-docker.pkg.dev
           username: ${{ secrets.GCR_USERNAME }}
           password: ${{ secrets.GCR_TOKEN }}
```

### Comparing `modelz-llm-23.6.2/.github/workflows/python-check.yml` & `modelz-llm-23.6.3/.github/workflows/python-check.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/.github/workflows/python-publish.yml` & `modelz-llm-23.6.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/.gitignore` & `modelz-llm-23.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/PKG-INFO` & `modelz-llm-23.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.2
+Version: 23.6.3
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.2 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.3 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.2/README.md` & `modelz-llm-23.6.3/README.md`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/build.envd` & `modelz-llm-23.6.3/build.envd`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/client.py` & `modelz-llm-23.6.3/client.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/images/base/Dockerfile` & `modelz-llm-23.6.3/images/base/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/images/chatglm-6b/Dockerfile` & `modelz-llm-23.6.3/images/chatglm-6b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/images/fastchat-t5-3b/Dockerfile` & `modelz-llm-23.6.3/images/fastchat-t5-3b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/images/llama-7b/Dockerfile` & `modelz-llm-23.6.3/images/llama-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/images/vicuna-7b/Dockerfile` & `modelz-llm-23.6.3/images/vicuna-7b/Dockerfile`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/pyproject.toml` & `modelz-llm-23.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/src/modelz_llm/cli.py` & `modelz-llm-23.6.3/src/modelz_llm/cli.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/src/modelz_llm/falcon_service.py` & `modelz-llm-23.6.3/src/modelz_llm/falcon_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/src/modelz_llm/mosec_service.py` & `modelz-llm-23.6.3/src/modelz_llm/mosec_service.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/src/modelz_llm/utils.py` & `modelz-llm-23.6.3/src/modelz_llm/utils.py`

 * *Files identical despite different names*

### Comparing `modelz-llm-23.6.2/src/modelz_llm.egg-info/PKG-INFO` & `modelz-llm-23.6.3/src/modelz_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelz-llm
-Version: 23.6.2
+Version: 23.6.3
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
-Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.2 Summary: LLM unified
+Metadata-Version: 2.1 Name: modelz-llm Version: 23.6.3 Summary: LLM unified
 service Author-email: TensorChord
 tensorchord.ai> Project-URL: Homepage, https://github.com/tensorchord/modelz-
 llm Classifier: Intended Audience :: Developers Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: gpu
                                  # Modelz LLM
                   [discord_invitation_link] [trackgit-views]
```

### Comparing `modelz-llm-23.6.2/src/modelz_llm.egg-info/SOURCES.txt` & `modelz-llm-23.6.3/src/modelz_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

