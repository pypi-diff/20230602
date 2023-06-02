# Comparing `tmp/deepflash2-0.2.2.tar.gz` & `tmp/deepflash2-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepflash2-0.2.2.tar", last modified: Thu Feb 16 06:46:16 2023, max compression
+gzip compressed data, was "deepflash2-0.2.3.tar", last modified: Fri Jun  2 06:33:55 2023, max compression
```

## Comparing `deepflash2-0.2.2.tar` & `deepflash2-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 06:46:16.774515 deepflash2-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     2348 2023-02-16 06:29:07.000000 deepflash2-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-02-16 06:29:07.000000 deepflash2-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-02-16 06:29:07.000000 deepflash2-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10039 2023-02-16 06:46:16.774515 deepflash2-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9273 2023-02-16 06:29:07.000000 deepflash2-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 06:46:16.773515 deepflash2-0.2.2/deepflash2/
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4982 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/_nbdev.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/all.py
--rw-r--r--   0 root         (0) root         (0)     3794 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/config.py
--rw-r--r--   0 root         (0) root         (0)    24035 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/data.py
--rw-r--r--   0 root         (0) root         (0)     8578 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/gt.py
--rw-r--r--   0 root         (0) root         (0)    80122 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/gui.py
--rw-r--r--   0 root         (0) root         (0)    10434 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/inference.py
--rw-r--r--   0 root         (0) root         (0)    27396 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/learner.py
--rw-r--r--   0 root         (0) root         (0)     4949 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/losses.py
--rw-r--r--   0 root         (0) root         (0)     6859 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/models.py
--rw-r--r--   0 root         (0) root         (0)     3578 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/tta.py
--rw-r--r--   0 root         (0) root         (0)    14606 2023-02-16 06:29:07.000000 deepflash2-0.2.2/deepflash2/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-16 06:46:16.774515 deepflash2-0.2.2/deepflash2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10039 2023-02-16 06:46:16.000000 deepflash2-0.2.2/deepflash2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      532 2023-02-16 06:46:16.000000 deepflash2-0.2.2/deepflash2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 06:46:16.000000 deepflash2-0.2.2/deepflash2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-16 06:38:02.000000 deepflash2-0.2.2/deepflash2.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      249 2023-02-16 06:46:16.000000 deepflash2-0.2.2/deepflash2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-02-16 06:46:16.000000 deepflash2-0.2.2/deepflash2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1082 2023-02-16 06:29:07.000000 deepflash2-0.2.2/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-16 06:46:16.774515 deepflash2-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2065 2023-02-16 06:29:07.000000 deepflash2-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:33:55.196368 deepflash2-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-06-02 06:27:19.000000 deepflash2-0.2.3/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 06:27:19.000000 deepflash2-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-02 06:27:19.000000 deepflash2-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-06-02 06:33:55.195368 deepflash2-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-06-02 06:27:19.000000 deepflash2-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:33:55.194368 deepflash2-0.2.3/deepflash2/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/_nbdev.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/all.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/config.py
+-rw-r--r--   0 root         (0) root         (0)    24035 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/data.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/gt.py
+-rw-r--r--   0 root         (0) root         (0)    80122 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/gui.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/inference.py
+-rw-r--r--   0 root         (0) root         (0)    27396 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/learner.py
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/losses.py
+-rw-r--r--   0 root         (0) root         (0)     6859 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/models.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/tta.py
+-rw-r--r--   0 root         (0) root         (0)    14606 2023-06-02 06:27:19.000000 deepflash2-0.2.3/deepflash2/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 06:33:55.195368 deepflash2-0.2.3/deepflash2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10156 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      532 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-02 06:33:55.000000 deepflash2-0.2.3/deepflash2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-06-02 06:27:45.000000 deepflash2-0.2.3/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 06:33:55.196368 deepflash2-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-06-02 06:27:19.000000 deepflash2-0.2.3/setup.py
```

### Comparing `deepflash2-0.2.2/CONTRIBUTING.md` & `deepflash2-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/LICENSE` & `deepflash2-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/PKG-INFO` & `deepflash2-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepflash2
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Deep learning pipeline for segmentation of fluorescent labels in microscopy images
 Home-page: https://github.com/matjesg/deepflash2
 Author: Matthias Griebel
 Author-email: matthias.griebel@uni-wuerzburg.com
 License: Apache Software License 2.0
 Keywords: unet,deep learning,semantic segmentation,microscopy,fluorescent labels
 Classifier: Development Status :: 3 - Alpha
@@ -24,21 +24,20 @@
 ![deepflash2](https://raw.githubusercontent.com/matjesg/deepflash2/master/nbs/media/logo/deepflash2_logo_medium.png)
 
 Official repository of deepflash2 - a deep-learning pipeline for segmentation of ambiguous microscopic images.
 
 [![PyPI](https://img.shields.io/pypi/v/deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/deepflash2/#description) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/deepflash2)](https://pypistats.org/packages/deepflash2)
 [![Conda (channel only)](https://img.shields.io/conda/vn/matjesg/deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/deepflash2)
-[![GitHub stars](https://img.shields.io/github/stars/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
-[![GitHub forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)](https://doi.org/10.5281/zenodo.7653312)
 ***
 
 __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for life science researchers. 
-> Read the [paper](https://arxiv.org/abs/2111.06693), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
+> Read the [paper](https://www.nature.com/articles/s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
 - **No coding skills required** (graphical user interface)
 - **Ground truth estimation** from the annotations of multiple experts for model training and validation
 - **Quality assurance and out-of-distribution detection** for reliable prediction on new data 
 - **Best-in-class performance** for semantic and instance segmentation
 
 <img src="https://github.com/matjesg/deepflash2/blob/master/nbs/media/sample_images.png?raw=true" width="800px" style="max-width: 800pxpx">
 
@@ -78,25 +77,30 @@
 | Expected Output | 5 GT Segmentation Masks | 5 models | 5 predicted segmentation masks  (semantic and instance) and uncertainty maps|
 | Estimated Time | ~ 1 min | ~ 150 min | ~ 4 min |
 
 Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU).
 
 ## Paper and Experiments 
 
-We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
+We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing) and [Zenodo](https://doi.org/10.5281/zenodo.7653312).
 
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/2111.06693). Please cite
+Our Nature Communications article is available [here](https://www.nature.com/articles/s41467-023-36960-9). Please cite
 
 ```
-@misc{griebel2021deepflash2,
-    title={Deep-learning in the bioimaging wild: Handling ambiguous data with deepflash2}, 
-    author={Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
-    year={2021},
-    eprint={2111.06693},
-    archivePrefix={arXiv}
+@article{Griebel2023,
+  doi = {10.1038/s41467-023-36960-9},
+  url = {https://doi.org/10.1038/s41467-023-36960-9},
+  year = {2023},
+  month = mar,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
+  title = {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+  journal = {Nature Communications}
 }
 ```
 
 
 
 ## System requirements
 > Works in the browser or on your local pc/server
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepflash2 Version: 0.2.2 Summary: A Deep learning
+Metadata-Version: 2.1 Name: deepflash2 Version: 0.2.3 Summary: A Deep learning
 pipeline for segmentation of fluorescent labels in microscopy images Home-page:
 https://github.com/matjesg/deepflash2 Author: Matthias Griebel Author-email:
 matthias.griebel@uni-wuerzburg.com License: Apache Software License 2.0
 Keywords: unet,deep learning,semantic segmentation,microscopy,fluorescent
 labels Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
@@ -13,64 +13,66 @@
 repository of deepflash2 - a deep-learning pipeline for segmentation of
 ambiguous microscopic images. [![PyPI](https://img.shields.io/pypi/v/
 deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/
 deepflash2/#description) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
 deepflash2)](https://pypistats.org/packages/deepflash2) [![Conda (channel
 only)](https://img.shields.io/conda/vn/matjesg/
 deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/
-deepflash2) [![GitHub stars](https://img.shields.io/github/stars/matjesg/
-deepflash2?style=social)](https://github.com/matjesg/deepflash2/) [![GitHub
-forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)]
-(https://github.com/matjesg/deepflash2/) *** __The best of two worlds:__
+deepflash2) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)]
+(https://doi.org/10.5281/zenodo.7653312) *** __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for
-life science researchers. > Read the [paper](https://arxiv.org/abs/2111.06693),
-watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or
-read the [docs](https://matjesg.github.io/deepflash2/). - **No coding skills
-required** (graphical user interface) - **Ground truth estimation** from the
-annotations of multiple experts for model training and validation - **Quality
-assurance and out-of-distribution detection** for reliable prediction on new
-data - **Best-in-class performance** for semantic and instance segmentation
-[https://github.com/matjesg/deepflash2/blob/master/nbs/media/
-sample_images.png?raw=true] [https://www.kaggle.com/static/images/medals/
-competitions/goldl@1x.png] **Kaggle Gold Medal and Innovation Price Winner:**
-The *deepflash2* Python API built the foundation for winning the [Innovation
-Award](https://hubmapconsortium.github.io/ccf/pages/kaggle.html) a Kaggle Gold
-Medal in the [HuBMAP - Hacking the Kidney](https://www.kaggle.com/c/hubmap-
-kidney-segmentation) challenge. Have a look at our [solution](https://
-www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ## Quick Start and Demo >
-Get started in less than a minute. Watch the tutorials for help. #### Demo on
-Hugging Face Spaces Go to the [demo space](https://huggingface.co/spaces/
-matjesg/deepflash2) -- inference only (no training possible). #### Demo usage
-with Google Colab For a quick start, run *deepflash2* in Google Colaboratory
-(Google account required). [![Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/matjesg/deepflash2/
-blob/master/deepflash2_GUI.ipynb)  The GUI provides a build-in use for our
-[sample data](https://github.com/matjesg/deepflash2/releases/tag/sample_data).
-1. Starting the GUI (in Colab or follow the installation instructions below) 2.
-Select the task (GT Estimation, Training, or Prediction) 3. Click the `Load
-Sample Data` button in the sidebar and continue to the next sidebar section.
-For futher instructions watch the [tutorials](https://matjesg.github.io/
-deepflash2/tutorial.html). We provide an overview of the tasks below: | |
-Ground Truth (GT) Estimation | Training | Prediction | |---|---|---|---| | Main
-Task | STAPLE or Majority Voting | Ensemble training and validation | Semantic
-and instance segmentation | | Sample Data | 5 masks from 5 experts each | 5
-image/mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
+life science researchers. > Read the [paper](https://www.nature.com/articles/
+s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/
+deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/
+deepflash2/). - **No coding skills required** (graphical user interface) -
+**Ground truth estimation** from the annotations of multiple experts for model
+training and validation - **Quality assurance and out-of-distribution
+detection** for reliable prediction on new data - **Best-in-class performance**
+for semantic and instance segmentation [https://github.com/matjesg/deepflash2/
+blob/master/nbs/media/sample_images.png?raw=true] [https://www.kaggle.com/
+static/images/medals/competitions/goldl@1x.png] **Kaggle Gold Medal and
+Innovation Price Winner:** The *deepflash2* Python API built the foundation for
+winning the [Innovation Award](https://hubmapconsortium.github.io/ccf/pages/
+kaggle.html) a Kaggle Gold Medal in the [HuBMAP - Hacking the Kidney](https://
+www.kaggle.com/c/hubmap-kidney-segmentation) challenge. Have a look at our
+[solution](https://www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ##
+Quick Start and Demo > Get started in less than a minute. Watch the tutorials
+for help. #### Demo on Hugging Face Spaces Go to the [demo space](https://
+huggingface.co/spaces/matjesg/deepflash2) -- inference only (no training
+possible). #### Demo usage with Google Colab For a quick start, run
+*deepflash2* in Google Colaboratory (Google account required). [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/matjesg/deepflash2/blob/master/
+deepflash2_GUI.ipynb)  The GUI provides a build-in use for our [sample data]
+(https://github.com/matjesg/deepflash2/releases/tag/sample_data). 1. Starting
+the GUI (in Colab or follow the installation instructions below) 2. Select the
+task (GT Estimation, Training, or Prediction) 3. Click the `Load Sample Data`
+button in the sidebar and continue to the next sidebar section. For futher
+instructions watch the [tutorials](https://matjesg.github.io/deepflash2/
+tutorial.html). We provide an overview of the tasks below: | | Ground Truth
+(GT) Estimation | Training | Prediction | |---|---|---|---| | Main Task |
+STAPLE or Majority Voting | Ensemble training and validation | Semantic and
+instance segmentation | | Sample Data | 5 masks from 5 experts each | 5 image/
+mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
 Segmentation Masks | 5 models | 5 predicted segmentation masks (semantic and
 instance) and uncertainty maps| | Estimated Time | ~ 1 min | ~ 150 min | ~ 4
 min | Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU). ##
 Paper and Experiments We provide a complete guide to reproduce our experiments
 using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/
 tree/master/paper). The data is currently available on [Google Drive](https://
-drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/
-2111.06693). Please cite ``` @misc{griebel2021deepflash2, title={Deep-learning
-in the bioimaging wild: Handling ambiguous data with deepflash2}, author=
-{Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and
-Philip Tovote and Robert Blum and Christoph M. Flath}, year={2021}, eprint=
-{2111.06693}, archivePrefix={arXiv} } ``` ## System requirements > Works in the
+drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing)
+and [Zenodo](https://doi.org/10.5281/zenodo.7653312). Our Nature Communications
+article is available [here](https://www.nature.com/articles/s41467-023-36960-
+9). Please cite ``` @article{Griebel2023, doi = {10.1038/s41467-023-36960-9},
+url = {https://doi.org/10.1038/s41467-023-36960-9}, year = {2023}, month = mar,
+publisher = {Springer Science and Business Media {LLC}}, volume = {14}, number
+= {1}, author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and
+Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath}, title
+= {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+journal = {Nature Communications} } ``` ## System requirements > Works in the
 browser or on your local pc/server *deepflash2* is designed to run on Windows,
 Linux, or Mac (x86-64) if [pytorch](https://pytorch.org/get-started/locally/
 ) is installable. We generally recommend using Google Colab as it only requires
 a Google Account and a device with a web browser. To run *deepflash2* locally,
 we recommend using a system with a GPU (e.g., 2 CPUs, 8 GB RAM, NVIDIA GPU with
 8GB VRAM or better). *deepflash2* requires Python>3.6 and the software
 dependencies are defined in the [settings.ini](https://github.com/matjesg/
```

### Comparing `deepflash2-0.2.2/README.md` & `deepflash2-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 ![deepflash2](https://raw.githubusercontent.com/matjesg/deepflash2/master/nbs/media/logo/deepflash2_logo_medium.png)
 
 Official repository of deepflash2 - a deep-learning pipeline for segmentation of ambiguous microscopic images.
 
 [![PyPI](https://img.shields.io/pypi/v/deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/deepflash2/#description) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/deepflash2)](https://pypistats.org/packages/deepflash2)
 [![Conda (channel only)](https://img.shields.io/conda/vn/matjesg/deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/deepflash2)
-[![GitHub stars](https://img.shields.io/github/stars/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
-[![GitHub forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)](https://doi.org/10.5281/zenodo.7653312)
 ***
 
 __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for life science researchers. 
-> Read the [paper](https://arxiv.org/abs/2111.06693), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
+> Read the [paper](https://www.nature.com/articles/s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
 - **No coding skills required** (graphical user interface)
 - **Ground truth estimation** from the annotations of multiple experts for model training and validation
 - **Quality assurance and out-of-distribution detection** for reliable prediction on new data 
 - **Best-in-class performance** for semantic and instance segmentation
 
 <img src="https://github.com/matjesg/deepflash2/blob/master/nbs/media/sample_images.png?raw=true" width="800px" style="max-width: 800pxpx">
 
@@ -59,25 +58,30 @@
 | Expected Output | 5 GT Segmentation Masks | 5 models | 5 predicted segmentation masks  (semantic and instance) and uncertainty maps|
 | Estimated Time | ~ 1 min | ~ 150 min | ~ 4 min |
 
 Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU).
 
 ## Paper and Experiments 
 
-We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
+We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing) and [Zenodo](https://doi.org/10.5281/zenodo.7653312).
 
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/2111.06693). Please cite
+Our Nature Communications article is available [here](https://www.nature.com/articles/s41467-023-36960-9). Please cite
 
 ```
-@misc{griebel2021deepflash2,
-    title={Deep-learning in the bioimaging wild: Handling ambiguous data with deepflash2}, 
-    author={Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
-    year={2021},
-    eprint={2111.06693},
-    archivePrefix={arXiv}
+@article{Griebel2023,
+  doi = {10.1038/s41467-023-36960-9},
+  url = {https://doi.org/10.1038/s41467-023-36960-9},
+  year = {2023},
+  month = mar,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
+  title = {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+  journal = {Nature Communications}
 }
 ```
 
 
 
 ## System requirements
 > Works in the browser or on your local pc/server
```

#### html2text {}

```diff
@@ -3,64 +3,66 @@
 repository of deepflash2 - a deep-learning pipeline for segmentation of
 ambiguous microscopic images. [![PyPI](https://img.shields.io/pypi/v/
 deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/
 deepflash2/#description) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
 deepflash2)](https://pypistats.org/packages/deepflash2) [![Conda (channel
 only)](https://img.shields.io/conda/vn/matjesg/
 deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/
-deepflash2) [![GitHub stars](https://img.shields.io/github/stars/matjesg/
-deepflash2?style=social)](https://github.com/matjesg/deepflash2/) [![GitHub
-forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)]
-(https://github.com/matjesg/deepflash2/) *** __The best of two worlds:__
+deepflash2) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)]
+(https://doi.org/10.5281/zenodo.7653312) *** __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for
-life science researchers. > Read the [paper](https://arxiv.org/abs/2111.06693),
-watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or
-read the [docs](https://matjesg.github.io/deepflash2/). - **No coding skills
-required** (graphical user interface) - **Ground truth estimation** from the
-annotations of multiple experts for model training and validation - **Quality
-assurance and out-of-distribution detection** for reliable prediction on new
-data - **Best-in-class performance** for semantic and instance segmentation
-[https://github.com/matjesg/deepflash2/blob/master/nbs/media/
-sample_images.png?raw=true] [https://www.kaggle.com/static/images/medals/
-competitions/goldl@1x.png] **Kaggle Gold Medal and Innovation Price Winner:**
-The *deepflash2* Python API built the foundation for winning the [Innovation
-Award](https://hubmapconsortium.github.io/ccf/pages/kaggle.html) a Kaggle Gold
-Medal in the [HuBMAP - Hacking the Kidney](https://www.kaggle.com/c/hubmap-
-kidney-segmentation) challenge. Have a look at our [solution](https://
-www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ## Quick Start and Demo >
-Get started in less than a minute. Watch the tutorials for help. #### Demo on
-Hugging Face Spaces Go to the [demo space](https://huggingface.co/spaces/
-matjesg/deepflash2) -- inference only (no training possible). #### Demo usage
-with Google Colab For a quick start, run *deepflash2* in Google Colaboratory
-(Google account required). [![Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/matjesg/deepflash2/
-blob/master/deepflash2_GUI.ipynb)  The GUI provides a build-in use for our
-[sample data](https://github.com/matjesg/deepflash2/releases/tag/sample_data).
-1. Starting the GUI (in Colab or follow the installation instructions below) 2.
-Select the task (GT Estimation, Training, or Prediction) 3. Click the `Load
-Sample Data` button in the sidebar and continue to the next sidebar section.
-For futher instructions watch the [tutorials](https://matjesg.github.io/
-deepflash2/tutorial.html). We provide an overview of the tasks below: | |
-Ground Truth (GT) Estimation | Training | Prediction | |---|---|---|---| | Main
-Task | STAPLE or Majority Voting | Ensemble training and validation | Semantic
-and instance segmentation | | Sample Data | 5 masks from 5 experts each | 5
-image/mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
+life science researchers. > Read the [paper](https://www.nature.com/articles/
+s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/
+deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/
+deepflash2/). - **No coding skills required** (graphical user interface) -
+**Ground truth estimation** from the annotations of multiple experts for model
+training and validation - **Quality assurance and out-of-distribution
+detection** for reliable prediction on new data - **Best-in-class performance**
+for semantic and instance segmentation [https://github.com/matjesg/deepflash2/
+blob/master/nbs/media/sample_images.png?raw=true] [https://www.kaggle.com/
+static/images/medals/competitions/goldl@1x.png] **Kaggle Gold Medal and
+Innovation Price Winner:** The *deepflash2* Python API built the foundation for
+winning the [Innovation Award](https://hubmapconsortium.github.io/ccf/pages/
+kaggle.html) a Kaggle Gold Medal in the [HuBMAP - Hacking the Kidney](https://
+www.kaggle.com/c/hubmap-kidney-segmentation) challenge. Have a look at our
+[solution](https://www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ##
+Quick Start and Demo > Get started in less than a minute. Watch the tutorials
+for help. #### Demo on Hugging Face Spaces Go to the [demo space](https://
+huggingface.co/spaces/matjesg/deepflash2) -- inference only (no training
+possible). #### Demo usage with Google Colab For a quick start, run
+*deepflash2* in Google Colaboratory (Google account required). [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/matjesg/deepflash2/blob/master/
+deepflash2_GUI.ipynb)  The GUI provides a build-in use for our [sample data]
+(https://github.com/matjesg/deepflash2/releases/tag/sample_data). 1. Starting
+the GUI (in Colab or follow the installation instructions below) 2. Select the
+task (GT Estimation, Training, or Prediction) 3. Click the `Load Sample Data`
+button in the sidebar and continue to the next sidebar section. For futher
+instructions watch the [tutorials](https://matjesg.github.io/deepflash2/
+tutorial.html). We provide an overview of the tasks below: | | Ground Truth
+(GT) Estimation | Training | Prediction | |---|---|---|---| | Main Task |
+STAPLE or Majority Voting | Ensemble training and validation | Semantic and
+instance segmentation | | Sample Data | 5 masks from 5 experts each | 5 image/
+mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
 Segmentation Masks | 5 models | 5 predicted segmentation masks (semantic and
 instance) and uncertainty maps| | Estimated Time | ~ 1 min | ~ 150 min | ~ 4
 min | Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU). ##
 Paper and Experiments We provide a complete guide to reproduce our experiments
 using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/
 tree/master/paper). The data is currently available on [Google Drive](https://
-drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/
-2111.06693). Please cite ``` @misc{griebel2021deepflash2, title={Deep-learning
-in the bioimaging wild: Handling ambiguous data with deepflash2}, author=
-{Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and
-Philip Tovote and Robert Blum and Christoph M. Flath}, year={2021}, eprint=
-{2111.06693}, archivePrefix={arXiv} } ``` ## System requirements > Works in the
+drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing)
+and [Zenodo](https://doi.org/10.5281/zenodo.7653312). Our Nature Communications
+article is available [here](https://www.nature.com/articles/s41467-023-36960-
+9). Please cite ``` @article{Griebel2023, doi = {10.1038/s41467-023-36960-9},
+url = {https://doi.org/10.1038/s41467-023-36960-9}, year = {2023}, month = mar,
+publisher = {Springer Science and Business Media {LLC}}, volume = {14}, number
+= {1}, author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and
+Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath}, title
+= {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+journal = {Nature Communications} } ``` ## System requirements > Works in the
 browser or on your local pc/server *deepflash2* is designed to run on Windows,
 Linux, or Mac (x86-64) if [pytorch](https://pytorch.org/get-started/locally/
 ) is installable. We generally recommend using Google Colab as it only requires
 a Google Account and a device with a web browser. To run *deepflash2* locally,
 we recommend using a system with a GPU (e.g., 2 CPUs, 8 GB RAM, NVIDIA GPU with
 8GB VRAM or better). *deepflash2* requires Python>3.6 and the software
 dependencies are defined in the [settings.ini](https://github.com/matjesg/
```

### Comparing `deepflash2-0.2.2/deepflash2/_nbdev.py` & `deepflash2-0.2.3/deepflash2/_nbdev.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/config.py` & `deepflash2-0.2.3/deepflash2/config.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/data.py` & `deepflash2-0.2.3/deepflash2/data.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/gt.py` & `deepflash2-0.2.3/deepflash2/gt.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/gui.py` & `deepflash2-0.2.3/deepflash2/gui.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/inference.py` & `deepflash2-0.2.3/deepflash2/inference.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/learner.py` & `deepflash2-0.2.3/deepflash2/learner.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/losses.py` & `deepflash2-0.2.3/deepflash2/losses.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/models.py` & `deepflash2-0.2.3/deepflash2/models.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/tta.py` & `deepflash2-0.2.3/deepflash2/tta.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2/utils.py` & `deepflash2-0.2.3/deepflash2/utils.py`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/deepflash2.egg-info/PKG-INFO` & `deepflash2-0.2.3/deepflash2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepflash2
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Deep learning pipeline for segmentation of fluorescent labels in microscopy images
 Home-page: https://github.com/matjesg/deepflash2
 Author: Matthias Griebel
 Author-email: matthias.griebel@uni-wuerzburg.com
 License: Apache Software License 2.0
 Keywords: unet,deep learning,semantic segmentation,microscopy,fluorescent labels
 Classifier: Development Status :: 3 - Alpha
@@ -24,21 +24,20 @@
 ![deepflash2](https://raw.githubusercontent.com/matjesg/deepflash2/master/nbs/media/logo/deepflash2_logo_medium.png)
 
 Official repository of deepflash2 - a deep-learning pipeline for segmentation of ambiguous microscopic images.
 
 [![PyPI](https://img.shields.io/pypi/v/deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/deepflash2/#description) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/deepflash2)](https://pypistats.org/packages/deepflash2)
 [![Conda (channel only)](https://img.shields.io/conda/vn/matjesg/deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/deepflash2)
-[![GitHub stars](https://img.shields.io/github/stars/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
-[![GitHub forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)](https://github.com/matjesg/deepflash2/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)](https://doi.org/10.5281/zenodo.7653312)
 ***
 
 __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for life science researchers. 
-> Read the [paper](https://arxiv.org/abs/2111.06693), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
+> Read the [paper](https://www.nature.com/articles/s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/deepflash2/).    
 - **No coding skills required** (graphical user interface)
 - **Ground truth estimation** from the annotations of multiple experts for model training and validation
 - **Quality assurance and out-of-distribution detection** for reliable prediction on new data 
 - **Best-in-class performance** for semantic and instance segmentation
 
 <img src="https://github.com/matjesg/deepflash2/blob/master/nbs/media/sample_images.png?raw=true" width="800px" style="max-width: 800pxpx">
 
@@ -78,25 +77,30 @@
 | Expected Output | 5 GT Segmentation Masks | 5 models | 5 predicted segmentation masks  (semantic and instance) and uncertainty maps|
 | Estimated Time | ~ 1 min | ~ 150 min | ~ 4 min |
 
 Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU).
 
 ## Paper and Experiments 
 
-We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
+We provide a complete guide to reproduce our experiments using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/tree/master/paper). The data is currently available on [Google Drive](https://drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing) and [Zenodo](https://doi.org/10.5281/zenodo.7653312).
 
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/2111.06693). Please cite
+Our Nature Communications article is available [here](https://www.nature.com/articles/s41467-023-36960-9). Please cite
 
 ```
-@misc{griebel2021deepflash2,
-    title={Deep-learning in the bioimaging wild: Handling ambiguous data with deepflash2}, 
-    author={Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
-    year={2021},
-    eprint={2111.06693},
-    archivePrefix={arXiv}
+@article{Griebel2023,
+  doi = {10.1038/s41467-023-36960-9},
+  url = {https://doi.org/10.1038/s41467-023-36960-9},
+  year = {2023},
+  month = mar,
+  publisher = {Springer Science and Business Media {LLC}},
+  volume = {14},
+  number = {1},
+  author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath},
+  title = {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+  journal = {Nature Communications}
 }
 ```
 
 
 
 ## System requirements
 > Works in the browser or on your local pc/server
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepflash2 Version: 0.2.2 Summary: A Deep learning
+Metadata-Version: 2.1 Name: deepflash2 Version: 0.2.3 Summary: A Deep learning
 pipeline for segmentation of fluorescent labels in microscopy images Home-page:
 https://github.com/matjesg/deepflash2 Author: Matthias Griebel Author-email:
 matthias.griebel@uni-wuerzburg.com License: Apache Software License 2.0
 Keywords: unet,deep learning,semantic segmentation,microscopy,fluorescent
 labels Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
@@ -13,64 +13,66 @@
 repository of deepflash2 - a deep-learning pipeline for segmentation of
 ambiguous microscopic images. [![PyPI](https://img.shields.io/pypi/v/
 deepflash2?color=blue&label=pypi%20version)](https://pypi.org/project/
 deepflash2/#description) [![PyPI - Downloads](https://img.shields.io/pypi/dm/
 deepflash2)](https://pypistats.org/packages/deepflash2) [![Conda (channel
 only)](https://img.shields.io/conda/vn/matjesg/
 deepflash2?color=seagreen&label=conda%20version)](https://anaconda.org/matjesg/
-deepflash2) [![GitHub stars](https://img.shields.io/github/stars/matjesg/
-deepflash2?style=social)](https://github.com/matjesg/deepflash2/) [![GitHub
-forks](https://img.shields.io/github/forks/matjesg/deepflash2?style=social)]
-(https://github.com/matjesg/deepflash2/) *** __The best of two worlds:__
+deepflash2) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7653312.svg)]
+(https://doi.org/10.5281/zenodo.7653312) *** __The best of two worlds:__
 Combining state-of-the-art deep learning with a barrier free environment for
-life science researchers. > Read the [paper](https://arxiv.org/abs/2111.06693),
-watch the [tutorials](https://matjesg.github.io/deepflash2/tutorial.html), or
-read the [docs](https://matjesg.github.io/deepflash2/). - **No coding skills
-required** (graphical user interface) - **Ground truth estimation** from the
-annotations of multiple experts for model training and validation - **Quality
-assurance and out-of-distribution detection** for reliable prediction on new
-data - **Best-in-class performance** for semantic and instance segmentation
-[https://github.com/matjesg/deepflash2/blob/master/nbs/media/
-sample_images.png?raw=true] [https://www.kaggle.com/static/images/medals/
-competitions/goldl@1x.png] **Kaggle Gold Medal and Innovation Price Winner:**
-The *deepflash2* Python API built the foundation for winning the [Innovation
-Award](https://hubmapconsortium.github.io/ccf/pages/kaggle.html) a Kaggle Gold
-Medal in the [HuBMAP - Hacking the Kidney](https://www.kaggle.com/c/hubmap-
-kidney-segmentation) challenge. Have a look at our [solution](https://
-www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ## Quick Start and Demo >
-Get started in less than a minute. Watch the tutorials for help. #### Demo on
-Hugging Face Spaces Go to the [demo space](https://huggingface.co/spaces/
-matjesg/deepflash2) -- inference only (no training possible). #### Demo usage
-with Google Colab For a quick start, run *deepflash2* in Google Colaboratory
-(Google account required). [![Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/matjesg/deepflash2/
-blob/master/deepflash2_GUI.ipynb)  The GUI provides a build-in use for our
-[sample data](https://github.com/matjesg/deepflash2/releases/tag/sample_data).
-1. Starting the GUI (in Colab or follow the installation instructions below) 2.
-Select the task (GT Estimation, Training, or Prediction) 3. Click the `Load
-Sample Data` button in the sidebar and continue to the next sidebar section.
-For futher instructions watch the [tutorials](https://matjesg.github.io/
-deepflash2/tutorial.html). We provide an overview of the tasks below: | |
-Ground Truth (GT) Estimation | Training | Prediction | |---|---|---|---| | Main
-Task | STAPLE or Majority Voting | Ensemble training and validation | Semantic
-and instance segmentation | | Sample Data | 5 masks from 5 experts each | 5
-image/mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
+life science researchers. > Read the [paper](https://www.nature.com/articles/
+s41467-023-36960-9), watch the [tutorials](https://matjesg.github.io/
+deepflash2/tutorial.html), or read the [docs](https://matjesg.github.io/
+deepflash2/). - **No coding skills required** (graphical user interface) -
+**Ground truth estimation** from the annotations of multiple experts for model
+training and validation - **Quality assurance and out-of-distribution
+detection** for reliable prediction on new data - **Best-in-class performance**
+for semantic and instance segmentation [https://github.com/matjesg/deepflash2/
+blob/master/nbs/media/sample_images.png?raw=true] [https://www.kaggle.com/
+static/images/medals/competitions/goldl@1x.png] **Kaggle Gold Medal and
+Innovation Price Winner:** The *deepflash2* Python API built the foundation for
+winning the [Innovation Award](https://hubmapconsortium.github.io/ccf/pages/
+kaggle.html) a Kaggle Gold Medal in the [HuBMAP - Hacking the Kidney](https://
+www.kaggle.com/c/hubmap-kidney-segmentation) challenge. Have a look at our
+[solution](https://www.kaggle.com/matjes/hubmap-deepflash2-judge-price) ##
+Quick Start and Demo > Get started in less than a minute. Watch the tutorials
+for help. #### Demo on Hugging Face Spaces Go to the [demo space](https://
+huggingface.co/spaces/matjesg/deepflash2) -- inference only (no training
+possible). #### Demo usage with Google Colab For a quick start, run
+*deepflash2* in Google Colaboratory (Google account required). [![Colab](https:
+//colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/matjesg/deepflash2/blob/master/
+deepflash2_GUI.ipynb)  The GUI provides a build-in use for our [sample data]
+(https://github.com/matjesg/deepflash2/releases/tag/sample_data). 1. Starting
+the GUI (in Colab or follow the installation instructions below) 2. Select the
+task (GT Estimation, Training, or Prediction) 3. Click the `Load Sample Data`
+button in the sidebar and continue to the next sidebar section. For futher
+instructions watch the [tutorials](https://matjesg.github.io/deepflash2/
+tutorial.html). We provide an overview of the tasks below: | | Ground Truth
+(GT) Estimation | Training | Prediction | |---|---|---|---| | Main Task |
+STAPLE or Majority Voting | Ensemble training and validation | Semantic and
+instance segmentation | | Sample Data | 5 masks from 5 experts each | 5 image/
+mask pairs | 5 images and 2 trained models | | Expected Output | 5 GT
 Segmentation Masks | 5 models | 5 predicted segmentation masks (semantic and
 instance) and uncertainty maps| | Estimated Time | ~ 1 min | ~ 150 min | ~ 4
 min | Times are estimated for Google Colab (with free NVIDIA Tesla K80 GPU). ##
 Paper and Experiments We provide a complete guide to reproduce our experiments
 using the *deepflash2 Python API* [here](https://github.com/matjesg/deepflash2/
 tree/master/paper). The data is currently available on [Google Drive](https://
-drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing).
-The preprint of our paper is available on [arXiv](https://arxiv.org/abs/
-2111.06693). Please cite ``` @misc{griebel2021deepflash2, title={Deep-learning
-in the bioimaging wild: Handling ambiguous data with deepflash2}, author=
-{Matthias Griebel and Dennis Segebarth and Nikolai Stein and Nina Schukraft and
-Philip Tovote and Robert Blum and Christoph M. Flath}, year={2021}, eprint=
-{2111.06693}, archivePrefix={arXiv} } ``` ## System requirements > Works in the
+drive.google.com/drive/folders/1r9AqP9qW9JThbMIvT0jhoA5mPxWEeIjs?usp=sharing)
+and [Zenodo](https://doi.org/10.5281/zenodo.7653312). Our Nature Communications
+article is available [here](https://www.nature.com/articles/s41467-023-36960-
+9). Please cite ``` @article{Griebel2023, doi = {10.1038/s41467-023-36960-9},
+url = {https://doi.org/10.1038/s41467-023-36960-9}, year = {2023}, month = mar,
+publisher = {Springer Science and Business Media {LLC}}, volume = {14}, number
+= {1}, author = {Matthias Griebel and Dennis Segebarth and Nikolai Stein and
+Nina Schukraft and Philip Tovote and Robert Blum and Christoph M. Flath}, title
+= {Deep learning-enabled segmentation of ambiguous bioimages with deepflash2},
+journal = {Nature Communications} } ``` ## System requirements > Works in the
 browser or on your local pc/server *deepflash2* is designed to run on Windows,
 Linux, or Mac (x86-64) if [pytorch](https://pytorch.org/get-started/locally/
 ) is installable. We generally recommend using Google Colab as it only requires
 a Google Account and a device with a web browser. To run *deepflash2* locally,
 we recommend using a system with a GPU (e.g., 2 CPUs, 8 GB RAM, NVIDIA GPU with
 8GB VRAM or better). *deepflash2* requires Python>3.6 and the software
 dependencies are defined in the [settings.ini](https://github.com/matjesg/
```

### Comparing `deepflash2-0.2.2/deepflash2.egg-info/SOURCES.txt` & `deepflash2-0.2.3/deepflash2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepflash2-0.2.2/settings.ini` & `deepflash2-0.2.3/settings.ini`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 user = matjesg
 description = A Deep learning pipeline for segmentation of fluorescent labels in microscopy images
 keywords = unet, deep learning, semantic segmentation, microscopy, fluorescent labels
 author = Matthias Griebel
 author_email = matthias.griebel@uni-wuerzburg.com
 copyright = Würzburg University
 branch = master
-version = 0.2.2
+version = 0.2.3
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = True
 license = apache2
 status = 2
-requirements = fastai>=2.1.7 zarr>=2.0 tifffile==2022.4.8 scikit-image imageio ipywidgets openpyxl imagecodecs albumentations>=1.0.0 natsort>=7.1.1 numba>=0.52.0 opencv-python-headless>=4.1.1,<4.5.5 timm>=0.5.4
+requirements = fastai>=2.1.7 zarr>=2.0 tifffile==2022.4.8 scikit-image imageio ipywidgets openpyxl imagecodecs albumentations>=1.0.0 natsort>=7.1.1 numba>=0.52.0 opencv-python-headless>=4.1.1,<4.5.5 timm==0.6.7
 pip_requirements = segmentation-models-pytorch-deepflash2
 conda_requirements = segmentation_models_pytorch>=0.3.0
 nbs_path = nbs
 doc_path = docs
 doc_host = https://matjesg.github.io
 doc_baseurl = /deepflash2/
 git_url = https://github.com/matjesg/deepflash2/tree/master/
```

### Comparing `deepflash2-0.2.2/setup.py` & `deepflash2-0.2.3/setup.py`

 * *Files identical despite different names*

