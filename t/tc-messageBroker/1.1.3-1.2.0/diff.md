# Comparing `tmp/tc-messageBroker-1.1.3.tar.gz` & `tmp/tc-messageBroker-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.1.3.tar", last modified: Thu Jun  1 07:46:04 2023, max compression
+gzip compressed data, was "tc-messageBroker-1.2.0.tar", last modified: Fri Jun  2 17:42:29 2023, max compression
```

## Comparing `tc-messageBroker-1.1.3.tar` & `tc-messageBroker-1.2.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (123)     9246 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.823849 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 07:46:04.000000 tc-messageBroker-1.1.3/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:46:04.827849 tc-messageBroker-1.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-01 07:45:45.000000 tc-messageBroker-1.1.3/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 17:42:29.000000 tc-messageBroker-1.2.0/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.263498 tc-messageBroker-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:29.267498 tc-messageBroker-1.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-02 17:42:09.000000 tc-messageBroker-1.2.0/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.1.3/PKG-INFO` & `tc-messageBroker-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.3
+Version: 1.2.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.3/README.md` & `tc-messageBroker-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/setup.py` & `tc-messageBroker-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.1.3",
+    version="1.2.0",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/message_broker.py` & `tc-messageBroker-1.2.0/tc_messageBroker/message_broker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pika
 
 # from typing import Callable
 import logging
 from datetime import datetime
 import json
+import functools
 
 
 class RabbitMQ:
     def __init__(self, broker_url: str, port: int, username: str, password: str):
         logging.basicConfig()
         logging.getLogger().setLevel(logging.INFO)
 
@@ -24,38 +25,49 @@
 
     def __new__(cls, broker_url: str, port: int, username: str, password: str):
         ## making it singleton
         if not hasattr(cls, "instance"):
             cls.instance = super(RabbitMQ, cls).__new__(cls)
         return cls.instance
 
-    def connect(self, queue_name: str, consume_options: dict = None) -> bool:
+    def connect(
+            self, 
+            queue_name: str, 
+            consume_options: dict = None,
+            heartbeat: int = 60
+        ) -> bool:
         """
         connect the rabbitMQ broker and start consuming
 
         Parameters:
         -------------
         queue_name : str
             the queue name to connect
         consume_options : dict
             additional arguments for basic_consume method
             default is `None`
+        heartbeat : int
+            the number of seconds for a message to stay alive
+            default is 60 seconds
 
         Returns:
         ---------
         is_successful : bool
             if True, connecting to rabbitMQ server was successful
             otherwise would return False
         """
         try:
             credentials = pika.PlainCredentials(self._username, self._password)
             amqpServer = self.broker_url
             self.connection = pika.BlockingConnection(
                 pika.ConnectionParameters(
-                    host=amqpServer, port=self.port, credentials=credentials
+                    host=amqpServer,
+                    port=self.port,
+                    credentials=credentials,
+                    heartbeat=heartbeat, ## disabling the heartbeat
                 ),
             )
             self.channel = self.connection.channel()
 
             # make sure that the channel is created,
             # if not this statement will create it
             self.channel.queue_declare(queue=queue_name)
@@ -89,29 +101,41 @@
             otherwise would return False and requeue the message
         """
         body_serialized = json.loads(body)
         event = body_serialized["event"]
 
         if event not in self.event_function.keys():
             logging.info(" An Event was received that doesn't exist")
-            self.channel.basic_reject(delivery_tag=method.delivery_tag, requeue=True)
+            self.connection.add_callback_threadsafe(
+                functools.partial(
+                    self.channel.basic_reject,
+                    delivery_tag=method.delivery_tag,
+                    requeue=True,
+                )
+            )
         else:
             self.event_function[event](body_serialized)
-            self.channel.basic_ack(delivery_tag=method.delivery_tag)
+            self.connection.add_callback_threadsafe(
+                functools.partial(
+                    self.channel.basic_ack,
+                    delivery_tag=method.delivery_tag,
+                )
+            )
 
     def consume(self, queue_name: str, consume_options: dict = None):
         """
         set consuming events from a queue
         """
         self.channel.queue_declare(queue=queue_name)
 
         self.channel.basic_consume(
             queue=queue_name,
             on_message_callback=self._consume_callback,
             arguments=consume_options,
+            auto_ack=False,
         )
 
     def publish(
         self, queue_name: str, event: str, content: dict, options: any = None
     ) -> None:
         """
         Publish a specific message to a specific queue directly
```

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             self._update_save(
                 transactions=tx_sorted,
                 mongo_creds=mongo_creds,
                 test=test_mode,
             )
 
         except Exception as exp:
+            logging.info(f"Error occured during the next function. Exception: {exp}")
             current_tx.error = str(exp)
 
             if current_tx.status != Status.SUCCESS:
                 current_tx.status = Status.FAILED
 
             self.status = Status.FAILED
```

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,37 +9,37 @@
             "properties": {
                 "name": {
                     "type": "string",
                 },
                 "transactions": {
                     "type": "array",
                     "items": {
-                            "type": "object",
-                            "properties": {
-                                "queue": {"type": "string"},
-                                "event": {"type": "string"},
-                                "order": {"type": ["integer", "string"]},
-                                "status": {
-                                    "type": "string",
-                                    "enum": [
-                                        Status.NOT_STARTED,
-                                        Status.IN_PROGRESS,
-                                        Status.SUCCESS,
-                                        Status.FAILED,
-                                        Status.CANCELLED,
-                                    ],
-                                },
-                                "message": {"type": "string"},
-                                "start": {},
-                                "end": {},
-                                "runtime": {"type": "number"},
-                                "error": {"type": "string"},
+                        "type": "object",
+                        "properties": {
+                            "queue": {"type": "string"},
+                            "event": {"type": "string"},
+                            "order": {"type": ["integer", "string"]},
+                            "status": {
+                                "type": "string",
+                                "enum": [
+                                    Status.NOT_STARTED,
+                                    Status.IN_PROGRESS,
+                                    Status.SUCCESS,
+                                    Status.FAILED,
+                                    Status.CANCELLED,
+                                ],
                             },
-                            "required": ["queue", "event", "order", "status"],
-                            "additionalProperties": False,
+                            "message": {"type": "string"},
+                            "start": {},
+                            "end": {},
+                            "runtime": {"type": "number"},
+                            "error": {"type": "string"},
+                        },
+                        "required": ["queue", "event", "order", "status"],
+                        "additionalProperties": False,
                     },
                     "additionalProperties": False,
                 },
             },
             "required": ["name", "transactions"],
             "additionalProperties": False,
         },
```

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc-messageBroker-1.2.0/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker.egg-info/PKG-INFO` & `tc-messageBroker-1.2.0/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.1.3
+Version: 1.2.0
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 
 # tc-messageBrokerPython
```

### Comparing `tc-messageBroker-1.1.3/tc_messageBroker.egg-info/SOURCES.txt` & `tc-messageBroker-1.2.0/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/integration/test_message_broker_exchange_points.py` & `tc-messageBroker-1.2.0/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/integration/test_mongodb.py` & `tc-messageBroker-1.2.0/tests/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/integration/test_saga.py` & `tc-messageBroker-1.2.0/tests/integration/test_saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_choreagraphy_base.py` & `tc-messageBroker-1.2.0/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_message_broker.py` & `tc-messageBroker-1.2.0/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_predefined_transactions.py` & `tc-messageBroker-1.2.0/tests/unit/test_predefined_transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_saga_base.py` & `tc-messageBroker-1.2.0/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_saga_base_utils.py` & `tc-messageBroker-1.2.0/tests/unit/test_saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_saga_next.py` & `tc-messageBroker-1.2.0/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_saga_start.py` & `tc-messageBroker-1.2.0/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.1.3/tests/unit/test_transactions.py` & `tc-messageBroker-1.2.0/tests/unit/test_transactions.py`

 * *Files identical despite different names*

