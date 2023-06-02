# Comparing `tmp/colablib-0.1.5.dev6.tar.gz` & `tmp/colablib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colablib-0.1.5.dev6.tar", last modified: Thu Jun  1 16:36:06 2023, max compression
+gzip compressed data, was "colablib-0.1.6.tar", last modified: Fri Jun  2 07:31:39 2023, max compression
```

## Comparing `colablib-0.1.5.dev6.tar` & `colablib-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.878610 colablib-0.1.5.dev6/
--rw-rw-rw-   0        0        0      218 2023-06-01 16:36:06.877610 colablib-0.1.5.dev6/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.5.dev6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.854871 colablib-0.1.5.dev6/colablib/
--rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.5.dev6/colablib/__init__.py
--rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.5.dev6/colablib/cprint.py
--rw-rw-rw-   0        0        0     1169 2023-06-01 11:43:55.000000 colablib-0.1.5.dev6/colablib/deb_utils.py
--rw-rw-rw-   0        0        0     2408 2023-06-01 09:46:58.000000 colablib-0.1.5.dev6/colablib/git_utils.py
--rw-rw-rw-   0        0        0     3799 2023-06-01 16:34:44.000000 colablib-0.1.5.dev6/colablib/model_downloader.py
--rw-rw-rw-   0        0        0     8696 2023-06-01 14:17:34.000000 colablib-0.1.5.dev6/colablib/model_validators.py
--rw-rw-rw-   0        0        0     3330 2023-06-01 12:22:37.000000 colablib-0.1.5.dev6/colablib/py_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 16:36:06.877610 colablib-0.1.5.dev6/colablib.egg-info/
--rw-rw-rw-   0        0        0      218 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 16:36:06.000000 colablib-0.1.5.dev6/colablib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 16:36:06.879613 colablib-0.1.5.dev6/setup.cfg
--rw-rw-rw-   0        0        0      316 2023-06-01 16:35:05.000000 colablib-0.1.5.dev6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/
+-rw-rw-rw-   0        0        0      213 2023-06-02 07:31:39.142990 colablib-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-06-01 08:34:56.000000 colablib-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.123374 colablib-0.1.6/colablib/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/__init__.py
+-rw-rw-rw-   0        0        0     1127 2023-06-01 09:15:56.000000 colablib-0.1.6/colablib/colored_print.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/colablib/sd_models/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/sd_models/__init__.py
+-rw-rw-rw-   0        0        0     3752 2023-06-02 05:08:40.000000 colablib-0.1.6/colablib/sd_models/downloader.py
+-rw-rw-rw-   0        0        0     9083 2023-06-02 06:32:59.000000 colablib-0.1.6/colablib/sd_models/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.142990 colablib-0.1.6/colablib/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-01 08:53:08.000000 colablib-0.1.6/colablib/utils/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-06-02 07:15:23.000000 colablib-0.1.6/colablib/utils/git_utils.py
+-rw-rw-rw-   0        0        0     3338 2023-06-02 07:15:25.000000 colablib-0.1.6/colablib/utils/py_utils.py
+-rw-rw-rw-   0        0        0     1180 2023-06-02 03:58:41.000000 colablib-0.1.6/colablib/utils/ubuntu_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 07:31:39.134917 colablib-0.1.6/colablib.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-06-02 07:31:39.000000 colablib-0.1.6/colablib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-02 07:31:38.000000 colablib-0.1.6/colablib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-02 07:31:39.142990 colablib-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      311 2023-06-02 07:31:30.000000 colablib-0.1.6/setup.py
```

### Comparing `colablib-0.1.5.dev6/colablib/cprint.py` & `colablib-0.1.6/colablib/colored_print.py`

 * *Files identical despite different names*

### Comparing `colablib-0.1.5.dev6/colablib/deb_utils.py` & `colablib-0.1.6/colablib/utils/ubuntu_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import zipfile
 import subprocess
 import requests
 import shutil
 from .py_utils import get_filename
 from tqdm import tqdm
-from .cprint import cprint
+from ..colored_print import cprint
 
 def ubuntu_deps(url, dst, desc=None):
     """
     Downloads, extracts, and installs .deb files from a given URL.
 
     Args:
         url (str): The URL to download the .deb files from.
@@ -25,15 +25,15 @@
         for chunk in response.iter_content(chunk_size=8192):
             file.write(chunk)
             
     with zipfile.ZipFile(filename, "r") as deps:
         deps.extractall(dst)
 
     if desc is None:
-        desc = cprint("Installing", color="green", tqdm_desc=True)
+        desc = cprint("Installing...", color="green", tqdm_desc=True)
 
     deb_files = [os.path.join(dst, f) for f in os.listdir(dst) if f.endswith('.deb')]
     for deb_file in tqdm(deb_files, desc=desc):
         os.system(f'dpkg -i {deb_file}')
         
     os.remove(filename)
     shutil.rmtree(dst)
```

### Comparing `colablib-0.1.5.dev6/colablib/git_utils.py` & `colablib-0.1.6/colablib/utils/git_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import subprocess
 import sys
-from .cprint import cprint
+from ..colored_print import cprint
 
 def clone_repo(url, directory=None, branch=None, commit_hash=None):
     """
     Clones a Git repository.
 
     Args:
         url (str): The URL of the Git repository.
```

### Comparing `colablib-0.1.5.dev6/colablib/model_downloader.py` & `colablib-0.1.6/colablib/sd_models/downloader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import subprocess
 import gdown
 import os
 import glob
 from pathlib import Path
-from .cprint import cprint
-from .py_utils import get_filename
-
-hf_token = "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"
-user_header = f"Authorization: Bearer {hf_token}"
+from ..colored_print import cprint
+from ..utils.py_utils import get_filename
 
 def get_supported_extensions():
     return tuple([".ckpt", ".safetensors", ".pt", ".pth"])
 
 def parse_args(config):
     args = []
 
@@ -67,27 +64,27 @@
             cprint(f"Filename obtained: {filename}", color="green")
         return filename
     else:
         if not quiet:
             cprint(f"Failed to obtain filename.", color="green")
         return None
     
-def download(url, dst):
+def download(url, dst, user_header=None):
     filename    = get_modelname(url, quiet=False)
 
     if "drive.google.com" in url:
         gdown_download(url, dst)
     elif url.startswith("/content/drive/MyDrive/"):
         filepath = os.path.join(dst, filename)
         Path(filepath).write_bytes(Path(url).read_bytes())
     else:
         if "huggingface.co" in url:
             if "/blob/" in url:
                 url = url.replace("/blob/", "/resolve/")
-        aria2_download(dst, filename, url)
+        aria2_download(dst, filename, url, user_header=user_header)
 
 def get_most_recent_file(directory):
     extensions = get_supported_extensions()
     cprint(f"Getting filename from most recent file...", color="green")
     
     files = glob.glob(os.path.join(directory, "*"))
     if not files:
```

### Comparing `colablib-0.1.5.dev6/colablib/model_validators.py` & `colablib-0.1.6/colablib/sd_models/validators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import gc
 import torch
 import json
 import hashlib
-from torch import load
 from safetensors.torch import load_file, safe_open
-from .cprint import cprint
+from ..colored_print import cprint
 
 class Validator:
     """
     Validator is a helper class for validating models, vae, and lora. 
     It provides utility methods for checking and loading different types of files.
     """
 
@@ -33,37 +32,39 @@
 
     @staticmethod
     def validate_model(model_path, map_location="cpu"):
         """
         Validates the model by attempting to load it.
         """
         if Validator.is_safetensors(model_path):
-            return Validator._attempt_load(model_path, load_file, map_location, ".ckpt")
+            try:
+                tmp = load_file(model_path, device=map_location)
+                del tmp
+                gc.collect()
+                torch.cuda.empty_cache()
+            except Exception as e:
+                print(e)
+                new_model_path = os.path.splitext(model_path)[0] + ".ckpt"
+                os.rename(model_path, new_model_path)
+                cprint(f"Model Info: model renamed to {os.path.basename(new_model_path)}", color="green")
+                return new_model_path
         elif Validator.is_ckpt(model_path):
-            return Validator._attempt_load(model_path, load, map_location, ".safetensors")
-        else:
-            return None
-
-    @staticmethod
-    def _attempt_load(model_path, load_func, map_location, new_ext):
-        """
-        Attempts to load a model given a specific load function, map location, and new extension.
-        """
-        try:
-            tmp = load_func(model_path, device=map_location)
-            del tmp
-            gc.collect()
-            torch.cuda.empty_cache()
-        except Exception:
-            new_model_path = os.path.splitext(model_path)[0] + new_ext
-            os.rename(model_path, new_model_path)
-            cprint(f"Model Info: model renamed to {os.path.basename(new_model_path)}", color="green")
-            return new_model_path
+            try:
+                tmp = torch.load(model_path, map_location=map_location)
+                del tmp
+                gc.collect()
+                torch.cuda.empty_cache()
+            except Exception as e:
+                cprint(e)
+                new_model_path = os.path.splitext(model_path)[0] + ".safetensors"
+                os.rename(model_path, new_model_path)
+                cprint(e, f"Model Info: model renamed to {os.path.basename(new_model_path)}", color="green")
+                return new_model_path
         return None
-
+    
     @staticmethod
     def validate_vae(vae_path):
         """
         Validates the vae by checking if its sha256 hash is in the expected hash list.
         """
         expected_hash = {
             'Animevae'                                : 'f921fb3f29891d2a77a6571e56b8b5052420d2884129517a333c60b1b4816cdf',
@@ -127,14 +128,19 @@
                             "alpha"     : lora_alpha,
                             "conv_dim"  : lora_conv_dim,
                             "conv_alpha": lora_conv_alpha,
                             "algo"      : lora_algo,
                             "unit"      : lora_unit,
                         }
 
+                        json_output_path = os.path.splitext(lora_path)[0] + '.json'
+
+                        with open(json_output_path, 'w') as outfile:
+                            json.dump(data_dict, outfile, indent=4)
+
                         output_list = [f"{key}: {value}" for key, value in data_dict.items() if value is not None]
                         
                         del metadata
                         return (True, f"LoRA Info: {output_list}")
                     elif lora_d8ahazard is not None:
                         del metadata
                         return (False, "LoRA Info: LoRA is not trained using 'kohya-ss/sd-scripts' but using 'd8ahazard/sd_dreambooth_extension'")
```

### Comparing `colablib-0.1.5.dev6/colablib/py_utils.py` & `colablib-0.1.6/colablib/utils/py_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 import requests
 import subprocess
 import sys
 import time 
 from urllib.parse import urlparse, unquote
-from .cprint import cprint
+from ..colored_print import cprint
 
 def is_google_colab():
     """
     Checks if the current environment is Google Colab.
 
     Returns:
         bool: True if it's Google Colab, False otherwise.
```

