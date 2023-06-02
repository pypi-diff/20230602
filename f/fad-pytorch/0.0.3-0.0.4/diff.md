# Comparing `tmp/fad_pytorch-0.0.3.tar.gz` & `tmp/fad_pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fad_pytorch-0.0.3.tar", last modified: Wed May 31 23:03:54 2023, max compression
+gzip compressed data, was "fad_pytorch-0.0.4.tar", last modified: Fri Jun  2 01:22:54 2023, max compression
```

## Comparing `fad_pytorch-0.0.3.tar` & `fad_pytorch-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.043086 fad_pytorch-0.0.3/
--rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/LICENSE
--rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/MANIFEST.in
--rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-31 23:03:54.042942 fad_pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)     1488 2023-05-25 07:08:29.000000 fad_pytorch-0.0.3/README.md
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.041853 fad_pytorch-0.0.3/fad_pytorch/
--rw-r--r--   0 shawley    (501) staff       (20)       22 2023-05-31 21:26:13.000000 fad_pytorch-0.0.3/fad_pytorch/__init__.py
--rw-r--r--   0 shawley    (501) staff       (20)    31046 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/_modidx.py
--rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/fad_pytorch/core.py
--rw-r--r--   0 shawley    (501) staff       (20)    12366 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_embed.py
--rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_gen.py
--rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/fad_score.py
--rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/pann.py
--rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.3/fad_pytorch/pann_pytorch_utils.py
--rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/fad_pytorch/sqrtm.py
-drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-05-31 23:03:54.042769 fad_pytorch-0.0.3/fad_pytorch.egg-info/
--rw-r--r--   0 shawley    (501) staff       (20)     2290 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 shawley    (501) staff       (20)      512 2023-05-31 23:03:54.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 shawley    (501) staff       (20)      176 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/entry_points.txt
--rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/not-zip-safe
--rw-r--r--   0 shawley    (501) staff       (20)       81 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/requires.txt
--rw-r--r--   0 shawley    (501) staff       (20)       12 2023-05-31 23:03:53.000000 fad_pytorch-0.0.3/fad_pytorch.egg-info/top_level.txt
--rw-r--r--   0 shawley    (501) staff       (20)     1144 2023-05-31 21:21:07.000000 fad_pytorch-0.0.3/settings.ini
--rw-r--r--   0 shawley    (501) staff       (20)       38 2023-05-31 23:03:54.043126 fad_pytorch-0.0.3/setup.cfg
--rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.3/setup.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.906273 fad_pytorch-0.0.4/
+-rw-r--r--   0 shawley    (501) staff       (20)     1072 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/LICENSE
+-rw-r--r--   0 shawley    (501) staff       (20)      111 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/MANIFEST.in
+-rw-r--r--   0 shawley    (501) staff       (20)     3998 2023-06-02 01:22:54.906129 fad_pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)     3196 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/README.md
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.905030 fad_pytorch-0.0.4/fad_pytorch/
+-rw-r--r--   0 shawley    (501) staff       (20)       22 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/fad_pytorch/__init__.py
+-rw-r--r--   0 shawley    (501) staff       (20)    31274 2023-06-01 23:44:14.000000 fad_pytorch-0.0.4/fad_pytorch/_modidx.py
+-rw-r--r--   0 shawley    (501) staff       (20)      142 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/fad_pytorch/core.py
+-rw-r--r--   0 shawley    (501) staff       (20)    16610 2023-06-02 01:22:48.000000 fad_pytorch-0.0.4/fad_pytorch/fad_embed.py
+-rw-r--r--   0 shawley    (501) staff       (20)     4423 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/fad_gen.py
+-rw-r--r--   0 shawley    (501) staff       (20)     3773 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/fad_score.py
+-rw-r--r--   0 shawley    (501) staff       (20)   123697 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/pann.py
+-rw-r--r--   0 shawley    (501) staff       (20)     9559 2023-05-25 06:50:08.000000 fad_pytorch-0.0.4/fad_pytorch/pann_pytorch_utils.py
+-rw-r--r--   0 shawley    (501) staff       (20)     8474 2023-05-31 21:21:07.000000 fad_pytorch-0.0.4/fad_pytorch/sqrtm.py
+drwxr-xr-x   0 shawley    (501) staff       (20)        0 2023-06-02 01:22:54.905966 fad_pytorch-0.0.4/fad_pytorch.egg-info/
+-rw-r--r--   0 shawley    (501) staff       (20)     3998 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 shawley    (501) staff       (20)      512 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 shawley    (501) staff       (20)      176 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/entry_points.txt
+-rw-r--r--   0 shawley    (501) staff       (20)        1 2023-05-24 22:59:30.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/not-zip-safe
+-rw-r--r--   0 shawley    (501) staff       (20)       93 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/requires.txt
+-rw-r--r--   0 shawley    (501) staff       (20)       12 2023-06-02 01:22:54.000000 fad_pytorch-0.0.4/fad_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 shawley    (501) staff       (20)     1274 2023-06-02 01:22:48.000000 fad_pytorch-0.0.4/settings.ini
+-rw-r--r--   0 shawley    (501) staff       (20)       38 2023-06-02 01:22:54.906311 fad_pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 shawley    (501) staff       (20)     2596 2023-05-24 22:59:09.000000 fad_pytorch-0.0.4/setup.py
```

### Comparing `fad_pytorch-0.0.3/LICENSE` & `fad_pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch/_modidx.py` & `fad_pytorch-0.0.4/fad_pytorch/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/fad_pytorch',
                 'doc_host': 'https://drscotthawley.github.io',
                 'git_url': 'https://github.com/drscotthawley/fad_pytorch',
                 'lib_path': 'fad_pytorch'},
   'syms': { 'fad_pytorch.core': {'fad_pytorch.core.foo': ('core.html#foo', 'fad_pytorch/core.py')},
             'fad_pytorch.fad_embed': { 'fad_pytorch.fad_embed.download_file': ('fad_embed.html#download_file', 'fad_pytorch/fad_embed.py'),
-                                       'fad_pytorch.fad_embed.embed_all': ('fad_embed.html#embed_all', 'fad_pytorch/fad_embed.py'),
+                                       'fad_pytorch.fad_embed.download_if_needed': ( 'fad_embed.html#download_if_needed',
+                                                                                     'fad_pytorch/fad_embed.py'),
+                                       'fad_pytorch.fad_embed.embed': ('fad_embed.html#embed', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.get_ckpt': ('fad_embed.html#get_ckpt', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.main': ('fad_embed.html#main', 'fad_pytorch/fad_embed.py'),
                                        'fad_pytorch.fad_embed.setup_embedder': ( 'fad_embed.html#setup_embedder',
                                                                                  'fad_pytorch/fad_embed.py')},
             'fad_pytorch.fad_gen': { 'fad_pytorch.fad_gen.gen': ('fad_gen.html#gen', 'fad_pytorch/fad_gen.py'),
                                      'fad_pytorch.fad_gen.main': ('fad_gen.html#main', 'fad_pytorch/fad_gen.py')},
             'fad_pytorch.fad_score': { 'fad_pytorch.fad_score.calc_mu_sigma': ('fad_score.html#calc_mu_sigma', 'fad_pytorch/fad_score.py'),
```

### Comparing `fad_pytorch-0.0.3/fad_pytorch/fad_embed.py` & `fad_pytorch-0.0.4/fad_pytorch/fad_embed.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_fad_embed.ipynb.
 
 # %% auto 0
-__all__ = ['GUDGUD_LICENSE', 'download_file', 'get_ckpt', 'setup_embedder', 'embed_all', 'main']
+__all__ = ['OPENL3_VERSION', 'GUDGUD_LICENSE', 'download_file', 'download_if_needed', 'get_ckpt', 'setup_embedder', 'embed',
+           'main']
 
 # %% ../nbs/02_fad_embed.ipynb 5
 import os
 import argparse
 import laion_clap 
 from laion_clap.training.data import get_audio_features
 from accelerate import Accelerator
@@ -15,19 +16,25 @@
 from aeiou.core import get_device, load_audio, get_audio_filenames, makedir
 from aeiou.datasets import AudioDataset
 from aeiou.hpc import HostPrinter
 from torch.utils.data import DataLoader
 from pathlib import Path
 import requests 
 from tqdm import tqdm
+import site 
+from einops import rearrange
 
 try:
     from fad_pytorch.pann import Cnn14_16k
 except: 
     from pann import Cnn14_16k
+    
+# there are TWO 'torchopenl3' repos!  they operate differently.
+OPENL3_VERSION = "turian" #  #  "hugo" | "turian". set to which version you've installed
+import torchopenl3
 
 # %% ../nbs/02_fad_embed.ipynb 7
 def download_file(url, local_filename):
     "Includes a progress bar.  from https://stackoverflow.com/a/37573701/4259243"
     response = requests.get(url, stream=True)
     total_size_in_bytes= int(response.headers.get('content-length', 0))
     block_size = 1024 #1 Kilobye
@@ -37,22 +44,30 @@
             progress_bar.update(len(data))
             file.write(data)
     progress_bar.close()
     if total_size_in_bytes != 0 and progress_bar.n != total_size_in_bytes:
         print("ERROR, something went wrong")
     return local_filename
 
+def download_if_needed(url, local_filename, accelerator=None):
+    "wrapper for download file"
+    if accelerator is None or accelerator.is_local_main_process:  # Only do this on one process instead of all
+        if not os.path.isfile(local_filename):
+            print(f"File {local_filename} not found, downloading from {url}")
+            download_file( url, local_filename)
+    if accelerator is not None: accelerator.wait_for_everyone()
+    return local_filename
+
 def get_ckpt(ckpt_file='music_speech_audioset_epoch_15_esc_89.98.pt',
              ckpt_base_url='https://huggingface.co/lukewys/laion_clap/blob/main',
-             ckpt_dl_path=os.path.expanduser("~/checkpoints")
+             ckpt_dl_path=os.path.expanduser("~/checkpoints"),
+             accelerator=None,
             ):
     ckpt_path = f"{ckpt_dl_path}/{ckpt_file}"
-    if not os.path.isfile(ckpt_path):
-        print(f"File {ckpt_path} not found, downloading from {ckpt_base_url}/{ckpt_file}")
-        download_file( f"{ckpt_base_url}/{ckpt_file}", ckpt_path)
+    download_if_needed( f"{ckpt_base_url}/{ckpt_file}" , ckpt_path)
     return ckpt_path
 
 # %% ../nbs/02_fad_embed.ipynb 8
 def setup_embedder(
         model_choice='clap', # 'clap' | 'vggish' | 'pann'
         device='cuda',
         ckpt_file='music_speech_audioset_epoch_15_esc_89.98.pt',  # NOTE: 'CLAP_CKPT' env var overrides ckpt_file kwarg
@@ -60,26 +75,27 @@
         # https://huggingface.co/lukewys/laion_clap/resolve/main/music_speech_audioset_epoch_15_esc_89.98.pt
         accelerator=None,
         ckpt_dl_path=os.path.expanduser("~/checkpoints"),
     ):
     "load the embedder model"
     embedder = None
     
+    sample_rate = 16000
     if model_choice == 'clap':
         clap_fusion, clap_amodel = True, "HTSAT-base"
         #doesn't work:  warnings.filterwarnings('ignore')  # temporarily disable CLAP warnings as they are super annoying. 
         clap_module = laion_clap.CLAP_Module(enable_fusion=clap_fusion, device=device, amodel=clap_amodel).requires_grad_(False).eval()
         clap_ckpt_path = os.getenv('CLAP_CKPT')  # NOTE: CLAP_CKPT env var overrides ckpt_file kwarg
         if clap_ckpt_path is not None:
             #print(f"Loading CLAP from {clap_ckpt_path}")
             clap_module.load_ckpt(ckpt=clap_ckpt_path, verbose=False)
         else:
-            if accelerator is None or accelerator.is_main_process: print(f"No CLAP checkpoint specified, using {ckpt_file}") 
+            print(f"No CLAP checkpoint specified, using {ckpt_file}") 
             clap_module = laion_clap.CLAP_Module(enable_fusion=False, amodel= 'HTSAT-base')
-            ckpt_path = get_ckpt(ckpt_file=ckpt_file, ckpt_base_url=ckpt_base_url, ckpt_dl_path=ckpt_dl_path)
+            ckpt_path = get_ckpt(ckpt_file=ckpt_file, ckpt_base_url=ckpt_base_url, ckpt_dl_path=ckpt_dl_path, accelerator=accelerator)
             clap_module.load_ckpt(ckpt_path, verbose=False)
             #clap_module.load_ckpt(model_id=1, verbose=False)
         #warnings.filterwarnings("default")   # turn warnings back on. 
         embedder = clap_module # synonyms 
         sample_rate = 48000
         
     # next two model loading codes from gudgud96's repo: https://github.com/gudgud96/frechet-audio-distance, LICENSE below
@@ -88,30 +104,45 @@
         use_pca=False
         use_activation=False
         if not use_pca:  embedder.postprocess = False
         if not use_activation: embedder.embeddings = torch.nn.Sequential(*list(embedder.embeddings.children())[:-1])
         sample_rate = 16000
 
     elif model_choice == "pann": # https://arxiv.org/abs/1912.10211
+        sample_rate = 16000
         model_path = os.path.join(torch.hub.get_dir(), "Cnn14_16k_mAP%3D0.438.pth")
-        if not(os.path.exists(model_path)):
-            torch.hub.download_url_to_file('https://zenodo.org/record/3987831/files/Cnn14_16k_mAP%3D0.438.pth', model_path)
-        embedder = Cnn14_16k(sample_rate=16000, window_size=512, hop_size=160, mel_bins=64, fmin=50, fmax=8000, classes_num=527)
+        if accelerator is None or accelerator.is_local_main_process:
+            if not(os.path.exists(model_path)):
+                torch.hub.download_url_to_file('https://zenodo.org/record/3987831/files/Cnn14_16k_mAP%3D0.438.pth', model_path)
+        if accelerator is not None: accelerator.wait_for_everyone()
+        embedder = Cnn14_16k(sample_rate=sample_rate, window_size=512, hop_size=160, mel_bins=64, fmin=50, fmax=8000, classes_num=527)
         checkpoint = torch.load(model_path, map_location=device)
         embedder.load_state_dict(checkpoint['model'])
-        sample_rate = 16000
-
+            
+    elif model_choice == "openl3" and OPENL3_VERSION == "hugo":  # hugo flores garcia's torchopenl3, https://github.com/hugofloresgarcia/torchopenl3
+        # openl3 repo doesn't install its weights if you do "pip install git+...", so here we download them separately
+        weights_dir = f"{site.getsitepackages()[0]}/torchopenl3/assets/weights"
+        makedir(weights_dir)
+        download_if_needed("https://github.com/hugofloresgarcia/torchopenl3/raw/main/torchopenl3/assets/weights/env-mel128", 
+                           f"{weights_dir}/music-mel128", accelerator=accelerator)
+        embedder = torchopenl3.OpenL3Embedding(input_repr='mel128', embedding_size=512, content_type='music')
+        sample_rate = 48000
+        
+    elif model_choice == "openl3" and OPENL3_VERSION == "turian":  # turian et al's torchopenl3, https://github.com/torchopenl3/torchopenl3
+        sample_rate = 48000
+        embedder = torchopenl3.models.load_audio_embedding_model(input_repr="mel256", content_type="music", embedding_size=512)
+        pass # turian et al's does all its setup when it's invoked 
     else:
         raise ValueError("Sorry, other models not supported yet")
         
-    embedder.eval()   
+    if hasattr(embedder,'eval'): embedder.eval()   
     return embedder, sample_rate
 
 
-GUDGUD_LICENSE = """
+GUDGUD_LICENSE = """For VGGish implementation:
 MIT License
 
 Copyright (c) 2022 Hao Hao Tan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
@@ -128,16 +159,17 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 # %% ../nbs/02_fad_embed.ipynb 10
-def embed_all(args): 
-    model_choice, real_path, fake_path, chunk_size, sr, max_batch_size = args.embed_model, args.real_path, args.fake_path, args.chunk_size, args.sr, args.batch_size
+def embed(args): 
+    model_choice, real_path, fake_path, chunk_size, sr, max_batch_size, debug = args.embed_model, args.real_path, args.fake_path, args.chunk_size, args.sr, args.batch_size, args.debug
+    sample_rate = sr
     local_rank = int(os.environ.get("LOCAL_RANK", 0))
     world_size = int(os.environ.get("WORLD_SIZE", 1))
     ddps = f"[{local_rank}/{world_size}]"  # string for distributed computing info, e.g. "[1/8]" 
 
     accelerator = Accelerator()
     hprint = HostPrinter(accelerator)  # hprint only prints on head node
     device = accelerator.device    # get_device()
@@ -159,82 +191,113 @@
     num_per_proc = minlen // world_size
     start = local_rank * num_per_proc
     end =  minlen if local_rank == world_size-1 else (local_rank+1) * num_per_proc
     #print(f"{ddps} start, end = ",start,end) 
     real_filenames, fake_filenames = real_filenames[start:end], fake_filenames[start:end]
     """
 
-    # setup embedder and dataloader
-    embedder, emb_sample_rate = setup_embedder(model_choice, device, accelerator)
-    if sr != emb_sample_rate:
-        hprint(f"\n*******\nWARNING: sr={sr} != {model_choice}'s emb_sample_rate={emb_sample_rate}. Will resample audio to the latter\n*******\n")
-        sr = emb_sample_rate
-    hprint(f"{ddps} Embedder '{model_choice}' ready to go!")
-
-    real_dataset = AudioDataset(real_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
-    fake_dataset = AudioDataset(fake_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
-    batch_size = min( len(real_dataset) // world_size , max_batch_size ) 
-    hprint(f"\nGiven max_batch_size = {max_batch_size}, len(real_dataset) = {len(real_dataset)}, and world_size = {world_size}, we'll use batch_size = {batch_size}")
-    real_dl = DataLoader(real_dataset, batch_size=batch_size, shuffle=False)
-    fake_dl = DataLoader(fake_dataset, batch_size=batch_size, shuffle=False)
-    
-    real_dl, fake_dl, embedder = accelerator.prepare( real_dl, fake_dl, embedder )  # prepare handles distributing things among GPUs
+    model_choices = [model_choice] if model_choice != 'all' else ['clap','vggish','pann','openl3']
     
-    # note that we don't actually care if real & fake files are pulled in the same order; we'll only be comparing the *distributions* of the data.
-    with torch.no_grad():
-        for dl, name in zip([real_dl, fake_dl],['real','fake']):
-            newdir_already = False
-            for i, data_dict in enumerate(dl):
-                audio, filename_batch = data_dict['inputs'], data_dict['filename']
-                if not newdir_already: 
-                    p = Path( filename_batch[0] )
-                    dir_already = True
-                    newdir = f"{p.parents[0]}_emb_{model_choice}"
-                    hprint(f"newdir = {newdir}")
-                    makedir(newdir) 
-
-                #print(f"{ddps} i = {i}/{len(real_dataset)}, filename = {filename_batch[0]}")
-                audio = audio.to(device)
-
-
-                if model_choice == 'clap': 
-                    while len(audio.shape) < 3: 
-                        audio = audio.unsqueeze(0) # add batch and/or channel dims 
-                    embeddings = embedder.get_audio_embedding_from_data(audio.mean(dim=1).to(device), use_tensor=True).to(audio.dtype)
-
-                elif model_choice == "vggish":
-                    audio = torch.mean(audio, dim=1)   # vggish requries we convert to mono
-                    embeddings = []                    # ...whoa, vggish can't even handle batches?  we have to pass 'em through singly?
-                    for bi, waveform in enumerate(audio): 
-                        e = embedder.forward(waveform.cpu().numpy(), emb_sample_rate)
-                        embeddings.append(e) 
-                    embeddings = torch.cat(embeddings, dim=0)
-
-                elif model_choice == "pann": 
-                    audio = torch.mean(audio, dim=1)  # mono only.  todo:  keepdim=True ?
-                    out = embedder.forward(audio, None)
-                    embeddings = out['embedding'].data
-
-                hprint(f"embeddings.shape = {embeddings.shape}")
-                # TODO: for now we'll just dump each batch on each proc to its own file; this could be improved
-                outfilename = f"{newdir}/emb_p{local_rank}_b{i}.pt"
-                print(f"{ddps} Saving embeddings to {outfilename}")
-                torch.save(embeddings.cpu().detach(), outfilename)
+    for model_choice in model_choices: # loop over multiple embedders
+        hprint(f"\n ** Model_choice = {model_choice}")
+        # setup embedder and dataloader
+        embedder, emb_sample_rate = setup_embedder(model_choice, device, accelerator)
+        if sr != emb_sample_rate:
+            hprint(f"\n*******\nWARNING: sr={sr} != {model_choice}'s emb_sample_rate={emb_sample_rate}. Will resample audio to the latter\n*******\n")
+            sr = emb_sample_rate
+        hprint(f"{ddps} Embedder '{model_choice}' ready to go!")
+
+        real_dataset = AudioDataset(real_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
+        fake_dataset = AudioDataset(fake_path, augs='Stereo(), PhaseFlipper()', sample_rate=emb_sample_rate, sample_size=chunk_size, return_dict=True, verbose=args.verbose)
+        batch_size = min( len(real_dataset) // world_size , max_batch_size ) 
+        hprint(f"\nGiven max_batch_size = {max_batch_size}, len(real_dataset) = {len(real_dataset)}, and world_size = {world_size}, we'll use batch_size = {batch_size}")
+        real_dl = DataLoader(real_dataset, batch_size=batch_size, shuffle=False)
+        fake_dl = DataLoader(fake_dataset, batch_size=batch_size, shuffle=False)
+
+        real_dl, fake_dl, embedder = accelerator.prepare( real_dl, fake_dl, embedder )  # prepare handles distributing things among GPUs
+
+        # note that we don't actually care if real & fake files are pulled in the same order; we'll only be comparing the *distributions* of the data.
+        with torch.no_grad():
+            for dl, name in zip([real_dl, fake_dl],['real','fake']):
+                newdir_already = False
+                for i, data_dict in enumerate(dl):
+                    audio, filename_batch = data_dict['inputs'], data_dict['filename']
+                    if not newdir_already: 
+                        p = Path( filename_batch[0] )
+                        dir_already = True
+                        newdir = f"{p.parents[0]}_emb_{model_choice}"
+                        hprint(f"newdir = {newdir}")
+                        makedir(newdir) 
+
+                    #print(f"{ddps} i = {i}/{len(real_dataset)}, filename = {filename_batch[0]}")
+                    audio = audio.to(device)
+
+
+                    if model_choice == 'clap': 
+                        while len(audio.shape) < 3: 
+                            audio = audio.unsqueeze(0) # add batch and/or channel dims 
+                        embeddings = embedder.get_audio_embedding_from_data(audio.mean(dim=1).to(device), use_tensor=True).to(audio.dtype)
+
+                    elif model_choice == "vggish":
+                        audio = torch.mean(audio, dim=1)   # vggish requries we convert to mono
+                        embeddings = []                    # ...whoa, vggish can't even handle batches?  we have to pass 'em through singly?
+                        for bi, waveform in enumerate(audio): 
+                            e = embedder.forward(waveform.cpu().numpy(), emb_sample_rate)
+                            embeddings.append(e) 
+                        embeddings = torch.cat(embeddings, dim=0)
+
+                    elif model_choice == "pann": 
+                        audio = torch.mean(audio, dim=1)  # mono only.  todo:  keepdim=True ?
+                        out = embedder.forward(audio, None)
+                        embeddings = out['embedding'].data
+                        
+                    elif model_choice == "openl3" and OPENL3_VERSION == "hugo":
+                        ##audio = torch.mean(audio, dim=1)  # mono only.
+                        embeddings = []
+                        for bi, waveform in enumerate( audio.cpu().numpy() ): # no batch processing, expects numpy 
+                            e = torchopenl3.embed(model=embedder, 
+                                audio=waveform, # shape sould be (channels, samples)
+                                sample_rate=emb_sample_rate, # sample rate of input file
+                                hop_size=1,  device=device)
+                            if debug: hprint(f"bi = {bi}, waveform.shape = {waveform.shape},  e.shape = {e.shape}") 
+                            embeddings.append(torch.tensor(e))
+                        embeddings = torch.cat(embeddings, dim=0)
+                        
+                    elif model_choice == "openl3" and OPENL3_VERSION == "turian":
+                        # Note: turian's can/will do multiple time-stamped embeddings if the sample_size is long enough! 
+                        
+                        audio = rearrange(audio, 'b c s -> b s c')  # make channels_first
+                        embeddings, timestamps = torchopenl3.get_audio_embedding(audio, emb_sample_rate, model=embedder)
+                        embeddings = torch.squeeze(embeddings, 1)  # get rid of any spurious dimensions of 1 in middle position 
+                        
+                    else:
+                        raise ValueError(f"Unknown model_choice = {model_choice}")
+
+                    hprint(f"embeddings.shape = {embeddings.shape}")
+                    # TODO: for now we'll just dump each batch on each proc to its own file; this could be improved
+                    outfilename = f"{newdir}/emb_p{local_rank}_b{i}.pt"
+                    hprint(f"{ddps} Saving embeddings to {outfilename}")
+                    torch.save(embeddings.cpu().detach(), outfilename)
+                    
+        del embedder
+        torch.cuda.empty_cache()
+        # end loop over various embedders
     return        
 
 # %% ../nbs/02_fad_embed.ipynb 11
 def main(): 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('embed_model', help='choice of embedding model: clap | vggish | pann', default='clap')
+    parser.add_argument('embed_model', help='choice of embedding model(s): clap | vggish | pann | openl3 | all ', default='clap')
     parser.add_argument('real_path', help='Path of files of real audio', default='real/')
     parser.add_argument('fake_path', help='Path of files of fake audio', default='fake/')
     parser.add_argument('--chunk_size', type=int, default=24000, help='Length of chunks (in audio samples) to embed')
     parser.add_argument('--batch_size', type=int, default=64, help='MAXIMUM Batch size for computing embeddings (may go smaller)')
     parser.add_argument('--sr', type=int, default=48000, help='sample rate (will resample inputs at this rate)')
     parser.add_argument('--verbose', action='store_true',  help='Show notices of resampling when reading files')
+    parser.add_argument('--debug', action='store_true',  help='Extra messages for debugging this program')
 
     args = parser.parse_args()
-    embed_all(args)
+    embed(args)
 
 # %% ../nbs/02_fad_embed.ipynb 12
 if __name__ == '__main__' and "get_ipython" not in dir():
     main()
```

### Comparing `fad_pytorch-0.0.3/fad_pytorch/fad_gen.py` & `fad_pytorch-0.0.4/fad_pytorch/fad_gen.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch/fad_score.py` & `fad_pytorch-0.0.4/fad_pytorch/fad_score.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch/pann.py` & `fad_pytorch-0.0.4/fad_pytorch/pann.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch/pann_pytorch_utils.py` & `fad_pytorch-0.0.4/fad_pytorch/pann_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch/sqrtm.py` & `fad_pytorch-0.0.4/fad_pytorch/sqrtm.py`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/fad_pytorch.egg-info/SOURCES.txt` & `fad_pytorch-0.0.4/fad_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fad_pytorch-0.0.3/settings.ini` & `fad_pytorch-0.0.4/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fad_pytorch
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fad_pytorch
@@ -34,10 +34,12 @@
 description = Frechet Audio Distance evaluation in PyTorch
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = drscotthawley
 
 ### Optional ###
-requirements = aeiou torch>=1.13.1 torchaudio>=0.13.1 laion-clap accelerate torchlibrosa
+requirements = aeiou torch>=1.13.1 torchaudio>=0.13.1 laion-clap accelerate torchlibrosa torchopenl3
+# torchopenl3 is turian et al's.  pypi won't let use hugo's: git+https://github.com/hugofloresgarcia/torchopenl3.git
+
 # dev_requirements = 
 console_scripts = fad_gen=fad_pytorch.fad_gen:main fad_score=fad_pytorch.fad_score:main fad_embed=fad_pytorch.fad_embed:main
```

### Comparing `fad_pytorch-0.0.3/setup.py` & `fad_pytorch-0.0.4/setup.py`

 * *Files identical despite different names*

