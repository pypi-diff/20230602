# Comparing `tmp/x21e8-0.7.0.tar.gz` & `tmp/x21e8-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x21e8-0.7.0.tar", max compression
+gzip compressed data, was "x21e8-0.7.1.tar", max compression
```

## Comparing `x21e8-0.7.0.tar` & `x21e8-0.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     5030 2023-05-19 22:45:24.773321 x21e8-0.7.0/README.md
--rw-r--r--   0        0        0      717 2023-05-19 22:45:24.777322 x21e8-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/__init__.py
--rw-r--r--   0        0        0     6082 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/liquid.py
--rw-r--r--   0        0        0        1 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/notarize.py
--rw-r--r--   0        0        0     2409 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/planetmint.py
--rw-r--r--   0        0        0      398 2023-05-19 22:45:24.777322 x21e8-0.7.0/x21e8/application/rddl.py
--rw-r--r--   0        0        0     1743 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/application/token.py
--rw-r--r--   0        0        0      765 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/config.py
--rw-r--r--   0        0        0     1001 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/main.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/__init__.py
--rw-r--r--   0        0        0      182 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/issuing_request.py
--rw-r--r--   0        0        0      188 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/nft_asset.py
--rw-r--r--   0        0        0      354 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/token_related_accounts.py
--rw-r--r--   0        0        0      494 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/models/transfer.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/__init__.py
--rw-r--r--   0        0        0     2220 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/liquid/__init__.py
--rwxr-xr-x   0        0        0    97346 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/network/liquid/util.py
--rw-r--r--   0        0        0     1693 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/assets.py
--rw-r--r--   0        0        0      375 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/config.py
--rw-r--r--   0        0        0     1096 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/data.py
--rw-r--r--   0        0        0     3892 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/machine.py
--rw-r--r--   0        0        0      925 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/seed.py
--rw-r--r--   0        0        0      630 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/utils.py
--rw-r--r--   0        0        0      619 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/routers/wallet.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/__init__.py
--rw-r--r--   0        0        0      256 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/cointype.py
--rw-r--r--   0        0        0     1035 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/encryption.py
--rw-r--r--   0        0        0     2237 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/utils/storage.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/__init__.py
--rw-r--r--   0        0        0      628 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/base_wallet.py
--rw-r--r--   0        0        0        0 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/__init__.py
--rw-r--r--   0        0        0     2771 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/keymanagement.py
--rw-r--r--   0        0        0     3231 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/planetmint/keystore.py
--rw-r--r--   0        0        0      720 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/seed.py
--rw-r--r--   0        0        0     4367 2023-05-19 22:45:24.781322 x21e8-0.7.0/x21e8/wallet/sw_wallet.py
--rw-r--r--   0        0        0     6001 1970-01-01 00:00:00.000000 x21e8-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5126 2023-06-02 15:02:32.985456 x21e8-0.7.1/README.md
+-rw-r--r--   0        0        0      794 2023-06-02 15:02:32.989456 x21e8-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/__init__.py
+-rw-r--r--   0        0        0     6082 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/liquid.py
+-rw-r--r--   0        0        0        1 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/notarize.py
+-rw-r--r--   0        0        0     2409 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/planetmint.py
+-rw-r--r--   0        0        0      398 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/rddl.py
+-rw-r--r--   0        0        0     1743 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/application/token.py
+-rw-r--r--   0        0        0      765 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/config.py
+-rw-r--r--   0        0        0     1001 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/main.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/__init__.py
+-rw-r--r--   0        0        0      182 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/issuing_request.py
+-rw-r--r--   0        0        0      188 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/nft_asset.py
+-rw-r--r--   0        0        0      354 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/token_related_accounts.py
+-rw-r--r--   0        0        0      494 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/models/transfer.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/__init__.py
+-rw-r--r--   0        0        0     2220 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/liquid/__init__.py
+-rwxr-xr-x   0        0        0    97346 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/network/liquid/util.py
+-rw-r--r--   0        0        0     1693 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/assets.py
+-rw-r--r--   0        0        0      375 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/config.py
+-rw-r--r--   0        0        0     1096 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/data.py
+-rw-r--r--   0        0        0     3885 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/machine.py
+-rw-r--r--   0        0        0      925 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/seed.py
+-rw-r--r--   0        0        0      630 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/utils.py
+-rw-r--r--   0        0        0      619 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/routers/wallet.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/cointype.py
+-rw-r--r--   0        0        0     1035 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/encryption.py
+-rw-r--r--   0        0        0     2237 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/utils/storage.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/__init__.py
+-rw-r--r--   0        0        0      628 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/base_wallet.py
+-rw-r--r--   0        0        0        0 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/planetmint/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-02 15:02:32.989456 x21e8-0.7.1/x21e8/wallet/planetmint/keymanagement.py
+-rw-r--r--   0        0        0     3231 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/planetmint/keystore.py
+-rw-r--r--   0        0        0      720 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/seed.py
+-rw-r--r--   0        0        0     4367 2023-06-02 15:02:32.993456 x21e8-0.7.1/x21e8/wallet/sw_wallet.py
+-rw-r--r--   0        0        0     6174 1970-01-01 00:00:00.000000 x21e8-0.7.1/PKG-INFO
```

### Comparing `x21e8-0.7.0/README.md` & `x21e8-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,22 +39,26 @@
 * RDDL network planetmint services (RESTFul)
 * RDDL network liquid services (RPC)
     * RPC URL
     * RPC port
     * RPC user
     * RPC password
 * web3storage token to store data
+* RDDL asset registration endpoint
+* RDDL CID resolver
 
 The configuration is set via environment variables such as
 * LQD_RPC_PORT
 * LQD_RPC_USER
 * LQD_RPC_PASSWORD
 * LQD_RPC_HOST
 * PLNTMNT_ENDPOINT
 * WEB3STORAGE_TOKEN
+* RDDL_ASSET_REG_ENDPOINT
+* CID_RESOLVER
 
 Alternatively, the variables can be defined within the ```.env``` file of the project. A example ```env.example``` file can be adjusted and copied to ```.env```.
 
 ## Service Execution
 ```bash
 uvicorn --log-level debug --reload x21e8.main:app
 ```
```

### Comparing `x21e8-0.7.0/pyproject.toml` & `x21e8-0.7.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "x21e8"
-version = "0.7.0"
-description = "x"
+version = "0.7.1"
+description = "x21e8 service to manage RDDL network identities on TrustAnchors and workflows."
 authors = ["Firat Berk Cakar <firat@riddleandcode.com>", "Jürgen Eckel <juergen@riddleandcode.com"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 TrezorCryptoTestRc = "*" 
 mnemonic = "^0.20"
```

### Comparing `x21e8-0.7.0/x21e8/application/liquid.py` & `x21e8-0.7.1/x21e8/application/liquid.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/application/planetmint.py` & `x21e8-0.7.1/x21e8/application/planetmint.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/application/token.py` & `x21e8-0.7.1/x21e8/application/token.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/config.py` & `x21e8-0.7.1/x21e8/config.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/main.py` & `x21e8-0.7.1/x21e8/main.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/network/liquid/__init__.py` & `x21e8-0.7.1/x21e8/network/liquid/__init__.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/network/liquid/util.py` & `x21e8-0.7.1/x21e8/network/liquid/util.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/routers/assets.py` & `x21e8-0.7.1/x21e8/routers/assets.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/routers/data.py` & `x21e8-0.7.1/x21e8/routers/data.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/routers/machine.py` & `x21e8-0.7.1/x21e8/routers/machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,38 +40,38 @@
         issued=issuing_request_input.amount,
         precision=issuing_request_input.precision,
         issuer_planetmint=wallet.get_planetmint_pubkey().hex(),
         issuer_liquid=wallet.get_liquid_address(),
         cid=issuing_request_input.cid,
     )
     try:
-        nft_cid = store_asset(nft_asset.__dict__)
+        nft_cid = store_asset(str(nft_asset.__dict__))
     except FileNotFoundError:
         raise HTTPException(
             status_code=421,
             detail="The hardware wallet needs to be provisioned by defining a master seed.",
         )
     try:
         token_nft = create_cid_based_asset(nft_cid, wallet)
     except PlanetmintException as e:
-        print(f"The Planetmint server configured does not support the given transaction schema. {e}")
+        print(f"The Planetmint server configured does not support the given transaction. {e}")
         raise HTTPException(
             status_code=423,
-            detail="The Planetmint server configured does not support the given transaction schema. {e}",
+            detail=f"The Planetmint server configured does not support the given transaction. {e}",
         )
 
     if check_if_tokens_should_be_issued(issuing_request_input):
         asset, asset_id, contract = LiquidNode().issue_tokens(issuing_request_input, token_nft["id"], nft_cid)
         print(f"Liquid issued token: {asset_id}  - {contract}")
         try:
             response = LiquidNode.register_asset(asset, contract, RDDL_ASSET_REG_ENDPOINT)
             print(f"RDDL asset registration: {response}")
         except Exception as e:
             print(f"Exception: RDDL asset registration - {e}")
-            raise HTTPException(status_code=425, detail="Exception: RDDL asset registration - {e}")
+            raise HTTPException(status_code=425, detail=f"Exception: RDDL asset registration - {e}")
 
     return {
         "w3storage.cid": nft_cid,
         "NFT token": token_nft["id"],
         "NFT transaction": token_nft,
     }
```

### Comparing `x21e8-0.7.0/x21e8/routers/seed.py` & `x21e8-0.7.1/x21e8/routers/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/routers/utils.py` & `x21e8-0.7.1/x21e8/routers/utils.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/routers/wallet.py` & `x21e8-0.7.1/x21e8/routers/wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/utils/encryption.py` & `x21e8-0.7.1/x21e8/utils/encryption.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/utils/storage.py` & `x21e8-0.7.1/x21e8/utils/storage.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/wallet/base_wallet.py` & `x21e8-0.7.1/x21e8/wallet/base_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/wallet/planetmint/keymanagement.py` & `x21e8-0.7.1/x21e8/wallet/planetmint/keymanagement.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/wallet/planetmint/keystore.py` & `x21e8-0.7.1/x21e8/wallet/planetmint/keystore.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/wallet/seed.py` & `x21e8-0.7.1/x21e8/wallet/seed.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/x21e8/wallet/sw_wallet.py` & `x21e8-0.7.1/x21e8/wallet/sw_wallet.py`

 * *Files identical despite different names*

### Comparing `x21e8-0.7.0/PKG-INFO` & `x21e8-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: x21e8
-Version: 0.7.0
-Summary: x
+Version: 0.7.1
+Summary: x21e8 service to manage RDDL network identities on TrustAnchors and workflows.
 Author: Firat Berk Cakar
 Author-email: firat@riddleandcode.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -66,22 +66,26 @@
 * RDDL network planetmint services (RESTFul)
 * RDDL network liquid services (RPC)
     * RPC URL
     * RPC port
     * RPC user
     * RPC password
 * web3storage token to store data
+* RDDL asset registration endpoint
+* RDDL CID resolver
 
 The configuration is set via environment variables such as
 * LQD_RPC_PORT
 * LQD_RPC_USER
 * LQD_RPC_PASSWORD
 * LQD_RPC_HOST
 * PLNTMNT_ENDPOINT
 * WEB3STORAGE_TOKEN
+* RDDL_ASSET_REG_ENDPOINT
+* CID_RESOLVER
 
 Alternatively, the variables can be defined within the ```.env``` file of the project. A example ```env.example``` file can be adjusted and copied to ```.env```.
 
 ## Service Execution
 ```bash
 uvicorn --log-level debug --reload x21e8.main:app
 ```
```

