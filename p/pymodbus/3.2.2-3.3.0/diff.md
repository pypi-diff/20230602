# Comparing `tmp/pymodbus-3.2.2.tar.gz` & `tmp/pymodbus-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodbus-3.2.2.tar", last modified: Tue Mar 21 09:21:00 2023, max compression
+gzip compressed data, was "pymodbus-3.3.0.tar", last modified: Fri Jun  2 13:19:46 2023, max compression
```

## Comparing `pymodbus-3.2.2.tar` & `pymodbus-3.3.0.tar`

### file list

```diff
@@ -1,120 +1,139 @@
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.497840 pymodbus-3.2.2/
--rw-r--r--   0 jan        (501) staff       (20)    23872 2023-03-21 08:34:16.000000 pymodbus-3.2.2/CHANGELOG.rst
--rw-r--r--   0 jan        (501) staff       (20)     1392 2023-03-21 09:20:42.000000 pymodbus-3.2.2/LICENSE
--rw-r--r--   0 jan        (501) staff       (20)       82 2023-03-21 09:20:42.000000 pymodbus-3.2.2/MANIFEST.in
--rw-r--r--   0 jan        (501) staff       (20)    18264 2023-03-21 09:21:00.497937 pymodbus-3.2.2/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)    16770 2023-03-21 09:20:42.000000 pymodbus-3.2.2/README.rst
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.489305 pymodbus-3.2.2/pymodbus/
--rw-r--r--   0 jan        (501) staff       (20)      337 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     9369 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/bit_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)     9267 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/bit_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.491104 pymodbus-3.2.2/pymodbus/client/
--rw-r--r--   0 jan        (501) staff       (20)      602 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    14117 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/base.py
--rw-r--r--   0 jan        (501) staff       (20)    20803 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/mixin.py
--rw-r--r--   0 jan        (501) staff       (20)    12788 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/serial.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.491229 pymodbus-3.2.2/pymodbus/client/serial_asyncio/
--rw-r--r--   0 jan        (501) staff       (20)    19422 2023-02-06 09:15:57.000000 pymodbus-3.2.2/pymodbus/client/serial_asyncio/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     6677 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/sync_diag.py
--rw-r--r--   0 jan        (501) staff       (20)    12579 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/tcp.py
--rw-r--r--   0 jan        (501) staff       (20)     7007 2023-03-20 15:38:56.000000 pymodbus-3.2.2/pymodbus/client/tls.py
--rw-r--r--   0 jan        (501) staff       (20)     8348 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/client/udp.py
--rw-r--r--   0 jan        (501) staff       (20)     8686 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/constants.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.491780 pymodbus-3.2.2/pymodbus/datastore/
--rw-r--r--   0 jan        (501) staff       (20)      491 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/datastore/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7339 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/datastore/context.py
--rw-r--r--   0 jan        (501) staff       (20)     4851 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/datastore/remote.py
--rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/datastore/simulator.py
--rw-r--r--   0 jan        (501) staff       (20)    11410 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/datastore/store.py
--rw-r--r--   0 jan        (501) staff       (20)    22668 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/device.py
--rw-r--r--   0 jan        (501) staff       (20)    30046 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/diag_message.py
--rw-r--r--   0 jan        (501) staff       (20)     6461 2023-02-06 09:07:10.000000 pymodbus-3.2.2/pymodbus/events.py
--rw-r--r--   0 jan        (501) staff       (20)     3206 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)    13690 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/factory.py
--rw-r--r--   0 jan        (501) staff       (20)    14722 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/file_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.492398 pymodbus-3.2.2/pymodbus/framer/
--rw-r--r--   0 jan        (501) staff       (20)     1618 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7560 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/ascii_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     8107 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/binary_framer.py
--rw-r--r--   0 jan        (501) staff       (20)    12645 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/rtu_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     8077 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/socket_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     6133 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/framer/tls_framer.py
--rw-r--r--   0 jan        (501) staff       (20)     3910 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/logging.py
--rw-r--r--   0 jan        (501) staff       (20)     7747 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/mei_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15468 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/other_message.py
--rw-r--r--   0 jan        (501) staff       (20)    15870 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/payload.py
--rw-r--r--   0 jan        (501) staff       (20)     7735 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/pdu.py
--rw-r--r--   0 jan        (501) staff       (20)        0 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/py.typed
--rw-r--r--   0 jan        (501) staff       (20)    14021 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/register_read_message.py
--rw-r--r--   0 jan        (501) staff       (20)    12160 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/register_write_message.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.492501 pymodbus-3.2.2/pymodbus/repl/
--rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.2.2/pymodbus/repl/__init__.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.493043 pymodbus-3.2.2/pymodbus/repl/client/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.2.2/pymodbus/repl/client/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     5187 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/repl/client/completer.py
--rw-r--r--   0 jan        (501) staff       (20)     9526 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/repl/client/helper.py
--rw-r--r--   0 jan        (501) staff       (20)    13101 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/repl/client/main.py
--rw-r--r--   0 jan        (501) staff       (20)    22965 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/repl/client/mclient.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.493418 pymodbus-3.2.2/pymodbus/repl/server/
--rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.2.2/pymodbus/repl/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     7436 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/repl/server/cli.py
--rw-r--r--   0 jan        (501) staff       (20)     6485 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/repl/server/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.493608 pymodbus-3.2.2/pymodbus/server/
--rw-r--r--   0 jan        (501) staff       (20)      975 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/server/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)    47535 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/server/async_io.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.493930 pymodbus-3.2.2/pymodbus/server/reactive/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.2.2/pymodbus/server/reactive/__init__.py
--rw-r--r--   0 jan        (501) staff       (20)     1977 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/server/reactive/default_config.py
--rw-r--r--   0 jan        (501) staff       (20)    18783 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/server/reactive/main.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.494430 pymodbus-3.2.2/pymodbus/server/simulator/
--rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.2.2/pymodbus/server/simulator/__init__.py
--rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.2.2/pymodbus/server/simulator/custom_actions.py
--rw-r--r--   0 jan        (501) staff       (20)    25067 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/server/simulator/http_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4067 2023-03-18 19:26:06.000000 pymodbus-3.2.2/pymodbus/server/simulator/main.py
--rw-r--r--   0 jan        (501) staff       (20)    23788 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/transaction.py
--rw-r--r--   0 jan        (501) staff       (20)     7986 2023-03-21 09:20:42.000000 pymodbus-3.2.2/pymodbus/utilities.py
--rw-r--r--   0 jan        (501) staff       (20)     1149 2023-03-21 08:34:16.000000 pymodbus-3.2.2/pymodbus/version.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.490110 pymodbus-3.2.2/pymodbus.egg-info/
--rw-r--r--   0 jan        (501) staff       (20)    18264 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/PKG-INFO
--rw-r--r--   0 jan        (501) staff       (20)     2793 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/SOURCES.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/dependency_links.txt
--rw-r--r--   0 jan        (501) staff       (20)      173 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/entry_points.txt
--rw-r--r--   0 jan        (501) staff       (20)      588 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/requires.txt
--rw-r--r--   0 jan        (501) staff       (20)        9 2023-03-21 09:21:00.000000 pymodbus-3.2.2/pymodbus.egg-info/top_level.txt
--rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.2.2/pymodbus.egg-info/zip-safe
--rw-r--r--   0 jan        (501) staff       (20)     2004 2023-03-21 09:20:42.000000 pymodbus-3.2.2/requirements.txt
--rw-r--r--   0 jan        (501) staff       (20)     7954 2023-03-21 09:21:00.499010 pymodbus-3.2.2/setup.cfg
--rw-r--r--   0 jan        (501) staff       (20)     1026 2023-03-19 11:03:53.000000 pymodbus-3.2.2/setup.py
-drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-03-21 09:21:00.497740 pymodbus-3.2.2/test/
--rw-r--r--   0 jan        (501) staff       (20)     3738 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_all_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     4594 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_bit_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5244 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_bit_write_messages.py
--rwxr-xr-x   0 jan        (501) staff       (20)    21201 2023-03-18 19:26:06.000000 pymodbus-3.2.2/test/test_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    16177 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_client_sync.py
--rwxr-xr-x   0 jan        (501) staff       (20)     4195 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_client_sync_diag.py
--rw-r--r--   0 jan        (501) staff       (20)    13200 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_device.py
--rw-r--r--   0 jan        (501) staff       (20)     7890 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_diag_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2359 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_events.py
--rwxr-xr-x   0 jan        (501) staff       (20)     3485 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_example_client_server.py
--rwxr-xr-x   0 jan        (501) staff       (20)     7225 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_examples.py
--rw-r--r--   0 jan        (501) staff       (20)      888 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_exceptions.py
--rw-r--r--   0 jan        (501) staff       (20)     8496 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_factory.py
--rw-r--r--   0 jan        (501) staff       (20)    10180 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_file_message.py
--rw-r--r--   0 jan        (501) staff       (20)    11670 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_framers.py
--rw-r--r--   0 jan        (501) staff       (20)     1232 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_logging.py
--rw-r--r--   0 jan        (501) staff       (20)     6297 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_mei_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     5687 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_other_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     8790 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_payload.py
--rw-r--r--   0 jan        (501) staff       (20)     2814 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_pdu.py
--rw-r--r--   0 jan        (501) staff       (20)     7450 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_register_read_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     7658 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_register_write_messages.py
--rw-r--r--   0 jan        (501) staff       (20)     2448 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_remote_datastore.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1472 2023-03-18 19:26:06.000000 pymodbus-3.2.2/test/test_repl_client.py
--rwxr-xr-x   0 jan        (501) staff       (20)    17547 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_server_asyncio.py
--rw-r--r--   0 jan        (501) staff       (20)     3546 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_server_context.py
--rwxr-xr-x   0 jan        (501) staff       (20)    10279 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_server_task.py
--rw-r--r--   0 jan        (501) staff       (20)    18293 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_simulator.py
--rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_transaction.py
--rwxr-xr-x   0 jan        (501) staff       (20)     1958 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_unix_socket.py
--rw-r--r--   0 jan        (501) staff       (20)     3107 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_utilities.py
--rw-r--r--   0 jan        (501) staff       (20)      743 2023-03-21 09:20:42.000000 pymodbus-3.2.2/test/test_version.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.515583 pymodbus-3.3.0/
+-rw-r--r--   0 jan        (501) staff       (20)    26147 2023-06-02 12:16:59.000000 pymodbus-3.3.0/CHANGELOG.rst
+-rw-r--r--   0 jan        (501) staff       (20)     1392 2023-06-02 12:16:19.000000 pymodbus-3.3.0/LICENSE
+-rw-r--r--   0 jan        (501) staff       (20)       82 2023-06-02 12:16:19.000000 pymodbus-3.3.0/MANIFEST.in
+-rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-02 13:19:46.515666 pymodbus-3.3.0/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)    16791 2023-06-02 12:17:24.000000 pymodbus-3.3.0/README.rst
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.504496 pymodbus-3.3.0/pymodbus/
+-rw-r--r--   0 jan        (501) staff       (20)      316 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     9369 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/bit_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     9267 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/bit_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.506046 pymodbus-3.3.0/pymodbus/client/
+-rw-r--r--   0 jan        (501) staff       (20)      602 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    11857 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/base.py
+-rw-r--r--   0 jan        (501) staff       (20)    20812 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/mixin.py
+-rw-r--r--   0 jan        (501) staff       (20)     9904 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/serial.py
+-rw-r--r--   0 jan        (501) staff       (20)     9645 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/tcp.py
+-rw-r--r--   0 jan        (501) staff       (20)     6879 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/tls.py
+-rw-r--r--   0 jan        (501) staff       (20)     5367 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/client/udp.py
+-rw-r--r--   0 jan        (501) staff       (20)     8654 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/constants.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.506581 pymodbus-3.3.0/pymodbus/datastore/
+-rw-r--r--   0 jan        (501) staff       (20)      491 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7312 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/context.py
+-rw-r--r--   0 jan        (501) staff       (20)     4851 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/remote.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    29689 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/datastore/simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)    11410 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/datastore/store.py
+-rw-r--r--   0 jan        (501) staff       (20)    22669 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/device.py
+-rw-r--r--   0 jan        (501) staff       (20)    30049 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/diag_message.py
+-rw-r--r--   0 jan        (501) staff       (20)     6481 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/events.py
+-rw-r--r--   0 jan        (501) staff       (20)     3206 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)    13673 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    14722 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/file_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507251 pymodbus-3.3.0/pymodbus/framer/
+-rw-r--r--   0 jan        (501) staff       (20)      509 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     7335 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/ascii_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     1822 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/base.py
+-rw-r--r--   0 jan        (501) staff       (20)     8043 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/binary_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)    13507 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/rtu_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     7903 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/socket_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     6100 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/framer/tls_framer.py
+-rw-r--r--   0 jan        (501) staff       (20)     3910 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     7745 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/mei_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15358 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/other_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    15651 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     7786 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)        0 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/py.typed
+-rw-r--r--   0 jan        (501) staff       (20)    14021 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/register_read_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    12160 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/register_write_message.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507358 pymodbus-3.3.0/pymodbus/repl/
+-rw-r--r--   0 jan        (501) staff       (20)       28 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.507846 pymodbus-3.3.0/pymodbus/repl/client/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/client/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     5187 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/repl/client/completer.py
+-rw-r--r--   0 jan        (501) staff       (20)     9526 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/helper.py
+-rw-r--r--   0 jan        (501) staff       (20)    13305 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/main.py
+-rw-r--r--   0 jan        (501) staff       (20)    23176 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/client/mclient.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508160 pymodbus-3.3.0/pymodbus/repl/server/
+-rw-r--r--   0 jan        (501) staff       (20)       19 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/repl/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     6912 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/server/cli.py
+-rw-r--r--   0 jan        (501) staff       (20)     6421 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/repl/server/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508390 pymodbus-3.3.0/pymodbus/server/
+-rw-r--r--   0 jan        (501) staff       (20)      975 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    47435 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/async_io.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.508739 pymodbus-3.3.0/pymodbus/server/reactive/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:07:10.000000 pymodbus-3.3.0/pymodbus/server/reactive/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)     1977 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/reactive/default_config.py
+-rw-r--r--   0 jan        (501) staff       (20)    18735 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/reactive/main.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.509297 pymodbus-3.3.0/pymodbus/server/simulator/
+-rw-r--r--   0 jan        (501) staff       (20)       18 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/__init__.py
+-rwxr-xr-x   0 jan        (501) staff       (20)      186 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/custom_actions.py
+-rw-r--r--   0 jan        (501) staff       (20)    25063 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/simulator/http_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     4068 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/server/simulator/main.py
+-rw-r--r--   0 jan        (501) staff       (20)     6788 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/setup.json
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.510828 pymodbus-3.3.0/pymodbus/server/simulator/web/
+-rw-r--r--   0 jan        (501) staff       (20)    11369 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple120.png
+-rw-r--r--   0 jan        (501) staff       (20)    15391 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple152.png
+-rw-r--r--   0 jan        (501) staff       (20)     4817 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple60.png
+-rw-r--r--   0 jan        (501) staff       (20)     6344 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/apple76.png
+-rw-r--r--   0 jan        (501) staff       (20)    12014 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/favicon.ico
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511585 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/
+-rw-r--r--   0 jan        (501) staff       (20)     4314 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/calls
+-rw-r--r--   0 jan        (501) staff       (20)     1132 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/log
+-rw-r--r--   0 jan        (501) staff       (20)     5850 2023-02-06 09:15:57.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+-rw-r--r--   0 jan        (501) staff       (20)     2710 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/registers
+-rw-r--r--   0 jan        (501) staff       (20)      893 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/generator/server
+-rw-r--r--   0 jan        (501) staff       (20)     1944 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/index.html
+-rw-r--r--   0 jan        (501) staff       (20)      919 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/pymodbus.css
+-rw-r--r--   0 jan        (501) staff       (20)      710 2023-06-01 14:23:34.000000 pymodbus-3.3.0/pymodbus/server/simulator/web/welcome.html
+-rw-r--r--   0 jan        (501) staff       (20)    23769 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transaction.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511809 pymodbus-3.3.0/pymodbus/transport/
+-rw-r--r--   0 jan        (501) staff       (20)      109 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/__init__.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.511902 pymodbus-3.3.0/pymodbus/transport/serial_asyncio/
+-rw-r--r--   0 jan        (501) staff       (20)    19336 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/serial_asyncio/__init__.py
+-rw-r--r--   0 jan        (501) staff       (20)    14300 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/transport/transport.py
+-rw-r--r--   0 jan        (501) staff       (20)     7797 2023-06-02 12:16:19.000000 pymodbus-3.3.0/pymodbus/utilities.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.505208 pymodbus-3.3.0/pymodbus.egg-info/
+-rw-r--r--   0 jan        (501) staff       (20)    18285 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/PKG-INFO
+-rw-r--r--   0 jan        (501) staff       (20)     3509 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/SOURCES.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/dependency_links.txt
+-rw-r--r--   0 jan        (501) staff       (20)      173 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/entry_points.txt
+-rw-r--r--   0 jan        (501) staff       (20)      481 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/requires.txt
+-rw-r--r--   0 jan        (501) staff       (20)        9 2023-06-02 13:19:46.000000 pymodbus-3.3.0/pymodbus.egg-info/top_level.txt
+-rw-r--r--   0 jan        (501) staff       (20)        1 2022-11-08 12:27:57.000000 pymodbus-3.3.0/pymodbus.egg-info/zip-safe
+-rw-r--r--   0 jan        (501) staff       (20)     1897 2023-06-02 12:16:19.000000 pymodbus-3.3.0/requirements.txt
+-rw-r--r--   0 jan        (501) staff       (20)     4391 2023-06-02 13:19:46.516276 pymodbus-3.3.0/setup.cfg
+-rw-r--r--   0 jan        (501) staff       (20)     1105 2023-06-02 12:17:58.000000 pymodbus-3.3.0/setup.py
+drwxr-xr-x   0 jan        (501) staff       (20)        0 2023-06-02 13:19:46.515489 pymodbus-3.3.0/test/
+-rw-r--r--   0 jan        (501) staff       (20)     3738 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_all_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     4594 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_bit_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5244 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_bit_write_messages.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    19470 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client.py
+-rw-r--r--   0 jan        (501) staff       (20)     1315 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client_faulty_response.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    16833 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_client_sync.py
+-rw-r--r--   0 jan        (501) staff       (20)    13200 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_device.py
+-rw-r--r--   0 jan        (501) staff       (20)     8330 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_diag_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2359 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_events.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     3503 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_example_client_server.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     7225 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_examples.py
+-rw-r--r--   0 jan        (501) staff       (20)      771 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_exceptions.py
+-rw-r--r--   0 jan        (501) staff       (20)     8499 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_factory.py
+-rw-r--r--   0 jan        (501) staff       (20)    10180 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_file_message.py
+-rw-r--r--   0 jan        (501) staff       (20)    10928 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_framers.py
+-rw-r--r--   0 jan        (501) staff       (20)     1238 2023-06-02 12:18:32.000000 pymodbus-3.3.0/test/test_logging.py
+-rw-r--r--   0 jan        (501) staff       (20)     6297 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_mei_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     5687 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_other_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     8771 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_payload.py
+-rw-r--r--   0 jan        (501) staff       (20)     2814 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_pdu.py
+-rw-r--r--   0 jan        (501) staff       (20)     7450 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_register_read_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     7658 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_register_write_messages.py
+-rw-r--r--   0 jan        (501) staff       (20)     2448 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_remote_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1463 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_repl_client.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    17385 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_asyncio.py
+-rw-r--r--   0 jan        (501) staff       (20)     3546 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_context.py
+-rw-r--r--   0 jan        (501) staff       (20)     8192 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_multidrop.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    10893 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_server_task.py
+-rw-r--r--   0 jan        (501) staff       (20)    18298 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_simulator.py
+-rw-r--r--   0 jan        (501) staff       (20)      649 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_sparse_datastore.py
+-rwxr-xr-x   0 jan        (501) staff       (20)    30391 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_transaction.py
+-rwxr-xr-x   0 jan        (501) staff       (20)     1974 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_unix_socket.py
+-rw-r--r--   0 jan        (501) staff       (20)     3107 2023-06-02 12:16:19.000000 pymodbus-3.3.0/test/test_utilities.py
```

### Comparing `pymodbus-3.2.2/CHANGELOG.rst` & `pymodbus-3.3.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,68 @@
+version 3.3.0
+----------------------------------------------------------
+* Stabilize windows tests. (#1567)
+* Bump mypy 1.3.0 (#1568)
+* Transport integrated in async clients. (#1541)
+* Client async corrections (due to 3.1.2) (#1565)
+* Server_async[udp], solve 3.1.1 problem. (#1564)
+* Remove ModbusTcpDiagClient. (#1560)
+* Remove old method from Python2/3 transition (#1559)
+* Switch to ruff's version of bandit (#1557)
+* Allow reading/writing address 0 in the simulator (#1552)
+* Remove references to "defer_start". (#1548)
+* Client more robust against faulty response. (#1547)
+* Fix missing package_data directives for simulator web (#1544)
+* Fix installation instructions (#1543)
+* Solve pytest timeout problem. (#1540)
+* DiagnosticStatus encode missing tuple check. (#1533)
+* test SparseDataStore. (#1532)
+* BinaryPayloadBuilder.to_string to BinaryPayloadBuilder.encode (#1526)
+* Adding flake8-pytest-style` to ruff (#1520)
+* Simplify version management. (#1522)
+* pylint and pre-commit autoupdate (#1519)
+* Add type hint (#1512)
+* Add action to lock issues/PR. (#1508)
+* New common transport layer. (#1492)
+* Solve serial close raise problem.
+* Remove old config values (#1503)
+* Document pymodbus.simulator. (#1502)
+* Refactor REPL server to reduce complexity (#1499)
+* Don't catch KeyboardInterrupt twice for REPL server (#1498)
+* Refactor REPL client to reduce complexity (#1489)
+* pymodbus.server: listen on ID 1 by default (#1496)
+* Clean framer/__init__.py (#1494)
+* Duplicate transactions in UDP. (#1486)
+* clean ProcessIncommingPacket. (#1491)
+* Enable pyupgrade (U) rules in ruff (#1484)
+* clean_workflow.yaml solve parameter problem.
+* Correct wrong import in test. (#1483)
+* Implement pyflakes-simplify (#1480)
+* Test case for UDP duplicate msg issue (#1470)
+* Test of write_coil. (#1479)
+* Test reuse of client object. (#1475)
+* Comment about addressing when shared=false (#1474)
+* Remove old aliases to OSError (#1473)
+* pymodbus.simulator fixes (#1463)
+* Fix wrong error message with pymodbus console (#1456)
+* update modbusrtuframer (#1435)
+* Server multidrop test.: (#1451)
+* mypy problem ModbusResponse.
+
+Thanks to:
+  Alex
+  Christian Krause
+  corollaries
+  dhoomakethu
+  Ghostkeeper
+  jan iversen
+  James Braza
+  Kenny Johansson
+  Pavel Kostromitinov
+
 version 3.2.2 (picked from dev, only bugfixes)
 ----------------------------------------------------------
 * Add forgotten await
 
 version 3.2.1 (picked from dev, only bugfixes)
 ----------------------------------------------------------
 * add missing server.start(). (#1443)
```

### Comparing `pymodbus-3.2.2/LICENSE` & `pymodbus-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/PKG-INFO` & `pymodbus-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.2.2
+Version: 3.3.0
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -55,17 +55,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python 2.7.x - 3.7).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.2.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.2.2>`_ is the current release (Supports Python >=3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
@@ -280,15 +280,15 @@
 and maintenance development is merged here.
 
 -----------------------------------------------------------
 Install with Docker
 -----------------------------------------------------------
 Pull the latest image on ``dev`` branch with ``docker pull ghcr.io/pymodbus-dev/pymodbus:dev``::
 
-   doker pull ghcr.io/pymodbus-dev/pymodbus:dev
+   ❯ docker pull ghcr.io/pymodbus-dev/pymodbus:dev
    dev: Pulling from pymodbus-dev/pymodbus
    548fcab5fe88: Pull complete
    a4d3f9f008ef: Pull complete
    eb83acb05730: Pull complete
    71cd28d529fd: Pull complete
    66607ad8f4f0: Pull complete
    64dff4c66d3b: Pull complete
@@ -402,16 +402,15 @@
    make html
 
 ------------------------------------------------------------
 Contributing
 ------------------------------------------------------------
 Just fork the repo and raise your PR against `dev` branch.
 
-Here are some of the items waiting to be done:
-   https://github.com/pymodbus-dev/pymodbus/blob/dev/doc/TODO
+We always have more work than time, so feel free to open a discussion / issue on a theme you want to solve.
 
 ------------------------------------------------------------
 License Information
 ------------------------------------------------------------
 
 Pymodbus is built on top of code developed from/by:
   * Copyright (c) 2001-2005 S.W.A.C. GmbH, Germany.
```

### Comparing `pymodbus-3.2.2/README.rst` & `pymodbus-3.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python 2.7.x - 3.7).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.2.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.2.2>`_ is the current release (Supports Python >=3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
@@ -241,15 +241,15 @@
 and maintenance development is merged here.
 
 -----------------------------------------------------------
 Install with Docker
 -----------------------------------------------------------
 Pull the latest image on ``dev`` branch with ``docker pull ghcr.io/pymodbus-dev/pymodbus:dev``::
 
-   doker pull ghcr.io/pymodbus-dev/pymodbus:dev
+   ❯ docker pull ghcr.io/pymodbus-dev/pymodbus:dev
    dev: Pulling from pymodbus-dev/pymodbus
    548fcab5fe88: Pull complete
    a4d3f9f008ef: Pull complete
    eb83acb05730: Pull complete
    71cd28d529fd: Pull complete
    66607ad8f4f0: Pull complete
    64dff4c66d3b: Pull complete
@@ -363,16 +363,15 @@
    make html
 
 ------------------------------------------------------------
 Contributing
 ------------------------------------------------------------
 Just fork the repo and raise your PR against `dev` branch.
 
-Here are some of the items waiting to be done:
-   https://github.com/pymodbus-dev/pymodbus/blob/dev/doc/TODO
+We always have more work than time, so feel free to open a discussion / issue on a theme you want to solve.
 
 ------------------------------------------------------------
 License Information
 ------------------------------------------------------------
 
 Pymodbus is built on top of code developed from/by:
   * Copyright (c) 2001-2005 S.W.A.C. GmbH, Germany.
```

### Comparing `pymodbus-3.2.2/pymodbus/bit_read_message.py` & `pymodbus-3.3.0/pymodbus/bit_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/bit_write_message.py` & `pymodbus-3.3.0/pymodbus/bit_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/client/__init__.py` & `pymodbus-3.3.0/pymodbus/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/client/base.py` & `pymodbus-3.3.0/pymodbus/client/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Base for all clients."""
 from __future__ import annotations
 
 import asyncio
 import socket
 from dataclasses import dataclass
-from typing import Any, Callable, Optional, Tuple, Type
+from typing import Any, Callable
 
 from pymodbus.client.mixin import ModbusClientMixin
 from pymodbus.constants import Defaults
-from pymodbus.exceptions import ConnectionException, NotImplementedException
+from pymodbus.exceptions import ConnectionException
 from pymodbus.factory import ClientDecoder
 from pymodbus.framer import ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.transaction import DictTransactionManager
+from pymodbus.transport import BaseTransport
 from pymodbus.utilities import ModbusTransactionState
 
 
-class ModbusBaseClient(ModbusClientMixin):
+class ModbusBaseClient(ModbusClientMixin, BaseTransport):
     """**ModbusBaseClient**
 
     **Parameters common to all clients**:
 
     :param framer: (optional) Modbus Framer class.
     :param timeout: (optional) Timeout for a request, in seconds.
     :param retries: (optional) Max number of retries per request.
@@ -35,115 +36,112 @@
     :param kwargs: (optional) Experimental parameters.
 
     .. tip::
         Common parameters and all external methods for all clients are documented here,
         and not repeated with each client.
 
     .. tip::
-        **delay_ms** doubles automatically with each unsuccessful connect, from
+        **reconnect_delay** doubles automatically with each unsuccessful connect, from
         **reconnect_delay** to **reconnect_delay_max**.
         Set `reconnect_delay=0` to avoid automatic reconnection.
 
-    :mod:`ModbusBaseClient` is normally not referenced outside :mod:`pymodbus`,
-    unless you want to make a custom client.
-
-    Custom client class **must** inherit :mod:`ModbusBaseClient`, example::
-
-        from pymodbus.client import ModbusBaseClient
-
-        class myOwnClient(ModbusBaseClient):
-
-            def __init__(self, **kwargs):
-                super().__init__(kwargs)
-
-        def run():
-            client = myOwnClient(...)
-            client.connect()
-            rr = client.read_coils(0x01)
-            client.close()
+    :mod:`ModbusBaseClient` is normally not referenced outside :mod:`pymodbus`.
 
     **Application methods, common to all clients**:
     """
 
     @dataclass
     class _params:  # pylint: disable=too-many-instance-attributes
         """Parameter class."""
 
         host: str = None
         port: str | int = None
-        framer: Type[ModbusFramer] = None
+        framer: type[ModbusFramer] = None
         timeout: float = None
         retries: int = None
         retry_on_empty: bool = None
         close_comm_on_error: bool = None
         strict: bool = None
         broadcast_enable: bool = None
         kwargs: dict = None
         reconnect_delay: int = None
-        reconnect_delay_max: int = None
-        on_reconnect_callback: Optional[Callable[[], None]] = None
 
         baudrate: int = None
         bytesize: int = None
         parity: str = None
         stopbits: int = None
         handle_local_echo: bool = None
 
-        source_address: Tuple[str, int] = None
+        source_address: tuple[str, int] = None
 
         sslctx: str = None
         certfile: str = None
         keyfile: str = None
         password: str = None
         server_hostname: str = None
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        framer: Type[ModbusFramer] = None,
+        framer: type[ModbusFramer] = None,
         timeout: str | float = Defaults.Timeout,
         retries: str | int = Defaults.Retries,
         retry_on_empty: bool = Defaults.RetryOnEmpty,
         close_comm_on_error: bool = Defaults.CloseCommOnError,
         strict: bool = Defaults.Strict,
         broadcast_enable: bool = Defaults.BroadcastEnable,
-        reconnect_delay: int = Defaults.ReconnectDelay,
-        reconnect_delay_max: int = Defaults.ReconnectDelayMax,
-        on_reconnect_callback: Optional[Callable[[], None]] = None,
+        reconnect_delay: int = 0.1,
+        reconnect_delay_max: int = 300,
+        on_reconnect_callback: Callable[[], None] | None = None,
         **kwargs: Any,
     ) -> None:
         """Initialize a client instance."""
+        BaseTransport.__init__(
+            self,
+            "comm",
+            (reconnect_delay * 1000, reconnect_delay_max * 1000),
+            timeout * 1000,
+            framer,
+            lambda: None,
+            self.cb_base_connection_lost,
+            self.cb_base_handle_data,
+        )
+        self.framer = framer
         self.params = self._params()
         self.params.framer = framer
         self.params.timeout = float(timeout)
         self.params.retries = int(retries)
         self.params.retry_on_empty = bool(retry_on_empty)
         self.params.close_comm_on_error = bool(close_comm_on_error)
         self.params.strict = bool(strict)
         self.params.broadcast_enable = bool(broadcast_enable)
         self.params.reconnect_delay = int(reconnect_delay)
-        self.params.reconnect_delay_max = int(reconnect_delay_max)
-        self.params.on_reconnect_callback = on_reconnect_callback
+        self.reconnect_delay_max = int(reconnect_delay_max)
+        self.on_reconnect_callback = on_reconnect_callback
         self.params.kwargs = kwargs
+        self.retry_on_empty: int = 0
+        # -> retry read on nothing
+
+        self.slaves: list[int] = []
+        # -> list of acceptable slaves (0 for accept all)
 
         # Common variables.
         self.framer = self.params.framer(ClientDecoder(), self)
         self.transaction = DictTransactionManager(
             self, retries=retries, retry_on_empty=retry_on_empty, **kwargs
         )
-        self.delay_ms = self.params.reconnect_delay
-        self.use_protocol = False
-        self._connected = False
+        self.reconnect_delay = self.params.reconnect_delay
+        self.reconnect_delay_current = self.params.reconnect_delay
+        self.use_sync = False
         self.use_udp = False
         self.state = ModbusTransactionState.IDLE
         self.last_frame_end: float = 0
         self.silent_interval: float = 0
-        self.transport = None
 
         # Initialize  mixin
-        super().__init__()
+        ModbusClientMixin.__init__(self)
 
     # ----------------------------------------------------------------------- #
     # Client external interface
     # ----------------------------------------------------------------------- #
     def register(self, custom_response_class: ModbusResponse) -> None:
         """Register a custom response class with the decoder (call **sync**).
 
@@ -151,73 +149,42 @@
         :raises MessageRegisterException: Check exception text.
 
         Use register() to add non-standard responses (like e.g. a login prompt) and
         have them interpreted automatically.
         """
         self.framer.decoder.register(custom_response_class)
 
-    def connect(self):
-        """Connect to the modbus remote host (call **sync/async**).
-
-        :raises ModbusException: Different exceptions, check exception text.
-
-        **Remark** Retries are handled automatically after first successful connect.
-        """
-        raise NotImplementedException
-
-    def is_socket_open(self) -> bool:
-        """Return whether socket/serial is open or not (call **sync**)."""
-        raise NotImplementedException
-
     def idle_time(self) -> float:
         """Time before initiating next transaction (call **sync**).
 
         Applications can call message functions without checking idle_time(),
         this is done automatically.
         """
         if self.last_frame_end is None or self.silent_interval is None:
             return 0
         return self.last_frame_end + self.silent_interval
 
-    def reset_delay(self) -> None:
-        """Reset wait time before next reconnect to minimal period (call **sync**)."""
-        self.delay_ms = self.params.reconnect_delay
-
     def execute(self, request: ModbusRequest = None) -> ModbusResponse:
         """Execute request and get response (call **sync/async**).
 
         :param request: The request to process
         :returns: The result of the request execution
         :raises ConnectionException: Check exception text.
         """
-        if self.use_protocol:
-            if not self._connected:
-                raise ConnectionException(f"Not connected[{str(self)}]")
-            return self.async_execute(request)
-        if not self.connect():
-            raise ConnectionException(f"Failed to connect[{str(self)}]")
-        return self.transaction.execute(request)
-
-    def close(self) -> None:
-        """Close the underlying socket connection (call **sync/async**)."""
-        raise NotImplementedException
+        if self.use_sync:
+            if not self.connect():
+                raise ConnectionException(f"Failed to connect[{str(self)}]")
+            return self.transaction.execute(request)
+        if not self.transport:
+            raise ConnectionException(f"Not connected[{str(self)}]")
+        return self.async_execute(request)
 
     # ----------------------------------------------------------------------- #
     # Merged client methods
     # ----------------------------------------------------------------------- #
-    def client_made_connection(self, protocol):
-        """Run transport specific connection."""
-
-    def client_lost_connection(self, protocol):
-        """Run transport specific connection lost."""
-
-    def datagram_received(self, data, _addr):
-        """Receive datagram."""
-        self.data_received(data)
-
     async def async_execute(self, request=None):
         """Execute requests asynchronously."""
         request.transaction_id = self.transaction.getNextTID()
         packet = self.framer.buildPacket(request)
         Log.debug("send: {}", packet, ":hex")
         if self.use_udp:
             self.transport.sendto(packet)
@@ -226,58 +193,37 @@
         req = self._build_response(request.transaction_id)
         if self.params.broadcast_enable and not request.slave_id:
             resp = b"Broadcast write sent - no response expected"
         else:
             try:
                 resp = await asyncio.wait_for(req, timeout=self.params.timeout)
             except asyncio.exceptions.TimeoutError:
-                self.connection_lost("trying to send")
+                self.close(reconnect=True)
                 raise
         return resp
 
-    def connection_made(self, transport):
-        """Call when a connection is made.
+    def cb_base_handle_data(self, data: bytes) -> int:
+        """Handle received data
 
-        The transport argument is the transport representing the connection.
+        returns number of bytes consumed
         """
-        self.transport = transport
-        Log.debug("Client connected to modbus server")
-        self._connected = True
-        self.client_made_connection(self)
-
-    def connection_lost(self, reason):
-        """Call when the connection is lost or closed.
+        Log.debug("recv: {}", data, ":hex")
+        self.framer.processIncomingPacket(data, self._handle_response, slave=0)
+        return len(data)
 
-        The argument is either an exception object or None
-        """
-        if self.transport:
-            self.transport.abort()
-            if hasattr(self.transport, "_sock"):
-                self.transport._sock.close()  # pylint: disable=protected-access
-            self.transport = None
-        self.client_lost_connection(self)
-        Log.debug("Client disconnected from modbus server: {}", reason)
-        self._connected = False
+    def cb_base_connection_lost(self, _reason: Exception) -> None:
+        """Handle lost connection"""
         for tid in list(self.transaction):
             self.raise_future(
                 self.transaction.getTransaction(tid),
                 ConnectionException("Connection lost during request"),
             )
 
-    def data_received(self, data):
-        """Call when some data is received.
-
-        data is a non-empty bytes object containing the incoming data.
-        """
-        Log.debug("recv: {}", data, ":hex")
-        self.framer.processIncomingPacket(data, self._handle_response, slave=0)
-
-    def create_future(self):
-        """Help function to create asyncio Future object."""
-        return asyncio.Future()
+    async def connect(self):
+        """Connect to the modbus remote host."""
 
     def raise_future(self, my_future, exc):
         """Set exception of a future if not done."""
         if not my_future.done():
             my_future.set_exception(exc)
 
     def _handle_response(self, reply, **_kwargs):
@@ -288,36 +234,25 @@
                 if not handler.done():
                     handler.set_result(reply)
             else:
                 Log.debug("Unrequested message: {}", reply, ":str")
 
     def _build_response(self, tid):
         """Return a deferred response for the current request."""
-        my_future = self.create_future()
-        if not self._connected:
+        my_future = asyncio.Future()
+        if not self.transport:
             self.raise_future(my_future, ConnectionException("Client is not connected"))
         else:
             self.transaction.addTransaction(my_future, tid)
         return my_future
 
-    @property
-    def async_connected(self):
-        """Return connection status."""
-        return self._connected
-
-    async def async_close(self):
-        """Close connection."""
-        if self.transport:
-            self.transport.close()
-        self._connected = False
-
     # ----------------------------------------------------------------------- #
     # Internal methods
     # ----------------------------------------------------------------------- #
-    def send(self, request):
+    def send(self, request):  # pylint: disable=invalid-overridden-method
         """Send request.
 
         :meta private:
         """
         if self.state != ModbusTransactionState.RETRYING:
             Log.debug('New Transaction state "SENDING"')
             self.state = ModbusTransactionState.SENDING
@@ -331,15 +266,15 @@
         return size
 
     @classmethod
     def _get_address_family(cls, address):
         """Get the correct address family."""
         try:
             _ = socket.inet_pton(socket.AF_INET6, address)
-        except socket.error:  # not a valid ipv6 address
+        except OSError:  # not a valid ipv6 address
             return socket.AF_INET
         return socket.AF_INET6
 
     # ----------------------------------------------------------------------- #
     # The magic methods
     # ----------------------------------------------------------------------- #
     def __enter__(self):
@@ -365,15 +300,15 @@
 
     def __exit__(self, klass, value, traceback):
         """Implement the client with exit block."""
         self.close()
 
     async def __aexit__(self, klass, value, traceback):
         """Implement the client with exit block."""
-        await self.close()
+        self.close()
 
     def __str__(self):
         """Build a string representation of the connection.
 
         :returns: The string representation
         """
         return f"{self.__class__.__name__} {self.params.host}:{self.params.port}"
```

### Comparing `pymodbus-3.2.2/pymodbus/client/mixin.py` & `pymodbus-3.3.0/pymodbus/client/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
         :raises ModbusException:
         """
         return self.execute(
             pdu_reg_read.ReadWriteMultipleRegistersRequest(
                 read_address=read_address,
                 read_count=read_count,
                 write_address=write_address,
-                values=values,
+                write_registers=values,
                 slave=slave,
                 **kwargs,
             )
         )
 
     def read_fifo_queue(self, address: int = 0x0000, **kwargs: Any) -> ModbusResponse:
         """Read FIFO queue (code 0x18).
```

### Comparing `pymodbus-3.2.2/pymodbus/client/serial.py` & `pymodbus-3.3.0/pymodbus/client/serial.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Modbus client async serial communication."""
 import asyncio
 import time
+from contextlib import suppress
 from functools import partial
 from typing import Any, Type
 
 from pymodbus.client.base import ModbusBaseClient
-from pymodbus.client.serial_asyncio import create_serial_connection
 from pymodbus.constants import Defaults
 from pymodbus.exceptions import ConnectionException
 from pymodbus.framer import ModbusFramer
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
 from pymodbus.logging import Log
 from pymodbus.utilities import ModbusTransactionState
 
 
-try:
+with suppress(ImportError):
     import serial
-except ImportError:
-    pass
 
 
 class AsyncModbusSerialClient(ModbusBaseClient, asyncio.Protocol):
     """**AsyncModbusSerialClient**.
 
     :param port: Serial port used for communication.
     :param framer: (optional) Framer class.
@@ -39,15 +37,15 @@
         from pymodbus.client import AsyncModbusSerialClient
 
         async def run():
             client = AsyncModbusSerialClient("dev/serial0")
 
             await client.connect()
             ...
-            await client.close()
+            client.close()
     """
 
     transport = None
     framer = None
 
     def __init__(
         self,
@@ -57,116 +55,38 @@
         bytesize: int = Defaults.Bytesize,
         parity: str = Defaults.Parity,
         stopbits: int = Defaults.Stopbits,
         handle_local_echo: bool = Defaults.HandleLocalEcho,
         **kwargs: Any,
     ) -> None:
         """Initialize Asyncio Modbus Serial Client."""
-        super().__init__(framer=framer, **kwargs)
-        self.use_protocol = True
+        asyncio.Protocol.__init__(self)
+        ModbusBaseClient.__init__(self, framer=framer, **kwargs)
         self.params.port = port
         self.params.baudrate = baudrate
         self.params.bytesize = bytesize
         self.params.parity = parity
         self.params.stopbits = stopbits
         self.params.handle_local_echo = handle_local_echo
-        self.loop = None
-        self._connected_event = asyncio.Event()
-        self._reconnect_task = None
-
-    async def close(self):  # pylint: disable=invalid-overridden-method
-        """Stop connection."""
-
-        # prevent reconnect:
-        self.delay_ms = 0
-        if self.connected:
-            if self.transport:
-                self.transport.close()
-            await self.async_close()
-            await asyncio.sleep(0.1)
-
-        # if there is an unfinished delayed reconnection attempt pending, cancel it
-        if self._reconnect_task:
-            self._reconnect_task.cancel()
-            self._reconnect_task = None
-
-    def _create_protocol(self):
-        """Create a protocol instance."""
-        return self
+        self.setup_serial(False, port, baudrate, bytesize, parity, stopbits)
 
     @property
     def connected(self):
         """Connect internal."""
-        return self._connected_event.is_set()
+        return self.transport is not None
 
-    async def connect(self):  # pylint: disable=invalid-overridden-method
+    async def connect(self):
         """Connect Async client."""
-        # get current loop, if there are no loop a RuntimeError will be raised
-        self.loop = asyncio.get_running_loop()
-
-        Log.debug("Starting serial connection")
-        try:
-            await create_serial_connection(
-                self.loop,
-                self._create_protocol,
-                self.params.port,
-                baudrate=self.params.baudrate,
-                bytesize=self.params.bytesize,
-                stopbits=self.params.stopbits,
-                parity=self.params.parity,
-                timeout=self.params.timeout,
-                **self.params.kwargs,
-            )
-            await self._connected_event.wait()
-            Log.info("Connected to {}", self.params.port)
-        except Exception as exc:  # pylint: disable=broad-except
-            Log.warning("Failed to connect: {}", exc)
-            if self.delay_ms > 0:
-                self._launch_reconnect()
-        return self.connected
-
-    def client_made_connection(self, protocol):
-        """Notify successful connection."""
-        Log.info("Serial connected.")
-        if not self.connected:
-            self._connected_event.set()
-        else:
-            Log.error("Factory protocol connect callback called while connected.")
-
-    def client_lost_connection(self, protocol):
-        """Notify lost connection."""
-        Log.info("Serial lost connection.")
-        if protocol is not self:
-            Log.error("Serial: protocol is not self.")
-
-        self._connected_event.clear()
-        if self.delay_ms:
-            self._launch_reconnect()
-
-    def _launch_reconnect(self):
-        """Launch delayed reconnection coroutine"""
-        if self._reconnect_task:
-            Log.warning(
-                "Ignoring launch of delayed reconnection, another is in progress"
-            )
-        else:
-            # store the future in a member variable so we know we have a pending reconnection attempt
-            # also prevents its garbage collection
-            self._reconnect_task = asyncio.create_task(self._reconnect())
-
-    async def _reconnect(self):
-        """Reconnect."""
-        Log.debug("Waiting {} ms before next connection attempt.", self.delay_ms)
-        await asyncio.sleep(self.delay_ms / 1000)
-        self.delay_ms = min(2 * self.delay_ms, self.params.reconnect_delay_max)
-
-        self._reconnect_task = None
-        if self.params.on_reconnect_callback:
-            self.params.on_reconnect_callback()
-        return await self.connect()
+        # if reconnect_delay_current was set to 0 by close(), we need to set it back again
+        # so this instance will work
+        self.reset_delay()
+
+        # force reconnect if required:
+        Log.debug("Connecting to {}.", self.params.host)
+        return await self.transport_connect()
 
 
 class ModbusSerialClient(ModbusBaseClient):
     """**ModbusSerialClient**.
 
     :param port: Serial port used for communication.
     :param framer: (optional) Framer class.
@@ -214,43 +134,43 @@
         self.params.port = port
         self.params.baudrate = baudrate
         self.params.bytesize = bytesize
         self.params.parity = parity
         self.params.stopbits = stopbits
         self.params.handle_local_echo = handle_local_echo
         self.socket = None
+        self.use_sync = True
 
         self.last_frame_end = None
 
-        self._t0 = float((1 + 8 + 2)) / self.params.baudrate
+        self._t0 = float(1 + 8 + 2) / self.params.baudrate
 
         """
         The minimum delay is 0.01s and the maximum can be set to 0.05s.
         Setting too large a setting affects efficiency.
         """
         self._recv_interval = (
             (round((100 * self._t0), 2) + 0.01)
             if (round((100 * self._t0), 2) + 0.01) < 0.05
             else 0.05
         )
 
-        if isinstance(self.framer, ModbusRtuFramer):
-            if self.params.baudrate > 19200:
-                self.silent_interval = 1.75 / 1000  # ms
-            else:
-                self.inter_char_timeout = 1.5 * self._t0
-                self.silent_interval = 3.5 * self._t0
-            self.silent_interval = round(self.silent_interval, 6)
+        if self.params.baudrate > 19200:
+            self.silent_interval = 1.75 / 1000  # ms
+        else:
+            self.inter_char_timeout = 1.5 * self._t0
+            self.silent_interval = 3.5 * self._t0
+        self.silent_interval = round(self.silent_interval, 6)
 
     @property
     def connected(self):
         """Connect internal."""
         return self.connect()
 
-    def connect(self):
+    def connect(self):  # pylint: disable=invalid-overridden-method
         """Connect to the modbus serial server."""
         if self.socket:
             return True
         try:
             self.socket = serial.serial_for_url(
                 self.params.port,
                 timeout=self.params.timeout,
@@ -264,15 +184,15 @@
                     self.socket.interCharTimeout = self.inter_char_timeout
                 self.last_frame_end = None
         except serial.SerialException as msg:
             Log.error("{}", msg)
             self.close()
         return self.socket is not None
 
-    def close(self):
+    def close(self):  # pylint: disable=arguments-differ
         """Close the underlying socket connection."""
         if self.socket:
             self.socket.close()
         self.socket = None
 
     def _in_waiting(self):
         """Return _in_waiting."""
```

### Comparing `pymodbus-3.2.2/pymodbus/client/serial_asyncio/__init__.py` & `pymodbus-3.3.0/pymodbus/transport/serial_asyncio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # Implementation of asyncio support.
 #
 # This file is part of pySerial. https://github.com/pyserial/pyserial-asyncio
 # (C) 2015-2020 pySerial-team
 #
 # SPDX-License-Identifier:    BSD-3-Clause
@@ -12,20 +11,21 @@
 
 Posix platforms only, Python 3.5+ only.
 
 Windows event loops can not wait for serial ports with the current
 implementation. It should be possible to get that working though.
 """
 import asyncio
+import contextlib
 import os
 
-try:
+
+with contextlib.suppress(ImportError):
     import serial
-except ImportError:
-    pass
+
 
 try:
     import termios
 except ImportError:
     termios = None
 
 __version__ = "0.6"
@@ -37,15 +37,15 @@
     A transport class is an abstraction of a communication channel.
     This allows protocol implementations to be developed against the
     transport abstraction without needing to know the details of the
     underlying channel, such as whether it is a pipe, a socket, or
     indeed a serial port.
 
 
-    You generally won’t instantiate a transport yourself; instead, you
+    You generally won`t instantiate a transport yourself; instead, you
     will call `create_serial_connection` which will create the
     transport and try to initiate the underlying communication channel,
     calling you back when it succeeds.
     """
 
     def __init__(self, loop, protocol, serial_instance):
         super().__init__()
@@ -125,15 +125,16 @@
                 self._protocol.data_received(data)
 
     def write(self, data):
         """Write some data to the transport.
 
         This method does not block; it buffers the data and arranges
         for it to be sent out asynchronously.  Writes made after the
-        transport has been closed will be ignored."""
+        transport has been closed will be ignored.
+        """
         if self._closing:
             return
 
         if self.get_write_buffer_size() == 0:
             self._write_buffer.append(data)
             self._ensure_writer()
         else:
@@ -147,15 +148,15 @@
         Always returns False.
         """
         return False
 
     def pause_reading(self):
         """Pause the receiving end of the transport.
 
-        No data will be passed to the protocol’s data_received() method
+        No data will be passed to the protocol`s data_received() method
         until resume_reading() is called.
         """
         self._remove_reader()
 
     def resume_reading(self):
         """Resume the receiving end of the transport.
 
@@ -163,15 +164,15 @@
         method until pause_reading() is called.
         """
         self._ensure_reader()
 
     def set_write_buffer_limits(self, high=None, low=None):
         """Set the high- and low-water limits for write flow control.
 
-        These two values control when the protocol’s
+        These two values control when the protocol`s
         pause_writing()and resume_writing() methods are called. If
         specified, the low-water limit must be less than or equal to
         the high-water limit. Neither high nor low can be negative.
         """
         self._set_write_buffer_limits(high=high, low=low)
         self._maybe_pause_protocol()
 
@@ -193,15 +194,15 @@
         and buffered data will be lost. No more data will be received
         and further writes will be ignored.  The protocol's
         connection_lost() method will eventually be called.
         """
         self._abort(None)
 
     def flush(self):
-        """clears output buffer and stops any more data being written"""
+        """Clears output buffer and stops any more data being written"""
         self._remove_writer()
         self._write_buffer.clear()
         self._maybe_resume_protocol()
 
     def _maybe_pause_protocol(self):
         """To be called whenever the write-buffer size increases.
 
@@ -357,15 +358,15 @@
     def _set_write_buffer_limits(self, high=None, low=None):
         """Ensure consistent write-buffer limits."""
         if high is None:
             high = 64 * 1024 if low is None else 4 * low
         if low is None:
             low = high // 4
         if not high >= low >= 0:
-            raise ValueError("high (%r) must be >= low (%r) must be >= 0" % (high, low))
+            raise ValueError(f"high ({high!r}) must be >= low ({low!r}) must be >= 0")
         self._high_water = high
         self._low_water = low
 
     def _fatal_error(self, exc, message="Fatal error on serial transport"):
         """Report a fatal error to the event-loop and abort the transport."""
         self._loop.call_exception_handler(
             {
@@ -418,28 +419,27 @@
 
         Informs the protocol through connection_lost() and clears
         pending buffers and closes the serial connection.
         """
         assert self._closing
         assert not self._has_writer
         assert not self._has_reader
-        try:
-            self._serial.flush()
-        except (serial.SerialException if os.name == "nt" else termios.error):
-            # ignore serial errors which may happen if the serial device was
-            # hot-unplugged.
-            pass
-        try:
-            self._protocol.connection_lost(exc)
-        finally:
-            self._write_buffer.clear()
+        if self._serial:
+            with contextlib.suppress(Exception):
+                self._serial.flush()
+
             self._serial.close()
             self._serial = None
-            self._protocol = None
-            self._loop = None
+        if self._protocol:
+            with contextlib.suppress(Exception):
+                self._protocol.connection_lost(exc)
+
+            self._write_buffer.clear()
+        self._write_buffer.clear()
+        self._loop = None
 
 
 async def create_serial_connection(loop, protocol_factory, *args, **kwargs):
     """Create a connection to a new serial port instance.
 
     This function is a coroutine which will try to establish the
     connection.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pymodbus-3.2.2/pymodbus/client/sync_diag.py` & `pymodbus-3.3.0/pymodbus/framer/tls_framer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,177 @@
-"""Sync diag."""
-
-__all__ = [
-    "ModbusTcpDiagClient",
-    "get_client",
-]
-
-import socket
-import time
-
-from pymodbus.client.tcp import ModbusTcpClient
-from pymodbus.constants import Defaults
-from pymodbus.exceptions import ConnectionException
-from pymodbus.framer.socket_framer import ModbusSocketFramer
+"""TLS framer."""
+# pylint: disable=missing-type-doc
+import struct
+
+from pymodbus.exceptions import (
+    InvalidMessageReceivedException,
+    ModbusIOException,
+)
+from pymodbus.framer.base import TLS_FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 
 
-LOG_MSGS = {
-    "conn_msg": "Connecting to modbus device %s",
-    "connfail_msg": "Connection to (%s, %s) failed: %s",
-    "discon_msg": "Disconnecting from modbus device %s",
-    "timelimit_read_msg": "Modbus device read took %.4f seconds, "
-    "returned %s bytes in timelimit read",
-    "timeout_msg": "Modbus device timeout after %.4f seconds, returned %s bytes %s",
-    "delay_msg": "Modbus device read took %.4f seconds, "
-    "returned %s bytes of %s expected",
-    "read_msg": "Modbus device read took %.4f seconds, "
-    "returned %s bytes of %s expected",
-    "unexpected_dc_msg": "%s %s",
-}
-
-
-class ModbusTcpDiagClient(ModbusTcpClient):
-    """Variant of pymodbus.client.ModbusTcpClient.
-
-    With additional logging to diagnose network issues.
-
-    The following events are logged:
-
-    +---------+-----------------------------------------------------------------+
-    | Level   | Events                                                          |
-    +=========+=================================================================+
-    | ERROR   | Failure to connect to modbus slave; unexpected disconnect by    |
-    |         | modbus slave                                                    |
-    +---------+-----------------------------------------------------------------+
-    | WARNING | Timeout on normal read; read took longer than warn_delay_limit  |
-    +---------+-----------------------------------------------------------------+
-    | INFO    | Connection attempt to modbus slave; disconnection from modbus   |
-    |         | slave; each time limited read                                   |
-    +---------+-----------------------------------------------------------------+
-    | DEBUG   | Normal read with timing information                             |
-    +---------+-----------------------------------------------------------------+
-
-    Reads are differentiated between "normal", which reads a specified number of
-    bytes, and "time limited", which reads all data for a duration equal to the
-    timeout period configured for this instance.
-    """
+# --------------------------------------------------------------------------- #
+# Modbus TLS Message
+# --------------------------------------------------------------------------- #
+
+
+class ModbusTlsFramer(ModbusFramer):
+    """Modbus TLS Frame controller
 
-    def __init__(
-        self,
-        host="127.0.0.1",
-        port=Defaults.TcpPort,
-        framer=ModbusSocketFramer,
-        **kwargs,
-    ):
-        """Initialize a client instance.
-
-        The keys of LOG_MSGS can be used in kwargs to customize the messages.
-
-        :param host: The host to connect to (default 127.0.0.1)
-        :param port: The modbus port to connect to (default 502)
-        :param source_address: The source address tuple to bind to (default ("", 0))
-        :param timeout: The timeout to use for this socket (default Defaults.Timeout)
-        :param warn_delay_limit: Log reads that take longer than this as warning.
-               Default True sets it to half of "timeout". None never logs these as
-               warning, 0 logs everything as warning.
-        :param framer: The modbus framer to use (default ModbusSocketFramer)
-
-        .. note:: The host argument will accept ipv4 and ipv6 hosts
-        """
-        self.warn_delay_limit = kwargs.get("warn_delay_limit", True)
-        super().__init__(host, port, framer, **kwargs)
-        if self.warn_delay_limit is True:
-            self.warn_delay_limit = self.params.timeout / 2
-
-        # Set logging messages, defaulting to LOG_MSGS
-        for (k_item, v_item) in LOG_MSGS.items():
-            self.__dict__[k_item] = kwargs.get(k_item, v_item)
-
-    def connect(self):
-        """Connect to the modbus tcp server.
-
-        :returns: True if connection succeeded, False otherwise
-        """
-        if self.socket:
-            return True
-        try:
-            Log.info(LOG_MSGS["conn_msg"], self)
-            self.socket = socket.create_connection(
-                (self.params.host, self.params.port),
-                timeout=self.params.timeout,
-                source_address=self.params.source_address,
-            )
-        except socket.error as msg:
-            Log.error(LOG_MSGS["connfail_msg"], self.params.host, self.params.port, msg)
-            self.close()
-        return self.socket is not None
-
-    def close(self):
-        """Close the underlying socket connection."""
-        if self.socket:
-            Log.info(LOG_MSGS["discon_msg"], self)
-            self.socket.close()
-        self.socket = None
-
-    def recv(self, size):
-        """Receive data."""
-        try:
-            start = time.time()
-
-            result = super().recv(size)
-
-            delay = time.time() - start
-            if self.warn_delay_limit is not None and delay >= self.warn_delay_limit:
-                self._log_delayed_response(len(result), size, delay)
-            elif not size:
-                Log.debug(LOG_MSGS["timelimit_read_msg"], delay, len(result))
-            else:
-                Log.debug(LOG_MSGS["read_msg"], delay, len(result), size)
-
-            return result
-        except ConnectionException as exc:
-            # Only log actual network errors, "if not self.socket" then it's a internal code issue
-            if "Connection unexpectedly closed" in exc.string:
-                Log.error(LOG_MSGS["unexpected_dc_msg"], self, exc)
-            raise ConnectionException from exc
-
-    def _log_delayed_response(self, result_len, size, delay):
-        """Log delayed response."""
-        if not size and result_len > 0:
-            Log.info(LOG_MSGS["timelimit_read_msg"], delay, result_len)
-        elif (
-            (not result_len) or (size and result_len < size)
-        ) and delay >= self.params.timeout:
-            size_txt = size if size else "in timelimit read"
-            read_type = f"of {size_txt} expected"
-            Log.warning(LOG_MSGS["timeout_msg"], delay, result_len, read_type)
-        else:
-            Log.warning(LOG_MSGS["delay_msg"], delay, result_len, size)
-
-    def __str__(self):
-        """Build a string representation of the connection.
-
-        :returns: The string representation
-        """
-        return f"ModbusTcpDiagClient({self.params.host}:{self.params.port})"
-
-
-def get_client():
-    """Return an appropriate client based on logging level.
-
-    This will be ModbusTcpDiagClient by default, or the parent class
-    if the log level is such that the diagnostic client will not log
-    anything.
+    No prefix MBAP header before decrypted PDU is used as a message frame for
+    Modbus Security Application Protocol.  It allows us to easily separate
+    decrypted messages which is PDU as follows:
 
-    :returns: ModbusTcpClient or a child class thereof
+        [ Function Code] [ Data ]
+          1b               Nb
     """
-    return ModbusTcpDiagClient
+
+    method = "tls"
+
+    def __init__(self, decoder, client=None):
+        """Initialize a new instance of the framer.
+
+        :param decoder: The decoder factory implementation to use
+        """
+        super().__init__(decoder, client)
+        self._buffer = b""
+        self._header = {}
+        self._hsize = 0x0
+
+    # ----------------------------------------------------------------------- #
+    # Private Helper Functions
+    # ----------------------------------------------------------------------- #
+    def checkFrame(self):
+        """Check and decode the next frame.
+
+        Return true if we were successful.
+        """
+        if self.isFrameReady():
+            # we have at least a complete message, continue
+            if len(self._buffer) - self._hsize >= 1:
+                return True
+        # we don't have enough of a message yet, wait
+        return False
+
+    def advanceFrame(self):
+        """Skip over the current framed message.
+
+        This allows us to skip over the current message after we have processed
+        it or determined that it contains an error. It also has to reset the
+        current frame header handle
+        """
+        self._buffer = b""
+        self._header = {}
+
+    def isFrameReady(self):
+        """Check if we should continue decode logic.
+
+        This is meant to be used in a while loop in the decoding phase to let
+        the decoder factory know that there is still data in the buffer.
+
+        :returns: True if ready, False otherwise
+        """
+        return len(self._buffer) > self._hsize
+
+    def addToFrame(self, message):
+        """Add new packet data to the current frame buffer.
+
+        :param message: The most recent packet
+        """
+        self._buffer += message
+
+    def getFrame(self):
+        """Return the next frame from the buffered data.
+
+        :returns: The next full frame buffer
+        """
+        return self._buffer[self._hsize :]
+
+    def populateResult(self, _result):
+        """Populate the modbus result."""
+        return
+
+    # ----------------------------------------------------------------------- #
+    # Public Member Functions
+    # ----------------------------------------------------------------------- #
+    def decode_data(self, data):
+        """Decode data."""
+        if len(data) > self._hsize:
+            (fcode,) = struct.unpack(TLS_FRAME_HEADER, data[0 : self._hsize + 1])
+            return {"fcode": fcode}
+        return {}
+
+    def processIncomingPacket(self, data, callback, slave, **kwargs):
+        """Process new packet pattern.
+
+        This takes in a new request packet, adds it to the current
+        packet stream, and performs framing on it. That is, checks
+        for complete messages, and once found, will process all that
+        exist.  This handles the case when we read N + 1 or 1 // N
+        messages at a time instead of 1.
+
+        The processed and decoded messages are pushed to the callback
+        function to process and send.
+
+        :param data: The new packet data
+        :param callback: The function to send results to
+        :param slave: Process if slave id matcheks, ignore otherwise (could be a
+               list of slave ids (server) or single slave id(client/server)
+        :param kwargs:
+        """
+        if not isinstance(slave, (list, tuple)):
+            slave = [slave]
+        # no slave id for Modbus Security Application Protocol
+        single = kwargs.get("single", True)
+        Log.debug("Processing: {}", data, ":hex")
+        self.addToFrame(data)
+
+        if not self.isFrameReady():
+            return
+        if not self.checkFrame():
+            Log.debug("Frame check failed, ignoring!!")
+            self.resetFrame()
+            return
+        if not self._validate_slave_id(slave, single):
+            Log.debug("Not in valid slave id - {}, ignoring!!", slave)
+            self.resetFrame()
+        self._process(callback)
+
+    def _process(self, callback, error=False):
+        """Process incoming packets irrespective error condition."""
+        data = self.getRawFrame() if error else self.getFrame()
+        if (result := self.decoder.decode(data)) is None:
+            raise ModbusIOException("Unable to decode request")
+        if error and result.function_code < 0x80:
+            raise InvalidMessageReceivedException(result)
+        self.populateResult(result)
+        self.advanceFrame()
+        callback(result)  # defer or push to a thread?
+
+    def resetFrame(self):
+        """Reset the entire message frame.
+
+        This allows us to skip ovver errors that may be in the stream.
+        It is hard to know if we are simply out of sync or if there is
+        an error in the stream as we have no way to check the start or
+        end of the message (python just doesn't have the resolution to
+        check for millisecond delays).
+        """
+        self._buffer = b""
+
+    def getRawFrame(self):
+        """Return the complete buffer."""
+        return self._buffer
+
+    def buildPacket(self, message):
+        """Create a ready to send modbus packet.
+
+        :param message: The populated request/response to send
+        """
+        data = message.encode()
+        packet = struct.pack(TLS_FRAME_HEADER, message.function_code)
+        packet += data
+        return packet
+
+
+# __END__
```

### Comparing `pymodbus-3.2.2/pymodbus/client/tcp.py` & `pymodbus-3.3.0/pymodbus/client/tcp.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,132 +30,53 @@
         from pymodbus.client import AsyncModbusTcpClient
 
         async def run():
             client = AsyncModbusTcpClient("localhost")
 
             await client.connect()
             ...
-            await client.close()
+            client.close()
     """
 
     def __init__(
         self,
         host: str,
         port: int = Defaults.TcpPort,
         framer: Type[ModbusFramer] = ModbusSocketFramer,
         source_address: Tuple[str, int] = None,
         **kwargs: Any,
     ) -> None:
         """Initialize Asyncio Modbus TCP Client."""
-        super().__init__(framer=framer, **kwargs)
-        self.use_protocol = True
+        asyncio.Protocol.__init__(self)
+        ModbusBaseClient.__init__(self, framer=framer, **kwargs)
         self.params.host = host
         self.params.port = port
         self.params.source_address = source_address
-        self.loop = None
-        self.connected = False
-        self.delay_ms = self.params.reconnect_delay
-        self._reconnect_task = None
+        if "internal_no_setup" in kwargs:
+            return
+        if host.startswith("unix:"):
+            self.setup_unix(False, host[5:])
+        else:
+            self.setup_tcp(False, host, port)
 
-    async def connect(self):  # pylint: disable=invalid-overridden-method
+    async def connect(self):
         """Initiate connection to start client."""
 
-        # if delay_ms was set to 0 by close(), we need to set it back again
+        # if reconnect_delay_current was set to 0 by close(), we need to set it back again
         # so this instance will work
         self.reset_delay()
 
         # force reconnect if required:
-        self.loop = asyncio.get_running_loop()
         Log.debug("Connecting to {}:{}.", self.params.host, self.params.port)
-        return await self._connect()
-
-    async def close(self):  # pylint: disable=invalid-overridden-method
-        """Stop client."""
-        self.delay_ms = 0
-        if self.connected:
-            if self.transport:
-                self.transport.abort()
-                self.transport.close()
-            await self.async_close()
-            await asyncio.sleep(0.1)
-
-        if self._reconnect_task:
-            self._reconnect_task.cancel()
-            self._reconnect_task = None
-
-    def _create_protocol(self):
-        """Create initialized protocol instance with function."""
-        return self
-
-    async def _connect(self):
-        """Connect."""
-        Log.debug("Connecting.")
-        try:
-            if self.params.host.startswith("unix:"):
-                transport, protocol = await asyncio.wait_for(
-                    self.loop.create_unix_connection(
-                        self._create_protocol, path=self.params.host[5:]
-                    ),
-                    timeout=self.params.timeout,
-                )
-            else:
-                transport, protocol = await asyncio.wait_for(
-                    self.loop.create_connection(
-                        self._create_protocol,
-                        host=self.params.host,
-                        port=self.params.port,
-                    ),
-                    timeout=self.params.timeout,
-                )
-        except Exception as exc:  # pylint: disable=broad-except
-            Log.warning("Failed to connect: {}", exc)
-            if self.delay_ms > 0:
-                self._launch_reconnect()
-        else:
-            Log.info("Connected to {}:{}.", self.params.host, self.params.port)
-            self.reset_delay()
-            return transport, protocol
-
-    def client_made_connection(self, protocol):
-        """Notify successful connection."""
-        Log.info("Protocol made connection.")
-        if not self.connected:
-            self.connected = True
-        else:
-            Log.error("Factory protocol connect callback called while connected.")
+        return await self.transport_connect()
 
-    def client_lost_connection(self, protocol):
-        """Notify lost connection."""
-        Log.info("Protocol lost connection.")
-        if protocol is not self:
-            Log.error("Factory protocol cb from unknown protocol instance.")
-
-        self.connected = False
-        if self.delay_ms > 0:
-            self._launch_reconnect()
-
-    def _launch_reconnect(self):
-        """Launch delayed reconnection coroutine"""
-        if self._reconnect_task:
-            Log.warning(
-                "Ignoring launch of delayed reconnection, another is in progress"
-            )
-        else:
-            self._reconnect_task = asyncio.create_task(self._reconnect())
-
-    async def _reconnect(self):
-        """Reconnect."""
-        Log.debug("Waiting {} ms before next connection attempt.", self.delay_ms)
-        await asyncio.sleep(self.delay_ms / 1000)
-        self.delay_ms = min(2 * self.delay_ms, self.params.reconnect_delay_max)
-
-        self._reconnect_task = None
-        if self.params.on_reconnect_callback:
-            self.params.on_reconnect_callback()
-        return await self._connect()
+    @property
+    def connected(self):
+        """Return true if connected."""
+        return self.transport is not None
 
 
 class ModbusTcpClient(ModbusBaseClient):
     """**ModbusTcpClient**.
 
     :param host: Host IP address or host name
     :param port: (optional) Port used for communication
@@ -189,21 +110,22 @@
     ) -> None:
         """Initialize Modbus TCP Client."""
         super().__init__(framer=framer, **kwargs)
         self.params.host = host
         self.params.port = port
         self.params.source_address = source_address
         self.socket = None
+        self.use_sync = True
 
     @property
     def connected(self):
         """Connect internal."""
-        return self.connect()
+        return self.transport is not None
 
-    def connect(self):
+    def connect(self):  # pylint: disable=invalid-overridden-method
         """Connect to the modbus tcp server."""
         if self.socket:
             return True
         try:
             if self.params.host.startswith("unix:"):
                 self.socket = socket.socket(socket.AF_UNIX)
                 self.socket.settimeout(self.params.timeout)
@@ -214,25 +136,25 @@
                     timeout=self.params.timeout,
                     source_address=self.params.source_address,
                 )
             Log.debug(
                 "Connection to Modbus server established. Socket {}",
                 self.socket.getsockname(),
             )
-        except socket.error as msg:
+        except OSError as msg:
             Log.error(
                 "Connection to ({}, {}) failed: {}",
                 self.params.host,
                 self.params.port,
                 msg,
             )
             self.close()
         return self.socket is not None
 
-    def close(self):
+    def close(self):  # pylint: disable=arguments-differ
         """Close the underlying socket connection."""
         if self.socket:
             self.socket.close()
         self.socket = None
 
     def _check_read_buffer(self):
         """Check read buffer."""
@@ -307,17 +229,15 @@
             # to avoid infinite loops when there isn't an expected response
             # size and the slave sends noisy data continuously.
             if time_ > end:
                 break
 
         return b"".join(data)
 
-    def _handle_abrupt_socket_close(
-        self, size, data, duration
-    ):  # pylint: disable=missing-type-doc
+    def _handle_abrupt_socket_close(self, size, data, duration):
         """Handle unexpected socket close by remote end.
 
         Intended to be invoked after determining that the remote end
         has unexpectedly closed the connection, to clean up and handle
         the situation appropriately.
 
         :param size: The number of bytes that was attempted to read
```

### Comparing `pymodbus-3.2.2/pymodbus/client/tls.py` & `pymodbus-3.3.0/pymodbus/client/tls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Modbus client async TLS communication."""
-import asyncio
 import socket
 import ssl
 from typing import Any, Type
 
 from pymodbus.client.tcp import AsyncModbusTcpClient, ModbusTcpClient
 from pymodbus.constants import Defaults
 from pymodbus.framer import ModbusFramer
@@ -36,81 +35,79 @@
     sslctx.options |= ssl.OP_NO_SSLv3
     sslctx.options |= ssl.OP_NO_SSLv2
     if certfile and keyfile:
         sslctx.load_cert_chain(certfile=certfile, keyfile=keyfile, password=password)
     return sslctx
 
 
-class AsyncModbusTlsClient(AsyncModbusTcpClient, asyncio.Protocol):
+class AsyncModbusTlsClient(AsyncModbusTcpClient):
     """**AsyncModbusTlsClient**.
 
     :param host: Host IP address or host name
     :param port: (optional) Port used for communication
     :param framer: (optional) Framer class
     :param source_address: (optional) Source address of client
     :param sslctx: (optional) SSLContext to use for TLS
     :param certfile: (optional) Cert file path for TLS server request
     :param keyfile: (optional) Key file path for TLS server request
     :param password: (optional) Password for for decrypting private key file
     :param server_hostname: (optional) Bind certificate to host
     :param kwargs: (optional) Experimental parameters
 
+    ..tip::
+        See ModbusBaseClient for common parameters.
+
     Example::
 
         from pymodbus.client import AsyncModbusTlsClient
 
         async def run():
             client = AsyncModbusTlsClient("localhost")
 
             await client.connect()
             ...
-            await client.close()
+            client.close()
     """
 
     def __init__(
         self,
         host: str,
         port: int = Defaults.TlsPort,
         framer: Type[ModbusFramer] = ModbusTlsFramer,
-        sslctx: str = None,
+        sslctx: ssl.SSLContext = None,
         certfile: str = None,
         keyfile: str = None,
         password: str = None,
         server_hostname: str = None,
         **kwargs: Any,
     ):
         """Initialize Asyncio Modbus TLS Client."""
-        super().__init__(host, port=port, framer=framer, **kwargs)
+        AsyncModbusTcpClient.__init__(
+            self, host, port=port, framer=framer, internal_no_setup=True, **kwargs
+        )
         self.sslctx = sslctx_provider(sslctx, certfile, keyfile, password)
-        self.params.sslctx = sslctx
         self.params.certfile = certfile
         self.params.keyfile = keyfile
         self.params.password = password
         self.params.server_hostname = server_hostname
-        AsyncModbusTcpClient.__init__(self, host, port=port, framer=framer, **kwargs)
+        self.setup_tls(
+            False, host, port, sslctx, certfile, keyfile, password, server_hostname
+        )
 
-    async def _connect(self):
-        """Connect to server."""
-        Log.debug("Connecting tls.")
-        try:
-            return await self.loop.create_connection(
-                self._create_protocol,
-                self.params.host,
-                self.params.port,
-                ssl=self.sslctx,
-                server_hostname=self.params.server_hostname,
-            )
-        except Exception as exc:  # pylint: disable=broad-except
-            Log.warning("Failed to connect: {}", exc)
-            if self.delay_ms > 0:
-                self._launch_reconnect()
-            return
-        Log.info("Connected to {}:{}.", self.params.host, self.params.port)
+    async def connect(self):
+        """Initiate connection to start client."""
+
+        # if reconnect_delay_current was set to 0 by close(), we need to set it back again
+        # so this instance will work
         self.reset_delay()
 
+        # force reconnect if required:
+        Log.debug("Connecting to {}:{}.", self.params.host, self.params.port)
+        return await self.transport_connect()
+
 
 class ModbusTlsClient(ModbusTcpClient):
     """**ModbusTlsClient**.
 
     :param host: Host IP address or host name
     :param port: (optional) Port used for communication
     :param framer: (optional) Framer class
@@ -118,14 +115,17 @@
     :param sslctx: (optional) SSLContext to use for TLS
     :param certfile: (optional) Cert file path for TLS server request
     :param keyfile: (optional) Key file path for TLS server request
     :param password: (optional) Password for decrypting private key file
     :param server_hostname: (optional) Bind certificate to host
     :param kwargs: (optional) Experimental parameters
 
+    ..tip::
+        See ModbusBaseClient for common parameters.
+
     Example::
 
         from pymodbus.client import ModbusTlsClient
 
         async def run():
             client = ModbusTlsClient("localhost")
 
@@ -157,30 +157,30 @@
         self.params.keyfile = keyfile
         self.params.password = password
         self.params.server_hostname = server_hostname
 
     @property
     def connected(self):
         """Connect internal."""
-        return self.connect()
+        return self.transport is not None
 
     def connect(self):
         """Connect to the modbus tls server."""
         if self.socket:
             return True
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             if self.params.source_address:
                 sock.bind(self.params.source_address)
             self.socket = self.sslctx.wrap_socket(
                 sock, server_side=False, server_hostname=self.params.host
             )
             self.socket.settimeout(self.params.timeout)
             self.socket.connect((self.params.host, self.params.port))
-        except socket.error as msg:
+        except OSError as msg:
             Log.error(
                 "Connection to ({}, {}) failed: {}",
                 self.params.host,
                 self.params.port,
                 msg,
             )
             self.close()
```

### Comparing `pymodbus-3.2.2/pymodbus/constants.py` & `pymodbus-3.3.0/pymodbus/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     .. attribute:: SlaveOff
 
        This indicates that the given modbus slave is not running
     """
 
     Waiting = 0xFFFF
     Ready = 0x0000
-    On = 0xFF00  # pylint: disable=invalid-name
+    On = 0xFF00
     Off = 0x0000
     SlaveOn = 0xFF
     SlaveOff = 0x00
 
     def __init__(self):
         """Prohibit objects."""
         raise RuntimeError(INTERNAL_ERROR)
```

### Comparing `pymodbus-3.2.2/pymodbus/datastore/context.py` & `pymodbus-3.3.0/pymodbus/datastore/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,40 +72,40 @@
 
         :param fc_as_hex: The function we are working with
         :param address: The starting address
         :param count: The number of values to test
         :returns: True if the request in within range, False otherwise
         """
         if not self.zero_mode:
-            address = address + 1
+            address += 1
         Log.debug("validate: fc-[{}] address-{}: count-{}", fc_as_hex, address, count)
         return self.store[self.decode(fc_as_hex)].validate(address, count)
 
     def getValues(self, fc_as_hex, address, count=1):
         """Get `count` values from datastore.
 
         :param fc_as_hex: The function we are working with
         :param address: The starting address
         :param count: The number of values to retrieve
         :returns: The requested values from a:a+c
         """
         if not self.zero_mode:
-            address = address + 1
+            address += 1
         Log.debug("getValues: fc-[{}] address-{}: count-{}", fc_as_hex, address, count)
         return self.store[self.decode(fc_as_hex)].getValues(address, count)
 
     def setValues(self, fc_as_hex, address, values):
         """Set the datastore with the supplied values.
 
         :param fc_as_hex: The function we are working with
         :param address: The starting address
         :param values: The new values to be set
         """
         if not self.zero_mode:
-            address = address + 1
+            address += 1
         Log.debug("setValues[{}] address-{}: count-{}", fc_as_hex, address, len(values))
         self.store[self.decode(fc_as_hex)].setValues(address, values)
 
     def register(self, function_code, fc_as_hex, datablock=None):
         """Register a datablock with the slave context.
 
         :param function_code: function code (int)
```

### Comparing `pymodbus-3.2.2/pymodbus/datastore/remote.py` & `pymodbus-3.3.0/pymodbus/datastore/remote.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/datastore/simulator.py` & `pymodbus-3.3.0/pymodbus/datastore/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,16 +550,17 @@
 
         :meta private:
         """
         if func_code in self._bits_func_code:
             # Bit count, correct to register count
             count = int((count + WORD_SIZE - 1) / WORD_SIZE)
             address = int(address / 16)
+
         real_address = self.fc_offset[func_code] + address
-        if real_address <= 0 or real_address > self.register_count:
+        if real_address < 0 or real_address > self.register_count:
             return False
 
         fx_write = func_code in self._write_func_code
         return self.loop_validate(real_address, real_address + count, fx_write)
 
     def getValues(self, func_code, address, count=1):
         """Return the requested values of the datastore.
```

### Comparing `pymodbus-3.2.2/pymodbus/datastore/store.py` & `pymodbus-3.3.0/pymodbus/datastore/store.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/device.py` & `pymodbus-3.3.0/pymodbus/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
     All activity should be logged here and all diagnostic requests
     should come from here.
     """
 
     __mode = "ASCII"
     __diagnostic = [False] * 16
     __listen_only = False
-    __delimiter = "\r"
+    __delimiter = b"\r"
     __counters = ModbusCountersHandler()
     __identity = ModbusDeviceIdentification()
     __plus = ModbusPlusStatistics()
     __events: List[ModbusEvent] = []
 
     # -------------------------------------------------------------------------#
     #  Magic
```

### Comparing `pymodbus-3.2.2/pymodbus/diag_message.py` & `pymodbus-3.3.0/pymodbus/diag_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,30 +142,30 @@
         """
         packet = struct.pack(">H", self.sub_function_code)
         if self.message is not None:
             if isinstance(self.message, str):
                 packet += self.message.encode()
             elif isinstance(self.message, bytes):
                 packet += self.message
-            elif isinstance(self.message, list):
+            elif isinstance(self.message, (list, tuple)):
                 for piece in self.message:
                     packet += struct.pack(">H", piece)
             elif isinstance(self.message, int):
                 packet += struct.pack(">H", self.message)
         return packet
 
     def decode(self, data):
         """Decode diagnostic response.
 
         :param data: The data to decode into the function code
         """
         word_len = len(data) // 2
         if len(data) % 2:
             word_len += 1
-            data = data + b"0"
+            data += b"0"
         data = struct.unpack(">" + "H" * word_len, data)
         (
             self.sub_function_code,  # pylint: disable=attribute-defined-outside-init
             self.message,
         ) = (
             data[0],
             data[1:],
```

### Comparing `pymodbus-3.2.2/pymodbus/events.py` & `pymodbus-3.3.0/pymodbus/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     """Define modbus events."""
 
     def encode(self):
         """Encode the status bits to an event message.
 
         :raises NotImplementedException:
         """
-        raise NotImplementedException()
+        raise NotImplementedException
 
     def decode(self, event):
         """Decode the event message to its status bits.
 
         :param event: The event to decode
         :raises NotImplementedException:
         """
-        raise NotImplementedException()
+        raise NotImplementedException
 
 
 class RemoteReceiveEvent(ModbusEvent):
     """Remote device MODBUS Receive Event.
 
     The remote device stores this type of event byte when a query message
     is received. It is stored before the remote device processes the message.
@@ -50,25 +50,25 @@
 
     def __init__(self, **kwargs):
         """Initialize a new event instance."""
         self.overrun = kwargs.get("overrun", False)
         self.listen = kwargs.get("listen", False)
         self.broadcast = kwargs.get("broadcast", False)
 
-    def encode(self):
+    def encode(self) -> bytes:
         """Encode the status bits to an event message.
 
         :returns: The encoded event message
         """
         bits = [False] * 3
         bits += [self.overrun, self.listen, self.broadcast, True]
         packet = pack_bitstring(bits)
         return packet
 
-    def decode(self, event):
+    def decode(self, event: bytes) -> None:
         """Decode the event message to its status bits.
 
         :param event: The event to decode
         """
         bits = unpack_bitstring(event)
         self.overrun = bits[4]
         self.listen = bits[5]
```

### Comparing `pymodbus-3.2.2/pymodbus/exceptions.py` & `pymodbus-3.3.0/pymodbus/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/factory.py` & `pymodbus-3.3.0/pymodbus/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,17 +80,21 @@
     GetCommEventLogRequest,
     GetCommEventLogResponse,
     ReadExceptionStatusRequest,
     ReadExceptionStatusResponse,
     ReportSlaveIdRequest,
     ReportSlaveIdResponse,
 )
-from pymodbus.pdu import ExceptionResponse, IllegalFunctionRequest
+from pymodbus.pdu import (
+    ExceptionResponse,
+    IllegalFunctionRequest,
+    ModbusRequest,
+    ModbusResponse,
+)
 from pymodbus.pdu import ModbusExceptions as ecode
-from pymodbus.pdu import ModbusRequest, ModbusResponse
 from pymodbus.register_read_message import (
     ReadHoldingRegistersRequest,
     ReadHoldingRegistersResponse,
     ReadInputRegistersRequest,
     ReadInputRegistersResponse,
     ReadWriteMultipleRegistersRequest,
     ReadWriteMultipleRegistersResponse,
@@ -160,15 +164,15 @@
     def getFCdict(cls):
         """Build function code - class list."""
         return {f.function_code: f for f in cls.__function_table}
 
     def __init__(self):
         """Initialize the client lookup tables."""
         functions = {f.function_code for f in self.__function_table}
-        self.__lookup = self.getFCdict()
+        self.lookup = self.getFCdict()
         self.__sub_lookup = {f: {} for f in functions}
         for f in self.__sub_function_table:
             self.__sub_lookup[f.function_code][f.sub_function_code] = f
 
     def decode(self, message):
         """Decode a request packet
 
@@ -183,31 +187,31 @@
 
     def lookupPduClass(self, function_code):
         """Use `function_code` to determine the class of the PDU.
 
         :param function_code: The function code specified in a frame.
         :returns: The class of the PDU that has a matching `function_code`.
         """
-        return self.__lookup.get(function_code, ExceptionResponse)
+        return self.lookup.get(function_code, ExceptionResponse)
 
     def _helper(self, data):
         """Generate the correct request object from a valid request packet.
 
         This decodes from a list of the currently implemented request types.
 
         :param data: The request packet to decode
         :returns: The decoded request or illegal function request object
         """
         function_code = int(data[0])
-        if not (request := self.__lookup.get(function_code, lambda: None)()):
+        if not (request := self.lookup.get(function_code, lambda: None)()):
             Log.debug("Factory Request[{}]", function_code)
             request = IllegalFunctionRequest(function_code)
         else:
-            fc_string = "%s: %s" % (  # pylint: disable=consider-using-f-string
-                str(self.__lookup[function_code])  # pylint: disable=use-maxsplit-arg
+            fc_string = "{}: {}".format(  # pylint: disable=consider-using-f-string
+                str(self.lookup[function_code])  # pylint: disable=use-maxsplit-arg
                 .split(".")[-1]
                 .rstrip('">"'),
                 function_code,
             )
             Log.debug("Factory Request[{}]", fc_string)
         request.decode(data[1:])
 
@@ -226,15 +230,15 @@
         """
         if function and not issubclass(function, ModbusRequest):
             raise MessageRegisterException(
                 f'"{function.__class__.__name__}" is Not a valid Modbus Message'
                 ". Class needs to be derived from "
                 "`pymodbus.pdu.ModbusRequest` "
             )
-        self.__lookup[function.function_code] = function
+        self.lookup[function.function_code] = function
         if hasattr(function, "sub_function_code"):
             if function.function_code not in self.__sub_lookup:
                 self.__sub_lookup[function.function_code] = {}
             self.__sub_lookup[function.function_code][
                 function.sub_function_code
             ] = function
 
@@ -289,26 +293,26 @@
         GetClearModbusPlusResponse,
         ReadDeviceInformationResponse,
     ]
 
     def __init__(self):
         """Initialize the client lookup tables."""
         functions = {f.function_code for f in self.function_table}
-        self.__lookup = {f.function_code: f for f in self.function_table}
+        self.lookup = {f.function_code: f for f in self.function_table}
         self.__sub_lookup = {f: {} for f in functions}
         for f in self.__sub_function_table:
             self.__sub_lookup[f.function_code][f.sub_function_code] = f
 
     def lookupPduClass(self, function_code):
         """Use `function_code` to determine the class of the PDU.
 
         :param function_code: The function code specified in a frame.
         :returns: The class of the PDU that has a matching `function_code`.
         """
-        return self.__lookup.get(function_code, ExceptionResponse)
+        return self.lookup.get(function_code, ExceptionResponse)
 
     def decode(self, message):
         """Decode a response packet.
 
         :param message: The raw packet to decode
         :return: The decoded modbus message or None if error
         """
@@ -326,23 +330,23 @@
         This decodes from a list of the currently implemented request types.
 
         :param data: The response packet to decode
         :returns: The decoded request or an exception response object
         :raises ModbusException:
         """
         fc_string = function_code = int(data[0])
-        if function_code in self.__lookup:
-            fc_string = "%s: %s" % (  # pylint: disable=consider-using-f-string
-                str(self.__lookup[function_code])  # pylint: disable=use-maxsplit-arg
+        if function_code in self.lookup:
+            fc_string = "{}: {}".format(  # pylint: disable=consider-using-f-string
+                str(self.lookup[function_code])  # pylint: disable=use-maxsplit-arg
                 .split(".")[-1]
                 .rstrip('">"'),
                 function_code,
             )
         Log.debug("Factory Response[{}]", fc_string)
-        response = self.__lookup.get(function_code, lambda: None)()
+        response = self.lookup.get(function_code, lambda: None)()
         if function_code > 0x80:
             code = function_code & 0x7F  # strip error portion
             response = ExceptionResponse(code, ecode.IllegalFunction)
         if not response:
             raise ModbusException(f"Unknown response {function_code}")
         response.decode(data[1:])
 
@@ -357,14 +361,14 @@
         """Register a function and sub function class with the decoder."""
         if function and not issubclass(function, ModbusResponse):
             raise MessageRegisterException(
                 f'"{function.__class__.__name__}" is Not a valid Modbus Message'
                 ". Class needs to be derived from "
                 "`pymodbus.pdu.ModbusResponse` "
             )
-        self.__lookup[function.function_code] = function
+        self.lookup[function.function_code] = function
         if hasattr(function, "sub_function_code"):
             if function.function_code not in self.__sub_lookup:
                 self.__sub_lookup[function.function_code] = {}
             self.__sub_lookup[function.function_code][
                 function.sub_function_code
             ] = function
```

### Comparing `pymodbus-3.2.2/pymodbus/file_message.py` & `pymodbus-3.3.0/pymodbus/file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/framer/__init__.py` & `pymodbus-3.3.0/pymodbus/framer/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 """Framer start."""
 # pylint: disable=missing-type-doc
+from typing import Any, Dict, Union
+
+from pymodbus.factory import ClientDecoder, ServerDecoder
 
 
 # Unit ID, Function Code
 BYTE_ORDER = ">"
 FRAME_HEADER = "BB"
 
 # Transaction Id, Protocol ID, Length, Unit ID, Function Code
@@ -14,36 +17,41 @@
 
 
 class ModbusFramer:
     """Base Framer class."""
 
     name = ""
 
-    def __init__(self, decoder, client=None):
+    def __init__(
+        self,
+        decoder: Union[ClientDecoder, ServerDecoder],
+        client=None,
+    ) -> None:
         """Initialize a new instance of the framer.
 
         :param decoder: The decoder implementation to use
         """
         self.decoder = decoder
         self.client = client
+        self._header: Dict[str, Any] = {}
 
-    def _validate_slave_id(self, slaves, single):
+    def _validate_slave_id(self, slaves: list, single: bool) -> bool:
         """Validate if the received data is valid for the client.
 
         :param slaves: list of slave id for which the transaction is valid
         :param single: Set to true to treat this as a single context
         :return:
         """
         if single:
             return True
         if 0 in slaves or 0xFF in slaves:
             # Handle Modbus TCP slave identifier (0x00 0r 0xFF)
             # in asynchronous requests
             return True
-        return self._header["uid"] in slaves  # pylint: disable=no-member
+        return self._header["uid"] in slaves
 
     def sendPacket(self, message):
         """Send packets on the bus.
 
         With 3.5char delay between frames
         :param message: Message to be sent over the bus
         :return:
```

### Comparing `pymodbus-3.2.2/pymodbus/framer/ascii_framer.py` & `pymodbus-3.3.0/pymodbus/framer/ascii_framer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Ascii_framer."""
 # pylint: disable=missing-type-doc
 import struct
 from binascii import a2b_hex, b2a_hex
 
 from pymodbus.exceptions import ModbusIOException
-from pymodbus.framer import BYTE_ORDER, FRAME_HEADER, ModbusFramer
+from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.utilities import checkLRC, computeLRC
 
 
 ASCII_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 
@@ -162,28 +162,28 @@
         :raises ModbusIOException:
         """
         if not isinstance(slave, (list, tuple)):
             slave = [slave]
         single = kwargs.get("single", False)
         self.addToFrame(data)
         while self.isFrameReady():
-            if self.checkFrame():
-                if self._validate_slave_id(slave, single):
-                    frame = self.getFrame()
-                    if (result := self.decoder.decode(frame)) is None:
-                        raise ModbusIOException("Unable to decode response")
-                    self.populateResult(result)
-                    self.advanceFrame()
-                    callback(result)  # defer this
-                else:
-                    header_txt = self._header["uid"]
-                    Log.error("Not a valid slave id - {}, ignoring!!", header_txt)
-                    self.resetFrame()
-            else:
+            if not self.checkFrame():
                 break
+            if not self._validate_slave_id(slave, single):
+                header_txt = self._header["uid"]
+                Log.error("Not a valid slave id - {}, ignoring!!", header_txt)
+                self.resetFrame()
+                continue
+
+            frame = self.getFrame()
+            if (result := self.decoder.decode(frame)) is None:
+                raise ModbusIOException("Unable to decode response")
+            self.populateResult(result)
+            self.advanceFrame()
+            callback(result)  # defer this
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         Built off of a  modbus request/response
 
         :param message: The request/response to send
@@ -192,21 +192,16 @@
         encoded = message.encode()
         buffer = struct.pack(
             ASCII_FRAME_HEADER, message.slave_id, message.function_code
         )
         checksum = computeLRC(encoded + buffer)
 
         packet = bytearray()
-        params = (message.slave_id, message.function_code)
         packet.extend(self._start)
-        packet.extend(
-            ("%02x%02x" % params).encode()  # pylint: disable=consider-using-f-string
-        )
+        packet.extend(f"{message.slave_id:02x}{message.function_code:02x}".encode())
         packet.extend(b2a_hex(encoded))
-        packet.extend(
-            ("%02x" % checksum).encode()  # pylint: disable=consider-using-f-string
-        )
+        packet.extend(f"{checksum:02x}".encode())
         packet.extend(self._end)
         return bytes(packet).upper()
 
 
 # __END__
```

### Comparing `pymodbus-3.2.2/pymodbus/framer/binary_framer.py` & `pymodbus-3.3.0/pymodbus/framer/binary_framer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Binary framer."""
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.exceptions import ModbusIOException
-from pymodbus.framer import BYTE_ORDER, FRAME_HEADER, ModbusFramer
+from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.utilities import checkCRC, computeCRC
 
 
 BINARY_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 # --------------------------------------------------------------------------- #
@@ -61,15 +61,15 @@
         """Decode data."""
         if len(data) > self._hsize:
             uid = struct.unpack(">B", data[1:2])[0]
             fcode = struct.unpack(">B", data[2:3])[0]
             return {"slave": uid, "fcode": fcode}
         return {}
 
-    def checkFrame(self):
+    def checkFrame(self) -> bool:
         """Check and decode the next frame.
 
         :returns: True if we are successful, False otherwise
         """
         start = self._buffer.find(self._start)
         if start == -1:
             return False
@@ -80,25 +80,25 @@
             self._header["len"] = end
             self._header["uid"] = struct.unpack(">B", self._buffer[1:2])[0]
             self._header["crc"] = struct.unpack(">H", self._buffer[end - 2 : end])[0]
             data = self._buffer[start + 1 : end - 2]
             return checkCRC(data, self._header["crc"])
         return False
 
-    def advanceFrame(self):
+    def advanceFrame(self) -> None:
         """Skip over the current framed message.
 
         This allows us to skip over the current message after we have processed
         it or determined that it contains an error. It also has to reset the
         current frame header handle
         """
         self._buffer = self._buffer[self._header["len"] + 2 :]
         self._header = {"crc": 0x0000, "len": 0, "uid": 0x00}
 
-    def isFrameReady(self):
+    def isFrameReady(self) -> bool:
         """Check if we should continue decode logic.
 
         This is meant to be used in a while loop in the decoding phase to let
         the decoder know that there is still data in the buffer.
 
         :returns: True if ready, False otherwise
         """
@@ -159,31 +159,28 @@
         :raises ModbusIOException:
         """
         self.addToFrame(data)
         if not isinstance(slave, (list, tuple)):
             slave = [slave]
         single = kwargs.get("single", False)
         while self.isFrameReady():
-            if self.checkFrame():
-                if self._validate_slave_id(slave, single):
-                    if (result := self.decoder.decode(self.getFrame())) is None:
-                        raise ModbusIOException("Unable to decode response")
-                    self.populateResult(result)
-                    self.advanceFrame()
-                    callback(result)  # defer or push to a thread?
-                else:
-                    header_txt = self._header["uid"]
-                    Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
-                    self.resetFrame()
-                    break
-
-            else:
+            if not self.checkFrame():
                 Log.debug("Frame check failed, ignoring!!")
                 self.resetFrame()
                 break
+            if not self._validate_slave_id(slave, single):
+                header_txt = self._header["uid"]
+                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
+                self.resetFrame()
+                break
+            if (result := self.decoder.decode(self.getFrame())) is None:
+                raise ModbusIOException("Unable to decode response")
+            self.populateResult(result)
+            self.advanceFrame()
+            callback(result)  # defer or push to a thread?
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The request/response to send
         :returns: The encoded packet
         """
```

### Comparing `pymodbus-3.2.2/pymodbus/framer/rtu_framer.py` & `pymodbus-3.3.0/pymodbus/framer/rtu_framer.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import struct
 import time
 
 from pymodbus.exceptions import (
     InvalidMessageReceivedException,
     ModbusIOException,
 )
-from pymodbus.framer import BYTE_ORDER, FRAME_HEADER, ModbusFramer
+from pymodbus.framer.base import BYTE_ORDER, FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 from pymodbus.utilities import ModbusTransactionState, checkCRC, computeCRC
 
 
 RTU_FRAME_HEADER = BYTE_ORDER + FRAME_HEADER
 
 
@@ -60,14 +60,15 @@
         """
         super().__init__(decoder, client)
         self._buffer = b""
         self._header = {"uid": 0x00, "len": 0, "crc": b"\x00\x00"}
         self._hsize = 0x01
         self._end = b"\x0d\x0a"
         self._min_frame_size = 4
+        self.function_codes = set(self.decoder.lookup) if self.decoder else {}
 
     # ----------------------------------------------------------------------- #
     # Private Helper Functions
     # ----------------------------------------------------------------------- #
     def decode_data(self, data):
         """Decode data."""
         if len(data) > self._hsize:
@@ -113,15 +114,15 @@
         an error in the stream as we have no way to check the start or
         end of the message (python just doesn't have the resolution to
         check for millisecond delays).
         """
         Log.debug(
             "Resetting frame - Current Frame in buffer - {}", self._buffer, ":hex"
         )
-        self._buffer = b""
+        # self._buffer = b""
         self._header = {"uid": 0x00, "len": 0, "crc": b"\x00\x00"}
 
     def isFrameReady(self):
         """Check if we should continue decode logic.
 
         This is meant to be used in a while loop in the decoding phase to let
         the decoder know that there is still data in the buffer.
@@ -187,14 +188,31 @@
         that is copied.
 
         :param result: The response packet
         """
         result.slave_id = self._header["uid"]
         result.transaction_id = self._header["uid"]
 
+    def getFrameStart(self, slaves, broadcast, skip_cur_frame):
+        """Scan buffer for a relevant frame start."""
+        start = 1 if skip_cur_frame else 0
+        if (buf_len := len(self._buffer)) < 4:
+            return False
+        for i in range(start, buf_len - 3):  # <slave id><function code><crc 2 bytes>
+            if not broadcast and self._buffer[i] not in slaves:
+                continue
+            if self._buffer[i + 1] not in self.function_codes:
+                continue
+            if i:
+                self._buffer = self._buffer[i:]  # remove preceding trash.
+            return True
+        if buf_len > 3:
+            self._buffer = self._buffer[-3:]
+        return False
+
     # ----------------------------------------------------------------------- #
     # Public Member Functions
     # ----------------------------------------------------------------------- #
     def processIncomingPacket(self, data, callback, slave, **kwargs):
         """Process new packet pattern.
 
         This takes in a new request packet, adds it to the current
@@ -210,33 +228,34 @@
         :param callback: The function to send results to
         :param slave: Process if slave id matches, ignore otherwise (could be a
                list of slave ids (server) or single slave id(client/server)
         :param kwargs:
         """
         if not isinstance(slave, (list, tuple)):
             slave = [slave]
+        broadcast = not slave[0]
         self.addToFrame(data)
         single = kwargs.get("single", False)
-        while True:
-            if self.isFrameReady():
-                if self.checkFrame():
-                    if self._validate_slave_id(slave, single):
-                        self._process(callback)
-                    else:
-                        header_txt = self._header["uid"]
-                        Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
-                        self.resetFrame()
-                        break
-                else:
-                    Log.debug("Frame check failed, ignoring!!")
-                    self.resetFrame()
-                    break
-            else:
+        skip_cur_frame = False
+        while self.getFrameStart(slave, broadcast, skip_cur_frame):
+            if not self.isFrameReady():
                 Log.debug("Frame - [{}] not ready", data)
                 break
+            if not self.checkFrame():
+                Log.debug("Frame check failed, ignoring!!")
+                self.resetFrame()
+                skip_cur_frame = True
+                continue
+            if not self._validate_slave_id(slave, single):
+                header_txt = self._header["uid"]
+                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
+                self.resetFrame()
+                skip_cur_frame = True
+                continue
+            self._process(callback)
 
     def buildPacket(self, message):
         """Create a ready to send modbus packet.
 
         :param message: The populated request/response to send
         """
         data = message.encode()
```

### Comparing `pymodbus-3.2.2/pymodbus/framer/socket_framer.py` & `pymodbus-3.3.0/pymodbus/framer/socket_framer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=missing-type-doc
 import struct
 
 from pymodbus.exceptions import (
     InvalidMessageReceivedException,
     ModbusIOException,
 )
-from pymodbus.framer import SOCKET_FRAME_HEADER, ModbusFramer
+from pymodbus.framer.base import SOCKET_FRAME_HEADER, ModbusFramer
 from pymodbus.logging import Log
 
 
 # --------------------------------------------------------------------------- #
 # Modbus TCP Message
 # --------------------------------------------------------------------------- #
 
@@ -133,66 +133,63 @@
                 "pid": pid,
                 "length": length,
                 "slave": uid,
                 "fcode": fcode,
             }
         return {}
 
-    def processIncomingPacket(self, data, callback, slave, **kwargs):
+    def processIncomingPacket(self, data, callback, slave, tid: int = None, **kwargs):
         """Process new packet pattern.
 
         This takes in a new request packet, adds it to the current
         packet stream, and performs framing on it. That is, checks
         for complete messages, and once found, will process all that
         exist.  This handles the case when we read N + 1 or 1 // N
         messages at a time instead of 1.
 
         The processed and decoded messages are pushed to the callback
         function to process and send.
-
-        :param data: The new packet data
-        :param callback: The function to send results to
-        :param slave: Process if slave id matches, ignore otherwise (could be a
-               list of slave ids (server) or single slave id(client/server)
-        :param kwargs:
         """
         if not isinstance(slave, (list, tuple)):
             slave = [slave]
         single = kwargs.get("single", False)
         Log.debug("Processing: {}", data, ":hex")
         self.addToFrame(data)
         while True:
-            if self.isFrameReady():
-                if self.checkFrame():
-                    if self._validate_slave_id(slave, single):
-                        self._process(callback)
-                    else:
-                        header_txt = self._header["uid"]
-                        Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
-                        self.resetFrame()
-                else:
-                    Log.debug("Frame check failed, ignoring!!")
-                    self.resetFrame()
-            else:
+            if not self.isFrameReady():
                 if len(self._buffer):
                     # Possible error ???
                     if self._header["len"] < 2:
-                        self._process(callback, error=True)
+                        self._process(callback, tid, error=True)
                 break
+            if not self.checkFrame():
+                Log.debug("Frame check failed, ignoring!!")
+                self.resetFrame()
+                continue
+            if not self._validate_slave_id(slave, single):
+                header_txt = self._header["uid"]
+                Log.debug("Not a valid slave id - {}, ignoring!!", header_txt)
+                self.resetFrame()
+                continue
+            self._process(callback, tid)
 
-    def _process(self, callback, error=False):
+    def _process(self, callback, tid, error=False):
         """Process incoming packets irrespective error condition."""
         data = self.getRawFrame() if error else self.getFrame()
         if (result := self.decoder.decode(data)) is None:
+            self.resetFrame()
             raise ModbusIOException("Unable to decode request")
         if error and result.function_code < 0x80:
             raise InvalidMessageReceivedException(result)
         self.populateResult(result)
         self.advanceFrame()
-        callback(result)  # defer or push to a thread?
+        if tid and tid != result.transaction_id:
+            self.resetFrame()
+        else:
+            callback(result)  # defer or push to a thread?
 
     def resetFrame(self):
         """Reset the entire message frame.
 
         This allows us to skip ovver errors that may be in the stream.
         It is hard to know if we are simply out of sync or if there is
         an error in the stream as we have no way to check the start or
```

### Comparing `pymodbus-3.2.2/pymodbus/logging.py` & `pymodbus-3.3.0/pymodbus/logging.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/mei_message.py` & `pymodbus-3.3.0/pymodbus/mei_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         """
         packet = struct.pack(
             ">BBB", self.sub_function_code, self.read_code, self.conformity
         )
         self.space_left = 253 - 6
         objects = b""
         try:
-            for (object_id, data) in iter(self.information.items()):
+            for object_id, data in iter(self.information.items()):
                 if isinstance(data, list):
                     for item in data:
                         objects += self._encode_object(object_id, item)
                 else:
                     objects += self._encode_object(object_id, data)
         except _OutOfSpaceException as exc:
             self.next_object_id = exc.oid
```

### Comparing `pymodbus-3.2.2/pymodbus/other_message.py` & `pymodbus-3.3.0/pymodbus/other_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,17 +471,13 @@
         :param data: The packet data to decode
         """
         self.byte_count = int(data[0])
         self.identifier = data[1 : self.byte_count + 1]
         status = int(data[-1])
         self.status = status == ModbusStatus.SlaveOn
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Build a representation of the response.
 
         :returns: The string representation of the response
         """
-        arguments = (self.function_code, self.identifier, self.status)
-        return (
-            "ReportSlaveIdResponse(%s, %s, %s)"  # pylint: disable=consider-using-f-string
-            % arguments
-        )
+        return f"ReportSlaveIdResponse({self.function_code}, {self.identifier}, {self.status})"
```

### Comparing `pymodbus-3.2.2/pymodbus/payload.py` & `pymodbus-3.3.0/pymodbus/payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 __all__ = [
     "BinaryPayloadBuilder",
     "BinaryPayloadDecoder",
 ]
 
 # pylint: disable=missing-type-doc
 from struct import pack, unpack
+from typing import List
 
 from pymodbus.constants import Endian
 from pymodbus.exceptions import ParameterException
 from pymodbus.logging import Log
 from pymodbus.utilities import (
-    make_byte_string,
     pack_bitstring,
     unpack_bitstring,
 )
 
 
 WC = {"b": 1, "h": 2, "e": 2, "i": 4, "l": 4, "q": 8, "f": 4, "d": 8}
 
@@ -63,45 +63,40 @@
         # Pack values back based on correct byte order   #
         # ---------------------------------------------- #
 
         :param fstring:
         :param value: Value to be packed
         :return:
         """
-        value = pack(
-            "!{}".format(fstring), value  # pylint: disable=consider-using-f-string
-        )
+        value = pack(f"!{fstring}", value)
         wordorder = WC.get(fstring.lower()) // 2
         upperbyte = f"!{wordorder}H"
         payload = unpack(upperbyte, value)
 
         if self._wordorder == Endian.Little:
             payload = list(reversed(payload))
 
         fstring = self._byteorder + "H"
         payload = [pack(fstring, word) for word in payload]
         payload = b"".join(payload)
 
         return payload
 
-    def to_string(self):
-        """Return the payload buffer as a string.
-
-        :returns: The payload buffer as a string
-        """
+    def encode(self) -> bytes:
+        """Get the payload buffer encoded in bytes."""
         return b"".join(self._payload)
 
-    def __str__(self):
+    def __str__(self) -> str:
         """Return the payload buffer as a string.
 
         :returns: The payload buffer as a string
         """
-        return self.to_string().decode("utf-8")
+        return self.encode().decode("utf-8")
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset the payload buffer."""
         self._payload = []
 
     def to_registers(self):
         """Convert the payload buffer to register layout that can be used as a context block.
 
         :returns: The register layout to use as a block
@@ -112,152 +107,151 @@
         if self._repack:
             payload = [unpack(self._byteorder + "H", value)[0] for value in payload]
         else:
             payload = [unpack(fstring, value)[0] for value in payload]
         Log.debug("{}", payload)
         return payload
 
-    def to_coils(self):
+    def to_coils(self) -> List[bool]:
         """Convert the payload buffer into a coil layout that can be used as a context block.
 
         :returns: The coil layout to use as a block
         """
         payload = self.to_registers()
         coils = [bool(int(bit)) for reg in payload for bit in format(reg, "016b")]
         return coils
 
-    def build(self):
+    def build(self) -> List[bytes]:
         """Return the payload buffer as a list.
 
         This list is two bytes per element and can
         thus be treated as a list of registers.
 
         :returns: The payload buffer as a list
         """
-        string = self.to_string()
-        length = len(string)
-        string = string + (b"\x00" * (length % 2))
-        return [string[i : i + 2] for i in range(0, length, 2)]
+        buffer = self.encode()
+        length = len(buffer)
+        buffer += b"\x00" * (length % 2)
+        return [buffer[i : i + 2] for i in range(0, length, 2)]
 
-    def add_bits(self, values):
+    def add_bits(self, values: List[bool]) -> None:
         """Add a collection of bits to be encoded.
 
         If these are less than a multiple of eight,
         they will be left padded with 0 bits to make
         it so.
 
         :param values: The value to add to the buffer
         """
         value = pack_bitstring(values)
         self._payload.append(value)
 
-    def add_8bit_uint(self, value):
+    def add_8bit_uint(self, value: int) -> None:
         """Add a 8 bit unsigned int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = self._byteorder + "B"
         self._payload.append(pack(fstring, value))
 
-    def add_16bit_uint(self, value):
+    def add_16bit_uint(self, value: int) -> None:
         """Add a 16 bit unsigned int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = self._byteorder + "H"
         self._payload.append(pack(fstring, value))
 
-    def add_32bit_uint(self, value):
+    def add_32bit_uint(self, value: int) -> None:
         """Add a 32 bit unsigned int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "I"
         # fstring = self._byteorder + "I"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_64bit_uint(self, value):
+    def add_64bit_uint(self, value: int) -> None:
         """Add a 64 bit unsigned int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "Q"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_8bit_int(self, value):
+    def add_8bit_int(self, value: int) -> None:
         """Add a 8 bit signed int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = self._byteorder + "b"
         self._payload.append(pack(fstring, value))
 
-    def add_16bit_int(self, value):
+    def add_16bit_int(self, value: int) -> None:
         """Add a 16 bit signed int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = self._byteorder + "h"
         self._payload.append(pack(fstring, value))
 
-    def add_32bit_int(self, value):
+    def add_32bit_int(self, value: int) -> None:
         """Add a 32 bit signed int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "i"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_64bit_int(self, value):
+    def add_64bit_int(self, value: int) -> None:
         """Add a 64 bit signed int to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "q"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_16bit_float(self, value):
+    def add_16bit_float(self, value: float) -> None:
         """Add a 16 bit float to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "e"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_32bit_float(self, value):
+    def add_32bit_float(self, value: float) -> None:
         """Add a 32 bit float to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "f"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_64bit_float(self, value):
+    def add_64bit_float(self, value: float) -> None:
         """Add a 64 bit float(double) to the buffer.
 
         :param value: The value to add to the buffer
         """
         fstring = "d"
         p_string = self._pack_words(fstring, value)
         self._payload.append(p_string)
 
-    def add_string(self, value):
+    def add_string(self, value: str) -> None:
         """Add a string to the buffer.
 
         :param value: The value to add to the buffer
         """
-        value = make_byte_string(value)
         fstring = self._byteorder + str(len(value)) + "s"
-        self._payload.append(pack(fstring, value))
+        self._payload.append(pack(fstring, value.encode()))
 
 
 class BinaryPayloadDecoder:
     """A utility that helps decode payload messages from a modbus response message.
 
     It really is just a simple wrapper around
     the struct module, however it saves time looking up the format
@@ -340,15 +334,14 @@
         # Change Word order if little endian word order  #
         # Pack values back based on correct byte order   #
         # ---------------------------------------------- #
         :param fstring:
         :param handle: Value to be unpacked
         :return:
         """
-        handle = make_byte_string(handle)
         wc_value = WC.get(fstring.lower()) // 2
         handle = unpack(f"!{wc_value}H", handle)
         if self._wordorder == Endian.Little:
             handle = list(reversed(handle))
 
         # Repack as unsigned Integer
         handle = [pack(self._byteorder + "H", p) for p in handle]
@@ -361,38 +354,34 @@
         self._pointer = 0x00
 
     def decode_8bit_uint(self):
         """Decode a 8 bit unsigned int from the buffer."""
         self._pointer += 1
         fstring = self._byteorder + "B"
         handle = self._payload[self._pointer - 1 : self._pointer]
-        handle = make_byte_string(handle)
         return unpack(fstring, handle)[0]
 
     def decode_bits(self, package_len=1):
         """Decode a byte worth of bits from the buffer."""
         self._pointer += package_len
         # fstring = self._endian + "B"
         handle = self._payload[self._pointer - 1 : self._pointer]
-        handle = make_byte_string(handle)
         return unpack_bitstring(handle)
 
     def decode_16bit_uint(self):
         """Decode a 16 bit unsigned int from the buffer."""
         self._pointer += 2
         fstring = self._byteorder + "H"
         handle = self._payload[self._pointer - 2 : self._pointer]
-        handle = make_byte_string(handle)
         return unpack(fstring, handle)[0]
 
     def decode_32bit_uint(self):
         """Decode a 32 bit unsigned int from the buffer."""
         self._pointer += 4
         fstring = "I"
-        # fstring = "I"
         handle = self._payload[self._pointer - 4 : self._pointer]
         handle = self._unpack_words(fstring, handle)
         return unpack("!" + fstring, handle)[0]
 
     def decode_64bit_uint(self):
         """Decode a 64 bit unsigned int from the buffer."""
         self._pointer += 8
@@ -402,23 +391,21 @@
         return unpack("!" + fstring, handle)[0]
 
     def decode_8bit_int(self):
         """Decode a 8 bit signed int from the buffer."""
         self._pointer += 1
         fstring = self._byteorder + "b"
         handle = self._payload[self._pointer - 1 : self._pointer]
-        handle = make_byte_string(handle)
         return unpack(fstring, handle)[0]
 
     def decode_16bit_int(self):
         """Decode a 16 bit signed int from the buffer."""
         self._pointer += 2
         fstring = self._byteorder + "h"
         handle = self._payload[self._pointer - 2 : self._pointer]
-        handle = make_byte_string(handle)
         return unpack(fstring, handle)[0]
 
     def decode_32bit_int(self):
         """Decode a 32 bit signed int from the buffer."""
         self._pointer += 4
         fstring = "i"
         handle = self._payload[self._pointer - 4 : self._pointer]
```

### Comparing `pymodbus-3.2.2/pymodbus/pdu.py` & `pymodbus-3.3.0/pymodbus/pdu.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,14 +140,16 @@
     def __init__(self, slave=Defaults.Slave, **kwargs):
         """Proxy the lower level initializer.
 
         :param slave: Modbus slave slave ID
 
         """
         super().__init__(slave, **kwargs)
+        self.bits = []
+        self.registers = []
 
     def isError(self):
         """Check if the error is a success or failure."""
         return self.function_code > 0x80  # pylint: disable=no-member
 
 
 # --------------------------------------------------------------------------- #
```

### Comparing `pymodbus-3.2.2/pymodbus/register_read_message.py` & `pymodbus-3.3.0/pymodbus/register_read_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/register_write_message.py` & `pymodbus-3.3.0/pymodbus/register_write_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/repl/client/completer.py` & `pymodbus-3.3.0/pymodbus/repl/client/completer.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/repl/client/helper.py` & `pymodbus-3.3.0/pymodbus/repl/client/helper.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/repl/client/main.py` & `pymodbus-3.3.0/pymodbus/repl/client/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,19 +91,15 @@
         if ctx is not None and ctx.token_normalize_func is not None:
             value = ctx.token_normalize_func(value)
             for choice in self.casted_choices:  # pylint: disable=no-member
                 if ctx.token_normalize_func(choice) == value:
                     return choice
 
         self.fail(
-            "invalid choice: %s. (choose from %s)"  # pylint: disable=consider-using-f-string
-            % (
-                value,
-                ", ".join(self.choices),
-            ),
+            f"invalid choice: {value}. (choose from {', '.join(self.choices)})",
             param,
             ctx,
         )
         return None
 
 
 def _process_args(args: list, string: bool = True):
@@ -147,98 +143,111 @@
             except ValueError:
                 click.secho("Error parsing argument", fg="yellow")
                 execute = False
                 break
     return kwargs, execute
 
 
-def cli(client):  # pylint: disable=too-complex
-    """Run client definition."""
-    use_keys = KeyBindings()
-    history_file = pathlib.Path.home().joinpath(".pymodhis")
-
-    @use_keys.add("c-space")
-    def _(event):
-        """Initialize autocompletion, or select the next completion."""
-        buff = event.app.current_buffer
-        if buff.complete_state:
-            buff.complete_next()
-        else:
-            buff.start_completion(select_first=False)
+class CLI:  # pylint: disable=too-few-public-methods
+    """Client definition."""
 
-    @use_keys.add("enter", filter=has_selected_completion)
-    def _(event):
-        """Make the enter key work as the tab key only when showing the menu."""
-        event.current_buffer.complete_state = None
-        buffer = event.cli.current_buffer
-        buffer.complete_state = None
-
-    session = PromptSession(
-        lexer=PygmentsLexer(PythonLexer),
-        completer=CmdCompleter(client),
-        style=style,
-        complete_while_typing=True,
-        bottom_toolbar=bottom_toolbar,
-        key_bindings=use_keys,
-        history=FileHistory(history_file),
-        auto_suggest=AutoSuggestFromHistory(),
-    )
-    click.secho(TITLE, fg="green")
-    result = None
-    while True:  # pylint: disable=too-many-nested-blocks
-        try:
-
-            text = session.prompt("> ", complete_while_typing=True)
-            if text.strip().lower() == "help":
-                print_formatted_text(HTML("<u>Available commands:</u>"))
-                for cmd, obj in sorted(session.completer.commands.items()):
-                    if cmd != "help":
-                        print_formatted_text(
-                            HTML(
-                                "<skyblue>{:45s}</skyblue>"  # pylint: disable=consider-using-f-string
-                                "<seagreen>{:100s}"
-                                "</seagreen>".format(cmd, obj.help_text)
-                            )
-                        )
-
-                continue
-            if text.strip().lower() == "exit":
-                raise EOFError()
-            if text.strip().lower().startswith("client."):
-                try:
-                    text = text.strip().split()
-                    cmd = text[0].split(".")[1]
-                    args = text[1:]
-                    kwargs, execute = _process_args(args, string=False)
-                    if execute:
-                        if text[0] in CLIENT_ATTRIBUTES:
-                            result = Result(getattr(client, cmd))
-                        else:
-                            result = Result(getattr(client, cmd)(**kwargs))
-                        result.print_result()
-                except Exception as exc:  # pylint: disable=broad-except
-                    click.secho(repr(exc), fg="red")
-            elif text.strip().lower().startswith("result."):
-                if result:
-                    words = text.lower().split()
-                    if words[0] == "result.raw":
-                        result.raw()
-                    if words[0] == "result.decode":
-                        args = words[1:]
-                        kwargs, execute = _process_args(args)
-                        if execute:
-                            result.decode(**kwargs)
-        except KeyboardInterrupt:
-            continue  # Control-C pressed. Try again.
-        except EOFError:
-            break  # Control-D pressed.
-        except Exception as exc:  # pylint: disable=broad-except
-            click.secho(str(exc), fg="red")
+    def __init__(self, client):
+        """Set up client and keybindings."""
+
+        use_keys = KeyBindings()
+        history_file = pathlib.Path.home().joinpath(".pymodhis")
+        self.client = client
+
+        @use_keys.add("c-space")
+        def _(event):
+            """Initialize autocompletion, or select the next completion."""
+            buff = event.app.current_buffer
+            if buff.complete_state:
+                buff.complete_next()
+            else:
+                buff.start_completion(select_first=False)
+
+        @use_keys.add("enter", filter=has_selected_completion)
+        def _(event):
+            """Make the enter key work as the tab key only when showing the menu."""
+            event.current_buffer.complete_state = None
+            buffer = event.cli.current_buffer
+            buffer.complete_state = None
+
+        self.session = PromptSession(
+            lexer=PygmentsLexer(PythonLexer),
+            completer=CmdCompleter(client),
+            style=style,
+            complete_while_typing=True,
+            bottom_toolbar=bottom_toolbar,
+            key_bindings=use_keys,
+            history=FileHistory(history_file),
+            auto_suggest=AutoSuggestFromHistory(),
+        )
+        click.secho(TITLE, fg="green")
+
+    def _print_command_help(self, commands):
+        """Print a list of commands with help text."""
+        for cmd, obj in sorted(commands.items()):
+            if cmd != "help":
+                print_formatted_text(
+                    HTML(
+                        "<skyblue>{:45s}</skyblue>"  # pylint: disable=consider-using-f-string
+                        "<seagreen>{:100s}"
+                        "</seagreen>".format(cmd, obj.help_text)
+                    )
+                )
+
+    def _process_client(self, text, client):
+        """Process client commands."""
+        text = text.strip().split()
+        cmd = text[0].split(".")[1]
+        args = text[1:]
+        kwargs, execute = _process_args(args, string=False)
+        if execute:
+            if text[0] in CLIENT_ATTRIBUTES:
+                result = Result(getattr(client, cmd))
+            else:
+                result = Result(getattr(client, cmd)(**kwargs))
+            result.print_result()
+
+    def _process_result(self, text, result):
+        """Process result commands."""
+        words = text.split()
+        if words[0] == "result.raw":
+            result.raw()
+        if words[0] == "result.decode":
+            args = words[1:]
+            kwargs, execute = _process_args(args)
+            if execute:
+                result.decode(**kwargs)
+
+    def run(self):
+        """Run the REPL."""
+        result = None
+        while True:
+            try:
+                text = self.session.prompt("> ", complete_while_typing=True)
+                if text.strip().lower() == "help":
+                    print_formatted_text(HTML("<u>Available commands:</u>"))
+                    self._print_command_help(self.session.completer.commands)
+                elif text.strip().lower() == "exit":
+                    raise EOFError()
+                elif text.strip().lower().startswith("client."):
+                    self._process_client(text, self.client)
+                elif text.strip().lower().startswith("result.") and result:
+                    self._process_result(text, result)
+            except KeyboardInterrupt:
+                continue  # Control-C pressed. Try again.
+            except EOFError:
+                break  # Control-D pressed.
+            except Exception as exc:  # pylint: disable=broad-except
+                click.secho(str(exc), fg="red")
 
-    click.secho("GoodBye!", fg="blue")
+        click.secho("GoodBye!", fg="blue")
 
 
 @click.group("pymodbus-repl")
 @click.version_option(str(pymodbus_version), message=TITLE)
 @click.option("--verbose", is_flag=True, default=False, help="Verbose logs")
 @click.option(
     "--broadcast-support",
@@ -273,15 +282,15 @@
         use_format = (
             "%(asctime)-15s %(threadName)-15s "
             "%(levelname)-8s %(module)-15s:%(lineno)-8s %(message)s"
         )
         logging.basicConfig(format=use_format)
         _logger.setLevel(logging.DEBUG)
     ctx.obj = {
-        "broadcast": broadcast_support,
+        "broadcast_enable": broadcast_support,
         "retry_on_empty": retry_on_empty,
         "retry_on_invalid": retry_on_error,
         "retries": retries,
         "reset_socket": reset_socket,
     }
 
 
@@ -303,15 +312,16 @@
 def tcp(ctx, host, port, framer):
     """Define TCP."""
     kwargs = {"host": host, "port": port}
     kwargs.update(**ctx.obj)
     if framer == "rtu":
         kwargs["framer"] = ModbusRtuFramer
     client = ModbusTcpClient(**kwargs)
-    cli(client)
+    cli = CLI(client)
+    cli.run()
 
 
 @main.command("serial")
 @click.pass_context
 @click.option(
     "--method",
     default="rtu",
@@ -423,12 +433,13 @@
         xonxoff=xonxoff,
         rtscts=rtscts,
         dsrdtr=dsrdtr,
         timeout=timeout,
         write_timeout=write_timeout,
         **ctx.obj,
     )
-    cli(client)
+    cli = CLI(client)
+    cli.run()
 
 
 if __name__ == "__main__":
     main()  # pylint: disable=no-value-for-parameter
```

### Comparing `pymodbus-3.2.2/pymodbus/repl/client/mclient.py` & `pymodbus-3.3.0/pymodbus/repl/client/mclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         :returns: List of register values
         """
         resp = super().read_coils(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "bits": resp.bits}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def read_discrete_inputs(self, address, count=1, slave=Defaults.Slave, **kwargs):
         """Read `count` number of discrete inputs starting at offset `address`.
 
         :param address: The starting address to read from
         :param count: The number of coils to read
         :param slave: Modbus slave slave ID
@@ -116,15 +116,15 @@
         :return: List of bits
         """
         resp = super().read_discrete_inputs(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "bits": resp.bits}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     @handle_brodcast
     def write_coil(self, address, value, slave=Defaults.Slave, **kwargs):
         """Write `value` to coil at `address`.
 
         :param address: coil offset to write to
         :param value: bit value to write
@@ -192,15 +192,15 @@
         :return:
         """
         resp = super().read_holding_registers(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "registers": resp.registers}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def read_input_registers(self, address, count=1, slave=Defaults.Slave, **kwargs):
         """Read `count` number of input registers starting at `address`.
 
         :param address: starting register offset to read from to
         :param count: Number of registers to read
         :param slave: Modbus slave slave ID
@@ -208,15 +208,15 @@
         :return:
         """
         resp = super().read_input_registers(  # pylint: disable=no-member
             address, count, slave, **kwargs
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "registers": resp.registers}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def readwrite_registers(
         self,
         read_address=0,
         read_count=0,
         write_address=0,
         values=0,
@@ -242,15 +242,15 @@
             write_address=write_address,
             values=values,
             slave=slave,
             **kwargs,
         )
         if not resp.isError():
             return {"function_code": resp.function_code, "registers": resp.registers}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def mask_write_register(
         self,
         address=0x0000,
         and_mask=0xFFFF,
         or_mask=0x0000,
         slave=Defaults.Slave,
@@ -271,15 +271,15 @@
         if not resp.isError():
             return {
                 "function_code": resp.function_code,
                 "address": resp.address,
                 "and mask": resp.and_mask,
                 "or mask": resp.or_mask,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def read_device_information(self, read_code=None, object_id=0x00, **kwargs):
         """Read the identification and additional information of remote slave.
 
         :param read_code:  Read Device ID code (0x01/0x02/0x03/0x04)
         :param object_id: Identification of the first object to obtain.
         :param kwargs:
@@ -293,15 +293,15 @@
                 "information": resp.information,
                 "object count": resp.number_of_objects,
                 "conformity": resp.conformity,
                 "next object id": resp.next_object_id,
                 "more follows": resp.more_follows,
                 "space left": resp.space_left,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
     def report_slave_id(self, slave=Defaults.Slave, **kwargs):
         """Report information about remote slave ID.
 
         :param slave: Modbus slave ID
         :param kwargs:
         :return:
@@ -311,28 +311,28 @@
         if not resp.isError():
             return {
                 "function_code": resp.function_code,
                 "identifier": resp.identifier.decode("cp1252"),
                 "status": resp.status,
                 "byte count": resp.byte_count,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=slave)
 
     def read_exception_status(self, slave=Defaults.Slave, **kwargs):
         """Read contents of eight Exception Status output in a remote device.
 
         :param slave: Modbus slave ID
         :param kwargs:
         :return:
         """
         request = ReadExceptionStatusRequest(slave, **kwargs)
         resp = self.execute(request)  # pylint: disable=no-member
         if not resp.isError():
             return {"function_code": resp.function_code, "status": resp.status}
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
     def get_com_event_counter(self, **kwargs):
         """Read status word and an event count.
 
         From the remote device's communication event counter.
 
         :param kwargs:
@@ -342,15 +342,15 @@
         resp = self.execute(request)  # pylint: disable=no-member
         if not resp.isError():
             return {
                 "function_code": resp.function_code,
                 "status": resp.status,
                 "count": resp.count,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
     def get_com_event_log(self, **kwargs):
         """Read status word.
 
         Event count, message count, and a field of event
         bytes from the remote device.
 
@@ -363,26 +363,26 @@
             return {
                 "function_code": resp.function_code,
                 "status": resp.status,
                 "message count": resp.message_count,
                 "event count": resp.event_count,
                 "events": resp.events,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
     def _execute_diagnostic_request(self, request):
         """Execute diagnostic request."""
         resp = self.execute(request)  # pylint: disable=no-member
         if not resp.isError():
             return {
                 "function code": resp.function_code,
                 "sub function code": resp.sub_function_code,
                 "message": resp.message,
             }
-        return ExtendedRequestSupport._process_exception(resp)
+        return ExtendedRequestSupport._process_exception(resp, slave=request.slave_id)
 
     def return_query_data(self, message=0, **kwargs):
         """Loop back data sent in response.
 
         :param message: Message to be looped back
         :param kwargs:
         :return:
```

### Comparing `pymodbus-3.2.2/pymodbus/repl/server/cli.py` & `pymodbus-3.3.0/pymodbus/repl/server/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,101 +101,105 @@
     print_formatted_text(HTML("<u>Available commands:</u>"))
     for cmd, hlp in sorted(COMMAND_HELPS.items()):
         print_formatted_text(
             HTML(f"<skyblue>{cmd:45s}</skyblue><seagreen>{hlp:100s}</seagreen>")
         )
 
 
-async def interactive_shell(server):  # pylint: disable=too-complex
-    """Run CLI interactive shell."""
+def print_title():
+    """Print title - large if there are sufficient columns, otherwise small."""
     col = get_terminal_width()
     max_len = max(  # pylint: disable=consider-using-generator
         [len(t) for t in TITLE.split("\n")]
     )
     if col > max_len:
         info(TITLE)
     else:
         print_formatted_text(
             HTML(f'<u><b><style color="green">{SMALL_TITLE}</style></b></u>')
         )
+
+
+async def interactive_shell(server):
+    """Run CLI interactive shell."""
+    print_title()
     info("")
     completer = NestedCompleter.from_nested_dict(COMMANDS)
     session = PromptSession(
         "SERVER > ", completer=completer, bottom_toolbar=BOTTOM_TOOLBAR
     )
 
     # Run echo loop. Read text from stdin, and reply it back.
-    while True:  # pylint: disable=too-many-nested-blocks
+    while True:
         try:
-            invalid_command = False
             result = await session.prompt_async()
             if result == "exit":
                 await server.web_app.shutdown()
                 break
             if result == "help":
                 print_help()
                 continue
             if result == "clear":
                 clear()
                 continue
             if command := result.split():
                 if command[0] not in COMMANDS:
-                    invalid_command = True
-                if invalid_command:
                     warning(f"Invalid command or invalid usage of command - {command}")
                     continue
                 if len(command) == 1:
                     warning(f'Usage: "{USAGE}"')
                 else:
-                    args = command[1:]
-                    skip_next = False
-                    val_dict = {}
-                    for index, arg in enumerate(args):
-                        if skip_next:
-                            skip_next = False
-                            continue
-                        if "=" in arg:
-                            arg, value = arg.split("=")
-                        elif arg in COMMAND_ARGS:
-                            try:
-                                value = args[index + 1]
-                                skip_next = True
-                            except IndexError:
-                                error(f"Missing value for argument - {arg}")
-                                warning('Usage: "{USAGE}"')
-                                break
-                        valid = True
-                        if arg == "response_type":
-                            if value not in RESPONSE_TYPES:
-                                warning(f"Invalid response type request - {value}")
-                                warning(f"Choose from {RESPONSE_TYPES}")
-                                valid = False
-                        elif arg in {  # pylint: disable=confusing-consecutive-elif
-                            "error_code",
-                            "delay_by",
-                            "clear_after",
-                            "data_len",
-                        }:
-                            try:
-                                value = int(value)
-                            except ValueError:
-                                warning(f"Expected integer value for {arg}")
-                                valid = False
-
-                        if valid:
-                            val_dict[arg] = value
-                    if val_dict:
+                    val_dict = _process_args(command[1:])
+                    if val_dict:  # pylint: disable=consider-using-assignment-expr
                         server.update_manipulator_config(val_dict)
                         # server.manipulator_config = val_dict
                 # result = await run_command(tester, *command)
 
         except (EOFError, KeyboardInterrupt):
             return
 
 
+def _process_args(args) -> dict:
+    """Process arguments passed to CLI."""
+    skip_next = False
+    val_dict = {}
+    for index, arg in enumerate(args):
+        if skip_next:
+            skip_next = False
+            continue
+        if "=" in arg:
+            arg, value = arg.split("=")
+        elif arg in COMMAND_ARGS:
+            try:
+                value = args[index + 1]
+                skip_next = True
+            except IndexError:
+                error(f"Missing value for argument - {arg}")
+            warning('Usage: "{USAGE}"')
+            break
+        if arg == "response_type":
+            if value not in RESPONSE_TYPES:
+                warning(f"Invalid response type request - {value}")
+                warning(f"Choose from {RESPONSE_TYPES}")
+                continue
+        elif arg in {  # pylint: disable=confusing-consecutive-elif
+            "error_code",
+            "delay_by",
+            "clear_after",
+            "data_len",
+        }:
+            try:
+                value = int(value)
+            except ValueError:
+                warning(f"Expected integer value for {arg}")
+                continue
+        val_dict[arg] = value
+    return val_dict
+
+
 async def main(server):
     """Run main."""
     # with patch_stdout():
     try:
         await interactive_shell(server)
     finally:
         pass
```

### Comparing `pymodbus-3.2.2/pymodbus/repl/server/main.py` & `pymodbus-3.3.0/pymodbus/repl/server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         "-f",
         case_sensitive=False,
         autocompletion=framers,
         help="Modbus framer to use",
     ),
     modbus_port: int = typer.Option(5020, "--modbus-port", "-p", help="Modbus port"),
     modbus_slave_id: List[int] = typer.Option(
-        None, "--slave-id", "-u", help="Supported Modbus slave id's"
+        [1], "--slave-id", "-u", help="Supported Modbus slave id's"
     ),
     modbus_config_path: Path = typer.Option(
         None, help="Path to additional modbus server config"
     ),
     randomize: int = typer.Option(
         0,
         "--random",
@@ -194,19 +194,16 @@
         slave=modbus_slave_id,
         loop=loop,
         single=False,
         data_block_settings=data_block_settings,
         **web_app_config,
         **modbus_config,
     )
-    try:
+    if repl:
+        loop.run_until_complete(run_repl(app))
+    else:
         loop.run_until_complete(app.run_async(repl))
-        if repl:
-            loop.run_until_complete(run_repl(app))
         loop.run_forever()
 
-    except CANCELLED_ERROR:
-        print("Done!!!!!")
-
 
 if __name__ == "__main__":
     app()
```

### Comparing `pymodbus-3.2.2/pymodbus/server/__init__.py` & `pymodbus-3.3.0/pymodbus/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/server/async_io.py` & `pymodbus-3.3.0/pymodbus/server/async_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """Implementation of a Threaded Modbus Server."""
 # pylint: disable=missing-type-doc
 import asyncio
 import ssl
 import time
 import traceback
+from contextlib import suppress
 from typing import Union
 
-from pymodbus.client.serial_asyncio import create_serial_connection
 from pymodbus.constants import Defaults
 from pymodbus.datastore import ModbusServerContext
 from pymodbus.device import ModbusControlBlock, ModbusDeviceIdentification
 from pymodbus.exceptions import NoSuchSlaveException, NotImplementedException
 from pymodbus.factory import ServerDecoder
 from pymodbus.logging import Log
 from pymodbus.pdu import ModbusExceptions as merror
 from pymodbus.transaction import (
     ModbusAsciiFramer,
     ModbusRtuFramer,
     ModbusSocketFramer,
     ModbusTlsFramer,
 )
+from pymodbus.transport.serial_asyncio import create_serial_connection
 
 
-try:
+with suppress(ImportError):
     import serial
-except ImportError:
-    pass
 
 
 def sslctx_provider(
     sslctx=None, certfile=None, keyfile=None, password=None, reqclicert=False
 ):
     """Provide the SSLContext for ModbusTlsServer.
 
@@ -160,15 +159,15 @@
         except Exception as exc:  # pylint: disable=broad-except
             Log.error(
                 "Datastore unable to fulfill request: {}; {}",
                 exc,
                 traceback.format_exc(),
             )
 
-    async def handle(self):  # pylint: disable=too-complex
+    async def handle(self):
         """Return Asyncio coroutine which represents a single conversation.
 
         between the modbus slave and master
 
         Once the client connection is established, the data chunks will be
         fed to this coroutine via the asyncio.Queue object which is fed by
         the ModbusBaseRequestHandler class's callback Future.
@@ -198,16 +197,14 @@
                 data = await self._recv_()
                 if isinstance(data, tuple):
                     # addr is populated when talking over UDP
                     data, *addr = data
                 else:
                     addr = (None,)  # empty tuple
 
-                if not isinstance(slaves, (list, tuple)):
-                    slaves = [slaves]
                 # if broadcast is enabled make sure to
                 # process requests to address 0
                 if self.server.broadcast_enable:  # pragma: no cover
                     if 0 not in slaves:
                         slaves.append(0)
 
                 Log.debug("Handling data: {}", data, ":hex")
@@ -385,15 +382,15 @@
     only difference is that we have to specify who to send the
     resulting packet data to.
     """
 
     def __init__(self, owner):
         """Initialize."""
         super().__init__(owner)
-        _future = asyncio.get_running_loop().create_future()
+        _future = asyncio.Future()
         self.server.on_connection_terminated = _future
 
     def connection_lost(self, call_exc):
         """Handle connection lost."""
         super().connection_lost(call_exc)
         self.server.on_connection_terminated.set_result(True)
 
@@ -532,15 +529,15 @@
         )
         self.broadcast_enable = kwargs.get("broadcast_enable", Defaults.BroadcastEnable)
         self.response_manipulator = kwargs.get("response_manipulator", None)
         if isinstance(identity, ModbusDeviceIdentification):
             self.control.Identity.update(identity)
 
         # asyncio future that will be done once server has started
-        self.serving = self.loop.create_future()
+        self.serving = asyncio.Future()
         # constructors cannot be declared async, so we have to
         # defer the initialization of the server
         self.server = None
         self.request_tracer = None
         self.factory_parms = {}
 
     async def serve_forever(self):
@@ -592,15 +589,14 @@
         self,
         context,
         framer=None,
         identity=None,
         address=None,
         handler=None,
         allow_reuse_address=False,
-        defer_start=False,
         backlog=20,
         **kwargs,
     ):
         """Initialize the socket server.
 
         If the identify structure is not passed in, the ModbusControlBlock
         uses its own empty structure.
@@ -640,22 +636,22 @@
         self.broadcast_enable = kwargs.get("broadcast_enable", Defaults.BroadcastEnable)
         self.response_manipulator = kwargs.get("response_manipulator", None)
         self.request_tracer = kwargs.get("request_tracer", None)
         if isinstance(identity, ModbusDeviceIdentification):
             self.control.Identity.update(identity)
 
         # asyncio future that will be done once server has started
-        self.serving = self.loop.create_future()
+        self.serving = asyncio.Future()
         # constructors cannot be declared async, so we have to
         # defer the initialization of the server
         self.server = None
         self.factory_parms = {
             "reuse_address": allow_reuse_address,
             "backlog": backlog,
-            "start_serving": not defer_start,
+            "start_serving": True,
         }
 
     async def serve_forever(self):
         """Start endless loop."""
         if self.server is None:
             self.server = await self.loop.create_server(
                 lambda: self.handler(self),
@@ -713,15 +709,14 @@
         sslctx=None,
         certfile=None,
         keyfile=None,
         password=None,
         reqclicert=False,
         handler=None,
         allow_reuse_address=False,
-        defer_start=False,
         backlog=20,
         **kwargs,
     ):
         """Overloaded initializer for the socket server.
 
         If the identify structure is not passed in, the ModbusControlBlock
         uses its own empty structure.
@@ -754,15 +749,14 @@
         super().__init__(
             context,
             framer=framer,
             identity=identity,
             address=address,
             handler=handler,
             allow_reuse_address=allow_reuse_address,
-            defer_start=defer_start,
             backlog=backlog,
             **kwargs,
         )
         self.sslctx = sslctx_provider(sslctx, certfile, keyfile, password, reqclicert)
         self.factory_parms["ssl"] = self.sslctx
 
 
@@ -777,15 +771,14 @@
     def __init__(
         self,
         context,
         framer=None,
         identity=None,
         address=None,
         handler=None,
-        defer_start=False,
         backlog=20,
         **kwargs,
     ):
         """Overloaded initializer for the socket server.
 
         If the identify structure is not passed in, the ModbusControlBlock
         uses its own empty structure.
@@ -800,15 +793,14 @@
                             to a missing slave
         :param broadcast_enable: True to treat slave_id 0 as broadcast address,
                             False to treat 0 as any other slave_id
         :param response_manipulator: Callback method for
                             manipulating the response
         """
         # TO BE REMOVED:
-        self.defer_start = defer_start
         self.backlog = backlog
         # ----------------
         self.loop = asyncio.get_running_loop()
         self.decoder = ServerDecoder()
         self.framer = framer or ModbusSocketFramer
         self.context = context or ModbusServerContext()
         self.control = ModbusControlBlock()
@@ -822,16 +814,17 @@
 
         if isinstance(identity, ModbusDeviceIdentification):
             self.control.Identity.update(identity)
 
         self.protocol = None
         self.endpoint = None
         self.on_connection_terminated = None
+        self.stop_serving = self.loop.create_future()
         # asyncio future that will be done once server has started
-        self.serving = self.loop.create_future()
+        self.serving = asyncio.Future()
         self.factory_parms = {
             "local_addr": self.address,
             "allow_broadcast": True,
         }
         self.request_tracer = None
 
     async def serve_forever(self):
@@ -845,31 +838,35 @@
             except asyncio.exceptions.CancelledError:
                 raise
             except Exception as exc:
                 Log.error("Server unexpected exception {}", exc)
                 raise RuntimeError(exc) from exc
             Log.info("Server(UDP) listening.")
             self.serving.set_result(True)
+            await self.stop_serving
         else:
             raise RuntimeError(
                 "Can't call serve_forever on an already running server object"
             )
 
     async def shutdown(self):
         """Shutdown server."""
         await self.server_close()
 
     async def server_close(self):
         """Close server."""
         if self.endpoint:
             self.endpoint.running = False
+        if not self.stop_serving.done():
+            self.stop_serving.set_result(True)
         if self.endpoint is not None and self.endpoint.handler_task is not None:
             self.endpoint.handler_task.cancel()
         if self.protocol is not None:
             self.protocol.close()
+            # TBD await self.protocol.wait_closed()
             self.protocol = None
 
 
 class ModbusSerialServer:  # pylint: disable=too-many-instance-attributes
     """A modbus threaded serial socket server.
 
     We inherit and overload the socket server so that we
@@ -1068,18 +1065,16 @@
 
     @classmethod
     async def run(cls, server, custom_functions):
         """Help starting/stopping server."""
         for func in custom_functions:
             server.decoder.register(func)
         cls.active_server = _serverList(server)
-        try:
+        with suppress(asyncio.exceptions.CancelledError):
             await server.serve_forever()
-        except asyncio.CancelledError:
-            pass
 
     @classmethod
     async def async_stop(cls):
         """Wait for server stop."""
         if not cls.active_server:
             raise RuntimeError("ServerAsyncStop called without server task active.")
         await cls.active_server.server.shutdown()
```

### Comparing `pymodbus-3.2.2/pymodbus/server/reactive/default_config.py` & `pymodbus-3.3.0/pymodbus/server/reactive/default_config.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/pymodbus/server/reactive/main.py` & `pymodbus-3.3.0/pymodbus/server/reactive/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         :param fc_as_hex: The function we are working with
         :param address: The starting address
         :param count: The number of values to retrieve
         :returns: The requested values from a:a+c
         """
         if not self.zero_mode:
-            address = address + 1
+            address += 1
         Log.debug("getValues: fc-[{}] address-{}: count-{}", fc_as_hex, address, count)
         _block_type = self.decode(fc_as_hex)
         if self._randomize > 0 and _block_type in {"d", "i"}:
             with self._lock:
                 if not (self._read_counter.get(_block_type) % self._randomize):
                     # Update values
                     if _block_type == "d":
@@ -211,15 +211,15 @@
         self._runner = web.AppRunner(self._web_app)
         self._host = host
         self._port = int(port)
         self._modbus_server = modbus_server
         self._add_routes()
         self._counter = 0
         self._modbus_server.response_manipulator = self.manipulate_response
-        self._manipulator_config = dict(**DEFAULT_MANIPULATOR)
+        self._manipulator_config = {**DEFAULT_MANIPULATOR}
         self._web_app.on_startup.append(self.start_modbus_server)
         self._web_app.on_shutdown.append(self.stop_modbus_server)
 
     @property
     def web_app(self):
         """Start web_app."""
         return self._web_app
@@ -505,14 +505,13 @@
             server = server(context, framer=framer, identity=identity, **kwargs)
         else:
             server = server(
                 context,
                 framer=framer,
                 identity=identity,
                 address=(host, modbus_port),
-                defer_start=False,
                 **kwargs,
             )
         return ReactiveServer(host, web_port, server)
 
 
 # __END__
```

### Comparing `pymodbus-3.2.2/pymodbus/server/simulator/http_server.py` & `pymodbus-3.3.0/pymodbus/server/simulator/http_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
                 address=response.address if hasattr(response, "address") else -1,
                 count=response.count if hasattr(response, "count") else -1,
                 data="-",
             )
             self.call_list.append(tracer)
             self.call_monitor.trace_response = False
 
-        if not self.call_response.active == RESPONSE_INACTIVE:
+        if self.call_response.active != RESPONSE_INACTIVE:
             return response, False
 
         skip_encoding = False
         if self.call_response.active == RESPONSE_EMPTY:
             Log.warning("Sending empty response")
             response.should_respond = False
         elif self.call_response.active == RESPONSE_NORMAL:
```

### Comparing `pymodbus-3.2.2/pymodbus/server/simulator/main.py` & `pymodbus-3.3.0/pymodbus/server/simulator/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
   --json_file JSON_FILE
                         name of json_file, default is "setup.json"
   --custom_actions_module CUSTOM_ACTIONS_MODULE
                         python file with custom actions, default is none
 """
 import argparse
 import asyncio
+import os
 
 from pymodbus import pymodbus_apply_logging_config
 from pymodbus.logging import Log
 from pymodbus.server.simulator.http_server import ModbusSimulatorServer
 
 
 def get_commandline():
@@ -67,26 +68,28 @@
         help="use <http_host> as host to bind http listen",
         type=str,
     )
     parser.add_argument(
         "--http_port",
         help="use <http_port> as port to bind http listen",
         type=str,
+        default=8081,
     )
     parser.add_argument(
         "--log",
         choices=["critical", "error", "warning", "info", "debug"],
         help="set log level, default is info",
         default="info",
         type=str,
     )
     parser.add_argument(
         "--json_file",
         help='name of json file, default is "setup.json"',
         type=str,
+        default=os.path.join(os.path.dirname(__file__), "setup.json"),
     )
     parser.add_argument(
         "--log_file",
         help='name of server log file, default is "server.log"',
         type=str,
     )
     parser.add_argument(
@@ -105,16 +108,14 @@
             cmd_args[argument] = args.__dict__[argument]
     return cmd_args
 
 
 async def run_main():
     """Run server async."""
     cmd_args = get_commandline()
-    cmd_args["http_port"] = 8081
-    cmd_args["json_file"] = "./pymodbus/server/simulator/setup.json"
     task = ModbusSimulatorServer(**cmd_args)
     await task.run_forever()
 
 
 def main():
     """Run server."""
     asyncio.run(run_main(), debug=True)
```

### Comparing `pymodbus-3.2.2/pymodbus/transaction.py` & `pymodbus-3.3.0/pymodbus/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     "ModbusTlsFramer",
     "ModbusRtuFramer",
     "ModbusAsciiFramer",
     "ModbusBinaryFramer",
 ]
 
 # pylint: disable=missing-type-doc
-import socket
 import struct
 import time
+from contextlib import suppress
 from functools import partial
 from threading import RLock
 
 from pymodbus.constants import Defaults
 from pymodbus.exceptions import (
     InvalidMessageReceivedException,
     ModbusIOException,
@@ -120,15 +120,15 @@
         ):
             return False
 
         if "length" in mbap and exp_resp_len:
             return mbap.get("length") == exp_resp_len
         return True
 
-    def execute(self, request):  # pylint: disable=too-complex
+    def execute(self, request):  # noqa: C901
         """Start the producer to send the next request to consumer.write(Frame(request))."""
         with self._transaction_lock:
             try:
                 Log.debug(
                     "Current transaction state - {}",
                     ModbusTransactionState.to_string(self.client.state),
                 )
@@ -147,15 +147,15 @@
                     response = b"Broadcast write sent - no response expected"
                 else:
                     expected_response_length = None
                     if not isinstance(self.client.framer, ModbusSocketFramer):
                         if hasattr(request, "get_response_pdu_size"):
                             response_pdu_size = request.get_response_pdu_size()
                             if isinstance(self.client.framer, ModbusAsciiFramer):
-                                response_pdu_size = response_pdu_size * 2
+                                response_pdu_size *= 2
                             if response_pdu_size:
                                 expected_response_length = (
                                     self._calculate_response_length(response_pdu_size)
                                 )
                     if (  # pylint: disable=simplifiable-if-statement
                         request.slave_id in self._no_response_devices
                     ):
@@ -213,15 +213,18 @@
                             break
                         # full = False
                     addTransaction = partial(  # pylint: disable=invalid-name
                         self.addTransaction,
                         tid=request.transaction_id,
                     )
                     self.client.framer.processIncomingPacket(
-                        response, addTransaction, request.slave_id
+                        response,
+                        addTransaction,
+                        request.slave_id,
+                        tid=request.transaction_id,
                     )
                     if not (response := self.getTransaction(request.transaction_id)):
                         if len(self.transactions):
                             response = self.getTransaction(tid=0)
                         else:
                             last_exception = last_exception or (
                                 "No Response received from the remote slave"
@@ -313,31 +316,27 @@
                 and self.client.handle_local_echo is True
             ):
                 if self._recv(size, full) != packet:
                     return b"", "Wrong local echo"
             result = self._recv(response_length, full)
             # result2 = self._recv(response_length, full)
             Log.debug("RECV: {}", result, ":hex")
-        except (
-            socket.error,
-            ModbusIOException,
-            InvalidMessageReceivedException,
-        ) as msg:
+        except (OSError, ModbusIOException, InvalidMessageReceivedException) as msg:
             if self.reset_socket:
                 self.client.close()
             Log.debug("Transaction failed. ({}) ", msg)
             last_exception = msg
             result = b""
         return result, last_exception
 
     def _send(self, packet, _retrying=False):
         """Send."""
         return self.client.framer.sendPacket(packet)
 
-    def _recv(self, expected_response_length, full):  # pylint: disable=too-complex
+    def _recv(self, expected_response_length, full):  # noqa: C901
         """Receive."""
         total = None
         if not full:
             exception_length = self._calculate_exception_length()
             if isinstance(self.client.framer, ModbusSocketFramer):
                 min_size = 8
             elif isinstance(self.client.framer, ModbusRtuFramer):
@@ -375,23 +374,22 @@
                             self.client.framer._hsize  # pylint: disable=protected-access
                         )
                         length = struct.unpack(">H", read_min[4:6])[0] - 1
                         expected_response_length = h_size + length
                     elif expected_response_length is None and isinstance(
                         self.client.framer, ModbusRtuFramer
                     ):
-                        try:
+                        with suppress(
+                            IndexError  # response length indeterminate with available bytes
+                        ):
                             expected_response_length = (
                                 self.client.framer.get_expected_response_length(
                                     read_min
                                 )
                             )
-                        except IndexError:
-                            # Could not determine response length with available bytes
-                            pass
                     if expected_response_length is not None:
                         expected_response_length -= min_size
                         total = expected_response_length + min_size
                 else:
                     expected_response_length = exception_length - min_size
                     total = expected_response_length + min_size
             else:
```

### Comparing `pymodbus-3.2.2/pymodbus/utilities.py` & `pymodbus-3.3.0/pymodbus/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "computeLRC",
     "checkLRC",
     "rtuFrameSize",
 ]
 
 # pylint: disable=missing-type-doc
 import struct
+from typing import List
 
 
 class ModbusTransactionState:  # pylint: disable=too-few-public-methods
     """Modbus Client States."""
 
     IDLE = 0
     SENDING = 1
@@ -102,18 +103,18 @@
 
     return property(getter, setter)
 
 
 # --------------------------------------------------------------------------- #
 # Bit packing functions
 # --------------------------------------------------------------------------- #
-def pack_bitstring(bits):
-    """Create a string out of an array of bits.
+def pack_bitstring(bits: List[bool]) -> bytes:
+    """Create a bytestring out of a list of bits.
 
-    :param bits: A bit array
+    :param bits: A list of bits
 
     example::
 
         bits   = [False, True, False, True]
         result = pack_bitstring(bits)
     """
     ret = b""
@@ -129,45 +130,34 @@
             packed >>= 1
     if 0 < i < 8:
         packed >>= 7 - i
         ret += struct.pack(">B", packed)
     return ret
 
 
-def unpack_bitstring(string):
-    """Create bit array out of a string.
+def unpack_bitstring(data: bytes) -> List[bool]:
+    """Create bit list out of a bytestring.
 
-    :param string: The modbus data packet to decode
+    :param data: The modbus data packet to decode
 
     example::
 
         bytes  = "bytes to decode"
         result = unpack_bitstring(bytes)
     """
-    byte_count = len(string)
+    byte_count = len(data)
     bits = []
     for byte in range(byte_count):
-        value = int(int(string[byte]))
+        value = int(int(data[byte]))
         for _ in range(8):
             bits.append((value & 1) == 1)
             value >>= 1
     return bits
 
 
-def make_byte_string(byte_string):
-    """Return byte string from a given string, python3 specific fix.
-
-    :param byte_string:
-    :return:
-    """
-    if isinstance(byte_string, str):
-        byte_string = byte_string.encode()
-    return byte_string
-
-
 # --------------------------------------------------------------------------- #
 # Error Detection Functions
 # --------------------------------------------------------------------------- #
 
 
 def __generate_crc16_table():
     """Generate a crc16 lookup table.
```

### Comparing `pymodbus-3.2.2/pymodbus.egg-info/PKG-INFO` & `pymodbus-3.3.0/pymodbus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymodbus
-Version: 3.2.2
+Version: 3.3.0
 Summary: A fully featured modbus protocol stack in python
 Home-page: https://github.com/pymodbus-dev/pymodbus/
 Author: "Galen Collins, Jan Iversen"
 Maintainer: "dhoomakethu, janiversen"
 License: BSD-3-Clause
 Project-URL: Source Code, https://github.com/pymodbus-dev/pymodbus
 Project-URL: Bug Reports, https://github.com/pymodbus-dev/pymodbus/issues
@@ -55,17 +55,17 @@
    :target: https://github.com/pymodbus-dev/pymodbus/pkgs/container/pymodbus
    :alt: Docker Tags
 
 ------------------------------------------------------------
 Supported versions
 ------------------------------------------------------------
 
-Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python 2.7.x - 3.7).
+Version `2.5.3 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v2.5.3>`_ is the last 2.x release (Supports python >= 2.7, no longer supported).
 
-Version `3.2.2 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.2.2>`_ is the current release (Supports Python >=3.8).
+Version `3.3.0 <https://github.com/pymodbus-dev/pymodbus/releases/tag/v3.3.0>`_ is the current release (Supports Python >= 3.8).
 
 .. important::
    All API changes after 3.0.0 are documented in `API_changes.rst <https://github.com/pymodbus-dev/pymodbus/blob/dev/API_changes.rst>`_
 
 
 ------------------------------------------------------------
 Summary
@@ -280,15 +280,15 @@
 and maintenance development is merged here.
 
 -----------------------------------------------------------
 Install with Docker
 -----------------------------------------------------------
 Pull the latest image on ``dev`` branch with ``docker pull ghcr.io/pymodbus-dev/pymodbus:dev``::
 
-   doker pull ghcr.io/pymodbus-dev/pymodbus:dev
+   ❯ docker pull ghcr.io/pymodbus-dev/pymodbus:dev
    dev: Pulling from pymodbus-dev/pymodbus
    548fcab5fe88: Pull complete
    a4d3f9f008ef: Pull complete
    eb83acb05730: Pull complete
    71cd28d529fd: Pull complete
    66607ad8f4f0: Pull complete
    64dff4c66d3b: Pull complete
@@ -402,16 +402,15 @@
    make html
 
 ------------------------------------------------------------
 Contributing
 ------------------------------------------------------------
 Just fork the repo and raise your PR against `dev` branch.
 
-Here are some of the items waiting to be done:
-   https://github.com/pymodbus-dev/pymodbus/blob/dev/doc/TODO
+We always have more work than time, so feel free to open a discussion / issue on a theme you want to solve.
 
 ------------------------------------------------------------
 License Information
 ------------------------------------------------------------
 
 Pymodbus is built on top of code developed from/by:
   * Copyright (c) 2001-2005 S.W.A.C. GmbH, Germany.
```

### Comparing `pymodbus-3.2.2/pymodbus.egg-info/SOURCES.txt` & `pymodbus-3.3.0/pymodbus.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,38 +21,36 @@
 pymodbus/payload.py
 pymodbus/pdu.py
 pymodbus/py.typed
 pymodbus/register_read_message.py
 pymodbus/register_write_message.py
 pymodbus/transaction.py
 pymodbus/utilities.py
-pymodbus/version.py
 pymodbus.egg-info/PKG-INFO
 pymodbus.egg-info/SOURCES.txt
 pymodbus.egg-info/dependency_links.txt
 pymodbus.egg-info/entry_points.txt
 pymodbus.egg-info/requires.txt
 pymodbus.egg-info/top_level.txt
 pymodbus.egg-info/zip-safe
 pymodbus/client/__init__.py
 pymodbus/client/base.py
 pymodbus/client/mixin.py
 pymodbus/client/serial.py
-pymodbus/client/sync_diag.py
 pymodbus/client/tcp.py
 pymodbus/client/tls.py
 pymodbus/client/udp.py
-pymodbus/client/serial_asyncio/__init__.py
 pymodbus/datastore/__init__.py
 pymodbus/datastore/context.py
 pymodbus/datastore/remote.py
 pymodbus/datastore/simulator.py
 pymodbus/datastore/store.py
 pymodbus/framer/__init__.py
 pymodbus/framer/ascii_framer.py
+pymodbus/framer/base.py
 pymodbus/framer/binary_framer.py
 pymodbus/framer/rtu_framer.py
 pymodbus/framer/socket_framer.py
 pymodbus/framer/tls_framer.py
 pymodbus/repl/__init__.py
 pymodbus/repl/client/__init__.py
 pymodbus/repl/client/completer.py
@@ -67,20 +65,37 @@
 pymodbus/server/reactive/__init__.py
 pymodbus/server/reactive/default_config.py
 pymodbus/server/reactive/main.py
 pymodbus/server/simulator/__init__.py
 pymodbus/server/simulator/custom_actions.py
 pymodbus/server/simulator/http_server.py
 pymodbus/server/simulator/main.py
+pymodbus/server/simulator/setup.json
+pymodbus/server/simulator/web/apple120.png
+pymodbus/server/simulator/web/apple152.png
+pymodbus/server/simulator/web/apple60.png
+pymodbus/server/simulator/web/apple76.png
+pymodbus/server/simulator/web/favicon.ico
+pymodbus/server/simulator/web/index.html
+pymodbus/server/simulator/web/pymodbus.css
+pymodbus/server/simulator/web/welcome.html
+pymodbus/server/simulator/web/generator/calls
+pymodbus/server/simulator/web/generator/log
+pymodbus/server/simulator/web/generator/pymodbus_icon_original.png
+pymodbus/server/simulator/web/generator/registers
+pymodbus/server/simulator/web/generator/server
+pymodbus/transport/__init__.py
+pymodbus/transport/transport.py
+pymodbus/transport/serial_asyncio/__init__.py
 test/test_all_messages.py
 test/test_bit_read_messages.py
 test/test_bit_write_messages.py
 test/test_client.py
+test/test_client_faulty_response.py
 test/test_client_sync.py
-test/test_client_sync_diag.py
 test/test_device.py
 test/test_diag_messages.py
 test/test_events.py
 test/test_example_client_server.py
 test/test_examples.py
 test/test_exceptions.py
 test/test_factory.py
@@ -93,13 +108,14 @@
 test/test_pdu.py
 test/test_register_read_messages.py
 test/test_register_write_messages.py
 test/test_remote_datastore.py
 test/test_repl_client.py
 test/test_server_asyncio.py
 test/test_server_context.py
+test/test_server_multidrop.py
 test/test_server_task.py
 test/test_simulator.py
+test/test_sparse_datastore.py
 test/test_transaction.py
 test/test_unix_socket.py
-test/test_utilities.py
-test/test_version.py
+test/test_utilities.py
```

### Comparing `pymodbus-3.2.2/requirements.txt` & `pymodbus-3.3.0/requirements.txt`

 * *Files 22% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # depending on the usage profile it might work on other versions.
 # python_version>=3.8
 
 # -------------------------------------------------------------------
 # Required packages.
 # -------------------------------------------------------------------
 # install:required
-setuptools<66.0.0
 
 # -------------------------------------------------------------------
 # optional packages.
 # -------------------------------------------------------------------
 # These packages are optional for the runtime, but demanded for
 # document generation, development and test.
 #
@@ -43,27 +42,23 @@
 sphinx-rtd-theme==1.1.1
 
 
 # -------------------------------------------------------------------
 # development, everything needed to develop/test/check.
 # -------------------------------------------------------------------
 # install:development
-bandit==1.7.4
 codespell==2.2.2
 coverage==7.1.0
-flake8==6.0.0
-flake8-docstrings==1.7.0
-flake8-noqa==1.3.0
-flake8-comprehensions==3.10.1
-mypy==1.0.1
+mypy==1.3.0
 pre-commit==3.1.1
 pyflakes==3.0.1
 pydocstyle==6.3.0
 pycodestyle==2.10.0
-pylint==2.15.10
+pylint==2.17.2
 pytest==7.2.1
 pytest-asyncio==0.20.3
 pytest-cov==4.0.0
 pytest-timeout==2.1.0
 pytest-xdist==3.1.0
+ruff==0.0.261
 types-Pygments
 types-pyserial
```

### Comparing `pymodbus-3.2.2/setup.py` & `pymodbus-3.3.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 # --------------------------------------------------------------------------- #
 # initialization
 # --------------------------------------------------------------------------- #
 from setuptools import setup
 
 
-dependencies = {}
+dependencies: dict = {}
 with open("requirements.txt") as reqs:
     option = None
     for line in reqs.read().split("\n"):
-        if line == "":
+        if not line:
             option = None
         elif line.startswith("# install:"):
             option = line.split(":")[1]
             dependencies[option] = []
         elif not line.startswith("#") and option:
             dependencies[option].append(line)
 
@@ -26,9 +26,11 @@
 
 # --------------------------------------------------------------------------- #
 # configuration
 # --------------------------------------------------------------------------- #
 setup(
     install_requires=install_req,
     extras_require=dependencies,
-    package_data={"pymodbus": ["py.typed"]},
+    package_data={
+        "pymodbus": ["py.typed", "server/simulator/setup.json", "server/simulator/web/**/*"],
+    },
 )
```

### Comparing `pymodbus-3.2.2/test/test_all_messages.py` & `pymodbus-3.3.0/test/test_all_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_bit_read_messages.py` & `pymodbus-3.3.0/test/test_bit_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_bit_write_messages.py` & `pymodbus-3.3.0/test/test_bit_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_client.py` & `pymodbus-3.3.0/test/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pymodbus.diag_message as pdu_diag
 import pymodbus.other_message as pdu_other_msg
 import pymodbus.register_read_message as pdu_reg_read
 import pymodbus.register_write_message as pdu_req_write
 from pymodbus.client.base import ModbusBaseClient
 from pymodbus.client.mixin import ModbusClientMixin
 from pymodbus.constants import Defaults
-from pymodbus.exceptions import ConnectionException, NotImplementedException
+from pymodbus.exceptions import ConnectionException
 from pymodbus.framer.ascii_framer import ModbusAsciiFramer
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
 from pymodbus.framer.socket_framer import ModbusSocketFramer
 from pymodbus.framer.tls_framer import ModbusTlsFramer
 
 
 @pytest.mark.parametrize(
@@ -34,15 +34,15 @@
             {"toggle": False},
             {"address": 0x01, "values": [False, True]},
             {"address": 0x01, "values": [22, 44]},
         ]
     ],
 )
 @pytest.mark.parametrize(
-    "method, arg, pdu_request",
+    ("method", "arg", "pdu_request"),
     [
         ("read_coils", 1, pdu_bit_read.ReadCoilsRequest),
         ("read_discrete_inputs", 1, pdu_bit_read.ReadDiscreteInputsRequest),
         ("read_holding_registers", 1, pdu_reg_read.ReadHoldingRegistersRequest),
         ("read_input_registers", 1, pdu_reg_read.ReadInputRegistersRequest),
         ("write_coil", 2, pdu_bit_write.WriteSingleCoilRequest),
         ("write_register", 2, pdu_req_write.WriteSingleRegisterRequest),
@@ -202,15 +202,15 @@
                     "source_address": None,
                 },
             },
         },
     ],
 )
 @pytest.mark.parametrize(
-    "type_args, clientclass",
+    ("type_args", "clientclass"),
     [
         # TBD ("serial", lib_client.AsyncModbusSerialClient),
         # TBD ("serial", lib_client.ModbusSerialClient),
         ("tcp", lib_client.AsyncModbusTcpClient),
         ("tcp", lib_client.ModbusTcpClient),
         ("tls", lib_client.AsyncModbusTlsClient),
         ("tls", lib_client.ModbusTlsClient),
@@ -235,199 +235,134 @@
             cur_args["pos_arg"],
             **arg_list["fix"]["opt_args"],
             **cur_args["opt_args"],
         )
         to_test = dict(arg_list["fix"]["opt_args"], **cur_args["opt_args"])
         to_test["host"] = cur_args["defaults"]["host"]
 
-    for arg, arg_test in to_test.items():
-        assert getattr(client.params, arg) == arg_test
-
     # Test information methods
     client.last_frame_end = 2
     client.silent_interval = 2
     assert client.idle_time() == 4
     client.last_frame_end = None
     assert not client.idle_time()
 
-    initial_delay = client.delay_ms
-    assert initial_delay > 0
-    client.delay_ms *= 2
-
-    assert client.delay_ms > initial_delay
-    client.reset_delay()
-    assert client.delay_ms == initial_delay
-
     rc1 = client._get_address_family("127.0.0.1")  # pylint: disable=protected-access
-    assert socket.AF_INET == rc1
+    assert rc1 == socket.AF_INET
     rc2 = client._get_address_family("::1")  # pylint: disable=protected-access
-    assert socket.AF_INET6 == rc2
+    assert rc2 == socket.AF_INET6
 
     # a successful execute
     client.connect = lambda: True
-    client._connected = True  # pylint: disable=protected-access
+    client.transport = lambda: None
     client.transaction = mock.Mock(**{"execute.return_value": True})
 
     # a unsuccessful connect
     client.connect = lambda: False
-    client._connected = False  # pylint: disable=protected-access
+    client.transport = None
     with pytest.raises(ConnectionException):
         client.execute()
 
 
-def test_client_modbusbaseclient():
+async def test_client_modbusbaseclient():
     """Test modbus base client class."""
     client = ModbusBaseClient(framer=ModbusAsciiFramer)
     client.register(pdu_bit_read.ReadCoilsResponse)
     buffer = "123ABC"
     assert client.send(buffer) == buffer
     assert client.recv(10) == 10
 
-    with pytest.raises(NotImplementedException):
-        client.connect()
-    with pytest.raises(NotImplementedException):
-        client.is_socket_open()
-    with pytest.raises(NotImplementedException):
-        client.close()
-
     with mock.patch(
         "pymodbus.client.base.ModbusBaseClient.connect"
     ) as p_connect, mock.patch(
         "pymodbus.client.base.ModbusBaseClient.close"
     ) as p_close:
-
         p_connect.return_value = True
         p_close.return_value = True
         with ModbusBaseClient(framer=ModbusAsciiFramer) as b_client:
             str(b_client)
         p_connect.return_value = False
 
 
-async def test_client_made_connection():
+async def test_client_connection_made():
     """Test protocol made connection."""
     client = lib_client.AsyncModbusTcpClient("127.0.0.1")
     assert not client.connected
-    client.client_made_connection(mock.sentinel.PROTOCOL)
+    client.connection_made(mock.sentinel.PROTOCOL)
     assert client.connected
 
-    client.client_made_connection(mock.sentinel.PROTOCOL_UNEXPECTED)
+    client.connection_made(mock.sentinel.PROTOCOL_UNEXPECTED)
     assert client.connected
 
 
-async def test_client_lost_connection():
+async def test_client_connection_lost():
     """Test protocol lost connection."""
     client = lib_client.AsyncModbusTcpClient("127.0.0.1")
     assert not client.connected
 
     # fake client is connected and *then* looses connection:
-    client.connected = True
     client.params.host = mock.sentinel.HOST
     client.params.port = mock.sentinel.PORT
-    with mock.patch(
-        "pymodbus.client.tcp.AsyncModbusTcpClient._launch_reconnect"
-    ) as mock_reconnect:
-        mock_reconnect.return_value = mock.sentinel.RECONNECT_GENERATOR
-
-        client.client_lost_connection(mock.sentinel.PROTOCOL_UNEXPECTED)
+    client.connection_lost(mock.sentinel.PROTOCOL_UNEXPECTED)
     assert not client.connected
-
-    client.connected = True
-    with mock.patch(
-        "pymodbus.client.tcp.AsyncModbusTcpClient._launch_reconnect"
-    ) as mock_reconnect:
-        mock_reconnect.return_value = mock.sentinel.RECONNECT_GENERATOR
-
-        client.client_lost_connection(mock.sentinel.PROTOCOL)
+    client.connection_lost(mock.sentinel.PROTOCOL)
     assert not client.connected
+    client.close()
 
 
 async def test_client_base_async():
     """Test modbus base client class."""
     with mock.patch(
         "pymodbus.client.base.ModbusBaseClient.connect"
     ) as p_connect, mock.patch(
         "pymodbus.client.base.ModbusBaseClient.close"
     ) as p_close:
-
-        loop = asyncio.get_event_loop()
-        p_connect.return_value = loop.create_future()
+        asyncio.get_event_loop()
+        p_connect.return_value = asyncio.Future()
         p_connect.return_value.set_result(True)
-        p_close.return_value = loop.create_future()
+        p_close.return_value = asyncio.Future()
         p_close.return_value.set_result(True)
         async with ModbusBaseClient(framer=ModbusAsciiFramer) as client:
             str(client)
-        p_connect.return_value = loop.create_future()
+        p_connect.return_value = asyncio.Future()
         p_connect.return_value.set_result(False)
-        p_close.return_value = loop.create_future()
+        p_close.return_value = asyncio.Future()
         p_close.return_value.set_result(False)
 
 
-@pytest.mark.skip
-async def test_client_protocol():
-    """Test base modbus async client."""
-    base = ModbusBaseClient(framer=ModbusSocketFramer)
-    assert base.transport is None
-    assert not base.async_connected
-
-    base.connection_made(mock.sentinel.TRANSPORT)
-    assert base.transport is mock.sentinel.TRANSPORT
-    base.client_made_connection.assert_called_once_with(  # pylint: disable=no-member
-        base
-    )
-    assert not base.client_lost_connection.call_count  # pylint: disable=no-member
-
-    base.connection_lost(mock.sentinel.REASON)
-    assert base.transport is None
-    assert not base.client_made_connection.call_count  # pylint: disable=no-member
-    base.client_lost_connection.assert_called_once_with(  # pylint: disable=no-member
-        base
-    )
-    base.raise_future = mock.MagicMock()
-    request = mock.MagicMock()
-    base.transaction.addTransaction(request, 1)
-    base.connection_lost(mock.sentinel.REASON)
-    base.raise_future.assert_called_once()
-    call_args = base.raise_future.call_args.args
-    assert call_args[0] == request
-    assert isinstance(call_args[1], ConnectionException)
-    base.transport = mock.MagicMock()
-    base.transport = None
-    await base.async_close()
-
-
 async def test_client_protocol_receiver():
     """Test the client protocol data received"""
     base = ModbusBaseClient(framer=ModbusSocketFramer)
     transport = mock.MagicMock()
     base.connection_made(transport)
     assert base.transport == transport
-    assert base.async_connected
+    assert base.transport
     data = b"\x00\x00\x12\x34\x00\x06\xff\x01\x01\x02\x00\x04"
 
     # setup existing request
     assert not list(base.transaction)
     response = base._build_response(0x00)  # pylint: disable=protected-access
     base.data_received(data)
     result = response.result()
     assert isinstance(result, pdu_bit_read.ReadCoilsResponse)
 
-    base._connected = False  # pylint: disable=protected-access
+    base.transport = None
     with pytest.raises(ConnectionException):
         await base._build_response(0x00)  # pylint: disable=protected-access
 
 
 async def test_client_protocol_response():
     """Test the udp client protocol builds responses"""
     base = ModbusBaseClient(framer=ModbusSocketFramer)
     response = base._build_response(0x00)  # pylint: disable=protected-access
     excp = response.exception()
     assert isinstance(excp, ConnectionException)
     assert not list(base.transaction)
 
-    base._connected = True  # pylint: disable=protected-access
+    base.transport = lambda: None
     base._build_response(0x00)  # pylint: disable=protected-access
     assert len(list(base.transaction)) == 1
 
 
 async def test_client_protocol_handler():
     """Test the client protocol handles responses"""
     base = ModbusBaseClient(framer=ModbusSocketFramer)
@@ -439,21 +374,18 @@
     base._handle_response(reply)  # pylint: disable=protected-access
     response = base._build_response(0x00)  # pylint: disable=protected-access
     base._handle_response(reply)  # pylint: disable=protected-access
     result = response.result()
     assert result == reply
 
 
+@pytest.mark.skip()
 async def test_client_protocol_execute():
     """Test the client protocol execute method"""
     base = ModbusBaseClient(host="127.0.0.1", framer=ModbusSocketFramer)
-    base.create_future = mock.MagicMock()
-    fut = asyncio.Future()
-    fut.set_result(fut)
-    base.create_future.return_value = fut
     transport = mock.MagicMock()
     base.connection_made(transport)
     base.transport.write = mock.Mock()
 
     request = pdu_bit_read.ReadCoilsRequest(1, 1)
     response = await base.async_execute(request)
     tid = request.transaction_id
@@ -474,59 +406,82 @@
     base.transport.sendto(bytes("00010000", "utf-8"))
 
 
 def test_client_udp_connect():
     """Test the Udp client connection method"""
     with mock.patch.object(socket, "socket") as mock_method:
 
-        class DummySocket:  # pylint: disable=too-few-public-methods
+        class DummySocket:
             """Dummy socket."""
 
+            fileno = 1
+
             def settimeout(self, *a, **kwa):
                 """Set timeout."""
 
+            def setblocking(self, _flag):
+                """Set blocking"""
+
         mock_method.return_value = DummySocket()
         client = lib_client.ModbusUdpClient("127.0.0.1")
         assert client.connect()
 
     with mock.patch.object(socket, "socket") as mock_method:
-        mock_method.side_effect = socket.error()
+        mock_method.side_effect = OSError()
         client = lib_client.ModbusUdpClient("127.0.0.1")
         assert not client.connect()
 
 
 def test_client_tcp_connect():
     """Test the tcp client connection method"""
     with mock.patch.object(socket, "create_connection") as mock_method:
         _socket = mock.MagicMock()
         mock_method.return_value = _socket
         client = lib_client.ModbusTcpClient("127.0.0.1")
         _socket.getsockname.return_value = ("dmmy", 1234)
         assert client.connect()
 
     with mock.patch.object(socket, "create_connection") as mock_method:
-        mock_method.side_effect = socket.error()
+        mock_method.side_effect = OSError()
         client = lib_client.ModbusTcpClient("127.0.0.1")
         assert not client.connect()
 
 
+def test_client_tcp_reuse():
+    """Test the tcp client connection method"""
+    with mock.patch.object(socket, "create_connection") as mock_method:
+        _socket = mock.MagicMock()
+        mock_method.return_value = _socket
+        client = lib_client.ModbusTcpClient("127.0.0.1")
+        _socket.getsockname.return_value = ("dmmy", 1234)
+        assert client.connect()
+    client.close()
+    with mock.patch.object(socket, "create_connection") as mock_method:
+        _socket = mock.MagicMock()
+        mock_method.return_value = _socket
+        client = lib_client.ModbusTcpClient("127.0.0.1")
+        _socket.getsockname.return_value = ("dmmy", 1234)
+        assert client.connect()
+    client.close()
+
+
 def test_client_tls_connect():
     """Test the tls client connection method"""
     with mock.patch.object(ssl.SSLSocket, "connect") as mock_method:
         client = lib_client.ModbusTlsClient("127.0.0.1")
         assert client.connect()
 
     with mock.patch.object(socket, "create_connection") as mock_method:
-        mock_method.side_effect = socket.error()
+        mock_method.side_effect = OSError()
         client = lib_client.ModbusTlsClient("127.0.0.1")
         assert not client.connect()
 
 
 @pytest.mark.parametrize(
-    "datatype,value,registers",
+    ("datatype", "value", "registers"),
     [
         (ModbusClientMixin.DATATYPE.STRING, "abcd", [0x6162, 0x6364]),
         (ModbusClientMixin.DATATYPE.STRING, "a", [0x6100]),
         (ModbusClientMixin.DATATYPE.UINT16, 27123, [0x69F3]),
         (ModbusClientMixin.DATATYPE.INT16, -27123, [0x960D]),
         (ModbusClientMixin.DATATYPE.UINT32, 27123, [0x0000, 0x69F3]),
         (ModbusClientMixin.DATATYPE.UINT32, 32145678, [0x01EA, 0x810E]),
```

### Comparing `pymodbus-3.2.2/test/test_client_sync.py` & `pymodbus-3.3.0/test/test_client_sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,18 +71,31 @@
 
     def test_udp_client_recv(self):
         """Test the udp client receive method"""
         client = ModbusUdpClient("127.0.0.1")
         with pytest.raises(ConnectionException):
             client.recv(1024)
         client.socket = mockSocket()
-        client.socket.mock_store(b"\x00" * 4)
+        client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(0) == b""
         assert client.recv(4) == b"\x00" * 4
 
+    def test_udp_client_recv_duplicate(self):
+        """Test the udp client receive method"""
+        test_msg = b"\x00\x01\x00\x00\x00\x05\x01\x04\x02\x00\x03"
+        client = ModbusUdpClient("127.0.0.1")
+        client.socket = mockSocket(copy_send=False)
+        client.socket.mock_prepare_receive(test_msg)
+        client.socket.mock_prepare_receive(test_msg)
+        reply_ok = client.read_input_registers(0x820, 1, 1)
+        assert not reply_ok.isError()
+        reply_none = client.read_input_registers(0x40, 10, 1)
+        assert reply_none.isError()
+        client.close()
+
     def test_udp_client_repr(self):
         """Test udp client representation."""
         client = ModbusUdpClient("127.0.0.1")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
             f"ipaddr={client.params.host}, port={client.params.port}, timeout={client.params.timeout}>"
         )
@@ -139,28 +152,28 @@
         mock_select.select.return_value = [True]
         mock_time.time.side_effect = count()
         client = ModbusTcpClient("127.0.0.1")
         with pytest.raises(ConnectionException):
             client.recv(1024)
         client.socket = mockSocket()
         assert client.recv(0) == b""
-        client.socket.mock_store(b"\x00" * 4)
+        client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(4) == b"\x00" * 4
 
         mock_socket = mock.MagicMock()
         mock_socket.recv.side_effect = iter([b"\x00", b"\x01", b"\x02"])
         client.socket = mock_socket
         client.params.timeout = 3
         assert client.recv(3) == b"\x00\x01\x02"
         mock_socket.recv.side_effect = iter([b"\x00", b"\x01", b"\x02"])
         assert client.recv(2) == b"\x00\x01"
         mock_select.select.return_value = [False]
         assert client.recv(2) == b""
         client.socket = mockSocket()
-        client.socket.mock_store(b"\x00")
+        client.socket.mock_prepare_receive(b"\x00")
         mock_select.select.return_value = [True]
         assert client.recv(None) in b"\x00"
 
         mock_socket = mock.MagicMock()
         mock_socket.recv.return_value = b""
         client.socket = mock_socket
         with pytest.raises(ConnectionException):
@@ -267,20 +280,20 @@
         mock_select.select.return_value = [True]
         client = ModbusTlsClient("127.0.0.1")
         with pytest.raises(ConnectionException):
             client.recv(1024)
         mock_time.time.side_effect = count()
 
         client.socket = mockSocket()
-        client.socket.mock_store(b"\x00" * 4)
+        client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(0) == b""
         assert client.recv(4) == b"\x00" * 4
 
         client.params.timeout = 2
-        client.socket.mock_store(b"\x00")
+        client.socket.mock_prepare_receive(b"\x00")
         assert b"\x00" in client.recv(None)
 
     def test_tls_client_repr(self):
         """Test tls client."""
         client = ModbusTlsClient("127.0.0.1")
         rep = (
             f"<{client.__class__.__name__} at {hex(id(client))} socket={client.socket}, "
@@ -418,18 +431,18 @@
     def test_serial_client_recv(self):
         """Test the serial client receive method"""
         client = ModbusSerialClient("/dev/null")
         with pytest.raises(ConnectionException):
             client.recv(1024)
         client.socket = mockSocket()
         assert client.recv(0) == b""
-        client.socket.mock_store(b"\x00" * 4)
+        client.socket.mock_prepare_receive(b"\x00" * 4)
         assert client.recv(4) == b"\x00" * 4
         client.socket = mockSocket()
-        client.socket.mock_store(b"")
+        client.socket.mock_prepare_receive(b"")
         assert client.recv(None) == b""
         client.socket.timeout = 0
         assert client.recv(0) == b""
 
     def test_serial_client_repr(self):
         """Test serial client."""
         client = ModbusSerialClient("/dev/null")
```

### Comparing `pymodbus-3.2.2/test/test_device.py` & `pymodbus-3.3.0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_diag_messages.py` & `pymodbus-3.3.0/test/test_diag_messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,20 +115,31 @@
         (ReturnSlaveBusyCountResponse, b"\x00\x11\x00\x00"),
         (ReturnSlaveBusCharacterOverrunCountResponse, b"\x00\x12\x00\x00"),
         (ReturnIopOverrunCountResponse, b"\x00\x13\x00\x00"),
         (ClearOverrunCountResponse, b"\x00\x14\x00\x00"),
         (GetClearModbusPlusResponse, b"\x00\x15\x00\x04" + b"\x00\x00" * 55),
     ]
 
+    def test_diagnostic_encode_decode(self):
+        """Testing diagnostic request/response can be decoded and encoded."""
+        for msg in (DiagnosticStatusRequest, DiagnosticStatusResponse):
+            msg_obj = msg()
+            data = b"\x00\x01\x02\x03"
+            msg_obj.decode(data)
+            result = msg_obj.encode()
+            assert data == result
+
     def test_diagnostic_requests_decode(self):
         """Testing diagnostic request messages encoding"""
         for msg, enc, _ in self.requests:
             handle = DiagnosticStatusRequest()
             handle.decode(enc)
             assert handle.sub_function_code == msg.sub_function_code
+            encoded = handle.encode()
+            assert enc == encoded
 
     def test_diagnostic_simple_requests(self):
         """Testing diagnostic request messages encoding"""
         request = DiagnosticStatusSimpleRequest(b"\x12\x34")
         request.sub_function_code = 0x1234
         with pytest.raises(NotImplementedException):
             request.execute()
```

### Comparing `pymodbus-3.2.2/test/test_events.py` & `pymodbus-3.3.0/test/test_events.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_example_client_server.py` & `pymodbus-3.3.0/test/test_example_client_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """Test helper get_commandline()"""
     args = get_commandline(cmdline=["--log", "info"])
     assert args.log == "info"
     assert args.host == "127.0.0.1"
 
 
 @pytest.mark.xdist_group(name="server_serialize")
-@pytest.mark.parametrize("test_comm, test_framer, test_port", TEST_COMMS_FRAMER)
+@pytest.mark.parametrize(("test_comm", "test_framer", "test_port"), TEST_COMMS_FRAMER)
 async def test_exp_async_server_client(
     test_comm,
     test_framer,
     test_port,
     mock_run_server,
 ):
     """Run async client and server."""
@@ -98,15 +98,17 @@
         "debug",
     ]
     test_client = setup_async_client(cmdline=cmdline)
     await run_async_client(test_client, modbus_calls=run_async_simple_calls)
 
 
 @pytest.mark.xdist_group(name="server_serialize")
-@pytest.mark.parametrize("test_comm, test_framer, test_port", [TEST_COMMS_FRAMER[0]])
+@pytest.mark.parametrize(
+    ("test_comm", "test_framer", "test_port"), [TEST_COMMS_FRAMER[0]]
+)
 def test_exp_sync_server_client(
     test_comm,
     test_framer,
     test_port,
 ):
     """Run sync client and server."""
     cmdline = [
```

### Comparing `pymodbus-3.2.2/test/test_examples.py` & `pymodbus-3.3.0/test/test_examples.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_exceptions.py` & `pymodbus-3.3.0/test/test_exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,13 +20,9 @@
         NotImplementedException("bad function"),
         ConnectionException("bad connection"),
     ]
 
     def test_exceptions(self):
         """Test all module exceptions"""
         for exc in self.exceptions:
-            try:
+            with pytest.raises(ModbusException, match="Modbus Error:"):
                 raise exc
-            except ModbusException as exc:
-                assert "Modbus Error:" in str(exc)
-                return
-            pytest.fail("Excepted a ModbusExceptions")
```

### Comparing `pymodbus-3.2.2/test/test_factory.py` & `pymodbus-3.3.0/test/test_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     bad = (
         (0x80, b"\x80\x00\x00\x00"),  # Unknown Function
         (0x81, b"\x81\x00\x00\x00"),  # error message
     )
 
     @pytest.fixture(autouse=True)
-    def setup(self):
+    def _setup(self):
         """Do common setup function."""
         self.client = ClientDecoder()
         self.server = ServerDecoder()
 
     def test_exception_lookup(self):
         """Test that we can look up exception messages"""
         for func, _ in self.exception:
@@ -117,28 +117,28 @@
         """Test a working request factory lookup"""
         for func, _ in self.request:
             request = self.client.lookupPduClass(func)
             assert request
 
     def test_response_working(self):
         """Test a working response factory decoders"""
-        for func, msg in self.response:
+        for _func, msg in self.response:
             self.client.decode(msg)
 
     def test_response_errors(self):
         """Test a response factory decoder exceptions"""
         with pytest.raises(ModbusException):
             self.client._helper(self.bad[0][1])  # pylint: disable=protected-access
         assert (
             self.client.decode(self.bad[1][1]).function_code == self.bad[1][0]
         ), "Failed to decode error PDU"
 
     def test_requests_working(self):
         """Test a working request factory decoders"""
-        for func, msg in self.request:
+        for _func, msg in self.request:
             self.server.decode(msg)
 
     def test_client_factory_fails(self):
         """Tests that a client factory will fail to decode a bad message"""
         self.client._helper = _raise_exception  # pylint: disable=protected-access
         actual = self.client.decode(None)
         assert not actual
```

### Comparing `pymodbus-3.2.2/test/test_file_message.py` & `pymodbus-3.3.0/test/test_file_message.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_framers.py` & `pymodbus-3.3.0/test/test_framers.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 from pymodbus.framer.rtu_framer import ModbusRtuFramer
 from pymodbus.utilities import ModbusTransactionState
 
 
 TEST_MESSAGE = b"\x00\x01\x00\x01\x00\n\xec\x1c"
 
 
-@pytest.fixture
-def rtu_framer():
+@pytest.fixture(name="rtu_framer")
+def fixture_rtu_framer():
     """RTU framer."""
     return ModbusRtuFramer(ClientDecoder())
 
 
-@pytest.fixture
-def ascii_framer():
+@pytest.fixture(name="ascii_framer")
+def fixture_ascii_framer():
     """Ascii framer."""
     return ModbusAsciiFramer(ClientDecoder())
 
 
 # @pytest.fixture
 # def binary_framer():
 #     """Binary framer."""
@@ -79,15 +79,15 @@
         assert framer._repeat == [  # pylint: disable=protected-access
             b"}"[0],
             b"{"[0],
         ]
 
 
 @pytest.mark.parametrize("data", [(b"", {}), (b"abcd", {"fcode": 98, "slave": 97})])
-def test_decode_data(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_decode_data(rtu_framer, data):
     """Test decode data."""
     data, expected = data
     decoded = rtu_framer.decode_data(data)
     assert decoded == expected
 
 
 @pytest.mark.parametrize(
@@ -95,15 +95,15 @@
     [
         (b"", False),
         (b"\x02\x01\x01\x00Q\xcc", True),
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD", True),  # valid frame
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAC", False),  # invalid frame CRC
     ],
 )
-def test_check_frame(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_check_frame(rtu_framer, data):
     """Test check frame."""
     data, expected = data
     rtu_framer._buffer = data  # pylint: disable=protected-access
     assert expected == rtu_framer.checkFrame()
 
 
 @pytest.mark.parametrize(
@@ -114,15 +114,15 @@
         (
             b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD\x12\x03",  # real case, frame size is 11
             {"uid": 0x00, "len": 11, "crc": b"\x00\x00"},
             b"\x12\x03",
         ),
     ],
 )
-def test_rtu_advance_framer(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_rtu_advance_framer(rtu_framer, data):
     """Test rtu advance framer."""
     before_buf, before_header, after_buf = data
 
     rtu_framer._buffer = before_buf  # pylint: disable=protected-access
     rtu_framer._header = before_header  # pylint: disable=protected-access
     rtu_framer.advanceFrame()
     assert rtu_framer._header == {  # pylint: disable=protected-access
@@ -130,39 +130,38 @@
         "len": 0,
         "crc": b"\x00\x00",
     }
     assert rtu_framer._buffer == after_buf  # pylint: disable=protected-access
 
 
 @pytest.mark.parametrize("data", [b"", b"abcd"])
-def test_rtu_reset_framer(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_rtu_reset_framer(rtu_framer, data):
     """Test rtu reset framer."""
     rtu_framer._buffer = data  # pylint: disable=protected-access
     rtu_framer.resetFrame()
     assert rtu_framer._header == {  # pylint: disable=protected-access
         "uid": 0x00,
         "len": 0,
         "crc": b"\x00\x00",
     }
-    assert rtu_framer._buffer == b""  # pylint: disable=protected-access
 
 
 @pytest.mark.parametrize(
     "data",
     [
         (b"", False),
         (b"\x11", False),
         (b"\x11\x03", False),
         (b"\x11\x03\x06", False),
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49", False),
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD", True),
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD\xAB\xCD", True),
     ],
 )
-def test_is_frame_ready(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_is_frame_ready(rtu_framer, data):
     """Test is frame ready."""
     data, expected = data
     rtu_framer._buffer = data  # pylint: disable=protected-access
     # rtu_framer.advanceFrame()
     assert rtu_framer.isFrameReady() == expected
 
 
@@ -172,17 +171,15 @@
         b"",
         b"\x11",
         b"\x11\x03",
         b"\x11\x03\x06",
         b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x43",
     ],
 )
-def test_rtu_populate_header_fail(
-    rtu_framer, data
-):  # pylint: disable=redefined-outer-name
+def test_rtu_populate_header_fail(rtu_framer, data):
     """Test rtu populate header fail."""
     with pytest.raises(IndexError):
         rtu_framer.populateHeader(data)
 
 
 @pytest.mark.parametrize(
     "data",
@@ -193,36 +190,36 @@
         ),
         (
             b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD\x11\x03",
             {"crc": b"\x49\xAD", "uid": 17, "len": 11},
         ),
     ],
 )
-def test_rtu_populate_header(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_rtu_populate_header(rtu_framer, data):
     """Test rtu populate header."""
     buffer, expected = data
     rtu_framer.populateHeader(buffer)
     assert rtu_framer._header == expected  # pylint: disable=protected-access
 
 
-def test_add_to_frame(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_add_to_frame(rtu_framer):
     """Test add to frame."""
     assert rtu_framer._buffer == b""  # pylint: disable=protected-access
     rtu_framer.addToFrame(b"abcd")
     assert rtu_framer._buffer == b"abcd"  # pylint: disable=protected-access
 
 
-def test_get_frame(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_get_frame(rtu_framer):
     """Test get frame."""
     rtu_framer.addToFrame(b"\x02\x01\x01\x00Q\xcc")
     rtu_framer.populateHeader(b"\x02\x01\x01\x00Q\xcc")
     assert rtu_framer.getFrame() == b"\x01\x01\x00"
 
 
-def test_populate_result(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_populate_result(rtu_framer):
     """Test populate result."""
     rtu_framer._header["uid"] = 255  # pylint: disable=protected-access
     result = mock.Mock()
     rtu_framer.populateResult(result)
     assert result.slave_id == 255
 
 
@@ -251,22 +248,22 @@
             17,
             False,
             True,
         ),  # good frame
         (
             b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD",
             16,
-            True,
+            False,
             False,
         ),  # incorrect slave id
         (b"\x11\x03\x06\xAE\x41\x56\x52\x43\x40\x49\xAD\x11\x03", 17, False, True),
         # good frame + part of next frame
     ],
 )
-def test_rtu_incoming_packet(rtu_framer, data):  # pylint: disable=redefined-outer-name
+def test_rtu_incoming_packet(rtu_framer, data):
     """Test rtu process incoming packet."""
     buffer, slaves, reset_called, process_called = data
 
     with mock.patch.object(
         rtu_framer,
         "_process",
         wraps=rtu_framer._process,  # pylint: disable=protected-access
@@ -274,21 +271,21 @@
         rtu_framer, "resetFrame", wraps=rtu_framer.resetFrame
     ) as mock_reset:
         rtu_framer.processIncomingPacket(buffer, mock.Mock(), slaves)
         assert mock_process.call_count == (1 if process_called else 0)
         assert mock_reset.call_count == (1 if reset_called else 0)
 
 
-def test_build_packet(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_build_packet(rtu_framer):
     """Test build packet."""
     message = ReadCoilsRequest(1, 10)
     assert rtu_framer.buildPacket(message) == TEST_MESSAGE
 
 
-def test_send_packet(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_send_packet(rtu_framer):
     """Test send packet."""
     message = TEST_MESSAGE
     client = ModbusBaseClient(framer=ModbusRtuFramer)
     client.state = ModbusTransactionState.TRANSACTION_COMPLETE
     client.silent_interval = 1
     client.last_frame_end = 1
     client.params.timeout = 0.25
@@ -296,49 +293,49 @@
     client.send = mock.Mock(return_value=len(message))
     rtu_framer.client = client
     assert rtu_framer.sendPacket(message) == len(message)
     client.state = ModbusTransactionState.PROCESSING_REPLY
     assert rtu_framer.sendPacket(message) == len(message)
 
 
-def test_recv_packet(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_recv_packet(rtu_framer):
     """Test receive packet."""
     message = TEST_MESSAGE
     client = mock.Mock()
     client.recv.return_value = message
     rtu_framer.client = client
     assert rtu_framer.recvPacket(len(message)) == message
 
 
-def test_process(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_process(rtu_framer):
     """Test process."""
 
     rtu_framer._buffer = TEST_MESSAGE  # pylint: disable=protected-access
     with pytest.raises(ModbusIOException):
         rtu_framer._process(None)  # pylint: disable=protected-access
 
 
-def test_get_raw_frame(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_get_raw_frame(rtu_framer):
     """Test get raw frame."""
     rtu_framer._buffer = TEST_MESSAGE  # pylint: disable=protected-access
     assert (
         rtu_framer.getRawFrame()
         == rtu_framer._buffer  # pylint: disable=protected-access
     )
 
 
-def test_validate__slave_id(rtu_framer):  # pylint: disable=redefined-outer-name
+def test_validate__slave_id(rtu_framer):
     """Test validate slave."""
     rtu_framer.populateHeader(TEST_MESSAGE)
     assert rtu_framer._validate_slave_id([0], False)  # pylint: disable=protected-access
     assert rtu_framer._validate_slave_id([1], True)  # pylint: disable=protected-access
 
 
 @pytest.mark.parametrize("data", [b":010100010001FC\r\n", b""])
-def test_decode_ascii_data(ascii_framer, data):  # pylint: disable=redefined-outer-name
+def test_decode_ascii_data(ascii_framer, data):
     """Test decode ascii."""
     data = ascii_framer.decode_data(data)
     assert isinstance(data, dict)
     if data:
         assert data.get("slave") == 1
         assert data.get("fcode") == 1
     else:
```

### Comparing `pymodbus-3.2.2/test/test_logging.py` & `pymodbus-3.3.0/test/test_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def test_log_simple(self):
         """Test simple string"""
         txt = "simple string"
         log_txt = Log.build_msg(txt)
         assert log_txt == txt
 
     @pytest.mark.parametrize(
-        "txt, result, params",
+        ("txt", "result", "params"),
         [
             ("string {} {} {}", "string 101 102 103", (101, 102, 103)),
             ("string {}", "string 0x41 0x42 0x43 0x44", (b"ABCD", ":hex")),
             ("string {}", "string 125", (125, ":str")),
         ],
     )
     def test_log_parms(self, txt, result, params):
```

### Comparing `pymodbus-3.2.2/test/test_mei_messages.py` & `pymodbus-3.3.0/test/test_mei_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_other_messages.py` & `pymodbus-3.3.0/test/test_other_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_payload.py` & `pymodbus-3.3.0/test/test_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         builder.add_8bit_int(-1)
         builder.add_16bit_int(-2)
         builder.add_32bit_int(-3)
         builder.add_64bit_int(-4)
         builder.add_32bit_float(1.25)
         builder.add_64bit_float(6.25)
         builder.add_16bit_uint(1)  # placeholder
-        builder.add_string(b"test")
+        builder.add_string("test")
         builder.add_bits(self.bitstring)
-        assert self.little_endian_payload == builder.to_string()
+        assert self.little_endian_payload == builder.encode()
 
     def test_big_endian_payload_builder(self):
         """Test basic bit message encoding/decoding"""
         builder = BinaryPayloadBuilder(byteorder=Endian.Big)
         builder.add_8bit_uint(1)
         builder.add_16bit_uint(2)
         builder.add_32bit_uint(3)
@@ -73,27 +73,27 @@
         builder.add_32bit_int(-3)
         builder.add_64bit_int(-4)
         builder.add_32bit_float(1.25)
         builder.add_64bit_float(6.25)
         builder.add_16bit_uint(1)  # placeholder
         builder.add_string("test")
         builder.add_bits(self.bitstring)
-        assert self.big_endian_payload == builder.to_string()
+        assert self.big_endian_payload == builder.encode()
 
     def test_payload_builder_reset(self):
         """Test basic bit message encoding/decoding"""
         builder = BinaryPayloadBuilder()
         builder.add_8bit_uint(0x12)
         builder.add_8bit_uint(0x34)
         builder.add_8bit_uint(0x56)
         builder.add_8bit_uint(0x78)
-        assert builder.to_string() == b"\x12\x34\x56\x78"
+        assert builder.encode() == b"\x12\x34\x56\x78"
         assert builder.build() == [b"\x12\x34", b"\x56\x78"]
         builder.reset()
-        assert not builder.to_string()
+        assert not builder.encode()
         assert not builder.build()
 
     def test_payload_builder_with_raw_payload(self):
         """Test basic bit message encoding/decoding"""
         _coils1 = [
             False,
             False,
@@ -162,23 +162,23 @@
             False,
             False,
         ]
 
         builder = BinaryPayloadBuilder(
             [b"\x12", b"\x34", b"\x56", b"\x78"], repack=True
         )
-        assert builder.to_string() == b"\x12\x34\x56\x78"
+        assert builder.encode() == b"\x12\x34\x56\x78"
         assert builder.to_registers() == [13330, 30806]
         coils = builder.to_coils()
         assert _coils1 == coils
 
         builder = BinaryPayloadBuilder(
             [b"\x12", b"\x34", b"\x56", b"\x78"], byteorder=Endian.Big
         )
-        assert builder.to_string() == b"\x12\x34\x56\x78"
+        assert builder.encode() == b"\x12\x34\x56\x78"
         assert builder.to_registers() == [4660, 22136]
         assert str(builder) == "\x12\x34\x56\x78"
         coils = builder.to_coils()
         assert _coils2 == coils
 
     # ----------------------------------------------------------------------- #
     # Payload Decoder Tests
```

### Comparing `pymodbus-3.2.2/test/test_pdu.py` & `pymodbus-3.3.0/test/test_pdu.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_register_read_messages.py` & `pymodbus-3.3.0/test/test_register_read_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_register_write_messages.py` & `pymodbus-3.3.0/test/test_register_write_messages.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_remote_datastore.py` & `pymodbus-3.3.0/test/test_remote_datastore.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_repl_client.py` & `pymodbus-3.3.0/test/test_repl_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Test client sync."""
+from contextlib import suppress
+
 from pymodbus.repl.client.main import _process_args
 from pymodbus.server.reactive.default_config import DEFAULT_CONFIG
 
 
 def test_repl_default_config():
     """Test default config can be loaded."""
     config = DEFAULT_CONFIG
@@ -28,21 +30,15 @@
 
     resp = _process_args(["value=11", "address=0x10"], False)
     assert resp == ({"address": 16, "value": 11}, True)
 
     resp = _process_args(["address=0b11", "value=0x10"], False)
     assert resp == ({"address": 3, "value": 16}, True)
 
-    try:
+    with suppress(ValueError):
         resp = _process_args(["address=0xhj", "value=0x10"], False)
-    except ValueError:
-        pass
 
-    try:
+    with suppress(ValueError):
         resp = _process_args(["address=11ah", "value=0x10"], False)
-    except ValueError:
-        pass
 
-    try:
+    with suppress(ValueError):
         resp = _process_args(["address=0b12", "value=0x10"], False)
-    except ValueError:
-        pass
```

### Comparing `pymodbus-3.2.2/test/test_server_asyncio.py` & `pymodbus-3.3.0/test/test_server_asyncio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test server asyncio."""
 import asyncio
 import logging
 import ssl
 from asyncio import CancelledError
+from contextlib import suppress
 from unittest import mock
 
 import pytest
 
 from pymodbus.datastore import (
     ModbusSequentialDataBlock,
     ModbusServerContext,
@@ -100,15 +101,15 @@
     task = None
     loop = None
     store = None
     context = None
     identity = None
 
     @pytest.fixture(autouse=True)
-    async def setup_teardown(self):
+    async def _setup_teardown(self):
         """Initialize the test environment by setting up a dummy store and context."""
         self.loop = asyncio.get_running_loop()
         self.store = ModbusSlaveContext(
             di=ModbusSequentialDataBlock(0, [17] * 100),
             co=ModbusSequentialDataBlock(0, [17] * 100),
             hr=ModbusSequentialDataBlock(0, [17] * 100),
             ir=ModbusSequentialDataBlock(0, [17] * 100),
@@ -123,36 +124,31 @@
         if self.server is not None:
             await self.server.server_close()
             self.server = None
         if self.task is not None:
             await asyncio.sleep(0.1)
             if not self.task.cancelled():
                 self.task.cancel()
-                try:
+                with suppress(CancelledError):
                     await self.task
-                except CancelledError:
-                    pass
                 self.task = None
         BasicClient.clear()
 
     def handle_task(self, result):
         """Handle task exit."""
-        try:
+        with suppress(CancelledError):
             result = result.result()
-        except CancelledError:
-            pass
 
     async def start_server(
-        self, do_forever=True, do_defer=True, do_tls=False, do_udp=False, do_ident=False
+        self, do_forever=True, do_tls=False, do_udp=False, do_ident=False
     ):
         """Handle setup and control of tcp server."""
         args = {
             "context": self.context,
             "address": SERV_ADDR,
-            "defer_start": do_defer,
         }
         if do_ident:
             args["identity"] = self.identity
         if do_tls:
             self.server = ModbusTlsServer(
                 self.context, ModbusTlsFramer, self.identity, SERV_ADDR
             )
@@ -175,17 +171,17 @@
         elif not do_udp:  # pylint: disable=confusing-consecutive-elif
             assert not self.server.server
         assert self.server.control.Identity.VendorName == "VendorName"
         await asyncio.sleep(0.1)
 
     async def connect_server(self):
         """Handle connect to server"""
-        BasicClient.connected = self.loop.create_future()
-        BasicClient.done = self.loop.create_future()
-        BasicClient.eof = self.loop.create_future()
+        BasicClient.connected = asyncio.Future()
+        BasicClient.done = asyncio.Future()
+        BasicClient.eof = asyncio.Future()
         random_port = self.server.server.sockets[0].getsockname()[
             1
         ]  # get the random server port
         (
             BasicClient.transport,
             BasicClient.my_protocol,
         ) = await self.loop.create_connection(
@@ -293,19 +289,18 @@
             assert self.server.control.Identity.VendorName == "VendorName"
             assert self.server.sslctx
 
     async def test_async_tls_server_serve_forever(self):
         """Test StartAsyncTcpServer serve_forever() method"""
         with mock.patch(
             "asyncio.base_events.Server.serve_forever", new_callable=mock.AsyncMock
-        ) as serve:
-            with mock.patch.object(ssl.SSLContext, "load_cert_chain"):
-                await self.start_server(do_tls=True, do_forever=False)
-                await self.server.serve_forever()
-                serve.assert_awaited()
+        ) as serve, mock.patch.object(ssl.SSLContext, "load_cert_chain"):
+            await self.start_server(do_tls=True, do_forever=False)
+            await self.server.serve_forever()
+            serve.assert_awaited()
 
     async def test_async_tls_server_serve_forever_twice(self):
         """Call on serve_forever() twice should result in a runtime error"""
         with mock.patch.object(ssl.SSLContext, "load_cert_chain"):
             await self.start_server(do_tls=True)
             with pytest.raises(RuntimeError):
                 await self.server.serve_forever()
@@ -382,31 +377,31 @@
         await self.server.server_close()
         self.server = None
 
     async def test_async_udp_server_roundtrip(self):
         """Test sending and receiving data on udp socket"""
         expected_response = b"\x01\x00\x00\x00\x00\x05\x01\x03\x02\x00\x11"  # value of 17 as per context
         BasicClient.dataTo = TEST_DATA  # slave 1, read register
-        BasicClient.done = self.loop.create_future()
+        BasicClient.done = asyncio.Future()
         await self.start_server(do_udp=True)
         random_port = self.server.protocol._sock.getsockname()[  # pylint: disable=protected-access
             1
         ]
         transport, _ = await self.loop.create_datagram_endpoint(
             BasicClient, remote_addr=("127.0.0.1", random_port)
         )
         await asyncio.wait_for(BasicClient.done, timeout=0.1)
         assert BasicClient.received_data == expected_response
         transport.close()
 
     async def test_async_udp_server_exception(self):
         """Test sending garbage data on a TCP socket should drop the connection"""
         BasicClient.dataTo = b"\xFF\xFF\xFF\xFF\xFF\xFF\xFF\xFF"
-        BasicClient.connected = self.loop.create_future()
-        BasicClient.done = self.loop.create_future()
+        BasicClient.connected = asyncio.Future()
+        BasicClient.done = asyncio.Future()
         await self.start_server(do_udp=True)
         with mock.patch(
             "pymodbus.transaction.ModbusSocketFramer.processIncomingPacket",
             new_callable=lambda: mock.Mock(side_effect=Exception),
         ):
             # get the random server port pylint: disable=protected-access
             random_port = self.server.protocol._sock.getsockname()[1]
```

### Comparing `pymodbus-3.2.2/test/test_server_context.py` & `pymodbus-3.3.0/test/test_server_context.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_server_task.py` & `pymodbus-3.3.0/test/test_server_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -140,107 +140,139 @@
     return cur_m["srv"], cur["srv_args"], cur_m["cli"], cur["cli_args"]
 
 
 @pytest.mark.xdist_group(name="server_serialize")
 @pytest.mark.parametrize("comm", TEST_TYPES)
 async def test_async_task_no_server(comm):
     """Test normal client/server handling."""
-    run_server, server_args, run_client, client_args = helper_config(comm, "async")
+    _run_server, _server_args, run_client, client_args = helper_config(comm, "async")
     client = run_client(**client_args)
     try:
         await client.connect()
-    except Exception as exc:  # pylint: disable=broad-except
-        assert False, f"unexpected exception: {exc}"
+    except Exception as exc:
+        raise AssertionError(f"unexpected exception: {exc}") from exc
     await asyncio.sleep(0.1)
     with pytest.raises((asyncio.exceptions.TimeoutError, ConnectionException)):
         await client.read_coils(1, 1, slave=0x01)
-    await client.close()
+    client.close()
 
 
 @pytest.mark.xdist_group(name="server_serialize")
 @pytest.mark.parametrize("comm", TEST_TYPES)
 async def test_async_task_ok(comm):
     """Test normal client/server handling."""
     run_server, server_args, run_client, client_args = helper_config(comm, "async")
 
     task = asyncio.create_task(run_server(**server_args))
     await asyncio.sleep(0.1)
     client = run_client(**client_args)
     await client.connect()
     await asyncio.sleep(0.1)
-    assert client._connected  # pylint: disable=protected-access
+    assert client.transport
     rr = await client.read_coils(1, 1, slave=0x01)
     assert len(rr.bits) == 8
 
-    await client.close()
+    client.close()
     await asyncio.sleep(0.1)
-    assert not client._connected  # pylint: disable=protected-access
+    assert not client.transport
     await server.ServerAsyncStop()
     task.cancel()
     await task
 
 
 @pytest.mark.xdist_group(name="server_serialize")
 @pytest.mark.parametrize("comm", TEST_TYPES)
-async def test_async_task_server_stop(comm):
+async def test_async_task_reuse(comm):
     """Test normal client/server handling."""
     run_server, server_args, run_client, client_args = helper_config(comm, "async")
+
     task = asyncio.create_task(run_server(**server_args))
     await asyncio.sleep(0.1)
+    client = run_client(**client_args)
+    await client.connect()
+    await asyncio.sleep(0.1)
+    assert client.transport
+    rr = await client.read_coils(1, 1, slave=0x01)
+    assert len(rr.bits) == 8
+
+    client.close()
+    await asyncio.sleep(0.1)
+    assert not client.transport
+
+    await client.connect()
+    await asyncio.sleep(0.1)
+    assert client.transport
+    rr = await client.read_coils(1, 1, slave=0x01)
+    assert len(rr.bits) == 8
+
+    client.close()
+    await asyncio.sleep(0.1)
+    assert not client.transport
+
+    await server.ServerAsyncStop()
+    task.cancel()
+    await task
+
+
+@pytest.mark.xdist_group(name="server_serialize")
+@pytest.mark.parametrize("comm", TEST_TYPES)
+async def test_async_task_server_stop(comm):
+    """Test normal client/server handling."""
+    run_server, server_args, run_client, client_args = helper_config(comm, "async")
+    task = asyncio.create_task(run_server(**server_args))
+    await asyncio.sleep(0.5)
 
     on_reconnect_callback = mock.Mock()
 
     client = run_client(**client_args, on_reconnect_callback=on_reconnect_callback)
     await client.connect()
-    assert client._connected  # pylint: disable=protected-access
+    assert client.transport
     rr = await client.read_coils(1, 1, slave=0x01)
     assert len(rr.bits) == 8
     on_reconnect_callback.assert_not_called()
 
     # Server breakdown
     await server.ServerAsyncStop()
     await task
 
     with pytest.raises((ConnectionException, asyncio.exceptions.TimeoutError)):
         rr = await client.read_coils(1, 1, slave=0x01)
-    assert not client._connected  # pylint: disable=protected-access
+    assert not client.transport
 
     # Server back online
     task = asyncio.create_task(run_server(**server_args))
-    await asyncio.sleep(0.1)
+    await asyncio.sleep(1)
 
     timer_allowed = 100
-    while not client._connected:  # pylint: disable=protected-access
+    while not client.transport and timer_allowed:
         await asyncio.sleep(0.1)
         timer_allowed -= 1
-        if not timer_allowed:
-            assert False, "client do not reconnect"
-    assert client._connected  # pylint: disable=protected-access
-    on_reconnect_callback.assert_called()
+    assert client.transport, "client do not reconnect"
+    # TBD on_reconnect_callback.assert_called()
 
     rr = await client.read_coils(1, 1, slave=0x01)
     assert len(rr.bits) == 8
 
-    await client.close()
+    client.close()
     await asyncio.sleep(0.5)
-    assert not client._connected  # pylint: disable=protected-access
+    assert not client.transport
     await server.ServerAsyncStop()
     await task
 
 
 @pytest.mark.xdist_group(name="server_serialize")
 @pytest.mark.parametrize("comm", TEST_TYPES)
 def test_sync_task_no_server(comm):
     """Test normal client/server handling."""
     run_server, server_args, run_client, client_args = helper_config(comm, "sync")
     client = run_client(**client_args)
     try:
         client.connect()
-    except Exception as exc:  # pylint: disable=broad-except
-        assert False, f"unexpected exception: {exc}"
+    except Exception as exc:
+        raise AssertionError(f"unexpected exception: {exc}") from exc
     sleep(0.1)
     if comm == "udp":
         rr = client.read_coils(1, 1, slave=0x01)
         assert isinstance(rr, ModbusIOException)
     else:
         with pytest.raises((asyncio.exceptions.TimeoutError, ConnectionException)):
             client.read_coils(1, 1, slave=0x01)
@@ -307,15 +339,15 @@
     sleep(0.1)
 
     timer_allowed = 100
     while not client.socket:
         sleep(0.1)
         timer_allowed -= 1
         if not timer_allowed:
-            assert False, "client do not reconnect"
+            pytest.fail("client do not reconnect")
     assert client.socket
 
     rr = client.read_coils(1, 1, slave=0x01)
     assert len(rr.bits) == 8
 
     client.close()
     sleep(0.5)
```

### Comparing `pymodbus-3.2.2/test/test_simulator.py` & `pymodbus-3.3.0/test/test_simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
             assert cell.access == str(reg.access), f"at register {test_reg}"
             assert cell.value == test_cell.value, f"at register {test_reg}"
             assert cell.action == test_cell.action, f"at register {test_reg}"
             assert cell.count_read == str(reg.count_read), f"at register {test_reg}"
             assert cell.count_write == str(reg.count_write), f"at register {test_reg}"
 
     @pytest.mark.parametrize(
-        "func,addr",
+        ("func", "addr"),
         [
             (FX_READ_BIT, 12),
             (FX_READ_REG, 16),
             (FX_READ_REG, 21),
             (FX_READ_REG, 33),
         ],
     )
```

### Comparing `pymodbus-3.2.2/test/test_transaction.py` & `pymodbus-3.3.0/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pymodbus-3.2.2/test/test_unix_socket.py` & `pymodbus-3.3.0/test/test_unix_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 @pytest_asyncio.fixture(name="_mock_run_server")
 async def _helper_server(path_addon):
     """Run server."""
     datablock = ModbusSequentialDataBlock(0x00, [17] * 100)
     context = ModbusSlaveContext(
         di=datablock, co=datablock, hr=datablock, ir=datablock, slave=1
     )
-    asyncio.create_task(
+    asyncio.create_task(  # noqa: RUF006
         StartAsyncUnixServer(
             context=ModbusServerContext(slaves=context, single=True),
             path=PATH + path_addon,
             framer=ModbusSocketFramer,
         )
     )
     await asyncio.sleep(0.1)
```

### Comparing `pymodbus-3.2.2/test/test_utilities.py` & `pymodbus-3.3.0/test/test_utilities.py`

 * *Files identical despite different names*

