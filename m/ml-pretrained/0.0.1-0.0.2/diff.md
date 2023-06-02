# Comparing `tmp/ml-pretrained-0.0.1.tar.gz` & `tmp/ml-pretrained-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-pretrained-0.0.1.tar", last modified: Fri Jun  2 05:02:24 2023, max compression
+gzip compressed data, was "ml-pretrained-0.0.2.tar", last modified: Fri Jun  2 05:13:27 2023, max compression
```

## Comparing `ml-pretrained-0.0.1.tar` & `ml-pretrained-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ck         (501) staff       (20)        0 2023-06-02 05:02:24.439438 ml-pretrained-0.0.1/
--rw-r--r--   0 ck         (501) staff       (20)      102 2023-06-02 01:59:28.000000 ml-pretrained-0.0.1/MANIFEST.in
--rw-r--r--   0 ck         (501) staff       (20)     2108 2023-06-02 05:02:24.439533 ml-pretrained-0.0.1/PKG-INFO
--rw-r--r--   0 ck         (501) staff       (20)     1570 2023-06-02 03:43:48.000000 ml-pretrained-0.0.1/README.md
-drwxr-xr-x   0 ck         (501) staff       (20)        0 2023-06-02 05:02:24.427355 ml-pretrained-0.0.1/ml_pretrained.egg-info/
--rw-r--r--   0 ck         (501) staff       (20)     2108 2023-06-02 05:02:24.000000 ml-pretrained-0.0.1/ml_pretrained.egg-info/PKG-INFO
--rw-r--r--   0 ck         (501) staff       (20)      537 2023-06-02 05:02:24.000000 ml-pretrained-0.0.1/ml_pretrained.egg-info/SOURCES.txt
--rw-r--r--   0 ck         (501) staff       (20)        1 2023-06-02 05:02:24.000000 ml-pretrained-0.0.1/ml_pretrained.egg-info/dependency_links.txt
--rw-r--r--   0 ck         (501) staff       (20)       59 2023-06-02 05:02:24.000000 ml-pretrained-0.0.1/ml_pretrained.egg-info/requires.txt
--rw-r--r--   0 ck         (501) staff       (20)       11 2023-06-02 05:02:24.000000 ml-pretrained-0.0.1/ml_pretrained.egg-info/top_level.txt
-drwxr-xr-x   0 ck         (501) staff       (20)        0 2023-06-02 05:02:24.434538 ml-pretrained-0.0.1/pretrained/
--rw-r--r--   0 ck         (501) staff       (20)       22 2023-06-02 03:54:38.000000 ml-pretrained-0.0.1/pretrained/__init__.py
--rw-r--r--   0 ck         (501) staff       (20)    16681 2023-06-02 02:08:26.000000 ml-pretrained-0.0.1/pretrained/blip.py
--rw-r--r--   0 ck         (501) staff       (20)    40892 2023-06-02 02:08:33.000000 ml-pretrained-0.0.1/pretrained/clip.py
--rw-r--r--   0 ck         (501) staff       (20)    26309 2023-06-02 02:08:42.000000 ml-pretrained-0.0.1/pretrained/hubert.py
--rw-r--r--   0 ck         (501) staff       (20)    22229 2023-06-02 02:08:58.000000 ml-pretrained-0.0.1/pretrained/llama.py
--rw-r--r--   0 ck         (501) staff       (20)    14935 2023-06-02 02:08:09.000000 ml-pretrained-0.0.1/pretrained/rwkv.py
--rw-r--r--   0 ck         (501) staff       (20)    60932 2023-06-02 04:31:17.000000 ml-pretrained-0.0.1/pretrained/sam.py
--rw-r--r--   0 ck         (501) staff       (20)    46647 2023-06-02 04:37:44.000000 ml-pretrained-0.0.1/pretrained/tacotron2.py
-drwxr-xr-x   0 ck         (501) staff       (20)        0 2023-06-02 05:02:24.438089 ml-pretrained-0.0.1/pretrained/vocoder/
--rw-r--r--   0 ck         (501) staff       (20)      922 2023-06-02 01:58:23.000000 ml-pretrained-0.0.1/pretrained/vocoder/__init__.py
--rw-r--r--   0 ck         (501) staff       (20)     9220 2023-06-02 02:10:01.000000 ml-pretrained-0.0.1/pretrained/vocoder/hifigan.py
--rw-r--r--   0 ck         (501) staff       (20)    13020 2023-06-02 02:10:15.000000 ml-pretrained-0.0.1/pretrained/vocoder/waveglow.py
--rw-r--r--   0 ck         (501) staff       (20)     1641 2023-06-02 02:06:52.000000 ml-pretrained-0.0.1/pyproject.toml
--rw-r--r--   0 ck         (501) staff       (20)      127 2023-06-02 05:02:24.440424 ml-pretrained-0.0.1/setup.cfg
--rw-r--r--   0 ck         (501) staff       (20)     1255 2023-06-02 03:46:22.000000 ml-pretrained-0.0.1/setup.py
-drwxr-xr-x   0 ck         (501) staff       (20)        0 2023-06-02 05:02:24.438829 ml-pretrained-0.0.1/tests/
--rw-r--r--   0 ck         (501) staff       (20)     2160 2023-06-02 04:46:37.000000 ml-pretrained-0.0.1/tests/test_rwkv.py
--rw-r--r--   0 ck         (501) staff       (20)      538 2023-06-02 04:37:53.000000 ml-pretrained-0.0.1/tests/test_tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.887265 ml-pretrained-0.0.2/ml_pretrained.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-02 05:13:27.000000 ml-pretrained-0.0.2/ml_pretrained.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/pretrained/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/blip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40892 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26309 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/hubert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60932 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46647 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/tacotron2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/pretrained/vocoder/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/hifigan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pretrained/vocoder/waveglow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:13:27.891265 ml-pretrained-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/tests/test_rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-02 05:13:10.000000 ml-pretrained-0.0.2/tests/test_tacotron2.py
```

### Comparing `ml-pretrained-0.0.1/PKG-INFO` & `ml-pretrained-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.1/README.md` & `ml-pretrained-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/ml_pretrained.egg-info/PKG-INFO` & `ml-pretrained-0.0.2/ml_pretrained.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-pretrained
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-pretrained
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-pretrained-0.0.1/ml_pretrained.egg-info/SOURCES.txt` & `ml-pretrained-0.0.2/ml_pretrained.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/blip.py` & `ml-pretrained-0.0.2/pretrained/blip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/clip.py` & `ml-pretrained-0.0.2/pretrained/clip.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/hubert.py` & `ml-pretrained-0.0.2/pretrained/hubert.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/llama.py` & `ml-pretrained-0.0.2/pretrained/llama.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/rwkv.py` & `ml-pretrained-0.0.2/pretrained/rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/sam.py` & `ml-pretrained-0.0.2/pretrained/sam.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/tacotron2.py` & `ml-pretrained-0.0.2/pretrained/tacotron2.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/vocoder/__init__.py` & `ml-pretrained-0.0.2/pretrained/vocoder/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/vocoder/hifigan.py` & `ml-pretrained-0.0.2/pretrained/vocoder/hifigan.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pretrained/vocoder/waveglow.py` & `ml-pretrained-0.0.2/pretrained/vocoder/waveglow.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/pyproject.toml` & `ml-pretrained-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/setup.py` & `ml-pretrained-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/tests/test_rwkv.py` & `ml-pretrained-0.0.2/tests/test_rwkv.py`

 * *Files identical despite different names*

### Comparing `ml-pretrained-0.0.1/tests/test_tacotron2.py` & `ml-pretrained-0.0.2/tests/test_tacotron2.py`

 * *Files identical despite different names*

