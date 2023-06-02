# Comparing `tmp/caikit-0.6.0.tar.gz` & `tmp/caikit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.6.0.tar` & `caikit-0.7.0.tar`

### file list

```diff
@@ -1,305 +1,304 @@
--rw-r--r--   0        0        0       60 2023-05-25 17:25:38.753862 caikit-0.6.0/.coveragerc
--rw-r--r--   0        0        0      676 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1452 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-05-25 17:25:38.753862 caikit-0.6.0/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      261 2023-05-25 17:25:38.753862 caikit-0.6.0/.gitignore
--rw-r--r--   0        0        0      324 2023-05-25 17:25:38.753862 caikit-0.6.0/.isort.cfg
--rw-r--r--   0        0        0      370 2023-05-25 17:25:38.753862 caikit-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-05-25 17:25:38.753862 caikit-0.6.0/.prettierignore
--rw-r--r--   0        0        0       12 2023-05-25 17:25:38.753862 caikit-0.6.0/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-05-25 17:25:38.753862 caikit-0.6.0/.pylintrc
--rw-r--r--   0        0        0       78 2023-05-25 17:25:38.753862 caikit-0.6.0/.whitesource
--rw-r--r--   0        0        0      368 2023-05-25 17:25:38.753862 caikit-0.6.0/CODEOWNERS
--rw-r--r--   0        0        0     7165 2023-05-25 17:25:38.753862 caikit-0.6.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-05-25 17:25:38.753862 caikit-0.6.0/LICENSE
--rw-r--r--   0        0        0     3734 2023-05-25 17:25:38.753862 caikit-0.6.0/README.md
--rw-r--r--   0        0        0      152 2023-05-25 17:25:38.753862 caikit-0.6.0/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit/config/__init__.py
--rw-r--r--   0        0        0     6052 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit/config/config.py
--rw-r--r--   0        0        0     6488 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-05-25 17:25:38.753862 caikit-0.6.0/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    35986 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4050 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    14380 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4858 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1564 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40212 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21296 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2834 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4718 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2802 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     6002 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30320 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6247 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11042 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4151 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    13024 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3895 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10721 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     7841 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0     6961 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/task.py
--rw-r--r--   0        0        0     1001 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21366 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     4935 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1648 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    32206 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0      530 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14200 2023-05-25 17:25:38.757862 caikit-0.6.0/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4659 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12101 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4311 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1480 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    16699 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3043 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5809 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    13914 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     7136 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    12688 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2571 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9476 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    15326 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5539 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6810 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    17892 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-05-25 17:25:38.761862 caikit-0.6.0/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      169 2023-05-25 17:25:38.761862 caikit-0.6.0/code-of-conduct.md
--rw-r--r--   0        0        0       68 2023-05-25 17:25:38.761862 caikit-0.6.0/docs-requirements.txt
--rw-r--r--   0        0        0      634 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/Makefile
--rw-r--r--   0        0        0     1610 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/architecture_club/README.md
--rw-r--r--   0        0        0     2660 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/conf.py
--rw-r--r--   0        0        0      225 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-25 17:25:38.761862 caikit-0.6.0/docs/make.bat
--rw-r--r--   0        0        0      837 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1427 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       72 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      742 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3067 2023-05-25 17:25:38.761862 caikit-0.6.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     1196 2023-05-25 17:25:42.985879 caikit-0.6.0/pyproject.toml
--rwxr-xr-x   0        0        0      639 2023-05-25 17:25:38.761862 caikit-0.6.0/scripts/check_deps.sh
--rwxr-xr-x   0        0        0      720 2023-05-25 17:25:38.761862 caikit-0.6.0/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-05-25 17:25:38.761862 caikit-0.6.0/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     3439 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/base.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/config/test_configs.py
--rw-r--r--   0        0        0     8956 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5033 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26459 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16232 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    20601 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     1104 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4357 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    12551 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/test_imports.py
--rw-r--r--   0        0        0    21373 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     5110 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/test_task.py
--rw-r--r--   0        0        0     7967 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4997 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      647 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1016 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      506 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     3034 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      410 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      157 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-05-25 17:25:38.765862 caikit-0.6.0/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1882 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      250 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      621 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1282 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      364 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     3349 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18431 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     4065 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/test_primitives.py
--rw-r--r--   0        0        0     1688 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     7859 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    15481 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3640 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7372 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    30156 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0    11106 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26269 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-05-25 17:25:38.769862 caikit-0.6.0/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2115 2023-05-25 17:25:38.769862 caikit-0.6.0/tox.ini
--rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 caikit-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-06-02 21:55:42.640922 caikit-0.7.0/.coveragerc
+-rw-r--r--   0        0        0      676 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1571 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-06-02 21:55:42.640922 caikit-0.7.0/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      246 2023-06-02 21:55:42.640922 caikit-0.7.0/.gitignore
+-rw-r--r--   0        0        0      324 2023-06-02 21:55:42.640922 caikit-0.7.0/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-06-02 21:55:42.640922 caikit-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-06-02 21:55:42.640922 caikit-0.7.0/.prettierignore
+-rw-r--r--   0        0        0       12 2023-06-02 21:55:42.640922 caikit-0.7.0/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-06-02 21:55:42.640922 caikit-0.7.0/.pylintrc
+-rw-r--r--   0        0        0      530 2023-06-02 21:55:42.640922 caikit-0.7.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-06-02 21:55:42.640922 caikit-0.7.0/.whitesource
+-rw-r--r--   0        0        0      368 2023-06-02 21:55:42.640922 caikit-0.7.0/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-06-02 21:55:42.640922 caikit-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-06-02 21:55:42.640922 caikit-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3734 2023-06-02 21:55:42.640922 caikit-0.7.0/README.md
+-rw-r--r--   0        0        0      152 2023-06-02 21:55:42.640922 caikit-0.7.0/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6052 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-06-02 21:55:42.640922 caikit-0.7.0/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    37315 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2446 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4997 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    14537 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4858 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40212 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21296 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2834 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4718 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2802 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     6002 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30320 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6247 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11042 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4151 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    13024 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3895 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10721 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     7590 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/task.py
+-rw-r--r--   0        0        0     1001 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21366 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     4935 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1648 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32206 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0      530 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-06-02 21:55:42.644922 caikit-0.7.0/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14335 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15675 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4659 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12101 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4311 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1480 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    12209 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    13914 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5613 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    11999 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     9476 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12441 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6810 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    19162 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    11539 2023-06-02 21:55:42.648922 caikit-0.7.0/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-06-02 21:55:42.648922 caikit-0.7.0/code-of-conduct.md
+-rw-r--r--   0        0        0       90 2023-06-02 21:55:42.648922 caikit-0.7.0/docs-requirements.txt
+-rw-r--r--   0        0        0      639 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0     1610 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-06-02 21:55:42.648922 caikit-0.7.0/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-06-02 21:55:42.652922 caikit-0.7.0/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1376 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       72 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3067 2023-06-02 21:55:42.652922 caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     1234 2023-06-02 21:55:46.829213 caikit-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-06-02 21:55:42.652922 caikit-0.7.0/releases.md
+-rwxr-xr-x   0        0        0      639 2023-06-02 21:55:42.652922 caikit-0.7.0/scripts/check_deps.sh
+-rwxr-xr-x   0        0        0      720 2023-06-02 21:55:42.652922 caikit-0.7.0/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-06-02 21:55:42.652922 caikit-0.7.0/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/base.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/config/test_configs.py
+-rw-r--r--   0        0        0     9913 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5033 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26459 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16232 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    23532 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    12551 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21849 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     6133 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/test_task.py
+-rw-r--r--   0        0        0     7967 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4997 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-06-02 21:55:42.652922 caikit-0.7.0/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     3034 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     5995 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0       24 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      157 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1257 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1942 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      250 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      620 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1368 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      364 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18431 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3105 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8307 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16742 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    33005 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-06-02 21:55:42.656923 caikit-0.7.0/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26059 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-06-02 21:55:42.660923 caikit-0.7.0/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2556 2023-06-02 21:55:42.660923 caikit-0.7.0/tox.ini
+-rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 caikit-0.7.0/PKG-INFO
```

### Comparing `caikit-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.7.0/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/.github/workflows/build-library.yml` & `caikit-0.7.0/.github/workflows/lint-code.yml`

 * *Files 20% similar despite different names*

```diff
@@ -8,43 +8,36 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-name: Build Caikit Core Library
+name: Lint and Format
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
 jobs:
   build:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version:
-          - setup: '3.8'
-            tox: 'py38'
-          - setup: '3.9'
-            tox: 'py39'
-          - setup: '3.10'
-            tox: 'py310'
-          - setup: '3.11'
-            tox: 'py311'
-
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python ${{ matrix.python-version.setup }}
+      - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version.setup }}
+          python-version: 3.9
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install -r setup_requirements.txt
-      - name: Build and test with tox
-        run: tox -e ${{ matrix.python-version.tox }}
-
+      - name: Check Formatting
+        run: tox -e fmt
+      - name: Run pylint
+        run: tox -e lint
+      - name: Setup Graphviz # `graphviz/dot` is required for the import checker
+        uses: ts-graphviz/setup-graphviz@v1
+      - name: Enforce import rules
+        run: tox -e imports
```

### Comparing `caikit-0.6.0/.github/workflows/publish-library.yml` & `caikit-0.7.0/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/.pylintrc` & `caikit-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/CONTRIBUTING.md` & `caikit-0.7.0/CONTRIBUTING.md`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ```sh
 tox
 ```
 
 Running tests against a single Python version can be done with:
 
 ```sh
-tox -e 3.9
+tox -e py
 ```
 
 ### Coding style
 
 Caikit follows the python [pep8](https://peps.python.org/pep-0008/) coding style. The coding style is enforced by the CI system, and your PR will fail until the style has been applied correctly.
 
 We use [pre-commit](https://pre-commit.com/) to enforce coding style using [black](https://github.com/psf/black), [prettier](https://github.com/prettier/prettier) and [isort](https://pycqa.github.io/isort/).
```

### Comparing `caikit-0.6.0/LICENSE` & `caikit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/README.md` & `caikit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit-overview.png` & `caikit-0.7.0/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/config/__init__.py` & `caikit-0.7.0/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/config/config.py` & `caikit-0.7.0/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/config/config.yml` & `caikit-0.7.0/caikit/config/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -89,23 +89,19 @@
 
     # Number of workers with which we will run the gRPC server
     server_thread_pool_size: 5
     use_abortable_threads: true
     # gRPC Server shutdown grace period
     server_shutdown_grace_period_seconds: 45
 
-    compiled_proto_module_dir: unused
-
     # Configuration items for service generation
     service_generation:
-        enabled: true
         module_guids:
             included: []
             excluded: []
-        primitive_data_model_types: []
         task_types:
             included: []
             excluded: []
 
     # Configuration for batch inference. This dict contains entries for individual
     # model types and can be extended using additional overlay config files to add
     # sections for model types beyond those listed here. Each section should contain
```

### Comparing `caikit-0.6.0/caikit/core/__init__.py` & `caikit-0.7.0/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/__init__.py` & `caikit-0.7.0/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/base.py` & `caikit-0.7.0/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.7.0/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.7.0/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/schemes/base.py` & `caikit-0.7.0/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.7.0/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.7.0/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/__init__.py` & `caikit-0.7.0/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/base.py` & `caikit-0.7.0/caikit/core/data_model/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 """Base classes and functionality for all data structures.
 """
 
 # metaclass-generated field members cannot be detected by pylint
 # pylint: disable=no-member
 
 # Standard
+from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Optional, Type, Union
 import base64
 import json
 
 # Third Party
 from google.protobuf import json_format
@@ -32,15 +33,15 @@
 from google.protobuf.message import Message as ProtoMessageType
 
 # First Party
 import alog
 
 # Local
 from ..toolkit.errors import error_handler
-from . import enums
+from . import enums, json_dict
 
 log = alog.use_channel("DATAM")
 error = error_handler.get(log)
 
 
 class _DataBaseMetaClass(type):
     """Meta class for all structures in the data model."""
@@ -305,14 +306,19 @@
                 error(
                     "<COR66616239E>",
                     AttributeError(
                         f"{type(self)} missing attribute {field} and no backend set"
                     ),
                 )
             attr_val = backend.get_attribute(self.__class__, field)
+            if isinstance(attr_val, self.__class__.OneofFieldVal):
+                log.debug2("Got a OneofFieldVal from the backend")
+                assert field in self.__class__._fields_oneofs_map
+                self._get_which_oneof_dict()[field] = attr_val.which_oneof
+                attr_val = attr_val.val
 
             # If the backend says that this attribute should be cached, set it
             # as an attribute on the class
             if backend.cache_attribute(field, attr_val):
                 setattr(self, field, attr_val)
 
             # Return the value found by the backend
@@ -408,14 +414,23 @@
     """Base class for all structures in the data model.
 
     Notes:
         All leaves in the hierarchy of derived classes should have a corresponding protobufs class
         defined in the interface definitions.  If not, an exception will be thrown at runtime.
     """
 
+    @dataclass
+    class OneofFieldVal:
+        """Helper struct that backends can use to return information about
+        values in oneofs along with which of the oneofs is currently valid
+        """
+
+        val: Any
+        which_oneof: str
+
     def __setattr__(self, name, val):
         """Handle attribute setting for oneofs and named fields with delegation
         to backends as needed
         """
         # If setting a oneof directly, remove any oneof information
         cls = self.__class__
         if name in cls._fields_oneofs_map:
@@ -479,14 +494,21 @@
         which_oneof = self._get_which_oneof_dict()
         if current_val := which_oneof.get(oneof_name):
             return current_val
 
         # Get the current value for the oneof and introspect which field its
         # type matches
         oneof_val = getattr(self, oneof_name)
+
+        # Re-check in case the getattr pulled a OneofFieldVal that populated the
+        # which_oneof dict with knowledge from the backend
+        if current_val := which_oneof.get(oneof_name):
+            return current_val
+
+        # Try to figure out the field based on the type
         which_field = self._infer_which_oneof(oneof_name, oneof_val)
         if which_field is not None:
             which_oneof[oneof_name] = which_field
         return which_field
 
     @classmethod
     def _infer_which_oneof(cls, oneof_name: str, oneof_val: Any) -> Optional[str]:
@@ -614,17 +636,20 @@
                         kwargs[field][key] = contained_class.from_proto(value)
                     # If it's not a message, the value can be left alone, i.e., it's a primitive
                     else:
                         kwargs[field][key] = value
 
             elif field in cls._fields_message:
                 if proto.HasField(field):
-                    contained_class = cls.get_class_for_proto(proto_attr)
-                    contained_obj = contained_class.from_proto(proto_attr)
-                    kwargs[field] = contained_obj
+                    if proto_attr.DESCRIPTOR.full_name == "google.protobuf.Struct":
+                        kwargs[field] = json_dict.struct_to_dict(proto_attr)
+                    else:
+                        contained_class = cls.get_class_for_proto(proto_attr)
+                        contained_obj = contained_class.from_proto(proto_attr)
+                        kwargs[field] = contained_obj
 
             elif field in cls._fields_message_repeated:
                 elements = []
                 contained_class = None
                 for item in proto_attr:
                     if contained_class is None:
                         contained_class = cls.get_class_for_proto(item)
@@ -748,15 +773,20 @@
                 or field in self._fields_enum_repeated
             ):
                 subproto = getattr(proto, field)
                 subproto.extend(attr)
 
             elif field in self._fields_message:
                 subproto = getattr(proto, field)
-                attr.fill_proto(subproto)
+                if subproto.DESCRIPTOR.full_name == "google.protobuf.Struct":
+                    subproto.CopyFrom(
+                        json_dict.dict_to_struct(attr, subproto.__class__)
+                    )
+                else:
+                    attr.fill_proto(subproto)
 
             elif field in self._fields_message_repeated:
                 subproto = getattr(proto, field)
                 for item in attr:
                     item.fill_proto(subproto.add())
 
             else:
```

### Comparing `caikit-0.6.0/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.7.0/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/data_backends/base.py` & `caikit-0.7.0/caikit/core/data_model/data_backends/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,39 +12,47 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 """The base class for data model object backends"""
 
 # Standard
-from typing import Any, Type
+from typing import Any, Type, Union
 import abc
 
+# Local
+from ..base import DataBase
+
 # DataModelBackendBase #########################################################
 
 
 class DataModelBackendBase(abc.ABC):
     """A base interface class for accessing data from within a given backend
     data layout
     """
 
     @abc.abstractmethod
-    def get_attribute(self, data_model_class: Type["DataBase"], name: str) -> Any:
+    def get_attribute(
+        self,
+        data_model_class: Type[DataBase],
+        name: str,
+    ) -> Union[Any, DataBase.OneofFieldVal]:
         """A data model backend must implement this in order to provide the
         frontend view the functionality needed to lazily extract data.
 
         Args:
             data_model_class:  Type[DataBase]
                 The frontend data model class that is accessing this attribute
             name:  str
                 The name of the attribute to access
 
         Returns:
-            value:  Any
-                The extracted attribute value
+            value:  Union[Any, OneofFieldVal]
+                The extracted attribute value or a OneofFieldVal that wraps the
+                field val with an indicator about the oneof field that is set.
         """
 
     # pylint: disable=unused-argument
     def cache_attribute(self, name: str, value: Any) -> bool:
         """Determine whether or not to cache the given attribute's result on the
         wrapping data model object.
```

### Comparing `caikit-0.6.0/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.7.0/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -99,8 +99,25 @@
             error.type_check("<COR85037213E>", Iterable, **{name: raw_value})
             field_dm_class = data_model_class.get_field_message_type(name)
             return [
                 field_dm_class.from_backend(self.__class__(entry))
                 for entry in raw_value
             ]
 
+        # If the target attribure is a oneof name, look for the oneof name in the data dict first.
+        # If it exists, infer the right field name based on the type of the value and return the
+        # field name and the value. If oneof name isn't in the data dict, check for field name
+        # instead and return the right value
+        if name in data_model_class._fields_oneofs_map:
+            if name in self._data_dict:
+                val = self._data_dict[name]
+                which_oneof = data_model_class._infer_which_oneof(name, val)
+                return data_model_class.OneofFieldVal(val=val, which_oneof=which_oneof)
+
+            oneof_fields = data_model_class._fields_oneofs_map[name]
+            for field in oneof_fields:
+                if field in self._data_dict:
+                    return data_model_class.OneofFieldVal(
+                        val=self._data_dict[field], which_oneof=field
+                    )
+
         return raw_value
```

### Comparing `caikit-0.6.0/caikit/core/data_model/dataobject.py` & `caikit-0.7.0/caikit/core/data_model/dataobject.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,32 +21,46 @@
 from enum import Enum
 from typing import Any, Callable, List, Type, Union, get_args, get_origin
 import dataclasses
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
+from google.protobuf import struct_pb2
 from google.protobuf.internal.enum_type_wrapper import EnumTypeWrapper
 import numpy as np
 
 # First Party
 from py_to_proto.dataclass_to_proto import PY_TO_PROTO_TYPES, DataclassConverter
 import alog
 import py_to_proto
 
 # Local
 from ..toolkit.errors import error_handler
 from . import enums
 from .base import DataBase, _DataBaseMetaClass
+from .json_dict import JsonDict
 
 ## Globals #####################################################################
 
 log = alog.use_channel("SCHEMA")
 error = error_handler.get(log)
 
+# Type mapping for type hints in @dataobject classes
+DATAOBJECT_PY_TO_PROTO_TYPES = {
+    JsonDict: struct_pb2.Struct,
+    np.int32: _descriptor.FieldDescriptor.TYPE_INT32,
+    np.int64: _descriptor.FieldDescriptor.TYPE_INT64,
+    np.uint32: _descriptor.FieldDescriptor.TYPE_UINT32,
+    np.uint64: _descriptor.FieldDescriptor.TYPE_UINT64,
+    np.float32: _descriptor.FieldDescriptor.TYPE_FLOAT,
+    np.float64: _descriptor.FieldDescriptor.TYPE_DOUBLE,
+    **PY_TO_PROTO_TYPES,
+}
+
 # Common package prefix
 CAIKIT_DATA_MODEL = "caikit_data_model"
 
 # Registry of auto-generated protos so that they can be rendered to .proto
 _AUTO_GEN_PROTO_CLASSES = []
 
 # Special attribute used to indicate which defaults are user provided
@@ -202,24 +216,14 @@
     """
     for proto_class in _AUTO_GEN_PROTO_CLASSES:
         proto_class.write_proto_file(interfaces_dir)
 
 
 ## Implementation Details ######################################################
 
-DATAOBJECT_PY_TO_PROTO_TYPES = {
-    np.int32: _descriptor.FieldDescriptor.TYPE_INT32,
-    np.int64: _descriptor.FieldDescriptor.TYPE_INT64,
-    np.uint32: _descriptor.FieldDescriptor.TYPE_UINT32,
-    np.uint64: _descriptor.FieldDescriptor.TYPE_UINT64,
-    np.float32: _descriptor.FieldDescriptor.TYPE_FLOAT,
-    np.float64: _descriptor.FieldDescriptor.TYPE_DOUBLE,
-    **PY_TO_PROTO_TYPES,
-}
-
 
 def _dataobject_to_proto(*args, **kwargs):
     kwargs.setdefault("type_mapping", DATAOBJECT_PY_TO_PROTO_TYPES)
     return _DataobjectConverter(*args, **kwargs).descriptor
 
 
 class _DataobjectConverter(DataclassConverter):
```

### Comparing `caikit-0.6.0/caikit/core/data_model/enums.py` & `caikit-0.7.0/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/producer.py` & `caikit-0.7.0/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.7.0/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/__init__.py` & `caikit-0.7.0/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/converter.py` & `caikit-0.7.0/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.7.0/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/data_stream.py` & `caikit-0.7.0/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/resolver.py` & `caikit-0.7.0/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/data_model/streams/validator.py` & `caikit-0.7.0/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/model_manager.py` & `caikit-0.7.0/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/module_backends/__init__.py` & `caikit-0.7.0/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/module_backends/backend_types.py` & `caikit-0.7.0/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/module_backends/base.py` & `caikit-0.7.0/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/module_backends/local_backend.py` & `caikit-0.7.0/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/module_backends/module_backend_config.py` & `caikit-0.7.0/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/__init__.py` & `caikit-0.7.0/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/base.py` & `caikit-0.7.0/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/config.py` & `caikit-0.7.0/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/decorator.py` & `caikit-0.7.0/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/loader.py` & `caikit-0.7.0/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/meta.py` & `caikit-0.7.0/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/modules/saver.py` & `caikit-0.7.0/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/registries.py` & `caikit-0.7.0/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/signature_parsing/__init__.py` & `caikit-0.7.0/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/signature_parsing/docstrings.py` & `caikit-0.7.0/caikit/core/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/signature_parsing/module_signature.py` & `caikit-0.7.0/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/signature_parsing/parsers.py` & `caikit-0.7.0/caikit/core/signature_parsing/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,19 +61,29 @@
     # Check the docstring
     type_from_docstring = docstrings.get_return_type(fn)
 
     if type_from_docstring:
         return type_from_docstring
 
     # If we get here, it means no annotation or docstring for type was provided
-    log.warning(
-        "Could not deduct output type from function %s for module class %s.",
-        fn_signature,
-        module_class.__name__,
-    )
+
+    # Warn unless this was a base function (e.g., don't warn if there is no train() override)
+    if fn.__module__ != ModuleBase.__module__:
+        log.warning(
+            "Could not deduct output type from function %s for module class %s.",
+            fn.__name__,
+            module_class.__name__,
+        )
+    else:
+        log.debug(
+            "Could not deduct output type from function %s for module class %s using %s.",
+            fn.__name__,
+            module_class.__name__,
+            fn.__qualname__,
+        )
 
 
 def get_argument_types(module_method: Callable) -> Dict[str, Type]:
     """Get the python types for each parameter to this method, returned in a dict.
     This does more than simply looking at inspect.Signature, see _get_argument_type
 
     Args:
```

### Comparing `caikit-0.6.0/caikit/core/task.py` & `caikit-0.7.0/caikit/core/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,26 @@
                         {parameter_type} is required"
                 )
         if type_mismatch_errors:
             raise TypeError(
                 f"Wrong types provided for parameters to {signature.module}: {type_mismatch_errors}"
             )
 
+        if signature.return_type != cls.get_output_type():
+            # Wrong return type: Just check to make sure it's not
+            # `Union[expected_type, other_types]`
+            if typing.get_origin(signature.return_type) != Union or (
+                typing.get_origin(signature.return_type) == Union
+                and cls.get_output_type() not in typing.get_args(signature.return_type)
+            ):
+                raise TypeError(
+                    f"Wrong output type for module {signature.module}: "
+                    f"Found {signature.return_type} but expected {cls.get_output_type()}"
+                )
+
     @classmethod
     def get_required_parameters(cls) -> Dict[str, ValidInputTypes]:
         """Get the set of input types required by this task
 
         NOTE: This method is automatically configured by the @task decorator
             and should not be overwritten by child classes.
         """
```

### Comparing `caikit-0.6.0/caikit/core/toolkit/__init__.py` & `caikit-0.7.0/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/compatibility.py` & `caikit-0.7.0/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/errors/__init__.py` & `caikit-0.7.0/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.7.0/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.7.0/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/fileio.py` & `caikit-0.7.0/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/isa.py` & `caikit-0.7.0/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/logging.py` & `caikit-0.7.0/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.7.0/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/serializers.py` & `caikit-0.7.0/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/core/toolkit/wip_decorator.py` & `caikit-0.7.0/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/__init__.py` & `caikit-0.7.0/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/common/__init__.py` & `caikit-0.7.0/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.7.0/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/common/data_model/producer.py` & `caikit-0.7.0/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/runtime/__init__.py` & `caikit-0.7.0/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.7.0/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.7.0/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/__init__.py` & `caikit-0.7.0/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/dump_services.py` & `caikit-0.7.0/caikit/runtime/dump_services.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,23 +23,20 @@
 
 def dump_services(output_dir: str):
     """
     Utility for rendering the all generated interfaces to proto files
     """
     inf_svc = ServicePackageFactory.get_service_package(
         ServicePackageFactory.ServiceType.INFERENCE,
-        ServicePackageFactory.ServiceSource.GENERATED,
     )
     train_svc = ServicePackageFactory.get_service_package(
         ServicePackageFactory.ServiceType.TRAINING,
-        ServicePackageFactory.ServiceSource.GENERATED,
     )
     train_mgt_svc = ServicePackageFactory.get_service_package(
         ServicePackageFactory.ServiceType.TRAINING_MANAGEMENT,
-        ServicePackageFactory.ServiceSource.GENERATED,
     )
 
     render_dataobject_protos(output_dir)
     inf_svc.service.write_proto_file(output_dir)
     train_svc.service.write_proto_file(output_dir)
     train_mgt_svc.service.write_proto_file(output_dir)
```

### Comparing `caikit-0.6.0/caikit/runtime/grpc_server.py` & `caikit-0.7.0/caikit/runtime/grpc_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,29 +17,34 @@
 from typing import Optional, Union
 import os
 import signal
 import socket
 
 # Third Party
 from grpc_health.v1 import health, health_pb2_grpc
+from grpc_reflection.v1alpha import reflection
 from prometheus_client import start_http_server
 from py_grpc_prometheus.prometheus_server_interceptor import PromServerInterceptor
 import grpc
 
 # First Party
 import aconfig
 import alog
 
 # Local
 # Get the injectable servicer class definitions
 from caikit import get_config
 from caikit.runtime.interceptors.caikit_runtime_server_wrapper import (
     CaikitRuntimeServerWrapper,
 )
-from caikit.runtime.protobufs import model_runtime_pb2_grpc, process_pb2_grpc
+from caikit.runtime.protobufs import (
+    model_runtime_pb2,
+    model_runtime_pb2_grpc,
+    process_pb2_grpc,
+)
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.servicers.model_runtime_servicer import ModelRuntimeServicerImpl
 from caikit.runtime.servicers.model_train_servicer import ModelTrainServicerImpl
 from caikit.runtime.servicers.training_management_servicer import (
     TrainingManagementServicerImpl,
@@ -84,37 +89,40 @@
         self.server = grpc.server(
             futures.ThreadPoolExecutor(
                 max_workers=self.config.runtime.server_thread_pool_size
             ),
             interceptors=(PROMETHEUS_METRICS_INTERCEPTOR,),
         )
 
+        # Start tracking service names for reflection
+        service_names = [reflection.SERVICE_NAME]
+
         # Intercept an Inference Service
         self._global_predict_servicer = GlobalPredictServicer(self.inference_service)
         self.server = CaikitRuntimeServerWrapper(
             server=self.server,
             global_predict=self._global_predict_servicer.Predict,
             intercepted_svc_descriptor=self.inference_service.descriptor,
-            excluded_methods=["/natural_language_understanding.CaikitRuntime/Echo"],
         )
+        service_names.append(self.inference_service.descriptor.full_name)
 
         # Register inference service
         self.inference_service.registration_function(
             self.inference_service.service, self.server
         )
 
         # And intercept a training service, if we have one
         if self.training_service:
             global_train_servicer = GlobalTrainServicer(self.training_service)
             self.server = CaikitRuntimeServerWrapper(
                 server=self.server,
                 global_predict=global_train_servicer.Train,
                 intercepted_svc_descriptor=self.training_service.descriptor,
-                excluded_methods=None,
             )
+            service_names.append(self.training_service.descriptor.full_name)
 
             # Register training service
             self.training_service.registration_function(
                 self.training_service.service, self.server
             )
 
             # Add model train servicer to the gRPC server
@@ -122,35 +130,41 @@
                 ModelTrainServicerImpl(self.training_service), self.server
             )
 
             # Add training management servicer to the gRPC server
             training_management_service: ServicePackage = (
                 ServicePackageFactory.get_service_package(
                     ServicePackageFactory.ServiceType.TRAINING_MANAGEMENT,
-                    ServicePackageFactory.ServiceSource.GENERATED,
                 )
             )
+            service_names.append(training_management_service.descriptor.full_name)
 
             training_management_service.registration_function(
                 TrainingManagementServicerImpl(), self.server
             )
 
         # Add model runtime servicer to the gRPC server
         model_runtime_pb2_grpc.add_ModelRuntimeServicer_to_server(
             ModelRuntimeServicerImpl(), self.server
         )
+        service_names.append(
+            model_runtime_pb2.DESCRIPTOR.services_by_name["ModelRuntime"].full_name
+        )
 
         # Add gRPC default health servicer.
         # We use the non-blocking implementation to avoid thread starvation.
         health_servicer = health.HealthServicer(
             experimental_non_blocking=True,
             experimental_thread_pool=futures.ThreadPoolExecutor(max_workers=1),
         )
         health_pb2_grpc.add_HealthServicer_to_server(health_servicer, self.server)
 
+        # Finally enable service reflection after all services are added
+        reflection.enable_server_reflection(service_names, self.server)
+
         # Listen on a unix socket as well for model mesh.
         if self.config.runtime.unix_socket_path and os.path.exists(
             self.config.runtime.unix_socket_path
         ):
             try:
                 self.server.add_insecure_port(
                     f"unix://{self.config.runtime.unix_socket_path}"
@@ -331,35 +345,25 @@
     # Start serving Prometheus metrics
     caikit_config = get_config()
     start_http_server(caikit_config.runtime.metrics.port)
 
     # Enable signal handling
     handle_terminations = True
 
-    # Assume we want compiled services for now
-    service_source = (
-        ServicePackageFactory.ServiceSource.GENERATED
-        if caikit_config.runtime.service_generation.enabled
-        else ServicePackageFactory.ServiceSource.COMPILED
-    )
-    log.debug("Running with service source: %s", service_source)
-
     # We should always be able to stand up an inference service
     inference_service: ServicePackage = ServicePackageFactory.get_service_package(
         ServicePackageFactory.ServiceType.INFERENCE,
-        service_source,
     )
 
     # But maybe not always a training service
     try:
         training_service: Optional[
             ServicePackage
         ] = ServicePackageFactory.get_service_package(
             ServicePackageFactory.ServiceType.TRAINING,
-            service_source,
         )
     except CaikitRuntimeException as e:
         log.warning("Cannot stand up training service, disabling training: %s", e)
         training_service = None
 
     server = RuntimeGRPCServer(
         inference_service=inference_service,
```

### Comparing `caikit-0.6.0/caikit/runtime/interceptors/__init__.py` & `caikit-0.7.0/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.7.0/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Standard
 import traceback
 
 # Third Party
+from grpc._utilities import RpcMethodHandler
 from prometheus_client import Gauge
 import grpc
 
 # First Party
 import alog
 
 # Local
@@ -38,54 +39,37 @@
     """This class wraps an underlying gRPC server for the purpose of
     intercepting the binding of servicers (e.g., the CaikitRuntimeServicer) to
     the server so that the RPC handlers that are registered to the server
     can optionally be replaced with a generic global predict RPC handler
     instead.
     """
 
-    def __init__(
-        self, server, global_predict, intercepted_svc_descriptor, excluded_methods
-    ):
+    def __init__(self, server, global_predict, intercepted_svc_descriptor):
         """Initialize a new CaikitRuntimeServerWrapper
 
         Args:
             server(grpc.Server): The server that is being wrapped
             global_predict(function): A function that will accept an arbitrary
                 gRPC request message and a grpc.ServicerContext, and return
                 a suitable gRPC response message
-            excluded_methods(list(string)): An optional list of fully-qualified
-                RPC methods to avoid intercepting (e.g.,
-                ['/natural_language_understanding.CaikitRuntime/Echo'])
         """
 
-        if not excluded_methods:
-            excluded_methods = []
-
         self._server = server
         self._global_predict = global_predict
         self._intercepted_svc_descriptor = intercepted_svc_descriptor
         self._intercepted_svc_name = self._intercepted_svc_descriptor.full_name
         self._intercepted_methods = []
-        self._unintercepted_methods = []
 
         for method in self._intercepted_svc_descriptor.methods:
             # Take the method short name (e.g., 'SyntaxIzumoPredict') and
             # concatenate it with the intercepted service name to produce
             # a fully qualified RPC method name that we wish to intercept
             # (e.g., '/natural_language_understanding.CaikitRuntime/SyntaxIzumoPredict')
             fqm = "/%s/%s" % (self._intercepted_svc_name, method.name)
 
-            if fqm in excluded_methods:
-                # We do not want to intercept this particular RPC
-                log.info(
-                    "<RUN59920454I>", "Bypassing interception of RPC method %s", fqm
-                )
-                self._unintercepted_methods.append((method.name, fqm))
-                continue
-
             log.info("<RUN81194024I>", "Intercepting RPC method %s", fqm)
             self._intercepted_methods.append((method.name, fqm))
 
     # **************************************************************************
     # Custom methods
     # **************************************************************************
 
@@ -107,51 +91,40 @@
                 A list of two-element tuples containing the short name (e.g.,
                 'SyntaxIzumoPredict') and fully-qualified name (e.g.,
                 '/natural_language_understanding.CaikitRuntime/SyntaxIzumoPredict')
                 of every RPC method intercepted by this server wrapper
         """
         return self._intercepted_methods
 
-    def unintercepted_methods(self):
-        """Get the list of un-intercepted (i.e., excluded) predict RPC methods
-
-        Returns:
-            list((string, string)):
-                A list of two-element tuples containing the short name (e.g.,
-                'Echo') and fully-qualified name (e.g.,
-                '/natural_language_understanding.CaikitRuntime/Echo')
-                of every RPC method *not* intercepted by this server wrapper
-        """
-        return self._unintercepted_methods
-
     @staticmethod
     def safe_rpc_wrapper(rpc):
         """This wrapper should be used to safely invoke an RPC. If used, it adds automatic error
         handling and conversion to the appropriate response for gRPC, as well as logging indicating
         if the the error was intentional (i.e., thrown as CaikitRuntimeException directly) or
         unexpected (i.e., thrown as a non GRPC error).
 
         Args:
             rpc(Function): Method attached to a servicer instance to be invoked in a safe manner.
 
         Returns:
             A function that takes a gRPC request message and ServicerContext, and safely invokes
             the provided RPC.
         """
-
-        if rpc is not None:
-            if rpc.__name__ == "safe_rpc_call":
-                return rpc
-            log.info(
-                "<RUN33333123I>",
-                "Wrapping safe rpc for %s",
-                rpc.__name__,
-            )
-        else:
-            log.info("<RUN33322123I>", "Wrapping safe rpc for %s", rpc)
+        if rpc is None:
+            message = "Programming error, RPC is None!"
+            log.error("<RUN33322123E>", message)
+            raise CaikitRuntimeException(grpc.StatusCode.INTERNAL, message)
+
+        if rpc.__name__ == "safe_rpc_call":
+            return rpc
+        log.info(
+            "<RUN33333123I>",
+            "Wrapping safe rpc for %s",
+            rpc.__name__,
+        )
 
         def safe_rpc_call(request, context):
             """This function should be used to safely invoke an RPC. If used, it adds automatic
             error handling and conversion to the appropriate response for gRPC, as well as logging
             indicating if the the error was intentional (i.e., thrown as CaikitRuntimeException
             directly) or unexpected (i.e., thrown as a non GRPC error).
 
@@ -221,77 +194,87 @@
                     # Make sure this is a unary-unary RPC
                     if not original_rpc_handler.unary_unary:
                         raise NotImplementedError("Unary-unary RPCs only!")
 
                     # Now, swap out the original unary-unary callable with our
                     # generic predict method, and add this newly re-routed RPC
                     # method handler to the dict of (method, handler) pairs
-                    rerouted_rpc_method_handlers[
-                        method
-                    ] = grpc.unary_unary_rpc_method_handler(
-                        self.safe_rpc_wrapper(self._global_predict),
-                        request_deserializer=original_rpc_handler.request_deserializer,
-                        response_serializer=original_rpc_handler.response_serializer,
-                    )
+                    safe_rpc_handler = self._make_new_handler(original_rpc_handler)
+                    rerouted_rpc_method_handlers[method] = safe_rpc_handler
                     log.info(
                         "<RUN30032825I>",
                         "Re-routing RPC %s from %s to %s",
                         fqm,
                         original_rpc_handler.unary_unary,
                         rerouted_rpc_method_handlers[method].unary_unary,
                     )
 
-                unintercepted_rpc_method_handlers = {}
-                for method, fqm in self.unintercepted_methods():
-                    # For the collection of predict RPCs that we explicitly
-                    # do *not* wish to intercept, we will use the original
-                    # unary-unary RPC handler method, but will wrap it in a
-                    # safe RPC call
-                    original_rpc_handler = handler.service(DummyHandlerCallDetails(fqm))
-                    unintercepted_rpc_method_handlers[
-                        method
-                    ] = grpc.unary_unary_rpc_method_handler(
-                        self.safe_rpc_wrapper(original_rpc_handler.unary_unary),
-                        request_deserializer=original_rpc_handler.request_deserializer,
-                        response_serializer=original_rpc_handler.response_serializer,
-                    )
-
-                # Now that we have re-rerouted all of the original RPC method
+                # Now that we have re-rerouted all the original RPC method
                 # handlers to the global predict RPC method handler, it is time
                 # to bind them to the underlying server that we are wrapping
-                all_rpc_handlers = dict(
-                    rerouted_rpc_method_handlers, **unintercepted_rpc_method_handlers
-                )
                 generic_handler = grpc.method_handlers_generic_handler(
-                    self.intercepted_service(), all_rpc_handlers
+                    self.intercepted_service(), rerouted_rpc_method_handlers
                 )
                 self._server.add_generic_rpc_handlers((generic_handler,))
                 log.info(
                     "<RUN24924908I>",
                     "Interception of service %s complete",
                     self.intercepted_service(),
                 )
 
             else:
                 # This is not the service whose RPC handlers we wish to
                 # intercept, so just pass the (unmodified) RPC handlers
                 # along to the underlying gRPC server we are wrapping
                 assert isinstance(handler, grpc._utilities.DictionaryGenericHandler)
                 for method in handler._method_handlers:
-                    # Wrap the RPC handler for this method in a safe RPC call
+                    # Wrap the RPC handler for this method in a safe RPC call,
+                    # but do not replace the handler with a global handler
                     original_rpc_handler = handler._method_handlers[method]
-                    safe_rpc_handler = grpc.unary_unary_rpc_method_handler(
-                        self.safe_rpc_wrapper(original_rpc_handler.unary_unary),
-                        request_deserializer=original_rpc_handler.request_deserializer,
-                        response_serializer=original_rpc_handler.response_serializer,
+                    safe_rpc_handler = self._make_new_handler(
+                        original_rpc_handler, replace_with_global_predict=False
                     )
                     handler._method_handlers[method] = safe_rpc_handler
 
                 self._server.add_generic_rpc_handlers(generic_rpc_handlers)
 
+    def _make_new_handler(
+        self,
+        original_rpc_handler: RpcMethodHandler,
+        replace_with_global_predict: bool = True,
+    ):
+        if original_rpc_handler.unary_unary:
+            return grpc.unary_unary_rpc_method_handler(
+                self.safe_rpc_wrapper(
+                    self._global_predict
+                    if replace_with_global_predict
+                    else original_rpc_handler.unary_unary
+                ),
+                request_deserializer=original_rpc_handler.request_deserializer,
+                response_serializer=original_rpc_handler.response_serializer,
+            )
+        if original_rpc_handler.unary_stream:
+            return grpc.unary_stream_rpc_method_handler(
+                self.safe_rpc_wrapper(original_rpc_handler.unary_stream),
+                request_deserializer=original_rpc_handler.request_deserializer,
+                response_serializer=original_rpc_handler.response_serializer,
+            )
+        if original_rpc_handler.stream_unary:
+            return grpc.stream_unary_rpc_method_handler(
+                self.safe_rpc_wrapper(original_rpc_handler.stream_unary),
+                request_deserializer=original_rpc_handler.request_deserializer,
+                response_serializer=original_rpc_handler.response_serializer,
+            )
+        # Else, it's stream-stream
+        return grpc.stream_stream_rpc_method_handler(
+            self.safe_rpc_wrapper(original_rpc_handler.stream_stream),
+            request_deserializer=original_rpc_handler.request_deserializer,
+            response_serializer=original_rpc_handler.response_serializer,
+        )
+
     # **************************************************************************
     # Pass-through (i.e., unchanged) grpc.Server methods
     # **************************************************************************
 
     def add_insecure_port(self, address):
         """Opens an insecure port for accepting RPCs.
```

### Comparing `caikit-0.6.0/caikit/runtime/metrics/__init__.py` & `caikit-0.7.0/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.7.0/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/__init__.py` & `caikit-0.7.0/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/batcher.py` & `caikit-0.7.0/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/loaded_model.py` & `caikit-0.7.0/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/model_loader.py` & `caikit-0.7.0/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/model_manager.py` & `caikit-0.7.0/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/model_sizer.py` & `caikit-0.7.0/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/model_management/training_manager.py` & `caikit-0.7.0/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/__init__.py` & `caikit-0.7.0/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.7.0/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.7.0/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.7.0/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.7.0/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.7.0/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.7.0/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.7.0/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/service_factory.py` & `caikit-0.7.0/caikit/runtime/service_factory.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 """This module is responsible for creating service objects for the runtime to consume"""
 # Standard
 from enum import Enum
 from types import ModuleType
 from typing import Callable, Set, Type
 import dataclasses
-import inspect
 
 # Third Party
 import google.protobuf.descriptor
 import google.protobuf.service
 import grpc
 
 # First Party
@@ -33,15 +32,14 @@
 from caikit import get_config
 from caikit.core import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
-from caikit.runtime.service_generation.core_module_helpers import get_module_info
 from caikit.runtime.service_generation.rpcs import snake_to_upper_camel
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils import import_util
 import caikit.core
 
 log = alog.use_channel("SVC-FACTORY")
 
@@ -82,86 +80,28 @@
     """Factory responsible for yielding the correct concrete ServicePackage implementation"""
 
     class ServiceType(Enum):
         INFERENCE = 1  # Inference service for the GlobalPredictServicer
         TRAINING = 2  # Training service for the GlobalTrainServicer
         TRAINING_MANAGEMENT = 3
 
-    class ServiceSource(Enum):
-        COMPILED = 1  # Pull from a protoc-compiled _pb2 module
-        GENERATED = 2  # Generate a service definition by inspecting the library's APIs
-
     @classmethod
-    def get_service_package(
-        cls,
-        service_type: ServiceType,
-        source: ServiceSource,
-    ) -> ServicePackage:
+    def get_service_package(cls, service_type: ServiceType) -> ServicePackage:
         """Public factory API. Returns a service package of the requested type, from the
         configured source.
 
         Args:
             service_type (ServicePackageFactory.ServiceType): The type of service to build,
                 to match the servicer implementation that will handle it. e.g. the
                 GlobalPredictServicer expects an "INFERENCE" service
-            source (ServicePackageFactory.ServiceSource): Describes where the service artifacts
-                should be pulled from or how they should be constructed
 
         Returns:
             ServicePackage: A container with properties referencing everything you need to bind a
                 concrete Servicer implementation to a protobufs Service and grpc Server
         """
-        if source == cls.ServiceSource.COMPILED:
-            # Use our import_utils to extract the correct bits out of a set of compiled pb2
-            # packages
-            lib_name = cls._get_lib_name_for_servicer()
-
-            if service_type == cls.ServiceType.INFERENCE:
-                # 🌶️🌶️🌶️! hardcoded service names
-                compiled_pb2_package = cls._get_compiled_proto_module(
-                    "caikit_runtime_pb2"
-                )
-                compiled_pb2_grpc_package = cls._get_compiled_proto_module(
-                    "caikit_runtime_pb2_grpc"
-                )
-            elif service_type == cls.ServiceType.TRAINING_MANAGEMENT:
-                raise CaikitRuntimeException(
-                    grpc.StatusCode.INTERNAL,
-                    "Not allowed to get Training Management services from compiled packages",
-                )
-            else:  # elif  service_type == cls.ServiceType.TRAINING:
-                # (using final _else_ for static analysis happiness)
-                # 🌶️🌶️🌶️! hardcoded service names
-                compiled_pb2_package = cls._get_compiled_proto_module(
-                    "caikit_runtime_train_pb2"
-                )
-                compiled_pb2_grpc_package = cls._get_compiled_proto_module(
-                    "caikit_runtime_train_pb2_grpc"
-                )
-
-            # Dynamically create a new module to hold all the service's messages
-            client_module = ModuleType(
-                "ClientMessages", "Package with service message class implementations"
-            )
-            for k, v in compiled_pb2_package.__dict__.items():
-                if inspect.isclass(v) and issubclass(
-                    v, google.protobuf.message.Message
-                ):
-                    setattr(client_module, k, v)
-
-            return ServicePackage(
-                service=cls._get_servicer_class(compiled_pb2_grpc_package, lib_name),
-                descriptor=cls._get_service_descriptor(compiled_pb2_package, lib_name),
-                registration_function=cls._get_servicer_function(
-                    compiled_pb2_grpc_package, lib_name
-                ),
-                stub_class=cls._get_servicer_stub(compiled_pb2_grpc_package, lib_name),
-                messages=client_module,
-            )
-
         if service_type == cls.ServiceType.TRAINING_MANAGEMENT:
             grpc_service = json_to_service(
                 name=TRAINING_MANAGEMENT_SERVICE_NAME,
                 package="caikit.runtime.training",
                 json_service_def=TRAINING_MANAGEMENT_SERVICE_SPEC,
             )
 
@@ -169,66 +109,63 @@
                 service=grpc_service.service_class,
                 descriptor=grpc_service.descriptor,
                 registration_function=grpc_service.registration_function,
                 stub_class=grpc_service.client_stub_class,
                 messages=None,  # we don't need messages here
             )
 
-        if source == cls.ServiceSource.GENERATED:
-            # First make sure we import the data model for the correct library
-            # !!!! This will use the `caikit_library` config
-            _ = import_util.get_data_model()
-
-            caikit_config = get_config()
-            lib = caikit_config.runtime.library
-            ai_domain_name = snake_to_upper_camel(lib.replace("caikit_", ""))
-            package_name = f"caikit.runtime.{ai_domain_name}"
-
-            # Then do API introspection to come up with all the API definitions to support
-            clean_modules = ServicePackageFactory._get_and_filter_modules(
-                caikit_config, lib
-            )
+        # First make sure we import the data model for the correct library
+        # !!!! This will use the `caikit_library` config
+        _ = import_util.get_data_model()
+
+        caikit_config = get_config()
+        lib = caikit_config.runtime.library
+        ai_domain_name = snake_to_upper_camel(lib.replace("caikit_", ""))
+        package_name = f"caikit.runtime.{ai_domain_name}"
+
+        # Then do API introspection to come up with all the API definitions to support
+        clean_modules = ServicePackageFactory._get_and_filter_modules(
+            caikit_config, lib
+        )
 
-            if service_type == cls.ServiceType.INFERENCE:
-                task_rpc_list = service_generation.create_inference_rpcs(clean_modules)
-                service_name = f"{ai_domain_name}Service"
-            else:  # service_type == cls.ServiceType.TRAINING
-                task_rpc_list = service_generation.create_training_rpcs(clean_modules)
-                service_name = f"{ai_domain_name}TrainingService"
-
-            task_rpc_list = [
-                rpc for rpc in task_rpc_list if rpc.return_type is not None
-            ]
-
-            request_data_models = [
-                rpc.create_request_data_model(package_name) for rpc in task_rpc_list
-            ]
-
-            client_module = ModuleType(
-                "ClientMessages",
-                "Package with service message class implementations",
-            )
+        if service_type == cls.ServiceType.INFERENCE:
+            task_rpc_list = service_generation.create_inference_rpcs(clean_modules)
+            service_name = f"{ai_domain_name}Service"
+        else:  # service_type == cls.ServiceType.TRAINING
+            task_rpc_list = service_generation.create_training_rpcs(clean_modules)
+            service_name = f"{ai_domain_name}TrainingService"
 
-            for dm_class in request_data_models:
-                # We need the message class that data model serializes to
-                setattr(client_module, dm_class.__name__, type(dm_class().to_proto()))
+        task_rpc_list = [rpc for rpc in task_rpc_list if rpc.return_type is not None]
 
-            rpc_jsons = [rpc.create_rpc_json(package_name) for rpc in task_rpc_list]
-            service_json = {"service": {"rpcs": rpc_jsons}}
-            grpc_service = json_to_service(
-                name=service_name, package=package_name, json_service_def=service_json
-            )
+        request_data_models = [
+            rpc.create_request_data_model(package_name) for rpc in task_rpc_list
+        ]
 
-            return ServicePackage(
-                service=grpc_service.service_class,
-                descriptor=grpc_service.descriptor,
-                registration_function=grpc_service.registration_function,
-                stub_class=grpc_service.client_stub_class,
-                messages=client_module,
-            )
+        client_module = ModuleType(
+            "ClientMessages",
+            "Package with service message class implementations",
+        )
+
+        for dm_class in request_data_models:
+            # We need the message class that data model serializes to
+            setattr(client_module, dm_class.__name__, type(dm_class().to_proto()))
+
+        rpc_jsons = [rpc.create_rpc_json(package_name) for rpc in task_rpc_list]
+        service_json = {"service": {"rpcs": rpc_jsons}}
+        grpc_service = json_to_service(
+            name=service_name, package=package_name, json_service_def=service_json
+        )
+
+        return ServicePackage(
+            service=grpc_service.service_class,
+            descriptor=grpc_service.descriptor,
+            registration_function=grpc_service.registration_function,
+            stub_class=grpc_service.client_stub_class,
+            messages=client_module,
+        )
 
     # Implementation details for pure python service packages #
     @staticmethod
     def _get_and_filter_modules(
         caikit_config: aconfig.Config, lib: str
     ) -> Set[Type[ModuleBase]]:
         clean_modules = set()
@@ -261,33 +198,52 @@
             caikit_config.runtime.service_generation
             and caikit_config.runtime.service_generation.module_guids
             and caikit_config.runtime.service_generation.module_guids.excluded
         )
 
         for ck_module in modules:
             # Only create for modules from defined included and exclusion list
-            module_info = get_module_info(ck_module)
-            if excluded_task_types and module_info.type in excluded_task_types:
-                log.debug("Skipping module %s of type %s", ck_module, module_info.type)
+
+            if not ck_module.TASK_CLASS:
+                log.debug(
+                    "Skipping module %s with no task",
+                    ck_module,
+                )
+                continue
+
+            if (
+                excluded_task_types
+                and ck_module.TASK_CLASS.__name__ in excluded_task_types
+            ):
+                log.debug(
+                    "Skipping module %s with excluded task %s",
+                    ck_module,
+                    ck_module.TASK_CLASS.__name__,
+                )
                 continue
 
             if excluded_modules and ck_module.MODULE_ID in excluded_modules:
-                log.debug("Skipping module %s of id %s", ck_module, ck_module.MODULE_ID)
+                log.debug(
+                    "Skipping module %s with excluded id %s",
+                    ck_module,
+                    ck_module.MODULE_ID,
+                )
                 continue
 
             # no inclusions specified means include everything
             if (included_task_types is None or included_task_types == []) and (
                 included_modules is None or included_modules == []
             ):
                 clean_modules.add(ck_module)
 
             # if inclusion is specified, use that
             else:
                 if (included_modules and ck_module.MODULE_ID in included_modules) or (
-                    included_task_types and module_info.type in included_task_types
+                    included_task_types
+                    and ck_module.TASK_CLASS.__name__ in included_task_types
                 ):
                     clean_modules.add(ck_module)
 
         log.debug(
             "Filtered list of modules %s after excluding task types: %s and modules ids: %s. \
                 Exclusions are defined in config",
             clean_modules,
@@ -313,33 +269,14 @@
 
         raise CaikitRuntimeException(
             grpc.StatusCode.INTERNAL,
             "Could not find service descriptor in caikit_runtime_pb2",
         )
 
     @staticmethod
-    def _get_servicer_function(
-        caikit_runtime_pb2_grpc,
-        lib_name,
-    ) -> Callable[[google.protobuf.service.Service, grpc.Server], None]:
-        """Get ServiceServicer function from caikit_runtime_pb2_grpc module"""
-        servicer = f"add_{lib_name}ServiceServicer_to_server"
-        train_servicer = f"add_{lib_name}TrainingServiceServicer_to_server"
-
-        if hasattr(caikit_runtime_pb2_grpc, servicer):
-            return getattr(caikit_runtime_pb2_grpc, servicer)
-        if hasattr(caikit_runtime_pb2_grpc, train_servicer):
-            return getattr(caikit_runtime_pb2_grpc, train_servicer)
-
-        raise CaikitRuntimeException(
-            grpc.StatusCode.INTERNAL,
-            "Could not find servicer function in caikit_runtime_pb2_grpc",
-        )
-
-    @staticmethod
     def _get_servicer_class(
         caikit_runtime_pb2_grpc,
         lib_name,
     ) -> Type[google.protobuf.service.Service]:
         """Get google.protobufs.service.Service interface class from
         caikit_runtime_pb2_grpc module"""
         servicer = f"{lib_name}ServiceServicer"
@@ -377,36 +314,7 @@
 
     @staticmethod
     def _get_lib_name_for_servicer() -> str:
         """Get caikit library name from Config, make upper case and not include caikit_"""
         lib_names = import_util.clean_lib_names(get_config().runtime.library)
         assert len(lib_names) == 1, "Only 1 caikit library supported for now"
         return snake_to_upper_camel(lib_names[0].replace("caikit_", ""))
-
-    @staticmethod
-    def _get_compiled_proto_module(
-        module: str,
-        config=None,
-    ) -> ModuleType:
-        """
-        Dynamically import the compiled service module. This is accomplished via dynamic
-        import on the RUNTIME_COMPILED_PROTO_MODULE_DIR's environment variable.
-
-        Args:
-            config(aconfig.Config): caikit configuration
-
-        Returns:
-            (module): Handle to the module after dynamic import
-        """
-        if not config:
-            config = get_config()
-        module_dir = config.runtime.compiled_proto_module_dir
-        service_proto_gen_module = import_util.get_dynamic_module(module, module_dir)
-        if service_proto_gen_module is None:
-            message = (
-                "Unable to load compiled proto module: %s within dir %s"
-                % (module)
-                % (module_dir)
-            )
-            log.error("<RUN22291313E>", message)
-            raise CaikitRuntimeException(grpc.StatusCode.INTERNAL, message)
-        return service_proto_gen_module
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `caikit-0.6.0/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.7.0/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.7.0/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/service_generation/rpcs.py` & `caikit-0.7.0/caikit/runtime/service_generation/rpcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 # limitations under the License.
 """
 This package has classes that will serialize a python interface to a protocol buffer interface.
 
 Typically used for `caikit.core.module`s that expose .train and .run functions.
 """
 # Standard
-from typing import Any, Dict, List, Optional, Tuple, Type, get_args
+from typing import Any, Dict, List, Optional, Type, Union, get_args, get_origin
 import abc
 import copy
 
 # First Party
 from py_to_proto.dataclass_to_proto import (  # NOTE: Imported from here for compatibility
     Annotated,
     FieldNumber,
 )
 import alog
 
 # Local
-from . import primitives, type_helpers
+from . import protoable, type_helpers
 from .compatibility_checker import ApiFieldNames
 from .data_stream_source import make_data_stream_source
-from caikit.core import ModuleBase
+from caikit.core import ModuleBase, TaskBase
 from caikit.core.data_model.base import DataBase
 from caikit.core.data_model.dataobject import (
     DataObjectBase,
     _DataObjectBaseMetaClass,
     dataobject,
 )
 from caikit.core.signature_parsing import CaikitMethodSignature, CustomSignature
@@ -109,79 +109,72 @@
     """Helper class to create a unique RPC corresponding with the train function
     for a given module class
     """
 
     def __init__(
         self,
         method_signature: CaikitMethodSignature,
-        primitive_data_model_types: List[str],
     ):
         """Initialize a .proto generator with a single module to convert
 
         Args:
             method_signature (CaikitMethodSignature): The module method signature to
             generate an RPC for
-
-            primitive_data_model_types: List[str]
-                List of primitive data model types for a caikit_* library, such as
-                caikit.interfaces.nlp.data_model.RawDocument for nlp domains
         """
         self.clz: Type[ModuleBase] = method_signature.module
         self._method = ModuleClassTrainRPC._mutate_method_signature_for_training(
-            method_signature, primitive_data_model_types
+            method_signature
         )
-        self.name = self._module_class_to_rpc_name()
+        self.name = ModuleClassTrainRPC.module_class_to_rpc_name(self.clz)
 
         # Compute the mapping from argument name to type for the module's run
         log.debug3("Param Dict: %s", self._method.parameters)
         log.debug3("Return Type: %s", self._method.return_type)
 
         # Store the input and output protobuf message types for this RPC
         self.return_type = self._method.return_type
         self._req = _RequestMessage(
-            self._module_class_to_req_name(),
+            ModuleClassTrainRPC.module_class_to_req_name(self.clz),
             self._method.parameters,
             self._method.default_parameters,
         )
 
     @property
     def module_list(self) -> List[Type[ModuleBase]]:
         """Returns a list containing the single caikit.core.module type that this RPC is for"""
         return [self.clz]
 
     @property
     def request(self) -> "_RequestMessage":
         return self._req
 
-    def _module_class_to_rpc_name(self) -> str:
+    @staticmethod
+    def module_class_to_rpc_name(module_class: Type[ModuleBase]) -> str:
         """Helper function to convert from the name of a module to the name of the
         request RPC function
         """
-        module_split = self.clz.__module__.split(".")
         return snake_to_upper_camel(
-            f"{module_split[1]}_{module_split[2]}_{self.clz.__name__}_Train"
+            f"{module_class.TASK_CLASS.__name__}_{module_class.__name__}_Train"
         )
 
-    def _module_class_to_req_name(self) -> str:
+    @staticmethod
+    def module_class_to_req_name(module_class: Type[ModuleBase]) -> str:
         """Helper function to convert from the name of a module to the name of the
         request RPC message
 
         Example: self.clz._module__ = sample_lib.modules.sample_task.sample_implementation
 
-        return: BlocksSampleTaskSampleModuleTrainRequest
+        return: SampleTaskSampleModuleTrainRequest
 
         """
-        module_split = self.clz.__module__.split(".")
-        return snake_to_upper_camel(
-            f"{module_split[1]}_{module_split[2]}_{self.clz.__name__}_TrainRequest"
-        )
+        return f"{ModuleClassTrainRPC.module_class_to_rpc_name(module_class)}Request"
 
     @staticmethod
     def _mutate_method_signature_for_training(
-        signature, primitive_data_model_types: List[str]
+        signature: CaikitMethodSignature,
     ) -> Optional[CaikitMethodSignature]:
         # Change return type for async training interface
         return_type = TrainingJob
 
         new_params = {"model_name": str}
         for name, typ in signature.parameters.items():
             if type_helpers.has_data_stream(typ):
@@ -194,60 +187,51 @@
                 ), "Cannot handle DataStream with multiple type args"
                 element_type = element_types[0]
                 new_params[name] = make_data_stream_source(element_type)
             elif type_helpers.is_model_type(typ):
                 # Found a model pointer
                 new_params[name] = ModelPointer
             else:
-                new_params[name] = primitives.extract_primitive_type_from_union(
+                new_params[name] = protoable.handle_protoables_in_union(
                     arg_type=typ,
-                    primitive_data_model_types=primitive_data_model_types,
                 )
 
         return CustomSignature(
             original_signature=signature, parameters=new_params, return_type=return_type
         )
 
 
 class TaskPredictRPC(CaikitRPCBase):
     """Helper class to create a unique RPC for the aggregate set of Modules that
     implement the same task
     """
 
     def __init__(
         self,
-        task: Tuple[str, str],
+        task: Type[TaskBase],
         method_signatures: List[CaikitMethodSignature],
-        primitive_data_model_types: List[str],
     ):
         """Initialize a .proto generator with all modules of a given task to convert
 
         Args:
-            task (Tuple[str, str]): The library / ai-problem-task combo that describes the task
-                type. For example: ("my_caikit_library", "classification")
+            task (Type[TaskBase]): Task type
 
             method_signatures (List[CaikitMethodSignature]): The list of method
                 signatures from concrete modules implementing this task
-
-            primitive_data_model_types: List[str]
-                List of primitive data model types for a caikit_* library, such as
-                caikit.interfaces.nlp.data_model.RawDocument for nlp domains
         """
         self.task = task
         self._module_list = [method.module for method in method_signatures]
         self._method_signatures = method_signatures
 
         # Aggregate the argument signature types into a single parameters_dict
         parameters_dict = {}
         default_parameters = {}
         for method in method_signatures:
             default_parameters.update(method.default_parameters)
-            primitive_arg_dict = primitives.to_primitive_signature(
-                method.parameters, primitive_data_model_types
-            )
+            primitive_arg_dict = protoable.to_protoable_signature(method.parameters)
             for arg_name, arg_type in primitive_arg_dict.items():
                 current_val = parameters_dict.get(arg_name, arg_type)
                 # TODO: raise runtime error here instead of assert!
                 # TODO: need to resolve Optional[T] vs. T - if both come in, use Optional[T]
                 assert (
                     current_val == arg_type
                 ), f"Conflicting value types for arg {arg_name}: {current_val} != {arg_type}"
@@ -258,15 +242,15 @@
             self._task_to_req_name(), parameters_dict, default_parameters
         )
 
         # Validate that the return_type of all modules in the grouping matches
         return_types = {method.return_type for method in method_signatures}
         assert len(return_types) == 1, f"Found multiple return types for task [{task}]"
         return_type = list(return_types)[0]
-        self.return_type = primitives.extract_data_model_type_from_union(return_type)
+        self.return_type = protoable.extract_data_model_type_from_union(return_type)
 
         # Create the rpc name based on the module type
         self.name = self._task_to_rpc_name()
 
     @property
     def module_list(self) -> List[Type[ModuleBase]]:
         """Returns the list of all caikit.core.modules that this RPC will be for. These should all
@@ -278,26 +262,25 @@
     def request(self) -> "_RequestMessage":
         return self._req
 
     def _task_to_req_name(self) -> str:
         """Helper function to convert the pair of library name and task name to
         a request message name
         """
-        return snake_to_upper_camel(f"{self.task[1]}_Request")
+        return snake_to_upper_camel(f"{self.task.__name__}_Request")
 
     def _task_to_rpc_name(self) -> str:
         """Helper function to convert the pair of library name and task name
         to an RPC name
 
         Example: self.task = (sample_lib, sample_task)
 
         return: SampleTaskPredict
         """
-
-        return snake_to_upper_camel(f"{self.task[1]}_Predict")
+        return snake_to_upper_camel(f"{self.task.__name__}_Predict")
 
 
 class _RequestMessage:
     """Helper class to create the input request message that wraps up the inputs
     for a given function. The request Contains N named data-model or primitive
     objects.
     """
@@ -315,22 +298,25 @@
         existing_fields = ApiFieldNames.get_fields_for_message(self.name)
 
         if len(existing_fields) > 0:
             last_used_number = max(existing_fields.values())
         else:
             last_used_number = 0
 
-        for _, (item_name, p) in enumerate(params.items()):
+        for _, (item_name, typ) in enumerate(params.items()):
             if item_name in existing_fields:
                 # if field existed previously, get the original number from there
                 num = existing_fields[item_name]
             else:
                 num = last_used_number + 1
-                last_used_number += 1
-            self.triples.append((p, item_name, num))
+                if get_origin(typ) is Union:
+                    last_used_number += len(get_args(typ))
+                else:
+                    last_used_number += 1
+            self.triples.append((typ, item_name, num))
 
         self.triples.sort(key=lambda x: x[2])
 
 
 def snake_to_upper_camel(string: str) -> str:
     """Simple snake -> upper camel conversion"""
     return "".join([part[0].upper() + part[1:] for part in string.split("_")])
```

### Comparing `caikit-0.6.0/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.7.0/caikit/runtime/service_generation/type_helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,42 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Some type conversion helpers for going between python and protocol buffer interfaces
 """
-
 # Standard
 from inspect import isclass
-from typing import Dict, Optional, Type, Union, get_args, get_origin
-
-# First Party
-# First party
-import alog
+from typing import Optional, Type, Union, get_args, get_origin
 
 # Local
 from caikit.core import ModuleBase
-from caikit.core.data_model import DataStream
-import caikit.core
-
-log = alog.use_channel("PGEN-TYPEHLP")
-
-# Constants #########################################
-# The common prefix for all data model package names
-caikit.core_DATA_MODEL_PREFIX = "caikit.core_data_model"
-
-# Mapping from native python types to the corresponding protobufs types
-PROTO_TYPE_MAP: Dict[Type, str] = {
-    float: "double",
-    int: "int32",
-    bool: "bool",
-    str: "string",
-    bytes: "bytes",
-}
+from caikit.core.data_model import DataBase, DataStream
 
 
 def has_data_stream(arg_type: Type) -> bool:
     """Recursive check for a DataStream container in a type annotation"""
     if _is_data_stream(arg_type):
         return True
 
@@ -79,9 +58,13 @@
     if typing_origin is Union:
         for typ in typing_args:
             if isclass(typ) and issubclass(typ, ModuleBase):
                 return True
     return False
 
 
+def is_data_model_type(arg_type: Type) -> bool:
+    return isclass(arg_type) and issubclass(arg_type, DataBase)
+
+
 def _is_data_stream(arg_type: Type) -> bool:
     return arg_type == DataStream or get_origin(arg_type) == DataStream
```

### Comparing `caikit-0.6.0/caikit/runtime/servicers/__init__.py` & `caikit-0.7.0/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.7.0/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.7.0/caikit/runtime/servicers/global_train_servicer.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,72 +9,75 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from importlib.metadata import version
-from typing import Optional, Type
+from typing import Optional
 from uuid import uuid4
 import concurrent.futures
-import importlib
 import multiprocessing
 import os
-import re
+import threading
 import traceback
 
 # Third Party
 from google.protobuf.descriptor import FieldDescriptor
-from grpc import StatusCode
-import grpc
+from grpc import ServicerContext, StatusCode
 
 # First Party
 import alog
 
 # Local
 from caikit import get_config
-from caikit.core import ModuleBase
 from caikit.interfaces.runtime.data_model import TrainingJob
 from caikit.runtime.model_management.model_manager import ModelManager
 from caikit.runtime.model_management.training_manager import TrainingManager
 from caikit.runtime.service_factory import ServicePackage
+from caikit.runtime.service_generation.rpcs import ModuleClassTrainRPC
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils.import_util import clean_lib_names, get_data_model
 from caikit.runtime.utils.servicer_util import (
     build_caikit_library_request_dict,
-    snake_to_upper_camel,
     validate_data_model,
 )
+from caikit.runtime.work_management.train_executors import (
+    LocalTrainSaveExecutor,
+    SubProcessTrainSaveExecutor,
+)
 import caikit.core
 
 log = alog.use_channel("GT-SERVICR-I")
-
+error = caikit.core.toolkit.errors.error_handler.get(log)
 
 # Protobuf non primitives
 # Ref: https://developers.google.com/protocol-buffers/docs/reference/cpp/google.protobuf.descriptor
 NON_PRIMITIVE_TYPES = [FieldDescriptor.TYPE_MESSAGE, FieldDescriptor.TYPE_ENUM]
 
-OOM_EXIT_CODE = 137
-
 # pylint: disable=too-many-instance-attributes
 class GlobalTrainServicer:
     """Something something about the train servicer"""
 
     def __init__(self, training_service: ServicePackage):
         self._training_service = training_service
         self._model_manager = ModelManager.get_instance()
         self.training_manager = TrainingManager.get_instance()
-        self.executor = concurrent.futures.ThreadPoolExecutor()
+        # NOTE: we are using ThreadPoolExecutor for simplicity of the
+        # the API with an intent to handle the training job
+        # in an async fashion with "Futures".
+        self.executor = concurrent.futures.ThreadPoolExecutor(max_workers=1)
         # store the map of model ids to job ids
         self.training_map = self.training_manager.training_futures
         caikit_config = get_config()
         self.training_output_dir = caikit_config.runtime.training.output_dir
         self.auto_load_trained_model = (
             caikit_config.runtime.training.auto_load_trained_model
         )
+
         self.use_subprocess = caikit_config.runtime.training.use_subprocess
 
         # TODO: think about if we really want to do this here:
         self.cdm = get_data_model()
 
         # Validate that the Caikit Library CDM is compatible with our service descriptor
         validate_data_model(self._training_service.descriptor)
@@ -94,15 +97,15 @@
             "<RUN76884779I>",
             "Constructed train service for library: %s, version: %s",
             self.library,
             lib_version,
         )
         super()
 
-    def Train(self, request, *_, **__) -> TrainingJob:
+    def Train(self, request, context, *_, **__) -> TrainingJob:
         """Global predict RPC -- Mocks the invocation of a Caikit Library module.train()
         method for a loaded Caikit Library model
         Args:
             request(object):
                 A deserialized RPC request message
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
         Returns:
@@ -110,32 +113,18 @@
                 A TrainingJob data model response object
         """
         desc_name = request.DESCRIPTOR.name
         outer_scope_name = "GlobalTrainServicer.Train:%s" % desc_name
 
         try:
             with alog.ContextLog(log.debug, outer_scope_name):
-                # BlocksSampleTaskSampleModuleTrainRequest
-                # getattr(importlib.import_module("sample_lib.modules.sample_task"), "SampleModule")
-                # TODO: fixme - temporary workaround for now
-                desc_name = desc_name.replace("TrainRequest", "")
-                split = re.split("(?<=.)(?=[A-Z])", desc_name)
-                model = None
-                try:
-                    model = getattr(
-                        importlib.import_module(
-                            f"{self.library}.{split[0].lower()}.{split[1].lower()}"
-                        ),
-                        f"{''.join(split[2:])}",
-                    )
-                except Exception:  # pylint: disable=broad-exception-caught
-                    for mod in caikit.core.registries.module_registry().values():
-                        module_split = mod.__module__.split(".")
-                        train_request_for_mod = snake_to_upper_camel(
-                            f"{module_split[1]}_{module_split[2]}_{mod.__name__}"
+                for mod in caikit.core.registries.module_registry().values():
+                    if mod.TASK_CLASS:
+                        train_request_for_mod = (
+                            ModuleClassTrainRPC.module_class_to_req_name(mod)
                         )
                         if train_request_for_mod == desc_name:
                             model = mod
                             break
 
                 # At this point, if model is still None, we don't know the module this request
                 # is for
@@ -147,14 +136,15 @@
                 # generate a unique training id
                 training_id = str(uuid4())
                 return self.run_training_job(
                     request=request,
                     model=model,
                     training_id=training_id,
                     training_output_dir=self.training_output_dir,
+                    context=context,
                 )
 
         except CaikitRuntimeException as e:
             log_dict = {
                 "log_code": "<RUN50530380W>",
                 "message": e.message,
                 "error_id": e.id,
@@ -189,14 +179,15 @@
 
     def run_training_job(
         self,
         request,
         model,
         training_id,
         training_output_dir,
+        context: ServicerContext,
         wait=False,
     ) -> TrainingJob:
         """Builds the request dict for calling the train function asynchronously,
         then returns the thread id"""
 
         # Figure out where this model will be saved
         model_name = request.model_name
@@ -205,63 +196,100 @@
         # Build the full set of kwargs for the train and save call
         kwargs = {
             "module_class": model,
             "model_path": model_path,
             **build_caikit_library_request_dict(request, model.train),
         }
 
-        # If running with a subprocess, set the target and args accordingly
-        target = (
-            self._train_and_save_model_subproc
-            if self.use_subprocess
-            else self._train_and_save_model
-        )
+        # If running with a subprocess, set the target, events and args accordingly
+        if self.use_subprocess:
+            cancel_event = multiprocessing.Event()
+            target = SubProcessTrainSaveExecutor(cancel_event)
+        else:
+            cancel_event = threading.Event()
+            target = LocalTrainSaveExecutor(cancel_event)
+
         log.debug2(
             "Training with %s",
             "SUBPROCESS" if self.use_subprocess else "MAIN PROCESS",
         )
 
         # start training asynchronously
         thread_future = self.run_async(
-            runnable_func=target,
+            runnable_executor=target,
             kwargs=kwargs,
             model_name=model_name,
             model_path=model_path,
         )
+
         self.training_map[training_id] = thread_future
 
-        # if requested, block until the training completes
+        # Create a callback to register termination of training
+        def rpc_termination_callback():
+            """Function to be called when the RPC is terminated.
+            This can happen when the training is completed or
+            when we receive a cancellation request.
+            """
+            for event in target.events:
+                if not event.is_set():
+                    event.set()
+
+        # if requested, wait for training to complete, thus
+        # allowing different servicers to cancel the request
+        # in case needed. This does make this call synchronous,
+        # but that is the intent of this function, since for async request
+        # we have separate function below returning futures.
+        # TODO: In future, for the case where we want to execute the training
+        # in async manner, we would implement a separate "cancel" / "delete"
+        # API which would integrate with different training backends
+        # as per their interface requirements.
         if wait:
+            # NOTE: callback registration needs to be before
+            # waiting for the future, otherwise request will wait before registering
+            # callback
+            # Add callback for termination of request
+            callback_registered = context.add_callback(rpc_termination_callback)
+
+            if not callback_registered:
+                log.warning(
+                    "<RUN54118242W>",
+                    "Failed to register rpc termination callback, aborting rpc",
+                )
+                raise CaikitRuntimeException(
+                    StatusCode.ABORTED,
+                    "Could not register RPC callback, call has likely terminated.",
+                )
+
             with alog.ContextTimer(log.debug, "Training %s complete in: ", training_id):
                 thread_future.result()
 
         # return TrainingJob object
         return TrainingJob(
             model_name=request.model_name, training_id=training_id
         ).to_proto()
 
     def run_async(
         self,
-        runnable_func,
+        runnable_executor,
         kwargs,
         model_name,
         model_path,
     ) -> concurrent.futures.Future:
         """Runs the train function in a thread and saves the trained model in a callback"""
+
         if self.auto_load_trained_model:
 
             def target(*args, **kwargs):
-                runnable_func(*args, **kwargs)
+                runnable_executor.train_and_save_model(*args, **kwargs)
                 return self._load_trained_model(model_name, model_path)
 
         else:
-            target = runnable_func
+            target = runnable_executor.train_and_save_model
 
-        future = self.executor.submit(target, **kwargs)
-        return future
+        return self.executor.submit(target, **kwargs)
 
     def _get_model_path(
         self,
         training_output_dir: Optional[str],
         model_name: str,
         training_id: str,
     ) -> str:
@@ -283,131 +311,7 @@
         log.debug("Autoloading trained model %s", model_name)
         self._model_manager.load_model(
             model_id=model_name,
             local_model_path=model_path,
             model_type="standalone",
         )
         return self._model_manager.retrieve_model(model_name)
-
-    @staticmethod
-    def _train_and_save_model(
-        module_class: Type[ModuleBase],
-        model_path: str,
-        *args,
-        **kwargs,
-    ):
-        """This function performs a single training and can be run inside a
-        subprocess if needed
-        """
-        try:
-            # Train it
-            with alog.ContextTimer(
-                log.debug, "Done training %s in: ", module_class.__name__
-            ):
-                model = module_class.train(*args, **kwargs)
-
-            # Save it
-            with alog.ContextTimer(
-                log.debug,
-                "Done saving %s to %s in: ",
-                module_class.__name__,
-                model_path,
-            ):
-                model.save(model_path)
-
-        # Handle errors as CaikitRuntime errors with appropriate error codes
-        except CaikitRuntimeException as e:
-            log.warning(
-                {
-                    "log_code": "<RUN555430380W>",
-                    "message": e.message,
-                    "error_id": e.id,
-                    **e.metadata,
-                }
-            )
-            raise e
-        except (TypeError, ValueError) as e:
-            log.warning(
-                {
-                    "log_code": "<RUN868639039W>",
-                    "message": repr(e),
-                    "stack_trace": traceback.format_exc(),
-                }
-            )
-            raise CaikitRuntimeException(
-                StatusCode.INVALID_ARGUMENT,
-                f"Exception raised during training. This may be a problem with your input: {e}",
-            ) from e
-        except Exception as e:
-            log.warning(
-                {
-                    "log_code": "<RUN490967039W>",
-                    "message": repr(e),
-                    "stack_trace": traceback.format_exc(),
-                }
-            )
-            raise CaikitRuntimeException(
-                StatusCode.INTERNAL,
-                f"Exception raised during training: {e}",
-            ) from e
-
-    @classmethod
-    def _train_and_save_model_subproc(cls, *args, **kwargs):
-        """This function runs _train_and_save_model in a subprocess"""
-
-        proc = cls._ErrorCaptureProcess(
-            target=cls._train_and_save_model,
-            args=args,
-            kwargs=kwargs,
-        )
-
-        proc.start()
-        proc.join()
-
-        # If an error occurred, reraise it here
-        # TODO: Make sure the stack trace is preserved
-        if proc.error is not None:
-            if isinstance(proc.error, CaikitRuntimeException):
-                raise proc.error
-            raise CaikitRuntimeException(
-                grpc.StatusCode.INTERNAL,
-                "Error caught in training subprocess",
-            ) from proc.error
-
-        # If process exited with a non-zero exit code
-        if proc.exitcode and proc.exitcode != os.EX_OK:
-            if proc.exitcode == OOM_EXIT_CODE:
-                exception = CaikitRuntimeException(
-                    grpc.StatusCode.RESOURCE_EXHAUSTED,
-                    "Training process died with OOM error!",
-                )
-            else:
-                exception = CaikitRuntimeException(
-                    grpc.StatusCode.UNKNOWN,
-                    f"Training process died with exit code {proc.exitcode}",
-                )
-            raise exception
-
-    class _ErrorCaptureProcess(multiprocessing.get_context("fork").Process):
-        """This class wraps a Process and keeps track of any errors that occur
-        during execution
-
-        NOTE: We explicitly use "fork" here for two reasons:
-            1. It's faster
-            2. Due to the auto-generated classes with stream sources, "spawn"
-               can result in missing classes since it performs a full re-import,
-               but does not regenerate the service APIs
-        """
-
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-            self.error = None
-
-        def run(self, *args, **kwargs):
-            try:
-                return super().run(*args, **kwargs)
-
-            # Catch any errors thrown within a subprocess so that they can be
-            # forwarded to the parent
-            # pylint: disable=broad-exception-caught
-            except Exception as err:
-                self.error = err
```

### Comparing `caikit-0.6.0/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.7.0/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.7.0/caikit/runtime/servicers/model_train_servicer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,32 @@
 
 # First Party
 import alog
 
 # Local
 from caikit.runtime.protobufs import process_pb2, process_pb2_grpc
 from caikit.runtime.service_factory import ServicePackage
+from caikit.runtime.service_generation.rpcs import ModuleClassTrainRPC
 from caikit.runtime.servicers.global_train_servicer import GlobalTrainServicer
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
-from caikit.runtime.utils.servicer_util import snake_to_upper_camel
 import caikit.core
 
 log = alog.use_channel("MT-SERVICR-I")
 
 
 class ModelTrainServicerImpl(process_pb2_grpc.ProcessServicer):
     """This class contains the implementation of the Model Train process.proto
     interface (a.k.a. the Process Servicer).
     """
 
     def __init__(self, training_service: ServicePackage):
         self._training_service = training_service
         self._gts = GlobalTrainServicer(self._training_service)
 
-    def Run(self, request, context=None):
+    def Run(self, request, context):
         """`Run` RPC -- launches a training job.
         Args:
             request(process_pb2.ProcessRequest):
                 Generated from process.proto
             context(grpc.ServicerContext): Context object (contains request metadata, etc)
         Returns:
             process_pb2.ProcessResponse:
@@ -67,18 +67,15 @@
                 raise CaikitRuntimeException(
                     grpc.StatusCode.INVALID_ARGUMENT,
                     "Model Train not able to parse module for this Train Request",
                 )
 
             # prepare the model's train request
             training_params = json.loads(request_dict["training_params"])
-            module_split = train_module.__module__.split(".")
-            request_name = snake_to_upper_camel(
-                f"{module_split[1]}_{module_split[2]}_{train_module.__name__}_TrainRequest"
-            )
+            request_name = ModuleClassTrainRPC.module_class_to_req_name(train_module)
             log.debug("<RUN22972949D>", "request_name: %s", request_name)
 
             if not hasattr(self._training_service.messages, request_name):
                 raise CaikitRuntimeException(
                     grpc.StatusCode.INTERNAL,
                     f"Model Train not able to create a request for {request_name}",
                 )
@@ -86,19 +83,21 @@
             # construct the protobufs message request with train params
             train_message_request = ParseDict(
                 training_params,
                 req_name_func(),
             )
             # make the train call
             log.debug("Training output dir: %s", request.training_output_dir)
+
             training_response = self._gts.run_training_job(
                 request=train_message_request,
                 model=train_module,
                 training_id=request.trainingID,
                 training_output_dir=request.training_output_dir,
+                context=context,
                 wait=True,
             )
             log.debug("<RUN00837184D>", "training_response: %s", training_response)
             # return response
             process_response = process_pb2.ProcessResponse(
                 trainingID=training_response.training_id,
                 customTrainingID=request.customTrainingID,
```

### Comparing `caikit-0.6.0/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.7.0/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/types/__init__.py` & `caikit-0.7.0/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/types/aborted_exception.py` & `caikit-0.7.0/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.7.0/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.7.0/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/utils/__init__.py` & `caikit-0.7.0/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/utils/import_util.py` & `caikit-0.7.0/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/utils/servicer_util.py` & `caikit-0.7.0/caikit/runtime/utils/servicer_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -234,69 +234,99 @@
     log.debug("valid kwarg names: %s", valid_kwarg_names)
     cdm = get_data_model()
     try:
         log.debug2(
             "We are looping though these fields: %s",
             [field.name for field in request.DESCRIPTOR.fields],
         )
+        # get all oneof fields excluding from optional oneofs
+        one_of_fields = []
+        for oneof_name, oneof in request.DESCRIPTOR.oneofs_by_name.items():
+            one_of_fields.extend(
+                [
+                    field.name
+                    for field in oneof.fields
+                    if len(oneof.fields) != 1
+                    or oneof_name != f"_{oneof.fields[0].name}"
+                ]
+            )
         for field in request.DESCRIPTOR.fields:
+            field_name = field.name
+            field_value = None
+            log.debug2("processing field: %s", field_name)
+
+            # check for oneofs
+            if field_name in one_of_fields:
+                # get the containing oneof name
+                oneof_name = field.containing_oneof.name
+                # Check if the field is the one set in the oneof
+                if request.WhichOneof(oneof_name) == field_name:
+                    # get the field_value
+                    field_value = getattr(request, field_name)
+                    # change the field_name to be of the oneof name
+                    log.debug3(
+                        "changing field name %s to be of the oneof: %s",
+                        field_name,
+                        oneof_name,
+                    )
+                    field_name = oneof_name
 
-            log.debug2("processing field: %s", field.name)
             #  Need to not pass in any arg that is not supported by the function
-            if field.name not in valid_kwarg_names:
+            if field_name not in valid_kwarg_names:
                 continue
-            field_value = getattr(request, field.name)
+            if field_value is None:
+                field_value = getattr(request, field_name)
             if is_protobuf_primitive_field(field):
                 # We don't need to convert this field to a Caikit Library CDM instance
                 # We also don't set the field if it is an int 0, which happens by default
                 # if a value is left empty, otherwise we would be sending values like 0 for limit
                 # bool is a subclass of int (https://docs.python.org/3/library/functions.html#bool)
                 # so this needs to be handled separately
                 log.debug2(
                     "<RUN51658873D>",
                     "Field name [%s] with value [%s] is a primitive of type [%s]",
-                    field.name,
+                    field_name,
                     field_value,
                     type(field_value),
                 )
                 try:
                     # optional primitive
-                    if request.HasField(field.name):
-                        caikit_library_request_dict[field.name] = field_value
+                    if request.HasField(field_name):
+                        caikit_library_request_dict[field_name] = field_value
                 except ValueError as e:
                     # non-optional primitives and iterables
                     log.debug2(
                         "failed to check HasField on field %s, error: %s",
-                        field.name,
+                        field_name,
                         e,
                     )
                     # iterables
                     if isinstance(field_value, Iterable):
                         if len(field_value) != 0:
                             # cast only if it's actually a list
                             if not isinstance(field_value, (str, bytes)):
-                                if "training_data" in field.name:
+                                if "training_data" in field_name:
                                     caikit_library_request_dict[
-                                        field.name
+                                        field_name
                                     ] = DataStream.from_iterable(field_value)
                                 else:
-                                    caikit_library_request_dict[field.name] = list(
+                                    caikit_library_request_dict[field_name] = list(
                                         field_value
                                     )
                             # if not, pass it as is. (non-optional str & bytes)
                             else:
-                                caikit_library_request_dict[field.name] = field_value
+                                caikit_library_request_dict[field_name] = field_value
                     # non-iterable primitives
                     else:
-                        caikit_library_request_dict[field.name] = field_value
+                        caikit_library_request_dict[field_name] = field_value
             else:
                 log.debug2(
                     "<RUN55658873D>",
                     "field is not primitive: %s (%s) type(%s)",
-                    field.name,
+                    field_name,
                     field_value,
                     type(field_value),
                 )
                 # iterables
                 if isinstance(field_value, Iterable):
                     if len(field_value) != 0:
                         # We sure we want a DataStream? - after huddling
@@ -318,39 +348,39 @@
                             caikit_library_class = getattr(cdm, class_name)
                             # Use the Caikit Library CDM class's from_proto
                             # method to turn our protobufs field message into an
                             # instance of the Caikit Library CDM class
                             instance = caikit_library_class.from_proto(field_item)
                             instances.append(instance)
 
-                        if "training_data" in field.name:
+                        if "training_data" in field_name:
                             data_stream = DataStream.from_iterable(instances)
-                            caikit_library_request_dict[field.name] = data_stream
+                            caikit_library_request_dict[field_name] = data_stream
                         else:
-                            caikit_library_request_dict[field.name] = field_value
+                            caikit_library_request_dict[field_name] = field_value
                 else:
                     log.debug2(
                         "<RUN55258876D>",
                         "field is not primitive, and also not an Iterable: %s (%s) type(%s)",
-                        field.name,
+                        field_name,
                         field_value,
                         type(field_value),
                     )
                     # if it's a custom datastream dataobject
                     stream_source = get_data_stream_source(field_value)
                     if stream_source:
                         caikit_library_request_dict[
-                            field.name
+                            field_name
                         ] = stream_source.to_data_stream()
 
                     else:
                         log.debug2(
                             "<RUN64546176D>",
                             "field should not have stream source: %s (%s) type(%s)",
-                            field.name,
+                            field_name,
                             field_value,
                             type(field_value),
                         )
                         # Start by getting the class name for this particular
                         # field (e.g., RawDocument)
                         class_name = type(field_value).DESCRIPTOR.name
 
@@ -359,29 +389,29 @@
                             log.debug2("field_value is a ModelPointer obj")
                             if field_value.model_id:
                                 model_manager = ModelManager.get_instance()
                                 model_retrieved = model_manager.retrieve_model(
                                     field_value.model_id
                                 )
                                 caikit_library_request_dict[
-                                    field.name
+                                    field_name
                                 ] = model_retrieved
                         else:
                             # Now get the Caikit Library CDM class of the same
                             # name
                             caikit_library_class = getattr(cdm, class_name)
                             # Use the Caikit Library CDM class's from_proto
                             # method to turn our protobufs field message into an
                             # instance of the Caikit Library CDM class
                             instance = caikit_library_class.from_proto(field_value)
                             # Add to the request dictionary, using the message
                             # field's name as the key (since, by convention, the
                             # argument name to the module run function will be
                             # the same as the field name)
-                            caikit_library_request_dict[field.name] = instance
+                            caikit_library_request_dict[field_name] = instance
 
         log.debug2(
             "caikit_library_request_dict returned is: %s", caikit_library_request_dict
         )
 
         return caikit_library_request_dict
```

### Comparing `caikit-0.6.0/caikit/runtime/work_management/__init__.py` & `caikit-0.7.0/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/work_management/abortable_action.py` & `caikit-0.7.0/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/work_management/call_aborter.py` & `caikit-0.7.0/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.7.0/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/Makefile` & `caikit-0.7.0/docs/Makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
 SPHINXOPTS    ?=
 SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
+SOURCEDIR     = source
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
```

### Comparing `caikit-0.6.0/docs/adrs/010-data-model-definition.md` & `caikit-0.7.0/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/adrs/015-runtime-service-generation.md` & `caikit-0.7.0/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/adrs/018-shared-backends.md` & `caikit-0.7.0/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/adrs/019-loader-stack.md` & `caikit-0.7.0/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/architecture_club/04-25-23.md` & `caikit-0.7.0/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/docs/conf.py` & `caikit-0.7.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-sys.path.insert(0, os.path.abspath("../"))
+sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Caikit"
 copyright = "2023, The Caikit Authors"
 author = "The Caikit Authors"
@@ -26,26 +26,36 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    "sphinx.ext.autodoc",
+    # Generate complete API docs by parsing source code
+    "autoapi.extension",
+    # Add links to source from generated docs
     "sphinx.ext.viewcode",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "caikit/config"]
 
+# -- autoapi configuration ---------------------------------------------------
+
+# Language of source code to parse
+autoapi_type = "python"
+
+# Source code to parse to generate API docs relative to 'docs/source' directory
+autoapi_dirs = [os.path.join("..", "..", "caikit")]
+
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
```

### Comparing `caikit-0.6.0/docs/make.bat` & `caikit-0.7.0/docs/make.bat`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pushd %~dp0
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
-set SOURCEDIR=.
+set SOURCEDIR=source
 set BUILDDIR=_build
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
 	echo.installed, then set the SPHINXBUILD environment variable to point
```

### Comparing `caikit-0.6.0/examples/start_runtime_with_sample_lib.py` & `caikit-0.7.0/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/README.md` & `caikit-0.7.0/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/client.py` & `caikit-0.7.0/examples/text-sentiment/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 # Local
 from caikit.runtime.service_factory import ServicePackageFactory
 from text_sentiment.data_model import TextInput
 
 inference_service = ServicePackageFactory().get_service_package(
     ServicePackageFactory.ServiceType.INFERENCE,
-    ServicePackageFactory.ServiceSource.GENERATED,
 )
 
 port = 8085
 channel = grpc.insecure_channel(f"localhost:{port}")
 
 client_stub = inference_service.stub_class(channel)
```

### Comparing `caikit-0.6.0/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.7.0/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/start_runtime.py` & `caikit-0.7.0/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.7.0/tests/runtime/generated/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# Standard
+import os
+import sys
 
-runtime:
-    library: text_sentiment
-    service_generation:
-        primitive_data_model_types:
-            - "text_sentiment.data_model.classification.TextInput"
+# Allow generated _pb2 files in here to import each other
+script_loc = os.path.dirname(os.path.realpath(__file__))
+sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/pyproject.toml` & `caikit-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.6.0"
+version = "0.7.0"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "alchemy-config>=1.1.1,<2.0.0",
     "alchemy-logging>=1.0.4,<2.0.0",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1,<0.16.0",
     "grpcio-health-checking>=1.35.0,<2.0",
+    "grpcio-reflection>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0,!=1.55.0",
     "ijson>=3.1.4,<3.3.0",
     "import-tracker>=3.1.5,<4",
     "munch>=2.5.0,<4.0",
     "numpy>=1.20,<2",
     "prometheus_client>=0.12.0,<1.0",
     "protobuf>=3.19.0,<5",
```

### Comparing `caikit-0.6.0/scripts/check_deps.sh` & `caikit-0.7.0/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/scripts/fmt.sh` & `caikit-0.7.0/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/__init__.py` & `caikit-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/config/test_configs.py` & `caikit-0.7.0/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/conftest.py` & `caikit-0.7.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,24 +56,28 @@
 
 
 @pytest.fixture(autouse=True, scope="session")
 def test_environment():
     """The most important fixture: This runs caikit configuration with the base test config overrides"""
     test_config_path = os.path.join(FIXTURES_DIR, "config", "config.yml")
     caikit.configure(test_config_path)
+    # import the mock backend that is specified in the config
+    # This is required to run any test that loads a model
+    # Local
+    from tests.core.helpers import MockBackend
+
     yield
     # No cleanup required...?
 
 
 @pytest.fixture(scope="session")
 def sample_inference_service(render_protos) -> ServicePackage:
     """Service package pointing to `sample_lib` for testing"""
     inference_service = ServicePackageFactory().get_service_package(
         ServicePackageFactory.ServiceType.INFERENCE,
-        ServicePackageFactory.ServiceSource.GENERATED,
     )
     if render_protos:
         render_dataobject_protos("tests/protos")
     return inference_service
 
 
 @pytest.fixture(scope="session")
@@ -86,47 +90,69 @@
 
 
 @pytest.fixture(scope="session")
 def sample_train_service(render_protos) -> ServicePackage:
     """Service package pointing to `sample_lib` for testing"""
     training_service = ServicePackageFactory().get_service_package(
         ServicePackageFactory.ServiceType.TRAINING,
-        ServicePackageFactory.ServiceSource.GENERATED,
     )
     if render_protos:
         render_dataobject_protos("tests/protos")
     return training_service
 
 
 @pytest.fixture(scope="session")
 def sample_train_servicer(sample_train_service) -> GlobalTrainServicer:
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     yield servicer
 
 
+@contextmanager
+def runtime_grpc_test_server(*args, **kwargs):
+    """Helper to wrap creation of RuntimeGRPCServer in temporary configurations"""
+    with tempfile.TemporaryDirectory() as workdir:
+        temp_log_dir = os.path.join(workdir, "metering_logs")
+        temp_save_dir = os.path.join(workdir, "training_output")
+        os.makedirs(temp_log_dir)
+        os.makedirs(temp_save_dir)
+        with temp_config(
+            {
+                "runtime": {
+                    "metering": {"log_dir": temp_log_dir},
+                    "training": {"output_dir": temp_save_dir},
+                }
+            },
+            "merge",
+        ):
+            with RuntimeGRPCServer(*args, **kwargs) as server:
+                # Give tests access to the workdir
+                server.workdir = workdir
+                yield server
+
+
 @pytest.fixture(scope="session")
 def runtime_grpc_server(
     sample_inference_service, sample_train_service
 ) -> RuntimeGRPCServer:
-    server = RuntimeGRPCServer(
+    with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=sample_train_service,
-    )
+    ) as server:
 
-    grpc_thread = threading.Thread(
-        target=server.start,
-    )
-    grpc_thread.setDaemon(False)
-    grpc_thread.start()
-    _check_server_readiness(server)
-    yield server
-
-    # teardown
-    server.stop(0)
-    grpc_thread.join()
+        grpc_thread = threading.Thread(
+            target=server.start,
+        )
+        grpc_thread.daemon = False
+        grpc_thread.start()
+        _check_server_readiness(server)
+        yield server
+
+        # teardown
+        server.stop(0)
+        grpc_thread.join()
 
 
 @pytest.fixture(scope="session")
 def inference_stub(sample_inference_service, runtime_grpc_server) -> Type:
     inference_stub = sample_inference_service.stub_class(
         runtime_grpc_server.make_local_channel()
     )
```

### Comparing `caikit-0.6.0/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.7.0/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.7.0/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.7.0/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/streams/test_converter.py` & `caikit-0.7.0/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.7.0/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.7.0/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/streams/test_resolver.py` & `caikit-0.7.0/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/streams/test_validator.py` & `caikit-0.7.0/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/test_base.py` & `caikit-0.7.0/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/test_dataobject.py` & `caikit-0.7.0/tests/core/data_model/test_dataobject.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,43 +21,71 @@
 import copy
 import json
 import os
 import tempfile
 
 # Third Party
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool, message
+from google.protobuf import descriptor_pb2, descriptor_pool, message, struct_pb2
 import numpy as np
 import pytest
 
 # First Party
 from py_to_proto.dataclass_to_proto import Annotated, FieldNumber, OneofField
 
 # Local
 from caikit.core import (  # NOTE: Imported from the top to validate
     DataObjectBase,
     dataobject,
 )
 from caikit.core.data_model import enums
 from caikit.core.data_model.base import DataBase, _DataBaseMetaClass
+from caikit.core.data_model.data_backends.dict_backend import DictBackend
 from caikit.core.data_model.dataobject import (
     _AUTO_GEN_PROTO_CLASSES,
     render_dataobject_protos,
 )
+from caikit.core.data_model.json_dict import JsonDict
 from caikit.core.toolkit.isa import isprotobufenum
 
 ## Helpers #####################################################################
 
 
 @pytest.fixture(autouse=True)
 def temp_dpool():
     """Fixture to isolate the descriptor pool used in each test"""
     dpool = descriptor_pool.DescriptorPool()
     global_dpool = descriptor_pool._DEFAULT
     descriptor_pool._DEFAULT = dpool
+    fd = descriptor_pb2.FileDescriptorProto()
+    struct_pb2.DESCRIPTOR.CopyToProto(fd)
+    dpool.Add(fd)
+
+    ##
+    # HACK! Doing this _appears_ to solve the mysterious segfault cause by
+    # using Struct inside a temporary descriptor pool. The inspiration for this
+    # was:
+    #
+    # https://github.com/protocolbuffers/protobuf/issues/12047
+    #
+    # NOTE: This only works for protobuf 4.X (and as far as we know, it's not
+    #     needed for 3.X)
+    ##
+    try:
+        # Third Party
+        from google.protobuf.message_factory import GetMessageClassesForFiles
+
+        msgs = GetMessageClassesForFiles([fd.name], dpool)
+        _ = msgs["google.protobuf.Struct"]
+        _ = msgs["google.protobuf.Value"]
+        _ = msgs["google.protobuf.ListValue"]
+
+    # Nothing to do for protobuf 3.X
+    except ImportError:
+        pass
     yield dpool
     # pylint: disable=duplicate-code
     descriptor_pool._DEFAULT = global_dpool
 
 
 @pytest.fixture(autouse=True)
 def reset_global_protobuf_registry():
@@ -491,14 +519,36 @@
     json_repr_foo = foo1.to_json()
     assert json.loads(json_repr_foo) == {
         "foo_int": 2,
     }
     assert Foo.from_json(json_repr_foo) == foo1
 
 
+def test_dataobject_oneof_from_backend():
+    """Make sure that a oneof can be correctly accessed from a backend"""
+
+    @dataobject
+    class Foo(DataObjectBase):
+        foo: Union[int, str]
+
+    data_dict1 = {"fooint": 1234}
+    backend1 = DictBackend(data_dict1)
+    msg1 = Foo.from_backend(backend1)
+    assert msg1.foo == 1234
+    assert msg1.fooint == 1234
+    assert msg1.which_oneof("foo") == "fooint"
+
+    data_dict2 = {"foo": 1234}
+    backend2 = DictBackend(data_dict2)
+    msg2 = Foo.from_backend(backend2)
+    assert msg2.foo == 1234
+    assert msg2.fooint == 1234
+    assert msg2.which_oneof("foo") == "fooint"
+
+
 def test_dataobject_round_trip_json():
     """Make sure that a dataobject class can serialize to/from json"""
 
     @dataobject
     class BazObj(DataObjectBase):
         foo: str
         bar: int
@@ -723,7 +773,42 @@
         descriptor.fields_by_name["float32"].type
         == _descriptor.FieldDescriptor.TYPE_FLOAT
     )
     assert (
         descriptor.fields_by_name["float64"].type
         == _descriptor.FieldDescriptor.TYPE_DOUBLE
     )
+
+
+@pytest.mark.parametrize("run_num", range(100))
+def test_dataobject_jsondict(temp_dpool, run_num):
+    """Make sure that a JsonDict type is handled correctly in a dataobject
+
+    NOTE: This test is repeated 100x due to a strange segfault in `upb` that it
+        can trigger. The workaround above in `temp_dpool` should solve it, but
+        we retain the repetition to catch anything that's missed.
+    """
+
+    @dataobject
+    class Foo(DataObjectBase):
+        js_dict: JsonDict
+
+    # Make sure the field has the right type
+    Struct = temp_dpool.FindMessageTypeByName("google.protobuf.Struct")
+    assert Foo._proto_class.DESCRIPTOR.fields_by_name["js_dict"].message_type == Struct
+
+    # Make sure dict is preserved on init
+    js_dict = {"foo": {"bar": [1, 2, 3]}}
+    foo = Foo(js_dict)
+    assert foo.js_dict == js_dict
+
+    # Make sure conversion to struct happens on to_proto
+    foo_proto = foo.to_proto()
+    assert set(foo_proto.js_dict.fields.keys()) == set(js_dict.keys())
+    assert foo_proto.js_dict.fields["foo"].struct_value
+    assert set(foo_proto.js_dict.fields["foo"].struct_value.fields.keys()) == set(
+        js_dict["foo"].keys()
+    )
+
+    # Make sure conversion back to dict happens on from_proto
+    foo2 = Foo.from_proto(foo_proto)
+    assert foo2.js_dict == foo.js_dict
```

### Comparing `caikit-0.6.0/tests/core/data_model/test_enums.py` & `caikit-0.7.0/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/data_model/test_producer.py` & `caikit-0.7.0/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/helpers.py` & `caikit-0.7.0/tests/core/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 backend_types.register_backend_type(MockBackend)
 
 
 # Add a new shared load backend that tests can use
 class TestLoader(SharedLoadBackendBase):
     backend_type = "TESTLOADER"
+    __test__ = False
 
     def load(self, model_path: str, *args, **kwargs) -> Optional[ModuleBase]:
         # allow config.model_type to control whether this loader barfs
         if "model_type" in self.config and "model_type" in kwargs:
             if self.config["model_type"] != kwargs["model_type"]:
                 # Don't load in this loader
                 return None
```

### Comparing `caikit-0.6.0/tests/core/module_backends/test_backend_types.py` & `caikit-0.7.0/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.7.0/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/modules/test_module.py` & `caikit-0.7.0/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/modules/test_module_metadata.py` & `caikit-0.7.0/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/signature_parsing/__init__.py` & `caikit-0.7.0/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.7.0/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/signature_parsing/test_parsers.py` & `caikit-0.7.0/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/test_imports.py` & `caikit-0.7.0/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/test_model_manager.py` & `caikit-0.7.0/tests/core/test_model_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,24 +171,34 @@
         self.assertIsInstance(model, caikit.core.ModuleBase)
 
     def test_import_module_registry(self):
         """Make sure that the module registry can be imported from model_manager"""
         # pylint: disable = import-outside-toplevel,no-name-in-module,unused-import
         from caikit.core.model_manager import module_registry  # isort: skip
 
+    def test_load_model_with_no_module_id(self):
+        """Test that we can load a module with the legacy block_id instead of module_id, and that
+        a DeprecationWarning is raised.
+        """
+        model_path = os.path.join(self.fixtures_dir, DUMMY_NO_ID_MODEL_NAME)
+        with pytest.deprecated_call():
+            model = caikit.core.load(model_path)
+            self.assertIsInstance(model, caikit.core.ModuleBase)
+
 
 # Pytest tests #########################################################
 
 # Setup #########################################################################
 
 DUMMY_MODULE_ID = "foo"
 
 TEST_DATA_PATH = os.path.join("tests", "fixtures")
 DUMMY_LOCAL_MODEL_NAME = "dummy_module_foo"
 DUMMY_BACKEND_MODEL_NAME = "dummy_module_backend"
+DUMMY_NO_ID_MODEL_NAME = "dummy_module_no_id"
 CONFIG_FILE_NAME = "config.yml"
 
 
 def setup_saved_model(mock_backend_class):
     """Fixture to create and cleanup a dummy loadable model"""
 
     backend_types.register_backend_type(LocalBackend)
```

### Comparing `caikit-0.6.0/tests/core/test_no_write_permissions.py` & `caikit-0.7.0/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/test_task.py` & `caikit-0.7.0/tests/core/test_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ## Tests #######################################################################
 # Standard
+from typing import Union
 import uuid
 
 # Third Party
 import pytest
 
 # Local
 from caikit.core import TaskBase, task
@@ -36,15 +37,15 @@
             output_type=SampleOutputType,
         )
         class SampleTask:
             pass
 
 
 def test_task_decorator_validates_output_is_data_model():
-    with pytest.raises(TypeError):
+    with pytest.raises(TypeError, match=".*str.* is not a subclass"):
 
         @task(
             required_parameters={"sample_input": SampleInputType},
             output_type=str,
         )
         class SampleTask(TaskBase):
             pass
@@ -126,14 +127,51 @@
             id=str(uuid.uuid4()), name="Stuff", version="0.0.1", task=SomeTask
         )
         class Stuff(caikit.core.ModuleBase):
             def run(self, foo: int):
                 pass
 
 
+def test_task_validation_throws_on_wrong_return_type():
+    @task(
+        required_parameters={"foo": int},
+        output_type=SampleOutputType,
+    )
+    class SomeTask(TaskBase):
+        pass
+
+    with pytest.raises(
+        TypeError,
+        match="Wrong output type for module",
+    ):
+
+        @caikit.core.module(
+            id=str(uuid.uuid4()), name="Stuff", version="0.0.1", task=SomeTask
+        )
+        class Stuff(caikit.core.ModuleBase):
+            def run(self, foo: int) -> SampleInputType:
+                pass
+
+
+def test_task_validation_accepts_union_outputs():
+    @task(
+        required_parameters={"foo": int},
+        output_type=SampleOutputType,
+    )
+    class SomeTask(TaskBase):
+        pass
+
+    @caikit.core.module(
+        id=str(uuid.uuid4()), name="Stuff", version="0.0.1", task=SomeTask
+    )
+    class Stuff(caikit.core.ModuleBase):
+        def run(self, foo: int) -> Union[SampleOutputType, int, str]:
+            pass
+
+
 def test_task_validation_throws_on_missing_parameter():
     @task(
         required_parameters={"foo": int},
         output_type=SampleOutputType,
     )
     class SomeTask(TaskBase):
         pass
```

### Comparing `caikit-0.6.0/tests/core/toolkit/test_compatibility.py` & `caikit-0.7.0/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/toolkit/test_error_handler.py` & `caikit-0.7.0/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/toolkit/test_fileio.py` & `caikit-0.7.0/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.7.0/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/toolkit/test_serializers.py` & `caikit-0.7.0/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.7.0/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/data_model_helpers.py` & `caikit-0.7.0/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/config/config.yml` & `caikit-0.7.0/tests/fixtures/config/config.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Config for tests
 runtime:
     find_available_port: true
-    compiled_proto_module_dir: tests.fixtures.protobufs
 
     metering:
         # Switch on metering by default
         enabled: true
         # Directory to save metrics files
         log_dir: "test/metering_logs"
         # Write to log file every N seconds
```

### Comparing `caikit-0.6.0/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.7.0/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/dummy_module/config.yml` & `caikit-0.7.0/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.7.0/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/fixtures.py` & `caikit-0.7.0/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/invalid.zip` & `caikit-0.7.0/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/linux.txt` & `caikit-0.7.0/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/primitive_party.proto` & `caikit-0.7.0/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.7.0/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.7.0/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,11 +50,12 @@
     def train(
         cls,
         training_data: DataStream[int],
         sample_input: Union[SampleInputType, str],
         batch_size: int = 64,
     ) -> "OtherModule":
         """Sample training method that produces a trained model"""
+        assert type(sample_input) == SampleInputType or str
         # Barf if we were incorrectly passed data not in datastream format
         assert type(training_data) == DataStream
         assert batch_size > 0
         return cls(batch_size=batch_size)
```

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A hypothetical inner module that transforms some output type rather than taking domain input
 """
 # Local
 from ...data_model.sample import SampleOutputType
 import caikit.core
 
 
-@caikit.core.module("00110203-baad-beef-0809-0a0b02dd0e0f", "SampleModule", "0.0.1")
+@caikit.core.module("00110203-baad-beef-0809-0a0b02dd0e0f", "InnerModule", "0.0.1")
 class InnerModule(caikit.core.ModuleBase):
     def __init__(self, batch_size=64, learning_rate=0.0015):
         super().__init__()
         self.batch_size = batch_size
         self.learning_rate = learning_rate
 
     def run(self, some_input: SampleOutputType) -> SampleOutputType:
```

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """
 A module meant to flex a bit of the protobufs primitive support
 """
 # Standard
 from typing import List
 
 # Local
-from ...data_model.sample import SampleOutputType
+from ...data_model.sample import SampleInputType, SampleOutputType, SampleTask
 from caikit.core.modules import ModuleSaver
 import caikit.core
 
 
-@caikit.core.module("00112233-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1")
+@caikit.core.module(
+    "00112233-0405-0607-0809-0a0b02dd0e0f", "SampleModule", "0.0.1", SampleTask
+)
 class SamplePrimitiveModule(caikit.core.ModuleBase):
     def __init__(self):
         super().__init__()
 
     @classmethod
     def load(cls, model_path, **kwargs):
         return cls()
 
     def run(
         self,
+        sample_input: SampleInputType,
         bool_type: bool,
         int_type: int,
         float_type: float,
         str_type: str,
         bytes_type: bytes,
         list_type: List[str],
     ) -> SampleOutputType:
```

### Comparing `caikit-0.6.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.7.0/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/generated/__init__.py` & `caikit-0.7.0/tests/runtime/metrics/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# Standard
-import os
-import sys
-
-# Allow generated _pb2 files in here to import each other
-script_loc = os.path.dirname(os.path.realpath(__file__))
-sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.6.0/tests/runtime/metrics/__init__.py` & `caikit-0.7.0/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.7.0/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/__init__.py` & `caikit-0.7.0/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/test_batcher.py` & `caikit-0.7.0/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/test_model_loader.py` & `caikit-0.7.0/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/test_model_manager.py` & `caikit-0.7.0/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.7.0/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/model_management/test_training_manager.py` & `caikit-0.7.0/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/service_generation/test_create_service.py` & `caikit-0.7.0/tests/runtime/service_generation/test_create_service.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,39 +7,50 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# Standard
+import uuid
 
 # Local
 from caikit.runtime.service_generation.create_service import (
     create_inference_rpcs,
     create_training_rpcs,
 )
+from sample_lib.data_model import SampleInputType, SampleOutputType, SampleTask
+from sample_lib.modules import SampleModule
+import caikit
 import sample_lib
 
 ## Setup ########################################################################
 
 widget_class = sample_lib.modules.sample_task.SampleModule
-untrainable_module_class = sample_lib.modules.sample_task.SamplePrimitiveModule
 
 ## Tests ########################################################################
 
 ### create_inference_rpcs tests #################################################
 
 
-def test_create_inference_rpcs_for_module_with_no_run_function():
-    class Foo:
-        def __init__(self):
+def test_create_inference_rpcs_uses_task_from_module_decorator():
+    # make a new module with SampleTask
+    @caikit.module(
+        id=str(uuid.uuid4()), name="something", version="0.0.0", task=SampleTask
+    )
+    class NewModule(caikit.core.ModuleBase):
+        def run(self, sample_input: SampleInputType) -> SampleOutputType:
             pass
 
-    rpcs = create_inference_rpcs([Foo])
-    assert len(rpcs) == 0
+    # SampleModule also implements `SampleTask`
+    rpcs = create_inference_rpcs([NewModule, SampleModule])
+    assert len(rpcs) == 1
+    assert NewModule in rpcs[0].module_list
+    assert SampleModule in rpcs[0].module_list
 
 
 def test_create_inference_rpcs():
     rpcs = create_inference_rpcs([widget_class])
     assert len(rpcs) == 1
     assert widget_class in rpcs[0].module_list
 
@@ -48,54 +59,58 @@
     module_list = [
         sample_lib.modules.sample_task.SampleModule,
         sample_lib.modules.sample_task.SamplePrimitiveModule,
         sample_lib.modules.other_task.OtherModule,
     ]
     rpcs = create_inference_rpcs(module_list)
 
-    # only 2 RPCs, Widget and Gadget because SampleWidget and AnotherWidget are of the same module type Widget
+    # only 2 RPCs, SampleModule and SamplePrimitiveModule have task SampleTask, OtherModule has task OtherTask
     assert len(rpcs) == 2
     assert sample_lib.modules.sample_task.SampleModule in rpcs[0].module_list
     assert sample_lib.modules.sample_task.SamplePrimitiveModule in rpcs[0].module_list
     assert sample_lib.modules.other_task.OtherModule in rpcs[1].module_list
 
 
-def test_create_inference_rpcs_remove_non_primitive_modules():
-    # NOTE: This requires Gadget to be in config since other modules do not have methods - TODO fix?
+def test_create_inference_rpcs_removes_modules_with_no_task():
     module_list = [
-        sample_lib.modules.sample_task.SampleModule,  # is a primitive module
-        sample_lib.modules.sample_task.InnerModule,  # not a primitive module
+        sample_lib.modules.sample_task.SampleModule,  # has a task
+        sample_lib.modules.sample_task.InnerModule,  # does not have a task
     ]
     rpcs = create_inference_rpcs(module_list)
 
-    # only 1 RPC, fidget is not valid
     assert len(rpcs) == 1
     assert sample_lib.modules.sample_task.SampleModule in rpcs[0].module_list
+    assert sample_lib.modules.sample_task.InnerModule not in rpcs[0].module_list
 
 
 ### create_training_rpcs tests #################################################
 
 
-def test_create_inference_rpcs_for_module_with_no_train_function():
-    class Foo:
-        def __init__(self):
+def test_no_training_rpcs_module_with_no_train_function():
+    @caikit.module(
+        id=str(uuid.uuid4()), name="something", version="0.0.0", task=SampleTask
+    )
+    class Foo(caikit.core.ModuleBase):
+        def run(self, sample_input: SampleInputType) -> SampleOutputType:
             pass
 
-        def run(self):
+        def train_in_progress(self):
             pass
 
-        def train_in_progress(self):
+    rpcs = create_training_rpcs([Foo])
+    assert len(rpcs) == 0
+
+
+def test_no_training_rpcs_for_module_with_no_task():
+    @caikit.module(id=str(uuid.uuid4()), name="something", version="0.0.0")
+    class Foo(caikit.core.ModuleBase):
+        def train(self, foo: int) -> "Foo":
             pass
 
-    rpcs = create_inference_rpcs([Foo])
+    rpcs = create_training_rpcs([Foo])
     assert len(rpcs) == 0
 
 
 def test_create_training_rpcs():
     rpcs = create_training_rpcs([widget_class])
     assert len(rpcs) == 1
     assert widget_class in rpcs[0].module_list
-
-
-def test_create_training_rpcs_without_train():
-    rpcs = create_training_rpcs([untrainable_module_class])
-    assert not rpcs
```

### Comparing `caikit-0.6.0/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.7.0/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.7.0/tests/runtime/service_generation/test_rpcs.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 """Tests for the rpc objects that hold our in-memory representation of
 what an RPC for a service looks like"""
 # Standard
 import uuid
 
 # Local
 from caikit.core import ModuleBase, TaskBase
-from caikit.core.signature_parsing import CaikitMethodSignature
-from caikit.runtime.service_generation.rpcs import TaskPredictRPC
-from sample_lib.data_model import SampleOutputType, SampleTask
+from caikit.runtime.service_generation.rpcs import ModuleClassTrainRPC, TaskPredictRPC
+from sample_lib.data_model import SampleOutputType
 import caikit.core
 
 
 def test_task_inference_rpc_with_all_optional_params():
     @caikit.core.task(
         required_parameters={"str_val": str}, output_type=SampleOutputType
     )
@@ -36,14 +35,41 @@
         id=str(uuid.uuid4()), name="testest", version="9.9.9", task=TestTask
     )
     class TestModule(ModuleBase):
         def run(self, str_val="I have a default") -> SampleOutputType:
             pass
 
     rpc = TaskPredictRPC(
-        task=("foo", "bar"),
-        method_signatures=[CaikitMethodSignature(TestModule, "run")],
-        primitive_data_model_types=[],
+        task=TestTask,
+        method_signatures=[TestModule.RUN_SIGNATURE],
     )
 
     data_model = rpc.create_request_data_model(package_name="blah")
     assert data_model is not None
+
+    assert rpc.name == "TestTaskPredict"
+
+
+def test_module_train_rpc():
+    @caikit.core.task(
+        required_parameters={"str_val": str}, output_type=SampleOutputType
+    )
+    class TestTask(TaskBase):
+        pass
+
+    @caikit.core.module(
+        id=str(uuid.uuid4()), name="testest", version="9.9.9", task=TestTask
+    )
+    class TestModule(ModuleBase):
+        def run(self, str_val: str) -> SampleOutputType:
+            pass
+
+        @classmethod
+        def train(cls, int_val: int, str_val: str) -> "TestModule":
+            pass
+
+    rpc = ModuleClassTrainRPC(method_signature=TestModule.TRAIN_SIGNATURE)
+
+    data_model = rpc.create_request_data_model(package_name="blah")
+    assert data_model is not None
+
+    assert rpc.name == "TestTaskTestModuleTrain"
```

### Comparing `caikit-0.6.0/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.7.0/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/servicers/__init__.py` & `caikit-0.7.0/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.7.0/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,36 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from unittest.mock import MagicMock, patch
+
+try:
+    # Standard
+    from test.support.threading_helper import catch_threading_exception
+except (NameError, ModuleNotFoundError):
+    from tests.base import catch_threading_exception
+
+# Standard
 import json
 import os
 import tempfile
 import threading
 import time
 import uuid
 
 # Third Party
 import grpc
 import pytest
 
 # Local
 from caikit.runtime.servicers.global_predict_servicer import GlobalPredictServicer
+from caikit.runtime.types.aborted_exception import AbortedException
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from sample_lib.data_model import SampleInputType, SampleOutputType
 from sample_lib.modules.sample_task import SampleModule
 from tests.fixtures import Fixtures
 import sample_lib
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
@@ -104,24 +113,28 @@
             sample_inference_service.messages.SampleTaskRequest(
                 sample_input=HAPPY_PATH_INPUT
             ),
             context,
         ),
     )
 
-    # Patch in the mock manager and start the prediction
-    with patch.object(sample_predict_servicer, "_model_manager", mock_manager):
-        predict_thread.start()
-        dummy_model.started.wait()
-        # Simulate a timeout or client abort
-        context.cancel()
-        predict_thread.join(10)
+    with catch_threading_exception() as cm:
+        # Patch in the mock manager and start the prediction
+        with patch.object(sample_predict_servicer, "_model_manager", mock_manager):
+            predict_thread.start()
+            dummy_model.started.wait()
+            # Simulate a timeout or client abort
+            context.cancel()
+            predict_thread.join(10)
+
+        # Make sure the prediction actually stopped
+        assert not predict_thread.is_alive()
 
-    # Make sure the prediction actually stopped
-    assert not predict_thread.is_alive()
+        # Make sure the correct exception was raised
+        assert cm.exc_type == AbortedException
 
 
 def test_metering_ignore_unsuccessful_calls(
     sample_inference_service, sample_predict_servicer, loaded_model_id
 ):
     with patch.object(
         sample_predict_servicer.rpc_meter, "update_metrics"
```

### Comparing `caikit-0.6.0/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.7.0/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from tempfile import TemporaryDirectory
+from unittest.mock import patch
+import multiprocessing
+import threading
 import time
 import uuid
 
 # Third Party
 import pytest
 
 # Local
@@ -83,24 +86,25 @@
     require any loaded model
     """
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
     model_name = random_test_id()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=model_name,
-            batch_size=42,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=model_name,
+        batch_size=42,
+        training_data=training_data,
     )
 
-    training_response = sample_train_servicer.Train(train_request)
+    training_response = sample_train_servicer.Train(
+        train_request, Fixtures.build_context("foo")
+    )
     assert training_response.model_name == model_name
+
     assert training_response.training_id is not None
     assert isinstance(training_response.training_id, str)
 
     result = sample_train_servicer.training_map.get(
         training_response.training_id
     ).result()
     assert result.batch_size == 42
@@ -136,25 +140,29 @@
     """Global train of TrainRequest returns a training job with the correct
     model name, and some training id for a basic train function that doesn't
     require any loaded model
     """
     batch_size = 42
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(jsondata=stream_type.JsonData(data=[1])).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
-            model_name="Other module Training",
-            training_data=training_data,
-            sample_input=SampleInputType(name="Gabe").to_proto(),
-            batch_size=batch_size,
-        )
+    train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
+        model_name="Other module Training",
+        training_data=training_data,
+        # either of the below lines work since it's a Union now
+        # TODO create a separate test, lazy
+        # sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        sample_inputstr="sample",
+        batch_size=batch_size,
     )
 
-    training_response = sample_train_servicer.Train(train_request)
+    training_response = sample_train_servicer.Train(
+        train_request, Fixtures.build_context("foo")
+    )
     assert training_response.model_name == "Other module Training"
+
     assert training_response.training_id is not None
     assert isinstance(training_response.training_id, str)
 
     result = sample_train_servicer.training_map.get(
         training_response.training_id
     ).result()
     assert result.batch_size == batch_size
@@ -165,15 +173,15 @@
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     inference_response = sample_predict_servicer.Predict(
         sample_inference_service.messages.OtherTaskRequest(
-            sample_input=SampleInputType(name="Gabe").to_proto()
+            sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto()
         ),
         Fixtures.build_context(training_response.model_name),
     )
     assert (
         inference_response
         == OtherOutputType(
             farewell=f"goodbye: Gabe {batch_size} times",
@@ -190,21 +198,23 @@
 ):
     """Global train of TrainRequest returns a training job with the correct model name, and some training id for a train function that requires another loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=loaded_model_id
     ).to_proto()
 
     training_request = (
-        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
+        sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
             model_name="AnotherWidget_Training",
             sample_block=sample_model,
         )
     )
 
-    training_response = sample_train_servicer.Train(training_request)
+    training_response = sample_train_servicer.Train(
+        training_request, Fixtures.build_context("foo")
+    )
 
     assert training_response.model_name == "AnotherWidget_Training"
     assert training_response.training_id is not None
     assert isinstance(training_response.training_id, str)
 
     training_result = sample_train_servicer.training_map.get(
         training_response.training_id
@@ -238,28 +248,27 @@
     sample_train_service, sample_inference_service, sample_predict_servicer
 ):
     """Check if run_train_job works as expected for syncronous requests"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(),
-            batch_size=42,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(),
+        batch_size=42,
+        training_data=training_data,
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
             SampleModule,
             training_id="dummy-training-id",
             training_output_dir=tmp_dir,
+            context=Fixtures.build_context("foo"),
             wait=True,
         )
 
         assert training_response.training_id == "dummy-training-id"
 
         inference_response = sample_predict_servicer.Predict(
             sample_inference_service.messages.SampleTaskRequest(
@@ -277,60 +286,58 @@
 
 def test_run_train_job_works_with_no_autoload(sample_train_service):
     """Check if run_train_job works with no auto-load doesn't load model"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=str(uuid.uuid4()),
-            batch_size=42,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=str(uuid.uuid4()),
+        batch_size=42,
+        training_data=training_data,
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     servicer.auto_load_trained_model = False
     init_loaded_models_count = len(servicer._model_manager.loaded_models)
 
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
             SampleModule,
             training_id="dummy-training-id",
             training_output_dir=tmp_dir,
+            context=Fixtures.build_context("foo"),
             wait=True,
         )
         assert training_response.training_id == "dummy-training-id"
         assert init_loaded_models_count == len(servicer._model_manager.loaded_models)
 
 
 def test_run_train_job_works_with_autoload(sample_train_service):
     """Check if run_train_job works with auto-load loading the model"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=str(uuid.uuid4()),
-            batch_size=42,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=str(uuid.uuid4()),
+        batch_size=42,
+        training_data=training_data,
     )
     servicer = GlobalTrainServicer(training_service=sample_train_service)
     servicer.auto_load_trained_model = True
     init_loaded_models_count = len(servicer._model_manager.loaded_models)
 
     with TemporaryDirectory() as tmp_dir:
         training_response = servicer.run_training_job(
             train_request,
             SampleModule,
             training_id="dummy-training-id-2",
             training_output_dir=tmp_dir,
+            context=Fixtures.build_context("foo"),
             wait=True,
         )
         assert training_response.training_id == "dummy-training-id-2"
         assert init_loaded_models_count < len(servicer._model_manager.loaded_models)
 
 
 #############
@@ -343,44 +350,43 @@
 ):
     """Global train of TrainRequest raises when calling a train function that requires another loaded model, but model is not loaded"""
     model_id = random_test_id()
 
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=model_id
     ).to_proto()
-    request = (
-        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
-            model_name="AnotherWidget_Training",
-            sample_block=sample_model,
-        )
+    request = sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
+        model_name="AnotherWidget_Training",
+        sample_block=sample_model,
     )
 
     with pytest.raises(CaikitRuntimeException) as context:
-        sample_train_servicer.Train(request)
+        sample_train_servicer.Train(request, Fixtures.build_context("foo"))
 
     assert f"Model '{model_id}' not loaded" == context.value.message
 
 
-def test_global_train_Edge_Case_Widget_should_raise_when_error_surfaces_from_block(
+def test_global_train_Edge_Case_Widget_should_raise_when_error_surfaces_from_module(
     sample_train_service, sample_train_servicer
 ):
     """Test that if a module raises a ValueError, we should surface it to the user in a helpful way"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(),
-            batch_size=999,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(),
+        batch_size=999,
+        training_data=training_data,
     )
+
     with pytest.raises(CaikitRuntimeException) as context:
-        training_response = sample_train_servicer.Train(train_request)
+        training_response = sample_train_servicer.Train(
+            train_request, Fixtures.build_context("foo")
+        )
 
         training_result = sample_train_servicer.training_map.get(
             training_response.training_id
         ).result()
 
     assert f"This may be a problem with your input" in str(context.value.message)
 
@@ -389,60 +395,98 @@
     sample_train_service, sample_train_servicer
 ):
     """Test that if module goes into OOM we are able to surface error code"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(),
-            batch_size=42,
-            training_data=training_data,
-            oom_exit=True,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(),
+        batch_size=42,
+        training_data=training_data,
+        oom_exit=True,
     )
 
     # Enable sub-processing for test
     sample_train_servicer.use_subprocess = True
 
     with pytest.raises(CaikitRuntimeException) as context:
-        training_response = sample_train_servicer.Train(train_request)
+        training_response = sample_train_servicer.Train(
+            train_request, Fixtures.build_context("foo")
+        )
         sample_train_servicer.training_map.get(training_response.training_id).result()
 
     assert f"Training process died with OOM error!" in str(context.value.message)
 
 
 #####################################################################
 
-# NOTE: This test was commented out in the original unittest.TestCase impl - leaving as is
-# def test_global_train_aborts_long_running_trains(self):
-#     mock_manager = MagicMock()
-
-#     # return a dummy model from the mock model manager
-#     class UnresponsiveModel:
-#         started = threading.Event()
-
-#         def run(self, *args, **kwargs):
-#             self.started.set()
-#             while True:
-#                 time.sleep(0.01)
-
-#     dummy_model = UnresponsiveModel()
-#     mock_manager.retrieve_model.return_value = dummy_model
-
-#     context = Fixtures.build_context("test-any-unresponsive-model")
-#     train_thread = threading.Thread(
-#         target=self.train_servicer.Train,
-#         args=(self.HAPPY_PATH_FAKE_BLOCK_REQUEST, context),
-#     )
-
-#     # Patch in the mock manager and start the training
-#     with patch.object(self.train_servicer, "_model_manager", mock_manager):
-#         train_thread.start()
-#         dummy_model.started.wait()
-#         # Simulate a timeout or client abort
-#         context.cancel()
-#         train_thread.join(10)
 
-#     # Make sure the training job actually stopped
-#     self.assertFalse(train_thread.is_alive())
+def test_global_train_aborts_long_running_trains(
+    sample_train_service, sample_train_servicer
+):
+    stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
+    training_data = stream_type(
+        jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
+    ).to_proto()
+    training_id = random_test_id()
+
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=training_id,
+        batch_size=42,
+        training_data=training_data,
+        oom_exit=False,
+    )
+
+    # sample_train_servicer.use_subprocess = True
+    if sample_train_servicer.use_subprocess:
+        test_event = multiprocessing.Event()
+    else:
+        test_event = threading.Event()
+
+    def never_respond(*args, **kwargs):
+        """Never ending function"""
+        test_event.set()
+        while True:
+            time.sleep(0.01)
+
+    context = Fixtures.build_context("test-any-unresponsive-model")
+
+    servicer = GlobalTrainServicer(training_service=sample_train_service)
+
+    with TemporaryDirectory() as tmp_dir:
+        training_id = "dummy-training-id"
+        training_output_dir = tmp_dir
+        context = Fixtures.build_context("foo")
+
+        train_thread = threading.Thread(
+            target=servicer.run_training_job,
+            args=(
+                train_request,
+                SampleModule,
+                training_id,
+                training_output_dir,
+                context,
+            ),
+            kwargs={
+                "wait": True,
+            },
+        )
+
+    # NOTE: We are configuring following timeout
+    # to avoid tests from hanging
+    request_timeout = 10
+    test_event_timeout = 20
+    with patch(
+        f"{SampleModule.__module__}.{SampleModule.train.__qualname__}",
+        never_respond,
+    ):
+
+        train_thread.start()
+        test_event.wait(test_event_timeout)
+
+        # Simulate a timeout or client abort
+        context.cancel()
+        train_thread.join(request_timeout)
+
+    # Make sure the training job actually stopped
+    assert not train_thread.is_alive()
```

### Comparing `caikit-0.6.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.7.0/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,30 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 from threading import Event, Thread
 from unittest.mock import MagicMock, patch
+
+try:
+    # Standard
+    from test.support.threading_helper import catch_threading_exception
+except (NameError, ModuleNotFoundError):
+    from tests.base import catch_threading_exception
+
+# Standard
 import time
 import unittest
 
 # Local
 from caikit import get_config
 from caikit.runtime.protobufs import model_runtime_pb2
 from caikit.runtime.servicers.model_runtime_servicer import ModelRuntimeServicerImpl
+from caikit.runtime.types.aborted_exception import AbortedException
 from tests.fixtures import Fixtures
 
 
 class TestModelRuntimeServicerImpl(unittest.TestCase):
     """This test suite tests the ModelRuntimeServicerImpl class"""
 
     def setUp(self):
@@ -85,14 +94,18 @@
             started.set()
             while True:
                 time.sleep(0.01)
 
         mock_manager.load_model.side_effect = never_return
         load_thread = Thread(target=self.servicer.loadModel, args=(request, context))
 
-        with patch.object(self.servicer, "model_manager", mock_manager):
-            load_thread.start()
-            started.wait()
-            context.cancel()
-            load_thread.join(10)
+        with catch_threading_exception() as cm:
+            with patch.object(self.servicer, "model_manager", mock_manager):
+                load_thread.start()
+                started.wait()
+                context.cancel()
+                load_thread.join(10)
+
+            self.assertFalse(load_thread.is_alive())
 
-        self.assertFalse(load_thread.is_alive())
+            # Make sure the correct exception was raised
+            assert cm.exc_type == AbortedException
```

### Comparing `caikit-0.6.0/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.7.0/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # Local
 from caikit.interfaces.runtime.data_model import TrainingStatus
 from caikit.runtime.protobufs import process_pb2
 from caikit.runtime.servicers.model_train_servicer import ModelTrainServicerImpl
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from tests.conftest import temp_config
+from tests.fixtures import Fixtures
 import sample_lib
 
 
 @pytest.fixture
 def sample_model_train_servicer(sample_train_service) -> ModelTrainServicerImpl:
     servicer = ModelTrainServicerImpl(training_service=sample_train_service)
     yield servicer
@@ -75,30 +76,32 @@
         request_dict={
             "train_module": "00110203-0405-0607-0809-0a0b02dd0e0f",
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join(output_dir, training_id),
     )
     with pytest.raises(CaikitRuntimeException):
-        sample_model_train_servicer.Run(model_train_request)
+        context = Fixtures.build_context("foo")
+        sample_model_train_servicer.Run(model_train_request, context)
 
 
 def test_model_train_no_train_module_raises(sample_model_train_servicer, output_dir):
     training_id = str(uuid.uuid4())
     model_train_request = process_pb2.ProcessRequest(
         trainingID=training_id,
         customTrainingID=str(uuid.uuid4()),
         request_dict={
             "training_params": '{"model_name": "abc", "training_data": [1]}',
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join(output_dir, training_id),
     )
     with pytest.raises(CaikitRuntimeException):
-        sample_model_train_servicer.Run(model_train_request)
+        context = Fixtures.build_context("foo")
+        sample_model_train_servicer.Run(model_train_request, context)
 
 
 def test_model_train_incorrect_train_params_raises(
     sample_model_train_servicer, output_dir
 ):
     training_id = str(uuid.uuid4())
     model_train_request = process_pb2.ProcessRequest(
@@ -108,15 +111,16 @@
             "train_module": "00110203-0405-0607-0809-0a0b02dd0e0f",
             "training_params": '{"model_name": "abc", "training_data": "blah"}',
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join(output_dir, training_id),
     )
     with pytest.raises(CaikitRuntimeException):
-        sample_model_train_servicer.Run(model_train_request)
+        context = Fixtures.build_context("foo")
+        sample_model_train_servicer.Run(model_train_request, context)
 
 
 def test_model_train_incorrect_train_module_raises(
     sample_model_train_servicer, output_dir
 ):
     training_id = str(uuid.uuid4())
     model_train_request = process_pb2.ProcessRequest(
@@ -125,15 +129,17 @@
         request_dict={
             "train_module": "random_id",
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join(output_dir, training_id),
     )
     with pytest.raises(CaikitRuntimeException) as e:
-        sample_model_train_servicer.Run(model_train_request)
+        context = Fixtures.build_context("foo")
+        sample_model_train_servicer.Run(model_train_request, context)
+
     assert "Model Train not able to parse module for this Train Request" in str(e.value)
     assert e.value.status_code == grpc.StatusCode.INVALID_ARGUMENT
 
 
 def test_model_train_incorrect_train_request_raises(
     sample_model_train_servicer, output_dir
 ):
@@ -146,15 +152,17 @@
             "training_params": '{"model_name": "abc", "training_data": [1]}',
         },
         training_input_dir="training_input_dir",
         training_output_dir=os.path.join(output_dir, training_id),
     )
     with clear_messages_from_servicer(sample_model_train_servicer):
         with pytest.raises(CaikitRuntimeException) as e:
-            sample_model_train_servicer.Run(model_train_request)
+            context = Fixtures.build_context("foo")
+            sample_model_train_servicer.Run(model_train_request, context)
+
         assert "Model Train not able to create a request" in str(e.value)
         assert e.value.status_code == grpc.StatusCode.INTERNAL
 
 
 #####################################################################
 # Normal tests
 def test_model_train_sample_widget(sample_model_train_servicer, output_dir):
@@ -180,15 +188,16 @@
                     },
                 }
             ),
         },
         training_input_dir="training_input_dir",
         training_output_dir=training_output_dir,
     )
-    training_response = sample_model_train_servicer.Run(model_train_request)
+    context = Fixtures.build_context("test-any-unresponsive-model")
+    training_response = sample_model_train_servicer.Run(model_train_request, context)
     assert os.path.isdir(training_output_dir)
 
     # Make sure that the request completed synchronously
     assert (
         sample_model_train_servicer._gts.training_manager.get_training_status(
             training_id
         )
```

### Comparing `caikit-0.6.0/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.7.0/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/test_grpc_server.py` & `caikit-0.7.0/tests/runtime/test_grpc_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,34 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 # Have pylint ignore Class XXXX has no YYYY member so that we can use gRPC enums.
 # pylint: disable=E1101
 # Standard
+from contextlib import contextmanager
 from dataclasses import dataclass
 from unittest import mock
 import json
 import os
 import threading
 import time
 import uuid
 
 # Third Party
+from google.protobuf.descriptor_pool import DescriptorPool
+from grpc._utilities import RpcMethodHandler
 from grpc_health.v1 import health_pb2, health_pb2_grpc
+from grpc_reflection.v1alpha.proto_reflection_descriptor_database import (
+    ProtoReflectionDescriptorDatabase,
+)
 import grpc
 import pytest
 import tls_test_tools
 
 # First Party
 import alog
 
@@ -51,19 +58,21 @@
 from caikit.runtime.service_factory import ServicePackage, ServicePackageFactory
 from sample_lib.data_model import (
     OtherOutputType,
     SampleInputType,
     SampleOutputType,
     SampleTrainingType,
 )
-from tests.conftest import random_test_id, temp_config
+from tests.conftest import random_test_id, runtime_grpc_test_server, temp_config
 from tests.fixtures import Fixtures
 import caikit
 import sample_lib
 
+## Helpers #####################################################################
+
 log = alog.use_channel("TEST-SERVE-I")
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 HAPPY_PATH_TRAIN_RESPONSE = TrainingJob(
     model_name="dummy name", training_id="dummy id"
 ).to_proto()
@@ -72,14 +81,17 @@
 def is_good_train_response(actual_response, expected, model_name):
     assert dir(actual_response) == dir(expected)
     assert actual_response.training_id is not None
     assert isinstance(actual_response.training_id, str)
     assert actual_response.model_name == model_name
 
 
+## Tests #######################################################################
+
+
 def test_model_train(runtime_grpc_server):
     """Test model train's RUN function"""
     model_train_stub = process_pb2_grpc.ProcessStub(
         runtime_grpc_server.make_local_channel()
     )
     training_id = str(uuid.uuid4())
     model_train_request = process_pb2.ProcessRequest(
@@ -99,15 +111,17 @@
                             ]
                         },
                     },
                 }
             ),
         },
         training_input_dir="training_input_dir",
-        training_output_dir=os.path.join("test", "training_output", training_id),
+        training_output_dir=os.path.join(
+            runtime_grpc_server.workdir, "training_output", training_id
+        ),
     )
     training_response = model_train_stub.Run(model_train_request)
     assert isinstance(training_response, process_pb2.ProcessResponse)
     assert training_response == process_pb2.ProcessResponse(
         trainingID=model_train_request.trainingID,
         customTrainingID=model_train_request.customTrainingID,
     )
@@ -116,15 +130,14 @@
 
     # construct training request for training manager
     training_info_request = TrainingInfoRequest(training_id=training_id).to_proto()
 
     training_management_service: ServicePackage = (
         ServicePackageFactory().get_service_package(
             ServicePackageFactory.ServiceType.TRAINING_MANAGEMENT,
-            ServicePackageFactory.ServiceSource.GENERATED,
         )
     )
 
     training_management_stub = training_management_service.stub_class(
         runtime_grpc_server.make_local_channel()
     )
 
@@ -180,28 +193,29 @@
 ####### End-to-end tests for train a model and then predict with it
 def test_train_fake_module_ok_response_and_can_predict_with_trained_model(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
 ):
-    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrain successful response"""
+    """Test RPC CaikitRuntime.SampleTaskSampleModuleTrain successful response"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
     ).to_proto()
     model_name = random_test_id()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=model_name, training_data=training_data
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=model_name,
+        training_data=training_data,
     )
-    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
+
+    actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
+
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -222,20 +236,18 @@
     sample_inference_service,
 ):
     """Test RPC CaikitRuntime.WorkflowsSampleTaskSampleWorkflowTrain successful response with a loaded model"""
     sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
         model_id=loaded_model_id
     ).to_proto()
     model_name = random_test_id()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
-            model_name=model_name, sample_block=sample_model
-        )
+    train_request = sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
+        model_name=model_name, sample_block=sample_model
     )
-    actual_response = train_stub.ModulesSampleTaskCompositeModuleTrain(train_request)
+    actual_response = train_stub.SampleTaskCompositeModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -262,29 +274,30 @@
 
     # Train an OtherModule with batch size 100
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         file=stream_type.File(filename=sample_int_file)
     ).to_proto()
 
-    train_request = (
-        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
-            model_name="Bar Training", batch_size=100, training_data=training_data
-        )
+    train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
+        model_name="Bar Training",
+        sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        batch_size=100,
+        training_data=training_data,
     )
-    actual_response = train_stub.ModulesOtherTaskOtherModuleTrain(train_request)
+    actual_response = train_stub.OtherTaskOtherModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, "Bar Training")
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference, and the batch size 100 was used
     predict_request = sample_inference_service.messages.OtherTaskRequest(
-        sample_input=HAPPY_PATH_INPUT
+        sample_inputsampleinputtype=HAPPY_PATH_INPUT
     )
     trained_inference_response = inference_stub.OtherTaskPredict(
         predict_request, metadata=[("mm-model-id", actual_response.model_name)]
     )
     expected_trained_inference_response = OtherOutputType(
         farewell="goodbye: Gabe 100 times"
     ).to_proto()
@@ -300,31 +313,29 @@
     assert original_inference_response == expected_original_inference_response
 
 
 ##### Test different datastream types #####
 def test_train_fake_module_ok_response_with_datastream_jsondata(
     train_stub, inference_stub, sample_train_service, sample_inference_service
 ):
-    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrainRequest successful response with training data json type"""
+    """Test RPC CaikitRuntime.SampleTaskSampleModuleTrainRequest successful response with training data json type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(
             data=[SampleTrainingType(1), SampleTrainingType(2)]
         )
     ).to_proto()
     model_name = random_test_id()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=model_name,
-            batch_size=42,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=model_name,
+        batch_size=42,
+        training_data=training_data,
     )
 
-    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
+    actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -340,28 +351,26 @@
 def test_train_fake_module_ok_response_with_datastream_csv_file(
     train_stub,
     inference_stub,
     sample_train_service,
     sample_inference_service,
     sample_csv_file,
 ):
-    """Test RPC CaikitRuntime.ModulesSampleTaskSampleModuleTrainRequest successful response with training data file type"""
+    """Test RPC CaikitRuntime.SampleTaskSampleModuleTrainRequest successful response with training data file type"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         file=stream_type.File(filename=sample_csv_file)
     ).to_proto()
     model_name = random_test_id()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=model_name,
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=model_name,
+        training_data=training_data,
     )
 
-    actual_response = train_stub.ModulesSampleTaskSampleModuleTrain(train_request)
+    actual_response = train_stub.SampleTaskSampleModuleTrain(train_request)
     is_good_train_response(actual_response, HAPPY_PATH_TRAIN_RESPONSE, model_name)
 
     # give the trained model time to load
     # TODO: no sleeps in tests!
     time.sleep(1)
 
     # make sure the trained model can run inference
@@ -374,26 +383,26 @@
     assert inference_response == HAPPY_PATH_RESPONSE
 
 
 #### Error cases for train tests #####
 def test_train_fake_module_error_response_with_unloaded_model(
     train_stub, sample_train_service
 ):
-    """Test RPC CaikitRuntime.WorkflowsSampleTaskSampleWorkflowTrain error response because sample model is not loaded"""
+    """Test RPC CaikitRuntime.SampleTaskCompositeModuleTrain error response because sample model is not loaded"""
     with pytest.raises(grpc.RpcError) as context:
         sample_model = caikit.interfaces.runtime.data_model.ModelPointer(
             model_id=random_test_id()
         ).to_proto()
 
         train_request = (
-            sample_train_service.messages.ModulesSampleTaskCompositeModuleTrainRequest(
+            sample_train_service.messages.SampleTaskCompositeModuleTrainRequest(
                 model_name=random_test_id(), sample_block=sample_model
             )
         )
-        train_stub.ModulesSampleTaskCompositeModuleTrain(train_request)
+        train_stub.SampleTaskCompositeModuleTrain(train_request)
     assert context.value.code() == grpc.StatusCode.NOT_FOUND
 
 
 #### ModelRuntime tests ####
 def test_load_model_ok_response(runtime_grpc_server):
     """Test load model's successful response"""
     stub = model_runtime_pb2_grpc.ModelRuntimeStub(
@@ -624,15 +633,15 @@
     ca_key = tls_test_tools.generate_key()[0]
     ca_cert = tls_test_tools.generate_ca_cert(ca_key)
     tls_key, tls_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert, key=tls_key), client=KeyPair(cert="", key="")
     )
-    with RuntimeGRPCServer(
+    with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=None,
         tls_config_override=tls_config,
     ) as server:
         _assert_connection(_make_secure_channel(server, ca_cert))
 
 
@@ -641,15 +650,15 @@
     ca_key = tls_test_tools.generate_key()[0]
     ca_cert = tls_test_tools.generate_ca_cert(ca_key)
     tls_key, tls_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert, key=tls_key), client=KeyPair(cert=ca_cert, key="")
     )
-    with RuntimeGRPCServer(
+    with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=None,
         tls_config_override=tls_config,
     ) as server:
         client_key, client_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
         _assert_connection(
             _make_secure_channel(server, ca_cert, client_key, client_cert)
@@ -681,15 +690,15 @@
     with open(ca_cert_path, "w") as f:
         f.write(ca_cert)
 
     tls_config = TLSConfig(
         server=KeyPair(cert=tls_cert_path, key=tls_key_path),
         client=KeyPair(cert=ca_cert_path, key=""),
     )
-    with RuntimeGRPCServer(
+    with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=None,
         tls_config_override=tls_config,
     ) as server:
         client_key, client_cert = tls_test_tools.generate_derived_key_cert_pair(ca_key)
         _assert_connection(
             _make_secure_channel(server, ca_cert, client_key, client_cert)
@@ -697,15 +706,15 @@
 
 
 def test_metrics_stored_after_server_interrupt(
     loaded_model_id, sample_inference_service
 ):
     """This tests the gRPC server's behaviour when interrupted"""
 
-    with RuntimeGRPCServer(
+    with runtime_grpc_test_server(
         inference_service=sample_inference_service,
         training_service=None,
     ) as server:
         stub = sample_inference_service.stub_class(server.make_local_channel())
         predict_request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT
         )
@@ -744,21 +753,88 @@
             "runtime": {
                 "port": free_high_port,
                 "find_available_port": False,
             }
         },
         merge_strategy="merge",
     ):
-        with RuntimeGRPCServer(
+        with runtime_grpc_test_server(
             inference_service=sample_inference_service,
             training_service=None,
         ) as server:
             _assert_connection(grpc.insecure_channel(f"localhost:{free_high_port}"))
 
 
+def test_reflection_enabled(runtime_grpc_server):
+    """This pings the reflection API to ensure we can list the caikit services that are running"""
+    # See https://github.com/grpc/grpc/blob/master/doc/python/server_reflection.md
+    channel = runtime_grpc_server.make_local_channel()
+    reflection_db = ProtoReflectionDescriptorDatabase(channel)
+
+    desc_pool = DescriptorPool(reflection_db)
+    service_desc = desc_pool.FindServiceByName(
+        "caikit.runtime.SampleLib.SampleLibService"
+    )
+    method_desc = service_desc.FindMethodByName("SampleTaskPredict")
+    assert method_desc is not None
+
+
+def test_streaming_responses_work(runtime_grpc_server):
+    """This test uses the health check's Watch rpc to ensure that a unary->stream RPC functions
+    as expected."""
+    stub = health_pb2_grpc.HealthStub(runtime_grpc_server.make_local_channel())
+    req = health_pb2.HealthCheckRequest()
+    for response in stub.Watch(req):
+        assert response is not None
+        break
+
+
+def test_streaming_handlers_are_built_correctly(runtime_grpc_server):
+    """This is a very cheat-y test of a private method to check that we build our internal
+    handlers using the correct handler function"""
+
+    class FakeHandler:
+        pass
+
+    # NB: the unary_stream case is tested via health check watch in `test_streaming_responses_work`
+    # (unary_unary cases are checked in every other test)
+
+    stream_unary_handler = RpcMethodHandler(
+        request_streaming=True,
+        response_streaming=False,
+        request_deserializer="foo",
+        response_serializer="bar",
+        unary_unary=None,
+        stream_unary=FakeHandler,
+        unary_stream=None,
+        stream_stream=None,
+    )
+    new_handler = runtime_grpc_server.server._make_new_handler(
+        stream_unary_handler, replace_with_global_predict=False
+    )
+    assert new_handler.stream_unary is not None
+    assert new_handler.stream_unary.__name__ == "safe_rpc_call"
+
+    stream_stream_handler = RpcMethodHandler(
+        request_streaming=True,
+        response_streaming=True,
+        request_deserializer="foo",
+        response_serializer="bar",
+        unary_unary=None,
+        stream_unary=None,
+        unary_stream=None,
+        stream_stream=FakeHandler,
+    )
+    new_handler = runtime_grpc_server.server._make_new_handler(
+        stream_stream_handler, replace_with_global_predict=False
+    )
+    assert new_handler.stream_stream is not None
+    assert new_handler.stream_stream.__name__ == "safe_rpc_call"
+
+
 # Test implementation details #########################
 @dataclass
 class KeyPair:
     cert: str
     key: str
```

### Comparing `caikit-0.6.0/tests/runtime/utils/__init__.py` & `caikit-0.7.0/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/utils/test_import_util.py` & `caikit-0.7.0/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/utils/test_servicer_util.py` & `caikit-0.7.0/tests/runtime/utils/test_servicer_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,18 +338,16 @@
 
 
 def test_global_train_build_caikit_library_request_dict_creates_caikit_core_run_kwargs_not_fail_when_optional_proto_field_not_exist(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict creates module run kwargs from RPC msg
     and if not passed in request, it creates the fields with default values"""
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id()  # not having batch_size, and training_data
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id()  # not having batch_size, and training_data
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.sample_task.SampleModule().train,
     )
 
@@ -368,18 +366,16 @@
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict strips empty list from request"""
     # NOTE: not sure this test is relevant anymore, since nothing effectively gets removed?
     # the datastream is empty but it's not removed from request, which is expected
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(jsondata=stream_type.JsonData(data=[])).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(), training_data=training_data
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(), training_data=training_data
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.sample_task.SampleModule().train,
     )
 
@@ -392,20 +388,18 @@
 def test_global_train_build_caikit_library_request_dict_works_for_repeated_fields(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict works for repeated fields"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(jsondata=stream_type.JsonData(data=[])).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskListModuleTrainRequest(
-            model_name=random_test_id(),
-            training_data=training_data,
-            poison_pills=["Bob Marley", "Bunny Livingston"],
-        )
+    train_request = sample_train_service.messages.SampleTaskListModuleTrainRequest(
+        model_name=random_test_id(),
+        training_data=training_data,
+        poison_pills=["Bob Marley", "Bunny Livingston"],
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.sample_task.ListModule().train,
     )
 
@@ -422,18 +416,19 @@
     sample_train_service,
 ):
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceInt
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[100, 120])
     ).to_proto()
 
-    train_request = (
-        sample_train_service.messages.ModulesOtherTaskOtherModuleTrainRequest(
-            model_name="Bar Training", batch_size=100, training_data=training_data
-        )
+    train_request = sample_train_service.messages.OtherTaskOtherModuleTrainRequest(
+        model_name="Bar Training",
+        sample_inputsampleinputtype=SampleInputType(name="Gabe").to_proto(),
+        batch_size=100,
+        training_data=training_data,
     )
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.other_task.OtherModule().train,
     )
 
     expected_arguments = set(
@@ -449,19 +444,17 @@
 ):
     """Global train build_caikit_library_request_dict works for csv training data file"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         file=stream_type.File(filename=sample_csv_file)
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(),
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(),
+        training_data=training_data,
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.sample_task.SampleModule().train,
     )
 
@@ -475,20 +468,18 @@
     sample_train_service, sample_csv_file, sample_json_file
 ):
     """Global train build_caikit_library_request_dict works for list of data files"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         listoffiles=stream_type.ListOfFiles(files=[sample_csv_file, sample_json_file])
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskListModuleTrainRequest(
-            model_name=random_test_id(),
-            training_data=training_data,
-            poison_pills=["Bob Marley", "Bunny Livingston"],
-        )
+    train_request = sample_train_service.messages.SampleTaskListModuleTrainRequest(
+        model_name=random_test_id(),
+        training_data=training_data,
+        poison_pills=["Bob Marley", "Bunny Livingston"],
     )
 
     caikit.core_request = build_caikit_library_request_dict(
         train_request,
         sample_lib.modules.sample_task.ListModule().train,
     )
 
@@ -516,15 +507,15 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="json")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
+            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         # no error because at least 1 json file exists within the provided dir
         caikit.core_request = build_caikit_library_request_dict(
@@ -539,19 +530,17 @@
 def test_build_caikit_library_request_dict_raises_invalid_data_stream_source_file(
     sample_train_service,
 ):
     """Global train build_caikit_library_request_dict works for repeated fields"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(file=stream_type.File(filename="abc.blah")).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name=random_test_id(),
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name=random_test_id(),
+        training_data=training_data,
     )
 
     with pytest.raises(CaikitRuntimeException) as e:
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
             sample_lib.modules.sample_task.SampleModule().train,
         )
@@ -568,15 +557,15 @@
         handle.flush()
         fname = handle.name
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(file=stream_type.File(filename=fname)).to_proto()
         train_request = (
-            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
+            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
                 model_name="Foo Bar Training",
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
@@ -592,19 +581,17 @@
 ):
     """Global train build_caikit_library_request_dict raises for a file passed as directory"""
 
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         directory=stream_type.Directory(dirname=sample_csv_file)
     ).to_proto()
-    train_request = (
-        sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
-            model_name="Foo Bar Training",
-            training_data=training_data,
-        )
+    train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
+        model_name="Foo Bar Training",
+        training_data=training_data,
     )
 
     with pytest.raises(CaikitRuntimeException) as e:
         caikit.core_request = build_caikit_library_request_dict(
             train_request,
             sample_lib.modules.sample_task.SampleModule().train,
         )
@@ -625,15 +612,15 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="txt")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
+            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
@@ -658,15 +645,15 @@
         stream_type = (
             caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
         )
         training_data = stream_type(
             directory=stream_type.Directory(dirname=tempdir, extension="json")
         ).to_proto()
         train_request = (
-            sample_train_service.messages.ModulesSampleTaskSampleModuleTrainRequest(
+            sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
                 model_name=random_test_id(),
                 training_data=training_data,
             )
         )
 
         with pytest.raises(CaikitRuntimeException) as e:
             caikit.core_request = build_caikit_library_request_dict(
```

### Comparing `caikit-0.6.0/tests/runtime/work_management/__init__.py` & `caikit-0.7.0/examples/text-sentiment/text_sentiment/config.yml`

 * *Files 15% similar despite different names*

```diff
@@ -7,7 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+runtime:
+    library: text_sentiment
```

### Comparing `caikit-0.6.0/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.7.0/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.7.0/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.6.0/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.7.0/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
+try:
+    # Standard
+    from test.support.threading_helper import catch_threading_exception
+except (NameError, ModuleNotFoundError):
+    from tests.base import catch_threading_exception
+
+# Standard
 import threading
 import time
 import unittest
 
 # Local
+from caikit.runtime.types.thread_destroyed_exception import ThreadDestroyedException
 from caikit.runtime.work_management.destroyable_thread import DestroyableThread
 
 
 class TestDestroyableThread(unittest.TestCase):
     def test_threads_can_be_interrupted(self):
         def infinite_wait():
             while True:
@@ -82,19 +90,23 @@
             thread.get_or_throw()
 
         self.assertEqual(expected, ctx.exception)
 
     def test_threads_will_not_execute_if_destroyed_before_starting(self):
         thread = DestroyableThread(threading.Event(), lambda: time.sleep(1000))
 
-        thread.destroy()
-        thread.start()
-        thread.join(1)
+        with catch_threading_exception() as cm:
+            thread.destroy()
+            thread.start()
+            thread.join(1)
 
-        self.assertFalse(thread.is_alive())
+            self.assertFalse(thread.is_alive())
+
+            # Make sure the correct exception was raised
+            assert cm.exc_type == ThreadDestroyedException
 
     def test_event_is_set_on_completion(self):
         event = threading.Event()
         thread = DestroyableThread(event, lambda: None)
 
         self.assertFalse(event.is_set())
         thread.start()
```

### Comparing `caikit-0.6.0/tox.ini` & `caikit-0.7.0/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [tox]
-envlist =
-    3.{11,10,9,8}
+envlist = py, lint, fmt, proto3
 
 [testenv]
 description = run tests with pytest with coverage
 deps =
     pytest>=6.2.5,<7.0
     pytest-cov>=2.10.1,<3.0
     pytest-html>=3.1.1,<4.0
@@ -21,15 +20,15 @@
 ; Unclear: We probably want to test wheel packaging
 ; But! tox will fail when this is set and _any_ interpreter is missing
 ; Without this, sdist packaging is tested so that's a start.
 package=wheel
 
 [testenv:docs]
 recreate = True
-deps = 
+deps =
     -r {toxinidir}/docs-requirements.txt
     alchemy-config>=1.1.1,<2.0.0
     alchemy-logging>=1.0.4,<2.0.0
     anytree>=2.7.0,<3.0
     docstring-parser>=0.14.1,<0.16.0
     grpcio-health-checking>=1.35.0,<2.0
     grpcio>=1.35.0,<2.0
@@ -41,20 +40,19 @@
     PyYAML>=6.0,<7.0
     requests>=2.26.0,<3.0
     semver>=2.13.0,<4.0
     six>=1.16.0,<2.0.0
     tqdm>=4.59.0,<5.0.0
     py-to-proto>=0.2.0,<0.3.0
     import-tracker>=3.1.5,<4
-changedir = docs
+changedir = docs/source
 
 ; Disabled '-W' flag as warnings in the files
 ; TOTO: Add back in once build warnings fixed
 commands =
-  sphinx-apidoc -f -o api/ ../caikit
   sphinx-build -E -a -b html -T . _build/html
 skip_install = True
 
 [testenv:fmt]
 description = format with pre-commit
 deps = pre-commit>=3.0.4,<4.0
 commands = ./scripts/fmt.sh
@@ -78,7 +76,21 @@
 deps = flit==3.8
 passenv =
     FLIT_PASSWORD
 setenv =
     FLIT_USERNAME = __token__
 commands = flit publish
 skip_install = True
+
+# Ensure compatibility is maintained with protobuf 3.X
+[testenv:proto3]
+description = run tests with pytest with coverage
+deps =
+    pytest>=6.2.5,<7.0
+    pytest-cov>=2.10.1,<3.0
+    pytest-html>=3.1.1,<4.0
+    tls_test_tools>=0.1.1
+    wheel>=0.38.4
+commands =
+    pip uninstall grpcio-health-checking grpcio-reflection -y
+    pip install protobuf==3.19.0 grpcio-health-checking grpcio-reflection --upgrade
+    pytest --cov=caikit --cov-report=html {posargs:tests}
```

### Comparing `caikit-0.6.0/PKG-INFO` & `caikit-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.6.0
+Version: 0.7.0
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.16.0
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
+Requires-Dist: grpcio-reflection>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0,!=1.55.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
 Requires-Dist: import-tracker>=3.1.5,<4
 Requires-Dist: munch>=2.5.0,<4.0
 Requires-Dist: numpy>=1.20,<2
 Requires-Dist: prometheus_client>=0.12.0,<1.0
 Requires-Dist: protobuf>=3.19.0,<5
```

