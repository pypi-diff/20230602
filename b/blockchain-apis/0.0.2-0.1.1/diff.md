# Comparing `tmp/blockchain-apis-0.0.2.tar.gz` & `tmp/blockchain-apis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockchain-apis-0.0.2.tar", last modified: Tue May 30 21:20:17 2023, max compression
+gzip compressed data, was "blockchain-apis-0.1.1.tar", last modified: Fri Jun  2 15:26:58 2023, max compression
```

## Comparing `blockchain-apis-0.0.2.tar` & `blockchain-apis-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.0.2/LICENSE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4725 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3173 2023-05-30 21:17:27.000000 blockchain-apis-0.0.2/README.md
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.782270 blockchain-apis-0.0.2/blockchain_apis/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24803 2023-05-30 21:18:49.000000 blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24232 2023-05-30 21:19:58.000000 blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIsSync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       29 2023-05-30 15:57:13.000000 blockchain-apis-0.0.2/blockchain_apis/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.782270 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4725 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1708 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       61 2023-05-30 21:20:17.000000 blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.786270 blockchain-apis-0.0.2/blockchain_apis/exceptions/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainAPIsException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      717 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      710 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/ExchangeNotSupportedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      807 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/InvalidPageException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      830 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/PairNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      809 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/TokenNotFoundException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      743 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/TooManyRequestException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      727 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/UnauthorizedException.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       45 2023-05-30 15:57:38.000000 blockchain-apis-0.0.2/blockchain_apis/exceptions/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.786270 blockchain-apis-0.0.2/blockchain_apis/models/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/AmountIn.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      871 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/AmountOut.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      580 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Blockchain.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      548 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Exchange.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      878 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      678 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Pair.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      944 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      795 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Reserve.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      761 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1838 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/blockchain_apis/models/Tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       42 2023-05-30 15:57:25.000000 blockchain-apis-0.0.2/blockchain_apis/models/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1923 2023-05-30 21:12:34.000000 blockchain-apis-0.0.2/setup.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-30 21:20:17.790270 blockchain-apis-0.0.2/tests/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1565 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_in.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1541 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_in_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1569 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_out.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1545 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_amount_out_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      426 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_blockchains.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      420 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_blockchains_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      602 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_decimals.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      596 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_decimals_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1292 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_exchanges.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1232 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_exchanges_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      594 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_info.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      588 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_info_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2700 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_pairs.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2568 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_pairs_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1393 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_reserves.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1369 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_reserves_sync.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1250 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_tokens.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1190 2023-05-30 12:37:51.000000 blockchain-apis-0.0.2/tests/test_tokens_sync.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1095 2023-05-30 13:02:28.000000 blockchain-apis-0.1.1/LICENSE
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3170 2023-06-02 14:42:47.000000 blockchain-apis-0.1.1/README.md
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       38 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/setup.cfg
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1970 2023-06-02 15:26:36.000000 blockchain-apis-0.1.1/setup.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.523387 blockchain-apis-0.1.1/src/
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.523387 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4722 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/PKG-INFO
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1718 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/SOURCES.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/dependency_links.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       17 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/requires.txt
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       15 2023-06-02 15:26:58.000000 blockchain-apis-0.1.1/src/blockchain_apis.egg-info/top_level.txt
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    24566 2023-06-02 14:37:21.000000 blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    23995 2023-06-02 14:32:42.000000 blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIsSync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      620 2023-06-02 15:16:57.000000 blockchain-apis-0.1.1/src/blockchainapis/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/exceptions/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      454 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainAPIsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      706 2023-06-02 14:30:29.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      699 2023-06-02 14:30:27.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      796 2023-06-02 14:30:24.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/InvalidPageException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      819 2023-06-02 14:30:21.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/PairNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      798 2023-06-02 14:30:19.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/TokenNotFoundException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      733 2023-06-02 14:32:44.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/TooManyRequestsException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      716 2023-06-02 14:30:11.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/UnauthorizedException.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-06-02 14:32:35.000000 blockchain-apis-0.1.1/src/blockchainapis/exceptions/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.527387 blockchain-apis-0.1.1/src/blockchainapis/models/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      860 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/AmountIn.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      871 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/AmountOut.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      580 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Blockchain.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      548 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Exchange.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      865 2023-06-02 14:27:29.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      678 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Pair.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      935 2023-06-02 14:28:25.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      795 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Reserve.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      761 2023-05-30 12:37:51.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Token.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1828 2023-06-02 14:28:34.000000 blockchain-apis-0.1.1/src/blockchainapis/models/Tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1481 2023-06-02 14:07:13.000000 blockchain-apis-0.1.1/src/blockchainapis/models/__init__.py
+drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-06-02 15:26:58.531387 blockchain-apis-0.1.1/tests/
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1564 2023-06-02 14:28:02.000000 blockchain-apis-0.1.1/tests/test_amount_in.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1540 2023-06-02 14:36:02.000000 blockchain-apis-0.1.1/tests/test_amount_in_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1568 2023-06-02 14:36:08.000000 blockchain-apis-0.1.1/tests/test_amount_out.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1544 2023-06-02 14:27:58.000000 blockchain-apis-0.1.1/tests/test_amount_out_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      425 2023-06-02 14:36:12.000000 blockchain-apis-0.1.1/tests/test_blockchains.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      419 2023-06-02 14:36:10.000000 blockchain-apis-0.1.1/tests/test_blockchains_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      569 2023-06-02 14:36:32.000000 blockchain-apis-0.1.1/tests/test_decimals.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      563 2023-06-02 14:36:19.000000 blockchain-apis-0.1.1/tests/test_decimals_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1291 2023-06-02 14:36:44.000000 blockchain-apis-0.1.1/tests/test_exchanges.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1231 2023-06-02 14:36:34.000000 blockchain-apis-0.1.1/tests/test_exchanges_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      593 2023-06-02 14:36:49.000000 blockchain-apis-0.1.1/tests/test_info.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      587 2023-06-02 14:36:46.000000 blockchain-apis-0.1.1/tests/test_info_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2699 2023-06-02 14:36:53.000000 blockchain-apis-0.1.1/tests/test_pairs.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2567 2023-06-02 14:36:51.000000 blockchain-apis-0.1.1/tests/test_pairs_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1392 2023-06-02 14:36:57.000000 blockchain-apis-0.1.1/tests/test_reserves.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1368 2023-06-02 14:36:55.000000 blockchain-apis-0.1.1/tests/test_reserves_sync.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1249 2023-06-02 14:37:01.000000 blockchain-apis-0.1.1/tests/test_tokens.py
+-rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1189 2023-06-02 14:36:59.000000 blockchain-apis-0.1.1/tests/test_tokens_sync.py
```

### Comparing `blockchain-apis-0.0.2/LICENSE` & `blockchain-apis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/PKG-INFO` & `blockchain-apis-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.0.2
+Version: 0.1.1
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
@@ -61,15 +61,15 @@
 `pip install blockchain-apis`
 
 ### Get the current price of ethereum accross all blockchains
 
 ```python
 import asyncio
 
-from BlockchainAPIs import BlockchainAPIs
+from blockchainapis import BlockchainAPIs
 
 async def print_eth_price():
     blockchain_apis = BlockchainAPIs()
     # Get the price of selling 1 ETH to USDT in Ethereum
     eth_price = await blockchain_apis.amount_out(
         blockchain="ethereum",
         amountIn=1000000000000000000,
@@ -77,15 +77,14 @@
         tokenOut="0xdAC17F958D2ee523a2206206994597C13D831ec7"
     )
 
     print(eth_price)
     await blockchain_apis.close()
 
 asyncio.run(print_eth_price())
-
 ```
 
 #### Example response:
 
 ```json
 [
   {
@@ -134,9 +133,7 @@
     "tokenIn": "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2",
     "tokenOut": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
     "amountIn": 1000000000000000000,
     "amountOut": 1904261651
   }
 ]
 ```
-
-
```

### Comparing `blockchain-apis-0.0.2/README.md` & `blockchain-apis-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 `pip install blockchain-apis`
 
 ### Get the current price of ethereum accross all blockchains
 
 ```python
 import asyncio
 
-from BlockchainAPIs import BlockchainAPIs
+from blockchainapis import BlockchainAPIs
 
 async def print_eth_price():
     blockchain_apis = BlockchainAPIs()
     # Get the price of selling 1 ETH to USDT in Ethereum
     eth_price = await blockchain_apis.amount_out(
         blockchain="ethereum",
         amountIn=1000000000000000000,
@@ -44,15 +44,14 @@
         tokenOut="0xdAC17F958D2ee523a2206206994597C13D831ec7"
     )
 
     print(eth_price)
     await blockchain_apis.close()
 
 asyncio.run(print_eth_price())
-
 ```
 
 #### Example response:
 
 ```json
 [
   {
@@ -101,9 +100,7 @@
     "tokenIn": "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2",
     "tokenOut": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
     "amountIn": 1000000000000000000,
     "amountOut": 1904261651
   }
 ]
 ```
-
-
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIs.py` & `blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from typing import Any, Dict, List
 
 from aiohttp import ClientSession
 
-from models.Blockchain import Blockchain
-from models.Exchanges import Exchanges
-from models.Exchange import Exchange
-from models.Pairs import Pairs
-from models.Pair import Pair
-from models.Reserve import Reserve
-from models.AmountOut import AmountOut
-from models.AmountIn import AmountIn
-from models.Tokens import Tokens
-from models.Token import Token
-
-from exceptions.BlockchainNotSupportedException import BlockchainNotSupportedException
-from exceptions.ExchangeNotSupportedException import ExchangeNotSupportedException
-from exceptions.InvalidPageException import InvalidPageException
-from exceptions.TokenNotFoundException import TokenNotFoundException
-from exceptions.PairNotFoundException import PairNotFoundException
-from exceptions.TooManyRequestException import TooManyRequestException
-from exceptions.UnauthorizedException import UnauthorizedException
-
+from .models import Blockchain
+from .models import Exchanges
+from .models import Exchange
+from .models import Pairs
+from .models import Pair
+from .models import Reserve
+from .models import AmountOut
+from .models import AmountIn
+from .models import Tokens
+from .models import Token
+
+from .exceptions import BlockchainNotSupportedException
+from .exceptions import ExchangeNotSupportedException
+from .exceptions import InvalidPageException
+from .exceptions import TokenNotFoundException
+from .exceptions import PairNotFoundException
+from .exceptions import TooManyRequestsException
+from .exceptions import UnauthorizedException
 
 
 class BlockchainAPIs:
     """High-frequency DEX API
 
         
     Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
@@ -102,15 +101,15 @@
                     case "InvalidPageException":
                         raise InvalidPageException(response.status, error_data["detail"]["detail"])
                     case "TokenNotFoundException":
                         raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
                     case "PairNotFoundException":
                         raise PairNotFoundException(response.status, error_data["detail"]["detail"])
                     case "TooManyRequestException":
-                        raise TooManyRequestException(response.status, error_data["detail"]["detail"])
+                        raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
                     case "UnauthorizedException":
                         raise UnauthorizedException(response.status, error_data["detail"]["detail"])
                     case unknown:
                         raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
             return await response.json()
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/BlockchainAPIsSync.py` & `blockchain-apis-0.1.1/src/blockchainapis/BlockchainAPIsSync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import requests
 
 from typing import Any, Dict, List
 from urllib.parse import urljoin
 
-from models.Blockchain import Blockchain
-from models.Exchanges import Exchanges
-from models.Exchange import Exchange
-from models.Pairs import Pairs
-from models.Pair import Pair
-from models.Reserve import Reserve
-from models.AmountOut import AmountOut
-from models.AmountIn import AmountIn
-from models.Tokens import Tokens
-from models.Token import Token
-
-from exceptions.BlockchainNotSupportedException import BlockchainNotSupportedException
-from exceptions.ExchangeNotSupportedException import ExchangeNotSupportedException
-from exceptions.InvalidPageException import InvalidPageException
-from exceptions.TokenNotFoundException import TokenNotFoundException
-from exceptions.PairNotFoundException import PairNotFoundException
-from exceptions.TooManyRequestException import TooManyRequestException
-from exceptions.UnauthorizedException import UnauthorizedException
-
+from .models import Blockchain
+from .models import Exchanges
+from .models import Exchange
+from .models import Pairs
+from .models import Pair
+from .models import Reserve
+from .models import AmountOut
+from .models import AmountIn
+from .models import Tokens
+from .models import Token
+
+from .exceptions import BlockchainNotSupportedException
+from .exceptions import ExchangeNotSupportedException
+from .exceptions import InvalidPageException
+from .exceptions import TokenNotFoundException
+from .exceptions import PairNotFoundException
+from .exceptions import TooManyRequestsException
+from .exceptions import UnauthorizedException
 
 
 class BlockchainAPIsSync:
     """High-frequency DEX API
 
     Our API empowers you to access live financial data across multiple blockchains (currently supporting 6, with more on the way)
     with unparalleled speed and efficiency.
@@ -89,15 +88,15 @@
                 case "InvalidPageException":
                     raise InvalidPageException(response.status, error_data["detail"]["detail"])
                 case "TokenNotFoundException":
                     raise TokenNotFoundException(response.status, error_data["detail"]["detail"])
                 case "PairNotFoundException":
                     raise PairNotFoundException(response.status, error_data["detail"]["detail"])
                 case "TooManyRequestException":
-                    raise TooManyRequestException(response.status, error_data["detail"]["detail"])
+                    raise TooManyRequestsException(response.status, error_data["detail"]["detail"])
                 case "UnauthorizedException":
                     raise UnauthorizedException(response.status, error_data["detail"]["detail"])
                 case unknown:
                     raise Exception(f"Unkwnown Exception type: {unknown}.\nGot this exception while handling:\n{error_data} with status code: {response.status}")
 
         return response.json()
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/blockchain_apis.egg-info/PKG-INFO` & `blockchain-apis-0.1.1/src/blockchain_apis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockchain-apis
-Version: 0.0.2
+Version: 0.1.1
 Summary: Fastest and easiest way to access decentralized finance data
 Home-page: https://www.blockchainapis.io
 Author: Clarensia
 Author-email: contact@blockchainapis.io
 License: MIT
 Project-URL: Documentation, https://api.blockchainapis.io/docs
 Project-URL: Source, https://github.com/blockchainapis/blockchain-apis-python-client
@@ -61,15 +61,15 @@
 `pip install blockchain-apis`
 
 ### Get the current price of ethereum accross all blockchains
 
 ```python
 import asyncio
 
-from BlockchainAPIs import BlockchainAPIs
+from blockchainapis import BlockchainAPIs
 
 async def print_eth_price():
     blockchain_apis = BlockchainAPIs()
     # Get the price of selling 1 ETH to USDT in Ethereum
     eth_price = await blockchain_apis.amount_out(
         blockchain="ethereum",
         amountIn=1000000000000000000,
@@ -77,15 +77,14 @@
         tokenOut="0xdAC17F958D2ee523a2206206994597C13D831ec7"
     )
 
     print(eth_price)
     await blockchain_apis.close()
 
 asyncio.run(print_eth_price())
-
 ```
 
 #### Example response:
 
 ```json
 [
   {
@@ -134,9 +133,7 @@
     "tokenIn": "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2",
     "tokenOut": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
     "amountIn": 1000000000000000000,
     "amountOut": 1904261651
   }
 ]
 ```
-
-
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/BlockchainNotSupportedException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/BlockchainNotSupportedException.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class BlockchainNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid blockchain id is put during a call to the API.
     
     To get the list of valid blockchain ids, call `/blockchains`
     """
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/ExchangeNotSupportedException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/ExchangeNotSupportedException.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class ExchangeNotSupportedException(BlockchainAPIsException):
     """
     Thrown when an Invalid exchange id is given during a call to the API.
     
     To get the list of supported exchange ids, call `/exchanges`
     """
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/InvalidPageException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/InvalidPageException.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class InvalidPageException(BlockchainAPIsException):
     """
     Thrown when you given an invalid page index during calls to responses that
     gives paginated results.
     
     An invalid page is:
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/PairNotFoundException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/PairNotFoundException.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class PairNotFoundException(BlockchainAPIsException):
     """
     Thrown when you try to get some data about a pair that does not exist.
     
     To avoid getting this error, you can get the list of available pairs for
     the blockchain and exchange that you are interested in by calling `/exchanges/pairs`
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/TokenNotFoundException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/TokenNotFoundException.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class TokenNotFoundException(BlockchainAPIsException):
     """
     Thrown when you try to get informations on a token that does not exist inside of our database.
     
     At BlockchainAPIs, we only handle tokens that are inside of a liquidity pool.
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/TooManyRequestException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/TooManyRequestsException.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
+from .BlockchainAPIsException import BlockchainAPIsException
 
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
-
-class TooManyRequestException(BlockchainAPIsException):
+class TooManyRequestsException(BlockchainAPIsException):
     """
     Thrown when you are doing more request than you are allowed to the API.
     
     To prevent this exception you can:
     - Lower the amount of requests that you make to the API per second
     - Upgrade your subscription at: https://dashboard.blockchainapis.io/
     """
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/exceptions/UnauthorizedException.py` & `blockchain-apis-0.1.1/src/blockchainapis/exceptions/UnauthorizedException.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-
-from exceptions.BlockchainAPIsException import BlockchainAPIsException
+from .BlockchainAPIsException import BlockchainAPIsException
 
 class UnauthorizedException(BlockchainAPIsException):
     """
     Thrown when you are trying to make an API request with an invalid or expired
     API key.
     
     To prevent this exception, you can:
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/AmountIn.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/AmountIn.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/AmountOut.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/AmountOut.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Blockchain.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Blockchain.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Exchange.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Exchange.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Exchanges.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Exchanges.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import List
-from models.Exchange import Exchange
+
+from . import Exchange
 
 
 @dataclass(slots=True, frozen=True)
 class Exchanges:
     """The Exchanges model"""
 
     page: int
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Pair.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Pair.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Pairs.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Pairs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import List
-from models.Pair import Pair
+
+from . import Pair
 
 
 @dataclass(slots=True, frozen=True)
 class Pairs:
     """The Pairs model"""
 
     page: int
```

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Reserve.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Reserve.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Token.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Token.py`

 * *Files identical despite different names*

### Comparing `blockchain-apis-0.0.2/blockchain_apis/models/Tokens.py` & `blockchain-apis-0.1.1/src/blockchainapis/models/Tokens.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import List
-from models.Token import Token
+
+from . import Token
 
 
 @dataclass(slots=True, frozen=True)
 class Tokens:
     """The Tokens model"""
 
     page: int
```

### Comparing `blockchain-apis-0.0.2/setup.py` & `blockchain-apis-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
-setuptools.setup(
+setup(
     name = "blockchain-apis",
-    version = "0.0.2",
+    version = "0.1.1",
     author = "Clarensia",
     author_email = "contact@blockchainapis.io",
     description = "Fastest and easiest way to access decentralized finance data",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://www.blockchainapis.io",
     license="MIT",
@@ -40,14 +40,15 @@
     keywords='blockchain crypto cryptocurrency api arbitrage trading ethereum financial-data financial-analysis sdk python defi dex',
     project_urls = {
         'Documentation': 'https://api.blockchainapis.io/docs',
         'Source': 'https://github.com/blockchainapis/blockchain-apis-python-client',
         'Tracker': 'https://github.com/blockchainapis/blockchain-apis-python-client/issues',
         'Discord': 'https://discord.gg/GphRMJXmS5'
     },
-    package_dir = {"": "blockchain_apis"},
+    package_dir = {"": "src"},
+    packages = find_packages(where="src"),
     install_requires = [
         'aiohttp',
         'requests'
     ],
     python_requires = '>=3.10'
-)
+)
```

### Comparing `blockchain-apis-0.0.2/tests/test_amount_in.py` & `blockchain-apis-0.1.1/tests/test_amount_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestAmount_in(BlockchainAPIsTester):
     """
     Test for the method amount_in of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_amount_in_sync.py` & `blockchain-apis-0.1.1/tests/test_amount_in_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestAmount_in(BlockchainAPIsSyncTester):
     """
     Test for the method amount_in of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_amount_out.py` & `blockchain-apis-0.1.1/tests/test_amount_out.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestAmount_out(BlockchainAPIsTester):
     """
     Test for the method amount_out of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_amount_out_sync.py` & `blockchain-apis-0.1.1/tests/test_amount_out_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestAmount_out(BlockchainAPIsSyncTester):
     """
     Test for the method amount_out of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_decimals.py` & `blockchain-apis-0.1.1/tests/test_decimals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-
-from dataclasses import asdict
-
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestDecimals(BlockchainAPIsTester):
     """
     Test for the method decimals of BlockchainAPIs
     """
```

### Comparing `blockchain-apis-0.0.2/tests/test_decimals_sync.py` & `blockchain-apis-0.1.1/tests/test_info_sync.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
-class TestDecimals(BlockchainAPIsSyncTester):
+class TestInfo(BlockchainAPIsSyncTester):
     """
-    Test for the method decimals of BlockchainAPIs
+    Test for the method info of BlockchainAPIs
     """
 
-    def test_decimals_only_required(self):
-        api_result = self.api.decimals(blockchain="ethereum", token="0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
-        api_call = self.do_request("/v0/tokens/decimals", params={
+    def test_info_only_required(self):
+        api_result = self.api.info(blockchain="ethereum", token="0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2")
+        api_call = self.do_request("/v0/tokens/info", params={
             "blockchain": "ethereum",
             "token": "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
         })
-        self.assertEqual(api_result, api_call)
+        self.assertDictEqual(asdict(api_result), api_call)
```

### Comparing `blockchain-apis-0.0.2/tests/test_exchanges.py` & `blockchain-apis-0.1.1/tests/test_exchanges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestExchanges(BlockchainAPIsTester):
     """
     Test for the method exchanges of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_exchanges_sync.py` & `blockchain-apis-0.1.1/tests/test_exchanges_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestExchanges(BlockchainAPIsSyncTester):
     """
     Test for the method exchanges of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_info.py` & `blockchain-apis-0.1.1/tests/test_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestInfo(BlockchainAPIsTester):
     """
     Test for the method info of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_pairs.py` & `blockchain-apis-0.1.1/tests/test_pairs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestPairs(BlockchainAPIsTester):
     """
     Test for the method pairs of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_pairs_sync.py` & `blockchain-apis-0.1.1/tests/test_pairs_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestPairs(BlockchainAPIsSyncTester):
     """
     Test for the method pairs of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_reserves.py` & `blockchain-apis-0.1.1/tests/test_reserves.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestReserves(BlockchainAPIsTester):
     """
     Test for the method reserves of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_reserves_sync.py` & `blockchain-apis-0.1.1/tests/test_reserves_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestReserves(BlockchainAPIsSyncTester):
     """
     Test for the method reserves of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_tokens.py` & `blockchain-apis-0.1.1/tests/test_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsTester import BlockchainAPIsTester
 
 class TestTokens(BlockchainAPIsTester):
     """
     Test for the method tokens of BlockchainAPIs
```

### Comparing `blockchain-apis-0.0.2/tests/test_tokens_sync.py` & `blockchain-apis-0.1.1/tests/test_tokens_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from dataclasses import asdict
 
 from BlockchainAPIsSyncTester import BlockchainAPIsSyncTester
 
 class TestTokens(BlockchainAPIsSyncTester):
     """
     Test for the method tokens of BlockchainAPIs
```

