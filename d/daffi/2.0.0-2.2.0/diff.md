# Comparing `tmp/daffi-2.0.0.tar.gz` & `tmp/daffi-2.2.0.tar.gz`

## Comparing `daffi-2.0.0.tar` & `daffi-2.2.0.tar`

### file list

```diff
@@ -1,205 +1,216 @@
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 daffi-2.0.0/CHANGELOG.rst
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 daffi-2.0.0/mkdocs.yml
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 daffi-2.0.0/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 daffi-2.0.0/.github/workflows/test_and_validate.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 daffi-2.0.0/.github/workflows/test_and_validate_staging.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/__about__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/__init__.py
--rw-r--r--   0        0        0     7544 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/async_result.py
--rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/exceptions.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/execution_modifiers.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/globals.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/interface.py
--rw-r--r--   0        0        0    17498 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/ipc.py
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/method_executors.py
--rw-r--r--   0        0        0    11958 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/remote_call.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/settings.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/signals.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/store.py
--rw-r--r--   0        0        0    11170 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/__init__.py
--rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/controller.py
--rw-r--r--   0        0        0     7593 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/node.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/scheduler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/__init__.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/channel_store.py
--rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/controller_operations.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/freezable_queue.py
--rw-r--r--   0        0        0    17330 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/node_operations.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/streams_store.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/task_waiter.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/operations/ttl_store.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/proto/__init__.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/proto/message.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/proto/messager.proto
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/proto/messager_pb2.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/components/proto/messager_pb2_grpc.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/_alias.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/_base.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/_callback.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/_fetcher.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/decorators/_local.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/registry/__init__.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/registry/_base.py
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/registry/_callback.py
--rw-r--r--   0        0        0     9314 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/registry/_fetcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/colors.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/custom_types.py
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/debug.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/func_validation.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/logger.py
--rw-r--r--   0        0        0     6738 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/misc.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 daffi-2.0.0/daffi/utils/timeparse.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 daffi-2.0.0/docker/Dockerfile
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 daffi-2.0.0/docker/main.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/async-apps.md
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/execution-modifiers.md
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/global-object.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/index.md
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/node-and-controller.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/code-reference/callback.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/code-reference/fetcher.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/code-reference/global.md
--rw-r--r--   0        0        0   233533 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/bg.jpg
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/controller-plus-node-arch.drawio
--rw-r--r--   0        0        0    27050 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/controller-plus-node-arch.png
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/gitter.png
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/logo-white-sm.png
--rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/logo-white.png
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/logo.png
--rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/many-controllers.drawio
--rw-r--r--   0        0        0    38251 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/many-controllers.png
--rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/pdf-file.png
--rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/stand-alone-controller-arch.drawio
--rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/images/stand-alone-controller-arch.png
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/js/extra.js
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/aliased-methods.md
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/asynchronous-execution.md
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/basic-example.md
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/bidirectional-communication.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/broadcasting.md
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/callback-additional-arguments.md
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/fetchers-with-body.md
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/function-transfer.md
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/named-processes.md
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/private-methods.md
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/scheduling-tasks.md
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/stream-callback-to-fetcher.md
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 daffi-2.0.0/docs/usage/stream-fetcher-to-callback.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/docker-compose.yml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/colorizer/Dockerfile
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/colorizer/main.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/email_processor/Dockerfile
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/email_processor/main.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/web/Dockerfile
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/web/app.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/web/templates/base.html
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/docker/web/templates/index.html
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/classes_based/consumer.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/classes_based/publisher1.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/classes_based/publisher2.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/classes_based/publisher3.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/decorators_based/consumer.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/decorators_based/publisher1.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/decorators_based/publisher2.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/opencv_stream/decorators_based/publisher3.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/callbacks_from_class/consumer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/callbacks_from_class/publisher.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/eta/consumer.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/eta/publisher.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/kill_all/consumer.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/kill_all/publisher.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/no_return/consumer.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/no_return/publisher.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/scheduler/consumer.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/scheduler/publisher.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/stream/consumer.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/stream/publisher.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/transfer_and_call/consumer.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/transfer_and_call/publisher.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication/class_based/proc1.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication/class_based/proc2.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_generator/class_consumer.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callback_generator/class_publisher.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callbacks_from_class/consumer.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/callbacks_from_class/publisher.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/eta/class_consumer.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/eta/class_publisher.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/eta/consumer.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/eta/publisher.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/fetcher_generator/class_consumer.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/fetcher_generator/class_publisher.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/no_return/consumer.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/no_return/publisher.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/scheduler/consumer.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/scheduler/publisher.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/stream/consumer.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/stream/publisher.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/transfer_and_call/consumer.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/transfer_and_call/publisher.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 daffi-2.0.0/scripts/generate_coverage_summary.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 daffi-2.0.0/scripts/write_coverage_summary_report.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_many_callbacks.py
--rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_many_nodes.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_period.py
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_pipeline.py
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_stream_callback_to_fetcher.py
--rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_stream_fetcher_to_callback.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/test_trio.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/broadcast.jinja2
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/callback_per_node.jinja2
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/many_callbacks.jinja2
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/period1.jinja2
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/pipeline.jinja2
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/pipeline2.jinja2
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/stream.jinja2
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/stream_from_callback.jinja2
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/test_trio.jinja2
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/layout/async_callback.jinja2
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/layout/base.jinja2
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/layout/callback.jinja2
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/integration/templates/layout/macros.jinja2
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_async_result.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_callback_and_fecher_classes.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_callback_decorator.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_fetcher_decorator.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_freezable_queue.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_logger.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 daffi-2.0.0/tests/unit/test_misc.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 daffi-2.0.0/.gitignore
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 daffi-2.0.0/README.md
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daffi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     9288 2020-02-02 00:00:00.000000 daffi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 daffi-2.2.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 daffi-2.2.0/mkdocs.yml
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/test_and_validate.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 daffi-2.2.0/.github/workflows/test_and_validate_staging.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/__about__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/__init__.py
+-rw-r--r--   0        0        0     8482 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/async_result.py
+-rwxr-xr-x   0        0        0     1824 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/exceptions.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/execution_modifiers.py
+-rw-r--r--   0        0        0    15016 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/globals.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/interface.py
+-rw-r--r--   0        0        0    19209 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/ipc.py
+-rw-r--r--   0        0        0     8690 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/method_executors.py
+-rw-r--r--   0        0        0    12413 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/remote_call.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/settings.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/signals.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/store.py
+-rw-r--r--   0        0        0    15214 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/__init__.py
+-rw-r--r--   0        0        0     8498 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/controller.py
+-rw-r--r--   0        0        0     7925 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/node.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/scheduler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/__init__.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/channel_store.py
+-rw-r--r--   0        0        0    19283 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/controller_operations.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/freezable_queue.py
+-rw-r--r--   0        0        0    19083 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/node_operations.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/streams_store.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/task_waiter.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/operations/ttl_store.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/message.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager.proto
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager_pb2.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/components/proto/messager_pb2_grpc.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_alias.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_base.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_callback.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_fetcher.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/decorators/_local.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/__init__.py
+-rw-r--r--   0        0        0     3550 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_base.py
+-rw-r--r--   0        0        0     6299 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_callback.py
+-rw-r--r--   0        0        0     9460 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/registry/_fetcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/colors.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/custom_types.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/debug.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/func_validation.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/logger.py
+-rw-r--r--   0        0        0     6775 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/misc.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 daffi-2.2.0/daffi/utils/timeparse.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 daffi-2.2.0/docker/Dockerfile
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 daffi-2.2.0/docker/main.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/async-apps.md
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/execution-modifiers.md
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/global-object.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/index.md
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/node-and-controller.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/callback.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/fetcher.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/code-reference/global.md
+-rw-r--r--   0        0        0   233533 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/bg.jpg
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/controller-plus-node-arch.drawio
+-rw-r--r--   0        0        0    27050 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/controller-plus-node-arch.png
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/gitter.png
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo-white-sm.png
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo-white.png
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/logo.png
+-rw-r--r--   0        0        0    12737 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/many-controllers.drawio
+-rw-r--r--   0        0        0    38251 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/many-controllers.png
+-rw-r--r--   0        0        0    10070 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/pdf-file.png
+-rw-r--r--   0        0        0    10821 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/stand-alone-controller-arch.drawio
+-rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/images/stand-alone-controller-arch.png
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/js/extra.js
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/aliased-methods.md
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/asynchronous-execution.md
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/basic-example.md
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/bidirectional-communication.md
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/broadcasting.md
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/callback-additional-arguments.md
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/fetchers-with-body.md
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/function-transfer.md
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/named-processes.md
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/private-methods.md
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/scheduling-tasks.md
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/stream-callback-to-fetcher.md
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 daffi-2.2.0/docs/usage/stream-fetcher-to-callback.md
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/cert.pem
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/domains.ext
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/generate_certs.sh
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/key.pem
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/root_ca.pem
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/root_key.pem
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/certs/sign.csr
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/docker-compose.yml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/colorizer/Dockerfile
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/colorizer/main.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/email_processor/Dockerfile
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/email_processor/main.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/Dockerfile
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/app.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/templates/base.html
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/docker/web/templates/index.html
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/consumer.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher1.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher2.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/classes_based/publisher3.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/consumer.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher1.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher2.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/opencv_stream/decorators_based/publisher3.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/callbacks_from_class/consumer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/callbacks_from_class/publisher.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/eta/consumer.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/eta/publisher.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/kill_all/consumer.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/kill_all/publisher.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/no_return/consumer.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/no_return/publisher.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/scheduler/consumer.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/scheduler/publisher.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/stream/consumer.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/stream/publisher.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/transfer_and_call/consumer.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/transfer_and_call/publisher.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc1.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc2.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc1.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/class_based/proc2.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_auth_enabled/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_generator/class_consumer.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callback_generator/class_publisher.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callbacks_from_class/consumer.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/callbacks_from_class/publisher.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/class_consumer.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/class_publisher.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/consumer.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/eta/publisher.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/fetcher_generator/class_consumer.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/fetcher_generator/class_publisher.py
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/no_return/consumer.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/no_return/publisher.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/scheduler/consumer.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/scheduler/publisher.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/stream/consumer.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/stream/publisher.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/transfer_and_call/consumer.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/transfer_and_call/publisher.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 daffi-2.2.0/scripts/generate_coverage_summary.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 daffi-2.2.0/scripts/write_coverage_summary_report.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_many_callbacks.py
+-rw-r--r--   0        0        0     5075 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_many_nodes.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_period.py
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_pipeline.py
+-rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_stream_callback_to_fetcher.py
+-rw-r--r--   0        0        0     3377 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_stream_fetcher_to_callback.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/test_trio.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/broadcast.jinja2
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/callback_per_node.jinja2
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/many_callbacks.jinja2
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/period1.jinja2
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/pipeline.jinja2
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/pipeline2.jinja2
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/stream.jinja2
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/stream_from_callback.jinja2
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/test_trio.jinja2
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/async_callback.jinja2
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/base.jinja2
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/callback.jinja2
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/integration/templates/layout/macros.jinja2
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_async_result.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_callback_and_fecher_classes.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_callback_decorator.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_fetcher_decorator.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_freezable_queue.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_logger.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 daffi-2.2.0/tests/unit/test_misc.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 daffi-2.2.0/.gitignore
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 daffi-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 daffi-2.2.0/README.md
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 daffi-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9288 2020-02-02 00:00:00.000000 daffi-2.2.0/PKG-INFO
```

### Comparing `daffi-2.0.0/CHANGELOG.rst` & `daffi-2.2.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/mkdocs.yml` & `daffi-2.2.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     - named processes: usage/named-processes.md
     - stream from fetcher to callback: usage/stream-fetcher-to-callback.md
     - stream from callback to fetcher: usage/stream-callback-to-fetcher.md
     - function transfer: usage/function-transfer.md
     - bidirectional communication: usage/bidirectional-communication.md
     - asynchronous execution: usage/asynchronous-execution.md
     - broadcasting: usage/broadcasting.md
-    - task scheduling and butch delayed executon: usage/scheduling-tasks.md
+    - task scheduling and batch delayed execution: usage/scheduling-tasks.md
   - Node and Controller: node-and-controller.md
   - Global object: global-object.md
   - Asynchronous applications: async-apps.md
   - Execution modifiers: execution-modifiers.md
   - Code reference:
      - Global: code-reference/global.md
      - callback: code-reference/callback.md
```

### Comparing `daffi-2.0.0/.github/workflows/test_and_validate.yml` & `daffi-2.2.0/.github/workflows/test_and_validate.yml`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/.github/workflows/test_and_validate_staging.yml` & `daffi-2.2.0/.github/workflows/test_and_validate_staging.yml`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/async_result.py` & `daffi-2.2.0/daffi/async_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from anyio import sleep
 
 from daffi.components.proto.message import RpcMessage
 from daffi.exceptions import RemoteError, TimeoutError, InitializationError
 from daffi.utils.custom_types import RemoteResult, SchedulerTaskType
 from daffi.store import TttStore
+from daffi.utils.misc import run_in_threadpool
 
 
 __all__ = ["AsyncResult", "SchedulerTask"]
 
 
 class ResultInf(ABC):
     _awaited_results: ClassVar[TttStore] = TttStore()
@@ -187,18 +188,14 @@
         return self
 
 
 class IterableAsyncResult(AsyncResult):
     def __post_init__(self):
         self._queue = Queue()
 
-    def __iter__(self):
-        """Iterate over result items."""
-        yield from self.get()
-
     @property
     def ready(self):
         raise NotImplementedError()
 
     @property
     def error(self):
         raise NotImplementedError()
@@ -227,27 +224,54 @@
 
                     if completed:
                         break
 
                     yield result
 
         finally:
-            self.result = self._awaited_results.pop(self.uuid)
+            self.result = self._awaited_results.pop(self.uuid, None)
 
-    def get_async(self, timeout: Union[int, float] = None) -> RemoteResult:
-        # TODO need to find better way to handle queue items across threads for async applications.
-        raise NotImplementedError()
+    async def get_async(self, timeout: Union[int, float] = None) -> RemoteResult:
+        # `timeout` from arguments take precedence over class attribute `_timeout`
+        timeout = timeout or self._timeout
+
+        if self.result:
+            InitializationError("Generator has already been used").fire()
+
+        self.result = True
+        if timeout:
+            timeout_sentinel = time.time() + timeout
+        try:
+            while True:
+                wait = None if timeout is None else timeout_sentinel - time.time()
+                try:
+                    result, completed = await run_in_threadpool(self._queue.get, timeout=wait)
+                except Empty:
+                    TimeoutError(f"Function {self.func_name} result timed out").fire()
+                else:
+                    if isinstance(result, RemoteError):
+                        result.raise_with_trackeback()
+
+                    if completed:
+                        break
+
+                    yield result
+
+        finally:
+            self.result = self._awaited_results.pop(self.uuid)
 
     @classmethod
     def _set_and_trigger(cls, msg_uuid: int, result: Any, completed: Optional[bool] = True) -> NoReturn:
         AsyncResult._awaited_results[msg_uuid]._set((result, completed))
 
     def _set(self, item: Tuple):
         self._queue.put_nowait(item)
 
 
 def get_result_type(
     is_period: bool, is_generator: bool
-) -> Type[Union[AsyncResult, SchedulerTask, IterableAsyncResult]]:
+) -> Tuple[Type[Union[AsyncResult, SchedulerTask, IterableAsyncResult]], bool]:
     if is_generator:
-        return IterableAsyncResult
-    return SchedulerTask if is_period else AsyncResult
+        # Computed results for `IterableAsyncResult` are prohibited.
+        return IterableAsyncResult, False
+    res_type = SchedulerTask if is_period else AsyncResult
+    return res_type, True
```

### Comparing `daffi-2.0.0/daffi/exceptions.py` & `daffi-2.2.0/daffi/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     ...
 
 
 class StopComponentError(Exception):
     ...
 
 
+class ControllerUnavailable(Exception):
+    ...
+
+
 @dataclass
 class RemoteError:
     """It is not Exception itself but container to transfer exceptions from remove executor to caller."""
 
     info: Optional[str] = None
     traceback: Optional[bytes] = None
     _origin_traceback: TracebackType = field(repr=False, default=None)
@@ -66,12 +70,8 @@
         if self.traceback:
             traceback.print_tb(self.unpickled_trackeback)
 
     def raise_with_trackeback(self):
         if self.unpickled_trackeback:
             RemoteCallError(self.info).with_traceback(self.unpickled_trackeback).fire()
         else:
-            err = self._awaited_error_type(self.info)
-            if hasattr(err, "fire"):
-                err.fire()
-            else:
-                raise err
+            raise self._awaited_error_type(self.info)
```

### Comparing `daffi-2.0.0/daffi/execution_modifiers.py` & `daffi-2.2.0/daffi/execution_modifiers.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,27 +14,30 @@
     "is_exec_modifier_type",
 ]
 
 
 @dataclass
 class FG:
     timeout: Optional[TimeUnits] = None
+    receiver: Optional[str] = None
 
 
 @dataclass
 class BG:
     timeout: Optional[TimeUnits] = None
     eta: Optional[TimeUnits] = None
     return_result: Optional[bool] = True
+    receiver: Optional[str] = None
 
 
 @dataclass
 class PERIOD:
     at_time: Optional[Union[List[TimeUnits], TimeUnits]] = None
     interval: Optional[TimeUnits] = None
+    receiver: Optional[str] = None
 
 
 @dataclass
 class BROADCAST:
     eta: Optional[TimeUnits] = None
     timeout: Optional[TimeUnits] = None  # Works only with return_result=True
     return_result: Optional[bool] = True
```

### Comparing `daffi-2.0.0/daffi/globals.py` & `daffi-2.2.0/daffi/globals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import time
 from dataclasses import dataclass, field
 from threading import Event
 from typing import (
     Callable,
     Any,
     Optional,
     List,
@@ -14,15 +15,15 @@
     Tuple,
 )
 from anyio import sleep
 from tenacity import retry, retry_if_exception_type, wait_fixed, stop_after_attempt
 
 from daffi.utils import colors
 from daffi.utils.logger import get_daffi_logger
-from daffi.decorators import callback, __body_unknown__
+from daffi.decorators import callback
 from daffi.exceptions import InitializationError, GlobalContextError
 from daffi.ipc import Ipc
 from daffi.remote_call import LazyRemoteCall
 from daffi.utils.misc import Singleton, string_uuid
 from daffi.utils.func_validation import pretty_callbacks
 from daffi.registry._base import BaseRegistry
 
@@ -30,37 +31,46 @@
 
 __all__ = ["Global", "get_g"]
 
 
 @dataclass
 class Global(metaclass=Singleton):
     """
-    Main daffi entrypoint for all remote operations eg.
-    call remote callbacks, wait for remote processes, obtain additional information from remote etc.
+    The main entry point for all remote operations, such as calling remote callbacks,
+     waiting for remote processes, and obtaining additional information from remote sources.
     Args:
        process_name: Global process name. If specified it is used as reference key to Node process.
            By default randomly generated hash is used as reference.
        init_controller: Flag that indicates whether `Controller` should be instantiated in current process
        init_node: Flag that indicates whether `Node` should be instantiated in current process
        host: host to connect `Controller`/`Node` via tcp. If not provided then Global consider UNIX socket connection to be used.
        port: Optional port to connect `Controller`/`Node` via tcp. If not provided random port will be chosen.
        unix_sock_path: Folder where UNIX socket will be created. If not provided default path is < tmp directory >/dafi/
-          where `<tmp directory >` is default temporary directory on system.
-       on_connect: Function that will be executed when connection to Controller is established
+           where `<tmp directory >` is default temporary directory on system.
+       on_init: Function that will be executed once when Global object is initialized. `on_init` takes Global object as first argument
+       on_node_connect: Function that will be executed each time when connection
+           to Controller is established (IOW it works only for Nodes). `on_connect` takes Global object as first argument
+       on_node_disconnect: Function that will be executed each time when connection to Controller is lost
     """
 
     process_name: Optional[str] = field(default_factory=string_uuid)
     init_controller: Optional[bool] = False
     init_node: Optional[bool] = True
     host: Optional[str] = None
     port: Optional[int] = None
     unix_sock_path: Optional[os.PathLike] = None
-    on_connect: Optional[Callable[..., Any]] = None
+    ssl_certificate: Optional[os.PathLike] = None
+    ssl_key: Optional[os.PathLike] = None
+    on_init: Optional[Callable[["Global"], Any]] = None
+    on_node_connect: Optional[Callable[["Global", str], Any]] = None
+    on_node_disconnect: Optional[Callable[["Global", str], Any]] = None
 
     def __post_init__(self):
+        if self.process_name is None:
+            self.process_name = string_uuid()
         self.process_name = str(self.process_name)
 
         if not (self.init_controller or self.init_node):
             InitializationError(
                 "No components were found in current process."
                 " Provide at least one required argument"
                 " `init_controller=True` or `init_node=True`."
@@ -73,34 +83,47 @@
             ).fire()
 
         if not self.host and sys.platform == "win32":
             InitializationError(
                 "Windows platform doesn't support unix sockets. Provide host and port to use TCP"
             ).fire()
 
+        if self.ssl_certificate and not os.path.exists(self.ssl_certificate):
+            InitializationError("ssl_certificate: invalid path").fire()
+
+        if self.ssl_key and not os.path.exists(self.ssl_key):
+            InitializationError("ssl_key: invalid path").fire()
+
         self._global_terminate_event = Event()
         self.ipc = Ipc(
             process_name=self.process_name,
             init_controller=self.init_controller,
             init_node=self.init_node,
             global_terminate_event=self._global_terminate_event,
             host=self.host,
             port=self.port,
             unix_sock_path=self.unix_sock_path,
+            ssl_certificate=self.ssl_certificate,
+            ssl_key=self.ssl_key,
+            on_node_connect=self.on_node_connect,
+            on_node_disconnect=self.on_node_disconnect,
             logger=logger,
         )
 
         BaseRegistry._ipc = self.ipc
         self.ipc.start()
         if not self.ipc.wait():
             self.stop()
-            GlobalContextError("Unable to start daffi components.").fire()
+            logger.error("Unable to start daffi components.")
+            return
         self.port = self.ipc.port
-        if self.on_connect and callable(self.on_connect):
-            self.on_connect()
+        if self.on_init and callable(self.on_init):
+            self.on_init(self)
+        # Give some extra time for nodes to connect before using fetchers.
+        time.sleep(2)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
         if exc_type is not None:
@@ -132,35 +155,18 @@
         return self.ipc.join()
 
     async def join_async(self):
         """Async version of .join() method. Use this method if your application is asynchronous."""
         while self.ipc.is_alive():
             await sleep(0.5)
 
-    def stop(self, kill_all_connected_nodes: Optional[bool] = False):
-        """
-        Stop all components (Node/Controller) that is running are current process
-        Args:
-            kill_all_connected_nodes: Optional flag that indicated whether kill signal should be sent to all connected
-                nodes. This argument works only for those processes where controller is running.
+    def stop(self):
         """
-        res = None
-        if kill_all_connected_nodes:
-            if not self.is_controller:
-                logger.error("You can kill all nodes only from a process that has a controller")
-            else:
-                logger.debug(f"`Kill all` operation triggered ({self.process_name})")
-                res = self.kill_all()
+        Stop all components (Node/Controller) that is running are current process"""
         self.ipc.stop()
-        return res
-
-    def kill_all(self):
-        """Kill all connected nodes. This method works only for those processes where controller is running"""
-        res = self.ipc.kill_all()
-        return res
 
     def transfer_and_call(
         self, remote_process: str, func: Callable[..., Any], *args: Tuple[Any], **kwargs: Dict[Any, Any]
     ) -> Union[Coroutine, Any]:
         """
         Send function along with arguments to execute on remote process.
         This method has some limitations. For example you should import modules inside function
@@ -371,12 +377,7 @@
                     "condition": "at_time",
                     "func_name": task_ident.func_name,
                     "uuid": task_ident.msg_uuid,
                     "number_of_active_tasks": list(filter(None, at_time_tasks)),
                 }
             )
     return res
-
-
-@callback
-async def __kill_all() -> NoReturn:
-    __body_unknown__()
```

### Comparing `daffi-2.0.0/daffi/interface.py` & `daffi-2.2.0/daffi/interface.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/ipc.py` & `daffi-2.2.0/daffi/ipc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
-import time
-from itertools import chain, cycle
+from itertools import chain
 from logging import Logger
 from inspect import iscoroutinefunction
 from threading import Thread, Event
+from concurrent.futures import ThreadPoolExecutor
 from typing import NoReturn, Dict, Union, Optional, Callable, Any, Tuple, AsyncGenerator
 
 from anyio.from_thread import start_blocking_portal
 
 from daffi.utils import colors
 from daffi.settings import DEBUG
 from daffi.async_result import get_result_type, AsyncResult
@@ -36,37 +36,50 @@
         process_name: str,
         init_controller: bool,
         init_node: bool,
         global_terminate_event: Event,
         host: Optional[str] = None,
         port: Optional[int] = None,
         unix_sock_path: Optional[os.PathLike] = None,
+        ssl_certificate: Optional[os.PathLike] = None,
+        ssl_key: Optional[os.PathLike] = None,
+        on_node_connect: Optional[Callable[["Global", str], Any]] = None,
+        on_node_disconnect: Optional[Callable[["Global", str], Any]] = None,
         logger: Logger = None,
     ):
         super().__init__()
         self.process_name = process_name
         self.init_controller = init_controller
         self.init_node = init_node
         self.global_terminate_event = global_terminate_event
         self.host = host
         self.port = port
         self.unix_sock_path = unix_sock_path
+        self.ssl_certificate = ssl_certificate
+        self.ssl_key = ssl_key
+        self.on_node_connect = on_node_connect
+        self.on_node_disconnect = on_node_disconnect
         self.logger = logger
         self.async_backend = async_library()
 
         self.daemon = True
         self.global_condition_event = ConditionEvent()
         self.controller = self.node = None
         self.task_waiter = TaskWaiter(process_name)
 
         AsyncResult._ipc = self
 
         if not (self.init_controller or self.init_node):
             InitializationError("At least one of 'init_controller' or 'init_node' must be True.").fire()
 
+        if self.on_node_connect and iscoroutinefunction(self.on_node_connect):
+            raise InitializationError("`on_node_connect` callback should not be an asynchronous function.")
+        if self.on_node_disconnect and iscoroutinefunction(self.on_node_disconnect):
+            raise InitializationError("`on_node_disconnect` callback should not be an asynchronous function.")
+
         set_signal_handler(self.stop)
 
     @property
     def is_running(self) -> bool:
         """Return True if Node, Cotroller or Controller and Node were started successfully."""
         return self.global_condition_event.success
 
@@ -95,39 +108,51 @@
         timeout: Optional[Union[int, float]] = None,
         async_: Optional[bool] = False,
         eta: Optional[Union[int, float]] = 0,
         return_result: Optional[bool] = True,
         func_period: Optional[Period] = None,
         broadcast: Optional[bool] = False,
         stream: Optional[bool] = False,
+        receiver: Optional[str] = None,
     ):
         self._check_node()
-        assert func_name is not None
         data = search_remote_callback_in_mapping(self.node.node_callback_mapping, func_name, exclude=self.process_name)
+
         if not data:
             # Get all callbacks without local
             available_callbacks = pretty_callbacks(
                 mapping=self.node.node_callback_mapping, exclude_proc=self.process_name, format="string"
             )
             msg = (
-                f"function {func_name!r} not found on remote.\n Available registered callbacks:\n"
-                + f"{available_callbacks}"
+                f"function {func_name!r} not found on remote. "
+                f"If your goal is to run the fetcher immediately after initializing the process,"
+                f" consider using the `wait_function` or `wait_process` functions"
+                f" to ensure that the corresponding process is ready before proceeding."
+                f".\n Available registered callbacks:\n" + f"{available_callbacks}"
                 if available_callbacks
                 else "No available callbacks found on remotes"
             )
             GlobalContextError(msg).fire()
 
+        if receiver and receiver not in self.node.node_callback_mapping:
+            # Validate if provided receiver in the one that is registered
+
+            GlobalContextError(
+                f"Provided receiver {receiver} is not one that is registered."
+                f" Available receivers = {list(self.node.node_callback_mapping.keys())}"
+            ).fire()
+
         if stream:
             # Stream has special initialization and validation process.
             if async_:
                 # Start stream process in background without blocking main process execution.
                 stream_thread = Thread(target=self.stream, args=(func_name, args), daemon=True)
                 return stream_thread.start()
             # Block main process execution until stream is completed.
-            return self.stream(func_name, args)
+            return self.stream(func_name, receiver, args)
 
         _, remote_callback = data
         remote_callback.validate_provided_arguments(*args, **kwargs)
         result = None
 
         if remote_callback.is_generator and (broadcast or not return_result or func_period or async_):
             InitializationError("Remote callback which are generators works only with FG execution modifier!")
@@ -139,16 +164,17 @@
             transmitter=self.process_name,
             func_name=func_name,
             func_args=args,
             func_kwargs=kwargs,
             return_result=return_result or wait_in_task_waiter,
             period=func_period,
             timeout=timeout or 0,
+            receiver=receiver,
         )
-        result_class = get_result_type(
+        result_class, allow_compute = get_result_type(
             is_period=bool(func_period),
             is_generator=remote_callback.is_generator,
         )
 
         if return_result or func_period:
             result = result_class(msg=msg)
         if result:
@@ -163,15 +189,15 @@
 
         self.node.send_threadsave(msg, eta)
 
         if func_period:
             result._scheduler_type = func_period.scheduler_type
             return result.get()
 
-        if not async_ and return_result:
+        if not async_ and return_result and allow_compute:
             result = result.get(timeout=timeout)
         return result
 
     def run(self) -> NoReturn:
         if DEBUG:
             self.logger.info(f"{colors.yellow('DEBUG')} mode enabled.")
         self.logger.info("Components initialization...")
@@ -187,14 +213,17 @@
             with start_blocking_portal(backend="asyncio", backend_options=backend_options) as portal:
                 if self.init_controller:
                     self.controller = Controller(
                         process_name=self.process_name,
                         host=self.host,
                         port=self.port,
                         global_terminate_event=self.global_terminate_event,
+                        on_node_disconnect=self.on_node_disconnect,
+                        ssl_certificate=self.ssl_certificate,
+                        ssl_key=self.ssl_key,
                     )
 
                     c_future, _ = portal.start_task(
                         self.controller.handle,
                         name=Controller.__class__.__name__,
                     )
                     self.port = getattr(self.controller, "port", None)
@@ -203,14 +232,17 @@
                 if self.init_node:
                     self.node = Node(
                         process_name=self.process_name,
                         host=self.host,
                         port=self.port,
                         async_backend=self.async_backend,
                         global_terminate_event=self.global_terminate_event,
+                        on_node_connect=self.on_node_connect,
+                        ssl_certificate=self.ssl_certificate,
+                        ssl_key=self.ssl_key,
                     )
 
                     n_future, _ = portal.start_task(
                         self.node.handle,
                         name=Node.__class__.__name__,
                     )
 
@@ -219,31 +251,32 @@
                         name=self.task_waiter.__class__.__name__,
                     )
 
                 self.global_condition_event.mark_success()
                 self.global_terminate_event.wait()
 
                 # Wait controller and node to finish 'on_stop' lifecycle callbacks.
-                if self.node:
-                    self.node.stop(wait=True)
-                    self.task_waiter.stop()
-                if self.controller:
-                    self.controller.stop(wait=True)
-
+                with ThreadPoolExecutor(max_workers=3) as executor:
+                    executor.submit(self.task_waiter.stop)
+                    if self.node:
+                        executor.submit(self.node.stop, True)
+                    if self.controller:
+                        executor.submit(self.controller.stop, True)
+                    executor.shutdown(wait=True)
                 # Wait pending futures to complete their tasks
                 for future in filter(None, (c_future, n_future, tw_future)):
                     if not future.done():
                         future.cancel()
 
         if not self.global_condition_event.success:
             self.global_condition_event.mark_fail()
 
         clear_method_type_stores()
 
-    def stream(self, func_name, args: Tuple) -> NoReturn:
+    def stream(self, func_name: str, receiver: Optional[str], args: Tuple) -> NoReturn:
         from daffi.registry._fetcher import Args
 
         if self.is_running:
             self._check_node()
 
             if len(args) != 1:
                 InitializationError(
@@ -287,14 +320,21 @@
             # Register result in order to obtain all available receivers
             result = self.node.send_and_register_result(msg=msg)
 
             self.logger.debug("Wait available stream receivers")
             receivers = result.get()
             if not receivers:
                 InitializationError("Unable to find receivers for stream.").fire()
+            elif receiver and receiver not in receivers:
+                InitializationError(
+                    f"Provided receiver is not in the list of available receivers for fuction {func_name}."
+                    f" Available receivers = {receivers}"
+                ).fire()
+            elif receiver:
+                receivers = [receiver]
 
             # Register the same result second time to track stream errors (If happened)
             result = result._clone_and_register()
             stream_pair_was_closed = False
             with self.node.stream_store.request_multi_connection(
                 receivers=receivers, msg_uuid=str(msg.uuid)
             ) as stream_pair_group:
@@ -391,31 +431,14 @@
                 transmitter=self.process_name,
                 receiver=remote_process,
                 func_name=func_name,
                 func_args=(self.process_name,),
             )
             return self.node.send_and_register_result(msg=msg).get()
 
-    def kill_all(self) -> NoReturn:
-        if self.is_running:
-            self._check_node()
-            func_name = "__kill_all"
-            msg = RpcMessage(
-                flag=MessageFlag.STOP_REQUEST, transmitter=self.process_name, func_name=func_name, return_result=False
-            )
-            self.node.send_threadsave(msg, 0)
-            for i in cycle(range(1, 51)):
-                if not (diff := {k for k in self.controller_callback_mapping} - {self.process_name}):
-                    break
-                if i == 25:
-                    self.node.send_threadsave(msg, 0)
-                elif i == 50:
-                    self.logger.error(f"Node(s): {diff} are still pending after after kill signal.")
-                time.sleep(0.5)
-
     def stop(self, *args, **kwargs):
         if args:
             sig_num = args[0]
             sig_name = SIGNALS_TO_NAMES_DICT[sig_num]
             self.logger.warning(f"Terminated by signal {sig_name!r}")
 
         self.global_terminate_event.set()
```

### Comparing `daffi-2.0.0/daffi/method_executors.py` & `daffi-2.2.0/daffi/method_executors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import time
+import logging
 from inspect import Signature
 from typing import NamedTuple, Union
 
 import daffi
 from daffi.utils.misc import Singleton
-from daffi.exceptions import GlobalContextError
+from daffi.exceptions import GlobalContextError, InitializationError
 from daffi.utils.custom_types import GlobalCallback, P, RemoteResult
 from daffi.execution_modifiers import FG, BG, BROADCAST, PERIOD
 from daffi.settings import LOCAL_FETCHER_MAPPING, LOCAL_CALLBACK_MAPPING
 
 __all__ = ["CallbackExecutor", "ClassCallbackExecutor", "FetcherExecutor", "ClassFetcherExecutor"]
 
 # ----------------------------------------------------------------------------------------------------------------------
@@ -135,15 +137,29 @@
 # Fetcher types
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 def f__call__(self, *args, **kwargs) -> RemoteResult:
     """Trigger executor with assigned execution modifier."""
     # Get remote call by name
-    remote_call = getattr(_g().call, self.alias)
+    for attempt in range(5):
+        try:
+            # In case fetcher is using too early after application start.
+            # `Global` object might be not initialized at this moment.
+            g = _g()
+            break
+        except InitializationError:
+            # Keep fist attempt silent
+            if attempt > 1:
+                logging.error("Global object is not initialized. Awaiting...")
+            time.sleep(2)
+    else:
+        raise InitializationError("Global object initialization is missing!")
+
+    remote_call = getattr(g.call, self.alias)
     # Set fetcher
     remote_call._fetcher = self
     # Execute remote call
     return (remote_call & self.exec_modifier)(*args, **kwargs)
 
 
 def call(self, *args, exec_modifier: Union[FG, BG, BROADCAST, PERIOD] = FG, **kwargs):
```

### Comparing `daffi-2.0.0/daffi/remote_call.py` & `daffi-2.2.0/daffi/remote_call.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,28 +44,28 @@
     def __str__(self):
         sep = ", "
         args = sep.join(map(str, self.args))
         kwargs = sep.join(f", {k}={v}" for k, v in self.kwargs.items())
         args_kwargs = f"{args}{kwargs}".strip(",").strip()
         return f"<{self.__class__.__name__} {self.func_name}({args_kwargs})>"
 
-    def obtain_result_in_thread(self, next_operand: Union[FG, BG, BROADCAST, PERIOD]):
-        self._result = self & next_operand
+    def obtain_result_in_thread(self, exec_modifier: Union[FG, BG, BROADCAST, PERIOD]):
+        self._result = self & exec_modifier
 
     async def __process_await__(
-        self, next_operand: Union[FG, BG, BROADCAST, PERIOD], return_result: Optional[bool] = False
+        self, exec_modifier: Union[FG, BG, BROADCAST, PERIOD], return_result: Optional[bool] = False
     ):
         if self._fetcher and not self._fetcher.proxy:
             args = self._fetcher.wrapped(*self.args, **self.kwargs)
             if iscoroutine(args):
                 args = await args
             self.args, self.kwargs = Args._aggregate_args(args=args)
             self._fetcher = None
 
-        await to_thread.run_sync(self.obtain_result_in_thread, next_operand)
+        await to_thread.run_sync(self.obtain_result_in_thread, exec_modifier)
         if return_result:
             return self._result
         return self
 
     def __and__(self, other) -> RemoteResult:
         if self._result != _empty_result:
             return self._result
@@ -75,32 +75,34 @@
             if iscoroutine(args):
                 raise InitializationError("Use await to execute asynchronous fetcher!")
             self.args, self.kwargs = Args._aggregate_args(args=args)
 
         if self._fetcher and self._fetcher.is_generator:
             # This is gonna be stream.
             if is_exec_modifier_type(other, FG):
-                return self.stream(async_=False)
+                return self.stream(async_=False, receiver=other.receiver)
             elif is_exec_modifier_type(other, BG):
-                return self.stream(async_=True)
+                return self.stream(async_=True, receiver=other.receiver)
             else:
                 InitializationError(
                     f"Invalid execution modifier: {other}. "
                     f"Only {FG} and {BG} execution modifiers can be"
                     f" used with fetcher generators (streams to remote)"
                 )
 
         if is_exec_modifier_type(other, FG):
-            return self.fg(timeout=other.timeout)
+            return self.fg(timeout=other.timeout, receiver=other.receiver)
 
         elif is_exec_modifier_type(other, BG):
-            return self.bg(timeout=other.timeout, eta=other.eta, return_result=other.return_result)
+            return self.bg(
+                timeout=other.timeout, eta=other.eta, return_result=other.return_result, receiver=other.receiver
+            )
 
         elif is_exec_modifier_type(other, PERIOD):
-            return self.period(at_time=other.at_time, interval=other.interval)
+            return self.period(at_time=other.at_time, interval=other.interval, receiver=other.receiver)
 
         elif is_exec_modifier_type(other, BROADCAST):
             return self.broadcast(eta=other.eta, return_result=other.return_result, timeout=other.timeout)
 
         else:
             GlobalContextError(f"Invalid operand {type(other)}. Use one of {_available_operands}").fire()
 
@@ -110,41 +112,44 @@
         if data:
             return data[1]
 
     @property
     def exists(self) -> bool:
         return bool(self.info)
 
-    def fg(self, timeout: Optional[TimeUnits] = None) -> RemoteResult:
+    def fg(self, timeout: Optional[TimeUnits] = None, receiver: Optional[str] = None) -> RemoteResult:
         timeout = self._get_duration(timeout, "timeout")
         return self._ipc.call(
             self.func_name,
             args=self.args,
             kwargs=self.kwargs,
             timeout=timeout,
             async_=False,
             return_result=True,
+            receiver=receiver,
         )
 
     def bg(
         self,
         timeout: Optional[TimeUnits] = None,
         eta: Optional[TimeUnits] = None,
         return_result: Optional[bool] = True,
+        receiver: Optional[str] = None,
     ) -> AsyncResult:
         timeout = self._get_duration(timeout, "timeout")
         eta = self._get_duration(eta, "eta", 0)
         return self._ipc.call(
             self.func_name,
             args=self.args,
             kwargs=self.kwargs,
             timeout=timeout,
             eta=eta,
             async_=True,
             return_result=return_result,
+            receiver=receiver,
         )
 
     def broadcast(
         self,
         eta: Optional[TimeUnits] = None,
         return_result: Optional[bool] = False,
         timeout: Optional[TimeUnits] = None,
@@ -159,15 +164,18 @@
             eta=eta,
             async_=not return_result,
             return_result=return_result,
             broadcast=True,
         )
 
     def period(
-        self, at_time: Optional[Union[List[TimeUnits], TimeUnits]], interval: Optional[TimeUnits]
+        self,
+        at_time: Optional[Union[List[TimeUnits], TimeUnits]],
+        interval: Optional[TimeUnits],
+        receiver: Optional[str] = None,
     ) -> SchedulerTask:
         if at_time is not None:
             if isinstance(at_time, (int, float, str, timedelta, datetime)):
                 at_time = [at_time]
             at_time = [self._get_duration(i, "at_time", 0) for i in at_time]
         if interval is not None:
             interval = self._get_duration(interval, "interval", 0)
@@ -177,24 +185,27 @@
         return self._ipc.call(
             self.func_name,
             args=self.args,
             kwargs=self.kwargs,
             async_=True,
             return_result=False,
             func_period=func_period,
+            receiver=receiver,
         )
 
-    def stream(self, async_: bool) -> NoReturn:
+    def stream(self, async_: bool, receiver: Optional[str] = None) -> NoReturn:
         """
         Start stream to remote.
         This is implicit execution modifier when upstream fetcher is generator (contains `yield` statement(s))
         Args:
             async_: If True stream will be executed in background without blocking main process.
         """
-        return self._ipc.call(self.func_name, args=self.args, kwargs=None, stream=True, async_=async_)
+        return self._ipc.call(
+            self.func_name, args=self.args, kwargs=None, stream=True, async_=async_, receiver=receiver
+        )
 
     def _get_duration(self, val: TimeUnits, arg_name: str, default: Optional[int] = None) -> Union[int, float]:
         if val:
             if isinstance(val, timedelta):
                 val = val.total_seconds()
             elif isinstance(val, str):
                 val = timeparse(val)
@@ -293,15 +304,15 @@
             func_name=__self__._func_name,
             args=args,
             kwargs=kwargs,
             _fetcher=__self__._fetcher,
         )
         if __self__._exec_modifier:
             if __self__.is_async:
-                return remote_call.__process_await__(next_operand=__self__._exec_modifier, return_result=True)
+                return remote_call.__process_await__(exec_modifier=__self__._exec_modifier, return_result=True)
             return remote_call & __self__._exec_modifier
         return remote_call
 
     def __getattr__(self, item) -> RemoteCall:
         if self._global_terminate_event and self._global_terminate_event.is_set():
             GlobalContextError("Global can no longer accept remote calls because it was stopped").fire()
         self._func_name = item
```

### Comparing `daffi-2.0.0/daffi/settings.py` & `daffi-2.2.0/daffi/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 LOCAL_FETCHER_MAPPING: Dict[K, GlobalCallback] = dict()
 
 # Default callbacks that are used internally by daffi.
 WELL_KNOWN_CALLBACKS: Set[str] = {
     "__transfer_and_call",
     "__async_transfer_and_call",
     "__cancel_scheduled_task",
-    "__kill_all",
     "__get_all_period_tasks",
     "<unknown>",
 }
 
 
 def clear_method_type_stores():
     LOCAL_CALLBACK_MAPPING.clear()
```

### Comparing `daffi-2.0.0/daffi/store.py` & `daffi-2.2.0/daffi/store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/__init__.py` & `daffi-2.2.0/daffi/components/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,36 +5,44 @@
 import asyncio
 import traceback
 from pathlib import Path
 from random import randint
 from abc import abstractmethod
 from itertools import count
 from cached_property import cached_property
-from threading import Event as thEvent
-from typing import Optional, NoReturn, Callable, ClassVar, List
+from threading import Event as thEvent, Thread
+from typing import Optional, NoReturn, Callable, ClassVar, List, Any, Set
 from contextlib import asynccontextmanager
 from tempfile import gettempdir
 
-from grpc import aio, ChannelConnectivity
+
+from grpc import aio, ChannelConnectivity, ssl_channel_credentials, ssl_server_credentials
 from anyio.abc import TaskStatus
 from grpc.aio._call import AioRpcError
 from anyio import TASK_STATUS_IGNORED
 from tenacity import AsyncRetrying, wait_fixed, retry_if_exception_type, RetryCallState, wait_none
 
-from daffi.exceptions import StopComponentError
+from daffi.exceptions import StopComponentError, ControllerUnavailable, InitializationError, RemoteCallError
 from daffi.interface import ComponentI
 from daffi.components.proto import messager_pb2_grpc as grpc_messager
 from daffi.utils.misc import string_uuid
 
 
 class UnixBase(ComponentI, grpc_messager.MessagerServiceServicer):
     SOCK_FILE = ".sock"
 
-    def __init__(self, unix_sock_path: Optional[os.PathLike]):
+    def __init__(
+        self,
+        unix_sock_path: Optional[os.PathLike],
+        ssl_certificate: Optional[os.PathLike],
+        ssl_key: Optional[os.PathLike],
+    ):
         self.unix_sock_path = unix_sock_path
+        self.ssl_certificate = ssl_certificate
+        self.ssl_key = ssl_key
 
     def info(self) -> str:
         return f"unix socket: [ {self.unix_socket!r} ]"
 
     @cached_property
     def base_dir(self) -> os.PathLike:
         _base_dir = self.unix_sock_path or Path(gettempdir()) / "daffi"
@@ -47,49 +55,85 @@
         sock = "unix:///" + os.path.join(self.base_dir, self.SOCK_FILE).strip("unix:///")
         if os.path.exists(sock):
             os.remove(sock)
         return sock
 
     @asynccontextmanager
     async def connect_listener(self):
-        async with aio.insecure_channel(self.unix_socket, options=self.client_options) as aio_channel:
-            yield aio_channel
+        """UNIX Client"""
+        if self.ssl_certificate and self.ssl_key:
+            with open(self.ssl_certificate, "rb") as f:
+                creds = ssl_channel_credentials(f.read())
+            async with aio.secure_channel(self.unix_socket, creds) as aio_channel:
+                yield aio_channel
+        else:
+            async with aio.insecure_channel(self.unix_socket) as aio_channel:
+                yield aio_channel
 
     async def create_listener(self) -> NoReturn:
+        """UNIX Server"""
         server = aio.server()
         grpc_messager.add_MessagerServiceServicer_to_server(self, server)
-        server.add_insecure_port(self.unix_socket)
+        if self.ssl_certificate and self.ssl_key:
+            with open(self.ssl_key, "rb") as f:
+                private_key = f.read()
+            with open(self.ssl_certificate, "rb") as f:
+                certificate_chain = f.read()
+            server_credentials = ssl_server_credentials(((private_key, certificate_chain),))
+            server.add_secure_port(self.unix_socket, server_credentials)
+        else:
+            server.add_insecure_port(self.unix_socket)
         await server.start()
         return server
 
 
 class TcpBase(ComponentI, grpc_messager.MessagerServiceServicer):
-    def __init__(self, host: str, port: Optional[int]):
+    def __init__(
+        self, host: str, port: Optional[int], ssl_certificate: Optional[os.PathLike], ssl_key: Optional[os.PathLike]
+    ):
         self.host = host
         self.port = port
+        self.ssl_certificate = ssl_certificate
+        self.ssl_key = ssl_key
         if self.host in ("localhost", "0.0.0.0", "127.0.0.1", "192.168.0.1"):
             self.host = "[::]"
 
     def info(self) -> str:
         return f"tcp: [ host {self.host!r}, port: {self.port!r} ]"
 
     @asynccontextmanager
     async def connect_listener(self):
-        async with aio.insecure_channel(f"{self.host}:{self.port}", options=self.client_options) as aio_channel:
-            yield aio_channel
+        """TCP Client"""
+        listen_addr = f"{self.host}:{self.port}"
+        if self.ssl_certificate and self.ssl_key:
+            with open(self.ssl_certificate, "rb") as f:
+                creds = ssl_channel_credentials(f.read())
+            async with aio.secure_channel(listen_addr, creds) as aio_channel:
+                yield aio_channel
+        else:
+            async with aio.insecure_channel(listen_addr) as aio_channel:
+                yield aio_channel
 
-    async def create_listener(self, task_status: TaskStatus = TASK_STATUS_IGNORED) -> NoReturn:
+    async def create_listener(self) -> NoReturn:
+        """TCP Server"""
         if not self.port:
             await self.find_random_port()
         server = aio.server()
         grpc_messager.add_MessagerServiceServicer_to_server(self, server)
         listen_addr = f"{self.host}:{self.port}"
-        server.add_insecure_port(listen_addr)
+        if self.ssl_certificate and self.ssl_key:
+            with open(self.ssl_key, "rb") as f:
+                private_key = f.read()
+            with open(self.ssl_certificate, "rb") as f:
+                certificate_chain = f.read()
+            server_credentials = ssl_server_credentials(((private_key, certificate_chain),))
+            server.add_secure_port(listen_addr, server_credentials)
+        else:
+            server.add_insecure_port(listen_addr)
         await server.start()
-        task_status.started()
         return server
 
     async def find_random_port(self, min_port: Optional[int] = 49152, max_port: Optional[int] = 65536) -> NoReturn:
         """
         Bind this controller to a random port in a range.
         If the port range is unspecified, the system will choose the port.
         Args:
@@ -101,50 +145,59 @@
         while True:
             self.port = randint(min_port, max_port)
             if not await self.check_endpoint_is_busy():
                 break
 
 
 class ComponentsBase(UnixBase, TcpBase):
-    RETRY_TIMEOUT = 2  # 2 sec
+    RETRY_TIMEOUT = 1  # 1 sec
     IMMEDIATE_ACTION_ERRORS = (AioRpcError,)
-    NON_IMMEDIATE_ACTION_ERRORS = (AioRpcError, RuntimeError)
+    NON_IMMEDIATE_ACTION_ERRORS = (AioRpcError, RuntimeError, ControllerUnavailable)
     STOP_ACTION_ERRORS = (StopComponentError,)
 
     logger: logging.Logger = None
-    components: ClassVar[List[Callable]] = []
+    components: ClassVar[Set[Callable]] = set()
 
     def __init__(
         self,
         process_name: str,
         host: Optional[str] = None,
         port: Optional[int] = None,
         unix_sock_path: Optional[os.PathLike] = None,
+        ssl_certificate: Optional[os.PathLike] = None,
+        ssl_key: Optional[os.PathLike] = None,
         async_backend: Optional[str] = None,
         global_terminate_event: Optional[thEvent] = None,
+        on_node_connect: Optional[Callable[["Global", str], Any]] = None,
+        on_node_disconnect: Optional[Callable[["Global", str], Any]] = None,
     ):
         self._set_keyboard_interrupt_handler()
 
         self.process_name = process_name
         self.async_backend = async_backend or "asyncio"
         self.operations = None
         self.ident = string_uuid()
         self.global_terminate_event = global_terminate_event
+        self.on_node_connect = on_node_connect
+        self.on_node_disconnect = on_node_disconnect
         self._stopped = self._connected = False
         self.stop_event: bool = False
         self.stop_callbacks: List[Callable] = []
 
-        self.components.append(self)
+        self.components.add(self)
 
         if host:  # Check only host. Full host/port validation already took place before.
             self._base = TcpBase
-            self._base.__init__(self, host, port)
+            self._base.__init__(self, host, port, ssl_certificate, ssl_key)
         else:
             self._base = UnixBase
-            self._base.__init__(self, unix_sock_path)
+            self._base.__init__(self, unix_sock_path, ssl_certificate, ssl_key)
+
+    def __hash__(self):
+        return hash(self.__class__.__name__)
 
     @abstractmethod
     async def on_init(self) -> NoReturn:
         raise NotImplementedError
 
     @abstractmethod
     async def handle_operations(self, task_status: TaskStatus) -> NoReturn:
@@ -152,31 +205,33 @@
 
     @abstractmethod
     async def before_connect(self) -> NoReturn:
         raise NotImplementedError
 
     async def on_stop(self) -> NoReturn:
         while not self.stop_event:
-            await asyncio.sleep(0.1)
+            await asyncio.sleep(0.3)
+
+    async def on_terminate(self):
+        self.logger.info(f"{self.__class__.__name__} stopped.")
+        self._stopped = True
+        self.components.discard(self)
+        if not self.components:
+            # Cancel all existing asyncio tasks if component is the last one in termination chain. Eg if controller
+            # is running along with node then controller will be in charge of cleaning.
+            self.logger.debug("Cleaning asyncio tasks...")
+            tasks = [task for task in asyncio.all_tasks(asyncio.get_running_loop()) if not task.done()]
+            for task in tasks:
+                task.cancel()
 
     @abstractmethod
-    def on_error(self) -> NoReturn:
+    def on_error(self, exception: Exception) -> NoReturn:
         raise NotImplementedError
 
     @cached_property
-    def client_options(self):
-        """Grpc client options"""
-        # GRPC_ARG_KEEPALIVE_TIME_MS   "grpc.keepalive_time_ms"
-        #   After a duration of this time the client/server pings its peer to see if the transport is still alive.
-        # GRPC_ARG_KEEPALIVE_TIMEOUT_MS   "grpc.keepalive_timeout_ms"
-        #   After waiting for a duration of this time, if the keepalive ping
-        #   sender does not receive the ping ack, it will close the transport.
-        return [("grpc.keepalive_timeout_ms", 1000), ("grpc.keepalive_time_ms", 360000)]
-
-    @cached_property
     def info(self) -> str:
         return self._base.info(self)
 
     def stop(self, wait: Optional[bool] = False):
         self.stop_event = True
         if wait:
             for ind in count(1):
@@ -197,43 +252,81 @@
         if await self.check_endpoint_is_busy():
             self.logger.error(f"{self.info} is already allocated")
             raise StopComponentError()
         listener = await self._base.create_listener(self)
         self._connected = True
         return listener
 
+    async def execute_on_connect(self):
+        """Execute `on_connect` lifecycle handler in separate thread to prevent blocking main message handler."""
+        if self.on_node_connect:
+            # Execute `on_connect` lifecycle event in case such handler exists.
+            def _on_connect_wrapper(retry=True):
+                from daffi import get_g
+
+                while True:
+                    try:
+                        g = get_g()
+                        break
+                    except InitializationError:
+                        time.sleep(0.1)
+                try:
+                    self.on_node_connect(g, self.process_name)
+                except Exception as e:
+                    if isinstance(e, RemoteCallError) and retry:
+                        # another attempt to run the callback is allowed
+                        # if the error is related to access to a remote process
+                        time.sleep(1)
+                        return _on_connect_wrapper(retry=False)
+                    self.logger.error(
+                        f"Exception occurred while execution `on_node_connect` handler: {e}, type: {type(e)}"
+                    )
+
+            Thread(target=_on_connect_wrapper).start()
+
+    async def execute_on_disconnect(self, process_name):
+        if self.on_node_disconnect:
+
+            def _on_disconnect_wrapper():
+                from daffi import get_g
+
+                g = get_g()
+                try:
+                    self.on_node_disconnect(g, process_name)
+                except Exception as e:
+                    self.logger.error(
+                        f"Exception occurred while execution `on_node_disconnect` handler: {e}, type: {type(e)}"
+                    )
+
+            Thread(target=_on_disconnect_wrapper).start()
+
     def after_exception(self, retry_state: RetryCallState):
         """return the result of the last call attempt"""
 
-        self.on_error()
         retry_object = retry_state.retry_object
         attempt = retry_state.attempt_number
         exception = retry_state.outcome.exception()
+        self.on_error(exception)
 
         if type(exception) in self.IMMEDIATE_ACTION_ERRORS:
             if type(exception) == AioRpcError:
-                if "Cancelling all calls" in str(exception):
-                    self.logger.debug("Cancelling all tasks and stop.")
-                    self.stop()
-                    self.check_stopped_components()
-                    return
-                elif "Deadline Exceeded" in str(exception) or "Controller is down!" in str(exception):
+                if "Deadline Exceeded" in str(exception):
                     retry_object.begin()
                     retry_object.wait = wait_none()
                     return
 
         elif type(exception) in self.STOP_ACTION_ERRORS:
             self.logger.debug("Perform stop action")
             self.stop()
             self.check_stopped_components()
             return
 
         if type(exception) in self.NON_IMMEDIATE_ACTION_ERRORS:
             retry_object.wait = wait_fixed(self.RETRY_TIMEOUT)
-            if attempt == 3 or not attempt % 5:
+            if attempt == 3 or not attempt % 6:
                 self.logger.error(
                     f"Unable to connect {self.__class__.__name__}"
                     f" {self.process_name!r}. Error = {type(exception)} {exception}. Retrying..."
                 )
         else:
             retry_object.wait = wait_fixed(self.RETRY_TIMEOUT)
             self.logger.error(f"Unpredictable error during {self.__class__.__name__} execution")
@@ -243,46 +336,47 @@
 
     def check_stopped_components(self):
         if all(c.stop_event for c in self.components) and self.global_terminate_event:
             self.logger.debug("All components are stopped. Set global terminate event.")
             self.global_terminate_event.set()
 
     async def handle(self, task_status: TaskStatus = TASK_STATUS_IGNORED) -> NoReturn:
-        # Register on_stop actions
-        stop_task = asyncio.create_task(self.on_stop())
         await self.on_init()
 
         async for attempt in AsyncRetrying(
             reraise=True,
             retry=retry_if_exception_type((Exception,)),
             after=self.after_exception,
         ):
             with attempt:
-                if self.stop_event:
-                    return
+                if self.stop_event or self.global_terminate_event.is_set():
+                    break
 
                 await self.before_connect()
-                await self.handle_operations(task_status)
 
-        await stop_task
+                stop_task = asyncio.create_task(self.on_stop())
+                try:
+                    await asyncio.gather(self.handle_operations(task_status), stop_task)
+                finally:
+                    stop_task.cancel()
+
+        await self.on_terminate()
 
     def _set_keyboard_interrupt_handler(self) -> NoReturn:
         # Creating a handler
         def handle_unhandled_exception(exc_type, exc_value, exc_traceback):
             if issubclass(exc_type, KeyboardInterrupt):
                 # Will call default excepthook
                 sys.__excepthook__(exc_type, exc_value, exc_traceback)
                 return
                 # Create a critical level log message with info from the except hook.
             self.logger.error("Unhandled exception:", exc_info=(exc_type, exc_value, exc_traceback))
             for component in self.components:
                 component.stop()
-
-            if all(c.stop_event for c in self.components) and self.global_terminate_event:
-                self.global_terminate_event.set()
+            self.check_stopped_components()
 
         # Assign the excepthook to the handler
         sys.excepthook = handle_unhandled_exception
 
     async def check_endpoint_is_busy(self) -> bool:
         """Check if unix socket/host-port is already allocated"""
         async with self.connect_listener() as channel:
```

### Comparing `daffi-2.0.0/daffi/components/controller.py` & `daffi-2.2.0/daffi/components/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import asyncio
 from typing import NoReturn
 
-import grpc
 from anyio.abc import TaskStatus
 from anyio import create_task_group, move_on_after
 
 
 from daffi.utils import colors
 from daffi.utils.logger import get_daffi_logger
 from daffi.components import ComponentsBase
-from daffi.exceptions import GlobalContextError
+from daffi.exceptions import GlobalContextError, StopComponentError
 from daffi.components.proto.message import MessageFlag, messager_pb2, ServiceMessage
 from daffi.components.operations.controller_operations import ControllerOperations
 from daffi.components.operations.channel_store import ChannelPipe, MessageIterator, FreezableQueue
 
 
 class Controller(ComponentsBase):
 
@@ -44,31 +43,29 @@
         self.operations = ControllerOperations(logger=self.logger)
 
     async def on_stop(self) -> NoReturn:
         await super().on_stop()
         self.logger.debug("On stop event triggered")
         # Notify all nodes that controller has been terminated.
         await self.operations.on_controller_stopped(self.process_name)
-
         async with create_task_group() as sg:
-            with move_on_after(2):
-                sg.start_soon(FreezableQueue.clear_all)
-                await self.operations.wait_all_requests_done()
-            with move_on_after(2):
+            with move_on_after(0.5):
                 if self.listener:
-                    sg.start_soon(self.listener.stop, 2)
-        self.logger.info(f"{self.__class__.__name__} stopped.")
-        self._stopped = True
+                    sg.start_soon(self.listener.stop, 1)
+        await FreezableQueue.clear_all()
+        raise StopComponentError()
 
     async def before_connect(self) -> NoReturn:
         await FreezableQueue.clear_all()
         self.listener = None
+        if not getattr(self, "ping", None):
+            self.ping = asyncio.create_task(self.operations.on_ping())
 
-    def on_error(self) -> NoReturn:
-        pass
+    def on_error(self, exception: Exception) -> NoReturn:
+        self.logger.debug(f"{self.__class__.__name__} experienced error: {exception}. {type(exception)}")
 
     # ------------------------------------------------------------------------------------------------------------------
     # Message operations
     # ------------------------------------------------------------------------------------------------------------------
 
     async def handle_operations(self, task_status: TaskStatus) -> NoReturn:
         self.listener = await self.create_listener()
@@ -92,27 +89,27 @@
 
             elif msg.flag == MessageFlag.SUCCESS:
                 await self.operations.on_success(msg)
 
             elif msg.flag == MessageFlag.SCHEDULER_ERROR:
                 await self.operations.on_scheduler_error(msg)
 
-            elif msg.flag in (MessageFlag.BROADCAST, MessageFlag.STOP_REQUEST):
+            elif msg.flag == MessageFlag.BROADCAST:
                 await self.operations.on_broadcast(msg, self.process_name)
 
             elif msg.flag == MessageFlag.INIT_STREAM:
                 await self.operations.on_stream_init(msg)
 
             elif msg.flag == MessageFlag.STREAM_THROTTLE:
                 await self.operations.on_stream_throttle(msg)
 
             elif msg.flag == MessageFlag.RECEIVER_ERROR:
                 await self.operations.on_receiver_error(msg)
 
-        await self.operations.on_channel_close(channel, process_identificator)
+        await self.operations.on_channel_close(channel, process_identificator, self.execute_on_disconnect)
 
     async def communicate(self, request_iterator, context):
         try:
             ident = next(v for k, v in context.invocation_metadata() if k == "ident")
             # Modify ident in order to handle cases when Node and Controller are running in the same process
             ident = f"{ident}-node"
         except StopIteration:
```

### Comparing `daffi-2.0.0/daffi/components/node.py` & `daffi-2.2.0/daffi/components/node.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
+import time
+import asyncio
 from typing import Union, NoReturn
 from anyio import create_task_group
 from anyio._backends._asyncio import TaskGroup
 from anyio.abc import TaskStatus
 
 from daffi.utils import colors
 
 from daffi.utils.logger import get_daffi_logger
 from daffi.async_result import AsyncResult
 from daffi.components import ComponentsBase
-from daffi.components.proto.message import RpcMessage, ServiceMessage, MessageFlag
+from daffi.components.proto.message import RpcMessage, MessageFlag
 
 from daffi.components.scheduler import Scheduler
 from daffi.components.proto import messager_pb2_grpc as grpc_messager
 from daffi.exceptions import (
     UnableToFindCandidate,
     RemoteStoppedUnexpectedly,
     InitializationError,
+    ControllerUnavailable,
+    StopComponentError,
 )
-from daffi.settings import LOCAL_CALLBACK_MAPPING, WELL_KNOWN_CALLBACKS
 from daffi.components.operations.node_operations import NodeOperations
 from daffi.components.operations.channel_store import ChannelPipe, MessageIterator, FreezableQueue
 
 
 class Node(ComponentsBase):
 
     # ------------------------------------------------------------------------------------------------------------------
@@ -47,28 +50,31 @@
         self.scheduler = Scheduler(process_name=self.process_name, async_backend=self.async_backend)
 
     async def on_stop(self) -> NoReturn:
         await super().on_stop()
         self.logger.debug(f"On stop event triggered")
         await self.scheduler.on_scheduler_stop()
         self.operations.on_remote_error()
-
         if self.channel:
             await self.channel.clear_queue()
             await self.channel.stop()
         FreezableQueue.factory_remove(self.ident)
-        self.logger.info(f"{self.__class__.__name__} stopped.")
-        self._stopped = True
+        raise StopComponentError()
 
     async def before_connect(self) -> NoReturn:
         if not getattr(self, "channel", None):
             FreezableQueue.factory_remove(self.ident)
             self.channel = None
-
-    def on_error(self) -> NoReturn:
+        if getattr(self, "ping", None):
+            self.ping.cancel()
+        self.ping = None
+
+    def on_error(self, exception: Exception) -> NoReturn:
+        self.operations.handshake_ts = None
+        self.logger.debug(f"{self.__class__.__name__} experienced error: {exception}. {type(exception)}")
         if channel := getattr(self, "channel", None):
             channel.freeze(10)
         self.operations.on_remote_error()
 
     # ------------------------------------------------------------------------------------------------------------------
     # Message operations
     # ------------------------------------------------------------------------------------------------------------------
@@ -85,30 +91,29 @@
                 send_iterator=message_iterator, receive_iterator=receive_iterator, ident=self.ident
             )
             self.operations.channel = self.channel
 
             async with create_task_group() as sg:
                 sg.start_soon(self.read_commands, task_status, sg, stub)
                 sg.start_soon(self.read_streams, sg, stub)
+                self.ping = asyncio.create_task(self.operations.ping_task(sg))
+            # To retry connecting to the controller after the task group scope was cancelled due to an error,
+            # we need to generate an error that can be handled by the upstream exception wrapper.
+            raise ControllerUnavailable()
 
     async def read_commands(self, task_status: TaskStatus, sg: TaskGroup, stub):
-        local_mapping_without_well_known_callbacks = {
-            k: v.simplified() for k, v in LOCAL_CALLBACK_MAPPING.items() if k not in WELL_KNOWN_CALLBACKS
-        }
-        await self.channel.send(
-            ServiceMessage(
-                flag=MessageFlag.HANDSHAKE,
-                transmitter=self.process_name,
-                data=local_mapping_without_well_known_callbacks,
-            )
-        )
+        self.operations.last_ping_ts = time.time()
 
+        # Send initial handshake message
+        await self.operations.send_handshake(process_name=self.process_name)
         async for msg in self.channel:
             if msg.flag in (MessageFlag.HANDSHAKE, MessageFlag.UPDATE_CALLBACKS):
-                await self.operations.on_handshake(msg, task_status, self.process_name, self.info)
+                await self.operations.on_handshake(
+                    msg, task_status, self.process_name, self.info, self.execute_on_connect
+                )
 
             elif msg.flag in (MessageFlag.REQUEST, MessageFlag.BROADCAST):
                 await self.operations.on_request(msg, sg, self.process_name, self.scheduler)
 
             elif msg.flag == MessageFlag.SUCCESS:
                 await self.operations.on_success(msg, self.scheduler)
 
@@ -123,29 +128,29 @@
                 msg.loads()
                 if msg.flag == MessageFlag.REMOTE_STOPPED_UNEXPECTEDLY:
                     msg.error._awaited_error_type = RemoteStoppedUnexpectedly
                 else:
                     msg.error._awaited_error_type = UnableToFindCandidate
                 await self.operations.on_unable_to_find(msg)
 
-            elif msg.flag == MessageFlag.STOP_REQUEST:
-                await self.operations.on_stop_request()
-
             elif msg.flag == MessageFlag.INIT_STREAM:
                 await self.operations.on_stream_init(msg, stub, sg, self.process_name)
 
             elif msg.flag == MessageFlag.STREAM_ERROR:
                 await self.operations.on_stream_error(msg)
 
             elif msg.flag == MessageFlag.STREAM_THROTTLE:
                 await self.operations.on_stream_throttle(msg)
 
             elif msg.flag == MessageFlag.CONTROLLER_STOPPED_UNEXPECTEDLY:
                 self.operations.on_remote_error()
 
+            elif msg.flag == MessageFlag.PING:
+                await self.operations.on_ping()
+
     def send_threadsave(self, msg: RpcMessage, eta: Union[int, float]):
         """Send message outside of node executor scope."""
         self.channel.send_threadsave(msg, eta)
 
     def send_and_register_result(self, msg: RpcMessage) -> AsyncResult:
         if msg.return_result is False:
             InitializationError(
```

### Comparing `daffi-2.0.0/daffi/components/scheduler.py` & `daffi-2.2.0/daffi/components/scheduler.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/operations/channel_store.py` & `daffi-2.2.0/daffi/components/operations/channel_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/operations/controller_operations.py` & `daffi-2.2.0/daffi/components/operations/controller_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
 import asyncio
-from typing import Dict
-
-from anyio import sleep
+from typing import Dict, Callable, Any, Optional
 
 from daffi.settings import WELL_KNOWN_CALLBACKS, DEBUG
 from daffi.utils.custom_types import K, GlobalCallback
 from daffi.utils.misc import search_remote_callback_in_mapping, call_after
 from daffi.components.operations.streams_store import StreamPairStore
 from daffi.components.operations.channel_store import ChannelStore, ChannelPipe, FreezableQueue
 from daffi.components.proto.message import RpcMessage, ServiceMessage, MessageFlag, RemoteError
@@ -26,41 +24,48 @@
         self.controller_callback_mapping: Dict[K, Dict[K, GlobalCallback]] = dict()
         self.closed_procs: Dict[str, asyncio.Task] = dict()
 
         self.awaited_procs = OneToOneCallStore()
         self.awaited_broadcast_procs = OneToManyCallStore()
         self.awaited_stream_procs = OneToManyCallStore()
 
-    async def wait_all_requests_done(self):
-        while self.awaited_procs or self.awaited_broadcast_procs or self.awaited_stream_procs:
-            await sleep(0.1)
-
     async def on_controller_stopped(self, proc_name):
         async for proc, chan in self.channel_store.iterate():
             if proc != proc_name:
                 # Send updated self.controller_callback_mapping to all processes except transmitter process.
                 await chan.send(ServiceMessage(flag=MessageFlag.CONTROLLER_STOPPED_UNEXPECTEDLY, receiver=proc))
 
-    async def on_channel_close(self, channel: ChannelPipe, process_identificator: str):
+    async def on_channel_close(
+        self, channel: ChannelPipe, process_identificator: str, on_disconnect: Callable[[str], Any]
+    ):
         self.logger.debug(f"Channel {channel} (process={process_identificator}) is locked before closing")
         channel.lock()
         # Give 5 seconds to reconnect. If process unable to recconect within 5 seconds then channel will be
         # deleted and all other processes will be notified channel is not available anymore.
         if process_identificator not in self.closed_procs:
             self.closed_procs[process_identificator] = await call_after(
-                5, self._on_channel_close, channel=channel, process_identificator=process_identificator
+                5,
+                self._on_channel_close,
+                channel=channel,
+                process_identificator=process_identificator,
+                on_disconnect=on_disconnect,
             )
 
     async def on_all_channels_close(self):
         async for proc, chan in self.channel_store.iterate():
             await self._on_channel_close(chan, chan.ident)
 
-    async def _on_channel_close(self, channel: ChannelPipe, process_identificator: str):
+    async def _on_channel_close(
+        self, channel: ChannelPipe, process_identificator: str, on_disconnect: Optional[Callable[[str], Any]] = None
+    ):
+        self.logger.debug(f"Lock expired. Channel {channel} (process={process_identificator}) is about to be deleted.")
         self.closed_procs.pop(process_identificator, None)
         del_proc = await self.channel_store.find_process_name_by_channel(channel)
+        if on_disconnect:
+            await on_disconnect(del_proc)
         await self.channel_store.delete_channel(del_proc)
         self.controller_callback_mapping.pop(del_proc, None)
         FreezableQueue.factory_remove(process_identificator)
 
         # Delete RpcMessage pointers that deleted process expects to obtain.
         awaited_trmrs_for_single_message = self.awaited_procs.on_delete(del_proc)
         async for proc, chan in self.channel_store.iterate():
@@ -243,28 +248,28 @@
                         f" message: {msg}.\n"
                         f"Awaited stream entries: { self.awaited_stream_procs}.\n"
                         f"Awaited broadcast entries: {self.awaited_broadcast_procs}.\n"
                         f" Awaited one-to-one entries: {self.awaited_procs}."
                     )
                 msg.set_error(RemoteError(info=info))
                 await chan.send(msg)
-                self.logger.error(info)
+                self.logger.debug(info)
 
         else:
             if chan := await self.channel_store.get_chan(transmitter):
                 await chan.send(msg)
             else:
-                logging.error(f"Unable to send calculated result. Process {transmitter!r}.")
+                logging.debug(f"Unable to send result. Process {transmitter!r}.")
 
     async def on_scheduler_error(self, msg: RpcMessage):
         # Dont care about RpcMessage uuid. Scheduler tasks are long running processes. Sheduler can report about error
         # multiple times.
         self.awaited_procs.pop(msg.uuid, None)
         if not (chan := await self.channel_store.get_chan(msg.receiver)):
-            logging.error(f"Unable to send calculated result. Process {msg.receiver!r} is disconnected.")
+            logging.error(f"Unable to send result. Process {msg.receiver!r} is disconnected.")
         else:
             msg.flag = MessageFlag.SUCCESS
             await chan.send(msg)
 
     async def on_broadcast(self, msg: RpcMessage, process_name: str):
 
         transmitter = msg.transmitter
@@ -334,14 +339,23 @@
                 await trans_chan.send(msg)
             self.logger.error(info)
 
     async def on_stream_throttle(self, msg: ServiceMessage):
         if chan := await self.channel_store.get_chan(msg.receiver):
             await chan.send(msg)
 
+    async def on_ping(self):
+        msg = ServiceMessage(flag=MessageFlag.PING)
+        while True:
+            # Send ping message every 12 seconds
+            async for _, chan in self.channel_store.iterate():
+                # Send ping message to all processes.
+                await chan.send(msg)
+            await asyncio.sleep(5)
+
     async def on_receiver_error(self, msg: ServiceMessage):
         """
         MessageFlag.RECEIVER_ERROR
         Give extra information about why error happened.
         At this moment this method is not used since there is no implementation on Node side.
         But it might be helpful for debugging. That is why it is here.
         """
```

### Comparing `daffi-2.0.0/daffi/components/operations/freezable_queue.py` & `daffi-2.2.0/daffi/components/operations/freezable_queue.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/operations/node_operations.py` & `daffi-2.2.0/daffi/components/operations/node_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import time
 import pickle
 import logging
 import asyncio
-from typing import NoReturn, Dict
+from typing import NoReturn, Dict, Callable, Any
 from queue import Queue as thQueue
 
 from anyio import run
 from anyio._backends._asyncio import TaskGroup
 from anyio.abc import TaskStatus, CancelScope
 from grpc.aio._call import AioRpcError
 
@@ -16,14 +16,15 @@
 from daffi.components.proto.message import RpcMessage, ServiceMessage, MessageFlag, RemoteError, messager_pb2, Message
 
 from daffi.components.scheduler import Scheduler
 from daffi.utils.misc import run_in_threadpool, run_from_working_thread, iterate_in_threadpool
 
 from daffi.settings import (
     LOCAL_CALLBACK_MAPPING,
+    WELL_KNOWN_CALLBACKS,
 )
 from daffi.components.operations.channel_store import ChannelPipe
 from daffi.exceptions import StopComponentError, GlobalContextError, RemoteStoppedUnexpectedly
 from daffi.components.operations.streams_store import StreamPairStore
 
 import tblib.pickling_support
 
@@ -35,44 +36,62 @@
 
     def __init__(self, logger: logging.Logger, async_backend: str):
         self.logger = logger
         self._channel = None
         self.stream_store = StreamPairStore()
         self.async_backend = async_backend
         self.node_callback_mapping: Dict[K, Dict[K, GlobalCallback]] = dict()
-        self.init_ts = None  # Timestamp of handshake.
+        self.handshake_ts = None  # Timestamp of handshake.
+        self.last_ping_ts = time.time()
 
     @property
     def channel(self) -> ChannelPipe:
         return self._channel
 
     @channel.setter
     def channel(self, channel: ChannelPipe) -> NoReturn:
         self._channel = channel
         self._channel.proceed()
 
-    async def on_handshake(self, msg: ServiceMessage, task_status: TaskStatus, process_name: str, info: str):
+    async def send_handshake(self, process_name: str):
+        """Send initial handshake message"""
+        local_mapping_without_well_known_callbacks = {
+            k: v.simplified() for k, v in LOCAL_CALLBACK_MAPPING.items() if k not in WELL_KNOWN_CALLBACKS
+        }
+        await self.channel.send(
+            ServiceMessage(
+                flag=MessageFlag.HANDSHAKE,
+                transmitter=process_name,
+                data=local_mapping_without_well_known_callbacks,
+            )
+        )
+
+    async def on_handshake(
+        self, msg: ServiceMessage, task_status: TaskStatus, process_name: str, info: str, on_connect: Callable[[], Any]
+    ):
         try:
             msg.loads()
         except Exception as e:
             if msg.transmitter == process_name:
                 self.logger.error(f"{e}")
                 raise StopComponentError()
         else:
             self.node_callback_mapping = msg.data
-            if msg.transmitter == process_name and msg.flag == MessageFlag.HANDSHAKE:
-                # Prevent flooding to terminal if re-connections are happen too ofter.
-                if not self.init_ts or (time.time() - self.init_ts) > 2:
-                    self.init_ts = time.time()
-                    self.logger.info(
-                        f"Node has been started successfully. Process identificator: {process_name!r}. Connection info: {info}"
-                    )
+            if msg.transmitter == process_name and msg.flag == MessageFlag.HANDSHAKE and not self.handshake_ts:
+                self.handshake_ts = time.time()
+                self.logger.info(
+                    f"Node has been started successfully. Process identificator: {process_name!r}. Connection info: {info}"
+                )
                 if task_status._future._state == "PENDING":
                     # Consider Node to be started only after handshake response is received.
                     task_status.started("STARTED")
+                # It is important to execute `on_connect` after receiving handshake response from Controller as
+                # `on_connect` internal logic might rely on data obtained from remote processes so current process
+                # should be aware of all available callbacks that exists in remote processes.
+                await on_connect()
 
     async def on_request(
         self,
         msg: RpcMessage,
         sg: TaskGroup,
         process_name: str,
         scheduler: Scheduler,
@@ -114,15 +133,15 @@
 
     async def on_success(self, msg: RpcMessage, scheduler: Scheduler):
         msg.loads()
         error = msg.error
         if msg.return_result:
             ares = ResultInf._awaited_results.get(msg.uuid)
             if not ares and not error:
-                self.logger.warning(f"Result {msg.uuid} was deleted by timeout")
+                self.logger.debug(f"Result {msg.uuid} was deleted by timeout")
             elif not ares and error:
                 # Result already taken by timeout. No need to raise error but need to notify about
                 # finally remote call returned exception.
                 error.show_in_log(logger=self.logger)
 
             else:
                 result = error if error else msg.func_args[0]
@@ -152,18 +171,14 @@
         msg.loads()
         if msg.return_result:
             if ares := ResultInf._awaited_results.get(msg.uuid):
                 ares._set_and_trigger(msg.uuid, msg.error, completed=True)
         else:
             self.logger.error(msg.error.info)
 
-    async def on_stop_request(self):
-        self.logger.debug(f"Termination signal received.")
-        raise StopComponentError()
-
     async def on_stream_init(self, msg: RpcMessage, stub, sg, process_name):
         msg.loads()
         remote_callback = LOCAL_CALLBACK_MAPPING.get(msg.func_name)
         if not remote_callback:
             info = (
                 f"Function {msg.func_name!r} is not registered as callback locally."
                 f" Make sure python loaded module where callback is located."
@@ -199,14 +214,35 @@
 
     async def on_stream_throttle(self, msg: ServiceMessage):
         msg.loads()
         stream_pair_group = self.stream_store.stream_pair_group_store.get(str(msg.uuid))
         if stream_pair_group:
             stream_pair_group.throttle_time = msg.data
 
+    async def on_ping(self):
+        """Update the timestamp to reflect the most recent ping signal sent by the controller."""
+        self.logger.debug(f"Received `ping` signal from controller")
+        self.last_ping_ts = time.time()
+
+    async def ping_task(self, sg: TaskGroup):
+        """
+        Recurring task that monitors the timestamp of the last ping signal sent by the controller.
+        If this timestamp is deemed too old, the entire Node process will be restarted,
+        prompting new attempts to establish a connection with the controller.
+        """
+        while True:
+            await asyncio.sleep(5)
+            time_since_last_ping = time.time() - self.last_ping_ts
+            self.logger.debug(f"Time since last ping: {time_since_last_ping}")
+            if time_since_last_ping > 15:
+                self.on_remote_error()
+                await sg.cancel_scope.cancel()
+                sg.cancel_scope.deadline = 1
+                break
+
     def on_remote_error(self):
         err = RemoteError(
             info="Lost connection to Controller.",
             _awaited_error_type=RemoteStoppedUnexpectedly,
         )
         for msg_uuid, ares in ResultInf._awaited_results.items():
             ResultInf._set_and_trigger(msg_uuid, err, completed=True)
@@ -287,15 +323,15 @@
 
         stream_poller = asyncio.create_task(_stream_poller())
         try:
             await run_in_threadpool(_stream_executor)
             self.logger.debug(f"Stop streaming process for function: {message.func_name}. Process = {process_name}")
         except Exception as e:
             err_msg = (
-                f"Exception while streaming to function {message.func_name!r} on remote executor {process_name!r}. {e}"
+                f"Exception while streaming to function {message.func_name!r} on remote executor [{process_name}]. {e}"
             )
             error = RemoteError(info=err_msg, traceback=pickle.dumps(sys.exc_info()))
             self.logger.error(err_msg)
         finally:
             stream_poller.cancel()
 
         message_to_return = RpcMessage(
@@ -331,18 +367,18 @@
                 result = await run_from_working_thread(self.async_backend, remote_callback, *fn_args, **fn_kwargs)
             else:
                 result = await run_in_threadpool(remote_callback, *fn_args, **fn_kwargs)
         except TypeError as e:
             if "were given" in str(e) or "got an unexpected" in str(e) or "missing" in str(e):
                 info = f"{e}. Function signature is: {message.func_name}{remote_callback.signature}: ..."
             else:
-                info = f"Exception while processing function {message.func_name!r} on remote executor. {e}"
+                info = f"Exception while processing function {message.func_name!r} on remote executor [{process_name}]. {e}"
             error = RemoteError(info=info, traceback=pickle.dumps(sys.exc_info()))
         except Exception as e:
-            info = f"Exception while processing function {message.func_name!r} on remote executor. {e}"
+            info = f"Exception while processing function {message.func_name!r} on remote executor [{process_name}]. {e}"
             self.logger.error(info)
             error = RemoteError(info=info, traceback=pickle.dumps(sys.exc_info()))
 
         if message.return_result:
             try:
                 message_to_return = RpcMessage(
                     **_default_msg_kwargs,
@@ -410,18 +446,18 @@
                     await self.channel.send(message_to_return)
                     return
 
         except TypeError as e:
             if "were given" in str(e) or "got an unexpected" in str(e) or "missing" in str(e):
                 info = f"{e}. Function signature is: {message.func_name}{remote_callback.signature}: ..."
             else:
-                info = f"Exception while processing function {message.func_name!r} on remote executor. {e}"
+                info = f"Exception while processing function {message.func_name!r} on remote executor [{process_name}]. {e}"
             error = RemoteError(info=info, traceback=pickle.dumps(sys.exc_info()))
         except Exception as e:
-            info = f"Exception while processing function {message.func_name!r} on remote executor. {e}"
+            info = f"Exception while processing function {message.func_name!r} on remote executor [{process_name}]. {e}"
             self.logger.error(info)
             error = RemoteError(info=info, traceback=pickle.dumps(sys.exc_info()))
 
         if error:
             message_to_return = RpcMessage(
                 **_default_msg_kwargs,
                 error=error,
```

### Comparing `daffi-2.0.0/daffi/components/operations/streams_store.py` & `daffi-2.2.0/daffi/components/operations/streams_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/operations/task_waiter.py` & `daffi-2.2.0/daffi/components/operations/task_waiter.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/operations/ttl_store.py` & `daffi-2.2.0/daffi/components/operations/ttl_store.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/components/proto/message.py` & `daffi-2.2.0/daffi/components/proto/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,20 @@
     UPDATE_CALLBACKS = 4
     UNABLE_TO_FIND_CANDIDATE = 5
     UNABLE_TO_FIND_PROCESS = 6
     REMOTE_STOPPED_UNEXPECTEDLY = 7
     SCHEDULER_ERROR = 8
     SCHEDULER_ACCEPT = 9
     BROADCAST = 10
-    STOP_REQUEST = 11
-    INIT_STREAM = 12
-    STREAM_ERROR = 13
-    STREAM_THROTTLE = 14
-    RECEIVER_ERROR = 15
-    CONTROLLER_STOPPED_UNEXPECTEDLY = 16
+    INIT_STREAM = 11
+    STREAM_ERROR = 12
+    STREAM_THROTTLE = 13
+    RECEIVER_ERROR = 14
+    CONTROLLER_STOPPED_UNEXPECTEDLY = 15
+    PING = 16
 
 
 class Message(ABC):
 
     __data_fields__: ClassVar[Set[str]] = {}
 
     @staticmethod
```

### Comparing `daffi-2.0.0/daffi/components/proto/messager.proto` & `daffi-2.2.0/daffi/components/proto/messager.proto`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,14 @@
   UPDATE_CALLBACKS = 4;
   UNABLE_TO_FIND_CANDIDATE = 5;
   UNABLE_TO_FIND_PROCESS = 6;
   REMOTE_STOPPED_UNEXPECTEDLY = 7;
   SCHEDULER_ERROR = 8;
   SCHEDULER_ACCEPT = 9;
   BROADCAST = 10;
-  STOP_REQUEST = 11;
-  INIT_STREAM = 12;
-  STREAM_ERROR = 13;
-  STREAM_THROTTLE = 14;
-  RECEIVER_ERROR = 15;
-  CONTROLLER_STOPPED_UNEXPECTEDLY = 16;
+  INIT_STREAM = 11;
+  STREAM_ERROR = 12;
+  STREAM_THROTTLE = 13;
+  RECEIVER_ERROR = 14;
+  CONTROLLER_STOPPED_UNEXPECTEDLY = 15;
+  PING = 16;
 }
```

### Comparing `daffi-2.0.0/daffi/components/proto/messager_pb2.py` & `daffi-2.2.0/daffi/components/proto/messager_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x0emessager.proto"\x07\n\x05\x45mpty"Z\n\x07Message\x12\x1e\n\trpc_realm\x18\x01 \x01(\x0b\x32\t.RpcRealmH\x00\x12&\n\rservice_realm\x18\x02 \x01(\x0b\x32\r.ServiceRealmH\x00\x42\x07\n\x05realm"\xe9\x01\n\x08RpcRealm\x12\x1a\n\x04\x66lag\x18\x01 \x01(\x0e\x32\x0c.MessageFlag\x12\x0c\n\x04uuid\x18\x02 \x01(\r\x12\x13\n\x0btransmitter\x18\x03 \x01(\t\x12\x10\n\x08receiver\x18\x04 \x01(\t\x12\x11\n\tfunc_name\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x15\n\rreturn_result\x18\x07 \x01(\x08\x12\x17\n\x06period\x18\x08 \x01(\x0b\x32\x07.Period\x12\x0f\n\x07timeout\x18\t \x01(\x04\x12\x11\n\tcompleted\x18\n \x01(\x08\x12\x17\n\x0f\x63omplete_marker\x18\x0b \x01(\x08"\x86\x01\n\x0cServiceRealm\x12\x1a\n\x04\x66lag\x18\x01 \x01(\x0e\x32\x0c.MessageFlag\x12\x0c\n\x04uuid\x18\x02 \x01(\r\x12\x13\n\x0btransmitter\x18\x03 \x01(\t\x12\x10\n\x08receiver\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\x12\x17\n\x0f\x63omplete_marker\x18\x06 \x01(\x08""\n\x11IntervalCondition\x12\r\n\x05value\x18\x01 \x01(\x01" \n\x0f\x41tTimeCondition\x12\r\n\x05value\x18\x01 \x03(\x01"b\n\x06Period\x12&\n\x08interval\x18\x01 \x01(\x0b\x32\x12.IntervalConditionH\x00\x12#\n\x07\x61t_time\x18\x02 \x01(\x0b\x32\x10.AtTimeConditionH\x00\x42\x0b\n\tcondition*\xef\x02\n\x0bMessageFlag\x12\t\n\x05\x45MPTY\x10\x00\x12\r\n\tHANDSHAKE\x10\x01\x12\x0b\n\x07REQUEST\x10\x02\x12\x0b\n\x07SUCCESS\x10\x03\x12\x14\n\x10UPDATE_CALLBACKS\x10\x04\x12\x1c\n\x18UNABLE_TO_FIND_CANDIDATE\x10\x05\x12\x1a\n\x16UNABLE_TO_FIND_PROCESS\x10\x06\x12\x1f\n\x1bREMOTE_STOPPED_UNEXPECTEDLY\x10\x07\x12\x13\n\x0fSCHEDULER_ERROR\x10\x08\x12\x14\n\x10SCHEDULER_ACCEPT\x10\t\x12\r\n\tBROADCAST\x10\n\x12\x10\n\x0cSTOP_REQUEST\x10\x0b\x12\x0f\n\x0bINIT_STREAM\x10\x0c\x12\x10\n\x0cSTREAM_ERROR\x10\r\x12\x13\n\x0fSTREAM_THROTTLE\x10\x0e\x12\x12\n\x0eRECEIVER_ERROR\x10\x0f\x12#\n\x1f\x43ONTROLLER_STOPPED_UNEXPECTEDLY\x10\x10\x32\x92\x01\n\x0fMessagerService\x12%\n\x0b\x63ommunicate\x12\x08.Message\x1a\x08.Message(\x01\x30\x01\x12*\n\x14stream_to_controller\x12\x08.Message\x1a\x06.Empty(\x01\x12,\n\x16stream_from_controller\x12\x06.Empty\x1a\x08.Message0\x01\x62\x06proto3'
+    b'\n\x0emessager.proto"\x07\n\x05\x45mpty"Z\n\x07Message\x12\x1e\n\trpc_realm\x18\x01 \x01(\x0b\x32\t.RpcRealmH\x00\x12&\n\rservice_realm\x18\x02 \x01(\x0b\x32\r.ServiceRealmH\x00\x42\x07\n\x05realm"\xe9\x01\n\x08RpcRealm\x12\x1a\n\x04\x66lag\x18\x01 \x01(\x0e\x32\x0c.MessageFlag\x12\x0c\n\x04uuid\x18\x02 \x01(\r\x12\x13\n\x0btransmitter\x18\x03 \x01(\t\x12\x10\n\x08receiver\x18\x04 \x01(\t\x12\x11\n\tfunc_name\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\x0c\x12\x15\n\rreturn_result\x18\x07 \x01(\x08\x12\x17\n\x06period\x18\x08 \x01(\x0b\x32\x07.Period\x12\x0f\n\x07timeout\x18\t \x01(\x04\x12\x11\n\tcompleted\x18\n \x01(\x08\x12\x17\n\x0f\x63omplete_marker\x18\x0b \x01(\x08"\x86\x01\n\x0cServiceRealm\x12\x1a\n\x04\x66lag\x18\x01 \x01(\x0e\x32\x0c.MessageFlag\x12\x0c\n\x04uuid\x18\x02 \x01(\r\x12\x13\n\x0btransmitter\x18\x03 \x01(\t\x12\x10\n\x08receiver\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x05 \x01(\x0c\x12\x17\n\x0f\x63omplete_marker\x18\x06 \x01(\x08""\n\x11IntervalCondition\x12\r\n\x05value\x18\x01 \x01(\x01" \n\x0f\x41tTimeCondition\x12\r\n\x05value\x18\x01 \x03(\x01"b\n\x06Period\x12&\n\x08interval\x18\x01 \x01(\x0b\x32\x12.IntervalConditionH\x00\x12#\n\x07\x61t_time\x18\x02 \x01(\x0b\x32\x10.AtTimeConditionH\x00\x42\x0b\n\tcondition*\xe7\x02\n\x0bMessageFlag\x12\t\n\x05\x45MPTY\x10\x00\x12\r\n\tHANDSHAKE\x10\x01\x12\x0b\n\x07REQUEST\x10\x02\x12\x0b\n\x07SUCCESS\x10\x03\x12\x14\n\x10UPDATE_CALLBACKS\x10\x04\x12\x1c\n\x18UNABLE_TO_FIND_CANDIDATE\x10\x05\x12\x1a\n\x16UNABLE_TO_FIND_PROCESS\x10\x06\x12\x1f\n\x1bREMOTE_STOPPED_UNEXPECTEDLY\x10\x07\x12\x13\n\x0fSCHEDULER_ERROR\x10\x08\x12\x14\n\x10SCHEDULER_ACCEPT\x10\t\x12\r\n\tBROADCAST\x10\n\x12\x0f\n\x0bINIT_STREAM\x10\x0b\x12\x10\n\x0cSTREAM_ERROR\x10\x0c\x12\x13\n\x0fSTREAM_THROTTLE\x10\r\x12\x12\n\x0eRECEIVER_ERROR\x10\x0e\x12#\n\x1f\x43ONTROLLER_STOPPED_UNEXPECTEDLY\x10\x0f\x12\x08\n\x04PING\x10\x10\x32\x92\x01\n\x0fMessagerService\x12%\n\x0b\x63ommunicate\x12\x08.Message\x1a\x08.Message(\x01\x30\x01\x12*\n\x14stream_to_controller\x12\x08.Message\x1a\x06.Empty(\x01\x12,\n\x16stream_from_controller\x12\x06.Empty\x1a\x08.Message0\x01\x62\x06proto3'
 )
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "messager_pb2", globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     _MESSAGEFLAG._serialized_start = 663
-    _MESSAGEFLAG._serialized_end = 1030
+    _MESSAGEFLAG._serialized_end = 1022
     _EMPTY._serialized_start = 18
     _EMPTY._serialized_end = 25
     _MESSAGE._serialized_start = 27
     _MESSAGE._serialized_end = 117
     _RPCREALM._serialized_start = 120
     _RPCREALM._serialized_end = 353
     _SERVICEREALM._serialized_start = 356
     _SERVICEREALM._serialized_end = 490
     _INTERVALCONDITION._serialized_start = 492
     _INTERVALCONDITION._serialized_end = 526
     _ATTIMECONDITION._serialized_start = 528
     _ATTIMECONDITION._serialized_end = 560
     _PERIOD._serialized_start = 562
     _PERIOD._serialized_end = 660
-    _MESSAGERSERVICE._serialized_start = 1033
-    _MESSAGERSERVICE._serialized_end = 1179
+    _MESSAGERSERVICE._serialized_start = 1025
+    _MESSAGERSERVICE._serialized_end = 1171
 # @@protoc_insertion_point(module_scope)
```

### Comparing `daffi-2.0.0/daffi/components/proto/messager_pb2_grpc.py` & `daffi-2.2.0/daffi/components/proto/messager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/decorators/_base.py` & `daffi-2.2.0/daffi/decorators/_base.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/decorators/_callback.py` & `daffi-2.2.0/daffi/decorators/_callback.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/decorators/_fetcher.py` & `daffi-2.2.0/daffi/decorators/_fetcher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/registry/_base.py` & `daffi-2.2.0/daffi/registry/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,48 +3,52 @@
 
 from daffi.ipc import Ipc
 from daffi.utils import colors
 from daffi.utils.logger import get_daffi_logger
 
 logger = get_daffi_logger("registry", colors.blue)
 
-
 _base_class_defined = False
 
 
 class RegistryMeta(ABCMeta):
     def __new__(mcs, cls_name: str, bases: Tuple[Type[Any], ...], namespace: Dict[str, Any], **kwargs: Any) -> Type:
 
         if _base_class_defined:
             daffi_mro = []
             is_registry_class = cls_name in ("BaseRegistry", "Callback", "Fetcher")
             auto_init = None
             if not is_registry_class:
                 from daffi.registry import Callback
                 from daffi.registry import Fetcher
 
-                for _cls in (Fetcher, Callback):
-                    if _cls in bases:
+                _registry_methods = (Fetcher, Callback)
+
+                for _cls in bases:
+                    if hasattr(_cls, "__daffi_mro__"):
+                        # Take `__daffi_mro__` from base class if exists.
+                        daffi_mro.extend(_cls.__daffi_mro__)
+
+                    if _cls in _registry_methods and _cls not in daffi_mro:
                         daffi_mro.append(_cls)
 
                 if (auto_init := namespace.get("auto_init", None)) is None:
                     for base in bases:
-                        if auto_init := getattr(base, "auto_init", None) is not None:
+                        if (auto_init := getattr(base, "auto_init", None)) is not None:
                             namespace.update(auto_init=auto_init)
                             break
             if len(daffi_mro) == 2:
                 # Disable auto init forcibly if class is inherited from both `Callback` and `Fetcher`
                 auto_init = False
                 namespace.update(auto_init=auto_init)
             # Store all parent daffi classes to `__daffi_mro__` class attribute
             namespace.update(__daffi_mro__=daffi_mro)
             cls = _type = super().__new__(mcs, cls_name, bases, namespace, **kwargs)  # type: ignore
 
             if not is_registry_class:
-
                 if auto_init:
                     _type = _type()
 
                 for _initializator_cls in daffi_mro:
                     _initializator_cls._init_class(cls, _type)
             return cls
         else:
```

### Comparing `daffi-2.0.0/daffi/registry/_callback.py` & `daffi-2.2.0/daffi/registry/_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Callback(BaseRegistry):
     """
     Remote callback group representation. All public methods of class inherited from Callbacks become remote callbacks
     identified by they names.
     """
 
     # If auto_init=True then class will be implicitly instantiated.
-    auto_init: ClassVar[bool] = True
+    auto_init: ClassVar[bool] = False
 
     @staticmethod
     def _init_class(cls, instance_or_type) -> Union[Type, "Callback"]:
         """
         Register all public methods of class as callbacks.
         Args:
             instance_or_type: class type or class instance. This argument depends on `auto_init` value of base class
@@ -67,15 +67,15 @@
                 is_static=str(is_static_or_class_method) == "static",
                 is_generator=isgeneratorfunction(method),
             )
             name_in_mapping = method_alias in LOCAL_CALLBACK_MAPPING
             LOCAL_CALLBACK_MAPPING[method_alias] = cb
             if not name_in_mapping:
                 logger.info(
-                    f"callback {method_alias!r} is registered"
+                    f"callback {method_alias!r} <class {cls.__name__}> is registered"
                     + ("" if klass else f" (required {cls.__name__} initialization)")
                 )
 
             _updated = True
 
         if _updated:
             cls._update_callbacks()
```

### Comparing `daffi-2.0.0/daffi/registry/_fetcher.py` & `daffi-2.2.0/daffi/registry/_fetcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 # If proxy=True then method works as proxy (without body execution).
                 # IOW when proxy=True all provided arguments will be passed to remote callback as is.
                 proxy_=is_proxy,
                 exec_modifier_=cls.exec_modifier,
                 is_generator=is_generator,
             )
             LOCAL_FETCHER_MAPPING[f"{cls.__name__}-{origin_method_name}"] = cb
-            logger.info(f"fetcher {origin_method_name!r} is registered. (proxy={is_proxy})")
+            logger.info(f"fetcher {origin_method_name!r} <class {cls.__name__}> is registered. (proxy={is_proxy})")
 
         return instance_or_type
 
     @classmethod
     def _init_function(
         cls,
         fn: Callable[..., Any],
@@ -109,14 +109,18 @@
         exec_modifier: Union[FG, BG, BROADCAST, PERIOD] = FG,
     ) -> FetcherExecutor:
         """Register one function as remote fetcher (This method is used in `fetcher` decorator)."""
         from daffi.decorators import callback
 
         is_async = is_generator = is_proxy = False
 
+        if hasattr(fn, "__func__"):
+            # Bypass staticmethod/classmethod decorators
+            fn = fn.__func__
+
         if isinstance(fn, callback):
             is_async = fn._fn.is_async
             fn = fn._fn.wrapped
             is_generator = False
             # Enable proxy forcibly if function is used as fetcher and callback at once.
             # In this case function's body is used only by callback part
             is_proxy = True
```

### Comparing `daffi-2.0.0/daffi/utils/colors.py` & `daffi-2.2.0/daffi/utils/colors.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/utils/debug.py` & `daffi-2.2.0/daffi/utils/debug.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/daffi/utils/func_validation.py` & `daffi-2.2.0/daffi/utils/func_validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import inspect
 from typing import Callable, Any, Dict
 from daffi.utils.custom_types import P
+from daffi.exceptions import InitializationError
 
 
 def get_class_methods(klass):
     return [
         member
         for member in [getattr(klass, attr) for attr in dir(klass)]
         if inspect.isfunction(member) or inspect.ismethod(member)
@@ -83,15 +84,18 @@
     elif hasattr(func, "func_name"):
         name = func.func_name
     elif hasattr(func, "__name__"):
         name = func.__name__
     elif hasattr(func, "origin_name_"):
         name = func.origin_name_
     else:
-        name = "unknown"
+        raise InitializationError(
+            "Unable to retrieve fetcher name. If you have applied additional decorators"
+            " to the decorated function consider modifying the order of the decorators."
+        )
     # Hack to detect functions not defined at the module-level
     if hasattr(func, "func_globals") and name in func.func_globals:
         if func.func_globals[name] is not func:
             name = "%s-alias" % name
     if inspect.ismethod(func):
         # We need to add the name of the class
         if hasattr(func, "im_class"):
```

### Comparing `daffi-2.0.0/daffi/utils/logger.py` & `daffi-2.2.0/daffi/utils/logger.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,19 +16,21 @@
         return super().debug(msg=msg, *args, **kwargs)
 
 
 class ColoredFormatter(logging.Formatter):
     """A logging.Formatter which prints colored WARNING and ERROR messages"""
 
     def get_level_message(self, record):
-        if record.levelno >= logging.ERROR:
-            return colors.red(record.levelname)
-        if record.levelno >= logging.WARNING:
-            return colors.yellow(record.levelname)
-        return record.levelname
+        if record.levelno <= logging.INFO:
+            levelname = f"{colors.green(record.levelname)}:"
+        elif record.levelno <= logging.WARNING:
+            levelname = f"{colors.yellow(record.levelname)}:"
+        else:
+            levelname = f"{colors.red(record.levelname)}:"
+        return f"{levelname: <17}"
 
     def format(self, record):
         if isinstance(record.msg, bytes):
             record.msg = record.msg.decode("utf-8")
         message = super().format(record)
         return f"{self.get_level_message(record)} {message}"
```

### Comparing `daffi-2.0.0/daffi/utils/misc.py` & `daffi-2.2.0/daffi/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 A library of various helpers functions and classes
 """
-import re
 import types
 import inspect
 import asyncio
 from uuid import uuid4
 from random import choice
 from functools import partial
 from datetime import datetime
@@ -224,11 +223,12 @@
 
 
 def contains_explicit_return(fn: Callable[..., Any]) -> bool:
     """Return true if provided function has `return` statement based on source code (even in nested functions)"""
     # Get source code
     source = inspect.getsource(fn)
     if doc := fn.__doc__:
+        # Remove `docs` part from source code.
         code = source.split(doc)
         source = code[1]
     refined_source = [line.strip() for line in source.split("\n")]
     return any(exp.startswith("return") for exp in refined_source)
```

### Comparing `daffi-2.0.0/daffi/utils/timeparse.py` & `daffi-2.2.0/daffi/utils/timeparse.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/async-apps.md` & `daffi-2.2.0/docs/async-apps.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/execution-modifiers.md` & `daffi-2.2.0/docs/execution-modifiers.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/global-object.md` & `daffi-2.2.0/docs/global-object.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/index.md` & `daffi-2.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/node-and-controller.md` & `daffi-2.2.0/docs/node-and-controller.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/bg.jpg` & `daffi-2.2.0/docs/images/bg.jpg`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/controller-plus-node-arch.drawio` & `daffi-2.2.0/docs/images/controller-plus-node-arch.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/controller-plus-node-arch.png` & `daffi-2.2.0/docs/images/controller-plus-node-arch.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/gitter.png` & `daffi-2.2.0/docs/images/gitter.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/logo-white-sm.png` & `daffi-2.2.0/docs/images/logo-white-sm.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/logo-white.png` & `daffi-2.2.0/docs/images/logo-white.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/logo.png` & `daffi-2.2.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/many-controllers.drawio` & `daffi-2.2.0/docs/images/many-controllers.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/many-controllers.png` & `daffi-2.2.0/docs/images/many-controllers.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/pdf-file.png` & `daffi-2.2.0/docs/images/pdf-file.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/stand-alone-controller-arch.drawio` & `daffi-2.2.0/docs/images/stand-alone-controller-arch.drawio`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/images/stand-alone-controller-arch.png` & `daffi-2.2.0/docs/images/stand-alone-controller-arch.png`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/js/extra.js` & `daffi-2.2.0/docs/js/extra.js`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/stylesheets/extra.css` & `daffi-2.2.0/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/aliased-methods.md` & `daffi-2.2.0/docs/usage/aliased-methods.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/asynchronous-execution.md` & `daffi-2.2.0/docs/usage/asynchronous-execution.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/basic-example.md` & `daffi-2.2.0/docs/usage/basic-example.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/bidirectional-communication.md` & `daffi-2.2.0/docs/usage/bidirectional-communication.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/broadcasting.md` & `daffi-2.2.0/docs/usage/broadcasting.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/callback-additional-arguments.md` & `daffi-2.2.0/docs/usage/callback-additional-arguments.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/fetchers-with-body.md` & `daffi-2.2.0/docs/usage/fetchers-with-body.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/function-transfer.md` & `daffi-2.2.0/docs/usage/function-transfer.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/named-processes.md` & `daffi-2.2.0/docs/usage/named-processes.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/private-methods.md` & `daffi-2.2.0/docs/usage/private-methods.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/stream-callback-to-fetcher.md` & `daffi-2.2.0/docs/usage/stream-callback-to-fetcher.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/docs/usage/stream-fetcher-to-callback.md` & `daffi-2.2.0/docs/usage/stream-fetcher-to-callback.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/docker/colorizer/main.py` & `daffi-2.2.0/examples/docker/colorizer/main.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/docker/email_processor/main.py` & `daffi-2.2.0/examples/docker/email_processor/main.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/docker/web/app.py` & `daffi-2.2.0/examples/docker/web/app.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/docker/web/templates/base.html` & `daffi-2.2.0/examples/docker/web/templates/base.html`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/docker/web/templates/index.html` & `daffi-2.2.0/examples/docker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/classes_based/consumer.py` & `daffi-2.2.0/examples/opencv_stream/classes_based/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/classes_based/publisher1.py` & `daffi-2.2.0/examples/opencv_stream/classes_based/publisher1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/classes_based/publisher2.py` & `daffi-2.2.0/examples/opencv_stream/classes_based/publisher2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/classes_based/publisher3.py` & `daffi-2.2.0/examples/opencv_stream/classes_based/publisher3.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/decorators_based/consumer.py` & `daffi-2.2.0/examples/opencv_stream/decorators_based/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/decorators_based/publisher1.py` & `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/decorators_based/publisher2.py` & `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/opencv_stream/decorators_based/publisher3.py` & `daffi-2.2.0/examples/opencv_stream/decorators_based/publisher3.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/callbacks_from_class/consumer.py` & `daffi-2.2.0/examples/tcp/callbacks_from_class/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/callbacks_from_class/publisher.py` & `daffi-2.2.0/examples/tcp/callbacks_from_class/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/eta/consumer.py` & `daffi-2.2.0/examples/tcp/eta/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/eta/publisher.py` & `daffi-2.2.0/examples/tcp/eta/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/no_return/consumer.py` & `daffi-2.2.0/examples/tcp/no_return/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/no_return/publisher.py` & `daffi-2.2.0/examples/tcp/no_return/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/scheduler/consumer.py` & `daffi-2.2.0/examples/tcp/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/scheduler/publisher.py` & `daffi-2.2.0/examples/tcp/scheduler/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/stream/consumer.py` & `daffi-2.2.0/examples/tcp/stream/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/stream/publisher.py` & `daffi-2.2.0/examples/tcp/stream/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/transfer_and_call/consumer.py` & `daffi-2.2.0/examples/tcp/transfer_and_call/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication/class_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication/class_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_asyncio/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py` & `daffi-2.2.0/examples/tcp/two_processes_base_communication_trio/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py` & `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py` & `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_decorator/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py` & `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py` & `daffi-2.2.0/examples/unix_socket/callback_and_fetcher_in_one_class/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_generator/class_consumer.py` & `daffi-2.2.0/examples/unix_socket/callback_generator/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callback_generator/class_publisher.py` & `daffi-2.2.0/examples/unix_socket/callback_generator/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callbacks_from_class/consumer.py` & `daffi-2.2.0/examples/unix_socket/callbacks_from_class/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/callbacks_from_class/publisher.py` & `daffi-2.2.0/examples/unix_socket/callbacks_from_class/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/eta/class_consumer.py` & `daffi-2.2.0/examples/unix_socket/eta/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/eta/class_publisher.py` & `daffi-2.2.0/examples/unix_socket/eta/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/eta/consumer.py` & `daffi-2.2.0/examples/unix_socket/eta/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/eta/publisher.py` & `daffi-2.2.0/examples/unix_socket/eta/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/fetcher_generator/class_consumer.py` & `daffi-2.2.0/examples/unix_socket/fetcher_generator/class_consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/fetcher_generator/class_publisher.py` & `daffi-2.2.0/examples/unix_socket/fetcher_generator/class_publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/no_return/consumer.py` & `daffi-2.2.0/examples/unix_socket/no_return/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/no_return/publisher.py` & `daffi-2.2.0/examples/unix_socket/no_return/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/scheduler/consumer.py` & `daffi-2.2.0/examples/unix_socket/scheduler/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/scheduler/publisher.py` & `daffi-2.2.0/examples/unix_socket/scheduler/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/stream/consumer.py` & `daffi-2.2.0/examples/unix_socket/stream/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/stream/publisher.py` & `daffi-2.2.0/examples/unix_socket/stream/publisher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/transfer_and_call/consumer.py` & `daffi-2.2.0/examples/unix_socket/transfer_and_call/consumer.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_asyncio/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/class_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc1.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py` & `daffi-2.2.0/examples/unix_socket/two_processes_base_communication_trio/decorators_based/proc2.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/scripts/generate_coverage_summary.py` & `daffi-2.2.0/scripts/generate_coverage_summary.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/scripts/write_coverage_summary_report.py` & `daffi-2.2.0/scripts/write_coverage_summary_report.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/conftest.py` & `daffi-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/conftest.py` & `daffi-2.2.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_broadcast.py` & `daffi-2.2.0/tests/integration/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_many_callbacks.py` & `daffi-2.2.0/tests/integration/test_many_callbacks.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_many_nodes.py` & `daffi-2.2.0/tests/integration/test_many_nodes.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_period.py` & `daffi-2.2.0/tests/integration/test_period.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_pipeline.py` & `daffi-2.2.0/tests/integration/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_stream_callback_to_fetcher.py` & `daffi-2.2.0/tests/integration/test_stream_callback_to_fetcher.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_stream_fetcher_to_callback.py` & `daffi-2.2.0/tests/integration/test_stream_fetcher_to_callback.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/test_trio.py` & `daffi-2.2.0/tests/integration/test_trio.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/templates/test_trio.jinja2` & `daffi-2.2.0/tests/integration/templates/test_trio.jinja2`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/integration/templates/layout/base.jinja2` & `daffi-2.2.0/tests/integration/templates/layout/base.jinja2`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_async_result.py` & `daffi-2.2.0/tests/unit/test_async_result.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_callback_and_fecher_classes.py` & `daffi-2.2.0/tests/unit/test_callback_and_fecher_classes.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_callback_decorator.py` & `daffi-2.2.0/tests/unit/test_callback_decorator.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_fetcher_decorator.py` & `daffi-2.2.0/tests/unit/test_fetcher_decorator.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_freezable_queue.py` & `daffi-2.2.0/tests/unit/test_freezable_queue.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_logger.py` & `daffi-2.2.0/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/tests/unit/test_misc.py` & `daffi-2.2.0/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/.gitignore` & `daffi-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/LICENSE.txt` & `daffi-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/README.md` & `daffi-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `daffi-2.0.0/pyproject.toml` & `daffi-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "daffi"
 description = "Daffi is fast, simple and lightweight library for inter process communication"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = "MIT"
 keywords = ["rpc", "task", "queue", "job", "async", "python", "distributed", "stream", "grpc"]
 authors = [
   { name = "Volodymyr Boiko", email = "600apples@gmail.com" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `daffi-2.0.0/PKG-INFO` & `daffi-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffi
-Version: 2.0.0
+Version: 2.2.0
 Summary: Daffi is fast, simple and lightweight library for inter process communication
 Project-URL: Documentation, https://600apples.github.io/dafi/
 Project-URL: Source, https://github.com/600apples/dafi
 Author-email: Volodymyr Boiko <600apples@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: async,distributed,grpc,job,python,queue,rpc,stream,task
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development :: Object Brokering
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Clustering
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: anyio>=3.6.2
 Requires-Dist: cached-property>=1.5.2
 Requires-Dist: cachetools>=5.3.0
 Requires-Dist: colorama>=0.4.6; sys_platform == 'win32'
 Requires-Dist: dill>=0.3.6
 Requires-Dist: grpcio>=1.51.3
 Requires-Dist: protobuf>=4.21.12
```

