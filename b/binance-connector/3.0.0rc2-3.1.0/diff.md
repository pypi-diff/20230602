# Comparing `tmp/binance-connector-3.0.0rc2.tar.gz` & `tmp/binance-connector-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-connector-3.0.0rc2.tar", last modified: Fri Apr 21 06:58:31 2023, max compression
+gzip compressed data, was "binance-connector-3.1.0.tar", last modified: Fri Jun  2 07:47:13 2023, max compression
```

## Comparing `binance-connector-3.0.0rc2.tar` & `binance-connector-3.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.581536 binance-connector-3.0.0rc2/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.581536 binance-connector-3.0.0rc2/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/spot/
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_blvt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_bswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_c2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_fiat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_futures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_gift_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_loan.py
--rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_mining.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_pay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_rebate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_savings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_staking.py
--rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_sub_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/spot/_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.585536 binance-connector-3.0.0rc2/binance/websocket/spot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_market.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/spot/websocket_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/binance_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-21 06:58:31.000000 binance-connector-3.0.0rc2/binance_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-21 06:58:31.589536 binance-connector-3.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-21 06:58:21.000000 binance-connector-3.0.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-02 07:47:10.000000 binance-connector-3.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 07:47:10.000000 binance-connector-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-06-02 07:47:13.809712 binance-connector-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-06-02 07:47:10.000000 binance-connector-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.805711 binance-connector-3.1.0/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.805711 binance-connector-3.1.0/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/lib/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/binance/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_blvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_bswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_c2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_fiat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_gift_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_loan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33152 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_mining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_pay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_rebate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_savings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_staking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_sub_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/spot/_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/binance/websocket/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/binance/websocket/spot/websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_api/_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24597 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_api/_market.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_api/_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_api/_user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/spot/websocket_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-02 07:47:10.000000 binance-connector-3.1.0/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/binance_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-06-02 07:47:13.000000 binance-connector-3.1.0/binance_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-02 07:47:13.000000 binance-connector-3.1.0/binance_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:47:13.000000 binance-connector-3.1.0/binance_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-02 07:47:13.000000 binance-connector-3.1.0/binance_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 07:47:13.000000 binance-connector-3.1.0/binance_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:10.000000 binance-connector-3.1.0/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.809712 binance-connector-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-02 07:47:10.000000 binance-connector-3.1.0/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-02 07:47:13.809712 binance-connector-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-02 07:47:10.000000 binance-connector-3.1.0/setup.py
```

### Comparing `binance-connector-3.0.0rc2/LICENSE.md` & `binance-connector-3.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/PKG-INFO` & `binance-connector-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.0.0rc2
+Version: 3.1.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Binance Public API Connector Python
 [![PyPI version](https://img.shields.io/pypi/v/binance-connector)](https://pypi.python.org/pypi/binance-connector)
 [![Python version](https://img.shields.io/pypi/pyversions/binance-connector)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://binance-connector.readthedocs.io/en/stable/)
@@ -88,32 +87,42 @@
     [keys]
     api_key=abc123456
     api_secret=cba654321
     ```
 
 ### Authentication
 
-Binance supports HMAC and RSA API authentication.
+Binance supports HMAC, RSA and ED25519 API authentication.
 
 ```python
 
 # HMAC: pass API key and secret
 client = Client(api_key, api_secret)
 print(client.account())
 
 # RSA Keys
 client = Client(api_key=api_key, private_key=private_key)
 print(client.account())
 
+# ED25519 Keys
+api_key = ""
+private_key = "./private_key.pem"
+private_key_pass = "<password_if_applicable>"
+
+with open(private_key, 'rb') as f:
+    private_key = f.read()
+
+spot_client = Client(api_key=api_key, private_key=private_key, private_key_pass=private_key_pass)
+
 # Encrypted RSA Key
 client = Client(api_key=api_key, private_key=private_key, private_key_pass='password')
 print(client.account())
 ```
-
-Please find `examples/spot/trade/get_account.py` for more details.
+Please find `examples/spot/wallet/account_snapshot.py` for more details on ED25519.
+Please find `examples/spot/trade/get_account.py` for more details on RSA.
 
 ### Testnet
 
 [Spot Testnet](https://testnet.binance.vision/) is available, it can be used to test `/api/*` endpoints.
 
 - `/sapi/*` endpoints are not available.
 - No UI.
@@ -287,19 +296,22 @@
 # id provided by client
 my_client.ping_connectivity(id="my_request_id")
 
 # library will generate a random uuid string
 my_client.ping_connectivity()
 ```
 
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder.
 
 Example file "examples/websocket_api/app_demo.py" demonstrates how Websocket API and Websocket Stream can be used together.
 
-
 ### Connector v1 and v2
 
 ```python
 from binance.websocket.spot.websocket_client import SpotWebsocketClient as WebsocketClient
 
 def message_handler(message):
     print(message)
```

### Comparing `binance-connector-3.0.0rc2/README.md` & `binance-connector-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -69,32 +69,42 @@
     [keys]
     api_key=abc123456
     api_secret=cba654321
     ```
 
 ### Authentication
 
-Binance supports HMAC and RSA API authentication.
+Binance supports HMAC, RSA and ED25519 API authentication.
 
 ```python
 
 # HMAC: pass API key and secret
 client = Client(api_key, api_secret)
 print(client.account())
 
 # RSA Keys
 client = Client(api_key=api_key, private_key=private_key)
 print(client.account())
 
+# ED25519 Keys
+api_key = ""
+private_key = "./private_key.pem"
+private_key_pass = "<password_if_applicable>"
+
+with open(private_key, 'rb') as f:
+    private_key = f.read()
+
+spot_client = Client(api_key=api_key, private_key=private_key, private_key_pass=private_key_pass)
+
 # Encrypted RSA Key
 client = Client(api_key=api_key, private_key=private_key, private_key_pass='password')
 print(client.account())
 ```
-
-Please find `examples/spot/trade/get_account.py` for more details.
+Please find `examples/spot/wallet/account_snapshot.py` for more details on ED25519.
+Please find `examples/spot/trade/get_account.py` for more details on RSA.
 
 ### Testnet
 
 [Spot Testnet](https://testnet.binance.vision/) is available, it can be used to test `/api/*` endpoints.
 
 - `/sapi/*` endpoints are not available.
 - No UI.
@@ -268,19 +278,22 @@
 # id provided by client
 my_client.ping_connectivity(id="my_request_id")
 
 # library will generate a random uuid string
 my_client.ping_connectivity()
 ```
 
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder.
 
 Example file "examples/websocket_api/app_demo.py" demonstrates how Websocket API and Websocket Stream can be used together.
 
-
 ### Connector v1 and v2
 
 ```python
 from binance.websocket.spot.websocket_client import SpotWebsocketClient as WebsocketClient
 
 def message_handler(message):
     print(message)
```

### Comparing `binance-connector-3.0.0rc2/binance/api.py` & `binance-connector-3.1.0/binance/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 from .__version__ import __version__
 from binance.error import ClientError, ServerError
 from binance.lib.utils import get_timestamp
 from binance.lib.utils import cleanNoneValue
 from binance.lib.utils import encoded_string
 from binance.lib.utils import check_required_parameter
-from binance.lib.authentication import hmac_hashing, rsa_signature
+from binance.lib.authentication import hmac_hashing, rsa_signature, ed25519_signature
 
 
 class API(object):
     """API base class
 
     Keyword Args:
         base_url (str, optional): the API base url, useful to switch to testnet, etc. By default it's https://api.binance.com
@@ -145,17 +145,23 @@
 
         return data
 
     def _prepare_params(self, params):
         return encoded_string(cleanNoneValue(params))
 
     def _get_sign(self, payload):
-        if self.private_key:
-            return rsa_signature(self.private_key, payload, self.private_key_pass)
-        return hmac_hashing(self.api_secret, payload)
+        if self.private_key is not None:
+            try:
+                return ed25519_signature(
+                    self.private_key, payload, self.private_key_pass
+                )
+            except ValueError:
+                return rsa_signature(self.private_key, payload, self.private_key_pass)
+        else:
+            return hmac_hashing(self.api_secret, payload)
 
     def _dispatch_request(self, http_method):
         return {
             "GET": self.session.get,
             "DELETE": self.session.delete,
             "PUT": self.session.put,
             "POST": self.session.post,
```

### Comparing `binance-connector-3.0.0rc2/binance/error.py` & `binance-connector-3.1.0/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/lib/enums.py` & `binance-connector-3.1.0/binance/lib/enums.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/lib/utils.py` & `binance-connector-3.1.0/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/__init__.py` & `binance-connector-3.1.0/binance/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_blvt.py` & `binance-connector-3.1.0/binance/spot/_blvt.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_bswap.py` & `binance-connector-3.1.0/binance/spot/_bswap.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_c2c.py` & `binance-connector-3.1.0/binance/spot/_c2c.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_convert.py` & `binance-connector-3.1.0/binance/spot/_convert.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_data_stream.py` & `binance-connector-3.1.0/binance/spot/_data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_fiat.py` & `binance-connector-3.1.0/binance/spot/_fiat.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_futures.py` & `binance-connector-3.1.0/binance/spot/_futures.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_gift_card.py` & `binance-connector-3.1.0/binance/spot/_gift_card.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_loan.py` & `binance-connector-3.1.0/binance/spot/_loan.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_margin.py` & `binance-connector-3.1.0/binance/spot/_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_market.py` & `binance-connector-3.1.0/binance/spot/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_mining.py` & `binance-connector-3.1.0/binance/spot/_mining.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_nft.py` & `binance-connector-3.1.0/binance/spot/_nft.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_portfolio_margin.py` & `binance-connector-3.1.0/binance/spot/_portfolio_margin.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_savings.py` & `binance-connector-3.1.0/binance/spot/_savings.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_staking.py` & `binance-connector-3.1.0/binance/spot/_staking.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_sub_account.py` & `binance-connector-3.1.0/binance/spot/_sub_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_trade.py` & `binance-connector-3.1.0/binance/spot/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/spot/_wallet.py` & `binance-connector-3.1.0/binance/spot/_wallet.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/binance_socket_manager.py` & `binance-connector-3.1.0/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/__init__.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_api/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_account.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_api/_account.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_market.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_api/_market.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_trade.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_api/_trade.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_api/_user_data.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_api/_user_data.py`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/binance/websocket/spot/websocket_stream.py` & `binance-connector-3.1.0/binance/websocket/spot/websocket_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from binance.websocket.websocket_client import BinanceWebsocketClient
 
 
 class SpotWebsocketStreamClient(BinanceWebsocketClient):
-    ACTION_SUBSCRIBE = "SUBSCRIBE"
-    ACTION_UNSUBSCRIBE = "UNSUBSCRIBE"
-
     def __init__(
         self,
         stream_url="wss://stream.binance.com:9443",
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
```

### Comparing `binance-connector-3.0.0rc2/binance/websocket/websocket_client.py` & `binance-connector-3.1.0/binance/websocket/websocket_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import logging
 from binance.lib.utils import get_timestamp
 from binance.websocket.binance_socket_manager import BinanceSocketManager
 
 
 class BinanceWebsocketClient:
+    ACTION_SUBSCRIBE = "SUBSCRIBE"
+    ACTION_UNSUBSCRIBE = "UNSUBSCRIBE"
+
     def __init__(
         self,
         stream_url,
         on_message=None,
         on_open=None,
         on_close=None,
         on_error=None,
@@ -52,14 +55,22 @@
             on_close=on_close,
             on_error=on_error,
             on_ping=on_ping,
             on_pong=on_pong,
             logger=logger,
         )
 
+    def _single_stream(self, stream):
+        if isinstance(stream, str):
+            return True
+        elif isinstance(stream, list):
+            return False
+        else:
+            raise ValueError("Invalid stream name, expect string or array")
+
     def send(self, message: dict):
         self.socket_manager.send_message(json.dumps(message))
 
     def send_message_to_server(self, message, action=None, id=None):
         if not id:
             id = get_timestamp()
 
@@ -71,25 +82,21 @@
         if not id:
             id = get_timestamp()
         if self._single_stream(stream):
             stream = [stream]
         json_msg = json.dumps({"method": "SUBSCRIBE", "params": stream, "id": id})
         self.socket_manager.send_message(json_msg)
 
-    def unsubscribe(self, stream: str, id=None):
+    def unsubscribe(self, stream, id=None):
         if not id:
             id = get_timestamp()
-
-        if not self._single_stream(stream):
-            raise ValueError("Invalid stream name, expect a string")
-
-        stream = [stream]
-        self.socket_manager.send_message(
-            json.dumps({"method": "UNSUBSCRIBE", "params": stream, "id": id})
-        )
+        if self._single_stream(stream):
+            stream = [stream]
+        json_msg = json.dumps({"method": "UNSUBSCRIBE", "params": stream, "id": id})
+        self.socket_manager.send_message(json_msg)
 
     def ping(self):
         self.logger.debug("Sending ping to Binance WebSocket Server")
         self.socket_manager.ping()
 
     def stop(self, id=None):
         self.socket_manager.close()
@@ -103,15 +110,7 @@
         """
 
         if not id:
             id = get_timestamp()
         self.socket_manager.send_message(
             json.dumps({"method": "LIST_SUBSCRIPTIONS", "id": id})
         )
-
-    def _single_stream(self, stream):
-        if isinstance(stream, str):
-            return True
-        elif isinstance(stream, list):
-            return False
-        else:
-            raise ValueError("Invalid stream name, expect string or array")
```

### Comparing `binance-connector-3.0.0rc2/binance_connector.egg-info/PKG-INFO` & `binance-connector-3.1.0/binance_connector.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: binance-connector
-Version: 3.0.0rc2
+Version: 3.1.0
 Summary: This is a lightweight library that works as a connector to Binance public API.
 Home-page: https://github.com/binance/binance-connector-python
 License: MIT
 Keywords: Binance,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Binance Public API Connector Python
 [![PyPI version](https://img.shields.io/pypi/v/binance-connector)](https://pypi.python.org/pypi/binance-connector)
 [![Python version](https://img.shields.io/pypi/pyversions/binance-connector)](https://www.python.org/downloads/)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue)](https://binance-connector.readthedocs.io/en/stable/)
@@ -88,32 +87,42 @@
     [keys]
     api_key=abc123456
     api_secret=cba654321
     ```
 
 ### Authentication
 
-Binance supports HMAC and RSA API authentication.
+Binance supports HMAC, RSA and ED25519 API authentication.
 
 ```python
 
 # HMAC: pass API key and secret
 client = Client(api_key, api_secret)
 print(client.account())
 
 # RSA Keys
 client = Client(api_key=api_key, private_key=private_key)
 print(client.account())
 
+# ED25519 Keys
+api_key = ""
+private_key = "./private_key.pem"
+private_key_pass = "<password_if_applicable>"
+
+with open(private_key, 'rb') as f:
+    private_key = f.read()
+
+spot_client = Client(api_key=api_key, private_key=private_key, private_key_pass=private_key_pass)
+
 # Encrypted RSA Key
 client = Client(api_key=api_key, private_key=private_key, private_key_pass='password')
 print(client.account())
 ```
-
-Please find `examples/spot/trade/get_account.py` for more details.
+Please find `examples/spot/wallet/account_snapshot.py` for more details on ED25519.
+Please find `examples/spot/trade/get_account.py` for more details on RSA.
 
 ### Testnet
 
 [Spot Testnet](https://testnet.binance.vision/) is available, it can be used to test `/api/*` endpoints.
 
 - `/sapi/*` endpoints are not available.
 - No UI.
@@ -287,19 +296,22 @@
 # id provided by client
 my_client.ping_connectivity(id="my_request_id")
 
 # library will generate a random uuid string
 my_client.ping_connectivity()
 ```
 
+#### Combined Streams
+- If you set `is_combined` to `True`, `"/stream/"` will be appended to the `baseURL` to allow for Combining streams.
+- `is_combined` defaults to `False` and `"/ws/"` (raw streams) will be appended to the `baseURL`.
+
 More websocket examples are available in the `examples` folder.
 
 Example file "examples/websocket_api/app_demo.py" demonstrates how Websocket API and Websocket Stream can be used together.
 
-
 ### Connector v1 and v2
 
 ```python
 from binance.websocket.spot.websocket_client import SpotWebsocketClient as WebsocketClient
 
 def message_handler(message):
     print(message)
```

### Comparing `binance-connector-3.0.0rc2/binance_connector.egg-info/SOURCES.txt` & `binance-connector-3.1.0/binance_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-connector-3.0.0rc2/setup.py` & `binance-connector-3.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     keywords=["Binance", "Public API"],
     install_requires=[req for req in requirements],
     packages=find_packages(exclude=("tests",)),
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

