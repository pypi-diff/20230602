# Comparing `tmp/hlink-3.3.0.tar.gz` & `tmp/hlink-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlink-3.3.0.tar", last modified: Tue Dec 13 18:44:07 2022, max compression
+gzip compressed data, was "hlink-3.3.1.tar", last modified: Fri Jun  2 16:52:37 2023, max compression
```

## Comparing `hlink-3.3.0.tar` & `hlink-3.3.1.tar`

### file list

```diff
@@ -1,423 +1,424 @@
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:07.213688 hlink-3.3.0/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2022-12-08 21:42:38.000000 hlink-3.3.0/.dockerignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      113 2022-12-09 19:57:55.000000 hlink-3.3.0/.flake8
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:56.764845 hlink-3.3.0/.github/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.749340 hlink-3.3.0/.github/workflows/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      606 2022-12-13 16:04:48.000000 hlink-3.3.0/.github/workflows/docker-build.yml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      244 2022-12-08 21:42:38.000000 hlink-3.3.0/.gitignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      365 2022-12-08 21:42:38.000000 hlink-3.3.0/.pre-commit-config.yaml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      143 2022-12-08 21:42:38.000000 hlink-3.3.0/Dockerfile
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16726 2022-12-08 21:42:38.000000 hlink-3.3.0/LICENSE.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-13 16:10:13.000000 hlink-3.3.0/NOTICE.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25297 2022-12-13 18:44:07.196524 hlink-3.3.0/PKG-INFO
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     5005 2022-12-08 21:58:57.000000 hlink-3.3.0/README.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      107 2022-12-13 16:04:48.000000 hlink-3.3.0/conftest.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.773945 hlink-3.3.0/doc/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4019 2022-12-13 16:04:48.000000 hlink-3.3.0/doc/developer.md
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:58.328439 hlink-3.3.0/docs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      230 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/.buildinfo
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:58.807327 hlink-3.3.0/docs/.doctrees/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    42484 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/column_mapping_transforms.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   163686 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/comparison_types.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   135404 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/config.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    85920 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/environment.pickle
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/example_workflow.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4591 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/feature_selection_transforms.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/index.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8241 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/installation.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9987 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/introduction.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10613 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/link_tasks.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21501 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/models.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8890 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/pipeline_features.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    38499 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/running_the_program.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13195 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/substitutions.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30048 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.doctrees/use_examples.doctree
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/.nojekyll
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:38.000000 hlink-3.3.0/docs/CNAME
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:59.195497 hlink-3.3.0/docs/_sources/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7753 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/column_mapping_transforms.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36495 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/comparison_types.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    28870 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/config.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/feature_selection_transforms.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      750 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/index.rst.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/installation.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/introduction.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/link_tasks.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3609 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/models.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/pipeline_features.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/running_the_program.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/substitutions.md.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.3.0/docs/_sources/use_examples.md.txt
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:59.744084 hlink-3.3.0/docs/_static/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4418 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11185 2022-12-13 16:13:14.000000 hlink-3.3.0/docs/_static/alabaster.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14810 2022-12-13 16:13:14.000000 hlink-3.3.0/docs/_static/basic.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       42 2022-12-06 15:17:39.000000 hlink-3.3.0/docs/_static/custom.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8171 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/doctools.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/_static/documentation_options.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      286 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/file.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   287630 2022-12-08 21:42:39.000000 hlink-3.3.0/docs/_static/jquery-3.5.1.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   288580 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/jquery-3.6.0.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    89501 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/jquery.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4758 2022-12-13 16:13:14.000000 hlink-3.3.0/docs/_static/language_data.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/minus.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/plus.png
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5327 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/_static/pygments.css
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    17120 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/searchtools.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    68420 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/underscore-1.13.1.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19530 2022-12-06 15:25:11.000000 hlink-3.3.0/docs/_static/underscore.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36600 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/column_mapping_transforms.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   117860 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/comparison_types.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    97335 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/config.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14304 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/feature_selection_transforms.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3815 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/genindex.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14996 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/index.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6692 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/installation.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7895 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/introduction.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11432 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/link_tasks.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14355 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/models.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      527 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/objects.inv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9670 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/pipeline_features.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    26121 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/running_the_program.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4092 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/search.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    29129 2022-12-13 18:19:39.000000 hlink-3.3.0/docs/searchindex.js
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9992 2022-12-13 18:19:40.000000 hlink-3.3.0/docs/substitutions.html
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    22022 2022-12-13 18:19:40.000000 hlink-3.3.0/docs/use_examples.html
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:56.821423 hlink-3.3.0/examples/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:59.852742 hlink-3.3.0/examples/tutorial/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:39.000000 hlink-3.3.0/examples/tutorial/.gitignore
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6627 2022-12-08 21:42:39.000000 hlink-3.3.0/examples/tutorial/README.md
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:59.898489 hlink-3.3.0/examples/tutorial/data/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      285 2022-12-08 21:42:39.000000 hlink-3.3.0/examples/tutorial/data/A.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2022-12-08 21:42:39.000000 hlink-3.3.0/examples/tutorial/data/B.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2985 2022-12-09 21:06:40.000000 hlink-3.3.0/examples/tutorial/tutorial.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1012 2022-12-08 21:42:39.000000 hlink-3.3.0/examples/tutorial/tutorial_config.toml
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:59.946213 hlink-3.3.0/hlink/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.154169 hlink-3.3.0/hlink/configs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/configs/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2172 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/configs/load_config.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      479 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/errors.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.325078 hlink-3.3.0/hlink/linking/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      718 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/linking/README.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/linking/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.583377 hlink-3.3.0/hlink/linking/core/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/linking/core/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3406 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/core/classifier.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2068 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/core/column_mapping.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3084 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/linking/core/comparison.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    21403 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/core/comparison_feature.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4196 2022-12-08 21:42:39.000000 hlink-3.3.0/hlink/linking/core/dist_table.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7887 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/core/pipeline.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3865 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/core/substitutions.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4138 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/core/threshold.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    22452 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/core/transforms.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.677013 hlink-3.3.0/hlink/linking/hh_matching/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_matching/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      804 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/hh_matching/hh_matching.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3229 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_matching/link_step_block_on_households.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2234 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/hh_matching/link_step_filter.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.734965 hlink-3.3.0/hlink/linking/hh_matching/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      413 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_matching/templates/hh_blocked_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      566 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_matching/templates/hh_potential_matches.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.781158 hlink-3.3.0/hlink/linking/hh_model_exploration/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      282 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_model_exploration/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      992 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/hh_model_exploration/hh_model_exploration.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.807538 hlink-3.3.0/hlink/linking/hh_model_exploration/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_model_exploration/templates/.gitkeep
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.858543 hlink-3.3.0/hlink/linking/hh_training/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_training/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      940 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/hh_training/hh_training.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.886359 hlink-3.3.0/hlink/linking/hh_training/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/hh_training/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4518 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/link_run.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1699 2022-12-09 17:39:25.000000 hlink-3.3.0/hlink/linking/link_step.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6889 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/link_task.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.015849 hlink-3.3.0/hlink/linking/matching/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/matching/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      519 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/matching/_helpers.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5777 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/matching/link_step_explode.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4228 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/matching/link_step_match.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9301 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/matching/link_step_score.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      658 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/matching/matching.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.111294 hlink-3.3.0/hlink/linking/matching/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      772 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/matching/templates/potential_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      404 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/matching/templates/potential_matches_count.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      503 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/matching/templates/potential_matches_universe.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.289724 hlink-3.3.0/hlink/linking/model_exploration/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/model_exploration/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4731 2022-12-09 21:06:40.000000 hlink-3.3.0/hlink/linking/model_exploration/link_step_create_features.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3520 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/model_exploration/link_step_get_feature_importances.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/model_exploration/link_step_ingest_file.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21393 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/model_exploration/link_step_train_test_models.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      954 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/model_exploration/model_exploration.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.309099 hlink-3.3.0/hlink/linking/model_exploration/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/model_exploration/templates/.gitkeep
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.404656 hlink-3.3.0/hlink/linking/preprocessing/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      270 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4431 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/preprocessing/link_step_prep_dataframes.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7265 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/link_step_register_raw_dfs.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      509 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/preprocessing/preprocessing.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.570441 hlink-3.3.0/hlink/linking/preprocessing/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      431 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/attach_family_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      359 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/attach_neighbor_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      660 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/attach_related_col.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      885 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      471 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/hh_nbor.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      738 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/hh_nbor_rank.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      430 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/preprocessing/templates/training_data_subset.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.691896 hlink-3.3.0/hlink/linking/reporting/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      262 2022-12-08 21:42:40.000000 hlink-3.3.0/hlink/linking/reporting/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/reporting/link_step_export_crosswalk.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3664 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/reporting/link_step_report_r2_percent_linked.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    24145 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/reporting/link_step_report_representivity.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/reporting/reporting.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.715249 hlink-3.3.0/hlink/linking/reporting/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/reporting/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1817 2022-12-09 17:39:25.000000 hlink-3.3.0/hlink/linking/table.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3666 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/table_definitions.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.019762 hlink-3.3.0/hlink/linking/templates/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:01.974749 hlink-3.3.0/hlink/linking/templates/shared/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1003 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/aggregate_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1201 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/all_household_members.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      374 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/attach_variable.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1021 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/drop_links.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2205 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/hh_aggregate_features.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.036952 hlink-3.3.0/hlink/linking/templates/shared/includes/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1586 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1600 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      487 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/pl_easy_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      653 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/potential_matches_base_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      412 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/scored_potential_matches.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/select_columns.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      591 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/tfam_tables.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      702 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/training_features.sql
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      510 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/templates/shared/training_prepped.sql
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.169592 hlink-3.3.0/hlink/linking/training/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/training/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3834 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/training/link_step_create_comparison_features.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/training/link_step_ingest_file.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3061 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/linking/training/link_step_train_and_save_model.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.193929 hlink-3.3.0/hlink/linking/training/templates/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/training/templates/.gitkeep
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      813 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/training/training.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.292957 hlink-3.3.0/hlink/linking/transformers/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/linking/transformers/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1202 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/transformers/float_cast_transformer.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2480 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/transformers/interaction_transformer.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/transformers/rename_prob_column.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      648 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/linking/util.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.366183 hlink-3.3.0/hlink/scripts/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/scripts/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.517904 hlink-3.3.0/hlink/scripts/lib/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/scripts/lib/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14851 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/scripts/lib/conf_validations.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.596968 hlink-3.3.0/hlink/scripts/lib/experimental/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/scripts/lib/experimental/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4044 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/scripts/lib/experimental/reporting.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8493 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/scripts/lib/experimental/tfam.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3252 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/scripts/lib/io.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2704 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/scripts/lib/linking_ops.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5221 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/scripts/lib/table_ops.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      812 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/scripts/lib/util.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     9070 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/scripts/main.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    20516 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/scripts/main_loop.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.656665 hlink-3.3.0/hlink/spark/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/spark/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2494 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/spark/factory.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:02.688128 hlink-3.3.0/hlink/spark/jars/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)  6446850 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/spark/jars/hlink_lib-assembly-1.0.jar
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4786 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/spark/session.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:03.411013 hlink-3.3.0/hlink/tests/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/tests/__init__.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:03.672749 hlink-3.3.0/hlink/tests/conf/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1629 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/tests/conf/integration.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       17 2022-12-08 21:42:41.000000 hlink-3.3.0/hlink/tests/conf/missing_datasource_a.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       87 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/missing_datasource_b.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/no_id_column_a.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/no_id_column_b.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      123 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/test.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       81 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/test1.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      133 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/test_conf_flag_run.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      131 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/conf/test_run.json
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      859 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/conf_validations_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      920 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/config_loader_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    49636 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/tests/conftest.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:03.725533 hlink-3.3.0/hlink/tests/core/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/core/__init__.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10237 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/core/comparison_core_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10639 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/hh_matching_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4245 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/hh_model_exploration_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:05.648130 hlink-3.3.0/hlink/tests/input_data/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      706 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2250 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      221 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/birthyr_replace.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      630 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/calc_mfbpl_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      553 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/calc_mfbpl_b.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:05.756940 hlink-3.3.0/hlink/tests/input_data/conf_validation/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/conf_validation/a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/conf_validation/b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/conf_validation/empty.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      155 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/county_distances.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:05.854056 hlink-3.3.0/hlink/tests/input_data/crosswalk/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/crosswalk/hh_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       53 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/crosswalk/predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/crosswalk/raw_df_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      526 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/crosswalk/raw_df_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       67 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/female.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1034 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/ha_source.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/handle_null.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hb_source.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7441 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hh_matching_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8135 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hh_matching_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hh_predicted_matches_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      231 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hh_year_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      290 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hh_year_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    35038 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/hhpm_agg_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12461 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/households_b.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/integration_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/integration_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      283 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/jw_blocking_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      112 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/jw_blocking_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       32 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/male.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1893 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/matched_men.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3479 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/matching_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1614 2022-12-08 21:42:42.000000 hlink-3.3.0/hlink/tests/input_data/matching_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      196 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/nativity_test_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      208 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/nativity_test_data_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    87678 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/new_hh_test_td.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      255 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/popularity.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3712 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/potential_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4634 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/potential_matches_agg.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/potential_matches_ids_only.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      254 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/potential_matches_sql_condition_marst_warn.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/predicted_matches_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      332 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/predicted_matches_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1068 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/prepped_df_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      534 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/raw_df_reporting.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1022 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/region.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      361 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/regioncode.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39511 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/rel_rows_test_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33360 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/rel_rows_test_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/reporting_hh_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/reporting_predicted_matches.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      302 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/reporting_prepped_df_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6834 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/representivity.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      379 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/scored_matches_household_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      109 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/scored_matches_test_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      304 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/sql_condition_marst_warn_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      227 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/sql_condition_marst_warn_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    46345 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/statedist.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6776 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/street_abbrevs.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      820 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/street_abbrevs_most_common.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_csv_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       88 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_csv_data_b.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:05.942116 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/.part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1140 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.027862 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/.part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1116 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       94 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_prepped_data_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       97 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_prepped_data_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      159 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/test_street_names_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      234 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/threshold_ratio_test.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      191 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/threshold_ratio_test_data_2.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      180 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_doubled.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5567 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_households.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13866 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_households.parquet
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1863 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_long.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1527 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_long_a.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1472 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/input_data/training_data_long_b.csv
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36252 2022-12-08 21:42:43.000000 hlink-3.3.0/hlink/tests/integration_score_with_trained_models_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1488 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/integration_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      395 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/linking_util_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/logging_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4973 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/main_loop_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9909 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/main_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4216 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/matching_blocking_explode_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    42082 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/matching_comparison_features_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    14145 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/matching_geo_distance_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3065 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/matching_potential_matches_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2624 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/matching_potential_matches_universe_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6715 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/matching_scoring_test.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     7111 2022-12-09 21:06:41.000000 hlink-3.3.0/hlink/tests/matching_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    23929 2022-12-13 16:04:48.000000 hlink-3.3.0/hlink/tests/model_exploration_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.105105 hlink-3.3.0/hlink/tests/plugins/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/plugins/__init__.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    29857 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/plugins/datasources.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    12650 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/plugins/external_data_paths.py
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    62284 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/preprocessing_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3512 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/reporting_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1163 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/scala_udf_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2490 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/table_test.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7406 2022-12-09 21:06:42.000000 hlink-3.3.0/hlink/tests/training_test.py
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.324024 hlink-3.3.0/hlink/tests/validation_data/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.155652 hlink-3.3.0/hlink/tests/validation_data/crosswalks/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      106 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/crosswalks/crosswalk.csv
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      126 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/crosswalks/crosswalk_with_round.csv
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.267956 hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/._SUCCESS.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      116 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/.part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet.crc
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/_SUCCESS
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13348 2022-12-08 21:42:44.000000 hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:00.109546 hlink-3.3.0/hlink.egg-info/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25297 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/PKG-INFO
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14774 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/SOURCES.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        1 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/dependency_links.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       49 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/entry_points.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      238 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/requires.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       19 2022-12-13 18:43:56.000000 hlink-3.3.0/hlink.egg-info/top_level.txt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1179 2022-12-13 18:19:40.000000 hlink-3.3.0/pyproject.toml
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      110 2022-12-08 21:42:44.000000 hlink-3.3.0/pytest.ini
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.302564 hlink-3.3.0/scala_jar/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3774 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/build.sbt
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.359181 hlink-3.3.0/scala_jar/project/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/project/assembly.sbt
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       18 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/project/build.properties
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.365932 hlink-3.3.0/scala_jar/src/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.371321 hlink-3.3.0/scala_jar/src/main/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.382570 hlink-3.3.0/scala_jar/src/main/scala/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.386097 hlink-3.3.0/scala_jar/src/main/scala/com/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:43:57.394948 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:06.790576 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      535 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2249 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3382 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3170 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      556 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1494 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      703 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      764 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      889 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      473 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/JWCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      898 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1689 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      662 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      549 2022-12-08 21:42:44.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:45.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      545 2022-12-08 21:42:45.000000 hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2022-12-13 18:44:07.220485 hlink-3.3.0/setup.cfg
-drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2022-12-13 18:44:07.165314 hlink-3.3.0/sphinx-docs/
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      692 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/Makefile
--rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     7753 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/column_mapping_transforms.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36495 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/comparison_types.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2106 2022-12-09 21:06:42.000000 hlink-3.3.0/sphinx-docs/conf.py
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    28870 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/config.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/feature_selection_transforms.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      750 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/index.rst
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/installation.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/introduction.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/link_tasks.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      795 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/make.bat
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3609 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/models.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/pipeline_features.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/running_the_program.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/substitutions.md
--rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.3.0/sphinx-docs/use_examples.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:37.846302 hlink-3.3.1/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2022-12-08 21:42:38.000000 hlink-3.3.1/.dockerignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      113 2022-12-09 19:57:55.000000 hlink-3.3.1/.flake8
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:28.924366 hlink-3.3.1/.github/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.616162 hlink-3.3.1/.github/workflows/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      606 2022-12-13 16:04:48.000000 hlink-3.3.1/.github/workflows/docker-build.yml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      244 2022-12-08 21:42:38.000000 hlink-3.3.1/.gitignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      365 2022-12-08 21:42:38.000000 hlink-3.3.1/.pre-commit-config.yaml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      143 2022-12-08 21:42:38.000000 hlink-3.3.1/Dockerfile
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    16726 2022-12-08 21:42:38.000000 hlink-3.3.1/LICENSE.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-13 16:10:13.000000 hlink-3.3.1/NOTICE.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25515 2023-06-02 16:52:37.840112 hlink-3.3.1/PKG-INFO
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     5198 2023-05-04 18:45:31.000000 hlink-3.3.1/README.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      107 2022-12-13 16:04:48.000000 hlink-3.3.1/conftest.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.638100 hlink-3.3.1/doc/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4019 2022-12-13 16:04:48.000000 hlink-3.3.1/doc/developer.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:30.138183 hlink-3.3.1/docs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      230 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/.buildinfo
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:30.677325 hlink-3.3.1/docs/.doctrees/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    42484 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/column_mapping_transforms.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   163686 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/comparison_types.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   135404 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/config.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    85920 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/environment.pickle
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/example_workflow.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4591 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/feature_selection_transforms.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5278 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/index.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8241 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/installation.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9987 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/introduction.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10613 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/link_tasks.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21501 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/models.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8890 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/pipeline_features.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    38499 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/running_the_program.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13195 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/substitutions.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    30048 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.doctrees/use_examples.doctree
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/.nojekyll
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:38.000000 hlink-3.3.1/docs/CNAME
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:30.990396 hlink-3.3.1/docs/_sources/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8048 2023-05-12 14:35:46.000000 hlink-3.3.1/docs/_sources/column_mapping_transforms.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36878 2023-05-19 15:08:30.000000 hlink-3.3.1/docs/_sources/comparison_types.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    28870 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/config.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/feature_selection_transforms.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      750 2023-05-05 17:56:58.000000 hlink-3.3.1/docs/_sources/index.rst.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/installation.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/introduction.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/link_tasks.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3609 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/models.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/pipeline_features.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/running_the_program.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/substitutions.md.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.3.1/docs/_sources/use_examples.md.txt
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.399249 hlink-3.3.1/docs/_static/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4418 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11230 2023-06-02 16:21:42.000000 hlink-3.3.1/docs/_static/alabaster.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14810 2023-06-02 16:21:42.000000 hlink-3.3.1/docs/_static/basic.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       42 2023-05-04 19:24:37.000000 hlink-3.3.1/docs/_static/custom.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8171 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/doctools.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/_static/documentation_options.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      286 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/file.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   287630 2022-12-08 21:42:39.000000 hlink-3.3.1/docs/_static/jquery-3.5.1.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   288580 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/jquery-3.6.0.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    89501 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/jquery.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4758 2023-06-02 16:21:42.000000 hlink-3.3.1/docs/_static/language_data.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/minus.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/plus.png
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5327 2023-06-02 16:21:42.000000 hlink-3.3.1/docs/_static/pygments.css
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    17120 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/searchtools.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    68420 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/underscore-1.13.1.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    19530 2023-05-04 19:27:45.000000 hlink-3.3.1/docs/_static/underscore.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    31062 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/column_mapping_transforms.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)   118856 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/comparison_types.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    97335 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/config.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14304 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/feature_selection_transforms.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3815 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/genindex.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14996 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/index.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6692 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/installation.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7895 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/introduction.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11432 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/link_tasks.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14355 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/models.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      527 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/objects.inv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9670 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/pipeline_features.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    26167 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/running_the_program.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4092 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/search.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    28136 2023-06-02 16:21:42.000000 hlink-3.3.1/docs/searchindex.js
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9992 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/substitutions.html
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    22781 2023-06-02 16:37:27.000000 hlink-3.3.1/docs/use_examples.html
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:28.973401 hlink-3.3.1/examples/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.486832 hlink-3.3.1/examples/tutorial/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:39.000000 hlink-3.3.1/examples/tutorial/.gitignore
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6627 2022-12-08 21:42:39.000000 hlink-3.3.1/examples/tutorial/README.md
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.537284 hlink-3.3.1/examples/tutorial/data/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      285 2022-12-08 21:42:39.000000 hlink-3.3.1/examples/tutorial/data/A.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      226 2022-12-08 21:42:39.000000 hlink-3.3.1/examples/tutorial/data/B.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2985 2022-12-09 21:06:40.000000 hlink-3.3.1/examples/tutorial/tutorial.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1012 2022-12-08 21:42:39.000000 hlink-3.3.1/examples/tutorial/tutorial_config.toml
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.571885 hlink-3.3.1/hlink/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.757837 hlink-3.3.1/hlink/configs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/configs/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2172 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/configs/load_config.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      479 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/errors.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.947503 hlink-3.3.1/hlink/linking/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      718 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/linking/README.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/linking/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.162671 hlink-3.3.1/hlink/linking/core/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/linking/core/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3406 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/core/classifier.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2068 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/core/column_mapping.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3084 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/linking/core/comparison.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    21403 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/core/comparison_feature.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4196 2022-12-08 21:42:39.000000 hlink-3.3.1/hlink/linking/core/dist_table.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8115 2023-06-02 15:34:48.000000 hlink-3.3.1/hlink/linking/core/pipeline.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3865 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/core/substitutions.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4138 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/core/threshold.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    22452 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/core/transforms.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.283971 hlink-3.3.1/hlink/linking/hh_matching/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_matching/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      804 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/hh_matching/hh_matching.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3229 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_matching/link_step_block_on_households.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2234 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/hh_matching/link_step_filter.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.338139 hlink-3.3.1/hlink/linking/hh_matching/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      413 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_matching/templates/hh_blocked_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      566 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_matching/templates/hh_potential_matches.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.381641 hlink-3.3.1/hlink/linking/hh_model_exploration/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      282 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_model_exploration/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      992 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/hh_model_exploration/hh_model_exploration.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.404213 hlink-3.3.1/hlink/linking/hh_model_exploration/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_model_exploration/templates/.gitkeep
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.447548 hlink-3.3.1/hlink/linking/hh_training/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      265 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_training/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      940 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/hh_training/hh_training.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.471614 hlink-3.3.1/hlink/linking/hh_training/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/hh_training/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4518 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/link_run.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1699 2022-12-09 17:39:25.000000 hlink-3.3.1/hlink/linking/link_step.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6889 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/link_task.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.602356 hlink-3.3.1/hlink/linking/matching/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/matching/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      519 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/matching/_helpers.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5777 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/matching/link_step_explode.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4228 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/matching/link_step_match.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9301 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/matching/link_step_score.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      658 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/matching/matching.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.676019 hlink-3.3.1/hlink/linking/matching/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      772 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/matching/templates/potential_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      404 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/matching/templates/potential_matches_count.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      503 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/matching/templates/potential_matches_universe.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.807333 hlink-3.3.1/hlink/linking/model_exploration/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/model_exploration/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4731 2022-12-09 21:06:40.000000 hlink-3.3.1/hlink/linking/model_exploration/link_step_create_features.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3520 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/model_exploration/link_step_get_feature_importances.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/model_exploration/link_step_ingest_file.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    21393 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/model_exploration/link_step_train_test_models.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      954 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/model_exploration/model_exploration.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.828423 hlink-3.3.1/hlink/linking/model_exploration/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/model_exploration/templates/.gitkeep
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:32.922326 hlink-3.3.1/hlink/linking/preprocessing/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      270 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4431 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/preprocessing/link_step_prep_dataframes.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7265 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/link_step_register_raw_dfs.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      509 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/preprocessing/preprocessing.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.087891 hlink-3.3.1/hlink/linking/preprocessing/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      431 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/attach_family_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      359 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/attach_neighbor_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      660 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/attach_related_col.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      885 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      471 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/hh_nbor.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      738 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/hh_nbor_rank.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      430 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/preprocessing/templates/training_data_subset.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.191422 hlink-3.3.1/hlink/linking/reporting/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      262 2022-12-08 21:42:40.000000 hlink-3.3.1/hlink/linking/reporting/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/reporting/link_step_export_crosswalk.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3664 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/reporting/link_step_report_r2_percent_linked.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    24145 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/reporting/link_step_report_representivity.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/reporting/reporting.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.214934 hlink-3.3.1/hlink/linking/reporting/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/reporting/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1817 2022-12-09 17:39:25.000000 hlink-3.3.1/hlink/linking/table.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3666 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/table_definitions.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.126095 hlink-3.3.1/hlink/linking/templates/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.453499 hlink-3.3.1/hlink/linking/templates/shared/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1003 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/aggregate_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1201 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/all_household_members.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      374 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/attach_variable.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1021 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/drop_links.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2205 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/hh_aggregate_features.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.491412 hlink-3.3.1/hlink/linking/templates/shared/includes/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1586 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1600 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      487 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/pl_easy_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      653 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/potential_matches_base_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      412 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/scored_potential_matches.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      420 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/select_columns.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      591 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/tfam_tables.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      702 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/training_features.sql
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      510 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/templates/shared/training_prepped.sql
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.586873 hlink-3.3.1/hlink/linking/training/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      260 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/training/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3834 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/training/link_step_create_comparison_features.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      872 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/training/link_step_ingest_file.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3061 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/linking/training/link_step_train_and_save_model.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.605512 hlink-3.3.1/hlink/linking/training/templates/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/training/templates/.gitkeep
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      813 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/training/training.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.690169 hlink-3.3.1/hlink/linking/transformers/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/linking/transformers/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1202 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/transformers/float_cast_transformer.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2480 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/transformers/interaction_transformer.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      615 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/transformers/rename_prob_column.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      648 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/linking/util.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.752762 hlink-3.3.1/hlink/scripts/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/scripts/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.887339 hlink-3.3.1/hlink/scripts/lib/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/scripts/lib/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14851 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/scripts/lib/conf_validations.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:33.938335 hlink-3.3.1/hlink/scripts/lib/experimental/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/scripts/lib/experimental/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4044 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/scripts/lib/experimental/reporting.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8493 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/scripts/lib/experimental/tfam.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3252 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/scripts/lib/io.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2704 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/scripts/lib/linking_ops.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5221 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/scripts/lib/table_ops.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      812 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/scripts/lib/util.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     8340 2023-06-02 15:34:49.000000 hlink-3.3.1/hlink/scripts/main.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    20520 2023-06-02 15:34:49.000000 hlink-3.3.1/hlink/scripts/main_loop.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:34.052100 hlink-3.3.1/hlink/spark/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/spark/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2494 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/spark/factory.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:34.072985 hlink-3.3.1/hlink/spark/jars/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)  6446850 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/spark/jars/hlink_lib-assembly-1.0.jar
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4786 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/spark/session.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:34.644456 hlink-3.3.1/hlink/tests/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/tests/__init__.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:34.834931 hlink-3.3.1/hlink/tests/conf/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1629 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/tests/conf/integration.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       17 2022-12-08 21:42:41.000000 hlink-3.3.1/hlink/tests/conf/missing_datasource_a.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       87 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/missing_datasource_b.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/no_id_column_a.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      258 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/no_id_column_b.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      123 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/test.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       81 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/test1.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      133 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/test_conf_flag_run.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      131 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/conf/test_run.json
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      859 2023-05-05 19:00:53.000000 hlink-3.3.1/hlink/tests/conf_validations_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      920 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/config_loader_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    49636 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/tests/conftest.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:34.890271 hlink-3.3.1/hlink/tests/core/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/core/__init__.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10237 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/core/comparison_core_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1200 2023-06-02 15:34:49.000000 hlink-3.3.1/hlink/tests/core/pipeline_core_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    10639 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/hh_matching_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4245 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/hh_model_exploration_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.449693 hlink-3.3.1/hlink/tests/input_data/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      706 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2250 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      221 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/birthyr_replace.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      630 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/calc_mfbpl_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      553 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/calc_mfbpl_b.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.522415 hlink-3.3.1/hlink/tests/input_data/conf_validation/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/conf_validation/a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/conf_validation/b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/conf_validation/empty.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      155 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/county_distances.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.615007 hlink-3.3.1/hlink/tests/input_data/crosswalk/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       29 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/crosswalk/hh_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       53 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/crosswalk/predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/crosswalk/raw_df_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      526 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/crosswalk/raw_df_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       67 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/female.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1034 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/ha_source.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      687 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/handle_null.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hb_source.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7441 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hh_matching_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     8135 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hh_matching_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hh_predicted_matches_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      231 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hh_year_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      290 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hh_year_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    35038 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/hhpm_agg_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    12461 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/households_b.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/integration_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/integration_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      283 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/jw_blocking_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      112 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/jw_blocking_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       32 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/male.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1893 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/matched_men.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3479 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/matching_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1614 2022-12-08 21:42:42.000000 hlink-3.3.1/hlink/tests/input_data/matching_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      196 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/nativity_test_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      208 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/nativity_test_data_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    87678 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/new_hh_test_td.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      255 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/popularity.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3712 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/potential_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     4634 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/potential_matches_agg.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/potential_matches_ids_only.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      254 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/potential_matches_sql_condition_marst_warn.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       82 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/predicted_matches_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      332 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/predicted_matches_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1068 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/prepped_df_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      534 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/raw_df_reporting.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1022 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/region.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      361 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/regioncode.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    39511 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/rel_rows_test_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    33360 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/rel_rows_test_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       75 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/reporting_hh_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      102 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/reporting_predicted_matches.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      302 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/reporting_prepped_df_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6834 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/representivity.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      379 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/scored_matches_household_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      109 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/scored_matches_test_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      304 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/sql_condition_marst_warn_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      227 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/sql_condition_marst_warn_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    46345 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/statedist.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     6776 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/street_abbrevs.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      820 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/street_abbrevs_most_common.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       90 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_csv_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       88 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_csv_data_b.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.709310 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/.part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1140 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.799649 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       20 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/.part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1116 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       94 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_prepped_data_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       97 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_prepped_data_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      159 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/test_street_names_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      234 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/threshold_ratio_test.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      191 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/threshold_ratio_test_data_2.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       99 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      180 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_doubled.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     5567 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_households.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13866 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_households.parquet
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1863 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_long.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1527 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_long_a.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1472 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/input_data/training_data_long_b.csv
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36252 2022-12-08 21:42:43.000000 hlink-3.3.1/hlink/tests/integration_score_with_trained_models_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1488 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/integration_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      395 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/linking_util_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      514 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/logging_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4973 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/main_loop_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     9909 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/main_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     4216 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/matching_blocking_explode_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    42082 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/matching_comparison_features_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    14145 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/matching_geo_distance_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3065 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/matching_potential_matches_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     2624 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/matching_potential_matches_universe_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     6715 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/matching_scoring_test.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     7111 2022-12-09 21:06:41.000000 hlink-3.3.1/hlink/tests/matching_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    23929 2022-12-13 16:04:48.000000 hlink-3.3.1/hlink/tests/model_exploration_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.847623 hlink-3.3.1/hlink/tests/plugins/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/plugins/__init__.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    29857 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/plugins/datasources.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    12650 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/plugins/external_data_paths.py
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)    62284 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/preprocessing_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3512 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/reporting_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1163 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/scala_udf_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2490 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/table_test.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7406 2022-12-09 21:06:42.000000 hlink-3.3.1/hlink/tests/training_test.py
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.286161 hlink-3.3.1/hlink/tests/validation_data/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.897381 hlink-3.3.1/hlink/tests/validation_data/crosswalks/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      106 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/crosswalks/crosswalk.csv
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      126 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/crosswalks/crosswalk_with_round.csv
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:36.980136 hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        8 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/._SUCCESS.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      116 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/.part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet.crc
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        0 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/_SUCCESS
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    13348 2022-12-08 21:42:44.000000 hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:31.711573 hlink-3.3.1/hlink.egg-info/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    25515 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/PKG-INFO
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    14813 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/SOURCES.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)        1 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/dependency_links.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       49 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/entry_points.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      238 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/requires.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       19 2023-06-02 16:52:28.000000 hlink-3.3.1/hlink.egg-info/top_level.txt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1179 2023-06-02 16:37:27.000000 hlink-3.3.1/pyproject.toml
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      110 2022-12-08 21:42:44.000000 hlink-3.3.1/pytest.ini
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:37.003133 hlink-3.3.1/scala_jar/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3774 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/build.sbt
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:37.045615 hlink-3.3.1/scala_jar/project/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      277 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/project/assembly.sbt
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       18 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/project/build.properties
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.316331 hlink-3.3.1/scala_jar/src/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.325185 hlink-3.3.1/scala_jar/src/main/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.333142 hlink-3.3.1/scala_jar/src/main/scala/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.342315 hlink-3.3.1/scala_jar/src/main/scala/com/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:29.351669 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:37.438774 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      535 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2249 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     3382 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3170 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      556 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1494 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      703 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)      764 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      889 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      473 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/JWCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      898 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1689 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      662 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      549 2022-12-08 21:42:44.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1272 2022-12-08 21:42:45.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      545 2022-12-08 21:42:45.000000 hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)       38 2023-06-02 16:52:37.853626 hlink-3.3.1/setup.cfg
+drwxrwxr-x   0 rileyh   (42243) rileyh   (23521)        0 2023-06-02 16:52:37.809917 hlink-3.3.1/sphinx-docs/
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      692 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/Makefile
+-rwxrwxr-x   0 rileyh   (42243) rileyh   (23521)     8048 2023-05-12 14:35:46.000000 hlink-3.3.1/sphinx-docs/column_mapping_transforms.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    36878 2023-05-19 15:08:30.000000 hlink-3.3.1/sphinx-docs/comparison_types.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2106 2023-05-15 18:17:14.000000 hlink-3.3.1/sphinx-docs/conf.py
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    28870 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/config.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2773 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/feature_selection_transforms.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      750 2023-05-05 17:56:58.000000 hlink-3.3.1/sphinx-docs/index.rst
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      989 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/installation.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2574 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/introduction.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     2874 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/link_tasks.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)      795 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/make.bat
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     3609 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/models.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1731 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/pipeline_features.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)    11301 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/running_the_program.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     1978 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/substitutions.md
+-rw-rw-r--   0 rileyh   (42243) rileyh   (23521)     7114 2022-12-08 21:42:45.000000 hlink-3.3.1/sphinx-docs/use_examples.md
```

### Comparing `hlink-3.3.0/.github/workflows/docker-build.yml` & `hlink-3.3.1/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/LICENSE.txt` & `hlink-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/NOTICE.txt` & `hlink-3.3.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/PKG-INFO` & `hlink-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlink
-Version: 3.3.0
+Version: 3.3.1
 Summary: Fast supervised pyspark record linkage software
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
         
@@ -382,24 +382,28 @@
 Project-URL: Changelog, https://github.com/ipums/hlink/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: NOTICE.txt
 
 [![HLink Docker CI](https://github.com/ipums/hlink/actions/workflows/docker-build.yml/badge.svg)](https://github.com/ipums/hlink/actions/workflows/docker-build.yml)
 
 # hlink: hierarchical record linkage at scale
 
 hlink is a Python package that provides a flexible, configuration-driven solution to probabilistic record linking at scale. It provides a high-level API for python as well as a standalone command line interface for running linking jobs with little to no programming. hlink supports the linking process from beginning to end, including preprocessing, filtering, training, model exploration, blocking, feature generation and scoring.
 
 It is used at [IPUMS](https://www.ipums.org/) to link U.S. historical census data, but can be applied to any record linkage job. 
 A paper on the creation and applications of this program on historical census data can be found at <https://www.tandfonline.com/doi/full/10.1080/01615440.2021.1985027>.
 
+### Suggested Citation
+Wellington, J., R. Harper, and K.J. Thompson. 2022. "hlink." https://github.com/ipums/hlink: Institute for Social Research and Data Innovation, University of Minnesota.
+
 ## Installation
 
 hlink runs on Python 3.10.
 Java 8 or [Java 11](https://openjdk.org/install/) is required for the PySpark integration. 
 
 You can install the python package from pip:
 ```
```

### Comparing `hlink-3.3.0/README.md` & `hlink-3.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 # hlink: hierarchical record linkage at scale
 
 hlink is a Python package that provides a flexible, configuration-driven solution to probabilistic record linking at scale. It provides a high-level API for python as well as a standalone command line interface for running linking jobs with little to no programming. hlink supports the linking process from beginning to end, including preprocessing, filtering, training, model exploration, blocking, feature generation and scoring.
 
 It is used at [IPUMS](https://www.ipums.org/) to link U.S. historical census data, but can be applied to any record linkage job. 
 A paper on the creation and applications of this program on historical census data can be found at <https://www.tandfonline.com/doi/full/10.1080/01615440.2021.1985027>.
 
+### Suggested Citation
+Wellington, J., R. Harper, and K.J. Thompson. 2022. "hlink." https://github.com/ipums/hlink: Institute for Social Research and Data Innovation, University of Minnesota.
+
 ## Installation
 
 hlink runs on Python 3.10.
 Java 8 or [Java 11](https://openjdk.org/install/) is required for the PySpark integration. 
 
 You can install the python package from pip:
 ```
```

### Comparing `hlink-3.3.0/doc/developer.md` & `hlink-3.3.1/doc/developer.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/column_mapping_transforms.doctree` & `hlink-3.3.1/docs/.doctrees/column_mapping_transforms.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/comparison_types.doctree` & `hlink-3.3.1/docs/.doctrees/comparison_types.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/config.doctree` & `hlink-3.3.1/docs/.doctrees/config.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/environment.pickle` & `hlink-3.3.1/docs/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/example_workflow.doctree` & `hlink-3.3.1/docs/.doctrees/example_workflow.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/feature_selection_transforms.doctree` & `hlink-3.3.1/docs/.doctrees/feature_selection_transforms.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/index.doctree` & `hlink-3.3.1/docs/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/installation.doctree` & `hlink-3.3.1/docs/.doctrees/installation.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/introduction.doctree` & `hlink-3.3.1/docs/.doctrees/introduction.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/link_tasks.doctree` & `hlink-3.3.1/docs/.doctrees/link_tasks.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/models.doctree` & `hlink-3.3.1/docs/.doctrees/models.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/pipeline_features.doctree` & `hlink-3.3.1/docs/.doctrees/pipeline_features.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/running_the_program.doctree` & `hlink-3.3.1/docs/.doctrees/running_the_program.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/substitutions.doctree` & `hlink-3.3.1/docs/.doctrees/substitutions.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/.doctrees/use_examples.doctree` & `hlink-3.3.1/docs/.doctrees/use_examples.doctree`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/comparison_types.md.txt` & `hlink-3.3.1/docs/_sources/comparison_types.md.txt`

 * *Files 1% similar despite different names*

```diff
@@ -642,18 +642,19 @@
 column_name = "race"
 comparison_type = "fetch_b"
 categorical = true
 ```
 
 ### present_both_years
 
-Checks whether both column A and column B are present.
+Checks whether column A and column B are both present and both positive (> 0).
+Evaluates to 1 if both are present and positive and 0 otherwise.
 
 * Attributes:
-  * `column_name` -- Type: `string`. The column to check.
+  * `column_name` -- Type: `string`. The column to check. Must be a column with a numerical type.
 
 ```
 [[comparison_features]]
 alias = "sp_caution"
 column_names = ["spouse_bpl", "spouse_birthyr", "durmarr", "sploc"]
 comparison_type = "caution_comp_4"
 categorical = true
@@ -671,28 +672,37 @@
 [comparison_features.comp_d]
 column_name = "sploc"
 comparison_type = "present_both_years"
 ```
 
 ### neither_are_null
 
-Checks that neither column A nor column B is null.
+Checks that neither column A nor column B is null or the empty string `''`.
+Evaluates to 1 if neither column is null or `''` and evaluates to 0 otherwise.
 
 * Attributes:
-  * `column_name` -- Type: `string`. The column to check.
+  * `column_name` -- Type: `string`. The column of type string to check.
+
+```
+[[comparison_features]]
+alias = "mpres"
+column_name = "m_namefrst"
+comparison_type = "neither_are_null"
+categorical = true
+```
 
 ### present_and_matching_categorical
 
 Checks that both column A and column B are present and that they match according to SQL's `IS DISTINCT FROM`. Evaluates to 0, 1, or 2:
 
-0 -> columns are both present and match
+0 → columns are both present and match
 
-1 -> columns are both present but are distinct
+1 → columns are both present but are distinct
 
-2 -> one or both columns are missing
+2 → one or both columns are missing
 
 * Attributes:
   * `column_name` -- Type: `string`. Required. The column to check.
 
 ### present_and_not_equal
 
 Checks that column A and column B are both present but are not equal.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hlink-3.3.0/docs/_sources/config.md.txt` & `hlink-3.3.1/docs/_sources/config.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/feature_selection_transforms.md.txt` & `hlink-3.3.1/docs/_sources/feature_selection_transforms.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/index.rst.txt` & `hlink-3.3.1/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/installation.md.txt` & `hlink-3.3.1/docs/_sources/installation.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/introduction.md.txt` & `hlink-3.3.1/docs/_sources/introduction.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/link_tasks.md.txt` & `hlink-3.3.1/docs/_sources/link_tasks.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/models.md.txt` & `hlink-3.3.1/docs/_sources/models.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/pipeline_features.md.txt` & `hlink-3.3.1/docs/_sources/pipeline_features.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/running_the_program.md.txt` & `hlink-3.3.1/docs/_sources/running_the_program.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/substitutions.md.txt` & `hlink-3.3.1/docs/_sources/substitutions.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_sources/use_examples.md.txt` & `hlink-3.3.1/docs/_sources/use_examples.md.txt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/_sphinx_javascript_frameworks_compat.js` & `hlink-3.3.1/docs/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/alabaster.css` & `hlink-3.3.1/docs/_static/alabaster.css`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,17 @@
 }
 
 table.footnote td {
     padding: 0.3em 0.5em;
 }
 
 dl {
-    margin: 0;
+    margin-left: 0;
+    margin-right: 0;
+    margin-top: 0;
     padding: 0;
 }
 
 dl dd {
     margin-left: 30px;
 }
```

### Comparing `hlink-3.3.0/docs/_static/basic.css` & `hlink-3.3.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/doctools.js` & `hlink-3.3.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/jquery-3.5.1.js` & `hlink-3.3.1/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/jquery-3.6.0.js` & `hlink-3.3.1/docs/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/jquery.js` & `hlink-3.3.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/language_data.js` & `hlink-3.3.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/pygments.css` & `hlink-3.3.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/searchtools.js` & `hlink-3.3.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/underscore-1.13.1.js` & `hlink-3.3.1/docs/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/_static/underscore.js` & `hlink-3.3.1/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/docs/comparison_types.html` & `hlink-3.3.1/docs/comparison_types.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Comparison types, transform add-ons, aggregate features, and household aggregate features &#8212; hlink 3.3.0 documentation</title>
+    <title>Comparison types, transform add-ons, aggregate features, and household aggregate features &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -816,19 +816,20 @@
 <span class="n">comparison_type</span> <span class="o">=</span> <span class="s2">&quot;fetch_b&quot;</span>
 <span class="n">categorical</span> <span class="o">=</span> <span class="n">true</span>
 </pre></div>
 </div>
 </section>
 <section id="present-both-years">
 <h3>present_both_years<a class="headerlink" href="#present-both-years" title="Permalink to this heading">¶</a></h3>
-<p>Checks whether both column A and column B are present.</p>
+<p>Checks whether column A and column B are both present and both positive (&gt; 0).
+Evaluates to 1 if both are present and positive and 0 otherwise.</p>
 <ul class="simple">
 <li><p>Attributes:</p>
 <ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">column_name</span></code> – Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. The column to check.</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">column_name</span></code> – Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. The column to check. Must be a column with a numerical type.</p></li>
 </ul>
 </li>
 </ul>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="p">[[</span><span class="n">comparison_features</span><span class="p">]]</span>
 <span class="n">alias</span> <span class="o">=</span> <span class="s2">&quot;sp_caution&quot;</span>
 <span class="n">column_names</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;spouse_bpl&quot;</span><span class="p">,</span> <span class="s2">&quot;spouse_birthyr&quot;</span><span class="p">,</span> <span class="s2">&quot;durmarr&quot;</span><span class="p">,</span> <span class="s2">&quot;sploc&quot;</span><span class="p">]</span>
 <span class="n">comparison_type</span> <span class="o">=</span> <span class="s2">&quot;caution_comp_4&quot;</span>
@@ -848,29 +849,37 @@
 <span class="n">column_name</span> <span class="o">=</span> <span class="s2">&quot;sploc&quot;</span>
 <span class="n">comparison_type</span> <span class="o">=</span> <span class="s2">&quot;present_both_years&quot;</span>
 </pre></div>
 </div>
 </section>
 <section id="neither-are-null">
 <h3>neither_are_null<a class="headerlink" href="#neither-are-null" title="Permalink to this heading">¶</a></h3>
-<p>Checks that neither column A nor column B is null.</p>
+<p>Checks that neither column A nor column B is null or the empty string <code class="docutils literal notranslate"><span class="pre">''</span></code>.
+Evaluates to 1 if neither column is null or <code class="docutils literal notranslate"><span class="pre">''</span></code> and evaluates to 0 otherwise.</p>
 <ul class="simple">
 <li><p>Attributes:</p>
 <ul>
-<li><p><code class="docutils literal notranslate"><span class="pre">column_name</span></code> – Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. The column to check.</p></li>
+<li><p><code class="docutils literal notranslate"><span class="pre">column_name</span></code> – Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. The column of type string to check.</p></li>
 </ul>
 </li>
 </ul>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="p">[[</span><span class="n">comparison_features</span><span class="p">]]</span>
+<span class="n">alias</span> <span class="o">=</span> <span class="s2">&quot;mpres&quot;</span>
+<span class="n">column_name</span> <span class="o">=</span> <span class="s2">&quot;m_namefrst&quot;</span>
+<span class="n">comparison_type</span> <span class="o">=</span> <span class="s2">&quot;neither_are_null&quot;</span>
+<span class="n">categorical</span> <span class="o">=</span> <span class="n">true</span>
+</pre></div>
+</div>
 </section>
 <section id="present-and-matching-categorical">
 <h3>present_and_matching_categorical<a class="headerlink" href="#present-and-matching-categorical" title="Permalink to this heading">¶</a></h3>
 <p>Checks that both column A and column B are present and that they match according to SQL’s <code class="docutils literal notranslate"><span class="pre">IS</span> <span class="pre">DISTINCT</span> <span class="pre">FROM</span></code>. Evaluates to 0, 1, or 2:</p>
-<p>0 -&gt; columns are both present and match</p>
-<p>1 -&gt; columns are both present but are distinct</p>
-<p>2 -&gt; one or both columns are missing</p>
+<p>0 → columns are both present and match</p>
+<p>1 → columns are both present but are distinct</p>
+<p>2 → one or both columns are missing</p>
 <ul class="simple">
 <li><p>Attributes:</p>
 <ul>
 <li><p><code class="docutils literal notranslate"><span class="pre">column_name</span></code> – Type: <code class="docutils literal notranslate"><span class="pre">string</span></code>. Required. The column to check.</p></li>
 </ul>
 </li>
 </ul>
@@ -1252,15 +1261,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/comparison_types.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -681,17 +681,19 @@
 [[comparison_features]]
 alias = "race"
 column_name = "race"
 comparison_type = "fetch_b"
 categorical = true
 
 **** present_both_yearsÂ¶ ****
-Checks whether both column A and column B are present.
+Checks whether column A and column B are both present and both positive (> 0).
+Evaluates to 1 if both are present and positive and 0 otherwise.
     * Attributes:
-          o column_name â Type: string. The column to check.
+          o column_name â Type: string. The column to check. Must be a column
+            with a numerical type.
 [[comparison_features]]
 alias = "sp_caution"
 column_names = ["spouse_bpl", "spouse_birthyr", "durmarr", "sploc"]
 comparison_type = "caution_comp_4"
 categorical = true
 [comparison_features.comp_a]
 column_name = "spouse_bpl"
@@ -705,24 +707,30 @@
 comparison_type = "new_marr"
 upper_threshold = 7
 [comparison_features.comp_d]
 column_name = "sploc"
 comparison_type = "present_both_years"
 
 **** neither_are_nullÂ¶ ****
-Checks that neither column A nor column B is null.
+Checks that neither column A nor column B is null or the empty string ''.
+Evaluates to 1 if neither column is null or '' and evaluates to 0 otherwise.
     * Attributes:
-          o column_name â Type: string. The column to check.
+          o column_name â Type: string. The column of type string to check.
+[[comparison_features]]
+alias = "mpres"
+column_name = "m_namefrst"
+comparison_type = "neither_are_null"
+categorical = true
 
 **** present_and_matching_categoricalÂ¶ ****
 Checks that both column A and column B are present and that they match
 according to SQLâs IS DISTINCT FROM. Evaluates to 0, 1, or 2:
-0 -> columns are both present and match
-1 -> columns are both present but are distinct
-2 -> one or both columns are missing
+0 â columns are both present and match
+1 â columns are both present but are distinct
+2 â one or both columns are missing
     * Attributes:
           o column_name â Type: string. Required. The column to check.
 
 **** present_and_not_equalÂ¶ ****
 Checks that column A and column B are both present but are not equal.
     * Attributes:
           o column_name â Type: string. The column to check.
@@ -993,8 +1001,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Column_mapping_transforms
           o Next: Feature_Selection_transforms
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/config.html` & `hlink-3.3.1/docs/config.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Configuration &#8212; hlink 3.3.0 documentation</title>
+    <title>Configuration &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -911,15 +911,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/config.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -898,8 +898,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Advanced_Workflow_Examples
           o Next: Column_mapping_transforms
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/feature_selection_transforms.html` & `hlink-3.3.1/docs/feature_selection_transforms.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Feature Selection transforms &#8212; hlink 3.3.0 documentation</title>
+    <title>Feature Selection transforms &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -229,15 +229,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/feature_selection_transforms.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -108,8 +108,8 @@
 **** Related Topics ****
     * Documentation_overview
           o Previous: Comparison_types,_transform_add-ons,_aggregate_features,
             and_household_aggregate_features
           o Next: Pipeline_generated_features
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/genindex.html` & `hlink-3.3.1/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; hlink 3.3.0 documentation</title>
+    <title>Index &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -103,15 +103,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
     </div>
 
     
 
     
   </body>
```

#### html2text {}

```diff
@@ -21,8 +21,8 @@
     * Pipeline_Features
     * Substitutions
     * Models
 **** Related Topics ****
     * Documentation_overview
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13
```

### Comparing `hlink-3.3.0/docs/index.html` & `hlink-3.3.1/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to hlink’s documentation! &#8212; hlink 3.3.0 documentation</title>
+    <title>Welcome to hlink’s documentation! &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -220,15 +220,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/index.rst.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -109,8 +109,8 @@
     * Substitutions
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Next: Introduction
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/installation.html` & `hlink-3.3.1/docs/installation.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Installation &#8212; hlink 3.3.0 documentation</title>
+    <title>Installation &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -133,15 +133,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/installation.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -50,8 +50,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Introduction
           o Next: Link_Tasks
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/introduction.html` & `hlink-3.3.1/docs/introduction.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Introduction &#8212; hlink 3.3.0 documentation</title>
+    <title>Introduction &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -145,15 +145,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/introduction.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -61,8 +61,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Welcome_to_hlinkâs_documentation!
           o Next: Installation
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/link_tasks.html` & `hlink-3.3.1/docs/link_tasks.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Link Tasks &#8212; hlink 3.3.0 documentation</title>
+    <title>Link Tasks &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -204,15 +204,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/link_tasks.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -103,8 +103,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Installation
           o Next: Running_hlink
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/models.html` & `hlink-3.3.1/docs/models.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Models &#8212; hlink 3.3.0 documentation</title>
+    <title>Models &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -182,15 +182,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/models.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -93,8 +93,8 @@
           o decision_tree
           o gradient_boosted_trees
 **** Related Topics ****
     * Documentation_overview
           o Previous: Substitutions
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/objects.inv` & `hlink-3.3.1/docs/objects.inv`

 * *Files 26% similar despite different names*

#### Sphinx inventory

```diff
@@ -1,10 +1,10 @@
 # Sphinx inventory version 2
 # Project: hlink
-# Version: 3.3.0
+# Version: 3.3.1
 # The remainder of this file is compressed using zlib.
 
 column_mapping_transforms std:doc -1 column_mapping_transforms.html Column mapping transforms
 comparison_types std:doc -1 comparison_types.html Comparison types, transform add-ons, aggregate features, and household aggregate features
 config std:doc -1 config.html Configuration
 feature_selection_transforms std:doc -1 feature_selection_transforms.html Feature Selection transforms
 genindex std:label -1 genindex.html Index
```

### Comparing `hlink-3.3.0/docs/pipeline_features.html` & `hlink-3.3.1/docs/pipeline_features.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Pipeline generated features &#8212; hlink 3.3.0 documentation</title>
+    <title>Pipeline generated features &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -155,15 +155,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/pipeline_features.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -70,8 +70,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Feature_Selection_transforms
           o Next: Substitutions
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/running_the_program.html` & `hlink-3.3.1/docs/running_the_program.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Running hlink &#8212; hlink 3.3.0 documentation</title>
+    <title>Running hlink &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -130,15 +130,15 @@
                         Execute a single command then exit the program.
   --conf CONF, --run CONF
                         Specify a filepath where your config file for the run
                         is located.
 </pre></div>
 </div>
 <p>To run the program in interactive mode using a configuration file at a specified path, say <code class="docutils literal notranslate"><span class="pre">./fullcount_1870_1880.toml</span></code>, run a command following this pattern:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink --conf<span class="o">=</span>./full_count_1870_1880.toml
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>--conf<span class="o">=</span>./full_count_1870_1880.toml
 </pre></div>
 </div>
 <p>After the program has started, you will see a prompt that looks like this:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span>hlink $
 </pre></div>
 </div>
 <p>Type <code class="docutils literal notranslate"><span class="pre">help</span></code> or <code class="docutils literal notranslate"><span class="pre">?</span></code> and hit enter to see a list of commands; type <code class="docutils literal notranslate"><span class="pre">help</span> <span class="pre">&lt;command&gt;</span></code> to see the help text of a specific command.
@@ -243,15 +243,15 @@
 <li><p>Create a config file and put it in your hlink config directory.
 For example:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">/</span><span class="n">path</span><span class="o">/</span><span class="n">to</span><span class="o">/</span><span class="n">conf</span><span class="o">/</span><span class="n">full_count_1870_1880</span><span class="o">.</span><span class="n">toml</span>
 </pre></div>
 </div>
 </li>
 <li><p>Launch the hlink program in interactive mode:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink --conf<span class="o">=</span>/path/to/conf/full_count_1870_1880
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>--conf<span class="o">=</span>/path/to/conf/full_count_1870_1880
 </pre></div>
 </div>
 </li>
 <li><p>Run the tasks you want to complete:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span> hlink $ run_all_steps preprocessing training matching
 </pre></div>
 </div>
@@ -342,15 +342,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/running_the_program.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -264,8 +264,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Link_Tasks
           o Next: Advanced_Workflow_Examples
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/search.html` & `hlink-3.3.1/docs/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; hlink 3.3.0 documentation</title>
+    <title>Search &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -122,15 +122,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
     </div>
 
     
 
     
   </body>
```

#### html2text {}

```diff
@@ -22,8 +22,8 @@
     * Comparison_Types
     * Feature_Selection
     * Pipeline_Features
     * Substitutions
     * Models
 **** Related Topics ****
     * Documentation_overview
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13
```

### Comparing `hlink-3.3.0/docs/searchindex.js` & `hlink-3.3.1/docs/searchindex.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -8,67 +8,79 @@
         "below": [0, 1, 2, 3, 8, 9, 10],
         "repres": [0, 1, 2, 3, 9, 10],
         "type": [0, 2, 3, 4, 8, 10, 11, 12],
         "ar": [0, 1, 2, 3, 5, 6, 7, 8, 9, 10, 12],
         "us": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 11, 12],
         "context": [0, 1, 3, 9],
         "column_map": [0, 2],
+        "list": [0, 1, 2, 3, 4, 8, 10, 11],
+        "oper": [0, 2],
+        "singl": [0, 2, 10, 12],
+        "input": [0, 1, 2, 3, 6, 10, 11],
+        "output": [0, 1, 2, 3, 6, 7, 10, 12],
         "some": [0, 1, 3, 6, 10],
-        "refer": [0, 2],
+        "suffix": [0, 4],
         "b": [0, 1, 2, 4, 10],
         "These": [0, 1, 2, 3, 6, 8, 9],
         "mean": 0,
         "appli": [0, 2, 3, 12],
         "from": [0, 1, 2, 4, 6, 7, 8, 9, 10, 12],
         "onli": [0, 1, 2, 12],
         "one": [0, 1, 2, 4],
         "two": [0, 1, 2, 3, 6, 7, 9, 10, 12],
         "dataset": [0, 1, 2, 6, 7, 10, 12],
         "link": [0, 1, 2, 4, 6, 8],
-        "we": [0, 1, 10, 12],
-        "re": 0,
-        "try": [0, 2],
-        "peopl": [0, 1, 6, 10],
+        "A": [0, 1, 2, 9, 10],
+        "most": [0, 1, 10],
+        "both": [0, 1, 2, 12],
+        "independ": [0, 2],
         "more": [0, 1, 2, 7, 9, 10, 12],
         "than": [0, 1, 2, 8],
         "can": [0, 1, 2, 5, 6, 8, 10, 12],
         "order": [0, 2],
         "thei": [0, 1, 2, 10],
-        "list": [0, 1, 2, 3, 4, 8, 10, 11],
+        "re": 0,
+        "configur": [0, 1, 6, 7, 10, 12],
+        "file": [0, 1, 4, 6, 7, 10, 11, 12],
         "so": [0, 1, 2, 5, 12],
-        "output": [0, 1, 2, 3, 6, 7, 10, 12],
         "mai": [0, 2, 6, 10],
-        "input": [0, 1, 2, 3, 6, 10, 11],
         "anoth": [0, 1, 3],
+        "format": 0,
+        "The": [0, 1, 2, 3, 5, 7, 8, 9, 10, 12],
+        "letter": [0, 4],
+        "t": [0, 1, 2, 3, 12],
+        "u": 0,
+        "arbitrari": 0,
         "specifi": [0, 1, 2, 6, 7, 9, 10, 11],
         "column_nam": [0, 1, 2, 11],
         "attribut": [0, 1, 2, 3, 8, 9, 10, 11],
-        "config": [0, 1, 4, 7, 10, 12],
         "under": [0, 1, 2],
+        "its": [0, 1, 6, 10],
         "section": [0, 1, 2, 7, 12],
-        "The": [0, 1, 2, 3, 5, 7, 8, 9, 10, 12],
-        "indic": [0, 1, 12],
-        "which": [0, 1, 2, 3, 6, 9, 10, 12],
+        "name": [0, 1, 2, 4, 10, 11],
         "i": [0, 1, 2, 3, 5, 6, 7, 8, 10, 11, 12],
-        "ones": 0,
+        "alia": [0, 2],
         "along": [0, 1],
+        "which": [0, 1, 2, 3, 6, 9, 10, 12],
+        "must": [0, 1, 2, 8, 9, 11],
         "addit": [0, 1, 2, 3, 5, 6, 10],
         "vari": [0, 2],
         "inform": [0, 1, 2, 10],
         "given": [0, 1, 2, 3, 8, 12],
         "often": [0, 10],
-        "an": [0, 1, 2, 3, 6, 8, 10],
         "just": [0, 1, 2, 10, 12],
-        "name": [0, 1, 2, 4, 10, 11],
         "valu": [0, 1, 2, 4, 8, 9, 10, 11],
-        "alia": [0, 2],
+        "expect": [0, 1],
+        "an": [0, 1, 2, 3, 6, 8, 10],
+        "exampl": [0, 1, 2],
         "namefrst_split": [0, 2],
         "namefrst_clean": [0, 2],
         "add": [0, 4],
         "_": [0, 1, 2, 3, 4, 8, 9, 10],
+        "numer": [0, 1],
         "11": [0, 2, 5, 9],
         "concat": [0, 4],
         "concaten": [0, 1],
         "string": [0, 1, 2, 3, 8, 10, 11],
         "end": [0, 1, 2, 3, 11],
         "lowercas": [0, 4],
         "strip": [0, 4],
@@ -81,173 +93,65 @@
         "white": 0,
         "space": [0, 2, 3, 11],
         "start": [0, 11],
         "ration": [0, 4],
         "word": [0, 4],
         "replac": [0, 4],
         "sinc": [0, 2],
+        "peopl": [0, 1, 6, 10],
         "": [0, 1, 2, 6, 10, 11],
         "raw": [0, 2, 7, 10],
         "censu": [0, 12],
         "data": [0, 1, 4, 6, 7, 10],
         "contain": [0, 1, 11],
         "lead": 0,
         "better": [0, 6],
         "match": [0, 1, 4, 6, 10, 11, 12],
         "remov": [0, 4],
         "qmark": [0, 4],
         "hyphen": [0, 4],
-        "noth": 0,
         "punctuat": [0, 4],
-        "most": [0, 1, 10],
+        "thi": [0, 1, 2, 5, 6, 7, 9, 10, 12],
         "apostroph": [0, 4],
         "altern": [0, 2, 4],
-        "ani": [0, 1, 2, 5, 7, 8],
+        "If": [0, 1, 2, 3, 8, 10, 11],
+        "surround": 0,
+        "all": [0, 1, 2, 3, 8, 9, 10],
         "follow": [0, 1, 6, 10, 11, 12],
-        "suffix": [0, 4],
         "them": [0, 1],
         "jr": [0, 2],
         "sr": [0, 2],
         "ii": [0, 2],
         "iii": [0, 2],
         "stop": [0, 4],
         "last": [0, 1, 9],
         "street": [0, 1],
-        "allei": 0,
-        "alli": 0,
-        "ali": 0,
-        "anex": 0,
-        "annex": 0,
-        "av": [0, 11],
-        "aven": 0,
         "avenu": [0, 11],
-        "avn": 0,
-        "avnu": 0,
-        "avanu": 0,
-        "avaneu": 0,
-        "bg": 0,
         "blvd": 0,
-        "boul": 0,
-        "boulevard": 0,
-        "brg": 0,
-        "bridg": 0,
-        "burg": 0,
-        "camp": 0,
         "circl": 0,
-        "cor": 0,
-        "corner": 0,
         "court": 0,
-        "cp": 0,
-        "cre": 0,
-        "crescent": 0,
-        "ct": 0,
-        "dr": 0,
-        "driv": 0,
-        "drive": 0,
-        "est": 0,
-        "estat": 0,
-        "express": [0, 1, 2],
-        "expresswai": 0,
-        "ext": 0,
-        "extens": 0,
-        "ferri": 0,
-        "fort": 0,
-        "frt": 0,
-        "fry": 0,
-        "ft": 0,
-        "height": 0,
-        "ht": 0,
-        "island": 0,
-        "kei": [0, 1, 7, 10],
-        "ky": 0,
-        "ldg": 0,
-        "lodg": 0,
-        "mill": 0,
-        "ml": [0, 2, 4, 8, 9],
-        "mount": 0,
-        "mountain": 0,
-        "mountin": 0,
-        "mt": 0,
-        "mtn": 0,
-        "park": 0,
-        "parkwai": 0,
-        "pike": 0,
-        "pkwy": 0,
-        "pl": 0,
-        "place": 0,
-        "point": [0, 9, 12],
-        "pr": 0,
-        "prairi": 0,
-        "prk": 0,
-        "pt": 0,
-        "rad": 0,
-        "radial": 0,
-        "rd": 0,
-        "rest": 0,
-        "riv": 0,
-        "river": 0,
         "road": 0,
-        "rst": 0,
-        "spg": 0,
-        "spring": 0,
-        "sq": 0,
-        "squar": [0, 1],
-        "st": 0,
-        "sta": 0,
-        "station": 0,
-        "str": 0,
-        "strt": 0,
-        "ter": 0,
-        "terrac": 0,
-        "track": 0,
-        "trail": 0,
-        "trnpk": 0,
-        "turnpik": 0,
-        "un": 0,
-        "union": [0, 4],
-        "vallei": 0,
-        "valli": 0,
-        "via": [0, 5, 6],
-        "viaduct": 0,
-        "vill": 0,
-        "villag": 0,
-        "villiag": 0,
-        "well": [0, 2],
-        "wl": 0,
-        "south": 0,
-        "north": 0,
-        "east": 0,
-        "west": 0,
-        "n": [0, 8, 9],
-        "e": [0, 5],
-        "w": 0,
-        "block": [0, 4, 7],
         "prefix": [0, 4],
         "like": [0, 2, 10],
         "m": [0, 1],
         "mr": 0,
         "In": [0, 1, 6, 10, 12],
         "ah": 0,
         "chines": 0,
         "condens": [0, 4],
         "whitespac": [0, 4],
         "take": [0, 1, 2, 3, 10],
         "non": 0,
-        "singl": [0, 2, 10, 12],
-        "letter": [0, 4],
-        "If": [0, 1, 2, 3, 8, 10, 11],
         "leav": 0,
         "behind": 0,
         "arrai": [0, 2, 4, 8, 9],
         "index": [0, 4, 5],
         "select": [0, 1, 4, 6, 10, 12],
         "element": 0,
-        "posit": [0, 2, 4, 6],
-        "thi": [0, 1, 2, 5, 6, 7, 9, 10, 12],
-        "exampl": [0, 1, 2],
+        "posit": [0, 1, 2, 4, 6],
         "first": [0, 1, 2, 5, 10, 11],
         "second": [0, 1, 2, 11],
         "1": [0, 1, 2, 4, 7, 8, 9, 10, 12],
         "item": 0,
         "namefrst": [0, 1, 2],
         "set": [0, 1, 2, 3, 6, 7, 10, 12],
         "Then": [0, 5],
@@ -279,14 +183,15 @@
         "detail": [0, 2, 7, 10],
         "version": [0, 5, 12],
         "gener": [0, 1, 4, 6, 7, 10],
         "least": 0,
         "signific": 0,
         "digit": 0,
         "make": [0, 1, 2, 5, 12],
+        "we": [0, 1, 10, 12],
         "simpli": [0, 2],
         "drop": [0, 2, 10],
         "100": [0, 2, 12],
         "round": [0, 2, 7],
         "lowest": 0,
         "whole": [0, 6],
         "number": [0, 1, 2, 7, 8, 10],
@@ -295,23 +200,22 @@
         "bpl": [0, 1, 2],
         "bpl_root": 0,
         "when": [0, 1, 2, 3, 4, 12],
         "condit": [0, 1, 2, 3, 4],
         "logic": 0,
         "work": [0, 1, 2, 5, 10, 12],
         "sql": [0, 1, 2, 3, 4, 10],
+        "express": [0, 1, 2],
         "claus": [0, 1],
-        "els": [0, 1, 2, 3],
-        "all": [0, 1, 2, 3, 8, 9, 10],
+        "if_valu": 0,
+        "else_valu": 0,
         "race": [0, 1, 2, 9, 12],
         "ipum": [0, 6],
         "code": [0, 1, 2, 5],
         "categori": [0, 8],
-        "if_valu": 0,
-        "else_valu": 0,
         "get": [0, 1, 4, 10],
         "down": [0, 6, 12],
         "nearest": 0,
         "produc": [0, 10],
         "relat": [0, 1, 2],
         "between": [0, 1, 2, 6, 7, 10, 12],
         "hundr": 0,
@@ -339,15 +243,14 @@
         "12": 0,
         "relate_div_100": [0, 1, 2],
         "page": [1, 10],
         "ha": [1, 2, 6, 10, 12],
         "differ": [1, 2, 4, 6],
         "avail": [1, 2, 3, 5, 8, 9, 12],
         "comparison_featur": [1, 2],
-        "configur": [1, 6, 7, 10, 12],
         "relatematch": [1, 2],
         "comparison_typ": [1, 2],
         "categor": [1, 2, 8, 9],
         "true": [1, 2, 3, 9, 11, 12],
         "maximum": [1, 8],
         "jaro": [1, 9],
         "winkler": [1, 9],
@@ -373,40 +276,40 @@
         "geograph": 1,
         "filter": [1, 4, 7, 11],
         "major": [1, 10],
         "locat": [1, 2, 10],
         "chang": [1, 2, 5, 10, 12],
         "befor": [1, 2, 3, 5],
         "boundari": 1,
-        "A": [1, 2, 9, 10],
         "zero": 1,
         "jw_street": 1,
         "enum_dist": 1,
         "max": [1, 8, 10],
         "member": [1, 7],
         "neighborhood": 1,
         "surnam": 1,
         "related_individual_max_jw": 1,
         "namefrst_rel": 1,
         "assert": [1, 10],
         "same": [1, 2, 6, 7, 10],
-        "both": [1, 2, 12],
         "NOT": 1,
         "distinct": 1,
         "f1": 1,
         "evalu": [1, 2, 6, 8],
         "either": [1, 2, 6, 11],
+        "ani": [1, 2, 5, 7, 8],
         "potenti": [1, 4, 7],
         "mismatch": 1,
         "queri": [1, 2],
         "fi": 1,
         "OR": 1,
         "mi0": 1,
         "mi1": 1,
         "THEN": 1,
+        "els": [1, 2, 3],
         "first_init_col": 1,
         "namefrst_init": 1,
         "mid_init_col": 1,
         "namefrst_mid_init_2": 1,
         "f2": 1,
         "empti": 1,
         "null": [1, 2, 3],
@@ -441,14 +344,15 @@
         "record": [1, 2, 6],
         "being": [1, 7],
         "exact": [1, 2],
         "namefrst_unstd": [1, 2],
         "present": [1, 2, 9],
         "nonzero": 1,
         "primarili": 1,
+        "indic": [1, 12],
         "kind": 1,
         "incompar": 1,
         "akin": 1,
         "miss": [1, 10],
         "see": [1, 2, 5, 7, 10, 12],
         "also": [1, 2, 5, 6, 9, 10, 12],
         "univers": [1, 4],
@@ -513,15 +417,14 @@
         "birthyr_col": 1,
         "namefrst_related_row": 1,
         "replaced_birthyr": [1, 2, 3],
         "extra": 1,
         "children": 1,
         "who": 1,
         "base": [1, 2, 7],
-        "expect": 1,
         "count": [1, 10, 12],
         "suspect": [1, 6],
         "relate_col": 1,
         "histid_col": 1,
         "id": [1, 2],
         "birth": 1,
         "year": [1, 2, 3, 4],
@@ -575,15 +478,15 @@
         "hlink": [1, 2, 5, 6, 12],
         "core": [1, 10, 12],
         "dist_tabl": 1,
         "py": [1, 2],
         "There": [1, 3, 7],
         "sever": [1, 6],
         "wai": [1, 5, 10],
-        "file": [1, 4, 6, 7, 10, 11, 12],
+        "kei": [1, 7, 10],
         "key_count": 1,
         "secondari": 1,
         "serv": 1,
         "back": 1,
         "primari": [1, 6],
         "doe": [1, 12],
         "particularli": 1,
@@ -591,15 +494,14 @@
         "much": 1,
         "fewer": [1, 8],
         "combin": [1, 2, 3],
         "thu": 1,
         "risk": 1,
         "fill": 1,
         "aren": 1,
-        "t": [1, 2, 3, 12],
         "ex": 1,
         "even": 1,
         "though": 1,
         "distances_fil": 1,
         "path": [1, 2, 10, 11, 12],
         "table_nam": 1,
         "what": [1, 2, 10, 12],
@@ -642,14 +544,16 @@
         "from_statefip": 1,
         "to_statefip": 1,
         "distance_km": 1,
         "state_1900_1910_distances_km": 1,
         "fetch": 1,
         "neither": 1,
         "nor": 1,
+        "mpre": 1,
+        "m_namefrst": 1,
         "accord": 1,
         "niu": 1,
         "other": [1, 2, 12],
         "mfbplmatch": 1,
         "flexibl": 1,
         "user": [1, 10],
         "write": [1, 10, 12],
@@ -661,15 +565,14 @@
         "fallback": 1,
         "defin": [1, 8, 9, 10],
         "jw": 1,
         "comput": [1, 3],
         "nvl": 1,
         "spark": [1, 2, 5, 8, 9, 10, 12],
         "builtin": 1,
-        "its": [1, 6, 10],
         "argument": [1, 10, 12],
         "namelast_jw_max": 1,
         "namelast1": 1,
         "namelast2": 1,
         "namelast3": 1,
         "abov": [1, 5],
         "extend": 1,
@@ -678,19 +581,19 @@
         "top": [1, 4],
         "level": [1, 4, 10],
         "everi": 1,
         "jw_f": [1, 2, 12],
         "father_namefrst": 1,
         "rais": [1, 3],
         "exponenti": 1,
+        "squar": 1,
         "county_distance_squar": [1, 2, 12],
         "per": [1, 2, 8, 9, 10],
         "county_a": 1,
         "county_b": 1,
-        "numer": 1,
         "upper": 1,
         "gt": 1,
         "btwn": 1,
         "addl": 1,
         "var": [1, 2],
         "program": [1, 2, 7, 12],
         "report": [1, 4, 6, 10],
@@ -701,14 +604,15 @@
         "datasourc": [1, 2, 10],
         "yrimmig": 1,
         "immyear_diff": [1, 2, 9, 12],
         "To": [1, 5, 10],
         "includ": [1, 2, 9, 10],
         "train": [1, 4, 6, 8, 10],
         "independent_var": [1, 2, 12],
+        "config": [1, 4, 7, 10, 12],
         "templat": 1,
         "id_column": [1, 2],
         "_a": 1,
         "mult": 1,
         "exist": [1, 2, 10],
         "within": [1, 2, 6, 10, 11],
         "hh_train": [1, 2, 7, 10, 12],
@@ -716,14 +620,15 @@
         "highest": [1, 2],
         "against": [1, 11],
         "ten": [1, 2],
         "current": [1, 2, 10],
         "tell": 2,
         "how": 2,
         "descript": [2, 8, 10],
+        "refer": 2,
         "here": [2, 10, 12],
         "tutori": [2, 10],
         "script": [2, 6, 10],
         "discuss": 2,
         "readm": 2,
         "note": 2,
         "written": [2, 6],
@@ -738,15 +643,14 @@
         "10": [2, 5, 12],
         "age_2": 2,
         "derived_from": 2,
         "expand_length": 2,
         "explod": [2, 7],
         "jaro_winkl": 2,
         "namelast_jw": [2, 12],
-        "oper": 2,
         "threshold": [2, 8, 12],
         "feature_nam": 2,
         "79": 2,
         "84": 2,
         "complex": 2,
         "machin": [2, 6, 7, 10, 12],
         "learn": [2, 6, 7, 10, 12],
@@ -847,15 +751,14 @@
         "probit": [2, 4],
         "go": [2, 10],
         "your": [2, 5, 10, 12],
         "uniqu": 2,
         "identifi": [2, 6, 12],
         "full": [2, 12],
         "short": 2,
-        "must": [2, 8, 9, 11],
         "alphanumer": 2,
         "my_fil": 2,
         "subset": [2, 11],
         "limit": 2,
         "extract": 2,
         "new": [2, 12],
         "default": [2, 8, 10],
@@ -896,26 +799,27 @@
         "treat": [2, 9],
         "import": [2, 10, 12],
         "dure": 2,
         "hot": 2,
         "encod": [2, 3],
         "vector": [2, 9],
         "stage": 2,
+        "well": 2,
         "upper_threshold": 2,
         "cannot": 2,
         "robust": 2,
+        "ml": [2, 4, 8, 9],
         "typic": 2,
         "leverag": 2,
         "api": [2, 6, 9],
         "piplin": 2,
         "regionf": 2,
         "sex_regionf_interact": 2,
         "immyear_caut": [2, 9],
         "myriad": 2,
-        "independ": 2,
         "explor": [2, 4, 6, 10],
         "part": 2,
         "task": [2, 4, 6, 8, 12],
         "final": [2, 12],
         "drop_duplicate_a": 2,
         "time": [2, 10],
         "out": [2, 12],
@@ -929,14 +833,15 @@
         "hyper": [2, 6, 12],
         "paramet": [2, 6, 8, 10, 12],
         "eval": 2,
         "skip": [2, 7],
         "apply_model": 2,
         "run_all_step": [2, 10, 12],
         "command": [2, 6, 10, 12],
+        "try": 2,
         "creation": 2,
         "iter": 2,
         "scale": 2,
         "error": [2, 9],
         "1900": [2, 12],
         "about": [2, 10, 12],
         "1930": [2, 12],
@@ -1030,19 +935,21 @@
         "workflow": 4,
         "export": [4, 7, 10],
         "featur": [4, 6, 7, 8, 10],
         "reus": 4,
         "basic": 4,
         "map": [4, 7, 9],
         "substitut": [4, 7],
+        "block": [4, 7],
         "comparison": [4, 7],
         "pipelin": 4,
         "substr": 4,
         "ons": 4,
         "aggreg": 4,
+        "union": 4,
         "soundex": 4,
         "power": 4,
         "regex": 4,
         "random": [4, 8],
         "forest": [4, 8],
         "logist": [4, 8],
         "regress": [4, 8],
@@ -1050,14 +957,15 @@
         "gradient": [4, 8],
         "boost": [4, 8],
         "system": 5,
         "python": [5, 6, 10],
         "java": 5,
         "integr": 5,
         "apach": 5,
+        "via": [5, 6],
         "pyspark": [5, 8, 9, 10],
         "packag": 5,
         "org": 5,
         "latest": 5,
         "pip": 5,
         "easiest": [5, 10],
         "through": [5, 9, 10],
@@ -1066,14 +974,15 @@
         "clone": 5,
         "github": 5,
         "repositori": 5,
         "root": 5,
         "project": 5,
         "directori": [5, 10, 12],
         "develop": [5, 6],
+        "e": 5,
         "dev": 5,
         "edit": 5,
         "made": 5,
         "automat": [5, 7],
         "built": 5,
         "tool": [5, 6],
         "line": [6, 10],
@@ -1142,14 +1051,15 @@
         "featuresubsetstrategi": 8,
         "node": 8,
         "support": 8,
         "auto": 8,
         "onethird": 8,
         "sqrt": 8,
         "log2": 8,
+        "n": [8, 9],
         "15": 8,
         "generalizedlinearregress": 8,
         "famili": 8,
         "binomi": 8,
         "85": [8, 10],
         "logisticregress": 8,
         "decisiontreeclassifi": 8,
@@ -1160,14 +1070,15 @@
         "discard": 8,
         "maxbin": 8,
         "bin": 8,
         "discret": 8,
         "continu": [8, 9, 12],
         "gbtclassifi": 8,
         "mother": 9,
+        "point": [9, 12],
         "With": 9,
         "x": [9, 10],
         "y": 9,
         "hold": 9,
         "except": 9,
         "strictli": 9,
         "inf": 9,
@@ -1328,14 +1239,15 @@
         "launch": [10, 12],
         "my": [10, 12],
         "subhead": 11,
         "suppli": 11,
         "regex_word_replac": 11,
         "variant": 11,
         "abbrevi": 11,
+        "av": 11,
         "7th": 11,
         "swap": 11,
         "still": 11,
         "anywher": 11,
         "long": 11,
         "proceed": 11,
         "street_unstd": 11,
```

### Comparing `hlink-3.3.0/docs/substitutions.html` & `hlink-3.3.1/docs/substitutions.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Substitutions &#8212; hlink 3.3.0 documentation</title>
+    <title>Substitutions &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -170,15 +170,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/substitutions.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -75,8 +75,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Pipeline_generated_features
           o Next: Models
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/docs/use_examples.html` & `hlink-3.3.1/docs/use_examples.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Advanced Workflow Examples &#8212; hlink 3.3.0 documentation</title>
+    <title>Advanced Workflow Examples &#8212; hlink 3.3.1 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
@@ -47,34 +47,34 @@
 <li><p>Create a config file and put it in your hlink config directory.</p></li>
 <li><p>Launch the hlink program in interactive mode:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">hlink</span> <span class="o">--</span><span class="n">conf</span><span class="o">=</span><span class="n">full_count_1900_1910</span> <span class="o">--</span><span class="n">cores</span> <span class="mi">50</span> <span class="o">--</span><span class="n">executor_memory</span> <span class="mi">50</span><span class="n">G</span>
 </pre></div>
 </div>
 </li>
 <li><p>Run the preprocessing and training link tasks:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink $ run_all_steps preprocessing training
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>$<span class="w"> </span>run_all_steps<span class="w"> </span>preprocessing<span class="w"> </span>training
 </pre></div>
 </div>
 </li>
 <li><p>Ask the program what the arguments for the <code class="docutils literal notranslate"><span class="pre">csv</span></code> command are:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink $ ? csv
-Writes a dataframe out to csv.
-     Arg <span class="m">1</span>: dataframe
-     Arg <span class="m">2</span>: path
-     Arg <span class="m">3</span> <span class="o">(</span>optional<span class="o">)</span>: <span class="c1"># of partitions</span>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>$<span class="w"> </span>?<span class="w"> </span>csv
+Writes<span class="w"> </span>a<span class="w"> </span>dataframe<span class="w"> </span>out<span class="w"> </span>to<span class="w"> </span>csv.
+<span class="w">     </span>Arg<span class="w"> </span><span class="m">1</span>:<span class="w"> </span>dataframe
+<span class="w">     </span>Arg<span class="w"> </span><span class="m">2</span>:<span class="w"> </span>path
+<span class="w">     </span>Arg<span class="w"> </span><span class="m">3</span><span class="w"> </span><span class="o">(</span>optional<span class="o">)</span>:<span class="w"> </span><span class="c1"># of partitions</span>
 </pre></div>
 </div>
 </li>
 <li><p>Export the results using the <code class="docutils literal notranslate"><span class="pre">csv</span></code> command:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink $ csv training_features /my/output/training_data_1900_1910_HLINK_FEATURES.csv
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>$<span class="w"> </span>csv<span class="w"> </span>training_features<span class="w"> </span>/my/output/training_data_1900_1910_HLINK_FEATURES.csv
 </pre></div>
 </div>
 </li>
 <li><p>Continue with other linking work you might need to do with this year pair, otherwise shut down the hlink framework for this pair of linking years:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink $ q
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>$<span class="w"> </span>q
 </pre></div>
 </div>
 </li>
 <li><p>In the config file for the new year pairs (1910-1920, 1920-1930, etc.), point to this new file as your dataset, and set the <code class="docutils literal notranslate"><span class="pre">use_training_data_features</span></code></p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="c1"># config file for 1910-1920 linking run using the 1900-1910 training data with hlink-generated features</span>
 <span class="p">[</span><span class="n">training</span><span class="p">]</span>
 
@@ -133,15 +133,15 @@
 <span class="c1"># exploration and making decisions about your models and hyperparameters. This </span>
 <span class="c1"># section isn&#39;t used by the model exploration task.</span>
 <span class="n">chosen_model</span> <span class="o">=</span> <span class="p">{</span> <span class="nb">type</span> <span class="o">=</span> <span class="s2">&quot;logistic_regression&quot;</span><span class="p">,</span> <span class="n">threshold</span> <span class="o">=</span> <span class="mf">0.5</span><span class="p">,</span> <span class="n">threshold_ratio</span> <span class="o">=</span> <span class="mf">1.0</span> <span class="p">}</span>
 </pre></div>
 </div>
 </li>
 <li><p>Launch the hlink program in interactive mode:</p>
-<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink --conf<span class="o">=</span>full_count_1900_1910 --cores <span class="m">50</span> --executor_memory 50G
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>hlink<span class="w"> </span>--conf<span class="o">=</span>full_count_1900_1910<span class="w"> </span>--cores<span class="w"> </span><span class="m">50</span><span class="w"> </span>--executor_memory<span class="w"> </span>50G
 </pre></div>
 </div>
 </li>
 <li><p>Run the preprocessing and model exploration link tasks:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span>hlink $ run_all_steps preprocessing model_exploration
 </pre></div>
 </div>
@@ -234,15 +234,15 @@
       <div class="clearer"></div>
     </div>
     <div class="footer">
       &copy;2019-2022, IPUMS.
       
       |
       Powered by <a href="http://sphinx-doc.org/">Sphinx 5.1.1</a>
-      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.12</a>
+      &amp; <a href="https://github.com/bitprophet/alabaster">Alabaster 0.7.13</a>
       
       |
       <a href="_sources/use_examples.md.txt"
           rel="nofollow">Page source</a>
     </div>
```

#### html2text {}

```diff
@@ -168,8 +168,8 @@
     * Models
 **** Related Topics ****
     * Documentation_overview
           o Previous: Running_hlink
           o Next: Configuration
 **** Quick search ****
 [q                   ] [Go]
-©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.12 | Page_source
+©2019-2022, IPUMS. | Powered by Sphinx_5.1.1 & Alabaster_0.7.13 | Page_source
```

### Comparing `hlink-3.3.0/examples/tutorial/README.md` & `hlink-3.3.1/examples/tutorial/README.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/examples/tutorial/tutorial.py` & `hlink-3.3.1/examples/tutorial/tutorial.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/examples/tutorial/tutorial_config.toml` & `hlink-3.3.1/examples/tutorial/tutorial_config.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/configs/load_config.py` & `hlink-3.3.1/hlink/configs/load_config.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/README.md` & `hlink-3.3.1/hlink/linking/README.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/classifier.py` & `hlink-3.3.1/hlink/linking/core/classifier.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/column_mapping.py` & `hlink-3.3.1/hlink/linking/core/column_mapping.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/comparison.py` & `hlink-3.3.1/hlink/linking/core/comparison.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/comparison_feature.py` & `hlink-3.3.1/hlink/linking/core/comparison_feature.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/dist_table.py` & `hlink-3.3.1/hlink/linking/core/dist_table.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/pipeline.py` & `hlink-3.3.1/hlink/linking/core/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     StandardScaler,
     OneHotEncoder,
     VectorAssembler,
     Bucketizer,
 )
 import hlink.linking.transformers.interaction_transformer
 import hlink.linking.transformers.float_cast_transformer
+import logging
 
 
 def generate_pipeline_stages(conf, ind_vars, tf, tconf):
     """Creates a Spark ML pipeline from the pipeline features.
     Parameters
     ----------
     conf: dictionary
@@ -174,29 +175,30 @@
     ind_vars, cols_to_pass, comparison_features, pipeline_features, for_hh=False
 ):
     categorical_comparison_features = []
     categorical_pipeline_features = []
     cols = set(cols_to_pass + ind_vars)
 
     # Check for categorical features in all comparison features
-    for x in comparison_features:
-        if x["alias"] in cols:
-            if "categorical" in x.keys():
-                categorical_comparison_features.append(x["alias"])
-        else:
-            continue
+    for comparison_feature in comparison_features:
+        if comparison_feature["alias"] in cols and comparison_feature.get(
+            "categorical", False
+        ):
+            categorical_comparison_features.append(comparison_feature["alias"])
 
     # Check for categorical features in the pipeline-generated features (if exist)
 
     if pipeline_features is not None:
         for pipeline_feature in pipeline_features:
             if pipeline_feature["output_column"] in cols and pipeline_feature.get(
                 "categorical", False
             ):
                 categorical_pipeline_features.append(pipeline_feature["output_column"])
+    logging.info(f"Categorical Comparison features: {categorical_comparison_features}")
+    logging.info(f"Categorical Pipeline features: {categorical_pipeline_features}")
 
     return categorical_comparison_features, categorical_pipeline_features
 
 
 def get_pipeline_feature_input_cols(ind_vars, pipeline_features):
     pipeline_feature_input_cols = []
     if pipeline_features is not None:
```

### Comparing `hlink-3.3.0/hlink/linking/core/substitutions.py` & `hlink-3.3.1/hlink/linking/core/substitutions.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/threshold.py` & `hlink-3.3.1/hlink/linking/core/threshold.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/core/transforms.py` & `hlink-3.3.1/hlink/linking/core/transforms.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_matching/hh_matching.py` & `hlink-3.3.1/hlink/linking/hh_matching/hh_matching.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_matching/link_step_block_on_households.py` & `hlink-3.3.1/hlink/linking/hh_matching/link_step_block_on_households.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_matching/link_step_filter.py` & `hlink-3.3.1/hlink/linking/hh_matching/link_step_filter.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_matching/templates/hh_potential_matches.sql` & `hlink-3.3.1/hlink/linking/hh_matching/templates/hh_potential_matches.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_model_exploration/hh_model_exploration.py` & `hlink-3.3.1/hlink/linking/hh_model_exploration/hh_model_exploration.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/hh_training/hh_training.py` & `hlink-3.3.1/hlink/linking/hh_training/hh_training.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/link_run.py` & `hlink-3.3.1/hlink/linking/link_run.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/link_step.py` & `hlink-3.3.1/hlink/linking/link_step.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/link_task.py` & `hlink-3.3.1/hlink/linking/link_task.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/_helpers.py` & `hlink-3.3.1/hlink/linking/matching/_helpers.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/link_step_explode.py` & `hlink-3.3.1/hlink/linking/matching/link_step_explode.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/link_step_match.py` & `hlink-3.3.1/hlink/linking/matching/link_step_match.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/link_step_score.py` & `hlink-3.3.1/hlink/linking/matching/link_step_score.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/matching.py` & `hlink-3.3.1/hlink/linking/matching/matching.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/matching/templates/potential_matches.sql` & `hlink-3.3.1/hlink/linking/matching/templates/potential_matches.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/model_exploration/link_step_create_features.py` & `hlink-3.3.1/hlink/linking/model_exploration/link_step_create_features.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/model_exploration/link_step_get_feature_importances.py` & `hlink-3.3.1/hlink/linking/model_exploration/link_step_get_feature_importances.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/model_exploration/link_step_ingest_file.py` & `hlink-3.3.1/hlink/linking/model_exploration/link_step_ingest_file.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/model_exploration/link_step_train_test_models.py` & `hlink-3.3.1/hlink/linking/model_exploration/link_step_train_test_models.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/model_exploration/model_exploration.py` & `hlink-3.3.1/hlink/linking/model_exploration/model_exploration.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/preprocessing/link_step_prep_dataframes.py` & `hlink-3.3.1/hlink/linking/preprocessing/link_step_prep_dataframes.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/preprocessing/link_step_register_raw_dfs.py` & `hlink-3.3.1/hlink/linking/preprocessing/link_step_register_raw_dfs.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/preprocessing/templates/attach_related_col.sql` & `hlink-3.3.1/hlink/linking/preprocessing/templates/attach_related_col.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql` & `hlink-3.3.1/hlink/linking/preprocessing/templates/attach_related_cols_as_rows.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/preprocessing/templates/hh_nbor_rank.sql` & `hlink-3.3.1/hlink/linking/preprocessing/templates/hh_nbor_rank.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/reporting/link_step_export_crosswalk.py` & `hlink-3.3.1/hlink/linking/reporting/link_step_export_crosswalk.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/reporting/link_step_report_r2_percent_linked.py` & `hlink-3.3.1/hlink/linking/reporting/link_step_report_r2_percent_linked.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/reporting/link_step_report_representivity.py` & `hlink-3.3.1/hlink/linking/reporting/link_step_report_representivity.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/reporting/reporting.py` & `hlink-3.3.1/hlink/linking/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/table.py` & `hlink-3.3.1/hlink/linking/table.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/table_definitions.csv` & `hlink-3.3.1/hlink/linking/table_definitions.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/aggregate_features.sql` & `hlink-3.3.1/hlink/linking/templates/shared/aggregate_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/all_household_members.sql` & `hlink-3.3.1/hlink/linking/templates/shared/all_household_members.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/drop_links.sql` & `hlink-3.3.1/hlink/linking/templates/shared/drop_links.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/hh_aggregate_features.sql` & `hlink-3.3.1/hlink/linking/templates/shared/hh_aggregate_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql` & `hlink-3.3.1/hlink/linking/templates/shared/includes/all_household_members_selects_a.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql` & `hlink-3.3.1/hlink/linking/templates/shared/includes/all_household_members_selects_b.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/potential_matches_base_features.sql` & `hlink-3.3.1/hlink/linking/templates/shared/potential_matches_base_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/tfam_tables.sql` & `hlink-3.3.1/hlink/linking/templates/shared/tfam_tables.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/templates/shared/training_features.sql` & `hlink-3.3.1/hlink/linking/templates/shared/training_features.sql`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/training/link_step_create_comparison_features.py` & `hlink-3.3.1/hlink/linking/training/link_step_create_comparison_features.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/training/link_step_ingest_file.py` & `hlink-3.3.1/hlink/linking/training/link_step_ingest_file.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/training/link_step_train_and_save_model.py` & `hlink-3.3.1/hlink/linking/training/link_step_train_and_save_model.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/training/training.py` & `hlink-3.3.1/hlink/linking/training/training.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/transformers/float_cast_transformer.py` & `hlink-3.3.1/hlink/linking/transformers/float_cast_transformer.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/transformers/interaction_transformer.py` & `hlink-3.3.1/hlink/linking/transformers/interaction_transformer.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/transformers/rename_prob_column.py` & `hlink-3.3.1/hlink/linking/transformers/rename_prob_column.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/linking/util.py` & `hlink-3.3.1/hlink/linking/util.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/conf_validations.py` & `hlink-3.3.1/hlink/scripts/lib/conf_validations.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/experimental/reporting.py` & `hlink-3.3.1/hlink/scripts/lib/experimental/reporting.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/experimental/tfam.py` & `hlink-3.3.1/hlink/scripts/lib/experimental/tfam.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/io.py` & `hlink-3.3.1/hlink/scripts/lib/io.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/linking_ops.py` & `hlink-3.3.1/hlink/scripts/lib/linking_ops.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/table_ops.py` & `hlink-3.3.1/hlink/scripts/lib/table_ops.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/lib/util.py` & `hlink-3.3.1/hlink/scripts/lib/util.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/scripts/main.py` & `hlink-3.3.1/hlink/scripts/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is part of the ISRDI's hlink.
 # For copyright and licensing information, see the NOTICE and LICENSE files
 # in this project's top-level directory, and also on-line at:
 #   https://github.com/ipums/hlink
 
 import argparse
 import getpass
-from importlib import reload
 import logging
 import os
 from pathlib import Path
 import json
 import pkg_resources
 import readline
 import sys
@@ -221,39 +220,22 @@
         report_and_log_error("", err)
 
     while True:
         main = Main(LinkRun(spark, run_conf), start_task=args.task)
         try:
             main.cmdloop()
             if main.lastcmd == "reload":
-                _reload_modules()
-                # Reload modules twice in order to fix import problem
-                # with the _*.py files in the linking modules
-                _reload_modules()
+                logging.info("Reloading config file")
                 run_conf = load_conf(args.conf, args.user)
             else:
                 break
         except Exception as err:
             report_and_log_error("", err)
 
 
-def _reload_modules():
-    no_reloads = []
-    mods_to_reload_raw = [name for name, mod in sys.modules.items()]
-    # We need to order the modules to reload the _*.py files in the
-    # linking modules before loading the __init__.py files.
-    mods_to_reload_ordered = sorted(mods_to_reload_raw)[::-1]
-    for name in mods_to_reload_ordered:
-        if name.startswith("hlink") and name not in no_reloads:
-            reload(sys.modules[name])
-
-    # Here we should reset the classes in link_run.link_task_choices with
-    # the newly reloaded classes.
-
-
 def _setup_logging(conf):
     log_dir = Path(conf["log_dir"])
     log_dir.mkdir(exist_ok=True, parents=True)
 
     user = getpass.getuser()
     session_id = uuid.uuid4().hex
     conf_name = Path(conf["conf_path"]).stem
```

### Comparing `hlink-3.3.0/hlink/scripts/main_loop.py` & `hlink-3.3.1/hlink/scripts/main_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     def do_q(self, split_args):
         """Quits the program.
         Usage: q"""
         return True
 
     @split_and_check_args(0)
     def do_reload(self, split_args):
-        """Hot reload modules.
+        """Reload the config file.
         Usage: reload"""
         return "reload"
 
     @split_and_check_args(1)
     def do_set_link_task(self, split_args):
         """Set the linking task to run steps for.
         Arg 1: task
```

### Comparing `hlink-3.3.0/hlink/spark/factory.py` & `hlink-3.3.1/hlink/spark/factory.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/spark/jars/hlink_lib-assembly-1.0.jar` & `hlink-3.3.1/hlink/spark/jars/hlink_lib-assembly-1.0.jar`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/spark/session.py` & `hlink-3.3.1/hlink/spark/session.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/conf/integration.toml` & `hlink-3.3.1/hlink/tests/conf/integration.toml`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/conf_validations_test.py` & `hlink-3.3.1/hlink/tests/conf_validations_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/config_loader_test.py` & `hlink-3.3.1/hlink/tests/config_loader_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/conftest.py` & `hlink-3.3.1/hlink/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/core/comparison_core_test.py` & `hlink-3.3.1/hlink/tests/core/comparison_core_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/hh_matching_test.py` & `hlink-3.3.1/hlink/tests/hh_matching_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/hh_model_exploration_test.py` & `hlink-3.3.1/hlink/tests/hh_model_exploration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs.csv` & `hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv` & `hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv` & `hlink-3.3.1/hlink/tests/input_data/19thc_nativity_test_hhs_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/calc_mfbpl_a.csv` & `hlink-3.3.1/hlink/tests/input_data/calc_mfbpl_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/calc_mfbpl_b.csv` & `hlink-3.3.1/hlink/tests/input_data/calc_mfbpl_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/crosswalk/raw_df_a.csv` & `hlink-3.3.1/hlink/tests/input_data/crosswalk/raw_df_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/crosswalk/raw_df_b.csv` & `hlink-3.3.1/hlink/tests/input_data/crosswalk/raw_df_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/ha_source.csv` & `hlink-3.3.1/hlink/tests/input_data/ha_source.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/handle_null.csv` & `hlink-3.3.1/hlink/tests/input_data/handle_null.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/hb_source.csv` & `hlink-3.3.1/hlink/tests/input_data/hb_source.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/hh_matching_a.csv` & `hlink-3.3.1/hlink/tests/input_data/hh_matching_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/hh_matching_b.csv` & `hlink-3.3.1/hlink/tests/input_data/hh_matching_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/hhpm_agg_test.csv` & `hlink-3.3.1/hlink/tests/input_data/hhpm_agg_test.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/households_b.parquet` & `hlink-3.3.1/hlink/tests/input_data/households_b.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/matched_men.csv` & `hlink-3.3.1/hlink/tests/input_data/matched_men.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/matching_test_a.csv` & `hlink-3.3.1/hlink/tests/input_data/matching_test_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/matching_test_b.csv` & `hlink-3.3.1/hlink/tests/input_data/matching_test_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/new_hh_test_td.csv` & `hlink-3.3.1/hlink/tests/input_data/new_hh_test_td.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/potential_matches.csv` & `hlink-3.3.1/hlink/tests/input_data/potential_matches.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/potential_matches_agg.csv` & `hlink-3.3.1/hlink/tests/input_data/potential_matches_agg.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/prepped_df_reporting.csv` & `hlink-3.3.1/hlink/tests/input_data/prepped_df_reporting.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/raw_df_reporting.csv` & `hlink-3.3.1/hlink/tests/input_data/raw_df_reporting.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/region.csv` & `hlink-3.3.1/hlink/tests/input_data/region.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/rel_rows_test_a.csv` & `hlink-3.3.1/hlink/tests/input_data/rel_rows_test_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/rel_rows_test_b.csv` & `hlink-3.3.1/hlink/tests/input_data/rel_rows_test_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/representivity.csv` & `hlink-3.3.1/hlink/tests/input_data/representivity.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/statedist.csv` & `hlink-3.3.1/hlink/tests/input_data/statedist.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/street_abbrevs.csv` & `hlink-3.3.1/hlink/tests/input_data/street_abbrevs.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/street_abbrevs_most_common.csv` & `hlink-3.3.1/hlink/tests/input_data/street_abbrevs_most_common.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet` & `hlink-3.3.1/hlink/tests/input_data/test_parquet_data_a.parquet/part-00000-8465f06e-9bb0-4817-81eb-813ccf07429a-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet` & `hlink-3.3.1/hlink/tests/input_data/test_parquet_data_b.parquet/part-00000-bb515275-04b4-4a16-80f1-5cc21450b93f-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/training_data_households.csv` & `hlink-3.3.1/hlink/tests/input_data/training_data_households.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/training_data_households.parquet` & `hlink-3.3.1/hlink/tests/input_data/training_data_households.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/training_data_long.csv` & `hlink-3.3.1/hlink/tests/input_data/training_data_long.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/training_data_long_a.csv` & `hlink-3.3.1/hlink/tests/input_data/training_data_long_a.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/input_data/training_data_long_b.csv` & `hlink-3.3.1/hlink/tests/input_data/training_data_long_b.csv`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/integration_score_with_trained_models_test.py` & `hlink-3.3.1/hlink/tests/integration_score_with_trained_models_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/integration_test.py` & `hlink-3.3.1/hlink/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/logging_test.py` & `hlink-3.3.1/hlink/tests/logging_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/main_loop_test.py` & `hlink-3.3.1/hlink/tests/main_loop_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/main_test.py` & `hlink-3.3.1/hlink/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_blocking_explode_test.py` & `hlink-3.3.1/hlink/tests/matching_blocking_explode_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_comparison_features_test.py` & `hlink-3.3.1/hlink/tests/matching_comparison_features_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_geo_distance_test.py` & `hlink-3.3.1/hlink/tests/matching_geo_distance_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_potential_matches_test.py` & `hlink-3.3.1/hlink/tests/matching_potential_matches_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_potential_matches_universe_test.py` & `hlink-3.3.1/hlink/tests/matching_potential_matches_universe_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_scoring_test.py` & `hlink-3.3.1/hlink/tests/matching_scoring_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/matching_test.py` & `hlink-3.3.1/hlink/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/model_exploration_test.py` & `hlink-3.3.1/hlink/tests/model_exploration_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/plugins/datasources.py` & `hlink-3.3.1/hlink/tests/plugins/datasources.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/plugins/external_data_paths.py` & `hlink-3.3.1/hlink/tests/plugins/external_data_paths.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/preprocessing_test.py` & `hlink-3.3.1/hlink/tests/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/reporting_test.py` & `hlink-3.3.1/hlink/tests/reporting_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/scala_udf_test.py` & `hlink-3.3.1/hlink/tests/scala_udf_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/table_test.py` & `hlink-3.3.1/hlink/tests/table_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/training_test.py` & `hlink-3.3.1/hlink/tests/training_test.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet` & `hlink-3.3.1/hlink/tests/validation_data/training_p_all.parquet/part-00000-6c9e5760-174a-4652-b687-6823087ed5bf-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/hlink.egg-info/PKG-INFO` & `hlink-3.3.1/hlink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlink
-Version: 3.3.0
+Version: 3.3.1
 Summary: Fast supervised pyspark record linkage software
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
         
@@ -382,24 +382,28 @@
 Project-URL: Changelog, https://github.com/ipums/hlink/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
+License-File: NOTICE.txt
 
 [![HLink Docker CI](https://github.com/ipums/hlink/actions/workflows/docker-build.yml/badge.svg)](https://github.com/ipums/hlink/actions/workflows/docker-build.yml)
 
 # hlink: hierarchical record linkage at scale
 
 hlink is a Python package that provides a flexible, configuration-driven solution to probabilistic record linking at scale. It provides a high-level API for python as well as a standalone command line interface for running linking jobs with little to no programming. hlink supports the linking process from beginning to end, including preprocessing, filtering, training, model exploration, blocking, feature generation and scoring.
 
 It is used at [IPUMS](https://www.ipums.org/) to link U.S. historical census data, but can be applied to any record linkage job. 
 A paper on the creation and applications of this program on historical census data can be found at <https://www.tandfonline.com/doi/full/10.1080/01615440.2021.1985027>.
 
+### Suggested Citation
+Wellington, J., R. Harper, and K.J. Thompson. 2022. "hlink." https://github.com/ipums/hlink: Institute for Social Research and Data Innovation, University of Minnesota.
+
 ## Installation
 
 hlink runs on Python 3.10.
 Java 8 or [Java 11](https://openjdk.org/install/) is required for the PySpark integration. 
 
 You can install the python package from pip:
 ```
```

### Comparing `hlink-3.3.0/hlink.egg-info/SOURCES.txt` & `hlink-3.3.1/hlink.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -227,14 +227,15 @@
 hlink/tests/conf/no_id_column_b.toml
 hlink/tests/conf/test.json
 hlink/tests/conf/test1.toml
 hlink/tests/conf/test_conf_flag_run.json
 hlink/tests/conf/test_run.json
 hlink/tests/core/__init__.py
 hlink/tests/core/comparison_core_test.py
+hlink/tests/core/pipeline_core_test.py
 hlink/tests/input_data/19thc_nativity_test_hhs.csv
 hlink/tests/input_data/19thc_nativity_test_hhs_a.csv
 hlink/tests/input_data/19thc_nativity_test_hhs_b.csv
 hlink/tests/input_data/birthyr_replace.csv
 hlink/tests/input_data/calc_mfbpl_a.csv
 hlink/tests/input_data/calc_mfbpl_b.csv
 hlink/tests/input_data/county_distances.csv
```

### Comparing `hlink-3.3.0/pyproject.toml` & `hlink-3.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hlink"
-version = "3.3.0"
+version = "3.3.1"
 description = "Fast supervised pyspark record linkage software"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
```

### Comparing `hlink-3.3.0/scala_jar/build.sbt` & `hlink-3.3.1/scala_jar/build.sbt`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ArrayToString.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/AttachHHColumn.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/AttachRelatedRows.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ExtraChildren.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ExtractNeighbors.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHCompare.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHDrop.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HHGetFirstValue.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/HasMatchingElement.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/JWRate.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/JWRelatedRows.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/MaxJWCompare.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/ParseProbabilityVector.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/SerJaroWinklerSimilarity.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala` & `hlink-3.3.1/scala_jar/src/main/scala/com/isrdi/udfs/VectorToString.scala`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/Makefile` & `hlink-3.3.1/sphinx-docs/Makefile`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/comparison_types.md` & `hlink-3.3.1/sphinx-docs/comparison_types.md`

 * *Files 1% similar despite different names*

```diff
@@ -642,18 +642,19 @@
 column_name = "race"
 comparison_type = "fetch_b"
 categorical = true
 ```
 
 ### present_both_years
 
-Checks whether both column A and column B are present.
+Checks whether column A and column B are both present and both positive (> 0).
+Evaluates to 1 if both are present and positive and 0 otherwise.
 
 * Attributes:
-  * `column_name` -- Type: `string`. The column to check.
+  * `column_name` -- Type: `string`. The column to check. Must be a column with a numerical type.
 
 ```
 [[comparison_features]]
 alias = "sp_caution"
 column_names = ["spouse_bpl", "spouse_birthyr", "durmarr", "sploc"]
 comparison_type = "caution_comp_4"
 categorical = true
@@ -671,28 +672,37 @@
 [comparison_features.comp_d]
 column_name = "sploc"
 comparison_type = "present_both_years"
 ```
 
 ### neither_are_null
 
-Checks that neither column A nor column B is null.
+Checks that neither column A nor column B is null or the empty string `''`.
+Evaluates to 1 if neither column is null or `''` and evaluates to 0 otherwise.
 
 * Attributes:
-  * `column_name` -- Type: `string`. The column to check.
+  * `column_name` -- Type: `string`. The column of type string to check.
+
+```
+[[comparison_features]]
+alias = "mpres"
+column_name = "m_namefrst"
+comparison_type = "neither_are_null"
+categorical = true
+```
 
 ### present_and_matching_categorical
 
 Checks that both column A and column B are present and that they match according to SQL's `IS DISTINCT FROM`. Evaluates to 0, 1, or 2:
 
-0 -> columns are both present and match
+0 → columns are both present and match
 
-1 -> columns are both present but are distinct
+1 → columns are both present but are distinct
 
-2 -> one or both columns are missing
+2 → one or both columns are missing
 
 * Attributes:
   * `column_name` -- Type: `string`. Required. The column to check.
 
 ### present_and_not_equal
 
 Checks that column A and column B are both present but are not equal.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hlink-3.3.0/sphinx-docs/conf.py` & `hlink-3.3.1/sphinx-docs/conf.py`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/config.md` & `hlink-3.3.1/sphinx-docs/config.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/feature_selection_transforms.md` & `hlink-3.3.1/sphinx-docs/feature_selection_transforms.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/index.rst` & `hlink-3.3.1/sphinx-docs/index.rst`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/installation.md` & `hlink-3.3.1/sphinx-docs/installation.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/introduction.md` & `hlink-3.3.1/sphinx-docs/introduction.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/link_tasks.md` & `hlink-3.3.1/sphinx-docs/link_tasks.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/make.bat` & `hlink-3.3.1/sphinx-docs/make.bat`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/models.md` & `hlink-3.3.1/sphinx-docs/models.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/pipeline_features.md` & `hlink-3.3.1/sphinx-docs/pipeline_features.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/running_the_program.md` & `hlink-3.3.1/sphinx-docs/running_the_program.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/substitutions.md` & `hlink-3.3.1/sphinx-docs/substitutions.md`

 * *Files identical despite different names*

### Comparing `hlink-3.3.0/sphinx-docs/use_examples.md` & `hlink-3.3.1/sphinx-docs/use_examples.md`

 * *Files identical despite different names*

