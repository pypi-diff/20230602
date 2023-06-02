# Comparing `tmp/blockwise-parallel-transformer-0.1.1.tar.gz` & `tmp/blockwise-parallel-transformer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockwise-parallel-transformer-0.1.1.tar", last modified: Fri Jun  2 04:30:25 2023, max compression
+gzip compressed data, was "blockwise-parallel-transformer-0.3.2.tar", last modified: Fri Jun  2 01:14:31 2023, max compression
```

## Comparing `blockwise-parallel-transformer-0.1.1.tar` & `blockwise-parallel-transformer-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:30:25.163983 blockwise-parallel-transformer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-02 04:30:25.163983 blockwise-parallel-transformer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:30:25.163983 blockwise-parallel-transformer-0.1.1/blockwise_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel/blockwise_paralle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel/jax_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel/test1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:30:25.163983 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-02 04:30:25.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 04:30:25.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:30:25.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 04:30:25.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 04:30:25.000000 blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 04:30:25.163983 blockwise-parallel-transformer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-02 04:30:08.000000 blockwise-parallel-transformer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:31.228430 blockwise-parallel-transformer-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-02 01:14:31.228430 blockwise-parallel-transformer-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:31.224430 blockwise-parallel-transformer-0.3.2/blockwise_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel/blockwise_paralle.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel/jax_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:14:31.228430 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-02 01:14:31.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-02 01:14:31.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:14:31.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 01:14:31.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 01:14:31.000000 blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:14:31.228430 blockwise-parallel-transformer-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-02 01:14:20.000000 blockwise-parallel-transformer-0.3.2/setup.py
```

### Comparing `blockwise-parallel-transformer-0.1.1/LICENSE` & `blockwise-parallel-transformer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `blockwise-parallel-transformer-0.1.1/PKG-INFO` & `blockwise-parallel-transformer-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockwise-parallel-transformer
-Version: 0.1.1
+Version: 0.3.2
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/Blockwise-Parallel-Transformer
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `blockwise-parallel-transformer-0.1.1/README.md` & `blockwise-parallel-transformer-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,12 +95,12 @@
 
 [Whatsapp](https://api.whatsapp.com/send?text=Check%20out%20this%20PyTorch%20implementation%20of%20the%20Blockwise%20Parallel%20Transformer%20Attention%20module%20for%20efficiently%20handling%20long%20sequences%20in%20deep%20learning%20models%21%20https%3A%2F%2Fgithub.com%2Fkyegomez%2FBlockwise-Parallel-Transformer)
 
 
 # Roadmap
 * Pytorch Implementation
 
-* Reproduce Training and Experiment suite in paper
+* Reproduce 
 
 * Jax Implementation
 
 * Triton Implementation
```

### Comparing `blockwise-parallel-transformer-0.1.1/blockwise_parallel/blockwise_paralle.py` & `blockwise-parallel-transformer-0.3.2/blockwise_parallel/blockwise_paralle.py`

 * *Files identical despite different names*

### Comparing `blockwise-parallel-transformer-0.1.1/blockwise_parallel/test1.py` & `blockwise-parallel-transformer-0.3.2/blockwise_parallel/test1.py`

 * *Files identical despite different names*

### Comparing `blockwise-parallel-transformer-0.1.1/blockwise_parallel_transformer.egg-info/PKG-INFO` & `blockwise-parallel-transformer-0.3.2/blockwise_parallel_transformer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockwise-parallel-transformer
-Version: 0.1.1
+Version: 0.3.2
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/Blockwise-Parallel-Transformer
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `blockwise-parallel-transformer-0.1.1/setup.py` & `blockwise-parallel-transformer-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'blockwise-parallel-transformer',
   packages = find_packages(exclude=[]),
-  version = '0.1.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/Blockwise-Parallel-Transformer',
   keywords = [
```

