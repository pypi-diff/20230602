# Comparing `tmp/evalplus-0.1.4.tar.gz` & `tmp/evalplus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evalplus-0.1.4.tar", last modified: Fri May 12 04:36:57 2023, max compression
+gzip compressed data, was "evalplus-0.1.5.tar", last modified: Fri Jun  2 08:01:15 2023, max compression
```

## Comparing `evalplus-0.1.4.tar` & `evalplus-0.1.5.tar`

### file list

```diff
@@ -1,64 +1,72 @@
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.4/.dockerignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-09 16:43:25.000000 evalplus-0.1.4/.gitignore
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.4/.pre-commit-config.yaml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1142 2023-05-07 05:34:58.000000 evalplus-0.1.4/CITATION.cff
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.4/Dockerfile
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.4/LICENSE
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.4/MANIFEST.in
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7553 2023-05-12 04:36:57.255550 evalplus-0.1.4/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7106 2023-05-11 05:46:41.000000 evalplus-0.1.4/README.md
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.251550 evalplus-0.1.4/codegen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5418 2023-05-11 05:46:41.000000 evalplus-0.1.4/codegen/generate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    24360 2023-05-12 01:31:35.000000 evalplus-0.1.4/codegen/model.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.4/evalplus/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus/_version.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus/data/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7763 2023-05-10 06:14:35.000000 evalplus-0.1.4/evalplus/data/__init__.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus/eval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6808 2023-05-11 18:15:11.000000 evalplus-0.1.4/evalplus/eval/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.4/evalplus/eval/utils.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8663 2023-05-11 18:15:11.000000 evalplus-0.1.4/evalplus/evaluate.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus/gen/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.4/evalplus/gen/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.4/evalplus/gen/chatgpt_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.4/evalplus/gen/mut_gen.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.4/evalplus/gen/type_mut.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus/gen/util/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.4/evalplus/gen/util/__init__.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.4/evalplus/gen/util/api_request.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.4/evalplus/inputgen.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/evalplus.egg-info/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     7553 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/PKG-INFO
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1133 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/SOURCES.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/dependency_links.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/entry_points.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/requires.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-05-12 04:36:57.000000 evalplus-0.1.4/evalplus.egg-info/top_level.txt
--rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1950 2023-05-12 01:36:16.000000 evalplus-0.1.4/evo.sh
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/gallary/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    96092 2023-05-02 00:08:40.000000 evalplus-0.1.4/gallary/overview.png
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.4/gallary/render.gif
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.4/pyproject.toml
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.4/requirements-llm.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.4/requirements-tools.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.4/requirements.txt
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-05-12 04:36:57.255550 evalplus-0.1.4/setup.cfg
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/tools/
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/tools/_experimental/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.4/tools/_experimental/README.md
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/_experimental/set_cover.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/_experimental/topset_distill.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3428 2023-05-09 21:12:09.000000 evalplus-0.1.4/tools/checker.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/filter_inputs.py
-drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-05-12 04:36:57.255550 evalplus-0.1.4/tools/humaneval/
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/humaneval/check_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/humaneval/init_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.4/tools/init_ground_truth.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.4/tools/merge_dataset.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/render.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3737 2023-05-09 21:15:14.000000 evalplus-0.1.4/tools/sanitize.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.4/tools/stat_plus.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.4/tools/viz_passrate.py
--rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      917 2023-05-11 23:49:16.000000 evalplus-0.1.4/zipper.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3272 2023-05-07 04:41:37.000000 evalplus-0.1.5/.dockerignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3246 2023-05-09 16:43:25.000000 evalplus-0.1.5/.gitignore
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      458 2023-04-28 04:50:47.000000 evalplus-0.1.5/.pre-commit-config.yaml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1142 2023-05-07 05:34:58.000000 evalplus-0.1.5/CITATION.cff
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      290 2023-05-07 04:49:10.000000 evalplus-0.1.5/Dockerfile
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    11357 2023-04-16 19:02:05.000000 evalplus-0.1.5/LICENSE
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       39 2023-05-05 20:10:56.000000 evalplus-0.1.5/MANIFEST.in
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8763 2023-06-02 08:01:15.209326 evalplus-0.1.5/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8316 2023-06-02 08:00:30.000000 evalplus-0.1.5/README.md
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.205326 evalplus-0.1.5/codegen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     5418 2023-05-11 05:46:41.000000 evalplus-0.1.5/codegen/generate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    24360 2023-05-12 01:31:35.000000 evalplus-0.1.5/codegen/model.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.205326 evalplus-0.1.5/evalplus/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      120 2023-05-05 20:05:00.000000 evalplus-0.1.5/evalplus/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      160 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus/_version.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/data/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8038 2023-06-02 07:51:04.000000 evalplus-0.1.5/evalplus/data/__init__.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/eval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6860 2023-05-12 20:25:03.000000 evalplus-0.1.5/evalplus/eval/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     4021 2023-04-28 20:10:51.000000 evalplus-0.1.5/evalplus/eval/utils.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8749 2023-06-02 07:51:04.000000 evalplus-0.1.5/evalplus/evaluate.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/gen/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      753 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3046 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/chatgpt_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1052 2023-04-28 21:16:13.000000 evalplus-0.1.5/evalplus/gen/mut_gen.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)    10484 2023-04-28 20:25:40.000000 evalplus-0.1.5/evalplus/gen/type_mut.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/gen/util/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      722 2023-04-23 03:12:10.000000 evalplus-0.1.5/evalplus/gen/util/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1633 2023-04-28 19:25:35.000000 evalplus-0.1.5/evalplus/gen/util/api_request.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2614 2023-05-05 23:34:50.000000 evalplus-0.1.5/evalplus/inputgen.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus/tsr/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/__init__.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3684 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/coverage_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8091 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/minimization.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3562 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/mutation_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1887 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/run.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2165 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/sample_init.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      614 2023-06-02 07:46:01.000000 evalplus-0.1.5/evalplus/tsr/utils.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/evalplus.egg-info/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     8763 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/PKG-INFO
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1317 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        1 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      104 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/entry_points.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       91 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/requires.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)        9 2023-06-02 08:01:15.000000 evalplus-0.1.5/evalplus.egg-info/top_level.txt
+-rwxrwxr-x   0 jiawei    (1002) jiawei    (1002)     1989 2023-06-02 07:38:42.000000 evalplus-0.1.5/evo.sh
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/gallary/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   100686 2023-06-02 07:18:33.000000 evalplus-0.1.5/gallary/overview.png
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)   403455 2023-04-28 21:23:51.000000 evalplus-0.1.5/gallary/render.gif
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      246 2023-05-05 20:09:10.000000 evalplus-0.1.5/pyproject.toml
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       19 2023-05-05 07:23:28.000000 evalplus-0.1.5/requirements-llm.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       45 2023-05-05 23:33:51.000000 evalplus-0.1.5/requirements-tools.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       49 2023-05-05 23:26:08.000000 evalplus-0.1.5/requirements.txt
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      845 2023-06-02 08:01:15.209326 evalplus-0.1.5/setup.cfg
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/_experimental/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)       33 2023-04-28 19:21:13.000000 evalplus-0.1.5/tools/_experimental/README.md
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3238 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/_experimental/set_cover.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     2405 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/_experimental/topset_distill.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3428 2023-05-09 21:12:09.000000 evalplus-0.1.5/tools/checker.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1598 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/filter_inputs.py
+drwxrwxr-x   0 jiawei    (1002) jiawei    (1002)        0 2023-06-02 08:01:15.209326 evalplus-0.1.5/tools/humaneval/
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1099 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/humaneval/check_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3368 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/humaneval/init_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      844 2023-04-28 20:27:45.000000 evalplus-0.1.5/tools/init_ground_truth.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1340 2023-04-28 20:52:24.000000 evalplus-0.1.5/tools/merge_dataset.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6089 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/render.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     3737 2023-05-09 21:15:14.000000 evalplus-0.1.5/tools/sanitize.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)      741 2023-05-05 23:34:50.000000 evalplus-0.1.5/tools/stat_plus.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     6533 2023-05-01 07:40:47.000000 evalplus-0.1.5/tools/viz_passrate.py
+-rw-rw-r--   0 jiawei    (1002) jiawei    (1002)     1007 2023-06-02 07:51:04.000000 evalplus-0.1.5/zipper.sh
```

### Comparing `evalplus-0.1.4/.dockerignore` & `evalplus-0.1.5/.dockerignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/.gitignore` & `evalplus-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/CITATION.cff` & `evalplus-0.1.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/LICENSE` & `evalplus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/PKG-INFO` & `evalplus-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.4
+Version: 0.1.5
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -114,14 +114,22 @@
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
+🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
+# ...Or locally ⚠️
+# evalplus.evaluate --dataset humaneval --samples samples.jsonl
+```
+
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
@@ -134,14 +142,28 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* We will release an distilled version of HumanEval+ soon. Stay tuned!
+
+</div>
+</details>
+
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.4 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.5 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
 [https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
@@ -39,21 +39,36 @@
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
  To evaluate the samples: You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
 app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
 ...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
-use local GitHub repo? :: click to expand ::
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
+out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
+with the highest quality, achieving almost the same effectiveness of the full
+version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
+you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
+...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
+samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
+ ð¤ How long it would take? :: click to expand ::
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
+8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (~775 on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
+will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
```

### Comparing `evalplus-0.1.4/README.md` & `evalplus-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -100,14 +100,22 @@
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
+🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
+# ...Or locally ⚠️
+# evalplus.evaluate --dataset humaneval --samples samples.jsonl
+```
+
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
@@ -120,14 +128,28 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* We will release an distilled version of HumanEval+ soon. Stay tuned!
+
+</div>
+</details>
+
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
```

#### html2text {}

```diff
@@ -33,21 +33,36 @@
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
  To evaluate the samples: You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
 app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
 ...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
-use local GitHub repo? :: click to expand ::
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
+out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
+with the highest quality, achieving almost the same effectiveness of the full
+version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
+you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
+...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
+samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
+ ð¤ How long it would take? :: click to expand ::
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
+8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (~775 on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
+will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
```

### Comparing `evalplus-0.1.4/codegen/generate.py` & `evalplus-0.1.5/codegen/generate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/codegen/model.py` & `evalplus-0.1.5/codegen/model.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/data/__init__.py` & `evalplus-0.1.5/evalplus/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,22 @@
 CACHE_DIR = user_cache_dir("evalplus")
 
 
 HUMANEVAL_URL = (
     "https://github.com/openai/human-eval/raw/master/data/HumanEval.jsonl.gz"
 )
 HUMANEVAL_PLUS_VERSION = "v0.1.1"
-HUMANEVAL_PLUS_URL = f"https://github.com/ganler/release/releases/download/humanevalplus/HumanEvalPlus-{HUMANEVAL_PLUS_VERSION}.jsonl.gz"
+
+
+def get_dataset_metadata(name, version, mini):
+    assert name in ["HumanEvalPlus"], f"Unknown/unsupported dataset: {name}"
+    extra = "-Mini" if mini else ""
+    url = f"https://github.com/ganler/release/releases/download/humanevalplus/{name}{extra}-{version}.jsonl.gz"
+    cache_path = os.path.join(CACHE_DIR, f"{name}{extra}-{version}.jsonl")
+    return url, cache_path
 
 
 # hacky way to handle \n\r, etc in strings
 def to_raw(string):
     return string.encode("unicode-escape").decode().replace("\\\\", "\\")
 
 
@@ -68,15 +75,15 @@
     contains samples named in `[?].py` where `?` is the solution id starting with 0.
     Different from `sample.jsonl`, the solutions must be complete (with prompt prefix).
     """
 
     # if it is a file
     if os.path.isfile(sample_path):
         for i, sample in enumerate(stream_jsonl(sample_path)):
-            sample["identifier"] = sample["task_id"] + "_" + str(i)
+            sample["_identifier"] = sample["task_id"] + "_" + str(i)
             yield sample
     else:
         # if it is a folder
         for task_id in os.listdir(sample_path):
             task_path = os.path.join(sample_path, task_id)
             if os.path.isdir(task_path):
                 for solution_id in os.listdir(task_path):
@@ -87,27 +94,25 @@
                         yield {
                             "_identifier": solution_path,
                             "task_id": task_id.replace("HumanEval_", "HumanEval/"),
                             "solution": completion,
                         }
 
 
-def _ready_human_eval_plus_path() -> str:
-    plus_path = os.path.join(CACHE_DIR, f"HumanEvalPlus-{HUMANEVAL_PLUS_VERSION}.jsonl")
+def _ready_human_eval_plus_path(mini=False) -> str:
+    url, plus_path = get_dataset_metadata("HumanEvalPlus", HUMANEVAL_PLUS_VERSION, mini)
 
     # Check if human eval file exists in CACHE_DIR
     if not os.path.exists(plus_path):
         # Install HumanEval dataset and parse as jsonl
         # https://github.com/openai/human-eval/blob/master/data/HumanEval.jsonl.gz
         print("Downloading HumanEvalPlus dataset...")
         with tempdir.TempDir() as tmpdir:
-            plus_gz_path = os.path.join(
-                tmpdir, f"HumanEvalPlus-{HUMANEVAL_PLUS_VERSION}.jsonl.gz"
-            )
-            wget.download(HUMANEVAL_PLUS_URL, plus_gz_path)
+            plus_gz_path = os.path.join(tmpdir, f"data.jsonl.gz")
+            wget.download(url, plus_gz_path)
 
             with gzip.open(plus_gz_path, "rb") as f:
                 plus = f.read().decode("utf-8")
 
         # create CACHE_DIR if not exists
         if not os.path.exists(CACHE_DIR):
             os.makedirs(CACHE_DIR)
@@ -126,30 +131,31 @@
     """
     plus_path = _ready_human_eval_plus_path()
     with open(plus_path, "rb") as f:
         plus = f.read()
     return hashlib.md5(plus).hexdigest()
 
 
-def get_human_eval_plus(err_incomplete=True, get_hash=False) -> Dict[str, Dict]:
+def get_human_eval_plus(err_incomplete=True, mini=False) -> Dict[str, Dict]:
     """Get HumanEvalPlus locally.
     Args:
         err_incomplete (bool, optional): Whether to raise error if HumanEvalPlus is not complete. Defaults to True.
+        mini (bool, optional): Whether to use the mini version of HumanEvalPlus. Defaults to False.
     Returns:
         List[Dict[str, str]]: List of dicts with keys "task_id", "prompt", "contract", "canonical_solution", "base_input"
     Notes:
         "task_id" is the identifier string for the task
         "prompt" is the function signature with docstring
         "contract" is the assertions for the function's input (validity)
         "canonical_solution" is the ground-truth implementation for diff-testing
         "base_input" is the test inputs from original HumanEval
         "plus_input" is the test inputs brought by EvalPlus
         "atol" is the absolute tolerance for diff-testing
     """
-    plus_path = _ready_human_eval_plus_path()
+    plus_path = _ready_human_eval_plus_path(mini=mini)
     plus = {task["task_id"]: task for task in stream_jsonl(plus_path)}
     if err_incomplete:
         for task_id, task in plus.items():
             for key in [
                 "prompt",
                 "contract",
                 "canonical_solution",
```

### Comparing `evalplus-0.1.4/evalplus/eval/__init__.py` & `evalplus-0.1.5/evalplus/eval/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,17 +166,19 @@
     inputs: List[Any],
     entry_point: str,
     expected,
     atol,
     ref_time: List[float],
     fast_check: bool = False,
 ) -> Tuple[str, np.ndarray]:
-    min_limit = 0.05 if fast_check else 0.1
+    min_limit = 0.05
     time_limits = [max(min_limit, 2 * t) for t in ref_time]
-    timeout = min(5, sum(ref_time) + 1)
+    timeout = sum(time_limits) + 1
+    if not fast_check:
+        timeout += 1  # extra time for data collection
 
     # shared memory objects
     progress = Value("i", 0)
     stat = Value("i", _UNKNOWN)
     details = Array("b", [False for _ in range(len(inputs))])
 
     p = multiprocessing.Process(
```

### Comparing `evalplus-0.1.4/evalplus/eval/utils.py` & `evalplus-0.1.5/evalplus/eval/utils.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/evaluate.py` & `evalplus-0.1.5/evalplus/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,22 +119,22 @@
     if os.path.isfile(result_path) and not flags.i_just_wanna_run:
         print(f"Load from {result_path}")
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
     else:
-        problems = get_human_eval_plus()
+        problems = get_human_eval_plus(mini=flags.mini)
 
-        problem_hash = get_human_eval_plus_hash()
-        expected_output = get_groundtruth(problems, problem_hash)
+        dataset_hash = get_human_eval_plus_hash()
+        expected_output = get_groundtruth(problems, dataset_hash)
 
         results = {
             "date": datetime.now().strftime("%Y-%m-%d %H:%M"),
-            "hash": problem_hash,
+            "hash": dataset_hash,
             "eval": {},
         }
 
         with ProcessPoolExecutor(max_workers=n_workers) as executor:
             futures = []
             completion_id = Counter()
             n_samples = 0
@@ -152,15 +152,15 @@
                 remainings.add(sample["_identifier"])
                 args = (
                     completion_id[task_id],
                     problems[task_id],
                     solution,
                     expected_output[task_id],
                     flags.base_only,
-                    not flags.full,  # fast_check
+                    not flags.test_details,  # fast_check
                     sample["_identifier"],
                 )
                 futures.append(executor.submit(check_correctness, *args))
                 completion_id[task_id] += 1
                 n_samples += 1
 
             assert n_samples == len(remainings), "Missing problems in unfinished"
@@ -251,15 +251,16 @@
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--dataset", required=True, type=str)
     parser.add_argument("--samples", required=True, type=str)
     parser.add_argument("--base-only", action="store_true")
     parser.add_argument("--parallel", default=None, type=int)
     parser.add_argument("--i-just-wanna-run", action="store_true")
-    parser.add_argument("--full", action="store_true")
+    parser.add_argument("--test-details", action="store_true")
+    parser.add_argument("--mini", action="store_true")
     args = parser.parse_args()
 
     if args.dataset == "humaneval":
         evaluate_humaneval(args)
     else:
         raise NotImplementedError("Unsupported dataset: {}".format(args.dataset))
```

### Comparing `evalplus-0.1.4/evalplus/gen/__init__.py` & `evalplus-0.1.5/evalplus/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/gen/chatgpt_gen.py` & `evalplus-0.1.5/evalplus/gen/chatgpt_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/gen/mut_gen.py` & `evalplus-0.1.5/evalplus/gen/mut_gen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/gen/type_mut.py` & `evalplus-0.1.5/evalplus/gen/type_mut.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/gen/util/__init__.py` & `evalplus-0.1.5/evalplus/gen/util/__init__.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/gen/util/api_request.py` & `evalplus-0.1.5/evalplus/gen/util/api_request.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus/inputgen.py` & `evalplus-0.1.5/evalplus/inputgen.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/evalplus.egg-info/PKG-INFO` & `evalplus-0.1.5/evalplus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalplus
-Version: 0.1.4
+Version: 0.1.5
 Summary: "EvalPlus for rigourous evaluation of LLM-synthesized code"
 Home-page: https://github.com/evalplus/evalplus
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -114,14 +114,22 @@
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 ```bash
 evalplus.evaluate --dataset humaneval --samples samples.jsonl
 ```
 
+🚀 **Try out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests with the highest quality, achieving almost the same effectiveness of the full version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if you evaluate all tests regardless of fail-stop).
+
+```bash
+docker run -v $(pwd):/app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini
+# ...Or locally ⚠️
+# evalplus.evaluate --dataset humaneval --samples samples.jsonl
+```
+
 <details><summary>🤔 Want to use local GitHub repo? <i>:: click to expand ::</i></summary>
 <div>
 
 ```bash
 python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
 
@@ -134,14 +142,28 @@
 * `--parallel`: by default half of the cores
 * `--base-only` (store_ture): only run base HumanEval tests
 * `--i-just-wanna-run`: force a re-run
 
 </div>
 </details>
 
+<details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
+<div>
+
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-8 minute by using `--parallel 64` and `--test-details`.
+Here are some tips to speed up the evaluation:
+
+* Use `--parallel $(nproc)`
+* Do not use `--test-details` if you just want to quickly get pass@k as `--test-details` will run all tests (~775 on average for each task), while without `--test-details` the testing for a sample stops immediately when it fails the first test.
+* Use our pre-evaluated results (see [LLM-generated code](#-LLM-generated-code))
+* We will release an distilled version of HumanEval+ soon. Stay tuned!
+
+</div>
+</details>
+
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Computing expected output...
 Expected outputs computed in 15.18s
 Reading samples...
 164it [00:04, 37.79it/s]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalplus Version: 0.1.4 Summary: "EvalPlus for
+Metadata-Version: 2.1 Name: evalplus Version: 0.1.5 Summary: "EvalPlus for
 rigourous evaluation of LLM-synthesized code" Home-page: https://github.com/
 evalplus/evalplus License: Apache-2.0 Platform: any Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE # `EvalPlus
 (ð) => ð`
 [https://img.shields.io/pypi/v/evalplus?color=g] [https://img.shields.io/pypi/
@@ -39,21 +39,36 @@
 `canonical_solution` is the ground-truth implementation (re-implemented to fix
 bugs in HumanEval) + `base_input` is the test inputs in original HumanEval +
 `plus_input` is the test inputs brought by EvalPlus
  To evaluate the samples: You are strongly recommended to use a sandbox such as
 [docker](https://docs.docker.com/get-docker/): ```bash docker run -v $(pwd):/
 app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl ```
 ...Or if you want to try it locally regardless of the risks â ï¸: ```bash
-evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð¤ Want to
-use local GitHub repo? :: click to expand ::
+evalplus.evaluate --dataset humaneval --samples samples.jsonl ``` ð **Try
+out `HumanEvalPlus-Mini`!** which selects a *minimal* set of additional tests
+with the highest quality, achieving almost the same effectiveness of the full
+version. Just add a **`--mini`** flag, it can run 23+% faster! (even faster if
+you evaluate all tests regardless of fail-stop). ```bash docker run -v $(pwd):/
+app ganler/evalplus:v0.1.1 --dataset humaneval --samples samples.jsonl --mini #
+...Or locally â ï¸ # evalplus.evaluate --dataset humaneval --samples
+samples.jsonl ``` ð¤ Want to use local GitHub repo? :: click to expand ::
 ```bash python evalplus/evaluate.py --dataset humaneval --samples samples.jsonl
 ```
  â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores * `--base-only` (store_ture): only
 run base HumanEval tests * `--i-just-wanna-run`: force a re-run
+ ð¤ How long it would take? :: click to expand ::
+When running 200 samples x 164 tasks x ~775 tests, it can take around 4-
+8 minute by using `--parallel 64` and `--test-details`. Here are some tips to
+speed up the evaluation: * Use `--parallel $(nproc)` * Do not use `--test-
+details` if you just want to quickly get pass@k as `--test-details` will run
+all tests (~775 on average for each task), while without `--test-details` the
+testing for a sample stops immediately when it fails the first test. * Use our
+pre-evaluated results (see [LLM-generated code](#-LLM-generated-code)) * We
+will release an distilled version of HumanEval+ soon. Stay tuned!
  The output should be like (below is GPT-4 greedy decoding example): ```
 Computing expected output... Expected outputs computed in 15.18s Reading
 samples... 164it [00:04, 37.79it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
 164/164 [00:03<00:00, 44.75it/s] Base {'pass@1': 0.8841463414634146} Base +
 Extra {'pass@1': 0.75} ``` - `Base` is the `pass@k` for the original HumanEval
 - `Base + Extra` is the `pass@k` for the our **HumanEval+** (with extra tests)
```

### Comparing `evalplus-0.1.4/evalplus.egg-info/SOURCES.txt` & `evalplus-0.1.5/evalplus.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,21 @@
 evalplus/eval/utils.py
 evalplus/gen/__init__.py
 evalplus/gen/chatgpt_gen.py
 evalplus/gen/mut_gen.py
 evalplus/gen/type_mut.py
 evalplus/gen/util/__init__.py
 evalplus/gen/util/api_request.py
+evalplus/tsr/__init__.py
+evalplus/tsr/coverage_init.py
+evalplus/tsr/minimization.py
+evalplus/tsr/mutation_init.py
+evalplus/tsr/run.py
+evalplus/tsr/sample_init.py
+evalplus/tsr/utils.py
 gallary/overview.png
 gallary/render.gif
 tools/checker.py
 tools/filter_inputs.py
 tools/init_ground_truth.py
 tools/merge_dataset.py
 tools/render.py
```

### Comparing `evalplus-0.1.4/evo.sh` & `evalplus-0.1.5/evo.sh`

 * *Files 6% similar despite different names*

```diff
@@ -34,30 +34,30 @@
 # Set DATADIR and NCORES to default values if they are not provided by the user
 DATADIR=${DATADIR:-$DEFAULT_DATADIR}
 NCORES=${NCORES:-$DEFAULT_NCORES}
 JUST_RUN=${JUST_RUN:-$DEFAULT_JUST_RUN}
 
 export PYTHONPATH=$(pwd)
 
-models=("codegen-2b" "codegen-6b" "codegen-16b" "codegen2-1b"  "codegen2-3b"  "codegen2-7b" "vicuna-7b" "vicuna-13b" "stablelm-7b" "incoder-1b" "incoder-6b" "polycoder" "chatgpt" "starcoder" "santacoder" "gptneo-2b" "gpt-4")
+models=("codegen-2b" "codegen-6b" "codegen-16b" "codegen2-1b"  "codegen2-3b"  "codegen2-7b" "codegen2-16b" "vicuna-7b" "vicuna-13b" "stablelm-7b" "incoder-1b" "incoder-6b" "polycoder" "chatgpt" "starcoder" "santacoder" "gptneo-2b" "gpt-4" "gpt-j")
 temps=("0.0" "0.2" "0.4" "0.6" "0.8")
 
 if [ $JUST_RUN -eq 0 ]; then
   echo "Experiements won't run from scratch since JUST_RUN is set to 0. To run and override all experiements, add -j flag."
 else
   echo "Experiements will run from scratch since JUST_RUN is set to 1. To run without overriding all experiements, remove -j flag."
 fi
 
 for model in "${models[@]}"; do
   for temp in "${temps[@]}"; do
     folder="${DATADIR}/${model}_temp_${temp}"
     if [ -d "$folder" ]; then
       if [ $JUST_RUN -eq 1 ]; then
-        yes | python3 evalplus/evaluate.py --dataset humaneval --samples "$folder" --parallel ${NCORES} --i-just-wanna-run --full
+        yes | python3 evalplus/evaluate.py --dataset humaneval --samples "$folder" --parallel ${NCORES} --i-just-wanna-run --test-details
       else
-        python3 evalplus/evaluate.py --dataset humaneval --samples "$folder" --parallel ${NCORES} --full
+        python3 evalplus/evaluate.py --dataset humaneval --samples "$folder" --parallel ${NCORES} --test-details
       fi
     else
       echo "Folder does not exist: $folder"
     fi
   done
 done
```

### Comparing `evalplus-0.1.4/gallary/render.gif` & `evalplus-0.1.5/gallary/render.gif`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/setup.cfg` & `evalplus-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/_experimental/set_cover.py` & `evalplus-0.1.5/tools/_experimental/set_cover.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/_experimental/topset_distill.py` & `evalplus-0.1.5/tools/_experimental/topset_distill.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/checker.py` & `evalplus-0.1.5/tools/checker.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/filter_inputs.py` & `evalplus-0.1.5/tools/filter_inputs.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/humaneval/check_ground_truth.py` & `evalplus-0.1.5/tools/humaneval/check_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/humaneval/init_plus.py` & `evalplus-0.1.5/tools/humaneval/init_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/init_ground_truth.py` & `evalplus-0.1.5/tools/init_ground_truth.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/merge_dataset.py` & `evalplus-0.1.5/tools/merge_dataset.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/render.py` & `evalplus-0.1.5/tools/render.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/sanitize.py` & `evalplus-0.1.5/tools/sanitize.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/stat_plus.py` & `evalplus-0.1.5/tools/stat_plus.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/tools/viz_passrate.py` & `evalplus-0.1.5/tools/viz_passrate.py`

 * *Files identical despite different names*

### Comparing `evalplus-0.1.4/zipper.sh` & `evalplus-0.1.5/zipper.sh`

 * *Files 24% similar despite different names*

```diff
@@ -19,21 +19,22 @@
       exit 1
       ;;
   esac
 done
 
 DATADIR=${DATADIR:-$DEFAULT_DATADIR}
 
-models=("codegen-2b" "codegen-6b" "codegen-16b" "vicuna-7b" "vicuna-13b" "stablelm-7b" "incoder-1b" "incoder-6b" "polycoder" "chatgpt" "santacoder" "gptneo-2b" "gpt-4")
+# models=("codegen-2b" "codegen-6b" "codegen-16b" "vicuna-7b" "vicuna-13b" "stablelm-7b" "incoder-1b" "incoder-6b" "polycoder" "chatgpt" "santacoder" "gptneo-2b" "gpt-4")
+models=("gpt-j", "starcoder" "codegen2-16b" "codegen2-3b" "codegen2-7b" "codegen2-1b")
 temps=("0.0" "0.2" "0.4" "0.6" "0.8")
 
 for model in "${models[@]}"; do
   for temp in "${temps[@]}"; do
     folder="${DATADIR}/${model}_temp_${temp}"
     if [ -d "$folder" ]; then
         # exclude files with ".json" or ".bak" suffixes
-        zip -r "${folder}.zip" "$folder" -x "*.json" "*.bak"
+        zip -qr "${folder}.zip" "$folder" -x "*.json" "*.bak"
     else
       echo "Folder does not exist: $folder"
     fi
   done
 done
```

