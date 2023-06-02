# Comparing `tmp/Aruna-Python-API-1.1.0rc1.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.1.0rc1.tar", last modified: Fri Jun  2 08:49:14 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc2.tar", last modified: Fri Jun  2 09:22:40 2023, max compression
```

## Comparing `Aruna-Python-API-1.1.0rc1.tar` & `Aruna-Python-API-1.1.0rc2.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23232 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.709473 Aruna-Python-API-1.1.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.701473 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 09:22:40.000000 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-02 09:22:40.000000 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:22:40.000000 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-02 09:22:40.000000 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 09:22:40.000000 Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 09:22:40.709473 Aruna-Python-API-1.1.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.701473 Aruna-Python-API-1.1.0rc2/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.701473 Aruna-Python-API-1.1.0rc2/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.701473 Aruna-Python-API-1.1.0rc2/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/bundler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/bundler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/bundler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.705473 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:40.709473 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:22:13.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23232 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 09:22:40.709473 Aruna-Python-API-1.1.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 09:22:24.000000 Aruna-Python-API-1.1.0rc2/setup.py
```

### Comparing `Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc2/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 aruna/__init__.py
 aruna/api/__init__.py
 aruna/api/internal/__init__.py
 aruna/api/internal/v1/__init__.py
 aruna/api/internal/v1/authorize_pb2.py
 aruna/api/internal/v1/authorize_pb2.pyi
 aruna/api/internal/v1/authorize_pb2_grpc.py
+aruna/api/internal/v1/bundler_pb2.py
+aruna/api/internal/v1/bundler_pb2.pyi
+aruna/api/internal/v1/bundler_pb2_grpc.py
 aruna/api/internal/v1/notification_pb2.py
 aruna/api/internal/v1/notification_pb2.pyi
 aruna/api/internal/v1/notification_pb2_grpc.py
 aruna/api/internal/v1/proxy_pb2.py
 aruna/api/internal/v1/proxy_pb2.pyi
 aruna/api/internal/v1/proxy_pb2_grpc.py
 aruna/api/notification/__init__.py
```

### Comparing `Aruna-Python-API-1.1.0rc1/LICENSE` & `Aruna-Python-API-1.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/PKG-INFO` & `Aruna-Python-API-1.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc1
+Version: 1.1.0rc2
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc1/README.md` & `Aruna-Python-API-1.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%aruna/api/internal/v1/authorize.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a(aruna/api/storage/models/v1/models.proto\"K\n\rAuthorization\x12\x1c\n\tsecretkey\x18\x01 \x01(\tR\tsecretkey\x12\x1c\n\taccesskey\x18\x02 \x01(\tR\taccesskey\"W\n\nIdentifier\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x35\n\x06idtype\x18\x02 \x01(\x0e\x32\x1d.aruna.api.internal.v1.IdTypeR\x06idtype\"\xbe\x02\n\x10\x41uthorizeRequest\x12\x45\n\x08resource\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x08resource\x12\x41\n\nidentifier\x18\x02 \x01(\x0b\x32!.aruna.api.internal.v1.IdentifierR\nidentifier\x12T\n\x0fresource_action\x18\x03 \x01(\x0e\x32+.aruna.api.storage.models.v1.ResourceActionR\x0eresourceAction\x12J\n\rauthorization\x18\x04 \x01(\x0b\x32$.aruna.api.internal.v1.AuthorizationR\rauthorization\"#\n\x11\x41uthorizeResponse\x12\x0e\n\x02ok\x18\x01 \x01(\x08R\x02ok\"0\n\x10GetSecretRequest\x12\x1c\n\taccesskey\x18\x01 \x01(\tR\taccesskey\"_\n\x11GetSecretResponse\x12J\n\rauthorization\x18\x01 \x01(\x0b\x32$.aruna.api.internal.v1.AuthorizationR\rauthorization*E\n\x06IdType\x12\x17\n\x13ID_TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cID_TYPE_UUID\x10\x01\x12\x10\n\x0cID_TYPE_PATH\x10\x02\x32\xf0\x01\n\x18InternalAuthorizeService\x12`\n\tAuthorize\x12\'.aruna.api.internal.v1.AuthorizeRequest\x1a(.aruna.api.internal.v1.AuthorizeResponse\"\x00\x12`\n\tGetSecret\x12\'.aruna.api.internal.v1.GetSecretRequest\x1a(.aruna.api.internal.v1.GetSecretResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%aruna/api/internal/v1/authorize.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a(aruna/api/storage/models/v1/models.proto\"K\n\rAuthorization\x12\x1c\n\tsecretkey\x18\x01 \x01(\tR\tsecretkey\x12\x1c\n\taccesskey\x18\x02 \x01(\tR\taccesskey\"W\n\nIdentifier\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x35\n\x06idtype\x18\x02 \x01(\x0e\x32\x1d.aruna.api.internal.v1.IdTypeR\x06idtype\"\xbe\x02\n\x10\x41uthorizeRequest\x12\x45\n\x08resource\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x08resource\x12\x41\n\nidentifier\x18\x02 \x01(\x0b\x32!.aruna.api.internal.v1.IdentifierR\nidentifier\x12T\n\x0fresource_action\x18\x03 \x01(\x0e\x32+.aruna.api.storage.models.v1.ResourceActionR\x0eresourceAction\x12J\n\rauthorization\x18\x04 \x01(\x0b\x32$.aruna.api.internal.v1.AuthorizationR\rauthorization\"#\n\x11\x41uthorizeResponse\x12\x0e\n\x02ok\x18\x01 \x01(\x08R\x02ok\"0\n\x10GetSecretRequest\x12\x1c\n\taccesskey\x18\x01 \x01(\tR\taccesskey\"_\n\x11GetSecretResponse\x12J\n\rauthorization\x18\x01 \x01(\x0b\x32$.aruna.api.internal.v1.AuthorizationR\rauthorization\"g\n\x19GetTokenFromSecretRequest\x12J\n\rauthorization\x18\x01 \x01(\x0b\x32$.aruna.api.internal.v1.AuthorizationR\rauthorization\"2\n\x1aGetTokenFromSecretResponse\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token*E\n\x06IdType\x12\x17\n\x13ID_TYPE_UNSPECIFIED\x10\x00\x12\x10\n\x0cID_TYPE_UUID\x10\x01\x12\x10\n\x0cID_TYPE_PATH\x10\x02\x32\xed\x02\n\x18InternalAuthorizeService\x12`\n\tAuthorize\x12\'.aruna.api.internal.v1.AuthorizeRequest\x1a(.aruna.api.internal.v1.AuthorizeResponse\"\x00\x12`\n\tGetSecret\x12\'.aruna.api.internal.v1.GetSecretRequest\x1a(.aruna.api.internal.v1.GetSecretResponse\"\x00\x12{\n\x12GetTokenFromSecret\x12\x30.aruna.api.internal.v1.GetTokenFromSecretRequest\x1a\x31.aruna.api.internal.v1.GetTokenFromSecretResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.internal.v1.authorize_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1'
   _INTERNALAUTHORIZESERVICE._options = None
   _INTERNALAUTHORIZESERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
-  _IDTYPE._serialized_start=806
-  _IDTYPE._serialized_end=875
+  _IDTYPE._serialized_start=963
+  _IDTYPE._serialized_end=1032
   _AUTHORIZATION._serialized_start=135
   _AUTHORIZATION._serialized_end=210
   _IDENTIFIER._serialized_start=212
   _IDENTIFIER._serialized_end=299
   _AUTHORIZEREQUEST._serialized_start=302
   _AUTHORIZEREQUEST._serialized_end=620
   _AUTHORIZERESPONSE._serialized_start=622
   _AUTHORIZERESPONSE._serialized_end=657
   _GETSECRETREQUEST._serialized_start=659
   _GETSECRETREQUEST._serialized_end=707
   _GETSECRETRESPONSE._serialized_start=709
   _GETSECRETRESPONSE._serialized_end=804
-  _INTERNALAUTHORIZESERVICE._serialized_start=878
-  _INTERNALAUTHORIZESERVICE._serialized_end=1118
+  _GETTOKENFROMSECRETREQUEST._serialized_start=806
+  _GETTOKENFROMSECRETREQUEST._serialized_end=909
+  _GETTOKENFROMSECRETRESPONSE._serialized_start=911
+  _GETTOKENFROMSECRETRESPONSE._serialized_end=961
+  _INTERNALAUTHORIZESERVICE._serialized_start=1035
+  _INTERNALAUTHORIZESERVICE._serialized_end=1400
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,26 @@
 
 class GetSecretResponse(_message.Message):
     __slots__ = ["authorization"]
     AUTHORIZATION_FIELD_NUMBER: _ClassVar[int]
     authorization: Authorization
     def __init__(self, authorization: _Optional[_Union[Authorization, _Mapping]] = ...) -> None: ...
 
+class GetTokenFromSecretRequest(_message.Message):
+    __slots__ = ["authorization"]
+    AUTHORIZATION_FIELD_NUMBER: _ClassVar[int]
+    authorization: Authorization
+    def __init__(self, authorization: _Optional[_Union[Authorization, _Mapping]] = ...) -> None: ...
+
+class GetTokenFromSecretResponse(_message.Message):
+    __slots__ = ["token"]
+    TOKEN_FIELD_NUMBER: _ClassVar[int]
+    token: str
+    def __init__(self, token: _Optional[str] = ...) -> None: ...
+
 class Identifier(_message.Message):
     __slots__ = ["idtype", "name"]
     IDTYPE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     idtype: IdType
     name: str
     def __init__(self, name: _Optional[str] = ..., idtype: _Optional[_Union[IdType, str]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.AuthorizeResponse.FromString,
                 )
         self.GetSecret = channel.unary_unary(
                 '/aruna.api.internal.v1.InternalAuthorizeService/GetSecret',
                 request_serializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretResponse.FromString,
                 )
+        self.GetTokenFromSecret = channel.unary_unary(
+                '/aruna.api.internal.v1.InternalAuthorizeService/GetTokenFromSecret',
+                request_serializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretResponse.FromString,
+                )
 
 
 class InternalAuthorizeServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Authorize(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -37,27 +42,38 @@
 
     def GetSecret(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetTokenFromSecret(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_InternalAuthorizeServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Authorize': grpc.unary_unary_rpc_method_handler(
                     servicer.Authorize,
                     request_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.AuthorizeRequest.FromString,
                     response_serializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.AuthorizeResponse.SerializeToString,
             ),
             'GetSecret': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSecret,
                     request_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretRequest.FromString,
                     response_serializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretResponse.SerializeToString,
             ),
+            'GetTokenFromSecret': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetTokenFromSecret,
+                    request_deserializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.internal.v1.InternalAuthorizeService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -93,7 +109,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/aruna.api.internal.v1.InternalAuthorizeService/GetSecret',
             aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretRequest.SerializeToString,
             aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetSecretResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetTokenFromSecret(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.internal.v1.InternalAuthorizeService/GetTokenFromSecret',
+            aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretRequest.SerializeToString,
+            aruna_dot_api_dot_internal_dot_v1_dot_authorize__pb2.GetTokenFromSecretResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.notification.services.v1 import notification_service_pb2 as aruna_dot_api_dot_notification_dot_services_dot_v1_dot_notification__service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/internal/v1/notification.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a(aruna/api/storage/models/v1/models.proto\x1a=aruna/api/notification/services/v1/notification_service.proto\"\xc0\x02\n\x0f\x45mittedResource\x12\x42\n\x07project\x18\x01 \x01(\x0b\x32&.aruna.api.internal.v1.ProjectResourceH\x00R\x07project\x12K\n\ncollection\x18\x02 \x01(\x0b\x32).aruna.api.internal.v1.CollectionResourceH\x00R\ncollection\x12?\n\x06object\x18\x03 \x01(\x0b\x32%.aruna.api.internal.v1.ObjectResourceH\x00R\x06object\x12O\n\x0cobject_group\x18\x04 \x01(\x0b\x32*.aruna.api.internal.v1.ObjectGroupResourceH\x00R\x0bobjectGroupB\n\n\x08resource\"0\n\x0fProjectResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"X\n\x12\x43ollectionResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"\x9b\x01\n\x0eObjectResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12(\n\x10shared_object_id\x18\x03 \x01(\tR\x0esharedObjectId\x12\x1b\n\tobject_id\x18\x04 \x01(\tR\x08objectId\"\xb6\x01\n\x13ObjectGroupResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x33\n\x16shared_object_group_id\x18\x03 \x01(\tR\x13sharedObjectGroupId\x12&\n\x0fobject_group_id\x18\x04 \x01(\tR\robjectGroupId\"\x99\x02\n\x10\x45mitEventRequest\x12P\n\x0e\x65vent_resource\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\reventResource\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\x12L\n\nevent_type\x18\x03 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12\x44\n\tresources\x18\x04 \x03(\x0b\x32&.aruna.api.internal.v1.EmittedResourceR\tresources\"\x13\n\x11\x45mitEventResponse\"\x91\x02\n\x0bStreamGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12L\n\nevent_type\x18\x02 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12N\n\rresource_type\x18\x03 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x04 \x01(\tR\nresourceId\x12\x33\n\x16notify_on_sub_resource\x18\x05 \x01(\x08R\x13notifyOnSubResource\"\xa4\x02\n\x18\x43reateStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12L\n\nevent_type\x18\x02 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12N\n\rresource_type\x18\x03 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x04 \x01(\tR\nresourceId\x12\x33\n\x16notify_on_sub_resource\x18\x05 \x01(\x08R\x13notifyOnSubResource\"b\n\x19\x43reateStreamGroupResponse\x12\x45\n\x0cstream_group\x18\x01 \x01(\x0b\x32\".aruna.api.internal.v1.StreamGroupR\x0bstreamGroup\"U\n\x15GetStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12&\n\x0fstream_group_id\x18\x02 \x01(\tR\rstreamGroupId\"_\n\x16GetStreamGroupResponse\x12\x45\n\x0cstream_group\x18\x01 \x01(\x0b\x32\".aruna.api.internal.v1.StreamGroupR\x0bstreamGroup\"X\n\x18\x44\x65leteStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12&\n\x0fstream_group_id\x18\x02 \x01(\tR\rstreamGroupId\"\x1b\n\x19\x44\x65leteStreamGroupResponse\"\x8b\x01\n\x18GetSharedRevisionRequest\x12N\n\rresource_type\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\"I\n\x19GetSharedRevisionResponse\x12,\n\x12shared_revision_id\x18\x01 \x01(\tR\x10sharedRevisionId2\x91\x01\n\x1bInternalEventEmitterService\x12`\n\tEmitEvent\x12\'.aruna.api.internal.v1.EmitEventRequest\x1a(.aruna.api.internal.v1.EmitEventResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\x87\x04\n\x14InternalEventService\x12x\n\x11\x43reateStreamGroup\x12/.aruna.api.internal.v1.CreateStreamGroupRequest\x1a\x30.aruna.api.internal.v1.CreateStreamGroupResponse\"\x00\x12o\n\x0eGetStreamGroup\x12,.aruna.api.internal.v1.GetStreamGroupRequest\x1a-.aruna.api.internal.v1.GetStreamGroupResponse\"\x00\x12x\n\x11\x44\x65leteStreamGroup\x12/.aruna.api.internal.v1.DeleteStreamGroupRequest\x1a\x30.aruna.api.internal.v1.DeleteStreamGroupResponse\"\x00\x12x\n\x11GetSharedRevision\x12/.aruna.api.internal.v1.GetSharedRevisionRequest\x1a\x30.aruna.api.internal.v1.GetSharedRevisionResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/internal/v1/notification.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a(aruna/api/storage/models/v1/models.proto\x1a=aruna/api/notification/services/v1/notification_service.proto\"\xc0\x02\n\x0f\x45mittedResource\x12\x42\n\x07project\x18\x01 \x01(\x0b\x32&.aruna.api.internal.v1.ProjectResourceH\x00R\x07project\x12K\n\ncollection\x18\x02 \x01(\x0b\x32).aruna.api.internal.v1.CollectionResourceH\x00R\ncollection\x12?\n\x06object\x18\x03 \x01(\x0b\x32%.aruna.api.internal.v1.ObjectResourceH\x00R\x06object\x12O\n\x0cobject_group\x18\x04 \x01(\x0b\x32*.aruna.api.internal.v1.ObjectGroupResourceH\x00R\x0bobjectGroupB\n\n\x08resource\"0\n\x0fProjectResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"X\n\x12\x43ollectionResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"\x9b\x01\n\x0eObjectResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12(\n\x10shared_object_id\x18\x03 \x01(\tR\x0esharedObjectId\x12\x1b\n\tobject_id\x18\x04 \x01(\tR\x08objectId\"\xb6\x01\n\x13ObjectGroupResource\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x33\n\x16shared_object_group_id\x18\x03 \x01(\tR\x13sharedObjectGroupId\x12&\n\x0fobject_group_id\x18\x04 \x01(\tR\robjectGroupId\"\x99\x02\n\x10\x45mitEventRequest\x12P\n\x0e\x65vent_resource\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\reventResource\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\x12L\n\nevent_type\x18\x03 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12\x44\n\tresources\x18\x04 \x03(\x0b\x32&.aruna.api.internal.v1.EmittedResourceR\tresources\"\x13\n\x11\x45mitEventResponse\"\x91\x02\n\x0bStreamGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12L\n\nevent_type\x18\x02 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12N\n\rresource_type\x18\x03 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x04 \x01(\tR\nresourceId\x12\x33\n\x16notify_on_sub_resource\x18\x05 \x01(\x08R\x13notifyOnSubResource\"\xbe\x02\n\x18\x43reateStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12L\n\nevent_type\x18\x02 \x01(\x0e\x32-.aruna.api.notification.services.v1.EventTypeR\teventType\x12N\n\rresource_type\x18\x03 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x04 \x01(\tR\nresourceId\x12\x33\n\x16notify_on_sub_resource\x18\x05 \x01(\x08R\x13notifyOnSubResource\x12\x18\n\x07subject\x18\x06 \x01(\tR\x07subject\"b\n\x19\x43reateStreamGroupResponse\x12\x45\n\x0cstream_group\x18\x01 \x01(\x0b\x32\".aruna.api.internal.v1.StreamGroupR\x0bstreamGroup\"U\n\x15GetStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12&\n\x0fstream_group_id\x18\x02 \x01(\tR\rstreamGroupId\"_\n\x16GetStreamGroupResponse\x12\x45\n\x0cstream_group\x18\x01 \x01(\x0b\x32\".aruna.api.internal.v1.StreamGroupR\x0bstreamGroup\"X\n\x18\x44\x65leteStreamGroupRequest\x12\x14\n\x05token\x18\x01 \x01(\tR\x05token\x12&\n\x0fstream_group_id\x18\x02 \x01(\tR\rstreamGroupId\"\x1b\n\x19\x44\x65leteStreamGroupResponse\"\x8b\x01\n\x18GetSharedRevisionRequest\x12N\n\rresource_type\x18\x01 \x01(\x0e\x32).aruna.api.storage.models.v1.ResourceTypeR\x0cresourceType\x12\x1f\n\x0bresource_id\x18\x02 \x01(\tR\nresourceId\"I\n\x19GetSharedRevisionResponse\x12,\n\x12shared_revision_id\x18\x01 \x01(\tR\x10sharedRevisionId2\x91\x01\n\x1bInternalEventEmitterService\x12`\n\tEmitEvent\x12\'.aruna.api.internal.v1.EmitEventRequest\x1a(.aruna.api.internal.v1.EmitEventResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\x87\x04\n\x14InternalEventService\x12x\n\x11\x43reateStreamGroup\x12/.aruna.api.internal.v1.CreateStreamGroupRequest\x1a\x30.aruna.api.internal.v1.CreateStreamGroupResponse\"\x00\x12o\n\x0eGetStreamGroup\x12,.aruna.api.internal.v1.GetStreamGroupRequest\x1a-.aruna.api.internal.v1.GetStreamGroupResponse\"\x00\x12x\n\x11\x44\x65leteStreamGroup\x12/.aruna.api.internal.v1.DeleteStreamGroupRequest\x1a\x30.aruna.api.internal.v1.DeleteStreamGroupResponse\"\x00\x12x\n\x11GetSharedRevision\x12/.aruna.api.internal.v1.GetSharedRevisionRequest\x1a\x30.aruna.api.internal.v1.GetSharedRevisionResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.internal.v1.notification_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1'
@@ -41,27 +41,27 @@
   _EMITEVENTREQUEST._serialized_start=1008
   _EMITEVENTREQUEST._serialized_end=1289
   _EMITEVENTRESPONSE._serialized_start=1291
   _EMITEVENTRESPONSE._serialized_end=1310
   _STREAMGROUP._serialized_start=1313
   _STREAMGROUP._serialized_end=1586
   _CREATESTREAMGROUPREQUEST._serialized_start=1589
-  _CREATESTREAMGROUPREQUEST._serialized_end=1881
-  _CREATESTREAMGROUPRESPONSE._serialized_start=1883
-  _CREATESTREAMGROUPRESPONSE._serialized_end=1981
-  _GETSTREAMGROUPREQUEST._serialized_start=1983
-  _GETSTREAMGROUPREQUEST._serialized_end=2068
-  _GETSTREAMGROUPRESPONSE._serialized_start=2070
-  _GETSTREAMGROUPRESPONSE._serialized_end=2165
-  _DELETESTREAMGROUPREQUEST._serialized_start=2167
-  _DELETESTREAMGROUPREQUEST._serialized_end=2255
-  _DELETESTREAMGROUPRESPONSE._serialized_start=2257
-  _DELETESTREAMGROUPRESPONSE._serialized_end=2284
-  _GETSHAREDREVISIONREQUEST._serialized_start=2287
-  _GETSHAREDREVISIONREQUEST._serialized_end=2426
-  _GETSHAREDREVISIONRESPONSE._serialized_start=2428
-  _GETSHAREDREVISIONRESPONSE._serialized_end=2501
-  _INTERNALEVENTEMITTERSERVICE._serialized_start=2504
-  _INTERNALEVENTEMITTERSERVICE._serialized_end=2649
-  _INTERNALEVENTSERVICE._serialized_start=2652
-  _INTERNALEVENTSERVICE._serialized_end=3171
+  _CREATESTREAMGROUPREQUEST._serialized_end=1907
+  _CREATESTREAMGROUPRESPONSE._serialized_start=1909
+  _CREATESTREAMGROUPRESPONSE._serialized_end=2007
+  _GETSTREAMGROUPREQUEST._serialized_start=2009
+  _GETSTREAMGROUPREQUEST._serialized_end=2094
+  _GETSTREAMGROUPRESPONSE._serialized_start=2096
+  _GETSTREAMGROUPRESPONSE._serialized_end=2191
+  _DELETESTREAMGROUPREQUEST._serialized_start=2193
+  _DELETESTREAMGROUPREQUEST._serialized_end=2281
+  _DELETESTREAMGROUPRESPONSE._serialized_start=2283
+  _DELETESTREAMGROUPRESPONSE._serialized_end=2310
+  _GETSHAREDREVISIONREQUEST._serialized_start=2313
+  _GETSHAREDREVISIONREQUEST._serialized_end=2452
+  _GETSHAREDREVISIONRESPONSE._serialized_start=2454
+  _GETSHAREDREVISIONRESPONSE._serialized_end=2527
+  _INTERNALEVENTEMITTERSERVICE._serialized_start=2530
+  _INTERNALEVENTEMITTERSERVICE._serialized_end=2675
+  _INTERNALEVENTSERVICE._serialized_start=2678
+  _INTERNALEVENTSERVICE._serialized_end=3197
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,28 @@
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
     project_id: str
     def __init__(self, project_id: _Optional[str] = ..., collection_id: _Optional[str] = ...) -> None: ...
 
 class CreateStreamGroupRequest(_message.Message):
-    __slots__ = ["event_type", "notify_on_sub_resource", "resource_id", "resource_type", "token"]
+    __slots__ = ["event_type", "notify_on_sub_resource", "resource_id", "resource_type", "subject", "token"]
     EVENT_TYPE_FIELD_NUMBER: _ClassVar[int]
     NOTIFY_ON_SUB_RESOURCE_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_ID_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_TYPE_FIELD_NUMBER: _ClassVar[int]
+    SUBJECT_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     event_type: _notification_service_pb2.EventType
     notify_on_sub_resource: bool
     resource_id: str
     resource_type: _models_pb2.ResourceType
+    subject: str
     token: str
-    def __init__(self, token: _Optional[str] = ..., event_type: _Optional[_Union[_notification_service_pb2.EventType, str]] = ..., resource_type: _Optional[_Union[_models_pb2.ResourceType, str]] = ..., resource_id: _Optional[str] = ..., notify_on_sub_resource: bool = ...) -> None: ...
+    def __init__(self, token: _Optional[str] = ..., event_type: _Optional[_Union[_notification_service_pb2.EventType, str]] = ..., resource_type: _Optional[_Union[_models_pb2.ResourceType, str]] = ..., resource_id: _Optional[str] = ..., notify_on_sub_resource: bool = ..., subject: _Optional[str] = ...) -> None: ...
 
 class CreateStreamGroupResponse(_message.Message):
     __slots__ = ["stream_group"]
     STREAM_GROUP_FIELD_NUMBER: _ClassVar[int]
     stream_group: StreamGroup
     def __init__(self, stream_group: _Optional[_Union[StreamGroup, _Mapping]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.storage.services.v1 import object_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v1_dot_object__service__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!aruna/api/internal/v1/proxy.proto\x12\x15\x61runa.api.internal.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x32\x61runa/api/storage/services/v1/object_service.proto\x1a\x1bgoogle/api/visibility.proto\"\xff\x01\n\x08Location\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32#.aruna.api.internal.v1.LocationTypeR\x04type\x12\x16\n\x06\x62ucket\x18\x02 \x01(\tR\x06\x62ucket\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\x12#\n\ris_compressed\x18\x05 \x01(\x08R\x0cisCompressed\x12!\n\x0cis_encrypted\x18\x06 \x01(\x08R\x0bisEncrypted\x12%\n\x0e\x65ncryption_key\x18\x07 \x01(\tR\rencryptionKey\"?\n\x08PartETag\x12\x1f\n\x0bpart_number\x18\x01 \x01(\x03R\npartNumber\x12\x12\n\x04\x65tag\x18\x02 \x01(\tR\x04\x65tag\"r\n\x1aInitMultipartUploadRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\":\n\x1bInitMultipartUploadResponse\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\"\xd1\x01\n\x1c\x46inishMultipartUploadRequest\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x03 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x04 \x01(\tR\x0c\x63ollectionId\x12>\n\npart_etags\x18\x05 \x03(\x0b\x32\x1f.aruna.api.internal.v1.PartETagR\tpartEtags\"\x1f\n\x1d\x46inishMultipartUploadResponse\"R\n\x13\x44\x65leteObjectRequest\x12;\n\x08location\x18\x01 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"\x16\n\x14\x44\x65leteObjectResponse\"\xf8\x01\n\x15\x46inalizeObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12;\n\x08location\x18\x03 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12%\n\x0e\x63ontent_length\x18\x05 \x01(\x03R\rcontentLength\"\x18\n\x16\x46inalizeObjectResponse\"j\n\x1fGetOrCreateEncryptionKeyRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x1f\n\x0b\x65ndpoint_id\x18\x03 \x01(\tR\nendpointId\"c\n GetOrCreateEncryptionKeyResponse\x12%\n\x0e\x65ncryption_key\x18\x01 \x01(\tR\rencryptionKey\x12\x18\n\x07\x63reated\x18\x02 \x01(\x08R\x07\x63reated\"\xd3\x01\n\x1eGetOrCreateObjectByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x19\n\x08get_only\x18\x04 \x01(\x08R\x07getOnly\x12\x1f\n\x0b\x65ndpoint_id\x18\x05 \x01(\tR\nendpointId\"\xa7\x02\n\x1fGetOrCreateObjectByPathResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x44\n\tdataclass\x18\x03 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\'\n\x0frevision_number\x18\x05 \x01(\x03R\x0erevisionNumber\x12\x18\n\x07\x63reated\x18\x06 \x01(\x08R\x07\x63reated\"\x8f\x01\n\x18GetObjectLocationRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1f\n\x0brevision_id\x18\x02 \x01(\tR\nrevisionId\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\"\x95\x01\n\x19GetObjectLocationResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12;\n\x08location\x18\x02 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"U\n\x1cGetCollectionByBucketRequest\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\"c\n\x1dGetCollectionByBucketResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId*[\n\x0cLocationType\x12\x1d\n\x19LOCATION_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10LOCATION_TYPE_S3\x10\x01\x12\x16\n\x12LOCATION_TYPE_FILE\x10\x02\x32\x9a\x03\n\x14InternalProxyService\x12~\n\x13InitMultipartUpload\x12\x31.aruna.api.internal.v1.InitMultipartUploadRequest\x1a\x32.aruna.api.internal.v1.InitMultipartUploadResponse\"\x00\x12\x84\x01\n\x15\x46inishMultipartUpload\x12\x33.aruna.api.internal.v1.FinishMultipartUploadRequest\x1a\x34.aruna.api.internal.v1.FinishMultipartUploadResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.aruna.api.internal.v1.DeleteObjectRequest\x1a+.aruna.api.internal.v1.DeleteObjectResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\xbf\x05\n\x1cInternalProxyNotifierService\x12\x8a\x01\n\x17GetOrCreateObjectByPath\x12\x35.aruna.api.internal.v1.GetOrCreateObjectByPathRequest\x1a\x36.aruna.api.internal.v1.GetOrCreateObjectByPathResponse\"\x00\x12o\n\x0e\x46inalizeObject\x12,.aruna.api.internal.v1.FinalizeObjectRequest\x1a-.aruna.api.internal.v1.FinalizeObjectResponse\"\x00\x12\x8d\x01\n\x18GetOrCreateEncryptionKey\x12\x36.aruna.api.internal.v1.GetOrCreateEncryptionKeyRequest\x1a\x37.aruna.api.internal.v1.GetOrCreateEncryptionKeyResponse\"\x00\x12x\n\x11GetObjectLocation\x12/.aruna.api.internal.v1.GetObjectLocationRequest\x1a\x30.aruna.api.internal.v1.GetObjectLocationResponse\"\x00\x12\x84\x01\n\x15GetCollectionByBucket\x12\x33.aruna.api.internal.v1.GetCollectionByBucketRequest\x1a\x34.aruna.api.internal.v1.GetCollectionByBucketResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!aruna/api/internal/v1/proxy.proto\x12\x15\x61runa.api.internal.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x32\x61runa/api/storage/services/v1/object_service.proto\x1a\x1bgoogle/api/visibility.proto\"\xff\x01\n\x08Location\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32#.aruna.api.internal.v1.LocationTypeR\x04type\x12\x16\n\x06\x62ucket\x18\x02 \x01(\tR\x06\x62ucket\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\x12#\n\ris_compressed\x18\x05 \x01(\x08R\x0cisCompressed\x12!\n\x0cis_encrypted\x18\x06 \x01(\x08R\x0bisEncrypted\x12%\n\x0e\x65ncryption_key\x18\x07 \x01(\tR\rencryptionKey\"?\n\x08PartETag\x12\x1f\n\x0bpart_number\x18\x01 \x01(\x03R\npartNumber\x12\x12\n\x04\x65tag\x18\x02 \x01(\tR\x04\x65tag\"r\n\x1aInitMultipartUploadRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\":\n\x1bInitMultipartUploadResponse\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\"\xd1\x01\n\x1c\x46inishMultipartUploadRequest\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x03 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x04 \x01(\tR\x0c\x63ollectionId\x12>\n\npart_etags\x18\x05 \x03(\x0b\x32\x1f.aruna.api.internal.v1.PartETagR\tpartEtags\"\x1f\n\x1d\x46inishMultipartUploadResponse\"R\n\x13\x44\x65leteObjectRequest\x12;\n\x08location\x18\x01 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"\x16\n\x14\x44\x65leteObjectResponse\"\xf8\x01\n\x15\x46inalizeObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12;\n\x08location\x18\x03 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12%\n\x0e\x63ontent_length\x18\x05 \x01(\x03R\rcontentLength\"\x18\n\x16\x46inalizeObjectResponse\"j\n\x1fGetOrCreateEncryptionKeyRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x1f\n\x0b\x65ndpoint_id\x18\x03 \x01(\tR\nendpointId\"c\n GetOrCreateEncryptionKeyResponse\x12%\n\x0e\x65ncryption_key\x18\x01 \x01(\tR\rencryptionKey\x12\x18\n\x07\x63reated\x18\x02 \x01(\x08R\x07\x63reated\"\xd3\x01\n\x1eGetOrCreateObjectByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x19\n\x08get_only\x18\x04 \x01(\x08R\x07getOnly\x12\x1f\n\x0b\x65ndpoint_id\x18\x05 \x01(\tR\nendpointId\"\xa7\x02\n\x1fGetOrCreateObjectByPathResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x44\n\tdataclass\x18\x03 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\'\n\x0frevision_number\x18\x05 \x01(\x03R\x0erevisionNumber\x12\x18\n\x07\x63reated\x18\x06 \x01(\x08R\x07\x63reated\"\x8f\x01\n\x18GetObjectLocationRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1f\n\x0brevision_id\x18\x02 \x01(\tR\nrevisionId\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\"\x87\x01\n\nCORSConfig\x12\'\n\x0f\x61llowed_methods\x18\x01 \x03(\tR\x0e\x61llowedMethods\x12\'\n\x0f\x61llowed_origins\x18\x02 \x03(\tR\x0e\x61llowedOrigins\x12\'\n\x0f\x61llowed_headers\x18\x03 \x03(\tR\x0e\x61llowedHeaders\"\xe9\x01\n\x19GetObjectLocationResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12;\n\x08location\x18\x02 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\x12R\n\x13\x63ors_configurations\x18\x03 \x03(\x0b\x32!.aruna.api.internal.v1.CORSConfigR\x12\x63orsConfigurations\"U\n\x1cGetCollectionByBucketRequest\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\"c\n\x1dGetCollectionByBucketResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId*[\n\x0cLocationType\x12\x1d\n\x19LOCATION_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10LOCATION_TYPE_S3\x10\x01\x12\x16\n\x12LOCATION_TYPE_FILE\x10\x02\x32\x9a\x03\n\x14InternalProxyService\x12~\n\x13InitMultipartUpload\x12\x31.aruna.api.internal.v1.InitMultipartUploadRequest\x1a\x32.aruna.api.internal.v1.InitMultipartUploadResponse\"\x00\x12\x84\x01\n\x15\x46inishMultipartUpload\x12\x33.aruna.api.internal.v1.FinishMultipartUploadRequest\x1a\x34.aruna.api.internal.v1.FinishMultipartUploadResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.aruna.api.internal.v1.DeleteObjectRequest\x1a+.aruna.api.internal.v1.DeleteObjectResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\xbf\x05\n\x1cInternalProxyNotifierService\x12\x8a\x01\n\x17GetOrCreateObjectByPath\x12\x35.aruna.api.internal.v1.GetOrCreateObjectByPathRequest\x1a\x36.aruna.api.internal.v1.GetOrCreateObjectByPathResponse\"\x00\x12o\n\x0e\x46inalizeObject\x12,.aruna.api.internal.v1.FinalizeObjectRequest\x1a-.aruna.api.internal.v1.FinalizeObjectResponse\"\x00\x12\x8d\x01\n\x18GetOrCreateEncryptionKey\x12\x36.aruna.api.internal.v1.GetOrCreateEncryptionKeyRequest\x1a\x37.aruna.api.internal.v1.GetOrCreateEncryptionKeyResponse\"\x00\x12x\n\x11GetObjectLocation\x12/.aruna.api.internal.v1.GetObjectLocationRequest\x1a\x30.aruna.api.internal.v1.GetObjectLocationResponse\"\x00\x12\x84\x01\n\x15GetCollectionByBucket\x12\x33.aruna.api.internal.v1.GetCollectionByBucketRequest\x1a\x34.aruna.api.internal.v1.GetCollectionByBucketResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.internal.v1.proxy_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1'
   _INTERNALPROXYSERVICE._options = None
   _INTERNALPROXYSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
   _INTERNALPROXYNOTIFIERSERVICE._options = None
   _INTERNALPROXYNOTIFIERSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
-  _LOCATIONTYPE._serialized_start=2519
-  _LOCATIONTYPE._serialized_end=2610
+  _LOCATIONTYPE._serialized_start=2741
+  _LOCATIONTYPE._serialized_end=2832
   _LOCATION._serialized_start=184
   _LOCATION._serialized_end=439
   _PARTETAG._serialized_start=441
   _PARTETAG._serialized_end=504
   _INITMULTIPARTUPLOADREQUEST._serialized_start=506
   _INITMULTIPARTUPLOADREQUEST._serialized_end=620
   _INITMULTIPARTUPLOADRESPONSE._serialized_start=622
@@ -56,18 +56,20 @@
   _GETORCREATEENCRYPTIONKEYRESPONSE._serialized_end=1519
   _GETORCREATEOBJECTBYPATHREQUEST._serialized_start=1522
   _GETORCREATEOBJECTBYPATHREQUEST._serialized_end=1733
   _GETORCREATEOBJECTBYPATHRESPONSE._serialized_start=1736
   _GETORCREATEOBJECTBYPATHRESPONSE._serialized_end=2031
   _GETOBJECTLOCATIONREQUEST._serialized_start=2034
   _GETOBJECTLOCATIONREQUEST._serialized_end=2177
-  _GETOBJECTLOCATIONRESPONSE._serialized_start=2180
-  _GETOBJECTLOCATIONRESPONSE._serialized_end=2329
-  _GETCOLLECTIONBYBUCKETREQUEST._serialized_start=2331
-  _GETCOLLECTIONBYBUCKETREQUEST._serialized_end=2416
-  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_start=2418
-  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_end=2517
-  _INTERNALPROXYSERVICE._serialized_start=2613
-  _INTERNALPROXYSERVICE._serialized_end=3023
-  _INTERNALPROXYNOTIFIERSERVICE._serialized_start=3026
-  _INTERNALPROXYNOTIFIERSERVICE._serialized_end=3729
+  _CORSCONFIG._serialized_start=2180
+  _CORSCONFIG._serialized_end=2315
+  _GETOBJECTLOCATIONRESPONSE._serialized_start=2318
+  _GETOBJECTLOCATIONRESPONSE._serialized_end=2551
+  _GETCOLLECTIONBYBUCKETREQUEST._serialized_start=2553
+  _GETCOLLECTIONBYBUCKETREQUEST._serialized_end=2638
+  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_start=2640
+  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_end=2739
+  _INTERNALPROXYSERVICE._serialized_start=2835
+  _INTERNALPROXYSERVICE._serialized_end=3245
+  _INTERNALPROXYNOTIFIERSERVICE._serialized_start=3248
+  _INTERNALPROXYNOTIFIERSERVICE._serialized_end=3951
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,24 @@
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 LOCATION_TYPE_FILE: LocationType
 LOCATION_TYPE_S3: LocationType
 LOCATION_TYPE_UNSPECIFIED: LocationType
 
+class CORSConfig(_message.Message):
+    __slots__ = ["allowed_headers", "allowed_methods", "allowed_origins"]
+    ALLOWED_HEADERS_FIELD_NUMBER: _ClassVar[int]
+    ALLOWED_METHODS_FIELD_NUMBER: _ClassVar[int]
+    ALLOWED_ORIGINS_FIELD_NUMBER: _ClassVar[int]
+    allowed_headers: _containers.RepeatedScalarFieldContainer[str]
+    allowed_methods: _containers.RepeatedScalarFieldContainer[str]
+    allowed_origins: _containers.RepeatedScalarFieldContainer[str]
+    def __init__(self, allowed_methods: _Optional[_Iterable[str]] = ..., allowed_origins: _Optional[_Iterable[str]] = ..., allowed_headers: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class DeleteObjectRequest(_message.Message):
     __slots__ = ["location"]
     LOCATION_FIELD_NUMBER: _ClassVar[int]
     location: Location
     def __init__(self, location: _Optional[_Union[Location, _Mapping]] = ...) -> None: ...
 
 class DeleteObjectResponse(_message.Message):
@@ -83,20 +93,22 @@
     access_key: str
     endpoint_id: str
     path: str
     revision_id: str
     def __init__(self, path: _Optional[str] = ..., revision_id: _Optional[str] = ..., access_key: _Optional[str] = ..., endpoint_id: _Optional[str] = ...) -> None: ...
 
 class GetObjectLocationResponse(_message.Message):
-    __slots__ = ["location", "object"]
+    __slots__ = ["cors_configurations", "location", "object"]
+    CORS_CONFIGURATIONS_FIELD_NUMBER: _ClassVar[int]
     LOCATION_FIELD_NUMBER: _ClassVar[int]
     OBJECT_FIELD_NUMBER: _ClassVar[int]
+    cors_configurations: _containers.RepeatedCompositeFieldContainer[CORSConfig]
     location: Location
     object: _models_pb2.Object
-    def __init__(self, object: _Optional[_Union[_models_pb2.Object, _Mapping]] = ..., location: _Optional[_Union[Location, _Mapping]] = ...) -> None: ...
+    def __init__(self, object: _Optional[_Union[_models_pb2.Object, _Mapping]] = ..., location: _Optional[_Union[Location, _Mapping]] = ..., cors_configurations: _Optional[_Iterable[_Union[CORSConfig, _Mapping]]] = ...) -> None: ...
 
 class GetOrCreateEncryptionKeyRequest(_message.Message):
     __slots__ = ["endpoint_id", "hash", "path"]
     ENDPOINT_ID_FIELD_NUMBER: _ClassVar[int]
     HASH_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
     endpoint_id: str
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/models_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.1*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.2*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.1*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.2*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
```

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc2/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc1/setup.py` & `Aruna-Python-API-1.1.0rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.1.0-rc.1",
+    version="1.1.0-rc.2",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

