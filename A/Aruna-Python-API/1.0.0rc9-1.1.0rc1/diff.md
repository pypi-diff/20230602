# Comparing `tmp/Aruna-Python-API-1.0.0rc9.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.0.0rc9.tar", last modified: Thu Mar 16 14:03:43 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc1.tar", last modified: Fri Jun  2 08:49:14 2023, max compression
```

## Comparing `Aruna-Python-API-1.0.0rc9.tar` & `Aruna-Python-API-1.1.0rc1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.702358 Aruna-Python-API-1.0.0rc9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.694357 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-16 14:03:43.000000 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-03-16 14:03:43.000000 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:03:43.000000 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-16 14:03:43.000000 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 14:03:43.000000 Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-16 14:03:43.702358 Aruna-Python-API-1.0.0rc9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.694357 Aruna-Python-API-1.0.0rc9/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.694357 Aruna-Python-API-1.0.0rc9/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.694357 Aruna-Python-API-1.0.0rc9/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19733 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.698357 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:43.702358 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 14:03:17.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29817 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23315 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19904 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23300 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-16 14:03:43.702358 Aruna-Python-API-1.0.0rc9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-16 14:03:30.000000 Aruna-Python-API-1.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:49:14.000000 Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.451830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.455830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:48:29.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29783 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23232 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 08:49:14.459830 Aruna-Python-API-1.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-02 08:48:43.000000 Aruna-Python-API-1.1.0rc1/setup.py
```

### Comparing `Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.0.0rc9
+Version: 1.1.0rc1
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.0.0rc9/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc1/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/LICENSE` & `Aruna-Python-API-1.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/PKG-INFO` & `Aruna-Python-API-1.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.0.0rc9
+Version: 1.1.0rc1
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.0.0rc9/README.md` & `Aruna-Python-API-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,62 +12,62 @@
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.storage.services.v1 import object_service_pb2 as aruna_dot_api_dot_storage_dot_services_dot_v1_dot_object__service__pb2
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!aruna/api/internal/v1/proxy.proto\x12\x15\x61runa.api.internal.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x32\x61runa/api/storage/services/v1/object_service.proto\x1a\x1bgoogle/api/visibility.proto\"\xff\x01\n\x08Location\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32#.aruna.api.internal.v1.LocationTypeR\x04type\x12\x16\n\x06\x62ucket\x18\x02 \x01(\tR\x06\x62ucket\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\x12#\n\ris_compressed\x18\x05 \x01(\x08R\x0cisCompressed\x12!\n\x0cis_encrypted\x18\x06 \x01(\x08R\x0bisEncrypted\x12%\n\x0e\x65ncryption_key\x18\x07 \x01(\tR\rencryptionKey\"?\n\x08PartETag\x12\x1f\n\x0bpart_number\x18\x01 \x01(\x03R\npartNumber\x12\x12\n\x04\x65tag\x18\x02 \x01(\tR\x04\x65tag\"0\n\x1aInitMultipartUploadRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\":\n\x1bInitMultipartUploadResponse\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\"\x8f\x01\n\x1c\x46inishMultipartUploadRequest\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12>\n\npart_etags\x18\x03 \x03(\x0b\x32\x1f.aruna.api.internal.v1.PartETagR\tpartEtags\"\x1f\n\x1d\x46inishMultipartUploadResponse\"R\n\x13\x44\x65leteObjectRequest\x12;\n\x08location\x18\x01 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"\x16\n\x14\x44\x65leteObjectResponse\"\xf8\x01\n\x15\x46inalizeObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12;\n\x08location\x18\x03 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12%\n\x0e\x63ontent_length\x18\x05 \x01(\x03R\rcontentLength\"\x18\n\x16\x46inalizeObjectResponse\"j\n\x1fGetOrCreateEncryptionKeyRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x1f\n\x0b\x65ndpoint_id\x18\x03 \x01(\tR\nendpointId\"c\n GetOrCreateEncryptionKeyResponse\x12%\n\x0e\x65ncryption_key\x18\x01 \x01(\tR\rencryptionKey\x12\x18\n\x07\x63reated\x18\x02 \x01(\x08R\x07\x63reated\"\x97\x01\n\x1eGetOrCreateObjectByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\"\xa7\x02\n\x1fGetOrCreateObjectByPathResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x44\n\tdataclass\x18\x03 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\'\n\x0frevision_number\x18\x05 \x01(\x03R\x0erevisionNumber\x12\x18\n\x07\x63reated\x18\x06 \x01(\x08R\x07\x63reated\"\x8f\x01\n\x18GetObjectLocationRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1f\n\x0brevision_id\x18\x02 \x01(\tR\nrevisionId\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\"\x95\x01\n\x19GetObjectLocationResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12;\n\x08location\x18\x02 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"U\n\x1cGetCollectionByBucketRequest\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\"c\n\x1dGetCollectionByBucketResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId*[\n\x0cLocationType\x12\x1d\n\x19LOCATION_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10LOCATION_TYPE_S3\x10\x01\x12\x16\n\x12LOCATION_TYPE_FILE\x10\x02\x32\x9a\x03\n\x14InternalProxyService\x12~\n\x13InitMultipartUpload\x12\x31.aruna.api.internal.v1.InitMultipartUploadRequest\x1a\x32.aruna.api.internal.v1.InitMultipartUploadResponse\"\x00\x12\x84\x01\n\x15\x46inishMultipartUpload\x12\x33.aruna.api.internal.v1.FinishMultipartUploadRequest\x1a\x34.aruna.api.internal.v1.FinishMultipartUploadResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.aruna.api.internal.v1.DeleteObjectRequest\x1a+.aruna.api.internal.v1.DeleteObjectResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\xbf\x05\n\x1cInternalProxyNotifierService\x12\x8a\x01\n\x17GetOrCreateObjectByPath\x12\x35.aruna.api.internal.v1.GetOrCreateObjectByPathRequest\x1a\x36.aruna.api.internal.v1.GetOrCreateObjectByPathResponse\"\x00\x12o\n\x0e\x46inalizeObject\x12,.aruna.api.internal.v1.FinalizeObjectRequest\x1a-.aruna.api.internal.v1.FinalizeObjectResponse\"\x00\x12\x8d\x01\n\x18GetOrCreateEncryptionKey\x12\x36.aruna.api.internal.v1.GetOrCreateEncryptionKeyRequest\x1a\x37.aruna.api.internal.v1.GetOrCreateEncryptionKeyResponse\"\x00\x12x\n\x11GetObjectLocation\x12/.aruna.api.internal.v1.GetObjectLocationRequest\x1a\x30.aruna.api.internal.v1.GetObjectLocationResponse\"\x00\x12\x84\x01\n\x15GetCollectionByBucket\x12\x33.aruna.api.internal.v1.GetCollectionByBucketRequest\x1a\x34.aruna.api.internal.v1.GetCollectionByBucketResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!aruna/api/internal/v1/proxy.proto\x12\x15\x61runa.api.internal.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x32\x61runa/api/storage/services/v1/object_service.proto\x1a\x1bgoogle/api/visibility.proto\"\xff\x01\n\x08Location\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32#.aruna.api.internal.v1.LocationTypeR\x04type\x12\x16\n\x06\x62ucket\x18\x02 \x01(\tR\x06\x62ucket\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\x12#\n\ris_compressed\x18\x05 \x01(\x08R\x0cisCompressed\x12!\n\x0cis_encrypted\x18\x06 \x01(\x08R\x0bisEncrypted\x12%\n\x0e\x65ncryption_key\x18\x07 \x01(\tR\rencryptionKey\"?\n\x08PartETag\x12\x1f\n\x0bpart_number\x18\x01 \x01(\x03R\npartNumber\x12\x12\n\x04\x65tag\x18\x02 \x01(\tR\x04\x65tag\"r\n\x1aInitMultipartUploadRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\":\n\x1bInitMultipartUploadResponse\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\"\xd1\x01\n\x1c\x46inishMultipartUploadRequest\x12\x1b\n\tupload_id\x18\x01 \x01(\tR\x08uploadId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1b\n\tobject_id\x18\x03 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x04 \x01(\tR\x0c\x63ollectionId\x12>\n\npart_etags\x18\x05 \x03(\x0b\x32\x1f.aruna.api.internal.v1.PartETagR\tpartEtags\"\x1f\n\x1d\x46inishMultipartUploadResponse\"R\n\x13\x44\x65leteObjectRequest\x12;\n\x08location\x18\x01 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"\x16\n\x14\x44\x65leteObjectResponse\"\xf8\x01\n\x15\x46inalizeObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12;\n\x08location\x18\x03 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12%\n\x0e\x63ontent_length\x18\x05 \x01(\x03R\rcontentLength\"\x18\n\x16\x46inalizeObjectResponse\"j\n\x1fGetOrCreateEncryptionKeyRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\x12\x1f\n\x0b\x65ndpoint_id\x18\x03 \x01(\tR\nendpointId\"c\n GetOrCreateEncryptionKeyResponse\x12%\n\x0e\x65ncryption_key\x18\x01 \x01(\tR\rencryptionKey\x12\x18\n\x07\x63reated\x18\x02 \x01(\x08R\x07\x63reated\"\xd3\x01\n\x1eGetOrCreateObjectByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x19\n\x08get_only\x18\x04 \x01(\x08R\x07getOnly\x12\x1f\n\x0b\x65ndpoint_id\x18\x05 \x01(\tR\nendpointId\"\xa7\x02\n\x1fGetOrCreateObjectByPathResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x44\n\tdataclass\x18\x03 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12\x39\n\x06hashes\x18\x04 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\'\n\x0frevision_number\x18\x05 \x01(\x03R\x0erevisionNumber\x12\x18\n\x07\x63reated\x18\x06 \x01(\x08R\x07\x63reated\"\x8f\x01\n\x18GetObjectLocationRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1f\n\x0brevision_id\x18\x02 \x01(\tR\nrevisionId\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1f\n\x0b\x65ndpoint_id\x18\x04 \x01(\tR\nendpointId\"\x95\x01\n\x19GetObjectLocationResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12;\n\x08location\x18\x02 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x08location\"U\n\x1cGetCollectionByBucketRequest\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x1d\n\naccess_key\x18\x02 \x01(\tR\taccessKey\"c\n\x1dGetCollectionByBucketResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId*[\n\x0cLocationType\x12\x1d\n\x19LOCATION_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10LOCATION_TYPE_S3\x10\x01\x12\x16\n\x12LOCATION_TYPE_FILE\x10\x02\x32\x9a\x03\n\x14InternalProxyService\x12~\n\x13InitMultipartUpload\x12\x31.aruna.api.internal.v1.InitMultipartUploadRequest\x1a\x32.aruna.api.internal.v1.InitMultipartUploadResponse\"\x00\x12\x84\x01\n\x15\x46inishMultipartUpload\x12\x33.aruna.api.internal.v1.FinishMultipartUploadRequest\x1a\x34.aruna.api.internal.v1.FinishMultipartUploadResponse\"\x00\x12i\n\x0c\x44\x65leteObject\x12*.aruna.api.internal.v1.DeleteObjectRequest\x1a+.aruna.api.internal.v1.DeleteObjectResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\xbf\x05\n\x1cInternalProxyNotifierService\x12\x8a\x01\n\x17GetOrCreateObjectByPath\x12\x35.aruna.api.internal.v1.GetOrCreateObjectByPathRequest\x1a\x36.aruna.api.internal.v1.GetOrCreateObjectByPathResponse\"\x00\x12o\n\x0e\x46inalizeObject\x12,.aruna.api.internal.v1.FinalizeObjectRequest\x1a-.aruna.api.internal.v1.FinalizeObjectResponse\"\x00\x12\x8d\x01\n\x18GetOrCreateEncryptionKey\x12\x36.aruna.api.internal.v1.GetOrCreateEncryptionKeyRequest\x1a\x37.aruna.api.internal.v1.GetOrCreateEncryptionKeyResponse\"\x00\x12x\n\x11GetObjectLocation\x12/.aruna.api.internal.v1.GetObjectLocationRequest\x1a\x30.aruna.api.internal.v1.GetObjectLocationResponse\"\x00\x12\x84\x01\n\x15GetCollectionByBucket\x12\x33.aruna.api.internal.v1.GetCollectionByBucketRequest\x1a\x34.aruna.api.internal.v1.GetCollectionByBucketResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.internal.v1.proxy_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1'
   _INTERNALPROXYSERVICE._options = None
   _INTERNALPROXYSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
   _INTERNALPROXYNOTIFIERSERVICE._options = None
   _INTERNALPROXYNOTIFIERSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
-  _LOCATIONTYPE._serialized_start=2327
-  _LOCATIONTYPE._serialized_end=2418
+  _LOCATIONTYPE._serialized_start=2519
+  _LOCATIONTYPE._serialized_end=2610
   _LOCATION._serialized_start=184
   _LOCATION._serialized_end=439
   _PARTETAG._serialized_start=441
   _PARTETAG._serialized_end=504
   _INITMULTIPARTUPLOADREQUEST._serialized_start=506
-  _INITMULTIPARTUPLOADREQUEST._serialized_end=554
-  _INITMULTIPARTUPLOADRESPONSE._serialized_start=556
-  _INITMULTIPARTUPLOADRESPONSE._serialized_end=614
-  _FINISHMULTIPARTUPLOADREQUEST._serialized_start=617
-  _FINISHMULTIPARTUPLOADREQUEST._serialized_end=760
-  _FINISHMULTIPARTUPLOADRESPONSE._serialized_start=762
-  _FINISHMULTIPARTUPLOADRESPONSE._serialized_end=793
-  _DELETEOBJECTREQUEST._serialized_start=795
-  _DELETEOBJECTREQUEST._serialized_end=877
-  _DELETEOBJECTRESPONSE._serialized_start=879
-  _DELETEOBJECTRESPONSE._serialized_end=901
-  _FINALIZEOBJECTREQUEST._serialized_start=904
-  _FINALIZEOBJECTREQUEST._serialized_end=1152
-  _FINALIZEOBJECTRESPONSE._serialized_start=1154
-  _FINALIZEOBJECTRESPONSE._serialized_end=1178
-  _GETORCREATEENCRYPTIONKEYREQUEST._serialized_start=1180
-  _GETORCREATEENCRYPTIONKEYREQUEST._serialized_end=1286
-  _GETORCREATEENCRYPTIONKEYRESPONSE._serialized_start=1288
-  _GETORCREATEENCRYPTIONKEYRESPONSE._serialized_end=1387
-  _GETORCREATEOBJECTBYPATHREQUEST._serialized_start=1390
-  _GETORCREATEOBJECTBYPATHREQUEST._serialized_end=1541
-  _GETORCREATEOBJECTBYPATHRESPONSE._serialized_start=1544
-  _GETORCREATEOBJECTBYPATHRESPONSE._serialized_end=1839
-  _GETOBJECTLOCATIONREQUEST._serialized_start=1842
-  _GETOBJECTLOCATIONREQUEST._serialized_end=1985
-  _GETOBJECTLOCATIONRESPONSE._serialized_start=1988
-  _GETOBJECTLOCATIONRESPONSE._serialized_end=2137
-  _GETCOLLECTIONBYBUCKETREQUEST._serialized_start=2139
-  _GETCOLLECTIONBYBUCKETREQUEST._serialized_end=2224
-  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_start=2226
-  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_end=2325
-  _INTERNALPROXYSERVICE._serialized_start=2421
-  _INTERNALPROXYSERVICE._serialized_end=2831
-  _INTERNALPROXYNOTIFIERSERVICE._serialized_start=2834
-  _INTERNALPROXYNOTIFIERSERVICE._serialized_end=3537
+  _INITMULTIPARTUPLOADREQUEST._serialized_end=620
+  _INITMULTIPARTUPLOADRESPONSE._serialized_start=622
+  _INITMULTIPARTUPLOADRESPONSE._serialized_end=680
+  _FINISHMULTIPARTUPLOADREQUEST._serialized_start=683
+  _FINISHMULTIPARTUPLOADREQUEST._serialized_end=892
+  _FINISHMULTIPARTUPLOADRESPONSE._serialized_start=894
+  _FINISHMULTIPARTUPLOADRESPONSE._serialized_end=925
+  _DELETEOBJECTREQUEST._serialized_start=927
+  _DELETEOBJECTREQUEST._serialized_end=1009
+  _DELETEOBJECTRESPONSE._serialized_start=1011
+  _DELETEOBJECTRESPONSE._serialized_end=1033
+  _FINALIZEOBJECTREQUEST._serialized_start=1036
+  _FINALIZEOBJECTREQUEST._serialized_end=1284
+  _FINALIZEOBJECTRESPONSE._serialized_start=1286
+  _FINALIZEOBJECTRESPONSE._serialized_end=1310
+  _GETORCREATEENCRYPTIONKEYREQUEST._serialized_start=1312
+  _GETORCREATEENCRYPTIONKEYREQUEST._serialized_end=1418
+  _GETORCREATEENCRYPTIONKEYRESPONSE._serialized_start=1420
+  _GETORCREATEENCRYPTIONKEYRESPONSE._serialized_end=1519
+  _GETORCREATEOBJECTBYPATHREQUEST._serialized_start=1522
+  _GETORCREATEOBJECTBYPATHREQUEST._serialized_end=1733
+  _GETORCREATEOBJECTBYPATHRESPONSE._serialized_start=1736
+  _GETORCREATEOBJECTBYPATHRESPONSE._serialized_end=2031
+  _GETOBJECTLOCATIONREQUEST._serialized_start=2034
+  _GETOBJECTLOCATIONREQUEST._serialized_end=2177
+  _GETOBJECTLOCATIONRESPONSE._serialized_start=2180
+  _GETOBJECTLOCATIONRESPONSE._serialized_end=2329
+  _GETCOLLECTIONBYBUCKETREQUEST._serialized_start=2331
+  _GETCOLLECTIONBYBUCKETREQUEST._serialized_end=2416
+  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_start=2418
+  _GETCOLLECTIONBYBUCKETRESPONSE._serialized_end=2517
+  _INTERNALPROXYSERVICE._serialized_start=2613
+  _INTERNALPROXYSERVICE._serialized_end=3023
+  _INTERNALPROXYNOTIFIERSERVICE._serialized_start=3026
+  _INTERNALPROXYNOTIFIERSERVICE._serialized_end=3729
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -37,22 +37,26 @@
     def __init__(self, object_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., location: _Optional[_Union[Location, _Mapping]] = ..., hashes: _Optional[_Iterable[_Union[_models_pb2.Hash, _Mapping]]] = ..., content_length: _Optional[int] = ...) -> None: ...
 
 class FinalizeObjectResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class FinishMultipartUploadRequest(_message.Message):
-    __slots__ = ["part_etags", "path", "upload_id"]
+    __slots__ = ["collection_id", "object_id", "part_etags", "path", "upload_id"]
+    COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_ID_FIELD_NUMBER: _ClassVar[int]
     PART_ETAGS_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
     UPLOAD_ID_FIELD_NUMBER: _ClassVar[int]
+    collection_id: str
+    object_id: str
     part_etags: _containers.RepeatedCompositeFieldContainer[PartETag]
     path: str
     upload_id: str
-    def __init__(self, upload_id: _Optional[str] = ..., path: _Optional[str] = ..., part_etags: _Optional[_Iterable[_Union[PartETag, _Mapping]]] = ...) -> None: ...
+    def __init__(self, upload_id: _Optional[str] = ..., path: _Optional[str] = ..., object_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., part_etags: _Optional[_Iterable[_Union[PartETag, _Mapping]]] = ...) -> None: ...
 
 class FinishMultipartUploadResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class GetCollectionByBucketRequest(_message.Message):
     __slots__ = ["access_key", "bucket"]
@@ -105,22 +109,26 @@
     CREATED_FIELD_NUMBER: _ClassVar[int]
     ENCRYPTION_KEY_FIELD_NUMBER: _ClassVar[int]
     created: bool
     encryption_key: str
     def __init__(self, encryption_key: _Optional[str] = ..., created: bool = ...) -> None: ...
 
 class GetOrCreateObjectByPathRequest(_message.Message):
-    __slots__ = ["access_key", "object", "path"]
+    __slots__ = ["access_key", "endpoint_id", "get_only", "object", "path"]
     ACCESS_KEY_FIELD_NUMBER: _ClassVar[int]
+    ENDPOINT_ID_FIELD_NUMBER: _ClassVar[int]
+    GET_ONLY_FIELD_NUMBER: _ClassVar[int]
     OBJECT_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
     access_key: str
+    endpoint_id: str
+    get_only: bool
     object: _object_service_pb2.StageObject
     path: str
-    def __init__(self, path: _Optional[str] = ..., access_key: _Optional[str] = ..., object: _Optional[_Union[_object_service_pb2.StageObject, _Mapping]] = ...) -> None: ...
+    def __init__(self, path: _Optional[str] = ..., access_key: _Optional[str] = ..., object: _Optional[_Union[_object_service_pb2.StageObject, _Mapping]] = ..., get_only: bool = ..., endpoint_id: _Optional[str] = ...) -> None: ...
 
 class GetOrCreateObjectByPathResponse(_message.Message):
     __slots__ = ["collection_id", "created", "dataclass", "hashes", "object_id", "revision_number"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     CREATED_FIELD_NUMBER: _ClassVar[int]
     DATACLASS_FIELD_NUMBER: _ClassVar[int]
     HASHES_FIELD_NUMBER: _ClassVar[int]
@@ -131,18 +139,22 @@
     dataclass: _models_pb2.DataClass
     hashes: _containers.RepeatedCompositeFieldContainer[_models_pb2.Hash]
     object_id: str
     revision_number: int
     def __init__(self, object_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., dataclass: _Optional[_Union[_models_pb2.DataClass, str]] = ..., hashes: _Optional[_Iterable[_Union[_models_pb2.Hash, _Mapping]]] = ..., revision_number: _Optional[int] = ..., created: bool = ...) -> None: ...
 
 class InitMultipartUploadRequest(_message.Message):
-    __slots__ = ["path"]
+    __slots__ = ["collection_id", "object_id", "path"]
+    COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    OBJECT_ID_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
+    collection_id: str
+    object_id: str
     path: str
-    def __init__(self, path: _Optional[str] = ...) -> None: ...
+    def __init__(self, path: _Optional[str] = ..., object_id: _Optional[str] = ..., collection_id: _Optional[str] = ...) -> None: ...
 
 class InitMultipartUploadResponse(_message.Message):
     __slots__ = ["upload_id"]
     UPLOAD_ID_FIELD_NUMBER: _ClassVar[int]
     upload_id: str
     def __init__(self, upload_id: _Optional[str] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&aruna/api/storage/models/v1/auth.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd1\x01\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12Y\n\x10user_permissions\x18\x03 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\"\x99\x01\n\x0fProjectOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12\x19\n\x08user_ids\x18\x05 \x03(\tR\x07userIds\"\x8d\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x65xternal_id\x18\x02 \x01(\tR\nexternalId\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\"\xf5\x02\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x45\n\ntoken_type\x18\x04 \x01(\x0e\x32&.aruna.api.storage.models.v1.TokenTypeR\ttokenType\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12#\n\rcollection_id\x18\x07 \x01(\tR\x0c\x63ollectionId\x12\x1d\n\nproject_id\x18\x08 \x01(\tR\tprojectId\x12G\n\npermission\x18\t \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\xbd\x01\n\x11ProjectPermission\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\'\n\x0fservice_account\x18\x04 \x01(\x08R\x0eserviceAccount\"\xc2\x01\n\x1cProjectPermissionDisplayName\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName*\x96\x01\n\nPermission\x12\x1a\n\x16PERMISSION_UNSPECIFIED\x10\x00\x12\x13\n\x0fPERMISSION_NONE\x10\x01\x12\x13\n\x0fPERMISSION_READ\x10\x02\x12\x15\n\x11PERMISSION_APPEND\x10\x03\x12\x15\n\x11PERMISSION_MODIFY\x10\x04\x12\x14\n\x10PERMISSION_ADMIN\x10\x05*g\n\x08PermType\x12\x19\n\x15PERM_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0ePERM_TYPE_USER\x10\x01\x12\x17\n\x13PERM_TYPE_ANONYMOUS\x10\x02\x12\x13\n\x0fPERM_TYPE_TOKEN\x10\x03*W\n\tTokenType\x12\x1a\n\x16TOKEN_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13TOKEN_TYPE_PERSONAL\x10\x01\x12\x15\n\x11TOKEN_TYPE_SCOPED\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&aruna/api/storage/models/v1/auth.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd1\x01\n\x07Project\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12Y\n\x10user_permissions\x18\x03 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\"\x99\x01\n\x0fProjectOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12%\n\x0e\x63ollection_ids\x18\x04 \x03(\tR\rcollectionIds\x12\x19\n\x08user_ids\x18\x05 \x03(\tR\x07userIds\"\xd1\x01\n\x04User\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1f\n\x0b\x65xternal_id\x18\x02 \x01(\tR\nexternalId\x12!\n\x0c\x64isplay_name\x18\x03 \x01(\tR\x0b\x64isplayName\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12,\n\x12is_service_account\x18\x06 \x01(\x08R\x10isServiceAccount\x12\x14\n\x05\x65mail\x18\x07 \x01(\tR\x05\x65mail\"\xc9\x03\n\x05Token\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x45\n\ntoken_type\x18\x04 \x01(\x0e\x32&.aruna.api.storage.models.v1.TokenTypeR\ttokenType\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\x12\x39\n\nexpires_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\x12#\n\rcollection_id\x18\x07 \x01(\tR\x0c\x63ollectionId\x12\x1d\n\nproject_id\x18\x08 \x01(\tR\tprojectId\x12G\n\npermission\x18\t \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\x1d\n\nis_session\x18\n \x01(\x08R\tisSession\x12\x33\n\x07used_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x06usedAt\"\xbd\x01\n\x11ProjectPermission\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\'\n\x0fservice_account\x18\x04 \x01(\x08R\x0eserviceAccount\"\xc2\x01\n\x1cProjectPermissionDisplayName\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1d\n\nproject_id\x18\x02 \x01(\tR\tprojectId\x12G\n\npermission\x18\x03 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12!\n\x0c\x64isplay_name\x18\x04 \x01(\tR\x0b\x64isplayName*\x96\x01\n\nPermission\x12\x1a\n\x16PERMISSION_UNSPECIFIED\x10\x00\x12\x13\n\x0fPERMISSION_NONE\x10\x01\x12\x13\n\x0fPERMISSION_READ\x10\x02\x12\x15\n\x11PERMISSION_APPEND\x10\x03\x12\x15\n\x11PERMISSION_MODIFY\x10\x04\x12\x14\n\x10PERMISSION_ADMIN\x10\x05*g\n\x08PermType\x12\x19\n\x15PERM_TYPE_UNSPECIFIED\x10\x00\x12\x12\n\x0ePERM_TYPE_USER\x10\x01\x12\x17\n\x13PERM_TYPE_ANONYMOUS\x10\x02\x12\x13\n\x0fPERM_TYPE_TOKEN\x10\x03*W\n\tTokenType\x12\x1a\n\x16TOKEN_TYPE_UNSPECIFIED\x10\x00\x12\x17\n\x13TOKEN_TYPE_PERSONAL\x10\x01\x12\x15\n\x11TOKEN_TYPE_SCOPED\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.models.v1.auth_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1'
-  _PERMISSION._serialized_start=1382
-  _PERMISSION._serialized_end=1532
-  _PERMTYPE._serialized_start=1534
-  _PERMTYPE._serialized_end=1637
-  _TOKENTYPE._serialized_start=1639
-  _TOKENTYPE._serialized_end=1726
+  _PERMISSION._serialized_start=1534
+  _PERMISSION._serialized_end=1684
+  _PERMTYPE._serialized_start=1686
+  _PERMTYPE._serialized_end=1789
+  _TOKENTYPE._serialized_start=1791
+  _TOKENTYPE._serialized_end=1878
   _PROJECT._serialized_start=105
   _PROJECT._serialized_end=314
   _PROJECTOVERVIEW._serialized_start=317
   _PROJECTOVERVIEW._serialized_end=470
   _USER._serialized_start=473
-  _USER._serialized_end=614
-  _TOKEN._serialized_start=617
-  _TOKEN._serialized_end=990
-  _PROJECTPERMISSION._serialized_start=993
-  _PROJECTPERMISSION._serialized_end=1182
-  _PROJECTPERMISSIONDISPLAYNAME._serialized_start=1185
-  _PROJECTPERMISSIONDISPLAYNAME._serialized_end=1379
+  _USER._serialized_end=682
+  _TOKEN._serialized_start=685
+  _TOKEN._serialized_end=1142
+  _PROJECTPERMISSION._serialized_start=1145
+  _PROJECTPERMISSION._serialized_end=1334
+  _PROJECTPERMISSIONDISPLAYNAME._serialized_start=1337
+  _PROJECTPERMISSIONDISPLAYNAME._serialized_end=1531
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -69,46 +69,54 @@
     display_name: str
     permission: Permission
     project_id: str
     user_id: str
     def __init__(self, user_id: _Optional[str] = ..., project_id: _Optional[str] = ..., permission: _Optional[_Union[Permission, str]] = ..., display_name: _Optional[str] = ...) -> None: ...
 
 class Token(_message.Message):
-    __slots__ = ["collection_id", "created_at", "expires_at", "id", "name", "permission", "project_id", "token_type"]
+    __slots__ = ["collection_id", "created_at", "expires_at", "id", "is_session", "name", "permission", "project_id", "token_type", "used_at"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
+    IS_SESSION_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PERMISSION_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     TOKEN_TYPE_FIELD_NUMBER: _ClassVar[int]
+    USED_AT_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
     created_at: _timestamp_pb2.Timestamp
     expires_at: _timestamp_pb2.Timestamp
     id: str
+    is_session: bool
     name: str
     permission: Permission
     project_id: str
     token_type: TokenType
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., token_type: _Optional[_Union[TokenType, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., collection_id: _Optional[str] = ..., project_id: _Optional[str] = ..., permission: _Optional[_Union[Permission, str]] = ...) -> None: ...
+    used_at: _timestamp_pb2.Timestamp
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., token_type: _Optional[_Union[TokenType, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., expires_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., collection_id: _Optional[str] = ..., project_id: _Optional[str] = ..., permission: _Optional[_Union[Permission, str]] = ..., is_session: bool = ..., used_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class User(_message.Message):
-    __slots__ = ["active", "display_name", "external_id", "id", "is_admin"]
+    __slots__ = ["active", "display_name", "email", "external_id", "id", "is_admin", "is_service_account"]
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     DISPLAY_NAME_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
     EXTERNAL_ID_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     IS_ADMIN_FIELD_NUMBER: _ClassVar[int]
+    IS_SERVICE_ACCOUNT_FIELD_NUMBER: _ClassVar[int]
     active: bool
     display_name: str
+    email: str
     external_id: str
     id: str
     is_admin: bool
-    def __init__(self, id: _Optional[str] = ..., external_id: _Optional[str] = ..., display_name: _Optional[str] = ..., active: bool = ..., is_admin: bool = ...) -> None: ...
+    is_service_account: bool
+    def __init__(self, id: _Optional[str] = ..., external_id: _Optional[str] = ..., display_name: _Optional[str] = ..., active: bool = ..., is_admin: bool = ..., is_service_account: bool = ..., email: _Optional[str] = ...) -> None: ...
 
 class Permission(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class PermType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,38 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v1/models.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"?\n\rLabelOntology\x12.\n\x13required_label_keys\x18\x01 \x03(\tR\x11requiredLabelKeys\"8\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x19\n\x08\x61\x63\x63_size\x18\x02 \x01(\x03R\x07\x61\x63\x63Size\"\xc5\x01\n\x0f\x43ollectionStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12,\n\x12object_group_count\x18\x02 \x01(\x03R\x10objectGroupCount\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"\x98\x01\n\x10ObjectGroupStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12=\n\x0clast_updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"K\n\x07Version\x12\x14\n\x05major\x18\x01 \x01(\x05R\x05major\x12\x14\n\x05minor\x18\x02 \x01(\x05R\x05minor\x12\x14\n\x05patch\x18\x03 \x01(\x05R\x05patch\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v1.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\x1e\n\x06Origin\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02idJ\x04\x08\x01\x10\x02\"r\n\x06Source\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12H\n\x0bsource_type\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.SourceTypeR\nsourceType\"\xb1\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12%\n\x0eproxy_hostname\x18\x04 \x01(\tR\rproxyHostname\x12+\n\x11internal_hostname\x18\x05 \x01(\tR\x10internalHostname\x12-\n\x12\x64ocumentation_path\x18\x06 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x07 \x01(\x08R\x08isPublic\x12\x1d\n\nis_default\x18\x08 \x01(\x08R\tisDefault\"\x9e\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1a\n\x08\x66ilename\x18\x02 \x01(\tR\x08\x66ilename\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x1f\n\x0b\x63ontent_len\x18\x07 \x01(\x03R\ncontentLen\x12;\n\x06status\x18\x08 \x01(\x0e\x32#.aruna.api.storage.models.v1.StatusR\x06status\x12;\n\x06origin\x18\t \x01(\x0b\x32#.aruna.api.storage.models.v1.OriginR\x06origin\x12\x45\n\ndata_class\x18\n \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataClass\x12\x39\n\x06hashes\x18\x10 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\x1d\n\nrev_number\x18\x0c \x01(\x03R\trevNumber\x12;\n\x06source\x18\r \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x16\n\x06latest\x18\x0e \x01(\x08R\x06latest\x12\x1f\n\x0b\x61uto_update\x18\x0f \x01(\x08R\nautoUpdateJ\x04\x08\x0b\x10\x0c\"H\n\x07Objects\x12=\n\x07objects\x18\x01 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\"\xba\x03\n\x0bObjectGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12\x46\n\x0cmeta_objects\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0bmetaObjects\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"]\n\x0cObjectGroups\x12M\n\robject_groups\x18\x01 \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\"\xbb\x02\n\x13ObjectGroupOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x43\n\x05stats\x18\x08 \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\t \x01(\x03R\trevNumber\"~\n\x14ObjectGroupOverviews\x12\x66\n\x16object_group_overviews\x18\x01 \x03(\x0b\x32\x30.aruna.api.storage.models.v1.ObjectGroupOverviewR\x14objectGroupOverviews\"\x80\x03\n\x11ObjectGroupWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x1d\n\nobject_ids\x18\x08 \x03(\tR\tobjectIds\x12&\n\x0fmeta_object_ids\x18\t \x03(\tR\rmetaObjectIds\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"w\n\x12ObjectGroupWithIDs\x12\x61\n\x15object_group_with_ids\x18\x01 \x03(\x0b\x32..aruna.api.storage.models.v1.ObjectGroupWithIDR\x12objectGroupWithIds\"\x8b\x06\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12K\n\x0especifications\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0especifications\x12M\n\robject_groups\x18\n \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"X\n\x0b\x43ollections\x12I\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\'.aruna.api.storage.models.v1.CollectionR\x0b\x63ollections\"\xb8\x04\n\x12\x43ollectionOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"y\n\x13\x43ollectionOverviews\x12\x62\n\x14\x63ollection_overviews\x18\x01 \x03(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\x13\x63ollectionOverviews\"\x9d\x05\n\x10\x43ollectionWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x18\n\x07objects\x18\x08 \x03(\tR\x07objects\x12&\n\x0especifications\x18\t \x03(\tR\x0especifications\x12#\n\robject_groups\x18\n \x03(\tR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"r\n\x11\x43ollectionWithIDs\x12]\n\x13\x63ollection_with_ids\x18\x01 \x03(\x0b\x32-.aruna.api.storage.models.v1.CollectionWithIDR\x11\x63ollectionWithIds*\xb7\x01\n\x0cResourceType\x12\x1d\n\x19RESOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15RESOURCE_TYPE_PROJECT\x10\x01\x12\x1c\n\x18RESOURCE_TYPE_COLLECTION\x10\x02\x12\x1e\n\x1aRESOURCE_TYPE_OBJECT_GROUP\x10\x03\x12\x18\n\x14RESOURCE_TYPE_OBJECT\x10\x04\x12\x15\n\x11RESOURCE_TYPE_ALL\x10\x05*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\x8b\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x14\n\x10STATUS_AVAILABLE\x10\x02\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\x12\x10\n\x0cSTATUS_TRASH\x10\x05*k\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x03\"\x04\x08\x02\x10\x02\"\x04\x08\x04\x10\x07*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x03\x12\x18\n\x14\x44\x41TA_CLASS_PROTECTED\x10\x04*S\n\nSourceType\x12\x1b\n\x17SOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x13\n\x0fSOURCE_TYPE_URL\x10\x01\x12\x13\n\x0fSOURCE_TYPE_DOI\x10\x02*[\n\x0c\x45ndpointType\x12\x1d\n\x19\x45NDPOINT_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x45NDPOINT_TYPE_S3\x10\x01\x12\x16\n\x12\x45NDPOINT_TYPE_FILE\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v1/models.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"?\n\rLabelOntology\x12.\n\x13required_label_keys\x18\x01 \x03(\tR\x11requiredLabelKeys\"8\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x19\n\x08\x61\x63\x63_size\x18\x02 \x01(\x03R\x07\x61\x63\x63Size\"\xc5\x01\n\x0f\x43ollectionStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12,\n\x12object_group_count\x18\x02 \x01(\x03R\x10objectGroupCount\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"\x98\x01\n\x10ObjectGroupStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12=\n\x0clast_updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"K\n\x07Version\x12\x14\n\x05major\x18\x01 \x01(\x05R\x05major\x12\x14\n\x05minor\x18\x02 \x01(\x05R\x05minor\x12\x14\n\x05patch\x18\x03 \x01(\x05R\x05patch\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v1.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\x1e\n\x06Origin\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02idJ\x04\x08\x01\x10\x02\"r\n\x06Source\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12H\n\x0bsource_type\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.SourceTypeR\nsourceType\"\xf6\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12%\n\x0eproxy_hostname\x18\x04 \x01(\tR\rproxyHostname\x12+\n\x11internal_hostname\x18\x05 \x01(\tR\x10internalHostname\x12-\n\x12\x64ocumentation_path\x18\x06 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x07 \x01(\x08R\x08isPublic\x12\x1d\n\nis_default\x18\x08 \x01(\x08R\tisDefault\x12\x43\n\x06status\x18\t \x01(\x0e\x32+.aruna.api.storage.models.v1.EndpointStatusR\x06status\"\x9e\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1a\n\x08\x66ilename\x18\x02 \x01(\tR\x08\x66ilename\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x1f\n\x0b\x63ontent_len\x18\x07 \x01(\x03R\ncontentLen\x12;\n\x06status\x18\x08 \x01(\x0e\x32#.aruna.api.storage.models.v1.StatusR\x06status\x12;\n\x06origin\x18\t \x01(\x0b\x32#.aruna.api.storage.models.v1.OriginR\x06origin\x12\x45\n\ndata_class\x18\n \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataClass\x12\x39\n\x06hashes\x18\x10 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\x1d\n\nrev_number\x18\x0c \x01(\x03R\trevNumber\x12;\n\x06source\x18\r \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x16\n\x06latest\x18\x0e \x01(\x08R\x06latest\x12\x1f\n\x0b\x61uto_update\x18\x0f \x01(\x08R\nautoUpdateJ\x04\x08\x0b\x10\x0c\"H\n\x07Objects\x12=\n\x07objects\x18\x01 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\"\xba\x03\n\x0bObjectGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12\x46\n\x0cmeta_objects\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0bmetaObjects\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"]\n\x0cObjectGroups\x12M\n\robject_groups\x18\x01 \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\"\xbb\x02\n\x13ObjectGroupOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x43\n\x05stats\x18\x08 \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\t \x01(\x03R\trevNumber\"~\n\x14ObjectGroupOverviews\x12\x66\n\x16object_group_overviews\x18\x01 \x03(\x0b\x32\x30.aruna.api.storage.models.v1.ObjectGroupOverviewR\x14objectGroupOverviews\"\x80\x03\n\x11ObjectGroupWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x1d\n\nobject_ids\x18\x08 \x03(\tR\tobjectIds\x12&\n\x0fmeta_object_ids\x18\t \x03(\tR\rmetaObjectIds\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"w\n\x12ObjectGroupWithIDs\x12\x61\n\x15object_group_with_ids\x18\x01 \x03(\x0b\x32..aruna.api.storage.models.v1.ObjectGroupWithIDR\x12objectGroupWithIds\"\x8b\x06\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12K\n\x0especifications\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0especifications\x12M\n\robject_groups\x18\n \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"X\n\x0b\x43ollections\x12I\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\'.aruna.api.storage.models.v1.CollectionR\x0b\x63ollections\"\xb8\x04\n\x12\x43ollectionOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"y\n\x13\x43ollectionOverviews\x12\x62\n\x14\x63ollection_overviews\x18\x01 \x03(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\x13\x63ollectionOverviews\"\x9d\x05\n\x10\x43ollectionWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x18\n\x07objects\x18\x08 \x03(\tR\x07objects\x12&\n\x0especifications\x18\t \x03(\tR\x0especifications\x12#\n\robject_groups\x18\n \x03(\tR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"r\n\x11\x43ollectionWithIDs\x12]\n\x13\x63ollection_with_ids\x18\x01 \x03(\x0b\x32-.aruna.api.storage.models.v1.CollectionWithIDR\x11\x63ollectionWithIds*\xb7\x01\n\x0cResourceType\x12\x1d\n\x19RESOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15RESOURCE_TYPE_PROJECT\x10\x01\x12\x1c\n\x18RESOURCE_TYPE_COLLECTION\x10\x02\x12\x1e\n\x1aRESOURCE_TYPE_OBJECT_GROUP\x10\x03\x12\x18\n\x14RESOURCE_TYPE_OBJECT\x10\x04\x12\x15\n\x11RESOURCE_TYPE_ALL\x10\x05*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\xa2\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x14\n\x10STATUS_AVAILABLE\x10\x02\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\x12\x10\n\x0cSTATUS_TRASH\x10\x05\x12\x15\n\x11STATUS_FINALIZING\x10\x06*\xd2\x01\n\x0e\x45ndpointStatus\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNSPECIFIED\x10\x00\x12 \n\x1c\x45NDPOINT_STATUS_INITIALIZING\x10\x01\x12\x1d\n\x19\x45NDPOINT_STATUS_AVAILABLE\x10\x02\x12\x1c\n\x18\x45NDPOINT_STATUS_DEGRADED\x10\x03\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNAVAILABLE\x10\x04\x12\x1f\n\x1b\x45NDPOINT_STATUS_MAINTENANCE\x10\x05*k\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x03\"\x04\x08\x02\x10\x02\"\x04\x08\x04\x10\x07*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x03\x12\x18\n\x14\x44\x41TA_CLASS_PROTECTED\x10\x04*S\n\nSourceType\x12\x1b\n\x17SOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x13\n\x0fSOURCE_TYPE_URL\x10\x01\x12\x13\n\x0fSOURCE_TYPE_DOI\x10\x02*[\n\x0c\x45ndpointType\x12\x1d\n\x19\x45NDPOINT_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x45NDPOINT_TYPE_S3\x10\x01\x12\x16\n\x12\x45NDPOINT_TYPE_FILE\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.models.v1.models_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1'
-  _RESOURCETYPE._serialized_start=5855
-  _RESOURCETYPE._serialized_end=6038
-  _RESOURCEACTION._serialized_start=6041
-  _RESOURCEACTION._serialized_end=6228
-  _STATUS._serialized_start=6231
-  _STATUS._serialized_end=6370
-  _HASHALGORITHM._serialized_start=6372
-  _HASHALGORITHM._serialized_end=6479
-  _DATACLASS._serialized_start=6482
-  _DATACLASS._serialized_end=6623
-  _SOURCETYPE._serialized_start=6625
-  _SOURCETYPE._serialized_end=6708
-  _ENDPOINTTYPE._serialized_start=6710
-  _ENDPOINTTYPE._serialized_end=6801
+  _RESOURCETYPE._serialized_start=5924
+  _RESOURCETYPE._serialized_end=6107
+  _RESOURCEACTION._serialized_start=6110
+  _RESOURCEACTION._serialized_end=6297
+  _STATUS._serialized_start=6300
+  _STATUS._serialized_end=6462
+  _ENDPOINTSTATUS._serialized_start=6465
+  _ENDPOINTSTATUS._serialized_end=6675
+  _HASHALGORITHM._serialized_start=6677
+  _HASHALGORITHM._serialized_end=6784
+  _DATACLASS._serialized_start=6787
+  _DATACLASS._serialized_end=6928
+  _SOURCETYPE._serialized_start=6930
+  _SOURCETYPE._serialized_end=7013
+  _ENDPOINTTYPE._serialized_start=7015
+  _ENDPOINTTYPE._serialized_end=7106
   _KEYVALUE._serialized_start=106
   _KEYVALUE._serialized_end=156
   _LABELONTOLOGY._serialized_start=158
   _LABELONTOLOGY._serialized_end=221
   _STATS._serialized_start=223
   _STATS._serialized_end=279
   _COLLECTIONSTATS._serialized_start=282
@@ -51,37 +53,37 @@
   _HASH._serialized_start=713
   _HASH._serialized_end=801
   _ORIGIN._serialized_start=803
   _ORIGIN._serialized_end=833
   _SOURCE._serialized_start=835
   _SOURCE._serialized_end=949
   _ENDPOINT._serialized_start=952
-  _ENDPOINT._serialized_end=1257
-  _OBJECT._serialized_start=1260
-  _OBJECT._serialized_end=1930
-  _OBJECTS._serialized_start=1932
-  _OBJECTS._serialized_end=2004
-  _OBJECTGROUP._serialized_start=2007
-  _OBJECTGROUP._serialized_end=2449
-  _OBJECTGROUPS._serialized_start=2451
-  _OBJECTGROUPS._serialized_end=2544
-  _OBJECTGROUPOVERVIEW._serialized_start=2547
-  _OBJECTGROUPOVERVIEW._serialized_end=2862
-  _OBJECTGROUPOVERVIEWS._serialized_start=2864
-  _OBJECTGROUPOVERVIEWS._serialized_end=2990
-  _OBJECTGROUPWITHID._serialized_start=2993
-  _OBJECTGROUPWITHID._serialized_end=3377
-  _OBJECTGROUPWITHIDS._serialized_start=3379
-  _OBJECTGROUPWITHIDS._serialized_end=3498
-  _COLLECTION._serialized_start=3501
-  _COLLECTION._serialized_end=4280
-  _COLLECTIONS._serialized_start=4282
-  _COLLECTIONS._serialized_end=4370
-  _COLLECTIONOVERVIEW._serialized_start=4373
-  _COLLECTIONOVERVIEW._serialized_end=4941
-  _COLLECTIONOVERVIEWS._serialized_start=4943
-  _COLLECTIONOVERVIEWS._serialized_end=5064
-  _COLLECTIONWITHID._serialized_start=5067
-  _COLLECTIONWITHID._serialized_end=5736
-  _COLLECTIONWITHIDS._serialized_start=5738
-  _COLLECTIONWITHIDS._serialized_end=5852
+  _ENDPOINT._serialized_end=1326
+  _OBJECT._serialized_start=1329
+  _OBJECT._serialized_end=1999
+  _OBJECTS._serialized_start=2001
+  _OBJECTS._serialized_end=2073
+  _OBJECTGROUP._serialized_start=2076
+  _OBJECTGROUP._serialized_end=2518
+  _OBJECTGROUPS._serialized_start=2520
+  _OBJECTGROUPS._serialized_end=2613
+  _OBJECTGROUPOVERVIEW._serialized_start=2616
+  _OBJECTGROUPOVERVIEW._serialized_end=2931
+  _OBJECTGROUPOVERVIEWS._serialized_start=2933
+  _OBJECTGROUPOVERVIEWS._serialized_end=3059
+  _OBJECTGROUPWITHID._serialized_start=3062
+  _OBJECTGROUPWITHID._serialized_end=3446
+  _OBJECTGROUPWITHIDS._serialized_start=3448
+  _OBJECTGROUPWITHIDS._serialized_end=3567
+  _COLLECTION._serialized_start=3570
+  _COLLECTION._serialized_end=4349
+  _COLLECTIONS._serialized_start=4351
+  _COLLECTIONS._serialized_end=4439
+  _COLLECTIONOVERVIEW._serialized_start=4442
+  _COLLECTIONOVERVIEW._serialized_end=5010
+  _COLLECTIONOVERVIEWS._serialized_start=5012
+  _COLLECTIONOVERVIEWS._serialized_end=5133
+  _COLLECTIONWITHID._serialized_start=5136
+  _COLLECTIONWITHID._serialized_end=5805
+  _COLLECTIONWITHIDS._serialized_start=5807
+  _COLLECTIONWITHIDS._serialized_end=5921
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 
 DATA_CLASS_CONFIDENTIAL: DataClass
 DATA_CLASS_PRIVATE: DataClass
 DATA_CLASS_PROTECTED: DataClass
 DATA_CLASS_PUBLIC: DataClass
 DATA_CLASS_UNSPECIFIED: DataClass
 DESCRIPTOR: _descriptor.FileDescriptor
+ENDPOINT_STATUS_AVAILABLE: EndpointStatus
+ENDPOINT_STATUS_DEGRADED: EndpointStatus
+ENDPOINT_STATUS_INITIALIZING: EndpointStatus
+ENDPOINT_STATUS_MAINTENANCE: EndpointStatus
+ENDPOINT_STATUS_UNAVAILABLE: EndpointStatus
+ENDPOINT_STATUS_UNSPECIFIED: EndpointStatus
 ENDPOINT_TYPE_FILE: EndpointType
 ENDPOINT_TYPE_S3: EndpointType
 ENDPOINT_TYPE_UNSPECIFIED: EndpointType
 HASHALGORITHM_MD5: Hashalgorithm
 HASHALGORITHM_SHA256: Hashalgorithm
 HASHALGORITHM_UNSPECIFIED: Hashalgorithm
 RESOURCE_ACTION_APPEND: ResourceAction
@@ -30,14 +36,15 @@
 RESOURCE_TYPE_PROJECT: ResourceType
 RESOURCE_TYPE_UNSPECIFIED: ResourceType
 SOURCE_TYPE_DOI: SourceType
 SOURCE_TYPE_UNSPECIFIED: SourceType
 SOURCE_TYPE_URL: SourceType
 STATUS_AVAILABLE: Status
 STATUS_ERROR: Status
+STATUS_FINALIZING: Status
 STATUS_INITIALIZING: Status
 STATUS_TRASH: Status
 STATUS_UNAVAILABLE: Status
 STATUS_UNSPECIFIED: Status
 
 class Collection(_message.Message):
     __slots__ = ["created", "description", "hooks", "id", "is_public", "label_ontology", "labels", "latest", "name", "object_groups", "objects", "semantic_version", "specifications", "stats"]
@@ -154,32 +161,34 @@
 class Collections(_message.Message):
     __slots__ = ["collections"]
     COLLECTIONS_FIELD_NUMBER: _ClassVar[int]
     collections: _containers.RepeatedCompositeFieldContainer[Collection]
     def __init__(self, collections: _Optional[_Iterable[_Union[Collection, _Mapping]]] = ...) -> None: ...
 
 class Endpoint(_message.Message):
-    __slots__ = ["documentation_path", "ep_type", "id", "internal_hostname", "is_default", "is_public", "name", "proxy_hostname"]
+    __slots__ = ["documentation_path", "ep_type", "id", "internal_hostname", "is_default", "is_public", "name", "proxy_hostname", "status"]
     DOCUMENTATION_PATH_FIELD_NUMBER: _ClassVar[int]
     EP_TYPE_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     INTERNAL_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
     IS_DEFAULT_FIELD_NUMBER: _ClassVar[int]
     IS_PUBLIC_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PROXY_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
     documentation_path: str
     ep_type: EndpointType
     id: str
     internal_hostname: str
     is_default: bool
     is_public: bool
     name: str
     proxy_hostname: str
-    def __init__(self, id: _Optional[str] = ..., ep_type: _Optional[_Union[EndpointType, str]] = ..., name: _Optional[str] = ..., proxy_hostname: _Optional[str] = ..., internal_hostname: _Optional[str] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., is_default: bool = ...) -> None: ...
+    status: EndpointStatus
+    def __init__(self, id: _Optional[str] = ..., ep_type: _Optional[_Union[EndpointType, str]] = ..., name: _Optional[str] = ..., proxy_hostname: _Optional[str] = ..., internal_hostname: _Optional[str] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., is_default: bool = ..., status: _Optional[_Union[EndpointStatus, str]] = ...) -> None: ...
 
 class Hash(_message.Message):
     __slots__ = ["alg", "hash"]
     ALG_FIELD_NUMBER: _ClassVar[int]
     HASH_FIELD_NUMBER: _ClassVar[int]
     alg: Hashalgorithm
     hash: str
@@ -362,14 +371,17 @@
 
 class ResourceAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
+class EndpointStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
 class Hashalgorithm(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class DataClass(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class SourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.storage.models.v1 import query_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_query__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2aruna/api/storage/services/v1/object_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\"\x17\n\x03URL\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"\xf0\x02\n\x0bStageObject\x12\x1a\n\x08\x66ilename\x18\x01 \x01(\tR\x08\x66ilename\x12\x1f\n\x0b\x63ontent_len\x18\x04 \x01(\x03R\ncontentLen\x12;\n\x06source\x18\x05 \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x44\n\tdataclass\x18\x06 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12=\n\x06labels\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x08 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x19\n\x08sub_path\x18\t \x01(\tR\x07subPathJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xb9\x02\n\x1aInitializeNewObjectRequest\x12\x42\n\x06object\x18\x01 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x32\n\x15preferred_endpoint_id\x18\x04 \x01(\tR\x13preferredEndpointId\x12\x1c\n\tmultipart\x18\x05 \x01(\x08R\tmultipart\x12)\n\x10is_specification\x18\x06 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\x07 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\"|\n\x1bInitializeNewObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xb3\x01\n\x13GetUploadURLRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x1c\n\tmultipart\x18\x04 \x01(\x08R\tmultipart\x12\x1f\n\x0bpart_number\x18\x05 \x01(\x05R\npartNumber\"L\n\x14GetUploadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"8\n\x0e\x43ompletedParts\x12\x12\n\x04\x65tag\x18\x01 \x01(\tR\x04\x65tag\x12\x12\n\x04part\x18\x02 \x01(\x03R\x04part\"Y\n\x15GetDownloadURLRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"N\n\x16GetDownloadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"]\n\x1cGetDownloadLinksBatchRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"W\n\x1dGetDownloadLinksBatchResponse\x12\x36\n\x04urls\x18\x01 \x03(\x0b\x32\".aruna.api.storage.services.v1.URLR\x04urls\"a\n CreateDownloadLinksStreamRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"Y\n!CreateDownloadLinksStreamResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"\xc8\x02\n\x1a\x46inishObjectStagingRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x35\n\x04hash\x18\x04 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\x12\x1b\n\tno_upload\x18\x05 \x01(\x08R\x08noUpload\x12V\n\x0f\x63ompleted_parts\x18\x06 \x03(\x0b\x32-.aruna.api.storage.services.v1.CompletedPartsR\x0e\x63ompletedParts\x12\x1f\n\x0b\x61uto_update\x18\x07 \x01(\x08R\nautoUpdate\"Z\n\x1b\x46inishObjectStagingResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x82\x03\n\x13UpdateObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x1a\n\x08reupload\x18\x04 \x01(\x08R\x08reupload\x12\x32\n\x15preferred_endpoint_id\x18\x05 \x01(\tR\x13preferredEndpointId\x12\x1d\n\nmulti_part\x18\x06 \x01(\x08R\tmultiPart\x12)\n\x10is_specification\x18\x07 \x01(\x08R\x0fisSpecification\x12\x14\n\x05\x66orce\x18\x08 \x01(\x08R\x05\x66orce\x12\x35\n\x04hash\x18\t \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\"w\n\x14UpdateObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1d\n\nstaging_id\x18\x02 \x01(\tR\tstagingId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xec\x01\n\x1c\x43reateObjectReferenceRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\x12\x1c\n\twriteable\x18\x04 \x01(\x08R\twriteable\x12\x1f\n\x0b\x61uto_update\x18\x05 \x01(\x08R\nautoUpdate\x12\x19\n\x08sub_path\x18\x06 \x01(\tR\x07subPath\"\x1f\n\x1d\x43reateObjectReferenceResponse\"\x88\x01\n\x12\x43loneObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\"R\n\x13\x43loneObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x94\x01\n\x13\x44\x65leteObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x16\n\x14\x44\x65leteObjectResponse\"\x97\x01\n\x14\x44\x65leteObjectsRequest\x12\x1d\n\nobject_ids\x18\x01 \x03(\tR\tobjectIds\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x17\n\x15\x44\x65leteObjectsResponse\"t\n\rObjectWithURL\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\x12\x14\n\x05paths\x18\x03 \x03(\tR\x05paths\"s\n\x14GetObjectByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"]\n\x15GetObjectByIDResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"\xf5\x01\n\x11GetObjectsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12K\n\x0cpage_request\x18\x02 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12S\n\x0flabel_id_filter\x18\x03 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\rlabelIdFilter\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"\\\n\x12GetObjectsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"\xc5\x01\n\x19GetObjectRevisionsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"d\n\x1aGetObjectRevisionsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"}\n\x1eGetLatestObjectRevisionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x03 \x01(\x08R\x07withUrl\"g\n\x1fGetLatestObjectRevisionResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"]\n\x19GetObjectEndpointsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"a\n\x1aGetObjectEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"\xa7\x01\n\x18\x41\x64\x64LabelsToObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12I\n\rlabels_to_add\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x0blabelsToAdd\"X\n\x19\x41\x64\x64LabelsToObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x98\x01\n\x17SetHooksOfObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12;\n\x05hooks\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\"W\n\x18SetHooksOfObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x7f\n\x14GetReferencesRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\"\x9f\x01\n\x0fObjectReference\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\'\n\x0frevision_number\x18\x03 \x01(\x03R\x0erevisionNumber\x12!\n\x0cis_writeable\x18\x04 \x01(\x08R\x0bisWriteable\"g\n\x15GetReferencesResponse\x12N\n\nreferences\x18\x01 \x03(\x0b\x32..aruna.api.storage.services.v1.ObjectReferenceR\nreferences\":\n\x04Path\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x02 \x01(\x08R\nvisibility\"\x83\x01\n\x14GetObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12)\n\x10include_inactive\x18\x03 \x01(\x08R\x0fincludeInactive\"_\n\x15GetObjectPathResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"g\n\x15GetObjectPathsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12)\n\x10include_inactive\x18\x02 \x01(\x08R\x0fincludeInactive\"`\n\x16GetObjectPathsResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"v\n\x17\x43reateObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08sub_path\x18\x03 \x01(\tR\x07subPath\"S\n\x18\x43reateObjectPathResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"y\n\x1eSetObjectPathVisibilityRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x03 \x01(\x08R\nvisibility\"Z\n\x1fSetObjectPathVisibilityResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"T\n\x17GetObjectsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12%\n\x0ewith_revisions\x18\x02 \x01(\x08R\rwithRevisions\":\n$GetProjectCollectionIdsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"k\n%GetProjectCollectionIdsByPathResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"W\n\x18GetObjectsByPathResponse\x12;\n\x06object\x18\x03 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object2\x99\'\n\rObjectService\x12\xbe\x01\n\x13InitializeNewObject\x12\x39.aruna.api.storage.services.v1.InitializeNewObjectRequest\x1a:.aruna.api.storage.services.v1.InitializeNewObjectResponse\"0\x82\xd3\xe4\x93\x02*:\x01*\"%/v1/collection/{collection_id}/object\x12\xcd\x01\n\x0cGetUploadURL\x12\x32.aruna.api.storage.services.v1.GetUploadURLRequest\x1a\x33.aruna.api.storage.services.v1.GetUploadURLResponse\"T\x82\xd3\xe4\x93\x02N\x12L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/upload\x12\xc1\x01\n\x0eGetDownloadURL\x12\x34.aruna.api.storage.services.v1.GetDownloadURLRequest\x1a\x35.aruna.api.storage.services.v1.GetDownloadURLResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v1/collection/{collection_id}/object/{object_id}/download\x12\xc8\x01\n\x15GetDownloadLinksBatch\x12;.aruna.api.storage.services.v1.GetDownloadLinksBatchRequest\x1a<.aruna.api.storage.services.v1.GetDownloadLinksBatchResponse\"4\x82\xd3\xe4\x93\x02.\x12,/v1/collection/{collection_id}/objects/batch\x12\xda\x01\n\x19\x43reateDownloadLinksStream\x12?.aruna.api.storage.services.v1.CreateDownloadLinksStreamRequest\x1a@.aruna.api.storage.services.v1.CreateDownloadLinksStreamResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/v1/collection/{collection_id}/objects/stream0\x01\x12\xe5\x01\n\x13\x46inishObjectStaging\x12\x39.aruna.api.storage.services.v1.FinishObjectStagingRequest\x1a:.aruna.api.storage.services.v1.FinishObjectStagingResponse\"W\x82\xd3\xe4\x93\x02Q:\x01*2L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/finish\x12\xbc\x01\n\x0cUpdateObject\x12\x32.aruna.api.storage.services.v1.UpdateObjectRequest\x1a\x33.aruna.api.storage.services.v1.UpdateObjectResponse\"C\x82\xd3\xe4\x93\x02=:\x01*\"8/v1/collection/{collection_id}/object/{object_id}/update\x12\xf1\x01\n\x15\x43reateObjectReference\x12;.aruna.api.storage.services.v1.CreateObjectReferenceRequest\x1a<.aruna.api.storage.services.v1.CreateObjectReferenceResponse\"]\x82\xd3\xe4\x93\x02W:\x01*\"R/v1/collection/{collection_id}/object/{object_id}/reference/{target_collection_id}\x12\xb8\x01\n\x0b\x43loneObject\x12\x31.aruna.api.storage.services.v1.CloneObjectRequest\x1a\x32.aruna.api.storage.services.v1.CloneObjectResponse\"B\x82\xd3\xe4\x93\x02<:\x01*\"7/v1/collection/{collection_id}/object/{object_id}/clone\x12\xb5\x01\n\x0c\x44\x65leteObject\x12\x32.aruna.api.storage.services.v1.DeleteObjectRequest\x1a\x33.aruna.api.storage.services.v1.DeleteObjectResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01**1/v1/collection/{collection_id}/object/{object_id}\x12\xad\x01\n\rDeleteObjects\x12\x33.aruna.api.storage.services.v1.DeleteObjectsRequest\x1a\x34.aruna.api.storage.services.v1.DeleteObjectsResponse\"1\x82\xd3\xe4\x93\x02+:\x01**&/v1/collection/{collection_id}/objects\x12\xb5\x01\n\rGetObjectByID\x12\x33.aruna.api.storage.services.v1.GetObjectByIDRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectByIDResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/collection/{collection_id}/object/{object_id}\x12\xa1\x01\n\nGetObjects\x12\x30.aruna.api.storage.services.v1.GetObjectsRequest\x1a\x31.aruna.api.storage.services.v1.GetObjectsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1/collection/{collection_id}/objects\x12\xce\x01\n\x12GetObjectRevisions\x12\x38.aruna.api.storage.services.v1.GetObjectRevisionsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectRevisionsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/revisions\x12\xda\x01\n\x17GetLatestObjectRevision\x12=.aruna.api.storage.services.v1.GetLatestObjectRevisionRequest\x1a>.aruna.api.storage.services.v1.GetLatestObjectRevisionResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/collection/{collection_id}/object/{object_id}/latest\x12\xce\x01\n\x12GetObjectEndpoints\x12\x38.aruna.api.storage.services.v1.GetObjectEndpointsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectEndpointsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/endpoints\x12\xcf\x01\n\x11\x41\x64\x64LabelsToObject\x12\x37.aruna.api.storage.services.v1.AddLabelsToObjectRequest\x1a\x38.aruna.api.storage.services.v1.AddLabelsToObjectResponse\"G\x82\xd3\xe4\x93\x02\x41:\x01*2</v1/collection/{collection_id}/object/{object_id}/add_labels\x12\xcb\x01\n\x10SetHooksOfObject\x12\x36.aruna.api.storage.services.v1.SetHooksOfObjectRequest\x1a\x37.aruna.api.storage.services.v1.SetHooksOfObjectResponse\"F\x82\xd3\xe4\x93\x02@:\x01*2;/v1/collection/{collection_id}/object/{object_id}/set_hooks\x12\xc0\x01\n\rGetReferences\x12\x33.aruna.api.storage.services.v1.GetReferencesRequest\x1a\x34.aruna.api.storage.services.v1.GetReferencesResponse\"D\x82\xd3\xe4\x93\x02>\x12</v1/collection/{collection_id}/object/{object_id}/references\x12\xba\x01\n\rGetObjectPath\x12\x33.aruna.api.storage.services.v1.GetObjectPathRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectPathResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/collection/{collection_id}/object/{object_id}/path\x12\xab\x01\n\x0eGetObjectPaths\x12\x34.aruna.api.storage.services.v1.GetObjectPathsRequest\x1a\x35.aruna.api.storage.services.v1.GetObjectPathsResponse\",\x82\xd3\xe4\x93\x02&\x12$/v1/collection/{collection_id}/paths\x12\xc6\x01\n\x10\x43reateObjectPath\x12\x36.aruna.api.storage.services.v1.CreateObjectPathRequest\x1a\x37.aruna.api.storage.services.v1.CreateObjectPathResponse\"A\x82\xd3\xe4\x93\x02;:\x01*\"6/v1/collection/{collection_id}/object/{object_id}/path\x12\xdd\x01\n\x17SetObjectPathVisibility\x12=.aruna.api.storage.services.v1.SetObjectPathVisibilityRequest\x1a>.aruna.api.storage.services.v1.SetObjectPathVisibilityResponse\"C\x82\xd3\xe4\x93\x02=:\x01*28/v1/collection/{collection_id}/path/{path=**}/visibility\x12\xa6\x01\n\x10GetObjectsByPath\x12\x36.aruna.api.storage.services.v1.GetObjectsByPathRequest\x1a\x37.aruna.api.storage.services.v1.GetObjectsByPathResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/path/object/{path=**}\x12\xd1\x01\n\x1dGetProjectCollectionIdsByPath\x12\x43.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathRequest\x1a\x44.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1/path/collection/{path=**}B\x8f\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2aruna/api/storage/services/v1/object_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\"\x17\n\x03URL\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\"\xf0\x02\n\x0bStageObject\x12\x1a\n\x08\x66ilename\x18\x01 \x01(\tR\x08\x66ilename\x12\x1f\n\x0b\x63ontent_len\x18\x04 \x01(\x03R\ncontentLen\x12;\n\x06source\x18\x05 \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x44\n\tdataclass\x18\x06 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12=\n\x06labels\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x08 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x19\n\x08sub_path\x18\t \x01(\tR\x07subPathJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xb9\x02\n\x1aInitializeNewObjectRequest\x12\x42\n\x06object\x18\x01 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x32\n\x15preferred_endpoint_id\x18\x04 \x01(\tR\x13preferredEndpointId\x12\x1c\n\tmultipart\x18\x05 \x01(\x08R\tmultipart\x12)\n\x10is_specification\x18\x06 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\x07 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\"|\n\x1bInitializeNewObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xb3\x01\n\x13GetUploadURLRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x1c\n\tmultipart\x18\x04 \x01(\x08R\tmultipart\x12\x1f\n\x0bpart_number\x18\x05 \x01(\x05R\npartNumber\"L\n\x14GetUploadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"8\n\x0e\x43ompletedParts\x12\x12\n\x04\x65tag\x18\x01 \x01(\tR\x04\x65tag\x12\x12\n\x04part\x18\x02 \x01(\x03R\x04part\"Y\n\x15GetDownloadURLRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"N\n\x16GetDownloadURLResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"]\n\x1cGetDownloadLinksBatchRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"W\n\x1dGetDownloadLinksBatchResponse\x12\x36\n\x04urls\x18\x01 \x03(\x0b\x32\".aruna.api.storage.services.v1.URLR\x04urls\"a\n CreateDownloadLinksStreamRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x18\n\x07objects\x18\x02 \x03(\tR\x07objects\"Y\n!CreateDownloadLinksStreamResponse\x12\x34\n\x03url\x18\x01 \x01(\x0b\x32\".aruna.api.storage.services.v1.URLR\x03url\"\xc8\x02\n\x1a\x46inishObjectStagingRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1b\n\tupload_id\x18\x02 \x01(\tR\x08uploadId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\x12\x35\n\x04hash\x18\x04 \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hash\x12\x1b\n\tno_upload\x18\x05 \x01(\x08R\x08noUpload\x12V\n\x0f\x63ompleted_parts\x18\x06 \x03(\x0b\x32-.aruna.api.storage.services.v1.CompletedPartsR\x0e\x63ompletedParts\x12\x1f\n\x0b\x61uto_update\x18\x07 \x01(\x08R\nautoUpdate\"Z\n\x1b\x46inishObjectStagingResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\xf2\x02\n\x13UpdateObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x42\n\x06object\x18\x03 \x01(\x0b\x32*.aruna.api.storage.services.v1.StageObjectR\x06object\x12\x1a\n\x08reupload\x18\x04 \x01(\x08R\x08reupload\x12\x32\n\x15preferred_endpoint_id\x18\x05 \x01(\tR\x13preferredEndpointId\x12\x1d\n\nmulti_part\x18\x06 \x01(\x08R\tmultiPart\x12)\n\x10is_specification\x18\x07 \x01(\x08R\x0fisSpecification\x12\x35\n\x04hash\x18\t \x01(\x0b\x32!.aruna.api.storage.models.v1.HashR\x04hashJ\x04\x08\x08\x10\t\"w\n\x14UpdateObjectResponse\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12\x1d\n\nstaging_id\x18\x02 \x01(\tR\tstagingId\x12#\n\rcollection_id\x18\x03 \x01(\tR\x0c\x63ollectionId\"\xec\x01\n\x1c\x43reateObjectReferenceRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\x12\x1c\n\twriteable\x18\x04 \x01(\x08R\twriteable\x12\x1f\n\x0b\x61uto_update\x18\x05 \x01(\x08R\nautoUpdate\x12\x19\n\x08sub_path\x18\x06 \x01(\tR\x07subPath\"\x1f\n\x1d\x43reateObjectReferenceResponse\"\x88\x01\n\x12\x43loneObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x30\n\x14target_collection_id\x18\x03 \x01(\tR\x12targetCollectionId\"R\n\x13\x43loneObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x94\x01\n\x13\x44\x65leteObjectRequest\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x16\n\x14\x44\x65leteObjectResponse\"\x97\x01\n\x14\x44\x65leteObjectsRequest\x12\x1d\n\nobject_ids\x18\x01 \x03(\tR\tobjectIds\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\x12\x14\n\x05\x66orce\x18\x04 \x01(\x08R\x05\x66orce\"\x17\n\x15\x44\x65leteObjectsResponse\"t\n\rObjectWithURL\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\x12\x14\n\x05paths\x18\x03 \x03(\tR\x05paths\"s\n\x14GetObjectByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"]\n\x15GetObjectByIDResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"\xf5\x01\n\x11GetObjectsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12K\n\x0cpage_request\x18\x02 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12S\n\x0flabel_id_filter\x18\x03 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\rlabelIdFilter\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"\\\n\x12GetObjectsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"\xc5\x01\n\x19GetObjectRevisionsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\x12\x19\n\x08with_url\x18\x04 \x01(\x08R\x07withUrl\"d\n\x1aGetObjectRevisionsResponse\x12\x46\n\x07objects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x07objects\"}\n\x1eGetLatestObjectRevisionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08with_url\x18\x03 \x01(\x08R\x07withUrl\"g\n\x1fGetLatestObjectRevisionResponse\x12\x44\n\x06object\x18\x01 \x01(\x0b\x32,.aruna.api.storage.services.v1.ObjectWithURLR\x06object\"]\n\x19GetObjectEndpointsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\"a\n\x1aGetObjectEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"\xa7\x01\n\x18\x41\x64\x64LabelsToObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12I\n\rlabels_to_add\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x0blabelsToAdd\"X\n\x19\x41\x64\x64LabelsToObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x98\x01\n\x17SetHooksOfObjectRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12;\n\x05hooks\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\"W\n\x18SetHooksOfObjectResponse\x12;\n\x06object\x18\x01 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object\"\x7f\n\x14GetReferencesRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12%\n\x0ewith_revisions\x18\x03 \x01(\x08R\rwithRevisions\"\x9f\x01\n\x0fObjectReference\x12\x1b\n\tobject_id\x18\x01 \x01(\tR\x08objectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\'\n\x0frevision_number\x18\x03 \x01(\x03R\x0erevisionNumber\x12!\n\x0cis_writeable\x18\x04 \x01(\x08R\x0bisWriteable\"g\n\x15GetReferencesResponse\x12N\n\nreferences\x18\x01 \x03(\x0b\x32..aruna.api.storage.services.v1.ObjectReferenceR\nreferences\":\n\x04Path\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x02 \x01(\x08R\nvisibility\"\x83\x01\n\x14GetObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12)\n\x10include_inactive\x18\x03 \x01(\x08R\x0fincludeInactive\"_\n\x15GetObjectPathResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"g\n\x15GetObjectPathsRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12)\n\x10include_inactive\x18\x02 \x01(\x08R\x0fincludeInactive\"`\n\x16GetObjectPathsResponse\x12\x46\n\x0cobject_paths\x18\x01 \x03(\x0b\x32#.aruna.api.storage.services.v1.PathR\x0bobjectPaths\"v\n\x17\x43reateObjectPathRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x1b\n\tobject_id\x18\x02 \x01(\tR\x08objectId\x12\x19\n\x08sub_path\x18\x03 \x01(\tR\x07subPath\"S\n\x18\x43reateObjectPathResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"y\n\x1eSetObjectPathVisibilityRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x1e\n\nvisibility\x18\x03 \x01(\x08R\nvisibility\"Z\n\x1fSetObjectPathVisibilityResponse\x12\x37\n\x04path\x18\x01 \x01(\x0b\x32#.aruna.api.storage.services.v1.PathR\x04path\"T\n\x17GetObjectsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12%\n\x0ewith_revisions\x18\x02 \x01(\x08R\rwithRevisions\":\n$GetProjectCollectionIdsByPathRequest\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"k\n%GetProjectCollectionIdsByPathResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"W\n\x18GetObjectsByPathResponse\x12;\n\x06object\x18\x03 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x06object2\x99\'\n\rObjectService\x12\xbe\x01\n\x13InitializeNewObject\x12\x39.aruna.api.storage.services.v1.InitializeNewObjectRequest\x1a:.aruna.api.storage.services.v1.InitializeNewObjectResponse\"0\x82\xd3\xe4\x93\x02*:\x01*\"%/v1/collection/{collection_id}/object\x12\xcd\x01\n\x0cGetUploadURL\x12\x32.aruna.api.storage.services.v1.GetUploadURLRequest\x1a\x33.aruna.api.storage.services.v1.GetUploadURLResponse\"T\x82\xd3\xe4\x93\x02N\x12L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/upload\x12\xc1\x01\n\x0eGetDownloadURL\x12\x34.aruna.api.storage.services.v1.GetDownloadURLRequest\x1a\x35.aruna.api.storage.services.v1.GetDownloadURLResponse\"B\x82\xd3\xe4\x93\x02<\x12:/v1/collection/{collection_id}/object/{object_id}/download\x12\xc8\x01\n\x15GetDownloadLinksBatch\x12;.aruna.api.storage.services.v1.GetDownloadLinksBatchRequest\x1a<.aruna.api.storage.services.v1.GetDownloadLinksBatchResponse\"4\x82\xd3\xe4\x93\x02.\x12,/v1/collection/{collection_id}/objects/batch\x12\xda\x01\n\x19\x43reateDownloadLinksStream\x12?.aruna.api.storage.services.v1.CreateDownloadLinksStreamRequest\x1a@.aruna.api.storage.services.v1.CreateDownloadLinksStreamResponse\"8\x82\xd3\xe4\x93\x02\x32:\x01*\"-/v1/collection/{collection_id}/objects/stream0\x01\x12\xe5\x01\n\x13\x46inishObjectStaging\x12\x39.aruna.api.storage.services.v1.FinishObjectStagingRequest\x1a:.aruna.api.storage.services.v1.FinishObjectStagingResponse\"W\x82\xd3\xe4\x93\x02Q:\x01*2L/v1/collection/{collection_id}/object/{object_id}/staging/{upload_id}/finish\x12\xbc\x01\n\x0cUpdateObject\x12\x32.aruna.api.storage.services.v1.UpdateObjectRequest\x1a\x33.aruna.api.storage.services.v1.UpdateObjectResponse\"C\x82\xd3\xe4\x93\x02=:\x01*\"8/v1/collection/{collection_id}/object/{object_id}/update\x12\xf1\x01\n\x15\x43reateObjectReference\x12;.aruna.api.storage.services.v1.CreateObjectReferenceRequest\x1a<.aruna.api.storage.services.v1.CreateObjectReferenceResponse\"]\x82\xd3\xe4\x93\x02W:\x01*\"R/v1/collection/{collection_id}/object/{object_id}/reference/{target_collection_id}\x12\xb8\x01\n\x0b\x43loneObject\x12\x31.aruna.api.storage.services.v1.CloneObjectRequest\x1a\x32.aruna.api.storage.services.v1.CloneObjectResponse\"B\x82\xd3\xe4\x93\x02<:\x01*\"7/v1/collection/{collection_id}/object/{object_id}/clone\x12\xb5\x01\n\x0c\x44\x65leteObject\x12\x32.aruna.api.storage.services.v1.DeleteObjectRequest\x1a\x33.aruna.api.storage.services.v1.DeleteObjectResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01**1/v1/collection/{collection_id}/object/{object_id}\x12\xad\x01\n\rDeleteObjects\x12\x33.aruna.api.storage.services.v1.DeleteObjectsRequest\x1a\x34.aruna.api.storage.services.v1.DeleteObjectsResponse\"1\x82\xd3\xe4\x93\x02+:\x01**&/v1/collection/{collection_id}/objects\x12\xb5\x01\n\rGetObjectByID\x12\x33.aruna.api.storage.services.v1.GetObjectByIDRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectByIDResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/v1/collection/{collection_id}/object/{object_id}\x12\xa1\x01\n\nGetObjects\x12\x30.aruna.api.storage.services.v1.GetObjectsRequest\x1a\x31.aruna.api.storage.services.v1.GetObjectsResponse\".\x82\xd3\xe4\x93\x02(\x12&/v1/collection/{collection_id}/objects\x12\xce\x01\n\x12GetObjectRevisions\x12\x38.aruna.api.storage.services.v1.GetObjectRevisionsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectRevisionsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/revisions\x12\xda\x01\n\x17GetLatestObjectRevision\x12=.aruna.api.storage.services.v1.GetLatestObjectRevisionRequest\x1a>.aruna.api.storage.services.v1.GetLatestObjectRevisionResponse\"@\x82\xd3\xe4\x93\x02:\x12\x38/v1/collection/{collection_id}/object/{object_id}/latest\x12\xce\x01\n\x12GetObjectEndpoints\x12\x38.aruna.api.storage.services.v1.GetObjectEndpointsRequest\x1a\x39.aruna.api.storage.services.v1.GetObjectEndpointsResponse\"C\x82\xd3\xe4\x93\x02=\x12;/v1/collection/{collection_id}/object/{object_id}/endpoints\x12\xcf\x01\n\x11\x41\x64\x64LabelsToObject\x12\x37.aruna.api.storage.services.v1.AddLabelsToObjectRequest\x1a\x38.aruna.api.storage.services.v1.AddLabelsToObjectResponse\"G\x82\xd3\xe4\x93\x02\x41:\x01*2</v1/collection/{collection_id}/object/{object_id}/add_labels\x12\xcb\x01\n\x10SetHooksOfObject\x12\x36.aruna.api.storage.services.v1.SetHooksOfObjectRequest\x1a\x37.aruna.api.storage.services.v1.SetHooksOfObjectResponse\"F\x82\xd3\xe4\x93\x02@:\x01*2;/v1/collection/{collection_id}/object/{object_id}/set_hooks\x12\xc0\x01\n\rGetReferences\x12\x33.aruna.api.storage.services.v1.GetReferencesRequest\x1a\x34.aruna.api.storage.services.v1.GetReferencesResponse\"D\x82\xd3\xe4\x93\x02>\x12</v1/collection/{collection_id}/object/{object_id}/references\x12\xba\x01\n\rGetObjectPath\x12\x33.aruna.api.storage.services.v1.GetObjectPathRequest\x1a\x34.aruna.api.storage.services.v1.GetObjectPathResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/v1/collection/{collection_id}/object/{object_id}/path\x12\xab\x01\n\x0eGetObjectPaths\x12\x34.aruna.api.storage.services.v1.GetObjectPathsRequest\x1a\x35.aruna.api.storage.services.v1.GetObjectPathsResponse\",\x82\xd3\xe4\x93\x02&\x12$/v1/collection/{collection_id}/paths\x12\xc6\x01\n\x10\x43reateObjectPath\x12\x36.aruna.api.storage.services.v1.CreateObjectPathRequest\x1a\x37.aruna.api.storage.services.v1.CreateObjectPathResponse\"A\x82\xd3\xe4\x93\x02;:\x01*\"6/v1/collection/{collection_id}/object/{object_id}/path\x12\xdd\x01\n\x17SetObjectPathVisibility\x12=.aruna.api.storage.services.v1.SetObjectPathVisibilityRequest\x1a>.aruna.api.storage.services.v1.SetObjectPathVisibilityResponse\"C\x82\xd3\xe4\x93\x02=:\x01*28/v1/collection/{collection_id}/path/{path=**}/visibility\x12\xa6\x01\n\x10GetObjectsByPath\x12\x36.aruna.api.storage.services.v1.GetObjectsByPathRequest\x1a\x37.aruna.api.storage.services.v1.GetObjectsByPathResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/path/object/{path=**}\x12\xd1\x01\n\x1dGetProjectCollectionIdsByPath\x12\x43.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathRequest\x1a\x44.aruna.api.storage.services.v1.GetProjectCollectionIdsByPathResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/v1/path/collection/{path=**}B\x8f\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.object_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\rObjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
@@ -101,91 +101,91 @@
   _CREATEDOWNLOADLINKSSTREAMRESPONSE._serialized_start=1808
   _CREATEDOWNLOADLINKSSTREAMRESPONSE._serialized_end=1897
   _FINISHOBJECTSTAGINGREQUEST._serialized_start=1900
   _FINISHOBJECTSTAGINGREQUEST._serialized_end=2228
   _FINISHOBJECTSTAGINGRESPONSE._serialized_start=2230
   _FINISHOBJECTSTAGINGRESPONSE._serialized_end=2320
   _UPDATEOBJECTREQUEST._serialized_start=2323
-  _UPDATEOBJECTREQUEST._serialized_end=2709
-  _UPDATEOBJECTRESPONSE._serialized_start=2711
-  _UPDATEOBJECTRESPONSE._serialized_end=2830
-  _CREATEOBJECTREFERENCEREQUEST._serialized_start=2833
-  _CREATEOBJECTREFERENCEREQUEST._serialized_end=3069
-  _CREATEOBJECTREFERENCERESPONSE._serialized_start=3071
-  _CREATEOBJECTREFERENCERESPONSE._serialized_end=3102
-  _CLONEOBJECTREQUEST._serialized_start=3105
-  _CLONEOBJECTREQUEST._serialized_end=3241
-  _CLONEOBJECTRESPONSE._serialized_start=3243
-  _CLONEOBJECTRESPONSE._serialized_end=3325
-  _DELETEOBJECTREQUEST._serialized_start=3328
-  _DELETEOBJECTREQUEST._serialized_end=3476
-  _DELETEOBJECTRESPONSE._serialized_start=3478
-  _DELETEOBJECTRESPONSE._serialized_end=3500
-  _DELETEOBJECTSREQUEST._serialized_start=3503
-  _DELETEOBJECTSREQUEST._serialized_end=3654
-  _DELETEOBJECTSRESPONSE._serialized_start=3656
-  _DELETEOBJECTSRESPONSE._serialized_end=3679
-  _OBJECTWITHURL._serialized_start=3681
-  _OBJECTWITHURL._serialized_end=3797
-  _GETOBJECTBYIDREQUEST._serialized_start=3799
-  _GETOBJECTBYIDREQUEST._serialized_end=3914
-  _GETOBJECTBYIDRESPONSE._serialized_start=3916
-  _GETOBJECTBYIDRESPONSE._serialized_end=4009
-  _GETOBJECTSREQUEST._serialized_start=4012
-  _GETOBJECTSREQUEST._serialized_end=4257
-  _GETOBJECTSRESPONSE._serialized_start=4259
-  _GETOBJECTSRESPONSE._serialized_end=4351
-  _GETOBJECTREVISIONSREQUEST._serialized_start=4354
-  _GETOBJECTREVISIONSREQUEST._serialized_end=4551
-  _GETOBJECTREVISIONSRESPONSE._serialized_start=4553
-  _GETOBJECTREVISIONSRESPONSE._serialized_end=4653
-  _GETLATESTOBJECTREVISIONREQUEST._serialized_start=4655
-  _GETLATESTOBJECTREVISIONREQUEST._serialized_end=4780
-  _GETLATESTOBJECTREVISIONRESPONSE._serialized_start=4782
-  _GETLATESTOBJECTREVISIONRESPONSE._serialized_end=4885
-  _GETOBJECTENDPOINTSREQUEST._serialized_start=4887
-  _GETOBJECTENDPOINTSREQUEST._serialized_end=4980
-  _GETOBJECTENDPOINTSRESPONSE._serialized_start=4982
-  _GETOBJECTENDPOINTSRESPONSE._serialized_end=5079
-  _ADDLABELSTOOBJECTREQUEST._serialized_start=5082
-  _ADDLABELSTOOBJECTREQUEST._serialized_end=5249
-  _ADDLABELSTOOBJECTRESPONSE._serialized_start=5251
-  _ADDLABELSTOOBJECTRESPONSE._serialized_end=5339
-  _SETHOOKSOFOBJECTREQUEST._serialized_start=5342
-  _SETHOOKSOFOBJECTREQUEST._serialized_end=5494
-  _SETHOOKSOFOBJECTRESPONSE._serialized_start=5496
-  _SETHOOKSOFOBJECTRESPONSE._serialized_end=5583
-  _GETREFERENCESREQUEST._serialized_start=5585
-  _GETREFERENCESREQUEST._serialized_end=5712
-  _OBJECTREFERENCE._serialized_start=5715
-  _OBJECTREFERENCE._serialized_end=5874
-  _GETREFERENCESRESPONSE._serialized_start=5876
-  _GETREFERENCESRESPONSE._serialized_end=5979
-  _PATH._serialized_start=5981
-  _PATH._serialized_end=6039
-  _GETOBJECTPATHREQUEST._serialized_start=6042
-  _GETOBJECTPATHREQUEST._serialized_end=6173
-  _GETOBJECTPATHRESPONSE._serialized_start=6175
-  _GETOBJECTPATHRESPONSE._serialized_end=6270
-  _GETOBJECTPATHSREQUEST._serialized_start=6272
-  _GETOBJECTPATHSREQUEST._serialized_end=6375
-  _GETOBJECTPATHSRESPONSE._serialized_start=6377
-  _GETOBJECTPATHSRESPONSE._serialized_end=6473
-  _CREATEOBJECTPATHREQUEST._serialized_start=6475
-  _CREATEOBJECTPATHREQUEST._serialized_end=6593
-  _CREATEOBJECTPATHRESPONSE._serialized_start=6595
-  _CREATEOBJECTPATHRESPONSE._serialized_end=6678
-  _SETOBJECTPATHVISIBILITYREQUEST._serialized_start=6680
-  _SETOBJECTPATHVISIBILITYREQUEST._serialized_end=6801
-  _SETOBJECTPATHVISIBILITYRESPONSE._serialized_start=6803
-  _SETOBJECTPATHVISIBILITYRESPONSE._serialized_end=6893
-  _GETOBJECTSBYPATHREQUEST._serialized_start=6895
-  _GETOBJECTSBYPATHREQUEST._serialized_end=6979
-  _GETPROJECTCOLLECTIONIDSBYPATHREQUEST._serialized_start=6981
-  _GETPROJECTCOLLECTIONIDSBYPATHREQUEST._serialized_end=7039
-  _GETPROJECTCOLLECTIONIDSBYPATHRESPONSE._serialized_start=7041
-  _GETPROJECTCOLLECTIONIDSBYPATHRESPONSE._serialized_end=7148
-  _GETOBJECTSBYPATHRESPONSE._serialized_start=7150
-  _GETOBJECTSBYPATHRESPONSE._serialized_end=7237
-  _OBJECTSERVICE._serialized_start=7240
-  _OBJECTSERVICE._serialized_end=12257
+  _UPDATEOBJECTREQUEST._serialized_end=2693
+  _UPDATEOBJECTRESPONSE._serialized_start=2695
+  _UPDATEOBJECTRESPONSE._serialized_end=2814
+  _CREATEOBJECTREFERENCEREQUEST._serialized_start=2817
+  _CREATEOBJECTREFERENCEREQUEST._serialized_end=3053
+  _CREATEOBJECTREFERENCERESPONSE._serialized_start=3055
+  _CREATEOBJECTREFERENCERESPONSE._serialized_end=3086
+  _CLONEOBJECTREQUEST._serialized_start=3089
+  _CLONEOBJECTREQUEST._serialized_end=3225
+  _CLONEOBJECTRESPONSE._serialized_start=3227
+  _CLONEOBJECTRESPONSE._serialized_end=3309
+  _DELETEOBJECTREQUEST._serialized_start=3312
+  _DELETEOBJECTREQUEST._serialized_end=3460
+  _DELETEOBJECTRESPONSE._serialized_start=3462
+  _DELETEOBJECTRESPONSE._serialized_end=3484
+  _DELETEOBJECTSREQUEST._serialized_start=3487
+  _DELETEOBJECTSREQUEST._serialized_end=3638
+  _DELETEOBJECTSRESPONSE._serialized_start=3640
+  _DELETEOBJECTSRESPONSE._serialized_end=3663
+  _OBJECTWITHURL._serialized_start=3665
+  _OBJECTWITHURL._serialized_end=3781
+  _GETOBJECTBYIDREQUEST._serialized_start=3783
+  _GETOBJECTBYIDREQUEST._serialized_end=3898
+  _GETOBJECTBYIDRESPONSE._serialized_start=3900
+  _GETOBJECTBYIDRESPONSE._serialized_end=3993
+  _GETOBJECTSREQUEST._serialized_start=3996
+  _GETOBJECTSREQUEST._serialized_end=4241
+  _GETOBJECTSRESPONSE._serialized_start=4243
+  _GETOBJECTSRESPONSE._serialized_end=4335
+  _GETOBJECTREVISIONSREQUEST._serialized_start=4338
+  _GETOBJECTREVISIONSREQUEST._serialized_end=4535
+  _GETOBJECTREVISIONSRESPONSE._serialized_start=4537
+  _GETOBJECTREVISIONSRESPONSE._serialized_end=4637
+  _GETLATESTOBJECTREVISIONREQUEST._serialized_start=4639
+  _GETLATESTOBJECTREVISIONREQUEST._serialized_end=4764
+  _GETLATESTOBJECTREVISIONRESPONSE._serialized_start=4766
+  _GETLATESTOBJECTREVISIONRESPONSE._serialized_end=4869
+  _GETOBJECTENDPOINTSREQUEST._serialized_start=4871
+  _GETOBJECTENDPOINTSREQUEST._serialized_end=4964
+  _GETOBJECTENDPOINTSRESPONSE._serialized_start=4966
+  _GETOBJECTENDPOINTSRESPONSE._serialized_end=5063
+  _ADDLABELSTOOBJECTREQUEST._serialized_start=5066
+  _ADDLABELSTOOBJECTREQUEST._serialized_end=5233
+  _ADDLABELSTOOBJECTRESPONSE._serialized_start=5235
+  _ADDLABELSTOOBJECTRESPONSE._serialized_end=5323
+  _SETHOOKSOFOBJECTREQUEST._serialized_start=5326
+  _SETHOOKSOFOBJECTREQUEST._serialized_end=5478
+  _SETHOOKSOFOBJECTRESPONSE._serialized_start=5480
+  _SETHOOKSOFOBJECTRESPONSE._serialized_end=5567
+  _GETREFERENCESREQUEST._serialized_start=5569
+  _GETREFERENCESREQUEST._serialized_end=5696
+  _OBJECTREFERENCE._serialized_start=5699
+  _OBJECTREFERENCE._serialized_end=5858
+  _GETREFERENCESRESPONSE._serialized_start=5860
+  _GETREFERENCESRESPONSE._serialized_end=5963
+  _PATH._serialized_start=5965
+  _PATH._serialized_end=6023
+  _GETOBJECTPATHREQUEST._serialized_start=6026
+  _GETOBJECTPATHREQUEST._serialized_end=6157
+  _GETOBJECTPATHRESPONSE._serialized_start=6159
+  _GETOBJECTPATHRESPONSE._serialized_end=6254
+  _GETOBJECTPATHSREQUEST._serialized_start=6256
+  _GETOBJECTPATHSREQUEST._serialized_end=6359
+  _GETOBJECTPATHSRESPONSE._serialized_start=6361
+  _GETOBJECTPATHSRESPONSE._serialized_end=6457
+  _CREATEOBJECTPATHREQUEST._serialized_start=6459
+  _CREATEOBJECTPATHREQUEST._serialized_end=6577
+  _CREATEOBJECTPATHRESPONSE._serialized_start=6579
+  _CREATEOBJECTPATHRESPONSE._serialized_end=6662
+  _SETOBJECTPATHVISIBILITYREQUEST._serialized_start=6664
+  _SETOBJECTPATHVISIBILITYREQUEST._serialized_end=6785
+  _SETOBJECTPATHVISIBILITYRESPONSE._serialized_start=6787
+  _SETOBJECTPATHVISIBILITYRESPONSE._serialized_end=6877
+  _GETOBJECTSBYPATHREQUEST._serialized_start=6879
+  _GETOBJECTSBYPATHREQUEST._serialized_end=6963
+  _GETPROJECTCOLLECTIONIDSBYPATHREQUEST._serialized_start=6965
+  _GETPROJECTCOLLECTIONIDSBYPATHREQUEST._serialized_end=7023
+  _GETPROJECTCOLLECTIONIDSBYPATHRESPONSE._serialized_start=7025
+  _GETPROJECTCOLLECTIONIDSBYPATHRESPONSE._serialized_end=7132
+  _GETOBJECTSBYPATHRESPONSE._serialized_start=7134
+  _GETOBJECTSBYPATHRESPONSE._serialized_end=7221
+  _OBJECTSERVICE._serialized_start=7224
+  _OBJECTSERVICE._serialized_end=12241
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -467,34 +467,32 @@
 class URL(_message.Message):
     __slots__ = ["url"]
     URL_FIELD_NUMBER: _ClassVar[int]
     url: str
     def __init__(self, url: _Optional[str] = ...) -> None: ...
 
 class UpdateObjectRequest(_message.Message):
-    __slots__ = ["collection_id", "force", "hash", "is_specification", "multi_part", "object", "object_id", "preferred_endpoint_id", "reupload"]
+    __slots__ = ["collection_id", "hash", "is_specification", "multi_part", "object", "object_id", "preferred_endpoint_id", "reupload"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
-    FORCE_FIELD_NUMBER: _ClassVar[int]
     HASH_FIELD_NUMBER: _ClassVar[int]
     IS_SPECIFICATION_FIELD_NUMBER: _ClassVar[int]
     MULTI_PART_FIELD_NUMBER: _ClassVar[int]
     OBJECT_FIELD_NUMBER: _ClassVar[int]
     OBJECT_ID_FIELD_NUMBER: _ClassVar[int]
     PREFERRED_ENDPOINT_ID_FIELD_NUMBER: _ClassVar[int]
     REUPLOAD_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
-    force: bool
     hash: _models_pb2.Hash
     is_specification: bool
     multi_part: bool
     object: StageObject
     object_id: str
     preferred_endpoint_id: str
     reupload: bool
-    def __init__(self, object_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., object: _Optional[_Union[StageObject, _Mapping]] = ..., reupload: bool = ..., preferred_endpoint_id: _Optional[str] = ..., multi_part: bool = ..., is_specification: bool = ..., force: bool = ..., hash: _Optional[_Union[_models_pb2.Hash, _Mapping]] = ...) -> None: ...
+    def __init__(self, object_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., object: _Optional[_Union[StageObject, _Mapping]] = ..., reupload: bool = ..., preferred_endpoint_id: _Optional[str] = ..., multi_part: bool = ..., is_specification: bool = ..., hash: _Optional[_Union[_models_pb2.Hash, _Mapping]] = ...) -> None: ...
 
 class UpdateObjectResponse(_message.Message):
     __slots__ = ["collection_id", "object_id", "staging_id"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     OBJECT_ID_FIELD_NUMBER: _ClassVar[int]
     STAGING_ID_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse2\xb1\x0c\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.0.0-rc.9*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.1*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.0.0-rc.9*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.1*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
@@ -36,14 +36,16 @@
   _PROJECTSERVICE.methods_by_name['DestroyProject']._serialized_options = b'\202\323\344\223\002\032*\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['UpdateProject']._options = None
   _PROJECTSERVICE.methods_by_name['UpdateProject']._serialized_options = b'\202\323\344\223\002\032\032\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['RemoveUserFromProject']._options = None
   _PROJECTSERVICE.methods_by_name['RemoveUserFromProject']._serialized_options = b'\202\323\344\223\002&*$/v1/project/{project_id}/remove_user'
   _PROJECTSERVICE.methods_by_name['GetUserPermissionsForProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002#\022!/v1/project/{project_id}/get_user'
+  _PROJECTSERVICE.methods_by_name['GetAllUserPermissionsForProject']._options = None
+  _PROJECTSERVICE.methods_by_name['GetAllUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002$\022\"/v1/project/{project_id}/get_users'
   _PROJECTSERVICE.methods_by_name['EditUserPermissionsForProject']._options = None
   _PROJECTSERVICE.methods_by_name['EditUserPermissionsForProject']._serialized_options = b'\202\323\344\223\002\':\001*2\"/v1/project/{project_id}/edit_user'
   _CREATEPROJECTREQUEST._serialized_start=204
   _CREATEPROJECTREQUEST._serialized_end=280
   _CREATEPROJECTRESPONSE._serialized_start=282
   _CREATEPROJECTRESPONSE._serialized_end=336
   _ADDUSERTOPROJECTREQUEST._serialized_start=339
@@ -74,10 +76,16 @@
   _GETUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1281
   _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1284
   _GETUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1422
   _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1425
   _EDITUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1583
   _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1585
   _EDITUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1624
-  _PROJECTSERVICE._serialized_start=1627
-  _PROJECTSERVICE._serialized_end=3212
+  _USERWITHPROJECTPERMISSIONS._serialized_start=1627
+  _USERWITHPROJECTPERMISSIONS._serialized_end=1801
+  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_start=1803
+  _GETALLUSERPERMISSIONSFORPROJECTREQUEST._serialized_end=1874
+  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_start=1876
+  _GETALLUSERPERMISSIONSFORPROJECTRESPONSE._serialized_end=1998
+  _PROJECTSERVICE._serialized_start=2001
+  _PROJECTSERVICE._serialized_end=3809
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -52,14 +52,26 @@
     user_permission: _auth_pb2.ProjectPermission
     def __init__(self, project_id: _Optional[str] = ..., user_permission: _Optional[_Union[_auth_pb2.ProjectPermission, _Mapping]] = ...) -> None: ...
 
 class EditUserPermissionsForProjectResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
+class GetAllUserPermissionsForProjectRequest(_message.Message):
+    __slots__ = ["project_id"]
+    PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
+    project_id: str
+    def __init__(self, project_id: _Optional[str] = ...) -> None: ...
+
+class GetAllUserPermissionsForProjectResponse(_message.Message):
+    __slots__ = ["users"]
+    USERS_FIELD_NUMBER: _ClassVar[int]
+    users: _containers.RepeatedCompositeFieldContainer[UserWithProjectPermissions]
+    def __init__(self, users: _Optional[_Iterable[_Union[UserWithProjectPermissions, _Mapping]]] = ...) -> None: ...
+
 class GetProjectRequest(_message.Message):
     __slots__ = ["project_id"]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     project_id: str
     def __init__(self, project_id: _Optional[str] = ...) -> None: ...
 
 class GetProjectResponse(_message.Message):
@@ -115,7 +127,15 @@
     def __init__(self, project_id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
 
 class UpdateProjectResponse(_message.Message):
     __slots__ = ["project"]
     PROJECT_FIELD_NUMBER: _ClassVar[int]
     project: _auth_pb2.ProjectOverview
     def __init__(self, project: _Optional[_Union[_auth_pb2.ProjectOverview, _Mapping]] = ...) -> None: ...
+
+class UserWithProjectPermissions(_message.Message):
+    __slots__ = ["user", "user_permissions"]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    USER_PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
+    user: _auth_pb2.User
+    user_permissions: _auth_pb2.ProjectPermission
+    def __init__(self, user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ..., user_permissions: _Optional[_Union[_auth_pb2.ProjectPermission, _Mapping]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,19 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.RemoveUserFromProjectResponse.FromString,
                 )
         self.GetUserPermissionsForProject = channel.unary_unary(
                 '/aruna.api.storage.services.v1.ProjectService/GetUserPermissionsForProject',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectResponse.FromString,
                 )
+        self.GetAllUserPermissionsForProject = channel.unary_unary(
+                '/aruna.api.storage.services.v1.ProjectService/GetAllUserPermissionsForProject',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectResponse.FromString,
+                )
         self.EditUserPermissionsForProject = channel.unary_unary(
                 '/aruna.api.storage.services.v1.ProjectService/EditUserPermissionsForProject',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.EditUserPermissionsForProjectRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.EditUserPermissionsForProjectResponse.FromString,
                 )
 
 
@@ -155,14 +160,25 @@
 
         Get the user_permission of a specific user for the project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetAllUserPermissionsForProject(self, request, context):
+        """GetAllUserPermissionsForProject
+
+        Status: ALPHA
+
+        Get the user_permission of a specific user for the project.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def EditUserPermissionsForProject(self, request, context):
         """EditUserPermissionsForProject
 
         Status: STABLE
 
         Modifies the user_permission of a specific user for the project.
         """
@@ -209,14 +225,19 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.RemoveUserFromProjectResponse.SerializeToString,
             ),
             'GetUserPermissionsForProject': grpc.unary_unary_rpc_method_handler(
                     servicer.GetUserPermissionsForProject,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectResponse.SerializeToString,
             ),
+            'GetAllUserPermissionsForProject': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAllUserPermissionsForProject,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectResponse.SerializeToString,
+            ),
             'EditUserPermissionsForProject': grpc.unary_unary_rpc_method_handler(
                     servicer.EditUserPermissionsForProject,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.EditUserPermissionsForProjectRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.EditUserPermissionsForProjectResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -364,14 +385,31 @@
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.ProjectService/GetUserPermissionsForProject',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetUserPermissionsForProjectResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetAllUserPermissionsForProject(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.ProjectService/GetAllUserPermissionsForProject',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_project__service__pb2.GetAllUserPermissionsForProjectResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def EditUserPermissionsForProject(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0aruna/api/storage/services/v1/user_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"E\n\tExpiresAt\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\"8\n\x13RegisterUserRequest\x12!\n\x0c\x64isplay_name\x18\x01 \x01(\tR\x0b\x64isplayName\"/\n\x14RegisterUserResponse\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x81\x02\n\x15\x43reateAPITokenRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12G\n\nexpires_at\x18\x04 \x01(\x0b\x32(.aruna.api.storage.services.v1.ExpiresAtR\texpiresAt\x12G\n\npermission\x18\x05 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\"\xbd\x01\n\x16\x43reateAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\x12\"\n\rs3_access_key\x18\x03 \x01(\tR\x0bs3AccessKey\x12\"\n\rs3_secret_key\x18\x04 \x01(\tR\x0bs3SecretKey\"/\n\x12GetAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"O\n\x13GetAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"\x15\n\x13GetAPITokensRequest\"P\n\x14GetAPITokensResponse\x12\x38\n\x05token\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"2\n\x15\x44\x65leteAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"\x18\n\x16\x44\x65leteAPITokenResponse\"1\n\x16\x44\x65leteAPITokensRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x19\n\x17\x44\x65leteAPITokensResponse\")\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\xa9\x01\n\x0fGetUserResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12_\n\x13project_permissions\x18\x02 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x12projectPermissions\"H\n\x1cUpdateUserDisplayNameRequest\x12(\n\x10new_display_name\x18\x01 \x01(\tR\x0enewDisplayName\"V\n\x1dUpdateUserDisplayNameResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\"1\n\x16GetUserProjectsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"S\n\x0bUserProject\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"a\n\x17GetUserProjectsResponse\x12\x46\n\x08projects\x18\x01 \x03(\x0b\x32*.aruna.api.storage.services.v1.UserProjectR\x08projects\".\n\x13\x41\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x16\n\x14\x41\x63tivateUserResponse\"\x1d\n\x1bGetNotActivatedUsersRequest\"W\n\x1cGetNotActivatedUsersResponse\x12\x37\n\x05users\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v1.UserR\x05users2\xdb\r\n\x0bUserService\x12\x95\x01\n\x0cRegisterUser\x12\x32.aruna.api.storage.services.v1.RegisterUserRequest\x1a\x33.aruna.api.storage.services.v1.RegisterUserResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/v1/auth/register\x12\x9f\x01\n\x0c\x41\x63tivateUser\x12\x32.aruna.api.storage.services.v1.ActivateUserRequest\x1a\x33.aruna.api.storage.services.v1.ActivateUserResponse\"&\x82\xd3\xe4\x93\x02 :\x01*2\x1b/v1/user/{user_id}/activate\x12\x98\x01\n\x0e\x43reateAPIToken\x12\x34.aruna.api.storage.services.v1.CreateAPITokenRequest\x1a\x35.aruna.api.storage.services.v1.CreateAPITokenResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/v1/auth/token\x12\x97\x01\n\x0bGetAPIToken\x12\x31.aruna.api.storage.services.v1.GetAPITokenRequest\x1a\x32.aruna.api.storage.services.v1.GetAPITokenResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/auth/token/{token_id}\x12\x90\x01\n\x0cGetAPITokens\x12\x32.aruna.api.storage.services.v1.GetAPITokensRequest\x1a\x33.aruna.api.storage.services.v1.GetAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/auth/tokens\x12\xa0\x01\n\x0e\x44\x65leteAPIToken\x12\x34.aruna.api.storage.services.v1.DeleteAPITokenRequest\x1a\x35.aruna.api.storage.services.v1.DeleteAPITokenResponse\"!\x82\xd3\xe4\x93\x02\x1b*\x19/v1/auth/token/{token_id}\x12\x99\x01\n\x0f\x44\x65leteAPITokens\x12\x35.aruna.api.storage.services.v1.DeleteAPITokensRequest\x1a\x36.aruna.api.storage.services.v1.DeleteAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11*\x0f/v1/auth/tokens\x12z\n\x07GetUser\x12-.aruna.api.storage.services.v1.GetUserRequest\x1a..aruna.api.storage.services.v1.GetUserResponse\"\x10\x82\xd3\xe4\x93\x02\n\x12\x08/v1/user\x12\xb4\x01\n\x15UpdateUserDisplayName\x12;.aruna.api.storage.services.v1.UpdateUserDisplayNameRequest\x1a<.aruna.api.storage.services.v1.UpdateUserDisplayNameResponse\" \x82\xd3\xe4\x93\x02\x1a:\x01*2\x15/v1/user/display_name\x12\xa5\x01\n\x0fGetUserProjects\x12\x35.aruna.api.storage.services.v1.GetUserProjectsRequest\x1a\x36.aruna.api.storage.services.v1.GetUserProjectsResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/user/{user_id}/projects\x12\xaf\x01\n\x14GetNotActivatedUsers\x12:.aruna.api.storage.services.v1.GetNotActivatedUsersRequest\x1a;.aruna.api.storage.services.v1.GetNotActivatedUsersResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v1/user/not_activatedB\x8d\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0bUserServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0aruna/api/storage/services/v1/user_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"E\n\tExpiresAt\x12\x38\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\"h\n\x13RegisterUserRequest\x12!\n\x0c\x64isplay_name\x18\x01 \x01(\tR\x0b\x64isplayName\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\x12\x18\n\x07project\x18\x03 \x01(\tR\x07project\"/\n\x14RegisterUserResponse\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\xa0\x02\n\x15\x43reateAPITokenRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12G\n\nexpires_at\x18\x04 \x01(\x0b\x32(.aruna.api.storage.services.v1.ExpiresAtR\texpiresAt\x12G\n\npermission\x18\x05 \x01(\x0e\x32\'.aruna.api.storage.models.v1.PermissionR\npermission\x12\x1d\n\nis_session\x18\x06 \x01(\x08R\tisSession\"\xbd\x01\n\x16\x43reateAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\x12!\n\x0ctoken_secret\x18\x02 \x01(\tR\x0btokenSecret\x12\"\n\rs3_access_key\x18\x03 \x01(\tR\x0bs3AccessKey\x12\"\n\rs3_secret_key\x18\x04 \x01(\tR\x0bs3SecretKey\"/\n\x12GetAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"O\n\x13GetAPITokenResponse\x12\x38\n\x05token\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"\x15\n\x13GetAPITokensRequest\"P\n\x14GetAPITokensResponse\x12\x38\n\x05token\x18\x01 \x03(\x0b\x32\".aruna.api.storage.models.v1.TokenR\x05token\"2\n\x15\x44\x65leteAPITokenRequest\x12\x19\n\x08token_id\x18\x01 \x01(\tR\x07tokenId\"\x18\n\x16\x44\x65leteAPITokenResponse\"1\n\x16\x44\x65leteAPITokensRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x19\n\x17\x44\x65leteAPITokensResponse\")\n\x0eGetUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\xa9\x01\n\x0fGetUserResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12_\n\x13project_permissions\x18\x02 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x12projectPermissions\"H\n\x1cUpdateUserDisplayNameRequest\x12(\n\x10new_display_name\x18\x01 \x01(\tR\x0enewDisplayName\"V\n\x1dUpdateUserDisplayNameResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\"1\n\x16GetUserProjectsRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"S\n\x0bUserProject\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"a\n\x17GetUserProjectsResponse\x12\x46\n\x08projects\x18\x01 \x03(\x0b\x32*.aruna.api.storage.services.v1.UserProjectR\x08projects\"\x83\x01\n\x13\x41\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12S\n\rproject_perms\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0cprojectPerms\"\x16\n\x14\x41\x63tivateUserResponse\"\x1d\n\x1bGetNotActivatedUsersRequest\"W\n\x1cGetNotActivatedUsersResponse\x12\x37\n\x05users\x18\x01 \x03(\x0b\x32!.aruna.api.storage.models.v1.UserR\x05users\"E\n\x12GetAllUsersRequest\x12/\n\x13include_permissions\x18\x01 \x01(\x08R\x12includePermissions\"\x9b\x01\n\rUserWithPerms\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12S\n\rproject_perms\x18\x02 \x03(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0cprojectPerms\"k\n\x13GetAllUsersResponse\x12T\n\x0fuser_with_perms\x18\x01 \x03(\x0b\x32,.aruna.api.storage.services.v1.UserWithPermsR\ruserWithPerms\"0\n\x15\x44\x65\x61\x63tivateUserRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\"\x18\n\x16\x44\x65\x61\x63tivateUserResponse\"N\n\x16UpdateUserEmailRequest\x12\x17\n\x07user_id\x18\x01 \x01(\tR\x06userId\x12\x1b\n\tnew_email\x18\x02 \x01(\tR\x08newEmail\"P\n\x17UpdateUserEmailResponse\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user2\xb0\x11\n\x0bUserService\x12\x95\x01\n\x0cRegisterUser\x12\x32.aruna.api.storage.services.v1.RegisterUserRequest\x1a\x33.aruna.api.storage.services.v1.RegisterUserResponse\"\x1c\x82\xd3\xe4\x93\x02\x16:\x01*\"\x11/v1/auth/register\x12\xa7\x01\n\x0e\x44\x65\x61\x63tivateUser\x12\x34.aruna.api.storage.services.v1.DeactivateUserRequest\x1a\x35.aruna.api.storage.services.v1.DeactivateUserResponse\"(\x82\xd3\xe4\x93\x02\":\x01*2\x1d/v1/user/{user_id}/deactivate\x12\x9f\x01\n\x0c\x41\x63tivateUser\x12\x32.aruna.api.storage.services.v1.ActivateUserRequest\x1a\x33.aruna.api.storage.services.v1.ActivateUserResponse\"&\x82\xd3\xe4\x93\x02 :\x01*2\x1b/v1/user/{user_id}/activate\x12\x98\x01\n\x0e\x43reateAPIToken\x12\x34.aruna.api.storage.services.v1.CreateAPITokenRequest\x1a\x35.aruna.api.storage.services.v1.CreateAPITokenResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/v1/auth/token\x12\x97\x01\n\x0bGetAPIToken\x12\x31.aruna.api.storage.services.v1.GetAPITokenRequest\x1a\x32.aruna.api.storage.services.v1.GetAPITokenResponse\"!\x82\xd3\xe4\x93\x02\x1b\x12\x19/v1/auth/token/{token_id}\x12\x90\x01\n\x0cGetAPITokens\x12\x32.aruna.api.storage.services.v1.GetAPITokensRequest\x1a\x33.aruna.api.storage.services.v1.GetAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/v1/auth/tokens\x12\xa0\x01\n\x0e\x44\x65leteAPIToken\x12\x34.aruna.api.storage.services.v1.DeleteAPITokenRequest\x1a\x35.aruna.api.storage.services.v1.DeleteAPITokenResponse\"!\x82\xd3\xe4\x93\x02\x1b*\x19/v1/auth/token/{token_id}\x12\x99\x01\n\x0f\x44\x65leteAPITokens\x12\x35.aruna.api.storage.services.v1.DeleteAPITokensRequest\x1a\x36.aruna.api.storage.services.v1.DeleteAPITokensResponse\"\x17\x82\xd3\xe4\x93\x02\x11*\x0f/v1/auth/tokens\x12z\n\x07GetUser\x12-.aruna.api.storage.services.v1.GetUserRequest\x1a..aruna.api.storage.services.v1.GetUserResponse\"\x10\x82\xd3\xe4\x93\x02\n\x12\x08/v1/user\x12\xb4\x01\n\x15UpdateUserDisplayName\x12;.aruna.api.storage.services.v1.UpdateUserDisplayNameRequest\x1a<.aruna.api.storage.services.v1.UpdateUserDisplayNameResponse\" \x82\xd3\xe4\x93\x02\x1a:\x01*2\x15/v1/user/display_name\x12\x9b\x01\n\x0fUpdateUserEmail\x12\x35.aruna.api.storage.services.v1.UpdateUserEmailRequest\x1a\x36.aruna.api.storage.services.v1.UpdateUserEmailResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*2\x0e/v1/user/email\x12\xa5\x01\n\x0fGetUserProjects\x12\x35.aruna.api.storage.services.v1.GetUserProjectsRequest\x1a\x36.aruna.api.storage.services.v1.GetUserProjectsResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/v1/user/{user_id}/projects\x12\xaf\x01\n\x14GetNotActivatedUsers\x12:.aruna.api.storage.services.v1.GetNotActivatedUsersRequest\x1a;.aruna.api.storage.services.v1.GetNotActivatedUsersResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\x12\x16/v1/user/not_activated\x12\x8a\x01\n\x0bGetAllUsers\x12\x31.aruna.api.storage.services.v1.GetAllUsersRequest\x1a\x32.aruna.api.storage.services.v1.GetAllUsersResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/user/allB\x8d\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0bUserServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.user_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\013UserServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
   _USERSERVICE.methods_by_name['RegisterUser']._options = None
   _USERSERVICE.methods_by_name['RegisterUser']._serialized_options = b'\202\323\344\223\002\026:\001*\"\021/v1/auth/register'
+  _USERSERVICE.methods_by_name['DeactivateUser']._options = None
+  _USERSERVICE.methods_by_name['DeactivateUser']._serialized_options = b'\202\323\344\223\002\":\001*2\035/v1/user/{user_id}/deactivate'
   _USERSERVICE.methods_by_name['ActivateUser']._options = None
   _USERSERVICE.methods_by_name['ActivateUser']._serialized_options = b'\202\323\344\223\002 :\001*2\033/v1/user/{user_id}/activate'
   _USERSERVICE.methods_by_name['CreateAPIToken']._options = None
   _USERSERVICE.methods_by_name['CreateAPIToken']._serialized_options = b'\202\323\344\223\002\023:\001*\"\016/v1/auth/token'
   _USERSERVICE.methods_by_name['GetAPIToken']._options = None
   _USERSERVICE.methods_by_name['GetAPIToken']._serialized_options = b'\202\323\344\223\002\033\022\031/v1/auth/token/{token_id}'
   _USERSERVICE.methods_by_name['GetAPITokens']._options = None
@@ -38,62 +40,80 @@
   _USERSERVICE.methods_by_name['DeleteAPIToken']._serialized_options = b'\202\323\344\223\002\033*\031/v1/auth/token/{token_id}'
   _USERSERVICE.methods_by_name['DeleteAPITokens']._options = None
   _USERSERVICE.methods_by_name['DeleteAPITokens']._serialized_options = b'\202\323\344\223\002\021*\017/v1/auth/tokens'
   _USERSERVICE.methods_by_name['GetUser']._options = None
   _USERSERVICE.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002\n\022\010/v1/user'
   _USERSERVICE.methods_by_name['UpdateUserDisplayName']._options = None
   _USERSERVICE.methods_by_name['UpdateUserDisplayName']._serialized_options = b'\202\323\344\223\002\032:\001*2\025/v1/user/display_name'
+  _USERSERVICE.methods_by_name['UpdateUserEmail']._options = None
+  _USERSERVICE.methods_by_name['UpdateUserEmail']._serialized_options = b'\202\323\344\223\002\023:\001*2\016/v1/user/email'
   _USERSERVICE.methods_by_name['GetUserProjects']._options = None
   _USERSERVICE.methods_by_name['GetUserProjects']._serialized_options = b'\202\323\344\223\002\035\022\033/v1/user/{user_id}/projects'
   _USERSERVICE.methods_by_name['GetNotActivatedUsers']._options = None
   _USERSERVICE.methods_by_name['GetNotActivatedUsers']._serialized_options = b'\202\323\344\223\002\030\022\026/v1/user/not_activated'
+  _USERSERVICE.methods_by_name['GetAllUsers']._options = None
+  _USERSERVICE.methods_by_name['GetAllUsers']._serialized_options = b'\202\323\344\223\002\016\022\014/v1/user/all'
   _EXPIRESAT._serialized_start=186
   _EXPIRESAT._serialized_end=255
   _REGISTERUSERREQUEST._serialized_start=257
-  _REGISTERUSERREQUEST._serialized_end=313
-  _REGISTERUSERRESPONSE._serialized_start=315
-  _REGISTERUSERRESPONSE._serialized_end=362
-  _CREATEAPITOKENREQUEST._serialized_start=365
-  _CREATEAPITOKENREQUEST._serialized_end=622
-  _CREATEAPITOKENRESPONSE._serialized_start=625
-  _CREATEAPITOKENRESPONSE._serialized_end=814
-  _GETAPITOKENREQUEST._serialized_start=816
-  _GETAPITOKENREQUEST._serialized_end=863
-  _GETAPITOKENRESPONSE._serialized_start=865
-  _GETAPITOKENRESPONSE._serialized_end=944
-  _GETAPITOKENSREQUEST._serialized_start=946
-  _GETAPITOKENSREQUEST._serialized_end=967
-  _GETAPITOKENSRESPONSE._serialized_start=969
-  _GETAPITOKENSRESPONSE._serialized_end=1049
-  _DELETEAPITOKENREQUEST._serialized_start=1051
-  _DELETEAPITOKENREQUEST._serialized_end=1101
-  _DELETEAPITOKENRESPONSE._serialized_start=1103
-  _DELETEAPITOKENRESPONSE._serialized_end=1127
-  _DELETEAPITOKENSREQUEST._serialized_start=1129
-  _DELETEAPITOKENSREQUEST._serialized_end=1178
-  _DELETEAPITOKENSRESPONSE._serialized_start=1180
-  _DELETEAPITOKENSRESPONSE._serialized_end=1205
-  _GETUSERREQUEST._serialized_start=1207
-  _GETUSERREQUEST._serialized_end=1248
-  _GETUSERRESPONSE._serialized_start=1251
-  _GETUSERRESPONSE._serialized_end=1420
-  _UPDATEUSERDISPLAYNAMEREQUEST._serialized_start=1422
-  _UPDATEUSERDISPLAYNAMEREQUEST._serialized_end=1494
-  _UPDATEUSERDISPLAYNAMERESPONSE._serialized_start=1496
-  _UPDATEUSERDISPLAYNAMERESPONSE._serialized_end=1582
-  _GETUSERPROJECTSREQUEST._serialized_start=1584
-  _GETUSERPROJECTSREQUEST._serialized_end=1633
-  _USERPROJECT._serialized_start=1635
-  _USERPROJECT._serialized_end=1718
-  _GETUSERPROJECTSRESPONSE._serialized_start=1720
-  _GETUSERPROJECTSRESPONSE._serialized_end=1817
-  _ACTIVATEUSERREQUEST._serialized_start=1819
-  _ACTIVATEUSERREQUEST._serialized_end=1865
-  _ACTIVATEUSERRESPONSE._serialized_start=1867
-  _ACTIVATEUSERRESPONSE._serialized_end=1889
-  _GETNOTACTIVATEDUSERSREQUEST._serialized_start=1891
-  _GETNOTACTIVATEDUSERSREQUEST._serialized_end=1920
-  _GETNOTACTIVATEDUSERSRESPONSE._serialized_start=1922
-  _GETNOTACTIVATEDUSERSRESPONSE._serialized_end=2009
-  _USERSERVICE._serialized_start=2012
-  _USERSERVICE._serialized_end=3767
+  _REGISTERUSERREQUEST._serialized_end=361
+  _REGISTERUSERRESPONSE._serialized_start=363
+  _REGISTERUSERRESPONSE._serialized_end=410
+  _CREATEAPITOKENREQUEST._serialized_start=413
+  _CREATEAPITOKENREQUEST._serialized_end=701
+  _CREATEAPITOKENRESPONSE._serialized_start=704
+  _CREATEAPITOKENRESPONSE._serialized_end=893
+  _GETAPITOKENREQUEST._serialized_start=895
+  _GETAPITOKENREQUEST._serialized_end=942
+  _GETAPITOKENRESPONSE._serialized_start=944
+  _GETAPITOKENRESPONSE._serialized_end=1023
+  _GETAPITOKENSREQUEST._serialized_start=1025
+  _GETAPITOKENSREQUEST._serialized_end=1046
+  _GETAPITOKENSRESPONSE._serialized_start=1048
+  _GETAPITOKENSRESPONSE._serialized_end=1128
+  _DELETEAPITOKENREQUEST._serialized_start=1130
+  _DELETEAPITOKENREQUEST._serialized_end=1180
+  _DELETEAPITOKENRESPONSE._serialized_start=1182
+  _DELETEAPITOKENRESPONSE._serialized_end=1206
+  _DELETEAPITOKENSREQUEST._serialized_start=1208
+  _DELETEAPITOKENSREQUEST._serialized_end=1257
+  _DELETEAPITOKENSRESPONSE._serialized_start=1259
+  _DELETEAPITOKENSRESPONSE._serialized_end=1284
+  _GETUSERREQUEST._serialized_start=1286
+  _GETUSERREQUEST._serialized_end=1327
+  _GETUSERRESPONSE._serialized_start=1330
+  _GETUSERRESPONSE._serialized_end=1499
+  _UPDATEUSERDISPLAYNAMEREQUEST._serialized_start=1501
+  _UPDATEUSERDISPLAYNAMEREQUEST._serialized_end=1573
+  _UPDATEUSERDISPLAYNAMERESPONSE._serialized_start=1575
+  _UPDATEUSERDISPLAYNAMERESPONSE._serialized_end=1661
+  _GETUSERPROJECTSREQUEST._serialized_start=1663
+  _GETUSERPROJECTSREQUEST._serialized_end=1712
+  _USERPROJECT._serialized_start=1714
+  _USERPROJECT._serialized_end=1797
+  _GETUSERPROJECTSRESPONSE._serialized_start=1799
+  _GETUSERPROJECTSRESPONSE._serialized_end=1896
+  _ACTIVATEUSERREQUEST._serialized_start=1899
+  _ACTIVATEUSERREQUEST._serialized_end=2030
+  _ACTIVATEUSERRESPONSE._serialized_start=2032
+  _ACTIVATEUSERRESPONSE._serialized_end=2054
+  _GETNOTACTIVATEDUSERSREQUEST._serialized_start=2056
+  _GETNOTACTIVATEDUSERSREQUEST._serialized_end=2085
+  _GETNOTACTIVATEDUSERSRESPONSE._serialized_start=2087
+  _GETNOTACTIVATEDUSERSRESPONSE._serialized_end=2174
+  _GETALLUSERSREQUEST._serialized_start=2176
+  _GETALLUSERSREQUEST._serialized_end=2245
+  _USERWITHPERMS._serialized_start=2248
+  _USERWITHPERMS._serialized_end=2403
+  _GETALLUSERSRESPONSE._serialized_start=2405
+  _GETALLUSERSRESPONSE._serialized_end=2512
+  _DEACTIVATEUSERREQUEST._serialized_start=2514
+  _DEACTIVATEUSERREQUEST._serialized_end=2562
+  _DEACTIVATEUSERRESPONSE._serialized_start=2564
+  _DEACTIVATEUSERRESPONSE._serialized_end=2588
+  _UPDATEUSEREMAILREQUEST._serialized_start=2590
+  _UPDATEUSEREMAILREQUEST._serialized_end=2668
+  _UPDATEUSEREMAILRESPONSE._serialized_start=2670
+  _UPDATEUSEREMAILRESPONSE._serialized_end=2750
+  _USERSERVICE._serialized_start=2753
+  _USERSERVICE._serialized_end=4977
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -5,49 +5,63 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ActivateUserRequest(_message.Message):
-    __slots__ = ["user_id"]
+    __slots__ = ["project_perms", "user_id"]
+    PROJECT_PERMS_FIELD_NUMBER: _ClassVar[int]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
+    project_perms: _auth_pb2.ProjectPermission
     user_id: str
-    def __init__(self, user_id: _Optional[str] = ...) -> None: ...
+    def __init__(self, user_id: _Optional[str] = ..., project_perms: _Optional[_Union[_auth_pb2.ProjectPermission, _Mapping]] = ...) -> None: ...
 
 class ActivateUserResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class CreateAPITokenRequest(_message.Message):
-    __slots__ = ["collection_id", "expires_at", "name", "permission", "project_id"]
+    __slots__ = ["collection_id", "expires_at", "is_session", "name", "permission", "project_id"]
     COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_AT_FIELD_NUMBER: _ClassVar[int]
+    IS_SESSION_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     PERMISSION_FIELD_NUMBER: _ClassVar[int]
     PROJECT_ID_FIELD_NUMBER: _ClassVar[int]
     collection_id: str
     expires_at: ExpiresAt
+    is_session: bool
     name: str
     permission: _auth_pb2.Permission
     project_id: str
-    def __init__(self, project_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., name: _Optional[str] = ..., expires_at: _Optional[_Union[ExpiresAt, _Mapping]] = ..., permission: _Optional[_Union[_auth_pb2.Permission, str]] = ...) -> None: ...
+    def __init__(self, project_id: _Optional[str] = ..., collection_id: _Optional[str] = ..., name: _Optional[str] = ..., expires_at: _Optional[_Union[ExpiresAt, _Mapping]] = ..., permission: _Optional[_Union[_auth_pb2.Permission, str]] = ..., is_session: bool = ...) -> None: ...
 
 class CreateAPITokenResponse(_message.Message):
     __slots__ = ["s3_access_key", "s3_secret_key", "token", "token_secret"]
     S3_ACCESS_KEY_FIELD_NUMBER: _ClassVar[int]
     S3_SECRET_KEY_FIELD_NUMBER: _ClassVar[int]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     TOKEN_SECRET_FIELD_NUMBER: _ClassVar[int]
     s3_access_key: str
     s3_secret_key: str
     token: _auth_pb2.Token
     token_secret: str
     def __init__(self, token: _Optional[_Union[_auth_pb2.Token, _Mapping]] = ..., token_secret: _Optional[str] = ..., s3_access_key: _Optional[str] = ..., s3_secret_key: _Optional[str] = ...) -> None: ...
 
+class DeactivateUserRequest(_message.Message):
+    __slots__ = ["user_id"]
+    USER_ID_FIELD_NUMBER: _ClassVar[int]
+    user_id: str
+    def __init__(self, user_id: _Optional[str] = ...) -> None: ...
+
+class DeactivateUserResponse(_message.Message):
+    __slots__ = []
+    def __init__(self) -> None: ...
+
 class DeleteAPITokenRequest(_message.Message):
     __slots__ = ["token_id"]
     TOKEN_ID_FIELD_NUMBER: _ClassVar[int]
     token_id: str
     def __init__(self, token_id: _Optional[str] = ...) -> None: ...
 
 class DeleteAPITokenResponse(_message.Message):
@@ -88,14 +102,26 @@
 
 class GetAPITokensResponse(_message.Message):
     __slots__ = ["token"]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     token: _containers.RepeatedCompositeFieldContainer[_auth_pb2.Token]
     def __init__(self, token: _Optional[_Iterable[_Union[_auth_pb2.Token, _Mapping]]] = ...) -> None: ...
 
+class GetAllUsersRequest(_message.Message):
+    __slots__ = ["include_permissions"]
+    INCLUDE_PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
+    include_permissions: bool
+    def __init__(self, include_permissions: bool = ...) -> None: ...
+
+class GetAllUsersResponse(_message.Message):
+    __slots__ = ["user_with_perms"]
+    USER_WITH_PERMS_FIELD_NUMBER: _ClassVar[int]
+    user_with_perms: _containers.RepeatedCompositeFieldContainer[UserWithPerms]
+    def __init__(self, user_with_perms: _Optional[_Iterable[_Union[UserWithPerms, _Mapping]]] = ...) -> None: ...
+
 class GetNotActivatedUsersRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class GetNotActivatedUsersResponse(_message.Message):
     __slots__ = ["users"]
     USERS_FIELD_NUMBER: _ClassVar[int]
@@ -125,18 +151,22 @@
     PROJECT_PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
     USER_FIELD_NUMBER: _ClassVar[int]
     project_permissions: _containers.RepeatedCompositeFieldContainer[_auth_pb2.ProjectPermission]
     user: _auth_pb2.User
     def __init__(self, user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ..., project_permissions: _Optional[_Iterable[_Union[_auth_pb2.ProjectPermission, _Mapping]]] = ...) -> None: ...
 
 class RegisterUserRequest(_message.Message):
-    __slots__ = ["display_name"]
+    __slots__ = ["display_name", "email", "project"]
     DISPLAY_NAME_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
+    PROJECT_FIELD_NUMBER: _ClassVar[int]
     display_name: str
-    def __init__(self, display_name: _Optional[str] = ...) -> None: ...
+    email: str
+    project: str
+    def __init__(self, display_name: _Optional[str] = ..., email: _Optional[str] = ..., project: _Optional[str] = ...) -> None: ...
 
 class RegisterUserResponse(_message.Message):
     __slots__ = ["user_id"]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
     user_id: str
     def __init__(self, user_id: _Optional[str] = ...) -> None: ...
 
@@ -148,16 +178,38 @@
 
 class UpdateUserDisplayNameResponse(_message.Message):
     __slots__ = ["user"]
     USER_FIELD_NUMBER: _ClassVar[int]
     user: _auth_pb2.User
     def __init__(self, user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ...) -> None: ...
 
+class UpdateUserEmailRequest(_message.Message):
+    __slots__ = ["new_email", "user_id"]
+    NEW_EMAIL_FIELD_NUMBER: _ClassVar[int]
+    USER_ID_FIELD_NUMBER: _ClassVar[int]
+    new_email: str
+    user_id: str
+    def __init__(self, user_id: _Optional[str] = ..., new_email: _Optional[str] = ...) -> None: ...
+
+class UpdateUserEmailResponse(_message.Message):
+    __slots__ = ["user"]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    user: _auth_pb2.User
+    def __init__(self, user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ...) -> None: ...
+
 class UserProject(_message.Message):
     __slots__ = ["description", "id", "name"]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     description: str
     id: str
     name: str
     def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+
+class UserWithPerms(_message.Message):
+    __slots__ = ["project_perms", "user"]
+    PROJECT_PERMS_FIELD_NUMBER: _ClassVar[int]
+    USER_FIELD_NUMBER: _ClassVar[int]
+    project_perms: _containers.RepeatedCompositeFieldContainer[_auth_pb2.ProjectPermission]
+    user: _auth_pb2.User
+    def __init__(self, user: _Optional[_Union[_auth_pb2.User, _Mapping]] = ..., project_perms: _Optional[_Iterable[_Union[_auth_pb2.ProjectPermission, _Mapping]]] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.0.0rc9/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc1/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,19 @@
             channel: A grpc.Channel.
         """
         self.RegisterUser = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/RegisterUser',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserResponse.FromString,
                 )
+        self.DeactivateUser = channel.unary_unary(
+                '/aruna.api.storage.services.v1.UserService/DeactivateUser',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserResponse.FromString,
+                )
         self.ActivateUser = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/ActivateUser',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.ActivateUserRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.ActivateUserResponse.FromString,
                 )
         self.CreateAPIToken = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/CreateAPIToken',
@@ -59,24 +64,34 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserResponse.FromString,
                 )
         self.UpdateUserDisplayName = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/UpdateUserDisplayName',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameResponse.FromString,
                 )
+        self.UpdateUserEmail = channel.unary_unary(
+                '/aruna.api.storage.services.v1.UserService/UpdateUserEmail',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailResponse.FromString,
+                )
         self.GetUserProjects = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/GetUserProjects',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserProjectsRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserProjectsResponse.FromString,
                 )
         self.GetNotActivatedUsers = channel.unary_unary(
                 '/aruna.api.storage.services.v1.UserService/GetNotActivatedUsers',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersResponse.FromString,
                 )
+        self.GetAllUsers = channel.unary_unary(
+                '/aruna.api.storage.services.v1.UserService/GetAllUsers',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersResponse.FromString,
+                )
 
 
 class UserServiceServicer(object):
     """UserService
 
     Contains all methods that get/create or update Users and associated resource
     including all autorization methods
@@ -89,14 +104,25 @@
 
         This request should be called when a new user logs in for the first time
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DeactivateUser(self, request, context):
+        """DeActivateUser 
+
+        Status: ALPHA
+
+        This deactivates a specific user (Admin request)
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ActivateUser(self, request, context):
         """ActivateUser 
 
         Status: STABLE
 
         This activates a specific user (Admin request)
         """
@@ -178,14 +204,25 @@
 
         Updates the Displayname for the user (Personal only)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UpdateUserEmail(self, request, context):
+        """UpdateUserDisplayName
+
+        Status: ALPHA
+
+        Updates the email for the user (Personal only)
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetUserProjects(self, request, context):
         """GetUserProjects
 
         Status: STABLE
 
         Gets all project_ids a user is member of
         """
@@ -200,22 +237,38 @@
 
         Get all not activated users (Admin only)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetAllUsers(self, request, context):
+        """GetAllUsers
+
+        Status: ALPHA
+
+        Get all users inkluding permissions (Admin only)
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_UserServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'RegisterUser': grpc.unary_unary_rpc_method_handler(
                     servicer.RegisterUser,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserResponse.SerializeToString,
             ),
+            'DeactivateUser': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeactivateUser,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserResponse.SerializeToString,
+            ),
             'ActivateUser': grpc.unary_unary_rpc_method_handler(
                     servicer.ActivateUser,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.ActivateUserRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.ActivateUserResponse.SerializeToString,
             ),
             'CreateAPIToken': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateAPIToken,
@@ -248,24 +301,34 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserResponse.SerializeToString,
             ),
             'UpdateUserDisplayName': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdateUserDisplayName,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameResponse.SerializeToString,
             ),
+            'UpdateUserEmail': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateUserEmail,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailResponse.SerializeToString,
+            ),
             'GetUserProjects': grpc.unary_unary_rpc_method_handler(
                     servicer.GetUserProjects,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserProjectsRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetUserProjectsResponse.SerializeToString,
             ),
             'GetNotActivatedUsers': grpc.unary_unary_rpc_method_handler(
                     servicer.GetNotActivatedUsers,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersResponse.SerializeToString,
             ),
+            'GetAllUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetAllUsers,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.storage.services.v1.UserService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -290,14 +353,31 @@
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/RegisterUser',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.RegisterUserResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def DeactivateUser(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/DeactivateUser',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.DeactivateUserResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ActivateUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -426,14 +506,31 @@
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/UpdateUserDisplayName',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserDisplayNameResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def UpdateUserEmail(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/UpdateUserEmail',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.UpdateUserEmailResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetUserProjects(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -458,7 +555,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/GetNotActivatedUsers',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetNotActivatedUsersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetAllUsers(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.UserService/GetAllUsers',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_user__service__pb2.GetAllUsersResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `Aruna-Python-API-1.0.0rc9/setup.py` & `Aruna-Python-API-1.1.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.0.0-rc.9",
+    version="1.1.0-rc.1",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

