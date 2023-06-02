# Comparing `tmp/autora-experimentalist-falsification-1.0.1.tar.gz` & `tmp/autora-experimentalist-falsification-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-falsification-1.0.1.tar", last modified: Thu Jun  1 00:40:35 2023, max compression
+gzip compressed data, was "autora-experimentalist-falsification-1.0.2.tar", last modified: Fri Jun  2 14:13:47 2023, max compression
```

## Comparing `autora-experimentalist-falsification-1.0.1.tar` & `autora-experimentalist-falsification-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   352733 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/basic-usage-pooler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   349559 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/basic-usage-sampler.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/index-pooler.md
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/index-sampler.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/pooler-model-vs-data.png
--rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/pooler-mse.png
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/quickstart-pooler.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs_pooler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs_sampler.yml
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:46.996382 autora-experimentalist-falsification-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:46.996382 autora-experimentalist-falsification-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/docs/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)   352733 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/pooler/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/pooler/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/pooler/model-vs-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/pooler/mse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/pooler/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/docs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)   349559 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/sampler/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/sampler/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/docs/sampler/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:46.996382 autora-experimentalist-falsification-1.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/pooler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/pooler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/pooler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.000383 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/sampler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/sampler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-02 14:13:46.000000 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-02 14:13:46.000000 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:13:46.000000 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-02 14:13:46.000000 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 14:13:46.000000 autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:47.004383 autora-experimentalist-falsification-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/tests/test_exp_falsification_pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-02 14:13:36.000000 autora-experimentalist-falsification-1.0.2/tests/test_exp_falsification_sampler.py
```

### Comparing `autora-experimentalist-falsification-1.0.1/.github/workflows/python-publish.yml` & `autora-experimentalist-falsification-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/.gitignore` & `autora-experimentalist-falsification-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/.pre-commit-config.yaml` & `autora-experimentalist-falsification-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/docs/basic-usage-pooler.ipynb` & `autora-experimentalist-falsification-1.0.2/docs/pooler/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/docs/basic-usage-sampler.ipynb` & `autora-experimentalist-falsification-1.0.2/docs/sampler/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/docs/index-pooler.md` & `autora-experimentalist-falsification-1.0.2/docs/pooler/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 The dataset consists of 100 data points ranging from $X=0$ to $X=2\pi$.
 
 In addition, let's consider a linear regression as a model ($M$) of the data. 
 
 The following figure illustrates the prediction of the fitted linear regression
 (shown in blue) for the pre-collected sine dataset (conditions $X$ and observations $Y$; shown in red):
 
-![Linear Regression vs. Sinus Data](pooler-model-vs-data.png)
+![Linear Regression vs. Sinus Data](model-vs-data.png)
 
 One can observe that the linear regression is a poor fit for the sine data, in particular for regions around the 
 extrema of the sine function, as well as the lower and upper bounds of the domain.
 
 The figure below shows the mean-squared error (MSE) of the linear regression 
 as a function of the input $X$ (red dots):
 
-![MSE of Linear Regression](pooler-mse.png)
+![MSE of Linear Regression](mse.png)
 
 The falsification sampler attempts to predict the MSE of the linear regression using a neural network (shown in blue).
 
 Once the falsiifcaiton sampler has been trained, it can be used to identify novel experimental conditions $X'$ 
 that are predicted to maximize the predicted MSE, such as at the boundaries of the domain, 
 as well as around the extrema of the sine function. An example output of the falsification sampler is:
```

### Comparing `autora-experimentalist-falsification-1.0.1/docs/index-sampler.md` & `autora-experimentalist-falsification-1.0.2/docs/sampler/index.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/docs/pooler-model-vs-data.png` & `autora-experimentalist-falsification-1.0.2/docs/pooler/model-vs-data.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/docs/pooler-mse.png` & `autora-experimentalist-falsification-1.0.2/docs/pooler/mse.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/mkdocs/base.yml` & `autora-experimentalist-falsification-1.0.2/mkdocs/base.yml`

 * *Files 27% similar despite different names*

```diff
@@ -4,26 +4,16 @@
 
 site_name: Autonomous Empirical Research
 repo_url: 'https://github.com/autoresearch/autora'
 
 theme:
   name: material
 
-watch: ["src"]
 
 plugins:
-  gen-files:
-    scripts: [ "mkdocs/gen_ref_pages.py" ]
-  literate-nav:
-    nav_file: SUMMARY.md
-  section-index: {}
-  mkdocstrings:
-      handlers:
-        python: 
-          import: ["https://scikit-learn.org/stable/objects.inv"]
   mkdocs-jupyter:  # required to convert Jupyter notebooks
     include_source: true
     execute: false
     ignore_h1_titles: true
 
 markdown_extensions:
   pymdownx.arithmatex: # required for equation display
```

### Comparing `autora-experimentalist-falsification-1.0.1/pyproject.toml` & `autora-experimentalist-falsification-1.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [project]
 # UPDATE THIS BEFORE PUBLISHING
 name = "autora-experimentalist-falsification"
 description = "AutoRA Falsification Experimentalist"
 authors = [{ name = "Sebastian Musslick", email = "sebastian@musslick.de" }]
 dynamic = ["version"]
-
 readme = "README.md"
 license = { text = "MIT License" }
-requires-python = ">=3.8.10,<3.11"
 
 # ADD NEW DEPENDENCIES HERE
 dependencies = [
     "autora-core",
     "torch"
 ]
```

### Comparing `autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/pooler/falsification/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.2/src/autora/experimentalist/sampler/falsification/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/SOURCES.txt` & `autora-experimentalist-falsification-1.0.2/src/autora_experimentalist_falsification.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
-mkdocs_pooler.yml
-mkdocs_sampler.yml
+mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/basic-usage-pooler.ipynb
-docs/basic-usage-sampler.ipynb
-docs/index-pooler.md
-docs/index-sampler.md
-docs/pooler-model-vs-data.png
-docs/pooler-mse.png
-docs/quickstart-pooler.md
+.github/workflows/test-pytest.yml
 docs/javascripts/mathjax.js
+docs/pooler/Basic Usage.ipynb
+docs/pooler/index.md
+docs/pooler/model-vs-data.png
+docs/pooler/mse.png
+docs/pooler/quickstart.md
+docs/sampler/Basic Usage.ipynb
+docs/sampler/index.md
+docs/sampler/quickstart.md
 mkdocs/base.yml
-mkdocs/gen_ref_pages.py
 src/autora/experimentalist/pooler/falsification/__init__.py
 src/autora/experimentalist/sampler/falsification/__init__.py
 src/autora_experimentalist_falsification.egg-info/PKG-INFO
 src/autora_experimentalist_falsification.egg-info/SOURCES.txt
 src/autora_experimentalist_falsification.egg-info/dependency_links.txt
 src/autora_experimentalist_falsification.egg-info/requires.txt
 src/autora_experimentalist_falsification.egg-info/top_level.txt
```

### Comparing `autora-experimentalist-falsification-1.0.1/tests/README.md` & `autora-experimentalist-falsification-1.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_pooler.py` & `autora-experimentalist-falsification-1.0.2/tests/test_exp_falsification_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_sampler.py` & `autora-experimentalist-falsification-1.0.2/tests/test_exp_falsification_sampler.py`

 * *Files identical despite different names*

