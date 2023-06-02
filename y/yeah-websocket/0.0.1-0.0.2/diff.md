# Comparing `tmp/yeah_websocket-0.0.1.tar.gz` & `tmp/yeah_websocket-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeah_websocket-0.0.1.tar", last modified: Thu Jun  1 23:56:28 2023, max compression
+gzip compressed data, was "yeah_websocket-0.0.2.tar", last modified: Fri Jun  2 00:03:01 2023, max compression
```

## Comparing `yeah_websocket-0.0.1.tar` & `yeah_websocket-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 23:56:28.423497 yeah_websocket-0.0.1/
--rw-rw-rw-   0        0        0      166 2023-06-01 23:56:28.422177 yeah_websocket-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-01 23:56:28.423497 yeah_websocket-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      300 2023-06-01 23:55:41.000000 yeah_websocket-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 23:56:28.410714 yeah_websocket-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 23:56:28.421085 yeah_websocket-0.0.1/src/yeah_websocket.egg-info/
--rw-rw-rw-   0        0        0      166 2023-06-01 23:56:28.000000 yeah_websocket-0.0.1/src/yeah_websocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2023-06-01 23:56:28.000000 yeah_websocket-0.0.1/src/yeah_websocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 23:56:28.000000 yeah_websocket-0.0.1/src/yeah_websocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 23:56:28.000000 yeah_websocket-0.0.1/src/yeah_websocket.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 00:03:01.820515 yeah_websocket-0.0.2/
+-rw-rw-rw-   0        0        0      166 2023-06-02 00:03:01.819508 yeah_websocket-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-02 00:03:01.820515 yeah_websocket-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      300 2023-06-02 00:02:43.000000 yeah_websocket-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-02 00:03:01.802783 yeah_websocket-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-02 00:03:01.814979 yeah_websocket-0.0.2/src/yeah_websocket.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-06-02 00:03:01.000000 yeah_websocket-0.0.2/src/yeah_websocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-06-02 00:03:01.000000 yeah_websocket-0.0.2/src/yeah_websocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 00:03:01.000000 yeah_websocket-0.0.2/src/yeah_websocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-02 00:03:01.000000 yeah_websocket-0.0.2/src/yeah_websocket.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 00:03:01.818507 yeah_websocket-0.0.2/src/yeah_websocket_elay_py/
+-rw-rw-rw-   0        0        0        0 2023-06-01 23:50:52.000000 yeah_websocket-0.0.2/src/yeah_websocket_elay_py/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-06-01 23:34:21.000000 yeah_websocket-0.0.2/src/yeah_websocket_elay_py/client.py
+-rw-rw-rw-   0        0        0      221 2023-06-01 23:34:21.000000 yeah_websocket-0.0.2/src/yeah_websocket_elay_py/server.py
```

