# Comparing `tmp/bitcoin-utils-0.5.9.tar.gz` & `tmp/bitcoin-utils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin-utils-0.5.9.tar", last modified: Fri Mar  3 08:23:39 2023, max compression
+gzip compressed data, was "bitcoin-utils-0.6.1.tar", last modified: Fri Jun  2 10:28:25 2023, max compression
```

## Comparing `bitcoin-utils-0.5.9.tar` & `bitcoin-utils-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-03-03 08:23:39.953430 bitcoin-utils-0.5.9/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/LICENSE
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     4700 2023-03-03 08:23:39.953430 bitcoin-utils-0.5.9/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     4384 2023-02-07 09:28:14.000000 bitcoin-utils-0.5.9/README.rst
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-03-03 08:23:39.949430 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     4700 2023-03-03 08:23:39.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kostas   (30000) kostas   (30003)      486 2023-03-03 08:23:39.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-03-03 08:23:39.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/not-zip-safe
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       82 2023-03-03 08:23:39.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/requires.txt
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2023-03-03 08:23:39.000000 bitcoin-utils-0.5.9/bitcoin_utils.egg-info/top_level.txt
-drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-03-03 08:23:39.953430 bitcoin-utils-0.5.9/bitcoinutils/
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       23 2023-01-16 19:50:58.000000 bitcoin-utils-0.5.9/bitcoinutils/__init__.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5023 2023-01-16 19:50:58.000000 bitcoin-utils-0.5.9/bitcoinutils/bech32.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     2111 2023-01-16 19:50:58.000000 bitcoin-utils-0.5.9/bitcoinutils/constants.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    40872 2023-03-03 08:22:50.000000 bitcoin-utils-0.5.9/bitcoinutils/keys.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1834 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/proxy.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     5345 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/ripemd160.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    16118 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/script.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)      966 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/setup.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)    28180 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/transactions.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     3040 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/bitcoinutils/utils.py
--rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2023-03-03 08:23:39.953430 bitcoin-utils-0.5.9/setup.cfg
--rw-rw-r--   0 kostas   (30000) kostas   (30003)     1045 2023-01-06 11:32:26.000000 bitcoin-utils-0.5.9/setup.py
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1097 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/LICENSE
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5737 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5421 2023-06-02 10:26:34.000000 bitcoin-utils-0.6.1/README.rst
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5737 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)      535 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)        1 2023-01-10 09:09:10.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/not-zip-safe
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       98 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       13 2023-06-02 10:28:25.000000 bitcoin-utils-0.6.1/bitcoin_utils.egg-info/top_level.txt
+drwxrwxr-x   0 kostas   (30000) kostas   (30003)        0 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/bitcoinutils/
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       23 2023-05-18 16:07:35.000000 bitcoin-utils-0.6.1/bitcoinutils/__init__.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5023 2023-01-16 19:50:58.000000 bitcoin-utils-0.6.1/bitcoinutils/bech32.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     2138 2023-05-18 16:04:30.000000 bitcoin-utils-0.6.1/bitcoinutils/constants.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1944 2023-06-02 10:16:41.000000 bitcoin-utils-0.6.1/bitcoinutils/hdwallet.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    41391 2023-05-31 19:26:29.000000 bitcoin-utils-0.6.1/bitcoinutils/keys.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1834 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/bitcoinutils/proxy.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     5345 2023-05-30 16:59:52.000000 bitcoin-utils-0.6.1/bitcoinutils/ripemd160.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     6259 2023-05-19 14:21:51.000000 bitcoin-utils-0.6.1/bitcoinutils/schnorr.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    16142 2023-05-23 13:35:16.000000 bitcoin-utils-0.6.1/bitcoinutils/script.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)      966 2023-01-06 11:32:26.000000 bitcoin-utils-0.6.1/bitcoinutils/setup.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)    36448 2023-06-01 14:58:58.000000 bitcoin-utils-0.6.1/bitcoinutils/transactions.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     8345 2023-05-31 19:25:36.000000 bitcoin-utils-0.6.1/bitcoinutils/utils.py
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)       38 2023-06-02 10:28:25.305497 bitcoin-utils-0.6.1/setup.cfg
+-rw-rw-r--   0 kostas   (30000) kostas   (30003)     1074 2023-06-01 15:38:14.000000 bitcoin-utils-0.6.1/setup.py
```

### Comparing `bitcoin-utils-0.5.9/LICENSE` & `bitcoin-utils-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.5.9/PKG-INFO` & `bitcoin-utils-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: bitcoin-utils
-Version: 0.5.9
+Version: 0.6.1
 Summary: Bitcoin utility functions
 Home-page: https://github.com/karask/python-bitcoin-utils
 Author: Konstantinos Karasavvas
 Author-email: kkarasavvas@gmail.com
 License: MIT
 Keywords: bitcoin library utilities tools
 Platform: UNKNOWN
 License-File: LICENSE
 
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.5.9) and currently, it supports private/public keys, all type of addresses and creation of any transaction (incl. segwit) with all SIGHASH types. All script op codes are included. Timelock and non-standard transactions are supported. Currently, a simple node proxy exists to enable easy calls to a Bitcoin core node. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.1) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot default key path, with all SIGHASH types. All script op codes are included. Timelocks and non-standard transactions are supported. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
+Notes
+-----
+* For schnorr, bech32[m], ripemd160 the python Bitcoin Core reference implementations are used.
+* For making calls to a Bitcoin node a simple node proxy object exists, which wraps the python-bitcoinrpc library.
+* For Hierarchical Deterministic keys we wrap the python hdwallet library. For now we wrap only some very basic functionality to acquire a PrivateKey object that is used throughtout the library.
 
 Installation
 ------------
 Python version 3 is required. Then just install with:
 
 $ pip install bitcoin-utils
 
 Examples
 --------
 Keys and Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_addresses.py - creates a private key which we use to derive a public key and in turn an address. We also use the private key to sign a message and then verify it using the public key. 
 
+Hierarchical Deterministic Keys
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/hd_keys.py - creates an extended private key, from an xpriv/tpriv and path, which we use to derive a public key and in turn all different address.
+
 Segwit Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_segwit_addresses.py - creates P2WPKH, P2SH-P2WPKH, P2WSH and P2SH-P2WSH addresses.
 
 Transaction with P2PKH input and outputs
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/p2pkh_transaction.py - creates a simple transaction with one input and two outputs.
 
 Create a P2PKH Transaction with different SIGHASHes
@@ -65,10 +73,16 @@
 
 Spend from a timelocked address
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2sh_csv_p2pkh.py - spends from a P2SH(CSV+P2PKH) address as created from above.
 
 Use NodeProxy to make calls to a Bitcoin node
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/node_proxy.py - make Bitcoin command-line interface calls programmatically (NodeProxy wraps jsonrpc-requests library)
 
+Spend from a taproot address
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2tr_default_path.py - single input, single output default key path spending.
+
+Spend a multi input that contains both taproot and legacy UTXOs
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_multi_input_p2tr_and_p2pkh.py - three inputs (two taproot and one legacy), single legacy output.
+
 Please explore the codebase or the API documentation (BitcoinUtilities.pdf) for supported functionality and other options.
```

### Comparing `bitcoin-utils-0.5.9/README.rst` & `bitcoin-utils-0.6.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.5.9) and currently, it supports private/public keys, all type of addresses and creation of any transaction (incl. segwit) with all SIGHASH types. All script op codes are included. Timelock and non-standard transactions are supported. Currently, a simple node proxy exists to enable easy calls to a Bitcoin core node. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.1) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot default key path, with all SIGHASH types. All script op codes are included. Timelocks and non-standard transactions are supported. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
+Notes
+-----
+* For schnorr, bech32[m], ripemd160 the python Bitcoin Core reference implementations are used.
+* For making calls to a Bitcoin node a simple node proxy object exists, which wraps the python-bitcoinrpc library.
+* For Hierarchical Deterministic keys we wrap the python hdwallet library. For now we wrap only some very basic functionality to acquire a PrivateKey object that is used throughtout the library.
 
 Installation
 ------------
 Python version 3 is required. Then just install with:
 
 $ pip install bitcoin-utils
 
 Examples
 --------
 Keys and Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_addresses.py - creates a private key which we use to derive a public key and in turn an address. We also use the private key to sign a message and then verify it using the public key. 
 
+Hierarchical Deterministic Keys
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/hd_keys.py - creates an extended private key, from an xpriv/tpriv and path, which we use to derive a public key and in turn all different address.
+
 Segwit Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_segwit_addresses.py - creates P2WPKH, P2SH-P2WPKH, P2WSH and P2SH-P2WSH addresses.
 
 Transaction with P2PKH input and outputs
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/p2pkh_transaction.py - creates a simple transaction with one input and two outputs.
 
 Create a P2PKH Transaction with different SIGHASHes
@@ -53,8 +61,14 @@
 
 Spend from a timelocked address
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2sh_csv_p2pkh.py - spends from a P2SH(CSV+P2PKH) address as created from above.
 
 Use NodeProxy to make calls to a Bitcoin node
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/node_proxy.py - make Bitcoin command-line interface calls programmatically (NodeProxy wraps jsonrpc-requests library)
 
+Spend from a taproot address
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2tr_default_path.py - single input, single output default key path spending.
+
+Spend a multi input that contains both taproot and legacy UTXOs
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_multi_input_p2tr_and_p2pkh.py - three inputs (two taproot and one legacy), single legacy output.
+
 Please explore the codebase or the API documentation (BitcoinUtilities.pdf) for supported functionality and other options.
```

### Comparing `bitcoin-utils-0.5.9/bitcoin_utils.egg-info/PKG-INFO` & `bitcoin-utils-0.6.1/bitcoin_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 Metadata-Version: 2.1
 Name: bitcoin-utils
-Version: 0.5.9
+Version: 0.6.1
 Summary: Bitcoin utility functions
 Home-page: https://github.com/karask/python-bitcoin-utils
 Author: Konstantinos Karasavvas
 Author-email: kkarasavvas@gmail.com
 License: MIT
 Keywords: bitcoin library utilities tools
 Platform: UNKNOWN
 License-File: LICENSE
 
 python-bitcoin-utils
 ====================
 
 This is a bitcoin library that provides tools/utilities to interact with the Bitcoin network. One of the primary goals of the library is to explain the low-level details of Bitcoin. The code is easy to read and properly documented explaining in detail all the thorny aspects of the implementation. It is a low-level library which assumes some high-level understanding of how Bitcoin works. In the future this might change.
 
-This is an early version of the library (v0.5.9) and currently, it supports private/public keys, all type of addresses and creation of any transaction (incl. segwit) with all SIGHASH types. All script op codes are included. Timelock and non-standard transactions are supported. Currently, a simple node proxy exists to enable easy calls to a Bitcoin core node. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
+This is an early version of the library (v0.6.1) and currently, it supports private/public keys, all type of addresses and creation of any transaction, incl. segwit and taproot default key path, with all SIGHASH types. All script op codes are included. Timelocks and non-standard transactions are supported. Extra functionality will be added continuously and the documentation will be improved as the work progresses.
 
 The API documentation can be build with Sphinx but is also available as a PDF for convenience. One can currently use the library for experimenting and learning the inner workings of Bitcoin. It is not meant for production yet and parts of the API might be updated with new versions.
 
 Complementary to this library is a CC BY-SA 4.0 licensed `Bitcoin programming book <https://github.com/karask/bitcoin-textbook>`_.
 
+Notes
+-----
+* For schnorr, bech32[m], ripemd160 the python Bitcoin Core reference implementations are used.
+* For making calls to a Bitcoin node a simple node proxy object exists, which wraps the python-bitcoinrpc library.
+* For Hierarchical Deterministic keys we wrap the python hdwallet library. For now we wrap only some very basic functionality to acquire a PrivateKey object that is used throughtout the library.
 
 Installation
 ------------
 Python version 3 is required. Then just install with:
 
 $ pip install bitcoin-utils
 
 Examples
 --------
 Keys and Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_addresses.py - creates a private key which we use to derive a public key and in turn an address. We also use the private key to sign a message and then verify it using the public key. 
 
+Hierarchical Deterministic Keys
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/hd_keys.py - creates an extended private key, from an xpriv/tpriv and path, which we use to derive a public key and in turn all different address.
+
 Segwit Addresses
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/keys_segwit_addresses.py - creates P2WPKH, P2SH-P2WPKH, P2WSH and P2SH-P2WSH addresses.
 
 Transaction with P2PKH input and outputs
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/p2pkh_transaction.py - creates a simple transaction with one input and two outputs.
 
 Create a P2PKH Transaction with different SIGHASHes
@@ -65,10 +73,16 @@
 
 Spend from a timelocked address
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2sh_csv_p2pkh.py - spends from a P2SH(CSV+P2PKH) address as created from above.
 
 Use NodeProxy to make calls to a Bitcoin node
   https://github.com/karask/python-bitcoin-utils/blob/master/examples/node_proxy.py - make Bitcoin command-line interface calls programmatically (NodeProxy wraps jsonrpc-requests library)
 
+Spend from a taproot address
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_p2tr_default_path.py - single input, single output default key path spending.
+
+Spend a multi input that contains both taproot and legacy UTXOs
+  https://github.com/karask/python-bitcoin-utils/blob/master/examples/spend_multi_input_p2tr_and_p2pkh.py - three inputs (two taproot and one legacy), single legacy output.
+
 Please explore the codebase or the API documentation (BitcoinUtilities.pdf) for supported functionality and other options.
```

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/bech32.py` & `bitcoin-utils-0.6.1/bitcoinutils/bech32.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/constants.py` & `bitcoin-utils-0.6.1/bitcoinutils/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 P2PKH_ADDRESS = "p2pkh"
 P2SH_ADDRESS = "p2sh"
 P2WPKH_ADDRESS_V0 = "p2wpkhv0"
 P2WSH_ADDRESS_V0 = "p2wshv0"
 P2TR_ADDRESS_V1 = "p2trv1"
 
+TAPROOT_SIGHASH_ALL = 0x00
 SIGHASH_ALL = 0x01
 SIGHASH_NONE = 0x02
 SIGHASH_SINGLE = 0x03
 SIGHASH_ANYONECANPAY = 0x80
 
 TYPE_ABSOLUTE_TIMELOCK = 0x101
 TYPE_RELATIVE_TIMELOCK = 0x201
```

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/keys.py` & `bitcoin-utils-0.6.1/bitcoinutils/keys.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,71 +12,34 @@
 import re
 import struct
 import hashlib
 from abc import ABC, abstractmethod
 from base64 import b64encode, b64decode
 from binascii import unhexlify, hexlify
 from base58check import b58encode, b58decode
-from ecdsa import SigningKey, VerifyingKey, SECP256k1, ellipticcurve, numbertheory
+from ecdsa import SigningKey, VerifyingKey, SECP256k1, numbertheory, ellipticcurve
 from ecdsa.util import sigencode_string, sigdecode_string, sigencode_der
 from sympy.ntheory import sqrt_mod
 
 from bitcoinutils.constants import NETWORK_WIF_PREFIXES, \
         NETWORK_P2PKH_PREFIXES, NETWORK_P2SH_PREFIXES, SIGHASH_ALL, \
         P2PKH_ADDRESS, P2SH_ADDRESS, P2WPKH_ADDRESS_V0, P2WSH_ADDRESS_V0, \
-        P2TR_ADDRESS_V1, NETWORK_SEGWIT_PREFIXES
+        P2TR_ADDRESS_V1, NETWORK_SEGWIT_PREFIXES, TAPROOT_SIGHASH_ALL
 from bitcoinutils.setup import get_network
-from bitcoinutils.utils import bytes_from_int, encode_varint
+from bitcoinutils.utils import bytes32_from_int, encode_varint, add_magic_prefix, \
+                               hex_str_to_int, \
+                               tweak_taproot_pubkey, \
+                               tweak_taproot_privkey
 from bitcoinutils.ripemd160 import ripemd160
+from bitcoinutils.schnorr import schnorr_sign
+from bitcoinutils.utils import EcdsaParams
 import bitcoinutils.script
 import bitcoinutils.bech32
 
 
-# ECDSA curve using secp256k1 is defined by: y**2 = x**3 + 7
-# This is done modulo p which (secp256k1) is:
-# p is the finite field prime number and is equal to:
-# 2^256 - 2^32 - 2^9 - 2^8 - 2^7 - 2^6 - 2^4 - 1
-# Note that we could also get that from ecdsa lib from the curve, e.g.:
-# SECP256k1.__dict__['curve'].__dict__['_CurveFp__p']
-_p = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEFFFFFC2F
-# Curve's a and b are (y**2 = x**3 + a*x + b)
-_a = 0x0000000000000000000000000000000000000000000000000000000000000000
-_b = 0x0000000000000000000000000000000000000000000000000000000000000007
-# Curve's generator point is:
-_Gx = 0x79BE667EF9DCBBAC55A06295CE870B07029BFCDB2DCE28D959F2815B16F81798
-_Gy = 0x483ada7726a3c4655da4fbfc0e1108a8fd17b448a68554199c47d08ffb10d4b8
-# prime number of points in the group (the order)
-_order = 0xFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFEBAAEDCE6AF48A03BBFD25E8CD0364141
-
-# The ECDSA curve (secp256k1) is:
-# Note that we could get that from ecdsa lib, e.g.:
-# SECP256k1.__dict__['curve']
-_curve = ellipticcurve.CurveFp( _p, _a, _b )
-
-# The generator base point is:
-# Note that we could get that from ecdsa lib, e.g.:
-# SECP256k1.__dict__['generator']
-_G = ellipticcurve.Point( _curve, _Gx, _Gy, _order )
-
-
-
-
-# method used by both PrivateKey and PublicKey - TODO clean - add in another module?
-def add_magic_prefix(message):
-    magic_prefix = b'\x18Bitcoin Signed Message:\n'
-    # need to use varint for big messages
-    # note that previously big-endian was used but varint uses little-endian
-    # successfully tested with signatures from bitcoin core but keep this in mind
-    message_size = encode_varint(len(message))
-    message_encoded = message.encode('utf-8')
-    message_magic = magic_prefix + message_size + message_encoded
-    return message_magic
-
-
-
 class PrivateKey:
     """Represents an ECDSA private key.
 
     Attributes
     ----------
     key : bytes
         the raw key of 32 bytes
@@ -263,14 +226,21 @@
     def sign_segwit_input(self, tx, txin_index, script, amount, sighash=SIGHASH_ALL):
         # the tx knows how to calculate the digest for the corresponding
         # sighash)
         tx_digest = tx.get_transaction_segwit_digest(txin_index, script, amount, sighash)
         return self._sign_input(tx_digest, sighash)
 
 
+    def sign_taproot_input(self, tx, txin_index, utxo_scripts, amounts, sighash=TAPROOT_SIGHASH_ALL):
+        # the tx knows how to calculate the digest for the corresponding
+        # sighash)
+        tx_digest = tx.get_transaction_taproot_digest(txin_index, utxo_scripts, amounts, 0, sighash)
+        return self._sign_taproot_input(tx_digest, sighash)
+
+
     def _sign_input(self, tx_digest, sighash=SIGHASH_ALL):
         """Signs a transaction input with the private key
 
         Bitcoin uses the normal DER format for transactions. Each input is
         signed separately (thus txin_index is required). The script of the
         input we wish to spend is required and replaces the transaction's
         script sig in order to calculate the correct transaction hash (which
@@ -302,15 +272,15 @@
 
         # if high R re-sign until we get a low R value
         # if high R then its size will be 33 bytes to include the sign
         attempt = 1
         length_r = signature[3]
         while(length_r == 33):
             signature = self.key.sign_digest_deterministic(tx_digest,
-                                                           extra_entropy=bytes_from_int(attempt),
+                                                           extra_entropy=bytes32_from_int(attempt),
                                                            sigencode=sigencode_der,
                                                            hashfunc=hashlib.sha256)
             attempt += 1
             length_r = signature[3]
         
         
         # make sure that signature complies with Low S standardness rule of
@@ -343,65 +313,84 @@
         S = signature[5 + length_r + 1:]
         S_as_bigint = int( hexlify(S).decode('utf-8'), 16 )
 
         # update S -- Low S standardness rule
 
         # if length is 33 bytes then it contains a sign and thus is high S
         if(length_s == 33):
-            new_S_as_bigint = _order - S_as_bigint 
+            new_S_as_bigint = EcdsaParams._order - S_as_bigint 
             # convert bigint to bytes
+            # TODO maybe use f'{new_S_as_bigint:064x}' - make sure zfill pads the same
             new_S = unhexlify( format(new_S_as_bigint, 'x').zfill(64) )
             # new value should be 32 bytes
             assert len(new_S) == 0x20
             # reduce appropriate lengths
             length_s -= 1
             length_total -= 1
         else:
             new_S = S
 
 
-# TODO CLEAN old low std rules
-        #half_order = _order // 2
-        # if S is larger than half the order then substruct from order and
-        # use that as S since it is equivalent.
-        #if S_as_bigint > half_order:
-        #    # make sure length is 33 bytes (it should be)
-        #    assert length_s == 0x21
-
-        #    new_S_as_bigint = _order - S_as_bigint
-        #    # convert bigint to bytes
-        #    new_S = unhexlify( format(new_S_as_bigint, 'x').zfill(64) )
-        #    # new value should be 32 bytes
-        #    assert len(new_S) == 0x20
-        #    # reduce appropriate lengths
-        #    length_s -= 1
-        #    length_total -= 1
-        #else:
-        #    new_S = S
-
-
         # reconstruct signature
         signature = struct.pack('BBBB', der_prefix, length_total, der_type_int, length_r) + R + \
                         struct.pack('BB', der_type_int, length_s) + new_S
 
         # add sighash in the signature -- as one byte!
         signature += struct.pack('B', sighash)
 
         # note that this is the final sig that needs to be added in the
         # script_sig (i.e. the DER signature plus the sighash)
         return hexlify(signature).decode('utf-8')
 
 
+
+    def _sign_taproot_input(self, tx_digest, sighash=SIGHASH_ALL):
+        """Signs a taproot transaction input with the private key
+
+        Taproot uses Schnorr signatures. The format is just R and S so only
+        64 bytes. If SIGHASH_ALL then nothing is included (i.e. default).
+        If another sighash then it is included in the end (65 bytes).
+
+        Returns a signature for that input
+        """
+
+        # tweak private key before signing (tweaking code takes care of
+        # negating the private key if it is necessary (i.e. if
+        # the corresponding public key's y is odd).
+        tagged_key = tweak_taproot_privkey(self.key.to_string(), 'TapTweak')
+
+        byte_key = unhexlify(tagged_key)
+
+        # deterministic signing nonce is random and based in RFC6979
+        # it is the hash of the tx_digest and private key
+        # TODO not identical to Bitcoin Core's signature, rand_aux
+        # needs slight changes if we want identical signatures!
+        rand_aux = hashlib.sha256(tx_digest + byte_key).digest()
+
+        # use BIP-340 python's reference implementation for signing
+        sig = schnorr_sign(tx_digest, byte_key, rand_aux)
+
+        # 65 bytes if sighash is not TAPROOT_SIGHASH_ALL
+        if sighash != TAPROOT_SIGHASH_ALL:
+            sig += sighash.to_bytes(1, 'big')
+
+        sig_hex = hexlify(sig)
+        
+        return sig_hex 
+
+
+
     def get_public_key(self):
         """Returns the corresponding PublicKey"""
 
         verifying_key = hexlify(self.key.get_verifying_key().to_string())
         return PublicKey( '04' + verifying_key.decode('utf-8') )
 
 
+
 class PublicKey:
     """Represents an ECDSA public key.
 
     Attributes
     ----------
     key : bytes
         the raw public key of 64 bytes (x, y coordinates of the ECDSA curve)
@@ -416,22 +405,26 @@
         Class method that constructs the public key, confirms the address and
         verifies the signature
     verify(signature, message)
         returns true if the message was signed with this public key's
         corresponding private key.
     to_hex(compressed=True)
         returns the key as hex string (in SEC format - compressed by default)
+    to_taproot_hex()
+        returns the x coordinate only as hex string (needed for taproot)
     to_bytes()
         returns the key's raw bytes
     to_hash160()
         returns the hash160 hex string of the public key
     get_address(compressed=True))
         returns the corresponding P2pkhAddress object
     get_segwit_address()
         returns the corresponding P2wpkhAddress object
+    get_taproot_address()
+        returns the corresponding P2trAddress object
     """
 
 
     def __init__(self, hex_str):
         """
         Parameters
         ----------
@@ -444,44 +437,53 @@
             If first byte of public key (corresponding to SEC format) is
             invalid.
         """
 
         # expects key as hex string - SEC format
         first_byte_in_hex = hex_str[:2] # 2 since a byte is represented by 2 hex characters
         hex_bytes = unhexlify(hex_str)
+        # TODO needed?? - see flag below
+        taproot = False 
 
         # check if compressed or not
         if len(hex_bytes) > 33:
             # uncompressed - SEC format: 0x04 + x + y coordinates (x,y are 32 byte numbers)
             # remove first byte and instantiate ecdsa key
             self.key = VerifyingKey.from_string(hex_bytes[1:], curve=SECP256k1)
-        else:
+        elif len(hex_bytes) > 31:
+            # key is either compressed or in x-only taproot format
+
+            # taproot is 32 bytes and it should always be prefixed with 0x02
+            if len(hex_bytes) == 32:
+                taproot = True 
+
             # compressed - SEC FORMAT: 0x02|0x03 + x coordinate (if 02 then y
             # is even else y is odd. Calculate y and then instantiate the ecdsa key
             x_coord = int( hex_str[2:], 16 )
 
             # y = modulo_square_root( (x**3 + 7) mod p ) -- there will be 2 y values
-            y_values = sqrt_mod( (x_coord**3 + 7) % _p, _p, True )
+            y_values = sqrt_mod( (x_coord**3 + 7) % EcdsaParams._p, EcdsaParams._p, True )
 
             # check SEC format's first byte to determine which of the 2 values to use
-            if first_byte_in_hex == '02':
+            if first_byte_in_hex == '02' or taproot:
                 # y is the even value
                 if y_values[0] % 2 == 0:
                     y_coord = y_values[0]
                 else:
                     y_coord = y_values[1]
             elif first_byte_in_hex == '03':
                 # y is the odd value
                 if y_values[0] % 2 == 0:
                     y_coord = y_values[1]
                 else:
                     y_coord = y_values[0]
             else:
                 raise TypeError("Invalid SEC compressed format")
 
+            # TODO use f'{x_coord:064x}{y_coord:064x}' instead
             uncompressed_hex = "%0.64X%0.64X" % (x_coord, y_coord)
             uncompressed_hex_bytes = unhexlify(uncompressed_hex)
             self.key = VerifyingKey.from_string(uncompressed_hex_bytes, curve=SECP256k1)
 
 
     @classmethod
     def from_hex(cls, hex_str):
@@ -492,15 +494,15 @@
 
     def to_bytes(self):
         """Returns key's bytes"""
 
         return self.key.to_string()
 
 
-    def to_hex(self, compressed=True, taproot=False):
+    def to_hex(self, compressed=True):
         """Returns public key as a hex string (SEC format - compressed by
         default)"""
 
         key_hex = hexlify(self.key.to_string())
 
         if compressed:
             # check if y is even or odd (02 even, 03 odd)
@@ -508,31 +510,34 @@
                 key_str = b'02' + key_hex[:64]
             else:
                 key_str = b'03' + key_hex[:64]
         else:
             # uncompressed starts with 04
             key_str = b'04' + key_hex
 
-	# this was added for taproot but will be refactored!
-        #if compressed:
-        #    if not taproot:
-        #        # check if y is even or odd (02 even, 03 odd)
-        #        if int(key_hex[-2:], 16) % 2 == 0:
-        #            key_str = b'02' + key_hex[:64]
-        #        else:
-        #            key_str = b'03' + key_hex[:64]
-        #    else:
-        #        key_str = key_hex[:64]
-        #else:
-        #    # uncompressed starts with 04
-        #    key_str = b'04' + key_hex
-
         return key_str.decode('utf-8')
 
 
+    # TODO probably remove tagged flag in the future to always tag the public key
+    # Note that we do not optionally tag the private key when signing!!!
+    def to_taproot_hex(self, tagged=True):
+        """Returns the x coordinate of the public key as a hex string.
+
+        Tweaks and negates, if necessary, the key first.
+        """
+        if tagged:
+            # public key in x form only (TODO pass x-only for here rather than
+            # do it from tweak_taproot_pubkey!?)
+            pubkey = tweak_taproot_pubkey(self.key.to_string(), 'TapTweak')[:64]
+        else:
+            pubkey = self.to_hex(compressed=True)[2:]
+
+        return pubkey
+
+
     @classmethod
     def from_message_signature(self, signature):
         # TODO implement (add signature=None in __init__, etc.)
         # TODO plus does this apply to DER signatures as well?
         #return cls(signature=signature)
         raise BaseException('NO-OP!')
 
@@ -581,38 +586,38 @@
         message_digest = hashlib.sha256( hashlib.sha256(message_magic).digest() ).digest()
 
         #
         # use recid, r and s to get the point in the curve
         #
 
         # get signature's r and s
-        r,s = sigdecode_string(sig[1:], _order)
+        r,s = sigdecode_string(sig[1:], EcdsaParams._order)
 
         # ger R's x coordinate
-        x = r + (recid // 2) * _order
+        x = r + (recid // 2) * EcdsaParams._order
 
         # get R's y coordinate (y**2 = x**3 + 7)
-        y_values = sqrt_mod( (x**3 + 7) % _p, _p, True )
+        y_values = sqrt_mod( (x**3 + 7) % EcdsaParams._p, EcdsaParams._p, True )
         if (y_values[0] - recid) % 2 == 0:
             y = y_values[0]
         else:
             y = y_values[1]
 
         # get R (recovered ephemeral key) from x,y
-        R = ellipticcurve.Point(_curve, x, y, _order)
+        R = ellipticcurve.Point(EcdsaParams._curve, x, y, EcdsaParams._order)
 
         # get e (hash of message encoded as big integer)
         e = int(hexlify(message_digest), 16)
 
         # compute public key Q = r^-1 (sR - eG)
         # because Point substraction is not defined we will instead use:
         # Q = r^-1 (sR + (-eG) )
-        minus_e = -e % _order
-        inv_r = numbertheory.inverse_mod(r, _order)
-        Q = inv_r * ( s*R + minus_e*_G )
+        minus_e = -e % EcdsaParams._order
+        inv_r = numbertheory.inverse_mod(r, EcdsaParams._order)
+        Q = inv_r * ( s*R + minus_e*EcdsaParams._G )
 
         # instantiate the public key and verify message
         public_key = VerifyingKey.from_public_point( Q, curve = SECP256k1 )
         key_hex = hexlify(public_key.to_string()).decode('utf-8')
         pubkey = PublicKey.from_hex('04' + key_hex)
         if not pubkey.verify(signature, message):
             return False
@@ -669,28 +674,30 @@
         """Returns the corresponding P2WPKH address
 
         Only compressed is allowed. It is otherwise identical to normal P2PKH
         address.
         """
         hash160 = self._to_hash160(True)
         addr_string_hex = hexlify(hash160).decode('utf-8')
-        return P2wpkhAddress(witness_hash=addr_string_hex)
+        return P2wpkhAddress(witness_program=addr_string_hex)
+
+
+    def get_taproot_address(self):
+        """Returns the corresponding P2TR address
+
+        Only compressed is allowed. Taproot uses x-only public key with
+        even y (02 compressed keys). By default tagged_hashes are used.
+        """
 
-# TODO cleam tmp taproot stuff!	
-#    def get_taproot_address(self):
-#        """Returns the corresponding P2TR address
-#
-#        Only compressed is allowed. Taproot does not hash the public key
-#        so we store it directly.
-#        """
-#
-#        # Note that in taproot it is not really the hash.. just the compressed
-#        # public key without a prefix!
-#        pubkey = self.to_hex(compressed=True, taproot=True) 
-#        return P2trAddress(witness_hash=pubkey)
+        # Tweak public key (BIP340)
+        # https://bitcoin.stackexchange.com/a/116391/31844
+        # note that taproot's even y is checked/negated during tweaking
+        pubkey = tweak_taproot_pubkey(self.key.to_string(), 'TapTweak')[:64]
+
+        return P2trAddress(witness_program=pubkey)
 
 
 class Address(ABC):
     """Represents a Bitcoin address
 
     Attributes
     ----------
@@ -947,24 +954,26 @@
     """Represents a Bitcoin segwit address
 
     Note that currently the python bech32[m] reference implementation is used (by
     Pieter Wuille).
 
     Attributes
     ----------
-    witness_hash : str
-        the hash string representation of either the address; it can be either
-        a public key hash (P2WPKH) or the hash of the script (P2WSH)
+    witness_program : str
+        for segwit v0 this is the hash string representation of either the address;
+        it can be either a public key hash (P2WPKH) or the hash of the script (P2WSH)
+
+        for segwit v1 (aka taproot) this is the public key
 
     Methods
     -------
     from_address(address)
         instantiates an object from address string encoding
-    from_hash(hash_str)
-        instantiates an object from a hash hex string
+    from_program(hash_str)
+        instantiates an object from a witness program hex string
     from_script(witness_script)
         instantiates an object from a witness_script
     to_string()
         returns the address's string encoding (Bech32)
     to_hash()
         returns the address's hash hex string representation
 
@@ -972,23 +981,23 @@
     ------
     TypeError
         No parameters passed
     ValueError
         If an invalid address or hash is provided.
     """
     @abstractmethod
-    def __init__(self, address=None, witness_hash=None, script=None,
+    def __init__(self, address=None, witness_program=None, script=None,
                  version=P2WPKH_ADDRESS_V0):
         """
         Parameters
         ----------
         address : str
             the address as a string
-        witness_hash : str
-            the hash hex string representation
+        witness_program : str
+            the witness program hex string representation
         script : Script object
             instantiates an Address object from a witness script
         version : str
             specifies the default segwit version
 
         Raises
         ------
@@ -997,46 +1006,46 @@
         ValueError
             If an invalid address or hash is provided.
         """
 
         self.version = version
         if self.version == P2WPKH_ADDRESS_V0 or self.version == P2WSH_ADDRESS_V0:
             self.segwit_num_version = 0
-# TODO clean tmp taprrot stuff
-#        elif self.version == P2TR_ADDRESS_V1:
-#            self.segwit_num_version = 1
-#        else:
-#            raise TypeError("A valid segwit version is required.")
+        elif self.version == P2TR_ADDRESS_V1:
+            self.segwit_num_version = 1
+        else:
+            raise TypeError("A valid segwit version is required.")
 
-        if witness_hash:
-            self.witness_hash = witness_hash
+        # witness_program covers both v0 and v1
+        if witness_program:
+            self.witness_program = witness_program
         elif address:
-            self.witness_hash = self._address_to_hash(address)
+            self.witness_program = self._address_to_hash(address)
         elif script:
             # TODO for now just check that is an instance of Script
             if isinstance(script, bitcoinutils.script.Script):
-                self.witness_hash = self._script_to_hash(script)
+                self.witness_program = self._script_to_hash(script)
             else:
                 raise TypeError("A Script class is required.")
         else:
-            raise TypeError("A valid address or hash is required.")
+            raise TypeError("A valid address or witness program is required.")
 
 
     @classmethod
     def from_address(cls, address):
         """Creates an address object from an address string"""
 
         return cls(address=address)
 
 
     @classmethod
-    def from_hash(cls, witness_hash):
+    def from_witness_program(cls, witness_program):
         """Creates an address object from a hash string"""
 
-        return cls(witness_hash=witness_hash)
+        return cls(witness_program=witness_program)
 
 
     @classmethod
     def from_script(cls, script):
         """Creates an address object from a Script object"""
 
         return cls(script=script)
@@ -1065,28 +1074,27 @@
         """Converts a script to it's hash equivalent"""
 
         script_bytes = script.to_bytes()
         hashsha256 = hashlib.sha256(script_bytes).digest()
         return hexlify(hashsha256).decode('utf-8')
 
 
-    def to_hash(self):
-        """Returns as hash hex string"""
+    def to_witness_program(self):
+        """Returns witness program as hex string"""
 
-        return self.witness_hash
+        return self.witness_program
 
 
     def to_string(self):
         """Returns as address string
 
         Uses a segwit's python reference implementation for now. (TODO)
         """
 
-        # convert hex string hash to int array (required by bech32 lib)
-        hash_bytes = unhexlify( self.witness_hash.encode('utf-8') )
+        hash_bytes = unhexlify( self.witness_program.encode('utf-8') )
         witness_int_array = memoryview(hash_bytes).tolist()
 
         return bitcoinutils.bech32.encode(NETWORK_SEGWIT_PREFIXES[get_network()],
                                           self.segwit_num_version, witness_int_array)
 
 
 
@@ -1100,25 +1108,25 @@
     to_script_pub_key()
         returns the scriptPubKey of a P2WPKH witness script
     get_type()
         returns the type of address
     """
 
     # TODO allow creation directly from Bech32 address !!
-    def __init__(self, address=None, witness_hash=None,
+    def __init__(self, address=None, witness_program=None,                  # script=None, ?
                  version=P2WPKH_ADDRESS_V0):
         """Allow creation only from hash160 of public key"""
 
-        super().__init__(address=address, witness_hash=witness_hash,
+        super().__init__(address=address, witness_program=witness_program,  # script=None, ?
                          version=P2WPKH_ADDRESS_V0) # non-variable version
 
 
     def to_script_pub_key(self):
         """Returns the scriptPubKey of a P2WPKH witness script"""
-        return bitcoinutils.script.Script(['OP_0', self.to_hash()])
+        return bitcoinutils.script.Script(['OP_0', self.to_witness_program()])
 
 
     def get_type(self):
         """Returns the type of address"""
         return self.version
 
 
@@ -1131,66 +1139,61 @@
     -------
     from_script(witness_script)
         instantiates an object from a witness_script
     get_type()
         returns the type of address
     """
 
-    def __init__(self, address=None, witness_hash=None, script=None,
+    def __init__(self, address=None, witness_program=None, script=None,
                  version=P2WSH_ADDRESS_V0):
         """Allow creation only from hash160 of public key"""
 
-        super().__init__(address=None, witness_hash=None, script=script,
+        super().__init__(address=None, witness_program=None, script=script,
                          version=P2WSH_ADDRESS_V0) # non-variable version
 
 
     def to_script_pub_key(self):
         """Returns the scriptPubKey of a P2WPKH witness script"""
-        return bitcoinutils.script.Script(['OP_0', self.to_hash()])
+        return bitcoinutils.script.Script(['OP_0', self.to_witness_program()])
 
 
     def get_type(self):
         """Returns the type of address"""
         return self.version
 
 
-# TODO CLEAN UP tmp taproot stuff
-# this was added for taproot but will be refactored!
-#class P2trAddress(SegwitAddress):
-#    """Encapsulates a P2TR (Taproot) address.
-#
-#    Check Address class for details
-#
-#    Methods
-#    -------
-#    to_script_pub_key()
-#        returns the scriptPubKey of a P2WPKH witness script
-#    get_type()
-#        returns the type of address
-#    """
-#
-#    # TODO  DOES SegwitAddress's init from_script make sense for Taproot??
-#
-#    def __init__(self, address=None, witness_hash=None,
-#                 version=P2TR_ADDRESS_V1):
-#        """Allow creation only from address and public key (witness_hash is not
-#           a hash in taproot, just the compress public key hex)"""
-#
-#        super().__init__(address=address, witness_hash=witness_hash,
-#                         version=P2TR_ADDRESS_V1)
-#
-#
-#    def to_script_pub_key(self):
-#        """Returns the scriptPubKey of a P2TR witness script"""
-#        return bitcoinutils.script.Script(['OP_1', self.to_hash()])
-#
-#
-#    def get_type(self):
-#        """Returns the type of address"""
-#        return self.version
+class P2trAddress(SegwitAddress):
+    """Encapsulates a P2TR (Taproot) address.
+
+    Check Address class for details
+
+    Methods
+    -------
+    to_script_pub_key()
+        returns the scriptPubKey of a P2TR witness script
+    get_type()
+        returns the type of address
+    """
+
+    def __init__(self, address=None, witness_program=None,                  # script=None, ?
+                 version=P2TR_ADDRESS_V1):
+        """Allow creation only from witness program"""
+
+        super().__init__(address=address, witness_program=witness_program,  # script=None, ?
+                         version=P2TR_ADDRESS_V1)
+
+
+    def to_script_pub_key(self):
+        """Returns the scriptPubKey of a P2TR witness script"""
+        return bitcoinutils.script.Script(['OP_1', self.to_witness_program()])
+
+
+    def get_type(self):
+        """Returns the type of address"""
+        return self.version
 
 
 
 
 def main():
     pass
```

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/proxy.py` & `bitcoin-utils-0.6.1/bitcoinutils/proxy.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/ripemd160.py` & `bitcoin-utils-0.6.1/bitcoinutils/ripemd160.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/script.py` & `bitcoin-utils-0.6.1/bitcoinutils/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,17 +252,23 @@
         the list with all the script OP_CODES and data
 
     Methods
     -------
     to_bytes()
         returns a serialized byte version of the script
 
+    to_hex()
+        returns a serialized version of the script in hex
+
     get_script()
         returns the list of strings that makes up this script
 
+    copy()
+        creates a copy of the object (classmethod)
+
     Raises
     ------
     ValueError
         If string data is too large or integer is negative
     """
 
     def __init__(self, script):
@@ -308,51 +314,51 @@
             return b'\x4d' + struct.pack('<H', len(data_bytes)) + data_bytes
         elif len(data_bytes) < 0xffffffff:
             return b'\x4e' + struct.pack('<I', len(data_bytes)) + data_bytes
         else:
             raise ValueError("Data too large. Cannot push into script")
 
 
-    def _segwit_op_push_data(self, data):
+#    def _segwit_op_push_data(self, data):
         # expects data in hexadecimal characters and converts to bytes with
         # varint (or compact size) length prefix.
         #
         # TODO maybe, for convenience, also accept objects for public keys,
         # addresses, etc. and use isinstance and convert manually
-        data_bytes = unhexlify(data)
+#        data_bytes = unhexlify(data)
 
         # return prepended varint (compact size) length to data bytes
-        return prepend_varint(data_bytes)
+#        return prepend_varint(data_bytes)
 
 
 
     def _push_integer(self, integer):
         """Converts integer to bytes; as signed little-endian integer
 
         Currently supports only positive integers
         """
 
         if integer < 0:
             raise ValueError('Integer is currently required to be positive.')
 
-        # bytes requires to represent the integer
+        # bytes required to represent the integer
         number_of_bytes = (integer.bit_length() + 7) // 8
 
         # convert to little-endian bytes
         integer_bytes = integer.to_bytes(number_of_bytes, byteorder='little')
 
         # if last bit is set then we need to add sign to signify positive
         # integer
         if integer & (1 << number_of_bytes*8 - 1):
             integer_bytes += b'\x00'
 
         return self._op_push_data( hexlify(integer_bytes) )
 
 
-    def to_bytes(self, segwit = False):
+    def to_bytes(self):
         """Converts the script to bytes
 
         If an OP code the appropriate byte is included according to:
         https://en.bitcoin.it/wiki/Script
         If not consider it data (signature, public key, public key hash, etc.) and
         and include with appropriate OP_PUSHDATA OP code plus length
         """
@@ -365,22 +371,24 @@
             elif type(token) is int and token >= 0 and token <= 16:
                 script_bytes += OP_CODES['OP_' + str(token)]
             # it is data, so add accordingly
             else:
                 if type(token) is int:
                     script_bytes += self._push_integer(token)
                 else:
-                    if segwit:
-                        # probably add TxInputWitness which will know how to serialize
-                        script_bytes += self._segwit_op_push_data(token)
-                    else:
-                        script_bytes += self._op_push_data(token)
+                    script_bytes += self._op_push_data(token)
 
         return script_bytes
 
+
+    def to_hex(self):
+        """Converts to_bytes() to hex"""
+        return hexlify(self.to_bytes()).decode('utf-8')
+
+
     @staticmethod
     def from_raw(scriptraw, has_segwit=False):
         """
         Imports a Script commands list from raw hexadecimal data
             Attributes
             ----------
             txinputraw : string (hex)
@@ -416,14 +424,15 @@
                 data_size, size = vi_to_int(scriptraw[index:index + 9])
                 commands.append(scriptraw[index + size:index + size + data_size].hex())
                 index = index + data_size + size
 
 
         return Script(script=commands)
 
+
     def to_hex(self):
         """Converts the script to hexadecimal"""
 
         b = self.to_bytes()
         return hexlify(b).decode('utf-8')
```

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/setup.py` & `bitcoin-utils-0.6.1/bitcoinutils/setup.py`

 * *Files identical despite different names*

### Comparing `bitcoin-utils-0.5.9/bitcoinutils/transactions.py` & `bitcoin-utils-0.6.1/bitcoinutils/transactions.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 import hashlib
 import struct
 from binascii import unhexlify, hexlify
 
 from bitcoinutils.constants import DEFAULT_TX_SEQUENCE, DEFAULT_TX_LOCKTIME, \
                     DEFAULT_TX_VERSION, NEGATIVE_SATOSHI, \
                     EMPTY_TX_SEQUENCE, SIGHASH_ALL, SIGHASH_NONE, \
-                    SIGHASH_SINGLE, SIGHASH_ANYONECANPAY, \
+                    SIGHASH_SINGLE, SIGHASH_ANYONECANPAY, TAPROOT_SIGHASH_ALL, \
                     ABSOLUTE_TIMELOCK_SEQUENCE, REPLACE_BY_FEE_SEQUENCE, \
                     TYPE_ABSOLUTE_TIMELOCK, TYPE_RELATIVE_TIMELOCK, \
                     TYPE_REPLACE_BY_FEE, SATOSHIS_PER_BITCOIN
 from bitcoinutils.script import Script
-from bitcoinutils.utils import to_bytes, vi_to_int, encode_varint
+from bitcoinutils.utils import to_bytes, vi_to_int, encode_varint, \
+        tagged_hash, prepend_varint
 
 class TxInput:
     """Represents a transaction input.
 
     A transaction input requires a transaction id of a UTXO and the index of
     that UTXO.
 
@@ -34,22 +35,22 @@
     ----------
     txid : str
         the transaction id as a hex string (little-endian as displayed by
         tools)
     txout_index : int
         the index of the UTXO that we want to spend
     script_sig : list (strings)
-        the op code and data of the script as string
+        the script that satisfies the locking conditions (aka unlocking script)
     sequence : bytes
         the input sequence (for timelocks, RBF, etc.)
 
     Methods
     -------
-    stream()
-        converts TxInput to bytes
+    to_bytes()
+        serializes TxInput to bytes
     copy()
         creates a copy of the object (classmethod)
     """
 
     def __init__(self, txid, txout_index, script_sig=Script([]), sequence=DEFAULT_TX_SEQUENCE):
         """See TxInput description"""
 
@@ -61,16 +62,16 @@
         # if user provided a sequence it would be as string (for now...)
         if type(sequence) is str:
             self.sequence = unhexlify(sequence)
         else:
             self.sequence = sequence
 
 
-    def stream(self):
-        """Converts to bytes"""
+    def to_bytes(self):
+        """Serializes to bytes"""
 
         # Internally Bitcoin uses little-endian byte order as it improves
         # speed. Hashes are defined and implemented as big-endian thus
         # those are transmitted in big-endian order. However, when hashes are
         # displayed Bitcoin uses little-endian order because it is sometimes
         # convenient to consider hashes as little-endian integers (and not
         # strings)
@@ -138,29 +139,77 @@
     def copy(cls, txin):
         """Deep copy of TxInput"""
 
         return cls(txin.txid, txin.txout_index, txin.script_sig,
                        txin.sequence)
 
 
+class TxWitnessInput:
+    """A list of the witness items required to satisfy the locking conditions
+       of a segwit input (aka witness stack).
+
+    Attributes
+    ----------
+    stack : list
+        the witness items (hex str) list 
+
+    Methods
+    -------
+    to_bytes()
+        returns a serialized byte version of the witness items list
+    copy()
+        creates a copy of the object (classmethod)
+    """
+
+    def __init__(self, stack):
+        """See description"""
+
+        self.stack = stack
+
+    def to_bytes(self):
+        """Converts to bytes"""
+        stack_bytes = b''
+        for item in self.stack:
+            # witness items can only be data items (hex str)
+            item_bytes = prepend_varint( unhexlify(item) )
+            stack_bytes += item_bytes
+
+        return stack_bytes
+
+    @classmethod
+    def copy(cls, txwin):
+        """Deep copy of TxWitnessInput"""
+
+        return cls(txwin.stack)
+
+
+    def __str__(self):
+        return str({
+            "witness_items": self.stack,
+        })
+
+    def __repr__(self):
+        return self.__str__()
+
+
 
 class TxOutput:
     """Represents a transaction output
 
     Attributes
     ----------
     amount : int/float/Decimal
         the value we want to send to this output in satoshis
     script_pubkey : list (string)
         the script that will lock this amount
 
     Methods
     -------
-    stream()
-        converts TxInput to bytes
+    to_bytes()
+        serializes TxInput to bytes
     copy()
         creates a copy of the object (classmethod)
     """
 
 
     def __init__(self, amount, script_pubkey):
         """See TxOutput description"""
@@ -168,16 +217,16 @@
         if not isinstance(amount, int):
             raise TypeError("Amount needs to be in satoshis as an integer")
 
         self.amount = amount
         self.script_pubkey = script_pubkey
 
 
-    def stream(self):
-        """Converts to bytes"""
+    def to_bytes(self):
+        """Serializes to bytes"""
 
         # internally all little-endian except hashes
         # note struct uses little-endian by default
 
         amount_bytes = struct.pack('<q', self.amount)
         script_bytes = self.script_pubkey.to_bytes()
         data = amount_bytes + encode_varint(len(script_bytes)) + script_bytes
@@ -345,24 +394,28 @@
         A list of all the transaction outputs
     locktime : bytes
         The transaction's locktime parameter
     version : bytes
         The transaction version
     has_segwit : bool
         Specifies a tx that includes segwit inputs
-    witnesses : list (Script)
-        The witness scripts that correspond to the inputs
+    witnesses : list (TxWitnessInput)
+        The witness structure that corresponds to the inputs
 
 
     Methods
     -------
-    stream()
-        Converts Transaction to bytes
+    to_bytes()
+        Serializes Transaction to bytes
+    to_hex()
+        converts result of to_bytes to hexadecimal string
     serialize()
-        Converts Transaction to hex string
+        converts result of to_bytes to hexadecimal string
+    from_raw()
+        Instantiates a Transaction from serialized raw hexadacimal data (classmethod)
     get_txid()
         Calculates txid and returns it
     get_hash()
         Calculates tx hash (wtxid) and returns it
     get_wtxid()
         Calculates tx hash (wtxid) and returns it
     get_size()
@@ -428,15 +481,15 @@
         if rawtx[4:5] == b'\0':
             flag = rawtx[5:6]
             if flag == b'\1':
                 has_segwit = True
             cursor += 2
 
         # read the size (bytes length) of the integer representing the size of the inputs
-        # number and the the inputs number
+        # number and the inputs number
 
         n_inputs, size = vi_to_int(rawtx[cursor:cursor + 9])
         cursor += size
         inputs = []
 
         #iterate n_inputs times to read the inputs from raw
         for index in range(0,n_inputs):
@@ -447,15 +500,15 @@
         # read the size (bytes length) of the integer representing the size of the outputs
         # number and the the outputs number
         n_outputs, size = vi_to_int(rawtx[cursor:cursor + 9])
         cursor += size
         output_total = 0
 
         # iterate n_outputs times to read the inputs from raw
-        for index in range(0,n_outputs):
+        for index in range(0, n_outputs):
             output, cursor = TxOutput.from_raw(rawtx, cursor=cursor, has_segwit=has_segwit)
             outputs.append(output)
 
         witnesses = []
         if has_segwit == True:
             # iterate to read the witnesses for every input
             for n in range(0, len(inputs)):
@@ -465,15 +518,15 @@
                 for m in range(0, n_items):
                     witness = b'\0'
                     item_size, size = vi_to_int(rawtx[cursor:cursor + 9])
                     if item_size:
                         witness = rawtx[cursor + size:cursor + item_size + size]
                     cursor += item_size + size
                     witnesses_tmp.append(witness.hex())
-                witnesses.append(Script(script=witnesses_tmp))
+                witnesses.append(TxWitnessInput(stack=witnesses_tmp))
 
         return Transaction(inputs = inputs,
                            outputs = outputs,
                            has_segwit = has_segwit,
                            witnesses = witnesses)
 
 
@@ -494,20 +547,21 @@
 
     @classmethod
     def copy(cls, tx):
         """Deep copy of Transaction"""
 
         ins = [TxInput.copy(txin) for txin in tx.inputs]
         outs = [TxOutput.copy(txout) for txout in tx.outputs]
-        wits = [Script.copy(witness) for witness in tx.witnesses]
+        wits = [TxWitnessInput.copy(witness) for witness in tx.witnesses]
         return cls(ins, outs, tx.locktime, tx.version, tx.has_segwit, wits)
 
 
     def get_transaction_digest(self, txin_index, script, sighash=SIGHASH_ALL):
         """Returns the transaction's digest for signing.
+        https://en.bitcoin.it/wiki/OP_CHECKSIG
 
         |  SIGHASH types (see constants.py):
         |      SIGHASH_ALL - signs all inputs and outputs (default)
         |      SIGHASH_NONE - signs all of the inputs
         |      SIGHASH_SINGLE - signs all inputs but only txin_index output
         |      SIGHASH_ANYONECANPAY (only combined with one of the above)
         |      - with ALL - signs all outputs but only txin_index input
@@ -582,16 +636,16 @@
 
         # bitwise AND'ing 0x8n to 0x80 will result to true
         if sighash & SIGHASH_ANYONECANPAY:
             # ignore all other inputs from the signature which means that
             # anyone can add new inputs
             tmp_tx.inputs = [tmp_tx.inputs[txin_index]]
 
-        # get the byte stream of the temporary transaction
-        tx_for_signing = tmp_tx.stream(False)
+        # get the bytes of the temporary transaction
+        tx_for_signing = tmp_tx.to_bytes(False)
 
         # add sighash bytes to be hashed
         # Note that although sighash is one byte it is hashed as a 4 byte value.
         # There is no real reason for this other than that the original implementation
         # of Bitcoin stored sighash as an integer (which serializes as a 4
         # bytes), i.e. it should be converted to one byte before serialization.
         # It is converted to 1 byte before serializing to send to the network
@@ -600,15 +654,16 @@
         # create transaction digest -- note double hashing
         tx_digest = hashlib.sha256( hashlib.sha256(tx_for_signing).digest()).digest()
 
         return tx_digest
 
 
     def get_transaction_segwit_digest(self, txin_index, script, amount, sighash=SIGHASH_ALL):
-        """Returns the segwit transaction's digest for signing.
+        """Returns the segwit v0 transaction's digest for signing.
+           https://github.com/bitcoin/bips/blob/master/bip-0143.mediawiki
 
                 |  SIGHASH types (see constants.py):
                 |      SIGHASH_ALL - signs all inputs and outputs (default)
                 |      SIGHASH_NONE - signs all of the inputs
                 |      SIGHASH_SINGLE - signs all inputs but only txin_index output
                 |      SIGHASH_ANYONECANPAY (only combined with one of the above)
                 |      - with ALL - signs all outputs but only txin_index input
@@ -616,40 +671,42 @@
                 |      - with SINGLE - signs txin_index input and output
 
                 Attributes
                 ----------
                 txin_index : int
                     The index of the input that we wish to sign
                 script : list (string)
-                    The scriptPubKey of the UTXO that we want to spend
+                    The scriptCode (template) that corresponds to the segwit
+                    transaction output type that we want to spend
                 amount : int/float/Decimal
                     The amount of the UTXO to spend is included in the
                     signature for segwit (in satoshis)
                 sighash : int
                     The type of the signature hash to be created
-                """
+        """
 
         # clone transaction to modify without messing up the real transaction
+        # TODO tmp_tx is not really used for its to_bytes() - we can access self directly
         tmp_tx = Transaction.copy(self)
 
-        # TODO consult ref. impl. in BIP-143 and update if needed
-        # requires cleanup and further explanations
+        # defaults for BIP143
         hash_prevouts = b'\x00' * 32
         hash_sequence = b'\x00' * 32
         hash_outputs = b'\x00' * 32
 
-        # Judging the signature type
+        # acquiring the signature type
         basic_sig_hash_type = (sighash & 0x1f)
-        anyone_can_pay = sighash& 0xf0 == SIGHASH_ANYONECANPAY
+        anyone_can_pay = sighash & 0xf0 == SIGHASH_ANYONECANPAY
         sign_all = (basic_sig_hash_type != SIGHASH_SINGLE) and (basic_sig_hash_type != SIGHASH_NONE)
 
         # Hash all input
         if not anyone_can_pay:
             hash_prevouts = b''
             for txin in tmp_tx.inputs:
+                # TODO ? <L is 8 bytes, should be 4 bytes <I instead
                 hash_prevouts += unhexlify(txin.txid)[::-1] + \
                                     struct.pack('<L', txin.txout_index)
             hash_prevouts = hashlib.sha256(hashlib.sha256(hash_prevouts).digest()).digest()
 
         # Hash all input sequence
         if not anyone_can_pay and sign_all:
             hash_sequence = b''
@@ -669,26 +726,27 @@
             # Hash one output
             txout = tmp_tx.outputs[txin_index]
             amount_bytes = struct.pack('<q', txout.amount)
             script_bytes = txout.script_pubkey.to_bytes()
             hash_outputs = amount_bytes + struct.pack('B', len(script_bytes)) + script_bytes
             hash_outputs = hashlib.sha256(hashlib.sha256(hash_outputs).digest()).digest()
 
-        # add sighash bytes to be hashed
+        # add sighash version
         tx_for_signing = self.version
 
-        # add sighash bytes to be hashed
+        # add hash_prevouts and hash_sequence
         tx_for_signing += hash_prevouts + hash_sequence
 
-        # add tx txin
+        # add tx outpoint (utxo txid + index)
+        # TODO <L is 8 bytes, should be 4 bytes <I instead
         txin = self.inputs[txin_index]
         tx_for_signing += unhexlify(txin.txid)[::-1] + \
                           struct.pack('<L', txin.txout_index)
 
-        # add tx sign
+        # add tx script code
         tx_for_signing += struct.pack('B', len(script.to_bytes()))
         tx_for_signing += script.to_bytes()
 
         # add txin amount
         tx_for_signing += struct.pack('<q', amount)
 
         # add tx sequence
@@ -702,70 +760,220 @@
 
         # add sighash type
         tx_for_signing += struct.pack('<i', sighash)
 
         return hashlib.sha256(hashlib.sha256(tx_for_signing).digest()).digest()
 
 
-    def stream(self, has_segwit):
-        """Converts to bytes"""
+
+    # TODO Update doc with TAPROOT_SIGHASH_ALL
+    # clean prints after finishing other sighashes
+    def get_transaction_taproot_digest(self, txin_index, script_pubkeys, amounts, ext_flag=0, sighash=TAPROOT_SIGHASH_ALL):
+        """Returns the segwit v1 (taproot) transaction's digest for signing.
+           https://github.com/bitcoin/bips/blob/master/bip-0341.mediawiki
+           Also consult Bitcoin Core code at: https://github.com/bitcoin/bitcoin/blob/29c36f070618ea5148cd4b2da3732ee4d37af66b/src/script/interpreter.cpp#L1478
+           And: https://github.com/bitcoinops/taproot-workshop/blob/1d90851b8301fa4ac7469b9027f5ab543a67f269/test_framework/script.py#L730   (note, fields' order is old/wrong in this one)
+
+                |  SIGHASH types (see constants.py):
+                |      SIGHASH_ALL - signs all inputs and outputs (default)
+                |      SIGHASH_NONE - signs all of the inputs
+                |      SIGHASH_SINGLE - signs all inputs but only txin_index output
+                |      SIGHASH_ANYONECANPAY (only combined with one of the above)
+                |      - with ALL - signs all outputs but only txin_index input
+                |      - with NONE - signs only the txin_index input
+                |      - with SINGLE - signs txin_index input and output
+
+                Attributes
+                ----------
+                txin_index : int
+                    The index of the input that we wish to sign
+                script : list (string)
+                    The scriptCode (template) that corresponds to the segwit
+                    transaction output type that we want to spend
+                amount : int/float/Decimal
+                    The amount of the UTXO to spend is included in the
+                    signature for segwit (in satoshis)
+                ext_flag : int
+                    Extension mechanism, default is 0; 1 is for BIP342
+                sighash : int
+                    The type of the signature hash to be created
+        """
+
+        # clone transaction to modify without messing up the real transaction
+        # tmp_tx is not really used for its to_bytes() here
+        # TODO we could use self directly to access fields
+        tmp_tx = Transaction.copy(self)
+
+        # acquiring the signature type
+        #sign_all = sig_hash & 0x03 == SIGHASH_ALL
+        sighash_none = sighash & 0x03 == SIGHASH_NONE
+        sighash_single = sighash & 0x03 == SIGHASH_SINGLE
+        anyone_can_pay = sighash & 0x80 == SIGHASH_ANYONECANPAY
+
+        # add epoch
+        tx_for_signing = bytes([0])
+        
+        # add sighash type
+        tx_for_signing += bytes([sighash])
+
+        # add sighash version 
+        tx_for_signing += self.version
+
+        # add locktime
+        tx_for_signing += self.locktime
+
+        # defaults
+        hash_prevouts = b''
+        hash_amounts = b''
+        hash_script_pubkeys = b''
+        hash_sequences = b''
+        hash_outputs = b''
+
+
+        # Data about the transaction
+        if not anyone_can_pay:
+            #print('1')
+            # the SHA256 of the serialization of all input outpoints
+            for txin in tmp_tx.inputs:
+                hash_prevouts += unhexlify(txin.txid)[::-1] + \
+                                 struct.pack('<I', txin.txout_index)
+            hash_prevouts = hashlib.sha256(hash_prevouts).digest()
+            tx_for_signing += hash_prevouts
+
+            # the SHA256 of the serialization of all input amounts
+            for a in amounts:
+                hash_amounts += a.to_bytes(8, 'little')
+            hash_amounts = hashlib.sha256(hash_amounts).digest()
+            tx_for_signing += hash_amounts
+
+            # the SHA256 of all spent outputs' scriptPubKeys
+            for s in script_pubkeys:
+                s = s.to_hex()
+                script_len = int( len(s) / 2 )
+                hash_script_pubkeys += bytes([script_len]) + unhexlify(s)
+            hash_script_pubkeys = hashlib.sha256(hash_script_pubkeys).digest()
+            tx_for_signing += hash_script_pubkeys
+
+            # the SHA256 of the serialization of all input nSequence
+            for txin in tmp_tx.inputs:
+                hash_sequences += txin.sequence
+            hash_sequences = hashlib.sha256(hash_sequences).digest()
+            tx_for_signing += hash_sequences
+
+
+        if not (sighash_none or sighash_single):
+            #print('2')
+            for txout in tmp_tx.outputs:
+                amount_bytes = struct.pack('<Q', txout.amount)
+                script_bytes = txout.script_pubkey.to_bytes()
+                hash_outputs += amount_bytes + \
+                                struct.pack('B', len(script_bytes)) + \
+                                script_bytes
+            hash_outputs = hashlib.sha256(hash_outputs).digest()
+            tx_for_signing += hash_outputs
+
+
+        # Data about this input
+        spend_type = ext_flag * 2 + 0      # hard-coded annex_present
+        tx_for_signing += bytes([spend_type])
+
+        if anyone_can_pay:
+            #print('3')
+            txin = tmp_tx.inputs[txin_index]
+            # convert txid to big-endian first
+            tx_for_signing += unhexlify(txin.txid)[::-1] + \
+                              struct.pack('<I', txin.txout_index)
+
+            tx_for_signing += amounts[txin_index].to_bytes(8, 'little')
+
+            script_pubkey = script_pubkeys[txin_index].to_hex()
+            script_len = int( len(script_pubkey) / 2 )
+            tx_for_signing += bytes([script_len]) + unhexlify(script_pubkey)
+
+            tx_for_signing += txin.sequence
+        else:
+            #print('4')
+            tx_for_signing += txin_index.to_bytes(4, 'little')
+
+        # TODO if annex is present it should be added here
+
+        # Data about this output
+        if sighash_single:
+            #print('5')
+            txout = tmp_tx.outputs[txin_index]
+            amount_bytes = struct.pack('<Q', txout.amount)
+            script_bytes = txout.script_pubkey.to_bytes()
+            hash_output = amount_bytes + struct.pack('B', len(script_bytes)) + \
+                              script_bytes
+            tx_for_signing += hashlib.sha256(hash_output).digest()
+
+        # tagged hash the digest and return
+        return tagged_hash(tx_for_signing, "TapSighash").digest()
+
+
+
+    def to_bytes(self, has_segwit):
+        """Serializes to bytes"""
 
         data = self.version
-        if has_segwit and self.witnesses:
+        # we just check the flag and not actual witnesses so that
+        # the unsigned transactions also have the segwit marker/flag
+        # TODO make sure that this does not cause problems and delete comment
+        if has_segwit:   # and self.witnesses:
             # marker
             data += b'\x00'
             # flag
             data += b'\x01'
 
         txin_count_bytes = encode_varint(len(self.inputs))
         txout_count_bytes = encode_varint(len(self.outputs))
         data += txin_count_bytes
         for txin in self.inputs:
-            data += txin.stream()
+            data += txin.to_bytes()
         data += txout_count_bytes
         for txout in self.outputs:
-            data += txout.stream()
+            data += txout.to_bytes()
         if has_segwit:
             for witness in self.witnesses:
                 # add witnesses script Count
-                witnesses_count_bytes = chr(len(witness.script)).encode()
+                witnesses_count_bytes = chr(len(witness.stack)).encode()
                 data += witnesses_count_bytes
-                data += witness.to_bytes(True)
+                data += witness.to_bytes()
         data += self.locktime
         return data
 
 
     def get_txid(self):
         """Hashes the serialized (bytes) tx to get a unique id"""
 
-        data = self.stream(False)
+        data = self.to_bytes(False)
         hash = hashlib.sha256( hashlib.sha256(data).digest() ).digest()
         # note that we reverse the hash for display purposes
         return hexlify(hash[::-1]).decode('utf-8')
 
 
     def get_wtxid(self):
         """Hashes the serialized (bytes) tx including segwit marker and witnesses"""
 
-        return get_hash()
+        return self.get_hash()
 
 
     def get_hash(self):
         """Hashes the serialized (bytes) tx including segwit marker and witnesses"""
 
-        data = self.stream(self.has_segwit)
+        data = self.to_bytes(self.has_segwit)
         hash = hashlib.sha256( hashlib.sha256(data).digest() ).digest()
         # note that we reverse the hash for display purposes
         return hexlify(hash[::-1]).decode('utf-8')
 
 
     def get_size(self):
         """Gets the size of the transaction"""
 
-        return len(self.stream(self.has_segwit))
+        return len(self.to_bytes(self.has_segwit))
 
 
     def get_vsize(self):
         """Gets the virtual size of the transaction.
 
         For non-segwit txs this is identical to get_size(). For segwit txs the
         marker and witnesses length needs to be reduced to 1/4 of its original
@@ -781,32 +989,36 @@
         marker_size = 2
 
         wit_size = 0
         data = b''
 
         # count witnesses data
         for witness in self.witnesses:
-            # add witnesses script Count
-            witnesses_count_bytes = chr(len(witness.script)).encode()
-            data = witnesses_count_bytes
-            data += witness.to_bytes(True)
+            # add witnesses stack count
+            witnesses_count_bytes = chr(len(witness.stack)).encode()
+            data += witnesses_count_bytes
+            data += witness.to_bytes()
         wit_size = len(data)
-        # TODO when TxInputWitness is created it will contain it's own len or
-        # size method
 
         size = self.get_size() - (marker_size + wit_size)
         vsize = size + (marker_size + wit_size) / 4
 
         return int( math.ceil(vsize) )
 
 
+    def to_hex(self):
+        """Converts object to hexadecimal string"""
+
+        return hexlify(self.to_bytes(self.has_segwit)).decode('utf-8')
+
+
     def serialize(self):
-        """Converts to hex string"""
+        """Converts object to hexadecimal string"""
 
-        return hexlify(self.stream(self.has_segwit)).decode('utf-8')
+        return self.to_hex()
 
 
 def main():
     pass
 
 if __name__ == "__main__":
     main()
```

### Comparing `bitcoin-utils-0.5.9/setup.py` & `bitcoin-utils-0.6.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,16 @@
       url='https://github.com/karask/python-bitcoin-utils',
       license='MIT',
       keywords='bitcoin library utilities tools',
       install_requires=[
           'base58check>=1.0.2,<2.0',
           'ecdsa==0.17.0',
           'sympy>=1.2,<2.0',
-          'python-bitcoinrpc>=1.0,<2.0'
+          'python-bitcoinrpc>=1.0,<2.0',
+          'hdwallet==2.2.1'
       ],
       packages=['bitcoinutils'],
       #package_data={
       #    'bitcoinutils': ['requirements.txt']
       #},
       #include_package_data=True,
       zip_safe=False
```

