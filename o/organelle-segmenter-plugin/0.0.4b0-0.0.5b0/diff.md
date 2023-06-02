# Comparing `tmp/organelle-segmenter-plugin-0.0.4b0.tar.gz` & `tmp/organelle-segmenter-plugin-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "organelle-segmenter-plugin-0.0.4b0.tar", last modified: Sat May 13 07:15:19 2023, max compression
+gzip compressed data, was "organelle-segmenter-plugin-0.0.5b0.tar", last modified: Fri Jun  2 04:33:10 2023, max compression
```

## Comparing `organelle-segmenter-plugin-0.0.4b0.tar` & `organelle-segmenter-plugin-0.0.5b0.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.020208 organelle-segmenter-plugin-0.0.4b0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-ER.json
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-LD.json
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-golgi.json
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-lyso.json
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-masks2.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-mito.json
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412-perox.json
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/20230412_MCZ-masks.json
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/ER_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/LD_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-13 07:15:19.020208 organelle-segmenter-plugin-0.0.4b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/depricated/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/depricated/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/docs/organelle_segmenter_plugin.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/env_create.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/golgi_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/lyso_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/mask_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/masks_MCZ_test.json
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/masks_test.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/mito_test.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/mynewworkflow.json
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/new_ifer_nuclei.json
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/nuc.json
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/nuc2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.004208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.004208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.004208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/batch_processing_controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/workflow_select_controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/workflow_steps_controller_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/application_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/layer_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/router_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/state_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/view_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/viewer_abstraction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/model/segmenter_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/style_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/util/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/util/lazy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/_main_template_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/batch_processing_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/workflow_select_view_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/workflow_steps_view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/collapsible_box_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/file_input_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/warning_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/workflow_step_widget_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/workflow_thumbnails_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.000208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.020208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/expand_less_black_24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/expand_more_black_24dp.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/gear.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/icon-parameter-sweep.svg
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/warning.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.008208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/batch_processing_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/workflow_select_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/workflow_steps_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.012208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/layer_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/view_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/viewer_abstraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.012208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/model/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/model/segmenter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.020208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/styles/main.qss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.012208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/ui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.012208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/_main_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/batch_processing_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/workflow_select_view.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/workflow_steps_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/batch_complete_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/collapsible_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/float_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/param_sweep_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/warning_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/workflow_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/workflow_step_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 07:15:19.016208 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-13 07:15:18.000000 organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/perox_test.json
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-13 07:15:19.020208 organelle-segmenter-plugin-0.0.4b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-13 07:15:10.000000 organelle-segmenter-plugin-0.0.4b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.272527 organelle-segmenter-plugin-0.0.5b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-ER.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-LD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-golgi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-lyso.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-masks2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-mito.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412-perox.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/20230412_MCZ-masks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/ER_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/LD_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-02 04:33:10.272527 organelle-segmenter-plugin-0.0.5b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.268527 organelle-segmenter-plugin-0.0.5b0/depricated/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/depricated/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.268527 organelle-segmenter-plugin-0.0.5b0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/docs/organelle_segmenter_plugin.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/env_create.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/golgi_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/lyso_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/mask_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/masks_MCZ_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/masks_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/mito_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/mynewworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/new_ifer_nuclei.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/nuc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/nuc2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.252527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.252527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.256527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/batch_processing_controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/workflow_select_controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/workflow_steps_controller_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.256527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/application_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/layer_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/router_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/state_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/view_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/viewer_abstraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.256527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/model/segmenter_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/style_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.256527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/util/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/util/lazy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.256527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/_main_template_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/batch_processing_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/workflow_select_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/workflow_steps_view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.260527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/collapsible_box_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/file_input_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/warning_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/workflow_step_widget_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/workflow_thumbnails_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.248527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.268527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/expand_less_black_24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/expand_more_black_24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/gear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/icon-parameter-sweep.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/warning.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.260527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/batch_processing_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/workflow_select_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28107 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/workflow_steps_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.260527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/layer_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/view_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/viewer_abstraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.260527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/model/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/model/segmenter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.260527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/styles/main.qss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/ui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/_main_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/batch_processing_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/workflow_select_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/workflow_steps_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.264527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/batch_complete_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/collapsible_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/float_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/param_sweep_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/warning_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/workflow_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/workflow_step_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 04:33:10.268527 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 04:33:10.000000 organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/perox_test.json
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-02 04:33:10.272527 organelle-segmenter-plugin-0.0.5b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-02 04:33:02.000000 organelle-segmenter-plugin-0.0.5b0/setup.py
```

### Comparing `organelle-segmenter-plugin-0.0.4b0/.github/workflows/publish.yml` & `organelle-segmenter-plugin-0.0.5b0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/.gitignore` & `organelle-segmenter-plugin-0.0.5b0/.gitignore`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/.napari-hub/config.yml` & `organelle-segmenter-plugin-0.0.5b0/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-ER.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-ER.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-LD.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-LD.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-golgi.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-golgi.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-lyso.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-lyso.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-masks2.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-masks2.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-mito.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-mito.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412-perox.json` & `organelle-segmenter-plugin-0.0.5b0/20230412-perox.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/20230412_MCZ-masks.json` & `organelle-segmenter-plugin-0.0.5b0/20230412_MCZ-masks.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/CODE_OF_CONDUCT.md` & `organelle-segmenter-plugin-0.0.5b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/CONTRIBUTING.md` & `organelle-segmenter-plugin-0.0.5b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/ER_test.json` & `organelle-segmenter-plugin-0.0.5b0/ER_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/LD_test.json` & `organelle-segmenter-plugin-0.0.5b0/LD_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/LICENSE` & `organelle-segmenter-plugin-0.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/PKG-INFO` & `organelle-segmenter-plugin-0.0.5b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organelle-segmenter-plugin
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: A plugin that enables organelle segmentation, forked from tools from Allen Institute for Cell Science
 Home-page: https://github.com/ndcn/organelle-segmenter-plugin
 Author: Andy Henrie
 Author-email: ergonyc@gmail.com
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/ndcn/organelle-segmenter-plugin/issues
 Project-URL: Documentation, https://github.com/ndcn/organelle-segmenter-plugin#README.md
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `organelle-segmenter-plugin-0.0.4b0/README.md` & `organelle-segmenter-plugin-0.0.5b0/README.md`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/depricated/_setup.py` & `organelle-segmenter-plugin-0.0.5b0/depricated/_setup.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/depricated/plugin_preview.yml` & `organelle-segmenter-plugin-0.0.5b0/depricated/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/depricated/publish.yml` & `organelle-segmenter-plugin-0.0.5b0/depricated/publish.yml`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/depricated/setup.cfg` & `organelle-segmenter-plugin-0.0.5b0/depricated/setup.cfg`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/depricated/setup.py` & `organelle-segmenter-plugin-0.0.5b0/depricated/setup.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/docs/index.md` & `organelle-segmenter-plugin-0.0.5b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/docs/organelle_segmenter_plugin.md` & `organelle-segmenter-plugin-0.0.5b0/docs/organelle_segmenter_plugin.md`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/env_create.sh` & `organelle-segmenter-plugin-0.0.5b0/env_create.sh`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/golgi_test.json` & `organelle-segmenter-plugin-0.0.5b0/golgi_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/lyso_test.json` & `organelle-segmenter-plugin-0.0.5b0/lyso_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/mask_test.json` & `organelle-segmenter-plugin-0.0.5b0/mask_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/masks_MCZ_test.json` & `organelle-segmenter-plugin-0.0.5b0/masks_MCZ_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/masks_test.json` & `organelle-segmenter-plugin-0.0.5b0/masks_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/mito_test.json` & `organelle-segmenter-plugin-0.0.5b0/mito_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/mynewworkflow.json` & `organelle-segmenter-plugin-0.0.5b0/mynewworkflow.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/new_ifer_nuclei.json` & `organelle-segmenter-plugin-0.0.5b0/new_ifer_nuclei.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/nuc.json` & `organelle-segmenter-plugin-0.0.5b0/nuc.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/nuc2.json` & `organelle-segmenter-plugin-0.0.5b0/nuc2.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_dock_widget.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_reader.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_reader.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_style.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_style.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/conftest.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/batch_processing_controller_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/batch_processing_controller_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/workflow_select_controller_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/workflow_select_controller_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/controller/workflow_steps_controller_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/controller/workflow_steps_controller_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/application_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/application_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/controller_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/controller_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/layer_reader_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/layer_reader_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/router_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/router_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/view_manager_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/view_manager_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/view_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/view_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/core/viewer_abstraction_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/core/viewer_abstraction_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/mocks.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/mocks.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/model/segmenter_model_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/model/segmenter_model_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/style_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/style_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/util/convert_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/util/convert_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/batch_processing_view_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/batch_processing_view_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/workflow_select_view_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/workflow_select_view_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/view/workflow_steps_view_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/view/workflow_steps_view_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/collapsible_box_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/collapsible_box_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/warning_message_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/warning_message_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/workflow_step_widget_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/workflow_step_widget_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/_tests/widgets/workflow_thumbnails_test.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/_tests/widgets/workflow_thumbnails_test.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/gear.svg` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/gear.svg`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/icon-parameter-sweep.svg` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/icon-parameter-sweep.svg`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/assets/icons/warning.png` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/assets/icons/warning.png`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/_interfaces.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/_interfaces.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/batch_processing_controller.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/batch_processing_controller.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/workflow_select_controller.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/workflow_select_controller.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/controller/workflow_steps_controller.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/controller/workflow_steps_controller.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/_interfaces.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/_interfaces.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/application.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/application.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/controller.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/controller.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/layer_reader.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/layer_reader.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/router.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/router.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/view.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/view.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/view_manager.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/view_manager.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/core/viewer_abstraction.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/core/viewer_abstraction.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/model/segmenter_model.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/model/segmenter_model.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/napari.yaml` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/napari.yaml`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/styles/main.qss` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/styles/main.qss`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/convert.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/convert.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/debug_utils.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/debug_utils.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/directories.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/directories.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/util/ui_utils.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/util/ui_utils.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/_main_template.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/_main_template.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/batch_processing_view.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/batch_processing_view.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/workflow_select_view.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/workflow_select_view.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/view/workflow_steps_view.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/view/workflow_steps_view.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/batch_complete_dialog.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/batch_complete_dialog.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/collapsible_box.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/collapsible_box.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/file_input.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/file_input.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/float_slider.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/float_slider.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/form.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/form.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/param_sweep_widget.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/param_sweep_widget.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/warning_message.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/warning_message.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/workflow_buttons.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/workflow_buttons.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin/widgets/workflow_step_widget.py` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin/widgets/workflow_step_widget.py`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/PKG-INFO` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: organelle-segmenter-plugin
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: A plugin that enables organelle segmentation, forked from tools from Allen Institute for Cell Science
 Home-page: https://github.com/ndcn/organelle-segmenter-plugin
 Author: Andy Henrie
 Author-email: ergonyc@gmail.com
 License: BSD-3
 Project-URL: Bug Tracker, https://github.com/ndcn/organelle-segmenter-plugin/issues
 Project-URL: Documentation, https://github.com/ndcn/organelle-segmenter-plugin#README.md
@@ -17,15 +17,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
```

### Comparing `organelle-segmenter-plugin-0.0.4b0/organelle_segmenter_plugin.egg-info/SOURCES.txt` & `organelle-segmenter-plugin-0.0.5b0/organelle_segmenter_plugin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 ./organelle_segmenter_plugin/core/state.py
 ./organelle_segmenter_plugin/core/view.py
 ./organelle_segmenter_plugin/core/view_manager.py
 ./organelle_segmenter_plugin/core/viewer_abstraction.py
 ./organelle_segmenter_plugin/model/__init__.py
 ./organelle_segmenter_plugin/model/channel.py
 ./organelle_segmenter_plugin/model/segmenter_model.py
+./organelle_segmenter_plugin/styles/main.qss
 ./organelle_segmenter_plugin/util/__init__.py
 ./organelle_segmenter_plugin/util/convert.py
 ./organelle_segmenter_plugin/util/debug_utils.py
 ./organelle_segmenter_plugin/util/directories.py
 ./organelle_segmenter_plugin/util/lazy.py
 ./organelle_segmenter_plugin/util/ui_utils.py
 ./organelle_segmenter_plugin/view/__init__.py
```

### Comparing `organelle-segmenter-plugin-0.0.4b0/perox_test.json` & `organelle-segmenter-plugin-0.0.5b0/perox_test.json`

 * *Files identical despite different names*

### Comparing `organelle-segmenter-plugin-0.0.4b0/setup.cfg` & `organelle-segmenter-plugin-0.0.5b0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	Topic :: Scientific/Engineering :: Visualization
 	Topic :: Scientific/Engineering :: Information Analysis
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 	License :: OSI Approved :: BSD License
 project_urls = 
 	Bug Tracker = https://github.com/ndcn/organelle-segmenter-plugin/issues
 	Documentation = https://github.com/ndcn/organelle-segmenter-plugin#README.md
 	Source Code = https://github.com/ndcn/organelle-segmenter-plugin
 	User Support = https://github.com/ndcn/organelle-segmenter-plugin/issues
@@ -58,13 +58,13 @@
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
 	pytest-qt  # https://pytest-qt.readthedocs.io/en/latest/
 	napari
 	pyqt5
 
 [options.package_data]
-* = *.yaml
+* = *.yaml, *.json, styles/*.*, *.qss
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

