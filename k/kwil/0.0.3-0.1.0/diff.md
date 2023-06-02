# Comparing `tmp/kwil-0.0.3.tar.gz` & `tmp/kwil-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwil-0.0.3.tar", last modified: Wed Apr 19 22:10:21 2023, max compression
+gzip compressed data, was "kwil-0.1.0.tar", last modified: Fri Jun  2 19:39:58 2023, max compression
```

## Comparing `kwil-0.0.3.tar` & `kwil-0.1.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.011729 kwil-0.0.3/
--rw-r--r--   0 gavin      (501) staff       (20)     1064 2023-04-19 22:10:21.011576 kwil-0.0.3/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-19 19:09:29.000000 kwil-0.0.3/README.md
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.001652 kwil-0.0.3/kwil/
--rw-r--r--   0 gavin      (501) staff       (20)       87 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/__about__.py
--rw-r--r--   0 gavin      (501) staff       (20)      322 2023-04-12 20:39:28.000000 kwil-0.0.3/kwil/__init__.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.005232 kwil-0.0.3/kwil/_utils/
--rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.0.3/kwil/_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/action.py
--rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.0.3/kwil/_utils/dataset.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.005719 kwil-0.0.3/kwil/_utils/grpc/
--rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/grpc/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2935 2023-04-12 20:45:39.000000 kwil-0.0.3/kwil/_utils/grpc/client.py
--rw-r--r--   0 gavin      (501) staff       (20)     2183 2023-04-12 15:56:08.000000 kwil-0.0.3/kwil/_utils/method_formatters.py
--rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/naming_converter.py
--rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/request.py
--rw-r--r--   0 gavin      (501) staff       (20)      504 2023-04-09 22:05:10.000000 kwil-0.0.3/kwil/_utils/rpcs.py
--rw-r--r--   0 gavin      (501) staff       (20)     1807 2023-04-12 20:01:31.000000 kwil-0.0.3/kwil/_utils/signature.py
--rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/signing.py
--rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-04-12 14:59:57.000000 kwil-0.0.3/kwil/_utils/transaction.py
--rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/utils.py
--rw-r--r--   0 gavin      (501) staff       (20)     3566 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/_utils/validation.py
--rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/exceptions.py
--rw-r--r--   0 gavin      (501) staff       (20)     1436 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/kwild.py
--rw-r--r--   0 gavin      (501) staff       (20)     4463 2023-04-19 21:52:22.000000 kwil-0.0.3/kwil/main.py
--rw-r--r--   0 gavin      (501) staff       (20)     1774 2023-04-12 15:18:49.000000 kwil-0.0.3/kwil/manager.py
--rw-r--r--   0 gavin      (501) staff       (20)     1808 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/method.py
--rw-r--r--   0 gavin      (501) staff       (20)      783 2023-04-12 15:19:39.000000 kwil-0.0.3/kwil/middleware.py
--rw-r--r--   0 gavin      (501) staff       (20)     1014 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/module.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.006732 kwil-0.0.3/kwil/provider/
--rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.0.3/kwil/provider/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/provider/auto.py
--rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.0.3/kwil/provider/base.py
--rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil/provider/grpc.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:20.998353 kwil-0.0.3/kwil/tx/
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.010243 kwil-0.0.3/kwil/tx/v1/
--rw-r--r--   0 gavin      (501) staff       (20)     1511 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/account_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/account_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1388 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/broadcast_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/broadcast_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1360 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/config_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/config_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     3435 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/dataset_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/dataset_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/list_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/list_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1219 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/ping_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/ping_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1375 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/price_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/price_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     1264 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/query_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/query_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     4479 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/service_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/service_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     2062 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/tx_pb2.py
--rw-r--r--   0 gavin      (501) staff       (20)      159 2023-04-12 20:44:51.000000 kwil-0.0.3/kwil/tx/v1/tx_pb2_grpc.py
--rw-r--r--   0 gavin      (501) staff       (20)     3413 2023-04-12 20:01:31.000000 kwil-0.0.3/kwil/types.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.002475 kwil-0.0.3/kwil.egg-info/
--rw-r--r--   0 gavin      (501) staff       (20)     1064 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/PKG-INFO
--rw-r--r--   0 gavin      (501) staff       (20)     1398 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/SOURCES.txt
--rw-r--r--   0 gavin      (501) staff       (20)        1 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/dependency_links.txt
--rw-r--r--   0 gavin      (501) staff       (20)      306 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/requires.txt
--rw-r--r--   0 gavin      (501) staff       (20)       28 2023-04-19 22:10:20.000000 kwil-0.0.3/kwil.egg-info/top_level.txt
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.010713 kwil-0.0.3/kwil_typing/
--rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.0.3/kwil_typing/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil_typing/kvm.py
-drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-04-19 22:10:21.011247 kwil-0.0.3/kwil_utils/
--rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.0.3/kwil_utils/__init__.py
--rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.0.3/kwil_utils/types.py
--rw-r--r--   0 gavin      (501) staff       (20)     1558 2023-04-19 22:04:12.000000 kwil-0.0.3/pyproject.toml
--rw-r--r--   0 gavin      (501) staff       (20)       38 2023-04-19 22:10:21.011772 kwil-0.0.3/setup.cfg
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.755613 kwil-0.1.0/
+-rw-r--r--   0 gavin      (501) staff       (20)     6861 2023-06-02 19:39:58.755427 kwil-0.1.0/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)     6201 2023-05-31 19:24:44.000000 kwil-0.1.0/README.md
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.745364 kwil-0.1.0/kwil/
+-rw-r--r--   0 gavin      (501) staff       (20)       87 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/__about__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      322 2023-04-12 20:39:28.000000 kwil-0.1.0/kwil/__init__.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.749041 kwil-0.1.0/kwil/_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)        0 2023-04-03 19:04:31.000000 kwil-0.1.0/kwil/_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1555 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/action.py
+-rw-r--r--   0 gavin      (501) staff       (20)      346 2023-04-10 22:57:27.000000 kwil-0.1.0/kwil/_utils/dataset.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.749474 kwil-0.1.0/kwil/_utils/grpc/
+-rw-r--r--   0 gavin      (501) staff       (20)       56 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/grpc/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2937 2023-05-31 19:12:10.000000 kwil-0.1.0/kwil/_utils/grpc/client.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2198 2023-05-31 19:16:43.000000 kwil-0.1.0/kwil/_utils/method_formatters.py
+-rw-r--r--   0 gavin      (501) staff       (20)      719 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/naming_converter.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2796 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/request.py
+-rw-r--r--   0 gavin      (501) staff       (20)      506 2023-05-31 19:12:24.000000 kwil-0.1.0/kwil/_utils/rpcs.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1807 2023-05-26 21:24:33.000000 kwil-0.1.0/kwil/_utils/signature.py
+-rw-r--r--   0 gavin      (501) staff       (20)      185 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/signing.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1210 2023-05-26 21:24:33.000000 kwil-0.1.0/kwil/_utils/transaction.py
+-rw-r--r--   0 gavin      (501) staff       (20)      419 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/_utils/utils.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3567 2023-05-31 19:13:30.000000 kwil-0.1.0/kwil/_utils/validation.py
+-rw-r--r--   0 gavin      (501) staff       (20)      404 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/exceptions.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1438 2023-05-31 19:13:18.000000 kwil-0.1.0/kwil/kwild.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4040 2023-05-31 19:26:30.000000 kwil-0.1.0/kwil/main.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1788 2023-05-30 21:22:03.000000 kwil-0.1.0/kwil/manager.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1867 2023-05-30 21:32:24.000000 kwil-0.1.0/kwil/method.py
+-rw-r--r--   0 gavin      (501) staff       (20)      783 2023-04-12 15:19:39.000000 kwil-0.1.0/kwil/middleware.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1028 2023-05-30 21:22:28.000000 kwil-0.1.0/kwil/module.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.750482 kwil-0.1.0/kwil/provider/
+-rw-r--r--   0 gavin      (501) staff       (20)      167 2023-04-12 15:29:34.000000 kwil-0.1.0/kwil/provider/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/provider/auto.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2344 2023-04-12 15:25:27.000000 kwil-0.1.0/kwil/provider/base.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1634 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil/provider/grpc.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.742665 kwil-0.1.0/kwil/tx/
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.754197 kwil-0.1.0/kwil/tx/v1/
+-rw-r--r--   0 gavin      (501) staff       (20)     1548 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/account_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/account_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1425 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/broadcast_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/broadcast_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1397 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/config_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/config_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2573 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/dataset_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/dataset_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1301 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/list_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/list_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1256 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/ping_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/ping_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1412 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/price_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/price_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1304 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/query_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/query_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     4529 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/service_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)    14437 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/service_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     2074 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/tx_pb2.py
+-rw-r--r--   0 gavin      (501) staff       (20)      159 2023-05-30 19:26:06.000000 kwil-0.1.0/kwil/tx/v1/tx_pb2_grpc.py
+-rw-r--r--   0 gavin      (501) staff       (20)     3413 2023-05-26 21:24:33.000000 kwil-0.1.0/kwil/types.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.746098 kwil-0.1.0/kwil.egg-info/
+-rw-r--r--   0 gavin      (501) staff       (20)     6861 2023-06-02 19:39:58.000000 kwil-0.1.0/kwil.egg-info/PKG-INFO
+-rw-r--r--   0 gavin      (501) staff       (20)     1398 2023-06-02 19:39:58.000000 kwil-0.1.0/kwil.egg-info/SOURCES.txt
+-rw-r--r--   0 gavin      (501) staff       (20)        1 2023-06-02 19:39:58.000000 kwil-0.1.0/kwil.egg-info/dependency_links.txt
+-rw-r--r--   0 gavin      (501) staff       (20)      306 2023-06-02 19:39:58.000000 kwil-0.1.0/kwil.egg-info/requires.txt
+-rw-r--r--   0 gavin      (501) staff       (20)       28 2023-06-02 19:39:58.000000 kwil-0.1.0/kwil.egg-info/top_level.txt
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.754596 kwil-0.1.0/kwil_typing/
+-rw-r--r--   0 gavin      (501) staff       (20)       81 2023-04-12 15:29:41.000000 kwil-0.1.0/kwil_typing/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)      148 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil_typing/kvm.py
+drwxr-xr-x   0 gavin      (501) staff       (20)        0 2023-06-02 19:39:58.755097 kwil-0.1.0/kwil_utils/
+-rw-r--r--   0 gavin      (501) staff       (20)      129 2023-04-11 19:46:10.000000 kwil-0.1.0/kwil_utils/__init__.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1065 2023-04-05 19:34:56.000000 kwil-0.1.0/kwil_utils/types.py
+-rw-r--r--   0 gavin      (501) staff       (20)     1558 2023-06-02 19:35:48.000000 kwil-0.1.0/pyproject.toml
+-rw-r--r--   0 gavin      (501) staff       (20)       38 2023-06-02 19:39:58.755673 kwil-0.1.0/setup.cfg
```

### Comparing `kwil-0.0.3/kwil/_utils/action.py` & `kwil-0.1.0/kwil/_utils/action.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/_utils/grpc/client.py` & `kwil-0.1.0/kwil/_utils/grpc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     broadcast_pb2,
     account_pb2,
     config_pb2,
     price_pb2,
     dataset_pb2,
     tx_pb2,
     list_pb2,
-    service_pb2_grpc
+    service_pb2_grpc,
 )
 
 # timeout in seconds
 READY_TIMEOUT = 3
 REQUEST_TIMEOUT = 2
 
 
@@ -76,10 +76,10 @@
         req = account_pb2.GetAccountRequest(address=address)
         return self.tx_stub.GetAccount(req, timeout=self.request_timeout)
 
     def get_schema(self, db_id: DBIdentifier) -> dataset_pb2.GetSchemaResponse:
         req = dataset_pb2.GetSchemaRequest(dbid=db_id)
         return self.tx_stub.GetSchema(req, timeout=self.request_timeout)
 
-    def list_database(self, owner: HexAddress) -> list_pb2.ListDatabasesResponse:
+    def list_databases(self, owner: HexAddress) -> list_pb2.ListDatabasesResponse:
         req = list_pb2.ListDatabasesRequest(owner=owner)
         return self.tx_stub.ListDatabases(req, timeout=self.request_timeout)
```

### Comparing `kwil-0.0.3/kwil/_utils/method_formatters.py` & `kwil-0.1.0/kwil/_utils/method_formatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,21 +54,21 @@
 response_formatters: Dict[str, Callable[[Any], Any]] = {
     GRPC.kwil_ping: ping_response_formatter,
     GRPC.kwil_getSchema: extract_result("dataset"),
     GRPC.kwil_getConfig: identity,
     GRPC.kwil_getAccount: extract_result("account"),
     GRPC.kwil_estimatePrice: extract_result("price"),
     GRPC.kwil_broadcast: tx_receipt_decode,
-    GRPC.kwil_listDatabase: extract_result("databases"),
+    GRPC.kwil_listDatabases: extract_result("databases"),
     GRPC.kwil_query: query_decode,
 }
 
 
 def get_response_formatters(
-    method_name: RPCEndpoint, module: "Module"
+    method_name: RPCEndpoint, module: "Module"  # noqa: F821
 ) -> Callable[..., Any]:
     formatter_maps = (response_formatters,)
 
     return compose(
         *[
             formatter_map[method_name]
             for formatter_map in formatter_maps
```

### Comparing `kwil-0.0.3/kwil/_utils/naming_converter.py` & `kwil-0.1.0/kwil/_utils/naming_converter.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/_utils/request.py` & `kwil-0.1.0/kwil/_utils/request.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/_utils/signature.py` & `kwil-0.1.0/kwil/_utils/signature.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/_utils/transaction.py` & `kwil-0.1.0/kwil/_utils/transaction.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/_utils/validation.py` & `kwil-0.1.0/kwil/_utils/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 
 request_validators: Dict[RPCEndpoint, Callable[..., Any]] = {
     GRPC.kwil_ping: identity,
     GRPC.kwil_getConfig: identity,
     GRPC.kwil_getSchema: apply_validator_at_index(validate_db_identifier, 0),
     GRPC.kwil_getAccount: apply_validator_at_index(validate_address, 0),
-    GRPC.kwil_listDatabase: apply_validator_at_index(validate_address, 0),
+    GRPC.kwil_listDatabases: apply_validator_at_index(validate_address, 0),
     GRPC.kwil_broadcast: apply_validator_at_index(validate_tx_params, 0),
     GRPC.kwil_estimatePrice: apply_validator_at_index(validate_tx_params, 0),
     GRPC.kwil_query: compose(
         apply_validator_at_index(validate_db_identifier, 0),
         apply_validator_at_index(validate_query, 1),
     ),
 }
```

### Comparing `kwil-0.0.3/kwil/kwild.py` & `kwil-0.1.0/kwil/kwild.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,16 @@
     get_config: Method[Callable[[], ServiceConfig]] = Method(GRPC.kwil_getConfig)
 
 
 class Kwild(BaseKwild):
     """Kwil Chain class"""
 
     get_schema: Method[Callable[[DBIdentifier], DBSchema]] = Method(GRPC.kwil_getSchema)
-    list_database: Method[Callable[[HexAddress], List[DBSchema]]] = Method(
-        GRPC.kwil_listDatabase
+    list_databases: Method[Callable[[HexAddress], List[DBSchema]]] = Method(
+        GRPC.kwil_listDatabases
     )
     get_account: Method[Callable[[HexAddress], AccountInfo]] = Method(
         GRPC.kwil_getAccount
     )
     broadcast: Method[Callable[[TxParams], TxReceipt]] = Method(GRPC.kwil_broadcast)
     estimate_price: Method[Callable[[TxParams], str]] = Method(GRPC.kwil_estimatePrice)
     query: Method[Callable[[DBIdentifier, str], TxReceipt]] = Method(GRPC.kwil_query)
```

### Comparing `kwil-0.0.3/kwil/main.py` & `kwil-0.1.0/kwil/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Nonce,
     TxReceipt,
     DatasetIdentifier,
     DBIdentifier,
     ActionExecution,
 )
 from kwil._utils.transaction import sign_tx
-from kwil._utils.action import encode_action_inputs
 from kwil._utils.dataset import generate_dbi
 from kwil._utils.signing import load_wallet
 
 
 class BaseKwil:
     GRPCProvider = GRPCProvider
     RequestManager = DefaultRequestManager
@@ -83,58 +82,51 @@
         tx_params = TxParams(
             payloadType=payload_type,
             payload=payload,
             sender=self.wallet.address,
             fee="0",
             # SHOULD be done in result formatter
             nonce=Nonce(int(account_info["nonce"]) + 1),
-            # nonce=Nonce(1),
         )
 
         price = self.kwild.estimate_price(tx_params)
         tx_params["fee"] = price
         tx_params = sign_tx(tx_params, self.wallet)
         return tx_params
 
     def deploy_database(self, payload: bytes) -> TxReceipt:
         payload_type = TxPayloadType.DEPLOY_DATABASE
         tx_params = self._create_tx(payload_type, payload)
         return self.kwild.broadcast(tx_params)
 
-    def get_database(self, name: str, owner: Optional[str] = None) -> Dict[str, Any]:
-        if owner is None:
-            owner = self.wallet.address
-        db_identifier = generate_dbi(owner, name)
-        return self.kwild.get_schema(db_identifier)
+    def get_schema(self, db_id: DBIdentifier) -> Dict[str, Any]:
+        return self.kwild.get_schema(db_id)
 
-    def list_database(self, address: Optional[str] = None) -> List[Dict[str, Any]]:
+    def list_databases(self, address: Optional[str] = None) -> List[Dict[str, Any]]:
         if address is None:
             address = self.wallet.address
-        return self.kwild.list_database(address)
+        return self.kwild.list_databases(address)
 
     def drop_database(self, name: str) -> TxReceipt:
         payload_type = TxPayloadType.DROP_DATABASE
         db_identifier = DatasetIdentifier(owner=self.wallet.address, name=name)
         payload = json.dumps(db_identifier)
         tx_params = self._create_tx(payload_type, payload.encode())
         return self.kwild.broadcast(tx_params)
 
     def execute_action(
         self,
-        db_name: str,
+        db_id: DBIdentifier,
         action_name: str,
         inputs: List[Dict[str, Any]],
     ) -> TxReceipt:
         # TODO: dynamic call action
-        db_identifier = generate_dbi(self.wallet.address, db_name)
-        encoded_inputs = encode_action_inputs(inputs)
         exec_body = ActionExecution(
-            action=action_name, dbID=db_identifier, params=encoded_inputs
+            action=action_name, dbID=db_id, params=inputs
         )
         payload_type = TxPayloadType.EXECUTE_ACTION
         payload = json.dumps(exec_body).encode()
         tx_params = self._create_tx(payload_type, payload)
         return self.kwild.broadcast(tx_params)
 
-    def query(self, db_name: str, query: str) -> TxReceipt:
-        db_identifier = generate_dbi(self.wallet.address, db_name)
-        return self.kwild.query(db_identifier, query)
+    def query(self, db_id: DBIdentifier, query: str) -> TxReceipt:
+        return self.kwild.query(db_id, query)
```

### Comparing `kwil-0.0.3/kwil/manager.py` & `kwil-0.1.0/kwil/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class RequestManager:
     logger = logging.getLogger("kwil.RequestManager")
 
     _provider = None
 
     def __init__(
         self,
-        kwil: "Kwil",
+        kwil: "Kwil",  # noqa: F821
         provider: Optional[BaseProvider] = None,
         # middlewares: Optional[List[Tuple[str, Middleware]]] = None,
     ):
         self.kwil = kwil
 
         if provider is None:
             self.provider = AutoProvider()
```

### Comparing `kwil-0.0.3/kwil/method.py` & `kwil-0.1.0/kwil/method.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,24 +32,26 @@
     ):
         self.rpc_method = rpc_method
         self.request_formatters = request_formatters or get_request_formatters
         self.response_formatters = response_formatters or get_response_formatters
 
     # as Descriptor
     def __get__(
-        self, obj: Optional["Module"] = None, obj_type: Optional[Type["Module"]] = None
+        self,
+        obj: Optional["Module"] = None,  # noqa: F821
+        obj_type: Optional[Type["Module"]] = None,  # noqa: F821
     ) -> TFunc:
         if obj is None:
             raise TypeError("Methods must be called on an instance of a Module class")
         return obj.caller_fn(obj.kwil, self)
 
     def method_selector_fn(self) -> Callable[..., Any]:
         raise NotImplementedError("Must be implemented by subclasses")
 
-    def process_params(self, module: "Module", *args: Any) -> Any:
+    def process_params(self, module: "Module", *args: Any) -> Any:  # noqa: F821
         # to simplify, kwargs are not supported
 
         method = self.rpc_method
 
         response_formatters = self.response_formatters(method, module)
 
         _apply_request_validator(self.rpc_method, args, self.request_formatters(method))
```

### Comparing `kwil-0.0.3/kwil/middleware.py` & `kwil-0.1.0/kwil/middleware.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/module.py` & `kwil-0.1.0/kwil/module.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     else:
         return result
 
 
 class Module:
     @curry
     def caller_fn(
-        self, kwil: "Kwil", method: Method[Callable[..., Any]]
+        self, kwil: "Kwil", method: Method[Callable[..., Any]]  # noqa: F821
     ) -> Callable[..., Any]:
         def caller(*args: Any) -> Any:
             (method_str, args), response_formatters = method.process_params(self, *args)
             result = kwil.manager.request_blocking(method_str, args)
             return _apply_result_formatters(
                 method.rpc_method, response_formatters, result
             )
```

### Comparing `kwil-0.0.3/kwil/provider/auto.py` & `kwil-0.1.0/kwil/provider/auto.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/provider/base.py` & `kwil-0.1.0/kwil/provider/base.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/provider/grpc.py` & `kwil-0.1.0/kwil/provider/grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/tx/v1/account_pb2.py` & `kwil-0.1.0/kwil/tx/v1/account_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/account.proto\x12\x02tx\":\n\x07\x41\x63\x63ount\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0f\n\x07\x62\x61lance\x18\x02 \x01(\t\x12\r\n\x05nonce\x18\x03 \x01(\x03\"$\n\x11GetAccountRequest\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"2\n\x12GetAccountResponse\x12\x1c\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x0b.tx.AccountB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/account.proto\x12\x02tx\":\n\x07\x41\x63\x63ount\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0f\n\x07\x62\x61lance\x18\x02 \x01(\t\x12\r\n\x05nonce\x18\x03 \x01(\x03\"$\n\x11GetAccountRequest\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"2\n\x12GetAccountResponse\x12\x1c\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x0b.tx.AccountB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.account_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _ACCOUNT._serialized_start=32
   _ACCOUNT._serialized_end=90
   _GETACCOUNTREQUEST._serialized_start=92
   _GETACCOUNTREQUEST._serialized_end=128
   _GETACCOUNTRESPONSE._serialized_start=130
   _GETACCOUNTRESPONSE._serialized_end=180
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/broadcast_pb2.py` & `kwil-0.1.0/kwil/tx/v1/broadcast_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from kwil.tx.v1 import tx_pb2 as kwil_dot_tx_dot_v1_dot_tx__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1akwil/tx/v1/broadcast.proto\x12\x02tx\x1a\x13kwil/tx/v1/tx.proto\"&\n\x10\x42roadcastRequest\x12\x12\n\x02tx\x18\x01 \x01(\x0b\x32\x06.tx.Tx\"3\n\x11\x42roadcastResponse\x12\x1e\n\x07receipt\x18\x01 \x01(\x0b\x32\r.tx.TxReceiptB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1akwil/tx/v1/broadcast.proto\x12\x02tx\x1a\x13kwil/tx/v1/tx.proto\"&\n\x10\x42roadcastRequest\x12\x12\n\x02tx\x18\x01 \x01(\x0b\x32\x06.tx.Tx\"3\n\x11\x42roadcastResponse\x12\x1e\n\x07receipt\x18\x01 \x01(\x0b\x32\r.tx.TxReceiptB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.broadcast_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _BROADCASTREQUEST._serialized_start=55
   _BROADCASTREQUEST._serialized_end=93
   _BROADCASTRESPONSE._serialized_start=95
   _BROADCASTRESPONSE._serialized_end=146
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/config_pb2.py` & `kwil-0.1.0/kwil/tx/v1/config_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17kwil/tx/v1/config.proto\x12\x02tx\"\x12\n\x10GetConfigRequest\"\x83\x01\n\x11GetConfigResponse\x12\x1e\n\nchain_code\x18\x01 \x01(\x03R\nchain_code\x12*\n\x10provider_address\x18\x02 \x01(\tR\x10provider_address\x12\"\n\x0cpool_address\x18\x03 \x01(\tR\x0cpool_addressB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17kwil/tx/v1/config.proto\x12\x02tx\"\x12\n\x10GetConfigRequest\"\x83\x01\n\x11GetConfigResponse\x12\x1e\n\nchain_code\x18\x01 \x01(\x03R\nchain_code\x12*\n\x10provider_address\x18\x02 \x01(\tR\x10provider_address\x12\"\n\x0cpool_address\x18\x03 \x01(\tR\x0cpool_addressB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.config_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _GETCONFIGREQUEST._serialized_start=31
   _GETCONFIGREQUEST._serialized_end=49
   _GETCONFIGRESPONSE._serialized_start=52
   _GETCONFIGRESPONSE._serialized_end=183
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/dataset_pb2.py` & `kwil-0.1.0/kwil/tx/v1/dataset_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,38 +9,32 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/dataset.proto\x12\x02tx\" \n\x10GetSchemaRequest\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\t\"1\n\x11GetSchemaResponse\x12\x1c\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x0b.tx.Dataset\"^\n\x07\x44\x61taset\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x06tables\x18\x03 \x03(\x0b\x32\t.tx.Table\x12\x1b\n\x07\x61\x63tions\x18\x04 \x03(\x0b\x32\n.tx.Action\"N\n\x05Table\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\n.tx.Column\x12\x1a\n\x07indexes\x18\x03 \x03(\x0b\x32\t.tx.Index\"U\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x04type\x18\x02 \x01(\x0e\x32\x0c.tx.DataType\x12!\n\nattributes\x18\x03 \x03(\x0b\x32\r.tx.Attribute\";\n\tAttribute\x12\x1f\n\x04type\x18\x01 \x01(\x0e\x32\x11.tx.AttributeType\x12\r\n\x05value\x18\x02 \x01(\x0c\"C\n\x05Index\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x1b\n\x04type\x18\x03 \x01(\x0e\x32\r.tx.IndexType\"J\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x0e\n\x06inputs\x18\x03 \x03(\t\x12\x12\n\nstatements\x18\x04 \x03(\t*^\n\x08\x44\x61taType\x12\x15\n\x11INVALID_DATA_TYPE\x10\x00\x12\x12\n\x0eNULL_DATA_TYPE\x10\x01\x12\x14\n\x10STRING_DATA_TYPE\x10\x02\x12\x11\n\rINT_DATA_TYPE\x10\x03*\x90\x01\n\rAttributeType\x12\x15\n\x11INVALID_ATTRIBUTE\x10\x00\x12\x0f\n\x0bPRIMARY_KEY\x10\x01\x12\n\n\x06UNIQUE\x10\x02\x12\x0c\n\x08NOT_NULL\x10\x03\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x04\x12\x07\n\x03MIN\x10\x05\x12\x07\n\x03MAX\x10\x06\x12\x0e\n\nMIN_LENGTH\x10\x07\x12\x0e\n\nMAX_LENGTH\x10\x08*V\n\tIndexType\x12\x16\n\x12INVALID_INDEX_TYPE\x10\x00\x12\x14\n\x10\x42TREE_INDEX_TYPE\x10\x01\x12\x1b\n\x17UNIQUE_BTREE_INDEX_TYPE\x10\x02\x42\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/dataset.proto\x12\x02tx\" \n\x10GetSchemaRequest\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\t\"1\n\x11GetSchemaResponse\x12\x1c\n\x07\x64\x61taset\x18\x01 \x01(\x0b\x32\x0b.tx.Dataset\"^\n\x07\x44\x61taset\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x19\n\x06tables\x18\x03 \x03(\x0b\x32\t.tx.Table\x12\x1b\n\x07\x61\x63tions\x18\x04 \x03(\x0b\x32\n.tx.Action\"N\n\x05Table\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1b\n\x07\x63olumns\x18\x02 \x03(\x0b\x32\n.tx.Column\x12\x1a\n\x07indexes\x18\x03 \x03(\x0b\x32\t.tx.Index\"G\n\x06\x43olumn\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12!\n\nattributes\x18\x03 \x03(\x0b\x32\r.tx.Attribute\"(\n\tAttribute\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"4\n\x05Index\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\"J\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06public\x18\x02 \x01(\x08\x12\x0e\n\x06inputs\x18\x03 \x03(\t\x12\x12\n\nstatements\x18\x04 \x03(\tB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.dataset_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
-  _DATATYPE._serialized_start=586
-  _DATATYPE._serialized_end=680
-  _ATTRIBUTETYPE._serialized_start=683
-  _ATTRIBUTETYPE._serialized_end=827
-  _INDEXTYPE._serialized_start=829
-  _INDEXTYPE._serialized_end=915
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _GETSCHEMAREQUEST._serialized_start=32
   _GETSCHEMAREQUEST._serialized_end=64
   _GETSCHEMARESPONSE._serialized_start=66
   _GETSCHEMARESPONSE._serialized_end=115
   _DATASET._serialized_start=117
   _DATASET._serialized_end=211
   _TABLE._serialized_start=213
   _TABLE._serialized_end=291
   _COLUMN._serialized_start=293
-  _COLUMN._serialized_end=378
-  _ATTRIBUTE._serialized_start=380
-  _ATTRIBUTE._serialized_end=439
-  _INDEX._serialized_start=441
-  _INDEX._serialized_end=508
-  _ACTION._serialized_start=510
-  _ACTION._serialized_end=584
+  _COLUMN._serialized_end=364
+  _ATTRIBUTE._serialized_start=366
+  _ATTRIBUTE._serialized_end=406
+  _INDEX._serialized_start=408
+  _INDEX._serialized_end=460
+  _ACTION._serialized_start=462
+  _ACTION._serialized_end=536
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/list_pb2.py` & `kwil-0.1.0/kwil/tx/v1/list_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15kwil/tx/v1/list.proto\x12\x02tx\"%\n\x14ListDatabasesRequest\x12\r\n\x05owner\x18\x01 \x01(\t\"*\n\x15ListDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\tB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15kwil/tx/v1/list.proto\x12\x02tx\"%\n\x14ListDatabasesRequest\x12\r\n\x05owner\x18\x01 \x01(\t\"*\n\x15ListDatabasesResponse\x12\x11\n\tdatabases\x18\x01 \x03(\tB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.list_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _LISTDATABASESREQUEST._serialized_start=29
   _LISTDATABASESREQUEST._serialized_end=66
   _LISTDATABASESRESPONSE._serialized_start=68
   _LISTDATABASESRESPONSE._serialized_end=110
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/ping_pb2.py` & `kwil-0.1.0/kwil/tx/v1/ping_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15kwil/tx/v1/ping.proto\x12\x02tx\"\x1e\n\x0bPingRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\"\x1f\n\x0cPingResponse\x12\x0f\n\x07message\x18\x01 \x01(\tB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15kwil/tx/v1/ping.proto\x12\x02tx\"\x1e\n\x0bPingRequest\x12\x0f\n\x07message\x18\x01 \x01(\t\"\x1f\n\x0cPingResponse\x12\x0f\n\x07message\x18\x01 \x01(\tB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.ping_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _PINGREQUEST._serialized_start=29
   _PINGREQUEST._serialized_end=59
   _PINGRESPONSE._serialized_start=61
   _PINGRESPONSE._serialized_end=92
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/price_pb2.py` & `kwil-0.1.0/kwil/tx/v1/price_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from kwil.tx.v1 import tx_pb2 as kwil_dot_tx_dot_v1_dot_tx__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16kwil/tx/v1/price.proto\x12\x02tx\x1a\x13kwil/tx/v1/tx.proto\"*\n\x14\x45stimatePriceRequest\x12\x12\n\x02tx\x18\x01 \x01(\x0b\x32\x06.tx.Tx\"&\n\x15\x45stimatePriceResponse\x12\r\n\x05price\x18\x01 \x01(\tB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16kwil/tx/v1/price.proto\x12\x02tx\x1a\x13kwil/tx/v1/tx.proto\"*\n\x14\x45stimatePriceRequest\x12\x12\n\x02tx\x18\x01 \x01(\x0b\x32\x06.tx.Tx\"&\n\x15\x45stimatePriceResponse\x12\r\n\x05price\x18\x01 \x01(\tB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.price_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _ESTIMATEPRICEREQUEST._serialized_start=51
   _ESTIMATEPRICEREQUEST._serialized_end=93
   _ESTIMATEPRICERESPONSE._serialized_start=95
   _ESTIMATEPRICERESPONSE._serialized_end=133
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/query_pb2.py` & `kwil-0.1.0/kwil/tx/v1/query_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16kwil/tx/v1/query.proto\x12\x02tx\"+\n\x0cQueryRequest\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\"\x1f\n\rQueryResponse\x12\x0e\n\x06result\x18\x01 \x01(\x0c\x42\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16kwil/tx/v1/query.proto\x12\x02tx\"+\n\x0cQueryRequest\x12\x0c\n\x04\x64\x62id\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\"\x1f\n\rQueryResponse\x12\x0e\n\x06result\x18\x01 \x01(\x0c\x42\x35Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _QUERYREQUEST._serialized_start=30
   _QUERYREQUEST._serialized_end=73
   _QUERYRESPONSE._serialized_start=75
   _QUERYRESPONSE._serialized_end=106
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/service_pb2.py` & `kwil-0.1.0/kwil/tx/v1/service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 from kwil.tx.v1 import account_pb2 as kwil_dot_tx_dot_v1_dot_account__pb2
 from kwil.tx.v1 import config_pb2 as kwil_dot_tx_dot_v1_dot_config__pb2
 from kwil.tx.v1 import list_pb2 as kwil_dot_tx_dot_v1_dot_list__pb2
 from kwil.tx.v1 import dataset_pb2 as kwil_dot_tx_dot_v1_dot_dataset__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/service.proto\x12\x02tx\x1a\x1akwil/tx/v1/broadcast.proto\x1a\x16kwil/tx/v1/price.proto\x1a\x16kwil/tx/v1/query.proto\x1a\x15kwil/tx/v1/ping.proto\x1a\x18kwil/tx/v1/account.proto\x1a\x17kwil/tx/v1/config.proto\x1a\x15kwil/tx/v1/list.proto\x1a\x18kwil/tx/v1/dataset.proto\x1a\x1cgoogle/api/annotations.proto2\xcc\x05\n\tTxService\x12V\n\tBroadcast\x12\x14.tx.BroadcastRequest\x1a\x15.tx.BroadcastResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/api/v1/broadcast:\x01*\x12g\n\rEstimatePrice\x12\x18.tx.EstimatePriceRequest\x1a\x19.tx.EstimatePriceResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/api/v1/estimate_price:\x01*\x12\x46\n\x05Query\x12\x10.tx.QueryRequest\x1a\x11.tx.QueryResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/api/v1/query:\x01*\x12_\n\nGetAccount\x12\x15.tx.GetAccountRequest\x1a\x16.tx.GetAccountResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/accounts/{address}\x12?\n\x04Ping\x12\x0f.tx.PingRequest\x1a\x10.tx.PingResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/api/v1/ping\x12P\n\tGetConfig\x12\x14.tx.GetConfigRequest\x1a\x15.tx.GetConfigResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/api/v1/config\x12_\n\rListDatabases\x12\x18.tx.ListDatabasesRequest\x1a\x19.tx.ListDatabasesResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/databases\x12\x61\n\tGetSchema\x12\x14.tx.GetSchemaRequest\x1a\x15.tx.GetSchemaResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/databases/{dbid}/schemaB\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18kwil/tx/v1/service.proto\x12\x02tx\x1a\x1akwil/tx/v1/broadcast.proto\x1a\x16kwil/tx/v1/price.proto\x1a\x16kwil/tx/v1/query.proto\x1a\x15kwil/tx/v1/ping.proto\x1a\x18kwil/tx/v1/account.proto\x1a\x17kwil/tx/v1/config.proto\x1a\x15kwil/tx/v1/list.proto\x1a\x18kwil/tx/v1/dataset.proto\x1a\x1cgoogle/api/annotations.proto2\xd4\x05\n\tTxService\x12V\n\tBroadcast\x12\x14.tx.BroadcastRequest\x1a\x15.tx.BroadcastResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\"\x11/api/v1/broadcast:\x01*\x12g\n\rEstimatePrice\x12\x18.tx.EstimatePriceRequest\x1a\x19.tx.EstimatePriceResponse\"!\x82\xd3\xe4\x93\x02\x1b\"\x16/api/v1/estimate_price:\x01*\x12\x46\n\x05Query\x12\x10.tx.QueryRequest\x1a\x11.tx.QueryResponse\"\x18\x82\xd3\xe4\x93\x02\x12\"\r/api/v1/query:\x01*\x12_\n\nGetAccount\x12\x15.tx.GetAccountRequest\x1a\x16.tx.GetAccountResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/accounts/{address}\x12?\n\x04Ping\x12\x0f.tx.PingRequest\x1a\x10.tx.PingResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/api/v1/ping\x12P\n\tGetConfig\x12\x14.tx.GetConfigRequest\x1a\x15.tx.GetConfigResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/api/v1/config\x12g\n\rListDatabases\x12\x18.tx.ListDatabasesRequest\x1a\x19.tx.ListDatabasesResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/api/v1/{owner}/databases\x12\x61\n\tGetSchema\x12\x14.tx.GetSchemaRequest\x1a\x15.tx.GetSchemaResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/databases/{dbid}/schemaB5Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
   _TXSERVICE.methods_by_name['Broadcast']._options = None
   _TXSERVICE.methods_by_name['Broadcast']._serialized_options = b'\202\323\344\223\002\026\"\021/api/v1/broadcast:\001*'
   _TXSERVICE.methods_by_name['EstimatePrice']._options = None
   _TXSERVICE.methods_by_name['EstimatePrice']._serialized_options = b'\202\323\344\223\002\033\"\026/api/v1/estimate_price:\001*'
   _TXSERVICE.methods_by_name['Query']._options = None
   _TXSERVICE.methods_by_name['Query']._serialized_options = b'\202\323\344\223\002\022\"\r/api/v1/query:\001*'
   _TXSERVICE.methods_by_name['GetAccount']._options = None
   _TXSERVICE.methods_by_name['GetAccount']._serialized_options = b'\202\323\344\223\002\034\022\032/api/v1/accounts/{address}'
   _TXSERVICE.methods_by_name['Ping']._options = None
   _TXSERVICE.methods_by_name['Ping']._serialized_options = b'\202\323\344\223\002\016\022\014/api/v1/ping'
   _TXSERVICE.methods_by_name['GetConfig']._options = None
   _TXSERVICE.methods_by_name['GetConfig']._serialized_options = b'\202\323\344\223\002\020\022\016/api/v1/config'
   _TXSERVICE.methods_by_name['ListDatabases']._options = None
-  _TXSERVICE.methods_by_name['ListDatabases']._serialized_options = b'\202\323\344\223\002\023\022\021/api/v1/databases'
+  _TXSERVICE.methods_by_name['ListDatabases']._serialized_options = b'\202\323\344\223\002\033\022\031/api/v1/{owner}/databases'
   _TXSERVICE.methods_by_name['GetSchema']._options = None
   _TXSERVICE.methods_by_name['GetSchema']._serialized_options = b'\202\323\344\223\002!\022\037/api/v1/databases/{dbid}/schema'
   _TXSERVICE._serialized_start=262
-  _TXSERVICE._serialized_end=978
+  _TXSERVICE._serialized_end=986
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/tx/v1/service_pb2_grpc.py` & `kwil-0.1.0/kwil/tx/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil/tx/v1/tx_pb2.py` & `kwil-0.1.0/kwil/tx/v1/tx_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13kwil/tx/v1/tx.proto\x12\x02tx\"\x95\x01\n\x02Tx\x12\x0c\n\x04hash\x18\x01 \x01(\x0c\x12\"\n\x0cpayload_type\x18\x02 \x01(\x05R\x0cpayload_type\x12\x0f\n\x07payload\x18\x03 \x01(\x0c\x12\r\n\x05nonce\x18\x04 \x01(\x03\x12 \n\tsignature\x18\x05 \x01(\x0b\x32\r.tx.Signature\x12\x0b\n\x03\x66\x65\x65\x18\x06 \x01(\t\x12\x0e\n\x06sender\x18\x07 \x01(\t\"p\n\tSignature\x12(\n\x0fsignature_bytes\x18\x01 \x01(\x0cR\x0fsignature_bytes\x12\x39\n\x0esignature_type\x18\x02 \x01(\x0e\x32\x11.tx.SignatureTypeR\x0esignature_type\"7\n\tTxReceipt\x12\x0f\n\x07tx_hash\x18\x01 \x01(\x0c\x12\x0b\n\x03\x66\x65\x65\x18\x02 \x01(\t\x12\x0c\n\x04\x62ody\x18\x03 \x01(\x0c*\x85\x01\n\rSignatureType\x12\x19\n\x15INVALID_SINATURE_TYPE\x10\x00\x12\x1d\n\x19PK_SECP256K1_UNCOMPRESSED\x10\x01\x12\"\n\x1e\x41\x43\x43OUNT_SECP256K1_UNCOMPRESSED\x10\x02\x12\x16\n\x12\x45ND_SIGNATURE_TYPE\x10\x03\x42\x1eZ\x1ckwil/api/protobuf/tx/v1;txpbb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13kwil/tx/v1/tx.proto\x12\x02tx\"\x95\x01\n\x02Tx\x12\x0c\n\x04hash\x18\x01 \x01(\x0c\x12\"\n\x0cpayload_type\x18\x02 \x01(\x05R\x0cpayload_type\x12\x0f\n\x07payload\x18\x03 \x01(\x0c\x12\r\n\x05nonce\x18\x04 \x01(\x03\x12 \n\tsignature\x18\x05 \x01(\x0b\x32\r.tx.Signature\x12\x0b\n\x03\x66\x65\x65\x18\x06 \x01(\t\x12\x0e\n\x06sender\x18\x07 \x01(\t\"]\n\tSignature\x12(\n\x0fsignature_bytes\x18\x01 \x01(\x0cR\x0fsignature_bytes\x12&\n\x0esignature_type\x18\x02 \x01(\x05R\x0esignature_type\"7\n\tTxReceipt\x12\x0f\n\x07tx_hash\x18\x01 \x01(\x0c\x12\x0b\n\x03\x66\x65\x65\x18\x02 \x01(\t\x12\x0c\n\x04\x62ody\x18\x03 \x01(\x0c*\x85\x01\n\rSignatureType\x12\x19\n\x15INVALID_SINATURE_TYPE\x10\x00\x12\x1d\n\x19PK_SECP256K1_UNCOMPRESSED\x10\x01\x12\"\n\x1e\x41\x43\x43OUNT_SECP256K1_UNCOMPRESSED\x10\x02\x12\x16\n\x12\x45ND_SIGNATURE_TYPE\x10\x03\x42\x35Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpbb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kwil.tx.v1.tx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\034kwil/api/protobuf/tx/v1;txpb'
-  _SIGNATURETYPE._serialized_start=351
-  _SIGNATURETYPE._serialized_end=484
+  DESCRIPTOR._serialized_options = b'Z3github.com/kwilteam/kwil-db/api/protobuf/tx/v1;txpb'
+  _SIGNATURETYPE._serialized_start=332
+  _SIGNATURETYPE._serialized_end=465
   _TX._serialized_start=28
   _TX._serialized_end=177
   _SIGNATURE._serialized_start=179
-  _SIGNATURE._serialized_end=291
-  _TXRECEIPT._serialized_start=293
-  _TXRECEIPT._serialized_end=348
+  _SIGNATURE._serialized_end=272
+  _TXRECEIPT._serialized_start=274
+  _TXRECEIPT._serialized_end=329
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kwil-0.0.3/kwil/types.py` & `kwil-0.1.0/kwil/types.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil.egg-info/SOURCES.txt` & `kwil-0.1.0/kwil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/kwil_utils/types.py` & `kwil-0.1.0/kwil_utils/types.py`

 * *Files identical despite different names*

### Comparing `kwil-0.0.3/pyproject.toml` & `kwil-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=67.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kwil"
 description = 'Library for interacting with the kwil blockchain'
-version = "0.0.3"
+version = "0.1.0"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT License"}
 keywords = ["kwil"]
 authors = [
   { name = "yaiba", email = "4yaiba@gmail.com" },
 ]
```

