# Comparing `tmp/pyhectiqlab-2.1.7.tar.gz` & `tmp/pyhectiqlab-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/hectiq-lab/hectiq-lab/python-client/dist/.tmp-97xk7y4q/pyhectiqlab-2.1.7.tar", last modified: Thu Apr 20 19:29:33 2023, max compression
+gzip compressed data, was "/home/runner/work/hectiq-lab/hectiq-lab/python-client/dist/.tmp-r9lvckcz/pyhectiqlab-2.1.8.tar", last modified: Fri Jun  2 14:04:28 2023, max compression
```

## Comparing `pyhectiqlab-2.1.7.tar` & `pyhectiqlab-2.1.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/callbacks/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/config_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/events_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/mlmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/notebooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15922 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/paper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/pulse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30465 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyhectiqlab/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:29:13.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/artifacts/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/artifacts/test_img2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/create_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/dataset/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/mlmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img2.jpeg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:29:33.000000 pyhectiqlab-2.1.7/tests/step_artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)   158372 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step1.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   165197 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   726799 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   172506 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step4.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   165748 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step8.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)   153112 2023-04-20 19:29:09.000000 pyhectiqlab-2.1.7/tests/step_artifacts/step9.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab/callbacks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/callbacks/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      115 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/config_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/events_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4629 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/mlmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/notebooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15922 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/pulse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30216 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyhectiqlab/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:04:02.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/artifacts/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/artifacts/test_img2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/create_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/dataset/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/dataset/imgs/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/dataset/imgs/test_img2.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/mlmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/mlmodel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/mlmodel/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/mlmodel/imgs/test_img1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    21603 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/mlmodel/imgs/test_img2.jpeg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:04:28.000000 pyhectiqlab-2.1.8/tests/step_artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)   158372 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step1.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   165197 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   726799 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   172506 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step4.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   165748 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step8.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)   153112 2023-06-02 14:03:52.000000 pyhectiqlab-2.1.8/tests/step_artifacts/step9.jpeg
```

### Comparing `pyhectiqlab-2.1.7/LICENSE` & `pyhectiqlab-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/PKG-INFO` & `pyhectiqlab-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python client to use the Hectiq Lab
 Home-page: https://lab.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/apps.py` & `pyhectiqlab-2.1.8/pyhectiqlab/apps.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/auth.py` & `pyhectiqlab-2.1.8/pyhectiqlab/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/buffer.py` & `pyhectiqlab-2.1.8/pyhectiqlab/buffer.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/callbacks/keras.py` & `pyhectiqlab-2.1.8/pyhectiqlab/callbacks/keras.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/cli/auth.py` & `pyhectiqlab-2.1.8/pyhectiqlab/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/config.py` & `pyhectiqlab-2.1.8/pyhectiqlab/config.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/config_template.py` & `pyhectiqlab-2.1.8/pyhectiqlab/config_template.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/datasets.py` & `pyhectiqlab-2.1.8/pyhectiqlab/datasets.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/decorators.py` & `pyhectiqlab-2.1.8/pyhectiqlab/decorators.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/events_manager.py` & `pyhectiqlab-2.1.8/pyhectiqlab/events_manager.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/metrics.py` & `pyhectiqlab-2.1.8/pyhectiqlab/metrics.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/mlmodels.py` & `pyhectiqlab-2.1.8/pyhectiqlab/mlmodels.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/notebooks.py` & `pyhectiqlab-2.1.8/pyhectiqlab/notebooks.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/ops.py` & `pyhectiqlab-2.1.8/pyhectiqlab/ops.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/paper.py` & `pyhectiqlab-2.1.8/pyhectiqlab/paper.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/pulse.py` & `pyhectiqlab-2.1.8/pyhectiqlab/pulse.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/run.py` & `pyhectiqlab-2.1.8/pyhectiqlab/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,20 +93,14 @@
     def _setup_run(self):
         try:
             assert self.run_view.get('status_code')==200, f'An error occured. {str(self.run_view)}'
 
             if self.run_view.get("is_new", False)==False:
                 print(f"Attaching to an existing run (ID :{self.run_view.get('p_id')}).")
 
-            if self.run_view.get('readonly', True):
-                print("Warning::Run is read only because you are not the author of the run.")
-                self._read_only = True
-                self.setup_read_only()
-                return 
-
             if self.run_view.get('slug', None) is None:
                 print("An error occured while creating the run. Verify the project is correctly spelled and make sure you have access to the project. Switching to read only mode with an empty run.")
                 if self.run_view.get('detail'):
                     print("Error: ", self.run_view.get('detail'))
                 self.setup_read_only()
                 return
         except:
```

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/stream.py` & `pyhectiqlab-2.1.8/pyhectiqlab/stream.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/upload.py` & `pyhectiqlab-2.1.8/pyhectiqlab/upload.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/utils.py` & `pyhectiqlab-2.1.8/pyhectiqlab/utils.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab/watermark.py` & `pyhectiqlab-2.1.8/pyhectiqlab/watermark.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-2.1.8/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python client to use the Hectiq Lab
 Home-page: https://lab.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyhectiqlab-2.1.7/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-2.1.8/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/setup.py` & `pyhectiqlab-2.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
-__version__ = '2.1.7'
+__version__ = '2.1.8'
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
     "requests",
     "tqdm",
```

### Comparing `pyhectiqlab-2.1.7/tests/artifacts/test_img1.jpeg` & `pyhectiqlab-2.1.8/tests/artifacts/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/artifacts/test_img2.jpeg` & `pyhectiqlab-2.1.8/tests/artifacts/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/create_run.py` & `pyhectiqlab-2.1.8/tests/create_run.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/dataset/imgs/test_img1.jpeg` & `pyhectiqlab-2.1.8/tests/dataset/imgs/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/dataset/imgs/test_img2.jpeg` & `pyhectiqlab-2.1.8/tests/dataset/imgs/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img1.jpeg` & `pyhectiqlab-2.1.8/tests/mlmodel/imgs/test_img1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/mlmodel/imgs/test_img2.jpeg` & `pyhectiqlab-2.1.8/tests/mlmodel/imgs/test_img2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step1.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step1.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step2.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step2.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step3.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step3.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step4.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step4.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step8.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step8.jpeg`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-2.1.7/tests/step_artifacts/step9.jpeg` & `pyhectiqlab-2.1.8/tests/step_artifacts/step9.jpeg`

 * *Files identical despite different names*

