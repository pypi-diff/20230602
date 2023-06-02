# Comparing `tmp/image_ocr-0.0.0.tar.gz` & `tmp/image-ocr-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_ocr-0.0.0.tar", max compression
+gzip compressed data, was "image-ocr-0.0.1.tar", max compression
```

## Comparing `image_ocr-0.0.0.tar` & `image-ocr-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1022 2023-06-02 09:56:30.970258 image_ocr-0.0.0/LICENSE
--rw-r--r--   0        0        0     7324 2023-06-02 10:15:39.328317 image_ocr-0.0.0/README.md
--rw-r--r--   0        0        0      161 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/__init__.py
--rw-r--r--   0        0        0      867 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/config.py
--rw-r--r--   0        0        0    26309 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/data_generation.py
--rw-r--r--   0        0        0    19052 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/datasets.py
--rw-r--r--   0        0        0    30332 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/detection.py
--rw-r--r--   0        0        0     6354 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/evaluation.py
--rw-r--r--   0        0        0     2722 2023-06-02 09:56:30.978258 image_ocr-0.0.0/image_ocr/pipeline.py
--rw-r--r--   0        0        0    21180 2023-06-02 09:56:30.982258 image_ocr-0.0.0/image_ocr/recognition.py
--rw-r--r--   0        0        0    20719 2023-06-02 09:56:30.982258 image_ocr-0.0.0/image_ocr/tools.py
--rw-r--r--   0        0        0     1978 2023-06-02 10:15:38.836304 image_ocr-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     8245 2023-06-02 10:17:57.552855 image_ocr-0.0.0/setup.py
--rw-r--r--   0        0        0     8382 2023-06-02 10:17:57.554180 image_ocr-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1022 2023-06-02 09:56:30.970258 image-ocr-0.0.1/LICENSE
+-rw-r--r--   0        0        0     7324 2023-06-02 10:15:39.328317 image-ocr-0.0.1/README.md
+-rw-r--r--   0        0        0      161 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/__init__.py
+-rw-r--r--   0        0        0      867 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/config.py
+-rw-r--r--   0        0        0    26309 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/data_generation.py
+-rw-r--r--   0        0        0    19052 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/datasets.py
+-rw-r--r--   0        0        0    30332 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/detection.py
+-rw-r--r--   0        0        0     6354 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/evaluation.py
+-rw-r--r--   0        0        0     2722 2023-06-02 09:56:30.978258 image-ocr-0.0.1/image_ocr/pipeline.py
+-rw-r--r--   0        0        0    21161 2023-06-02 14:04:51.114453 image-ocr-0.0.1/image_ocr/recognition.py
+-rw-r--r--   0        0        0    20719 2023-06-02 09:56:30.982258 image-ocr-0.0.1/image_ocr/tools.py
+-rw-r--r--   0        0        0     1978 2023-06-02 14:08:27.088408 image-ocr-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8245 2023-06-02 14:08:53.467471 image-ocr-0.0.1/setup.py
+-rw-r--r--   0        0        0     8382 2023-06-02 14:08:53.468279 image-ocr-0.0.1/PKG-INFO
```

### Comparing `image_ocr-0.0.0/LICENSE` & `image-ocr-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/README.md` & `image-ocr-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/config.py` & `image-ocr-0.0.1/image_ocr/config.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/data_generation.py` & `image-ocr-0.0.1/image_ocr/data_generation.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/datasets.py` & `image-ocr-0.0.1/image_ocr/datasets.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/detection.py` & `image-ocr-0.0.1/image_ocr/detection.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/evaluation.py` & `image-ocr-0.0.1/image_ocr/evaluation.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/pipeline.py` & `image-ocr-0.0.1/image_ocr/pipeline.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/image_ocr/recognition.py` & `image-ocr-0.0.1/image_ocr/recognition.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,16 +79,16 @@
     num_channels = tf.shape(locnet_x)[3]
 
     locnet_y = tf.reshape(locnet_y, shape=(batch_size, 2, 3))
 
     locnet_y = tf.reshape(locnet_y, (-1, 2, 3))
     locnet_y = tf.cast(locnet_y, "float32")
 
-    output_height = output_size[0]
-    output_width = output_size[1]
+    output_height = output_size[0] if output_size[0] else 50
+    output_width = output_size[1] if output_size[1] else 7
     indices_grid = _meshgrid(output_height, output_width)
     indices_grid = tf.expand_dims(indices_grid, 0)
     indices_grid = tf.reshape(indices_grid, [-1])  # flatten?
     indices_grid = tf.tile(indices_grid, tf.stack([batch_size]))
     indices_grid = tf.reshape(indices_grid, tf.stack([batch_size, 3, -1]))
 
     transformed_grid = tf.matmul(locnet_y, indices_grid)
@@ -97,17 +97,14 @@
     x = tf.reshape(x_s, [-1])
     y = tf.reshape(y_s, [-1])
 
     # Interpolate
     height_float = tf.cast(height, dtype="float32")
     width_float = tf.cast(width, dtype="float32")
 
-    output_height = output_size[0]
-    output_width = output_size[1]
-
     x = tf.cast(x, dtype="float32")
     y = tf.cast(y, dtype="float32")
     x = 0.5 * (x + 1.0) * width_float
     y = 0.5 * (y + 1.0) * height_float
 
     x0 = tf.cast(tf.floor(x), "int32")
     x1 = x0 + 1
```

### Comparing `image_ocr-0.0.0/image_ocr/tools.py` & `image-ocr-0.0.1/image_ocr/tools.py`

 * *Files identical despite different names*

### Comparing `image_ocr-0.0.0/pyproject.toml` & `image-ocr-0.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 description = "A packaged and flexible version of the CRAFT text detector and Keras CRNN recognition model."
-homepage = "https://github.com/geo-tp/image_ocr"
+homepage = "https://github.com/geo-tp/image-ocr"
 license = "MIT"
-name = "image_ocr"
+name = "image-ocr"
 readme = "README.md"
-repository = "https://github.com/geo-tp/image_ocr"
+repository = "https://github.com/geo-tp/image-ocr"
 # Placeholder for poetry-dynamic-versioning
-version = "0.0.0"
+version = "0.0.1"
 
 # See https://python-poetry.org/docs/versions/ for allowed version specification formats
 [tool.poetry.dependencies]
 python = ">=3.9"
 validators = "*"
 essential_generators = "*"
 tqdm = "*"
@@ -52,15 +52,15 @@
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [tool.pytest.ini_options]
-addopts = "--cov=image_ocr --cov-report=term-missing"
+addopts = "--cov=keras_ocr --cov-report=term-missing"
 filterwarnings = [
     "ignore:the imp module is deprecated in favour of importlib;:DeprecationWarning"
 ]
 
 [tool.pylint.messages_control]
 disable = [
     "line-too-long",
```

### Comparing `image_ocr-0.0.0/setup.py` & `image-ocr-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
  'pyclipper',
  'shapely',
  'tqdm',
  'validators']
 
 setup_kwargs = {
     'name': 'image-ocr',
-    'version': '0.0.0',
+    'version': '0.0.1',
     'description': 'A packaged and flexible version of the CRAFT text detector and Keras CRNN recognition model.',
     'long_description': "# keras-ocr [![Documentation Status](https://readthedocs.org/projects/keras-ocr/badge/?version=latest)](https://keras-ocr.readthedocs.io/en/latest/?badge=latest)\n\nThis is a slightly polished and packaged version of the [Keras CRNN implementation](https://github.com/kurapan/CRNN) and the published [CRAFT text detection model](https://github.com/clovaai/CRAFT-pytorch). It provides a high level API for training a text detection and OCR pipeline.\n\nPlease see [the documentation](https://keras-ocr.readthedocs.io/) for more examples, including for training a custom model.\n\n## Getting Started\n\n### Installation\n\n`keras-ocr` supports Python >= 3.6 and TensorFlow >= 2.0.0.\n\n```bash\n# To install from master\npip install git+https://github.com/faustomorales/keras-ocr.git#egg=keras-ocr\n\n# To install from PyPi\npip install keras-ocr\n```\n\n### Using\n\nThe package ships with an easy-to-use implementation of the CRAFT text detection model from [this repository](https://github.com/clovaai/CRAFT-pytorch) and the CRNN recognition model from [this repository](https://github.com/kurapan/CRNN).\n\n```python\nimport matplotlib.pyplot as plt\n\nimport image_ocr\n\n# keras-ocr will automatically download pretrained\n# weights for the detector and recognizer.\npipeline = image_ocr.pipeline.Pipeline()\n\n# Get a set of three example images\nimages = [\n    image_ocr.tools.read(url) for url in [\n        'https://upload.wikimedia.org/wikipedia/commons/b/bd/Army_Reserves_Recruitment_Banner_MOD_45156284.jpg',\n        'https://upload.wikimedia.org/wikipedia/commons/e/e8/FseeG2QeLXo.jpg',\n        'https://upload.wikimedia.org/wikipedia/commons/b/b4/EUBanana-500x112.jpg'\n    ]\n]\n\n# Each list of predictions in prediction_groups is a list of\n# (word, box) tuples.\nprediction_groups = pipeline.recognize(images)\n\n# Plot the predictions\nfig, axs = plt.subplots(nrows=len(images), figsize=(20, 20))\nfor ax, image, predictions in zip(axs, images, prediction_groups):\n    image_ocr.tools.drawAnnotations(image=image, predictions=predictions, ax=ax)\n```\n\n![example of labeled image](https://raw.githubusercontent.com/faustomorales/keras-ocr/master/docs/_static/readme_labeled.jpg)\n\n## Comparing keras-ocr and other OCR approaches\n\nYou may be wondering how the models in this package compare to existing cloud OCR APIs. We provide some metrics below and [the notebook](https://drive.google.com/file/d/1FMS3aUZnBU4Tc6bosBPnrjdMoSrjZXRp/view?usp=sharing) used to compute them using the first 1,000 images in the COCO-Text validation set. We limited it to 1,000 because the Google Cloud free tier is for 1,000 calls a month at the time of this writing. As always, caveats apply:\n\n- No guarantees apply to these numbers -- please beware and compute your own metrics independently to verify them. As of this writing, they should be considered a very rough first draft. Please open an issue if you find a mistake. In particular, the cloud APIs have a variety of options that one can use to improve their performance and the responses can be parsed in different ways. It is possible that I made some error in configuration or parsing. Again, please open an issue if you find a mistake!\n- We ignore punctuation and letter case because the out-of-the-box recognizer in keras-ocr (provided by [this independent repository](https://github.com/kurapan/CRNN)) does not support either. Note that both AWS Rekognition and Google Cloud Vision support punctuation as well as upper and lowercase characters.\n- We ignore non-English text.\n- We ignore illegible text.\n\n| model                                                                                                                         | latency | precision | recall |\n| ----------------------------------------------------------------------------------------------------------------------------- | ------- | --------- | ------ |\n| [AWS](https://github.com/faustomorales/keras-ocr/releases/download/v0.8.4/aws_annotations.json)                               | 719ms   | 0.45      | 0.48   |\n| [GCP](https://github.com/faustomorales/keras-ocr/releases/download/v0.8.4/google_annotations.json)                            | 388ms   | 0.53      | 0.58   |\n| [keras-ocr](https://github.com/faustomorales/keras-ocr/releases/download/v0.8.4/image_ocr_annotations_scale_2.json) (scale=2) | 417ms   | 0.53      | 0.54   |\n| [keras-ocr](https://github.com/faustomorales/keras-ocr/releases/download/v0.8.4/image_ocr_annotations_scale_3.json) (scale=3) | 699ms   | 0.5       | 0.59   |\n\n- Precision and recall were computed based on an intersection over union of 50% or higher and a text similarity to ground truth of 50% or higher.\n- `keras-ocr` latency values were computed using a Tesla P4 GPU on Google Colab. `scale` refers to the argument provided to `image_ocr.pipelines.Pipeline()` which determines the upscaling applied to the image prior to inference.\n- Latency for the cloud providers was measured with sequential requests, so you can obtain significant speed improvements by making multiple simultaneous API requests.\n- Each of the entries provides a link to the JSON file containing the annotations made on each pass. You can use this with the notebook to compute metrics without having to make the API calls yourself (though you are encoraged to replicate it independently)!\n\n_Why not compare to Tesseract?_ In every configuration I tried, Tesseract did very poorly on this test. Tesseract performs best on scans of books, not on incidental scene text like that in this dataset.\n\n## Advanced Configuration\nBy default if a GPU is available Tensorflow tries to grab almost all of the available video memory, and this sucks if you're running multiple models with Tensorflow and Pytorch. Setting any value for the environment variable `MEMORY_GROWTH` will force Tensorflow to dynamically allocate only as much GPU memory as is needed.\n\nYou can also specify a limit per Tensorflow process by setting the environment variable `MEMORY_ALLOCATED` to any float, and this value is a float ratio of VRAM to the total amount present.\n\nTo apply these changes, call `image_ocr.config.configure()` at the top of your file where you import `image_ocr`.\n\n## Contributing\n\nTo work on the project, start by doing the following. These instructions probably do not yet work for Windows but if a Windows user has some ideas for how to fix that it would be greatly appreciated (I don't have a Windows machine to test on at the moment).\n\n```bash\n# Install local dependencies for\n# code completion, etc.\nmake init\n\n# Build the Docker container to run\n# tests and such.\nmake build\n```\n\n- You can get a JupyterLab server running to experiment with using `make lab`.\n- To run checks before committing code, you can use `make format-check type-check lint-check test`.\n- To view the documentation, use `make docs`.\n\nTo implement new features, please first file an issue proposing your change for discussion.\n\nTo report problems, please file an issue with sample code, expected results, actual results, and a complete traceback.\n\n## Troubleshooting\n\n- _This package is installing `opencv-python-headless` but I would prefer a different `opencv` flavor._ This is due to [aleju/imgaug#473](https://github.com/aleju/imgaug/issues/473). You can uninstall the unwanted OpenCV flavor after installing `keras-ocr`. We apologize for the inconvenience.\n",
     'author': 'Geo',
     'author_email': 'geoffrey.menon38@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
-    'url': 'https://github.com/geo-tp/image_ocr',
+    'url': 'https://github.com/geo-tp/image-ocr',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.9',
 }
```

### Comparing `image_ocr-0.0.0/PKG-INFO` & `image-ocr-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: image-ocr
-Version: 0.0.0
+Version: 0.0.1
 Summary: A packaged and flexible version of the CRAFT text detector and Keras CRNN recognition model.
-Home-page: https://github.com/geo-tp/image_ocr
+Home-page: https://github.com/geo-tp/image-ocr
 License: MIT
 Author: Geo
 Author-email: geoffrey.menon38@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,15 +21,15 @@
 Requires-Dist: essential_generators
 Requires-Dist: fonttools
 Requires-Dist: imgaug
 Requires-Dist: pyclipper
 Requires-Dist: shapely
 Requires-Dist: tqdm
 Requires-Dist: validators
-Project-URL: Repository, https://github.com/geo-tp/image_ocr
+Project-URL: Repository, https://github.com/geo-tp/image-ocr
 Description-Content-Type: text/markdown
 
 # keras-ocr [![Documentation Status](https://readthedocs.org/projects/keras-ocr/badge/?version=latest)](https://keras-ocr.readthedocs.io/en/latest/?badge=latest)
 
 This is a slightly polished and packaged version of the [Keras CRNN implementation](https://github.com/kurapan/CRNN) and the published [CRAFT text detection model](https://github.com/clovaai/CRAFT-pytorch). It provides a high level API for training a text detection and OCR pipeline.
 
 Please see [the documentation](https://keras-ocr.readthedocs.io/) for more examples, including for training a custom model.
```

