# Comparing `tmp/dpapi-ng-0.1.1.tar.gz` & `tmp/dpapi-ng-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpapi-ng-0.1.1.tar", last modified: Tue May 16 06:10:28 2023, max compression
+gzip compressed data, was "dpapi-ng-0.2.0.tar", last modified: Fri Jun  2 01:07:51 2023, max compression
```

## Comparing `dpapi-ng-0.1.1.tar` & `dpapi-ng-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/dpapi_ng/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31807 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)    20700 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_dns.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_epm.py
--rw-r--r--   0 runner    (1001) docker     (123)    26887 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_gkdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9837 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_pkcs7.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_bind.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_pdu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_security_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/src/dpapi_ng/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.342913 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 06:10:28.000000 dpapi-ng-0.1.1/src/dpapi_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:10:28.346913 dpapi-ng-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_epm.py
--rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_gkdi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-16 06:10:20.000000 dpapi-ng-0.1.1/tests/test_security_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.696030 dpapi-ng-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-02 01:07:51.696030 dpapi-ng-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 01:07:51.696030 dpapi-ng-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.688030 dpapi-ng-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.692030 dpapi-ng-0.2.0/src/dpapi_ng/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35216 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30391 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_dns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_epm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30113 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_gkdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_pkcs7.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.696030 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_bind.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_pdu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_security_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/src/dpapi_ng/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.692030 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-02 01:07:51.000000 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-02 01:07:51.000000 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 01:07:51.000000 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 01:07:51.000000 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-02 01:07:51.000000 dpapi-ng-0.2.0/src/dpapi_ng.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 01:07:51.696030 dpapi-ng-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_epm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24346 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_gkdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-02 01:07:42.000000 dpapi-ng-0.2.0/tests/test_security_descriptor.py
```

### Comparing `dpapi-ng-0.1.1/LICENSE` & `dpapi-ng-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/PKG-INFO` & `dpapi-ng-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpapi-ng
-Version: 0.1.1
+Version: 0.2.0
 Summary: DPAPI NG decryption for Python
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,25 +36,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
 License-File: LICENSE
 
-# dpapi_ng - Python DPAPI-NG Decryption Library
+# dpapi_ng - Python DPAPI-NG De-/Encryption Library
 
 [![Test workflow](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml/badge.svg)](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jborean93/dpapi-ng/branch/main/graph/badge.svg?token=UEA7VoocS5)](https://codecov.io/gh/jborean93/dpapi-ng)
 [![PyPI version](https://badge.fury.io/py/dpapi-ng.svg)](https://badge.fury.io/py/dpapi-ng)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jborean93/dpapi-ng/blob/main/LICENSE)
 
-Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, decryption in Python.
-It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret).
-This can be used on non-Windows hosts to decrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
-It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or by using the credentials of the supplied user to retrieve the required information over RPC.
+Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, de- and encryption in Python.
+It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret) and [NCryptProtectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptprotectsecret).
+This can be used on non-Windows hosts to de-/encrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
+It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or de-/encrypt by using the credentials of the supplied user to retrieve the required information over RPC.
 
 Currently only these protection descriptors are supported:
 
 |Type|Purpose|
 |-|-|
 |SID|Only the SID user or members of the SID group can decrypt the secret|
 
@@ -108,41 +108,58 @@
 git clone https://github.com/jborean93/dpapi-ng.git
 cd dpapi-ng
 pip install -e .
 ```
 
 ## Examples
 
-There is both a sync and asyncio API available to decrypt the blob.
+There is both a sync and asyncio API available to de-/encrypt a blob.
 
 ```python
 import dpapi_ng
 
-blob_bytes = b"..."
-dpapi_ng.ncrypt_unprotect_secret(blob_bytes)
 
-# The async equivalent to the above
-await dpapi_ng.async_ncrypt_unprotect_secret(blob_bytes)
+### DECRYPTION ###
+dpapi_ng_blob = b"..."
+decrypted_blob = dpapi_ng.ncrypt_unprotect_secret(dpapi_ng_blob)
+
+# async equivalent to the above
+decrypted_blob = await dpapi_ng.async_ncrypt_unprotect_secret(dpapi_ng_blob)
+
+
+### ENCRYPTION ###
+data = b"..."
+target_sid = "S-1-5-21-XXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX-XXXX"
+dpapi_ng_blob = dpapi_ng.ncrypt_protect_secret(data, target_sid)
+
+# async equivalent to the above
+dpapi_ng_blob = await dpapi_ng.async_ncrypt_protect_secret(data, target_sid)
 ```
 
-These functions return the decrypt bytes of the DPAPI-NG blob.
 To decrypt the blob, the key specified in the blob needs to be retrieved from the domain controller the blob was generated by.
-The domain controller hostname is retrieved through an `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` or with the value specified in the `server` kwarg.
+To encrypt a blob, the group key of the target SID specified needs to be retrieved.
+For decryption, the domain controller hostname is automatically retrieved through an DNS `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` with the domain name found in the DPAPI-NG blob or with the value specified in the `server` kwarg.
+For encryption, the domain controller hostname is either determined using the `domain_name` kwarg for a DNS `SRV` lookup, the `server` kwarg directly or by using the system's search domain (if available).
 It will attempt to authenticate with the current user identifier which on Linux will only exist if `kinit` has already been called to retrieve a user's ticket.
 Otherwise if no identity is available, the `username` and `password` kwargs can be used to specify a custom user.
 
-The following kwargs can be used for both `ncrypt_unprotect_secret` and `async_ncrypt_unprotect_secret`.
+The following kwargs can be used for `ncrypt_unprotect_secret`, `async_ncrypt_unprotect_secret`, `ncrypt_protect_secret` and `async_ncrypt_protect_secret`.
 
 * `server`: Use this server as the RPC target if a key needs to be retrieved
 * `username`: The username to authenticate as for the RPC connection
 * `password`: The password to authenticate with for the RPC connection
 * `auth_protocol`: The authentication protocol (`negotiate`, `kerberos`, `ntlm`) to use for the RPC connection
 * `cache`: A cache to store keys retrieved for future operation
 
-It is also possible to decrypt the DPAPI-NG blob by providing the root key stored in the domain.
+In addition to that, `ncrypt_protect_secret` and `async_ncrypt_protect_secret` take the following additional kwarg.
+
+* `domain_name`: The name of the domain/forest to use when looking up the RPC target to use when retrieving the key info
+* `root_key_identifier`: The root key identifier UUID, necessary in order to make the cache work for these functions
+
+It is also possible to encrypt and decrypt the DPAPI-NG blob by providing the root key stored in the domain.
 This can either be retrieved using an offline attack or through an LDAP query if running as a Domain Admin user.
 To retrieve the domain root keys using PowerShell the following can be run:
 
 ```powershell
 $configurationContext = (Get-ADRootDSE).configurationNamingContext
 $getParams = @{
     LDAPFilter = '(objectClass=msKds-ProvRootKey)'
@@ -189,15 +206,15 @@
     msKds-PrivateKeyLength \
     msKds-PublicKeyLength \
     msKds-RootKeyData
 ```
 
 _Note: ldapsearch will most likely need the -H and user bind information to succeed._
 
-The information retrieved there can be stored in a cache and used for subsequent `ncrypt_unprotect_secret` calls:
+The information retrieved there can be stored in a cache and used for subsequent `ncrypt_protect_secret` and `ncrypt_unprotect_secret` calls:
 
 ```python
 import uuid
 
 import dpapi_ng
 
 cache = dpapi_ng.KeyCache()
@@ -219,15 +236,16 @@
 ```
 
 Currently the `SP800_108_CTR_HMAC` KDF algorithm and `DH`, `ECDH_P256`, and `ECDH_P384` secret agreement algorithms have been tested to work.
 The `ECDH_P521` secret agreement algorithm should also work but has been untested as a test environment cannot be created with it right now.
 
 ## Special Thanks
 
-I would like to thank the following people (Twitter handles in brackets) for their help on this project:
+I would like to thank the following people (GitHub or Twitter handles in brackets) for their help on this project:
 
+* Georg Sieber (@schorschii) for implementing encryption support
 * Grzegorz Tworek (@0gtweet) and Michał Grzegorzewski for providing more information on the internal BCrypt* API workflow used in DPAPI-NG
 * Marc-André Moreau (@awakecoding) for their help with reverse engineering some of the Windows APIs and talking through some theories
 * SkelSec (@SkelSec) for help on the RPC calls and being available as a general sounding board for my theories
 * Steve Syfuhs (@SteveSyfuhs) for connecting me with some Microsoft engineers to help understand some undocumented logic
 
 Without their patience and knowledge this probably would not have been possible.
```

### Comparing `dpapi-ng-0.1.1/README.md` & `dpapi-ng-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# dpapi_ng - Python DPAPI-NG Decryption Library
+# dpapi_ng - Python DPAPI-NG De-/Encryption Library
 
 [![Test workflow](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml/badge.svg)](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jborean93/dpapi-ng/branch/main/graph/badge.svg?token=UEA7VoocS5)](https://codecov.io/gh/jborean93/dpapi-ng)
 [![PyPI version](https://badge.fury.io/py/dpapi-ng.svg)](https://badge.fury.io/py/dpapi-ng)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jborean93/dpapi-ng/blob/main/LICENSE)
 
-Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, decryption in Python.
-It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret).
-This can be used on non-Windows hosts to decrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
-It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or by using the credentials of the supplied user to retrieve the required information over RPC.
+Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, de- and encryption in Python.
+It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret) and [NCryptProtectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptprotectsecret).
+This can be used on non-Windows hosts to de-/encrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
+It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or de-/encrypt by using the credentials of the supplied user to retrieve the required information over RPC.
 
 Currently only these protection descriptors are supported:
 
 |Type|Purpose|
 |-|-|
 |SID|Only the SID user or members of the SID group can decrypt the secret|
 
@@ -66,41 +66,58 @@
 git clone https://github.com/jborean93/dpapi-ng.git
 cd dpapi-ng
 pip install -e .
 ```
 
 ## Examples
 
-There is both a sync and asyncio API available to decrypt the blob.
+There is both a sync and asyncio API available to de-/encrypt a blob.
 
 ```python
 import dpapi_ng
 
-blob_bytes = b"..."
-dpapi_ng.ncrypt_unprotect_secret(blob_bytes)
 
-# The async equivalent to the above
-await dpapi_ng.async_ncrypt_unprotect_secret(blob_bytes)
+### DECRYPTION ###
+dpapi_ng_blob = b"..."
+decrypted_blob = dpapi_ng.ncrypt_unprotect_secret(dpapi_ng_blob)
+
+# async equivalent to the above
+decrypted_blob = await dpapi_ng.async_ncrypt_unprotect_secret(dpapi_ng_blob)
+
+
+### ENCRYPTION ###
+data = b"..."
+target_sid = "S-1-5-21-XXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX-XXXX"
+dpapi_ng_blob = dpapi_ng.ncrypt_protect_secret(data, target_sid)
+
+# async equivalent to the above
+dpapi_ng_blob = await dpapi_ng.async_ncrypt_protect_secret(data, target_sid)
 ```
 
-These functions return the decrypt bytes of the DPAPI-NG blob.
 To decrypt the blob, the key specified in the blob needs to be retrieved from the domain controller the blob was generated by.
-The domain controller hostname is retrieved through an `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` or with the value specified in the `server` kwarg.
+To encrypt a blob, the group key of the target SID specified needs to be retrieved.
+For decryption, the domain controller hostname is automatically retrieved through an DNS `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` with the domain name found in the DPAPI-NG blob or with the value specified in the `server` kwarg.
+For encryption, the domain controller hostname is either determined using the `domain_name` kwarg for a DNS `SRV` lookup, the `server` kwarg directly or by using the system's search domain (if available).
 It will attempt to authenticate with the current user identifier which on Linux will only exist if `kinit` has already been called to retrieve a user's ticket.
 Otherwise if no identity is available, the `username` and `password` kwargs can be used to specify a custom user.
 
-The following kwargs can be used for both `ncrypt_unprotect_secret` and `async_ncrypt_unprotect_secret`.
+The following kwargs can be used for `ncrypt_unprotect_secret`, `async_ncrypt_unprotect_secret`, `ncrypt_protect_secret` and `async_ncrypt_protect_secret`.
 
 * `server`: Use this server as the RPC target if a key needs to be retrieved
 * `username`: The username to authenticate as for the RPC connection
 * `password`: The password to authenticate with for the RPC connection
 * `auth_protocol`: The authentication protocol (`negotiate`, `kerberos`, `ntlm`) to use for the RPC connection
 * `cache`: A cache to store keys retrieved for future operation
 
-It is also possible to decrypt the DPAPI-NG blob by providing the root key stored in the domain.
+In addition to that, `ncrypt_protect_secret` and `async_ncrypt_protect_secret` take the following additional kwarg.
+
+* `domain_name`: The name of the domain/forest to use when looking up the RPC target to use when retrieving the key info
+* `root_key_identifier`: The root key identifier UUID, necessary in order to make the cache work for these functions
+
+It is also possible to encrypt and decrypt the DPAPI-NG blob by providing the root key stored in the domain.
 This can either be retrieved using an offline attack or through an LDAP query if running as a Domain Admin user.
 To retrieve the domain root keys using PowerShell the following can be run:
 
 ```powershell
 $configurationContext = (Get-ADRootDSE).configurationNamingContext
 $getParams = @{
     LDAPFilter = '(objectClass=msKds-ProvRootKey)'
@@ -147,15 +164,15 @@
     msKds-PrivateKeyLength \
     msKds-PublicKeyLength \
     msKds-RootKeyData
 ```
 
 _Note: ldapsearch will most likely need the -H and user bind information to succeed._
 
-The information retrieved there can be stored in a cache and used for subsequent `ncrypt_unprotect_secret` calls:
+The information retrieved there can be stored in a cache and used for subsequent `ncrypt_protect_secret` and `ncrypt_unprotect_secret` calls:
 
 ```python
 import uuid
 
 import dpapi_ng
 
 cache = dpapi_ng.KeyCache()
@@ -177,15 +194,16 @@
 ```
 
 Currently the `SP800_108_CTR_HMAC` KDF algorithm and `DH`, `ECDH_P256`, and `ECDH_P384` secret agreement algorithms have been tested to work.
 The `ECDH_P521` secret agreement algorithm should also work but has been untested as a test environment cannot be created with it right now.
 
 ## Special Thanks
 
-I would like to thank the following people (Twitter handles in brackets) for their help on this project:
+I would like to thank the following people (GitHub or Twitter handles in brackets) for their help on this project:
 
+* Georg Sieber (@schorschii) for implementing encryption support
 * Grzegorz Tworek (@0gtweet) and Michał Grzegorzewski for providing more information on the internal BCrypt* API workflow used in DPAPI-NG
 * Marc-André Moreau (@awakecoding) for their help with reverse engineering some of the Windows APIs and talking through some theories
 * SkelSec (@SkelSec) for help on the RPC calls and being available as a general sounding board for my theories
 * Steve Syfuhs (@SteveSyfuhs) for connecting me with some Microsoft engineers to help understand some undocumented logic
 
 Without their patience and knowledge this probably would not have been possible.
```

### Comparing `dpapi-ng-0.1.1/pyproject.toml` & `dpapi-ng-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_asn1.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_asn1.py`

 * *Files 8% similar despite different names*

```diff
@@ -534,25 +534,41 @@
         self._data.extend(_pack_asn1_boolean(value, tag=tag))
 
     def write_enumerated(
         self,
         value: int,
         tag: t.Optional[ASN1Tag] = None,
     ) -> None:
-        """Write an ASN.1 ENUMEATES value.
+        """Write an ASN.1 ENUMERATED value.
 
         Writes a enumerated value to the current writer.
 
         Args:
             value: The enumerated/int to write.
             tag: Optional tag to use with the value, defaults to the ENUMERATED
                 universal tag.
         """
         self._data.extend(_pack_asn1_enumerated(value, tag=tag))
 
+    def write_generalized_time(
+        self,
+        value: str,
+        tag: t.Optional[ASN1Tag] = None,
+    ) -> None:
+        """Write an ASN.1 GENERALIZED_TIME value.
+
+        Writes a generalized time string to the current writer.
+
+        Args:
+            value: The generalized time to write.
+            tag: Optional tag to use with the value, defaults to the
+                GENERALIZED_TIME universal tag.
+        """
+        self._data.extend(_pack_asn1_generalized_time(value, tag=tag))
+
     def write_integer(
         self,
         value: int,
         tag: t.Optional[ASN1Tag] = None,
     ) -> None:
         """Write an ASN.1 INTEGER value.
 
@@ -571,20 +587,59 @@
         tag: t.Optional[ASN1Tag] = None,
     ) -> None:
         """Write an ASN.1 OCTET_STRING value.
 
         Writes a bytes string value to the current writer.
 
         Args:
-            value: The bool to write.
+            value: The bytes to write.
             tag: Optional tag to use with the value, defaults to the
                 OCTET_STRING universal tag.
         """
         self._data.extend(_pack_asn1_octet_string(value, tag=tag))
 
+    def write_object_identifier(
+        self,
+        value: str,
+        tag: t.Optional[ASN1Tag] = None,
+    ) -> None:
+        """Write an ASN.1 OBJECT_IDENTIFIER value.
+
+        Writes a bytes string value to the current writer.
+
+        Args:
+            value: The object identifier (string representation) to write.
+            tag: Optional tag to use with the value, defaults to the
+                OBJECT_IDENTIFIER universal tag.
+        """
+        self._data.extend(_pack_asn1_object_identifier(value, tag=tag))
+
+    def write_utf8_string(
+        self,
+        value: str,
+        tag: t.Optional[ASN1Tag] = None,
+    ) -> None:
+        """Write an ASN.1 UTF8_STRING value.
+
+        Writes a UTF-8 string value to the current writer.
+
+        Args:
+            value: The string to write.
+            tag: Optional tag to use with the value, defaults to the
+                UTF8_STRING universal tag.
+        """
+        self._data.extend(_pack_asn1_utf8_string(value, tag=tag))
+
+    def write_raw(
+        self,
+        value: bytes,
+    ) -> None:
+        """Appends raw values onto the ASN1 writer."""
+        self._data.extend(value)
+
     def get_data(self) -> bytearray:
         """Gets the data written to the writer.
 
         This is used to get the final ASN.1 value after all the values have
         been written to it. It cannot be called on a child writer returned by
         push_sequence or push_set.
 
@@ -691,14 +746,25 @@
     value: int,
     tag: t.Optional[ASN1Tag] = None,
 ) -> bytes:
     """Packs an int into an ASN.1 ENUMERATED byte value with optional universal tagging."""
     return _pack_asn1_integer(value, tag=tag or ASN1Tag.universal_tag(TypeTagNumber.ENUMERATED))
 
 
+def _pack_asn1_generalized_time(
+    value: str,
+    tag: t.Optional[ASN1Tag] = None,
+) -> bytes:
+    """Packs an int into an ASN.1 GENERALIZED_TIME byte value with optional universal tagging."""
+    if not tag:
+        tag = ASN1Tag.universal_tag(TypeTagNumber.GENERALIZED_TIME)
+
+    return _pack_asn1(tag.tag_class, tag.is_constructed, tag.tag_number, value.encode("utf-8"))
+
+
 def _pack_asn1_integer(
     value: int,
     tag: t.Optional[ASN1Tag] = None,
 ) -> bytes:
     """Packs an int value into an ASN.1 INTEGER byte value with optional universal tagging."""
     if not tag:
         tag = ASN1Tag.universal_tag(TypeTagNumber.INTEGER)
@@ -748,14 +814,55 @@
     """Packs an bytes value into an ASN.1 OCTET STRING byte value with optional universal tagging."""
     if not tag:
         tag = ASN1Tag.universal_tag(TypeTagNumber.OCTET_STRING)
 
     return _pack_asn1(tag.tag_class, tag.is_constructed, tag.tag_number, b_data)
 
 
+def _pack_asn1_object_identifier(
+    value: str,
+    tag: t.Optional[ASN1Tag] = None,
+) -> bytes:
+    """Packs an object identifier value represented as string into an
+    ASN.1 OBJECT IDENTIFIER value with optional universal tagging."""
+    if not tag:
+        tag = ASN1Tag.universal_tag(TypeTagNumber.OBJECT_IDENTIFIER)
+
+    return _pack_asn1(tag.tag_class, tag.is_constructed, tag.tag_number, _encode_object_identifier(value))
+
+
+def _pack_asn1_utf8_string(
+    value: str,
+    tag: t.Optional[ASN1Tag] = None,
+) -> bytes:
+    """Packs an object identifier value represented as string into an
+    ASN.1 UTF8 STRING byte value with optional universal tagging."""
+    if not tag:
+        tag = ASN1Tag.universal_tag(TypeTagNumber.UTF8_STRING)
+
+    return _pack_asn1(tag.tag_class, tag.is_constructed, tag.tag_number, value.encode("utf-8"))
+
+
+def _encode_object_identifier(oid: str) -> bytes:
+    """Encode an object identifier."""
+    cmps = list(map(int, oid.split(".")))
+    if cmps[0] > 39 or cmps[1] > 39:
+        raise ValueError("Illegal object identifier")
+    cmps = [40 * cmps[0] + cmps[1]] + cmps[2:]
+    cmps.reverse()
+    result = []
+    for cmp_data in cmps:
+        result.append(cmp_data & 0x7F)
+        while cmp_data > 0x7F:
+            cmp_data >>= 7
+            result.append(0x80 | (cmp_data & 0x7F))
+    result.reverse()
+    return bytes(result)
+
+
 def _read_asn1_header(
     data: t.Union[bytes, bytearray, memoryview],
 ) -> ASN1Header:
     """Reads the ASN.1 Tag and Length octets
 
     Reads the raw ASN.1 value to retrieve the tag and length values.
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_blob.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_blob.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright: (c) 2023, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 from __future__ import annotations
 
 import dataclasses
+import enum
 import typing as t
 import uuid
 
-from ._asn1 import ASN1Reader
+from ._asn1 import ASN1Reader, ASN1Writer
 from ._pkcs7 import (
+    AlgorithmIdentifier,
     ContentInfo,
+    EncryptedContentInfo,
     EnvelopedData,
+    KEKIdentifier,
     KEKRecipientInfo,
-    NCryptProtectionDescriptor,
+    OtherKeyAttribute,
 )
 from ._security_descriptor import ace_to_bytes, sd_to_bytes
 
 
 @dataclasses.dataclass(frozen=True)
 class KeyIdentifier:
     """Key Identifier.
@@ -117,93 +121,219 @@
             root_key_identifier=root_key_identifier,
             key_info=key_info,
             domain_name=domain,
             forest_name=forest,
         )
 
 
+class ProtectionDescriptorType(enum.Enum):
+    SID = "1.3.6.1.4.1.311.74.1.1"
+    KEY_FILE = "1.3.6.1.4.1.311.74.1.2"  # KeyFile in UF8String type
+    SDDL = "1.3.6.1.4.1.311.74.1.5"
+    LOCAL = "1.3.6.1.4.1.311.74.1.8"
+
+
+@dataclasses.dataclass(frozen=True)
+class ProtectionDescriptor:
+    type: ProtectionDescriptorType
+    value: str
+
+    def get_target_sd(self) -> bytes:
+        raise NotImplementedError()  # pragma: nocover
+
+    def pack(self) -> bytes:
+        writer = ASN1Writer()
+
+        with writer.push_sequence() as w:
+            w.write_object_identifier(self.type.value)
+
+            with w.push_sequence() as w1:
+                with w1.push_sequence() as w2:
+                    with w2.push_sequence() as w3:
+                        w3.write_utf8_string(self.type.name)
+                        w3.write_utf8_string(self.value)
+
+        return writer.get_data()
+
+    @classmethod
+    def parse(
+        cls,
+        value: str,
+    ) -> ProtectionDescriptor:
+        # Currently only the SID type is supported
+        return SIDDescriptor(value)
+
+    @classmethod
+    def unpack(
+        cls,
+        data: t.Union[bytes, bytearray, memoryview],
+    ) -> ProtectionDescriptor:
+        reader = ASN1Reader(data).read_sequence()
+        content_type = reader.read_object_identifier()
+
+        reader = reader.read_sequence().read_sequence().read_sequence()
+        value_type = reader.read_utf8_string()
+        value = reader.read_utf8_string()
+
+        if content_type == ProtectionDescriptorType.SID.value and value_type == "SID":
+            return SIDDescriptor(value)
+
+        else:
+            raise ValueError(f"DPAPI-NG protection descriptor type {content_type} '{value_type}' is unsupported")
+
+
+@dataclasses.dataclass(frozen=True)
+class SIDDescriptor(ProtectionDescriptor):
+    type: ProtectionDescriptorType = dataclasses.field(init=False, default=ProtectionDescriptorType.SID)
+
+    def get_target_sd(self) -> bytes:
+        # Build the target security descriptor from the SID passed in. This SD
+        # contains an ACE per target user with a mask of 0x3 and a final ACE of
+        # the current user with a mask of 0x2. When viewing this over the wire
+        # the current user is set as S-1-1-0 (World) and the owner/group is
+        # S-1-5-18 (SYSTEM).
+        return sd_to_bytes(
+            owner="S-1-5-18",
+            group="S-1-5-18",
+            dacl=[ace_to_bytes(self.value, 3), ace_to_bytes("S-1-1-0", 2)],
+        )
+
+
 @dataclasses.dataclass
 class DPAPINGBlob:
+    MICROSOFT_SOFTWARE_OID = "1.3.6.1.4.1.311.74.1"
+
     """DPAPI NG Blob.
 
     The unpacked DPAPI NG blob that contains the information needed to decrypt
     the encrypted content. The key identifier and protection descriptor can be
     used to generate the KEK. The KEK is used to decrypt the encrypted CEK. The
     CEK can be used to decrypt the encrypted contents.
 
     Args:
         key_identifier: The key identifier for the KEK.
-        security_descriptor: The Security Descriptor that protects the key.
+        protection_descriptor: The protection descriptor that protects the key.
         enc_cek: The encrypted CEK.
         enc_cek_algorithm: The encrypted CEK algorithm OID.
         enc_cek_parameters: The encrypted CEK algorithm parameters.
         enc_content: The encrypted content.
         enc_content_algorithm: The encrypted content algorithm OID.
         enc_content_parameters: The encrypted content parameters.
     """
 
     key_identifier: KeyIdentifier
-    security_descriptor: bytes
+    protection_descriptor: ProtectionDescriptor
     enc_cek: bytes
     enc_cek_algorithm: str
     enc_cek_parameters: t.Optional[bytes]
     enc_content: bytes
     enc_content_algorithm: str
     enc_content_parameters: t.Optional[bytes]
 
+    def pack(
+        self,
+        blob_in_envelope: bool = True,
+    ) -> bytes:
+        """Pack the DPAPI-NG Blob
+
+        Packs the DPAPI-NG blob into a byte string.
+
+        Args:
+            blob_in_envelope: True to store the encrypted blob in the
+                EnvelopedData structure (NCryptProtectSecret general), False to
+                append the encrypted blob after the EnvelopedData structure
+                (LAPS style).
+
+        Returns:
+            bytes: The DPAPI NG Blob data.
+        """
+        writer = ASN1Writer()
+
+        recipient_info = KEKRecipientInfo(
+            version=4,
+            kekid=KEKIdentifier(
+                key_identifier=self.key_identifier.pack(),
+                other=OtherKeyAttribute(
+                    key_attr_id=DPAPINGBlob.MICROSOFT_SOFTWARE_OID,
+                    key_attr=self.protection_descriptor.pack(),
+                ),
+            ),
+            key_encryption_algorithm=AlgorithmIdentifier(
+                self.enc_cek_algorithm,
+                self.enc_cek_parameters,
+            ),
+            encrypted_key=self.enc_cek,
+        )
+
+        enveloped_data = EnvelopedData(
+            version=2,
+            recipient_infos=[recipient_info],
+            encrypted_content_info=EncryptedContentInfo(
+                content_type=EnvelopedData.CONTENT_TYPE_DATA_OID,
+                algorithm=AlgorithmIdentifier(
+                    algorithm=self.enc_content_algorithm,
+                    parameters=self.enc_content_parameters,
+                ),
+                content=self.enc_content if blob_in_envelope else b"",
+            ),
+        )
+        writer = ASN1Writer()
+        enveloped_data.pack(writer)
+
+        content_info = ContentInfo(
+            content_type=EnvelopedData.CONTENT_TYPE_ENVELOPED_DATA_OID,
+            content=writer.get_data(),
+        )
+        writer = ASN1Writer()
+        content_info.pack(writer)
+
+        return b"".join(
+            [
+                writer.get_data(),
+                b"" if blob_in_envelope else self.enc_content,
+            ]
+        )
+
     @classmethod
     def unpack(
         cls,
         data: t.Union[bytes, bytearray, memoryview],
     ) -> DPAPINGBlob:
         view = memoryview(data)
         header = ASN1Reader(view).peek_header()
         content_info = ContentInfo.unpack(view[: header.tag_length + header.length], header=header)
         remaining_data = view[header.tag_length + header.length :]
 
-        if content_info.content_type != EnvelopedData.content_type:
+        if content_info.content_type != EnvelopedData.CONTENT_TYPE_ENVELOPED_DATA_OID:
             raise ValueError(f"DPAPI-NG blob content type '{content_info.content_type}' is unsupported")
         enveloped_data = EnvelopedData.unpack(content_info.content)
 
         if (
             enveloped_data.version != 2
             or len(enveloped_data.recipient_infos) != 1
             or not isinstance(enveloped_data.recipient_infos[0], KEKRecipientInfo)
             or enveloped_data.recipient_infos[0].version != 4
         ):
             raise ValueError(f"DPAPI-NG blob is not in the expected format")
 
         kek_info = enveloped_data.recipient_infos[0]
         key_identifier = KeyIdentifier.unpack(kek_info.kekid.key_identifier)
 
-        if not kek_info.kekid.other or kek_info.kekid.other.key_attr_id != "1.3.6.1.4.1.311.74.1":
+        if not kek_info.kekid.other or kek_info.kekid.other.key_attr_id != DPAPINGBlob.MICROSOFT_SOFTWARE_OID:
             raise ValueError("DPAPI-NG KEK Id is not in the expected format")
 
-        protection_descriptor = NCryptProtectionDescriptor.unpack(kek_info.kekid.other.key_attr or b"")
-        if protection_descriptor.content_type != "1.3.6.1.4.1.311.74.1.1" or protection_descriptor.type != "SID":
-            raise ValueError(f"DPAPI-NG protection descriptor type '{protection_descriptor.type}' is unsupported")
-
-        # Build the target security descriptor from the SID passed in. This SD
-        # contains an ACE per target user with a mask of 0x3 and a final ACE of
-        # the current user with a mask of 0x2. When viewing this over the wire
-        # the current user is set as S-1-1-0 (World) and the owner/group is
-        # S-1-5-18 (SYSTEM).
-        target_sd = sd_to_bytes(
-            owner="S-1-5-18",
-            group="S-1-5-18",
-            dacl=[ace_to_bytes(protection_descriptor.value, 3), ace_to_bytes("S-1-1-0", 2)],
-        )
+        protection_descriptor = ProtectionDescriptor.unpack(kek_info.kekid.other.key_attr or b"")
 
         # Some DPAPI blobs don't include the content in the PKCS7 payload but
         # just append after the blob.
         enc_content = enveloped_data.encrypted_content_info.content or remaining_data.tobytes()
 
         return DPAPINGBlob(
             key_identifier=key_identifier,
-            security_descriptor=target_sd,
+            protection_descriptor=protection_descriptor,
             enc_cek=kek_info.encrypted_key,
             enc_cek_algorithm=kek_info.key_encryption_algorithm.algorithm,
             enc_cek_parameters=kek_info.key_encryption_algorithm.parameters,
             enc_content=enc_content,
             enc_content_algorithm=enveloped_data.encrypted_content_info.algorithm.algorithm,
             enc_content_parameters=enveloped_data.encrypted_content_info.algorithm.parameters,
         )
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_client.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # Copyright: (c) 2023, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 from __future__ import annotations
 
+import time
 import typing as t
 import uuid
 
-from ._blob import DPAPINGBlob
-from ._crypto import cek_decrypt, content_decrypt
+from ._asn1 import ASN1Writer
+from ._blob import DPAPINGBlob, ProtectionDescriptor
+from ._crypto import (
+    AlgorithmOID,
+    cek_decrypt,
+    cek_encrypt,
+    cek_generate,
+    content_decrypt,
+    content_encrypt,
+)
 from ._dns import async_lookup_dc, lookup_dc
 from ._epm import EPM, EptMap, EptMapResult, TCPFloor, build_tcpip_tower
 from ._gkdi import (
     ISD_KEY,
     FFCDHParameters,
     GetKey,
     GroupKeyEnvelope,
     KDFParameters,
     compute_l1_key,
+    compute_l2_key,
 )
 from ._rpc import (
     NDR,
     NDR64,
     BindAck,
     CommandFlags,
     CommandPContext,
@@ -29,14 +39,16 @@
     Response,
     VerificationTrailer,
     async_create_rpc_connection,
     bind_time_feature_negotiation,
     create_rpc_connection,
 )
 
+_EPOCH_FILETIME = 116444736000000000  # 1970-01-01 as FILETIME
+
 _EPM_CONTEXTS = [
     ContextElement(
         context_id=0,
         abstract_syntax=EPM,
         transfer_syntaxes=[NDR64],
     )
 ]
@@ -222,14 +234,113 @@
         blob.enc_content_algorithm,
         blob.enc_content_parameters,
         cek,
         blob.enc_content,
     )
 
 
+def _encrypt_blob(
+    blob: bytes,
+    key: GroupKeyEnvelope,
+    protection_descriptor: ProtectionDescriptor,
+) -> bytes:
+    # Generate cek and encrypt our payload.
+    enc_cek_algorithm = AlgorithmOID.AES256_WRAP
+    cek, cek_iv = cek_generate(enc_cek_algorithm)
+
+    parameters_writer = ASN1Writer()
+    with parameters_writer.push_sequence() as parameters:
+        parameters.write_octet_string(cek_iv)
+        parameters.write_integer(16)
+
+    enc_content_algorithm = AlgorithmOID.AES256_GCM
+    enc_content_parameters = parameters_writer.get_data()
+    enc_content = content_encrypt(
+        enc_content_algorithm,
+        enc_content_parameters,
+        cek,
+        blob,
+    )
+
+    kek, key_identifier = key.new_kek()
+    enc_cek_parameters = None
+    enc_cek = cek_encrypt(
+        enc_cek_algorithm,
+        enc_cek_parameters,
+        kek,
+        cek,
+    )
+
+    return DPAPINGBlob(
+        key_identifier=key_identifier,
+        protection_descriptor=protection_descriptor,
+        enc_cek=enc_cek,
+        enc_cek_algorithm=enc_cek_algorithm,
+        enc_cek_parameters=enc_cek_parameters,
+        enc_content=enc_content,
+        enc_content_algorithm=enc_content_algorithm,
+        enc_content_parameters=enc_content_parameters,
+    ).pack()
+
+
+def _get_protection_gke_from_cache(
+    root_key_identifier: t.Optional[uuid.UUID],
+    target_sd: bytes,
+    cache: KeyCache,
+) -> t.Optional[GroupKeyEnvelope]:
+    if not root_key_identifier:
+        return None
+
+    # MS-GKDI 3.1.4.1 GetKey rules on how to generate the group key identifier
+    # values from the current time
+    # https://learn.microsoft.com/en-us/openspecs/windows_protocols/ms-gkdi/4cac87a3-521e-4918-a272-240f8fabed39
+    current_time = (time.time_ns() // 100) + _EPOCH_FILETIME
+    base = 360000000000  # 3.6 * 10**11
+    l0 = int(current_time / (32 * 32 * base))
+    l1 = int((current_time % (32 * 32 * base)) / (32 * base))
+    l2 = int((current_time % (32 * base)) / base)
+
+    rk = cache._get_key(
+        target_sd,
+        root_key_identifier,
+        l0,
+        l1,
+        l2,
+    )
+    if not rk:
+        return None
+
+    kdf_parameters = KDFParameters.unpack(rk.kdf_parameters)
+    l2_key = compute_l2_key(
+        kdf_parameters.hash_algorithm,
+        l1,
+        l2,
+        rk,
+    )
+
+    return GroupKeyEnvelope(
+        version=rk.version,
+        flags=rk.flags,
+        l0=l0,
+        l1=l1,
+        l2=l2,
+        root_key_identifier=root_key_identifier,
+        kdf_algorithm=rk.kdf_algorithm,
+        kdf_parameters=rk.kdf_parameters,
+        secret_algorithm=rk.secret_algorithm,
+        secret_parameters=rk.secret_parameters,
+        private_key_length=rk.private_key_length,
+        public_key_length=rk.public_key_length,
+        domain_name=rk.domain_name,
+        forest_name=rk.forest_name,
+        l1_key=b"",
+        l2_key=l2_key,
+    )
+
+
 class RootKey(t.NamedTuple):
     """The KDS Root Key."""
 
     key: bytes
     version: int
     kdf_algorithm: str
     kdf_parameters: bytes
@@ -474,45 +585,138 @@
         NotImplementedError: An unknown value was found and has not been
             implemented yet.
 
     _NCryptUnprotectSecret:
         https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret
     """
     blob = DPAPINGBlob.unpack(data)
+    target_sd = blob.protection_descriptor.get_target_sd()
 
     cache = cache or KeyCache()
     rk = cache._get_key(
-        blob.security_descriptor,
+        target_sd,
         blob.key_identifier.root_key_identifier,
         blob.key_identifier.l0,
         blob.key_identifier.l1,
         blob.key_identifier.l2,
     )
+
     if not rk:
         if not server:
             srv = lookup_dc(blob.key_identifier.domain_name)
             server = srv.target
 
         rk = _sync_get_key(
             server,
-            blob.security_descriptor,
+            target_sd,
             blob.key_identifier.root_key_identifier,
             blob.key_identifier.l0,
             blob.key_identifier.l1,
             blob.key_identifier.l2,
             username=username,
             password=password,
             auth_protocol=auth_protocol,
         )
 
-    cache._store_key(blob.security_descriptor, rk)
+    if not rk.is_public_key:
+        cache._store_key(target_sd, rk)
 
     return _decrypt_blob(blob, rk)
 
 
+def ncrypt_protect_secret(
+    data: bytes,
+    protection_descriptor: str,
+    root_key_identifier: t.Optional[uuid.UUID] = None,
+    server: t.Optional[str] = None,
+    domain_name: t.Optional[str] = None,
+    username: t.Optional[str] = None,
+    password: t.Optional[str] = None,
+    auth_protocol: str = "negotiate",
+    cache: t.Optional[KeyCache] = None,
+) -> bytes:
+    """Encrypt DPAPI-NG Blob.
+
+    Encrypts the blob provided as DPAPI-NG Blob. This is meant to
+    replicate the Win32 API `NCryptProtectSecret`_. While NCryptProtectSecret
+    supports multiple protection descriptor values, currently only the SID type
+    is supported.
+
+    Encrypting the DPAPI-NG blob requires making an RPC call to the domain
+    controller for the domain the blob was created in. It will attempt this
+    by looking up the DC through an SRV lookup but ``server`` can be specified
+    to avoid this SRV lookup.
+
+    The RPC call requires the caller to authenticate before the key information
+    is provided. Explicit credentials can be specified, if none are then the
+    current Kerberos ticket retrieved by ``kinit`` will be used instead. Make
+    sure to install the Kerberos extras package ``dpapi-ng[kerberos]`` to ensure
+    Kerberos auth can be used.
+
+    Args:
+        data: The bytes blob to encrypt.
+        protection_descriptor: The security identifier to protect the secret
+            with.
+        root_key_identifier: Use the root key identified by this id, if not set,
+            the root key id returned by the server will be used.
+        server: The domain controller to lookup the root key info.
+        domain_name: The domain name to query the domain controller hostname
+            via DNS.
+        username: The username to encrypt the DPAPI-NG blob as.
+        password: The password for the user.
+        auth_protocol: The authentication protocol to use, defaults to
+            ``negotiate`` but can be ``kerberos`` or ``ntlm``.
+        cache: Optional cache that is used as the key source to avoid making
+            the RPC call. This only works if root_key_identifier is also
+            specified.
+
+    Returns:
+        bytes: The encrypted DPAPI-NG data.
+
+    Raises:
+        ValueError: An invalid data structure was found.
+        NotImplementedError: An unknown value was found and has not been
+            implemented yet.
+
+    _NCryptProtectSecret:
+        https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptprotectsecret
+    """
+    l0 = -1
+    l1 = -1
+    l2 = -1
+
+    descriptor = ProtectionDescriptor.parse(protection_descriptor)
+    sd = descriptor.get_target_sd()
+
+    cache = cache or KeyCache()
+    rk = _get_protection_gke_from_cache(root_key_identifier, sd, cache)
+
+    if not rk:
+        if not server:
+            srv = lookup_dc(domain_name)
+            server = srv.target
+
+        rk = _sync_get_key(
+            server,
+            sd,
+            root_key_identifier,
+            l0,
+            l1,
+            l2,
+            username=username,
+            password=password,
+            auth_protocol=auth_protocol,
+        )
+
+    if not rk.is_public_key:
+        cache._store_key(sd, rk)
+
+    return _encrypt_blob(data, rk, descriptor)
+
+
 async def async_ncrypt_unprotect_secret(
     data: bytes,
     server: t.Optional[str] = None,
     username: t.Optional[str] = None,
     password: t.Optional[str] = None,
     auth_protocol: str = "negotiate",
     cache: t.Optional[KeyCache] = None,
@@ -552,36 +756,128 @@
         NotImplementedError: An unknown value was found and has not been
             implemented yet.
 
     _NCryptUnprotectSecret:
         https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret
     """
     blob = DPAPINGBlob.unpack(data)
+    target_sd = blob.protection_descriptor.get_target_sd()
 
     cache = cache or KeyCache()
     rk = cache._get_key(
-        blob.security_descriptor,
+        target_sd,
         blob.key_identifier.root_key_identifier,
         blob.key_identifier.l0,
         blob.key_identifier.l1,
         blob.key_identifier.l2,
     )
     if not rk:
         if not server:
             srv = await async_lookup_dc(blob.key_identifier.domain_name)
             server = srv.target
 
         rk = await _async_get_key(
             server,
-            blob.security_descriptor,
+            target_sd,
             blob.key_identifier.root_key_identifier,
             blob.key_identifier.l0,
             blob.key_identifier.l1,
             blob.key_identifier.l2,
             username=username,
             password=password,
             auth_protocol=auth_protocol,
         )
 
-    cache._store_key(blob.security_descriptor, rk)
+    if not rk.is_public_key:
+        cache._store_key(target_sd, rk)
 
     return _decrypt_blob(blob, rk)
+
+
+async def async_ncrypt_protect_secret(
+    data: bytes,
+    protection_descriptor: str,
+    root_key_identifier: t.Optional[uuid.UUID] = None,
+    server: t.Optional[str] = None,
+    domain_name: t.Optional[str] = None,
+    username: t.Optional[str] = None,
+    password: t.Optional[str] = None,
+    auth_protocol: str = "negotiate",
+    cache: t.Optional[KeyCache] = None,
+) -> bytes:
+    """Encrypt DPAPI-NG Blob.
+
+    Encrypts the blob provided as DPAPI-NG Blob. This is meant to
+    replicate the Win32 API `NCryptProtectSecret`_. While NCryptProtectSecret
+    supports multiple protection descriptor values, currently only the SID type
+    is supported.
+
+    Encrypting the DPAPI-NG blob requires making an RPC call to the domain
+    controller for the domain the blob was created in. It will attempt this
+    by looking up the DC through an SRV lookup but ``server`` can be specified
+    to avoid this SRV lookup.
+
+    The RPC call requires the caller to authenticate before the key information
+    is provided. Explicit credentials can be specified, if none are then the
+    current Kerberos ticket retrieved by ``kinit`` will be used instead. Make
+    sure to install the Kerberos extras package ``dpapi-ng[kerberos]`` to ensure
+    Kerberos auth can be used.
+
+    Args:
+        data: The bytes blob to encrypt.
+        protection_descriptor: The security identifier to protect the secret
+            with.
+        root_key_identifier: Use the root key identified by this id, if not set,
+            the root key id returned by the server will be used.
+        server: The domain controller to lookup the root key info.
+        domain_name: The domain name to query the domain controller hostname
+            via DNS.
+        username: The username to encrypt the DPAPI-NG blob as.
+        password: The password for the user.
+        auth_protocol: The authentication protocol to use, defaults to
+            ``negotiate`` but can be ``kerberos`` or ``ntlm``.
+        cache: Optional cache that is used as the key source to avoid making
+            the RPC call. This only works if root_key_identifier is also
+            specified.
+
+    Returns:
+        bytes: The encrypted DPAPI-NG data.
+
+    Raises:
+        ValueError: An invalid data structure was found.
+        NotImplementedError: An unknown value was found and has not been
+            implemented yet.
+
+    _NCryptProtectSecret:
+        https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptprotectsecret
+    """
+    l0 = -1
+    l1 = -1
+    l2 = -1
+
+    descriptor = ProtectionDescriptor.parse(protection_descriptor)
+    sd = descriptor.get_target_sd()
+
+    cache = cache or KeyCache()
+    rk = _get_protection_gke_from_cache(root_key_identifier, sd, cache)
+
+    if not rk:
+        if not server:
+            srv = await async_lookup_dc(domain_name)
+            server = srv.target
+
+        rk = await _async_get_key(
+            server,
+            sd,
+            root_key_identifier,
+            l0,
+            l1,
+            l2,
+            username=username,
+            password=password,
+            auth_protocol=auth_protocol,
+        )
+
+    if not rk.is_public_key:
+        cache._store_key(sd, rk)
+
+    return _encrypt_blob(data, rk, descriptor)
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_crypto.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_crypto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,110 @@
 # Copyright: (c) 2023, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 from __future__ import annotations
 
+import enum
+import os
 import typing as t
 
 from cryptography.hazmat.primitives import hashes, keywrap
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.ciphers.aead import AESGCM
 from cryptography.hazmat.primitives.kdf.concatkdf import ConcatKDFHash
 from cryptography.hazmat.primitives.kdf.kbkdf import KBKDFHMAC, CounterLocation, Mode
 
 from ._asn1 import ASN1Reader
 
 
+class AlgorithmOID(str, enum.Enum):
+    """OIDs for cryptographic algorithms."""
+
+    AES256_WRAP = "2.16.840.1.101.3.4.1.45"
+    AES256_GCM = "2.16.840.1.101.3.4.1.46"
+
+
 def cek_decrypt(
     algorithm: str,
     parameters: t.Optional[bytes],
     kek: bytes,
     value: bytes,
 ) -> bytes:
-    if algorithm == "2.16.840.1.101.3.4.1.45":  # AES256-wrap
+    if algorithm == AlgorithmOID.AES256_WRAP:
         return keywrap.aes_key_unwrap(kek, value)
 
     else:
         raise NotImplementedError(f"Unknown cek encryption algorithm OID '{algorithm}'")
 
 
+def cek_encrypt(
+    algorithm: str,
+    parameters: t.Optional[bytes],
+    kek: bytes,
+    value: bytes,
+) -> bytes:
+    if algorithm == AlgorithmOID.AES256_WRAP:
+        return keywrap.aes_key_wrap(kek, value)
+
+    else:
+        raise NotImplementedError(f"Unknown cek encryption algorithm OID '{algorithm}'")
+
+
+def cek_generate(
+    algorithm: str,
+) -> t.Tuple[bytes, bytes]:
+    if algorithm == AlgorithmOID.AES256_WRAP:
+        cek = AESGCM.generate_key(bit_length=256)
+        cek_iv = os.urandom(12)
+        return cek, cek_iv
+
+    else:
+        raise NotImplementedError(f"Unknown cek encryption algorithm OID '{algorithm}'")
+
+
 def content_decrypt(
     algorithm: str,
     parameters: t.Optional[bytes],
     cek: bytes,
     value: bytes,
 ) -> bytes:
-    if algorithm == "2.16.840.1.101.3.4.1.46":  # AES256-GCM
+    if algorithm == AlgorithmOID.AES256_GCM:
         if not parameters:
             raise ValueError("Expecting parameters for AES256 GCM decryption but received none.")
 
         reader = ASN1Reader(parameters).read_sequence()
         iv = reader.read_octet_string()
 
         cipher = AESGCM(cek)
         return cipher.decrypt(iv, value, None)
 
     else:
         raise NotImplementedError(f"Unknown content encryption algorithm OID '{algorithm}'")
 
 
+def content_encrypt(
+    algorithm: str,
+    parameters: t.Optional[bytes],
+    cek: bytes,
+    value: bytes,
+) -> bytes:
+    if algorithm == AlgorithmOID.AES256_GCM:
+        if not parameters:
+            raise ValueError("Expecting parameters for AES256 GCM encryption but received none.")
+
+        reader = ASN1Reader(parameters).read_sequence()
+        iv = reader.read_octet_string()
+
+        cipher = AESGCM(cek)
+        return cipher.encrypt(iv, value, None)
+
+    else:
+        raise NotImplementedError(f"Unknown content encryption algorithm OID '{algorithm}'")
+
+
 def kdf(
     algorithm: hashes.HashAlgorithm,
     secret: bytes,
     label: bytes,
     context: bytes,
     length: int,
 ) -> bytes:
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_dns.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_dns.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,52 +32,60 @@
         )
 
     # Sorts the array by lowest priority then highest weight.
     return sorted(answers, key=lambda a: (a.priority, -a.weight))[0]
 
 
 async def async_lookup_dc(
-    domain_name: str,
+    domain_name: t.Optional[str] = None,
 ) -> SrvRecord:
     """Lookup DC for domain name
 
-    Attempts to lookup LDAP server based on the domain name specified. This is
-    done through an SRV lookup for '_ldap._tcp.dc._msdcs.{domain_name}'.
+    Attempts to lookup LDAP server based on the domain name specified or the
+    system's search domain if available. This is done through an SRV lookup for
+    '_ldap._tcp.dc._msdcs.{domain_name}'.
 
     Args:
         domain_name: The domain to lookup the DC for.
 
     Returns:
         SrvRecord: The SRV record result.
 
     Raises:
         dns.exception.DNSException: DNS lookup error.
     """
 
-    record = f"_ldap._tcp.dc._msdcs.{domain_name}"
+    if domain_name:
+        record = f"_ldap._tcp.dc._msdcs.{domain_name}"
+    else:
+        record = f"_ldap._tcp.dc._msdcs"
 
-    answers = await dns.asyncresolver.resolve(record, "SRV")
+    answers = await dns.asyncresolver.resolve(record, "SRV", search=True)
     return _get_highest_answer(answers)
 
 
 def lookup_dc(
-    domain_name: str,
+    domain_name: t.Optional[str] = None,
 ) -> SrvRecord:
     """Lookup DC for domain name
 
-    Attempts to lookup LDAP server based on the domain name specified. This is
-    done through an SRV lookup for '_ldap._tcp.dc._msdcs.{domain_name}'.
+    Attempts to lookup LDAP server based on the domain name specified or the
+    system's search domain if available. This is done through an SRV lookup for
+    '_ldap._tcp.dc._msdcs.{domain_name}'.
 
     Args:
         domain_name: The domain to lookup the DC for.
 
     Returns:
         SrvRecord: The SRV record result.
 
     Raises:
         dns.exception.DNSException: DNS lookup error.
     """
 
-    record = f"_ldap._tcp.dc._msdcs.{domain_name}"
+    if domain_name:
+        record = f"_ldap._tcp.dc._msdcs.{domain_name}"
+    else:
+        record = f"_ldap._tcp.dc._msdcs"
 
-    answers = dns.resolver.resolve(record, "SRV")
+    answers = dns.resolver.resolve(record, "SRV", search=True)
     return _get_highest_answer(answers)
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_epm.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_epm.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_gkdi.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_gkdi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright: (c) 2023, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 from __future__ import annotations
 
 import dataclasses
 import math
+import os
 import typing as t
 import uuid
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 
 from ._blob import KeyIdentifier
@@ -213,16 +214,16 @@
 
     key_length: int
     magic: bytes = dataclasses.field(init=False, repr=False, default=b"\x44\x48\x50\x4D")
     field_order: int
     generator: int
 
     def pack(self) -> bytes:
-        b_field_order = self.field_order.to_bytes((self.field_order.bit_length() + 7) // 8, byteorder="big")
-        b_generator = self.generator.to_bytes((self.generator.bit_length() + 7) // 8, byteorder="big")
+        b_field_order = self.field_order.to_bytes(self.key_length, byteorder="big")
+        b_generator = self.generator.to_bytes(self.key_length, byteorder="big")
 
         return b"".join(
             [
                 (12 + len(b_field_order) + len(b_generator)).to_bytes(4, byteorder="little"),
                 self.magic,
                 self.key_length.to_bytes(4, byteorder="little"),
                 b_field_order,
@@ -272,17 +273,17 @@
     magic: bytes = dataclasses.field(init=False, repr=False, default=b"\x44\x48\x50\x42")
     key_length: int
     field_order: int
     generator: int
     public_key: int
 
     def pack(self) -> bytes:
-        b_field_order = self.field_order.to_bytes((self.field_order.bit_length() + 7) // 8, byteorder="big")
-        b_generator = self.generator.to_bytes((self.generator.bit_length() + 7) // 8, byteorder="big")
-        b_pub_key = self.public_key.to_bytes((self.public_key.bit_length() + 7) // 8, byteorder="big")
+        b_field_order = self.field_order.to_bytes(self.key_length, byteorder="big")
+        b_generator = self.generator.to_bytes(self.key_length, byteorder="big")
+        b_pub_key = self.public_key.to_bytes(self.key_length, byteorder="big")
 
         return b"".join(
             [
                 self.magic,
                 self.key_length.to_bytes(4, byteorder="little"),
                 b_field_order,
                 b_generator,
@@ -347,16 +348,17 @@
         return {
             "P256": (ec.SECP256R1(), hashes.SHA256()),
             "P384": (ec.SECP384R1(), hashes.SHA384()),
             "P521": (ec.SECP521R1(), hashes.SHA512()),
         }[self.curve_name]
 
     def pack(self) -> bytes:
-        b_x = self.x.to_bytes((self.x.bit_length() + 7) // 8, byteorder="big")
-        b_y = self.y.to_bytes((self.y.bit_length() + 7) // 8, byteorder="big")
+        b_x = self.x.to_bytes(self.key_length, byteorder="big")
+        b_y = self.y.to_bytes(self.key_length, byteorder="big")
+
         b_curve = {
             "P256": b"\x45\x43\x4B\x31",
             "P384": b"\x45\x43\x4B\x33",
             "P521": b"\x45\x43\x4B\x35",
         }.get(self.curve_name, None)
         if not b_curve:
             raise ValueError(f"Unknown curve '{self.curve_name}', cannot pack.")
@@ -501,15 +503,15 @@
             raise ValueError(f"L0 index {self.l0} does not match the requested L0 index {key_id.l0}")
 
         if self.kdf_algorithm != "SP800_108_CTR_HMAC":
             raise NotImplementedError(f"Unknown KDF algorithm '{self.kdf_algorithm}'")
 
         kdf_parameters = KDFParameters.unpack(self.kdf_parameters)
         hash_algo = kdf_parameters.hash_algorithm
-        l2_key = compute_l2_key(hash_algo, key_id, self)
+        l2_key = compute_l2_key(hash_algo, key_id.l1, key_id.l2, self)
 
         if key_id.is_public_key:
             return compute_kek_from_public_key(
                 algorithm=hash_algo,
                 seed=l2_key,
                 secret_algorithm=self.secret_algorithm,
                 secret_parameters=self.secret_parameters,
@@ -522,14 +524,63 @@
                 hash_algo,
                 l2_key,
                 KDS_SERVICE_LABEL,
                 key_id.key_info,
                 32,
             )
 
+    def new_kek(
+        self,
+    ) -> tuple[bytes, KeyIdentifier]:
+        if self.kdf_algorithm != "SP800_108_CTR_HMAC":
+            raise NotImplementedError(f"Unknown KDF algorithm '{self.kdf_algorithm}'")
+
+        kdf_parameters = KDFParameters.unpack(self.kdf_parameters)
+        hash_algo = kdf_parameters.hash_algorithm
+
+        if self.is_public_key:
+            # If is_public_key flag is set, the L2 key is the peer's public key
+            private_key = os.urandom(math.ceil(self.private_key_length / 8))
+            kek = compute_kek(
+                algorithm=hash_algo,
+                secret_algorithm=self.secret_algorithm,
+                secret_parameters=self.secret_parameters,
+                private_key=private_key,
+                public_key=self.l2_key,
+            )
+
+            key_info = compute_public_key(
+                secret_algorithm=self.secret_algorithm,
+                secret_parameters=self.secret_parameters,
+                private_key=private_key,
+                peer_public_key=self.l2_key,
+            )
+        else:
+            key_info = os.urandom(32)
+            kek = kdf(
+                hash_algo,
+                self.l2_key,
+                KDS_SERVICE_LABEL,
+                key_info,
+                32,
+            )
+
+        key_identifier = KeyIdentifier(
+            version=1,
+            flags=self.flags,
+            l0=self.l0,
+            l1=self.l1,
+            l2=self.l2,
+            root_key_identifier=self.root_key_identifier,
+            key_info=key_info,
+            domain_name=self.domain_name,
+            forest_name=self.forest_name,
+        )
+        return kek, key_identifier
+
     @classmethod
     def unpack(
         cls,
         data: t.Union[bytes, bytearray, memoryview],
     ) -> GroupKeyEnvelope:
         view = memoryview(data)
 
@@ -636,33 +687,34 @@
         compute_kdf_context(root_key_id, l0, 31, -1) + target_sd,
         64,
     )
 
 
 def compute_l2_key(
     algorithm: hashes.HashAlgorithm,
-    request: KeyIdentifier,
+    request_l1: int,
+    request_l2: int,
     rk: GroupKeyEnvelope,
 ) -> bytes:
     l1 = rk.l1
     l1_key = rk.l1_key
     l2 = rk.l2
     l2_key = rk.l2_key
-    reseed_l2 = l2 == 31 or rk.l1 != request.l1
+    reseed_l2 = l2 == 31 or rk.l1 != request_l1
 
     # MS-GKDI 2.2.4 Group key Envelope
     # If the value in the L2 index field is equal to 31, this contains the
     # L1 key with group key identifier (L0 index, L1 index, -1). In all
     # other cases, this field contains the L1 key with group key identifier
     # (L0 index, L1 index - 1, -1). If this field is present, its length
     # MUST be equal to 64 bytes.
-    if l2 != 31 and l1 != request.l1:
+    if l2 != 31 and l1 != request_l1:
         l1 -= 1
 
-    while l1 != request.l1:
+    while l1 != request_l1:
         reseed_l2 = True
         l1 -= 1
 
         l1_key = kdf(
             algorithm,
             l1_key,
             KDS_SERVICE_LABEL,
@@ -686,15 +738,15 @@
                 rk.l0,
                 l1,
                 l2,
             ),
             64,
         )
 
-    while l2 != request.l2:
+    while l2 != request_l2:
         l2 -= 1
 
         l2_key = kdf(
             algorithm,
             l2_key,
             KDS_SERVICE_LABEL,
             compute_kdf_context(
@@ -729,38 +781,54 @@
     algorithm: hashes.HashAlgorithm,
     seed: bytes,
     secret_algorithm: str,
     secret_parameters: t.Optional[bytes],
     public_key: bytes,
     private_key_length: int,
 ) -> bytes:
-    # Special thanks for Grzegorz Tworek (@0gtweet) and Michał Grzegorzewski
-    # for providing access to CQDPAPINGPFXDecrypter.exe which contains the
-    # BCrypt* APIs Microsoft use to derive the KEK.
-
     private_key = kdf(
         algorithm,
         seed,
         KDS_SERVICE_LABEL,
         (secret_algorithm + "\0").encode("utf-16-le"),
         private_key_length,
     )
 
+    return compute_kek(
+        algorithm,
+        secret_algorithm=secret_algorithm,
+        secret_parameters=secret_parameters,
+        private_key=private_key,
+        public_key=public_key,
+    )
+
+
+def compute_kek(
+    algorithm: hashes.HashAlgorithm,
+    secret_algorithm: str,
+    secret_parameters: t.Optional[bytes],
+    private_key: bytes,
+    public_key: bytes,
+) -> bytes:
+    # Special thanks for Grzegorz Tworek (@0gtweet) and Michał Grzegorzewski
+    # for providing access to CQDPAPINGPFXDecrypter.exe which contains the
+    # BCrypt* APIs Microsoft use to derive the KEK.
+
     secret_hash_algorithm: hashes.HashAlgorithm
     if secret_algorithm == "DH":
         # p = FFCDHParameters.unpack(secret_parameters or b"")
         # We can derive the shared secret based on the DH formula.
         # s = y**x mod p
         dh_pub_key = FFCDHKey.unpack(public_key)
         shared_secret_int = pow(
             dh_pub_key.public_key,
             int.from_bytes(private_key, byteorder="big"),
             dh_pub_key.field_order,
         )
-        shared_secret = shared_secret_int.to_bytes((shared_secret_int.bit_length() + 7) // 8, byteorder="big")
+        shared_secret = shared_secret_int.to_bytes(dh_pub_key.key_length, byteorder="big")
         secret_hash_algorithm = hashes.SHA256()
 
     elif secret_algorithm.startswith("ECDH_P"):
         ecdh_pub_key_info = ECDHKey.unpack(public_key)
         curve, secret_hash_algorithm = ecdh_pub_key_info.curve_and_hash
 
         ecdh_pub_key = ec.EllipticCurvePublicNumbers(ecdh_pub_key_info.x, ecdh_pub_key_info.y, curve).public_key()
@@ -794,7 +862,51 @@
     return kdf(
         algorithm,
         secret,
         KDS_SERVICE_LABEL,
         kek_context,
         32,
     )
+
+
+def compute_public_key(
+    secret_algorithm: str,
+    secret_parameters: t.Optional[bytes],
+    private_key: bytes,
+    peer_public_key: bytes,
+) -> bytes:
+    if secret_algorithm == "DH":
+        dh_pub_key = FFCDHKey.unpack(peer_public_key)
+
+        # We can derive our public key based on the DH formula.
+        # X = G**x mod p
+        my_pub_key = pow(
+            dh_pub_key.generator,
+            int.from_bytes(private_key, byteorder="big"),
+            dh_pub_key.field_order,
+        )
+        return FFCDHKey(
+            dh_pub_key.key_length,
+            dh_pub_key.field_order,
+            dh_pub_key.generator,
+            my_pub_key,
+        ).pack()
+
+    elif secret_algorithm.startswith("ECDH_P"):
+        ecdh_pub_key = ECDHKey.unpack(peer_public_key)
+        curve = ecdh_pub_key.curve_and_hash[0]
+
+        ecdh_private = ec.derive_private_key(
+            int.from_bytes(private_key, byteorder="big"),
+            curve,
+        )
+        my_ecdh_pub_key = ecdh_private.public_key().public_numbers()
+
+        return ECDHKey(
+            ecdh_pub_key.curve_name,
+            ecdh_pub_key.key_length,
+            my_ecdh_pub_key.x,
+            my_ecdh_pub_key.y,
+        ).pack()
+
+    else:
+        raise NotImplementedError(f"Unknown secret agreement algorithm '{secret_algorithm}'")
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/__init__.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_auth.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_auth.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_bind.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_bind.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_client.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_client.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_pdu.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_pdu.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_request.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_request.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_rpc/_verification.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_rpc/_verification.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng/_security_descriptor.py` & `dpapi-ng-0.2.0/src/dpapi_ng/_security_descriptor.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng.egg-info/PKG-INFO` & `dpapi-ng-0.2.0/src/dpapi_ng.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpapi-ng
-Version: 0.1.1
+Version: 0.2.0
 Summary: DPAPI NG decryption for Python
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,25 +36,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: kerberos
 License-File: LICENSE
 
-# dpapi_ng - Python DPAPI-NG Decryption Library
+# dpapi_ng - Python DPAPI-NG De-/Encryption Library
 
 [![Test workflow](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml/badge.svg)](https://github.com/jborean93/dpapi-ng/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jborean93/dpapi-ng/branch/main/graph/badge.svg?token=UEA7VoocS5)](https://codecov.io/gh/jborean93/dpapi-ng)
 [![PyPI version](https://badge.fury.io/py/dpapi-ng.svg)](https://badge.fury.io/py/dpapi-ng)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jborean93/dpapi-ng/blob/main/LICENSE)
 
-Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, decryption in Python.
-It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret).
-This can be used on non-Windows hosts to decrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
-It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or by using the credentials of the supplied user to retrieve the required information over RPC.
+Library for [DPAPI NG](https://learn.microsoft.com/en-us/windows/win32/seccng/cng-dpapi), also known as CNG DPAPI, de- and encryption in Python.
+It is designed to replicate the behaviour of [NCryptUnprotectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptunprotectsecret) and [NCryptProtectSecret](https://learn.microsoft.com/en-us/windows/win32/api/ncryptprotect/nf-ncryptprotect-ncryptprotectsecret).
+This can be used on non-Windows hosts to de-/encrypt DPAPI NG protected secrets, like PFX user protected password, or LAPS encrypted password.
+It can either decrypt any DPAPI NG blobs using an offline copy of the domain's root key or de-/encrypt by using the credentials of the supplied user to retrieve the required information over RPC.
 
 Currently only these protection descriptors are supported:
 
 |Type|Purpose|
 |-|-|
 |SID|Only the SID user or members of the SID group can decrypt the secret|
 
@@ -108,41 +108,58 @@
 git clone https://github.com/jborean93/dpapi-ng.git
 cd dpapi-ng
 pip install -e .
 ```
 
 ## Examples
 
-There is both a sync and asyncio API available to decrypt the blob.
+There is both a sync and asyncio API available to de-/encrypt a blob.
 
 ```python
 import dpapi_ng
 
-blob_bytes = b"..."
-dpapi_ng.ncrypt_unprotect_secret(blob_bytes)
 
-# The async equivalent to the above
-await dpapi_ng.async_ncrypt_unprotect_secret(blob_bytes)
+### DECRYPTION ###
+dpapi_ng_blob = b"..."
+decrypted_blob = dpapi_ng.ncrypt_unprotect_secret(dpapi_ng_blob)
+
+# async equivalent to the above
+decrypted_blob = await dpapi_ng.async_ncrypt_unprotect_secret(dpapi_ng_blob)
+
+
+### ENCRYPTION ###
+data = b"..."
+target_sid = "S-1-5-21-XXXXXXXXXX-XXXXXXXXXX-XXXXXXXXXX-XXXX"
+dpapi_ng_blob = dpapi_ng.ncrypt_protect_secret(data, target_sid)
+
+# async equivalent to the above
+dpapi_ng_blob = await dpapi_ng.async_ncrypt_protect_secret(data, target_sid)
 ```
 
-These functions return the decrypt bytes of the DPAPI-NG blob.
 To decrypt the blob, the key specified in the blob needs to be retrieved from the domain controller the blob was generated by.
-The domain controller hostname is retrieved through an `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` or with the value specified in the `server` kwarg.
+To encrypt a blob, the group key of the target SID specified needs to be retrieved.
+For decryption, the domain controller hostname is automatically retrieved through an DNS `SRV` lookup of `_ldap._tcp.dc._msdcs.{domain_name}` with the domain name found in the DPAPI-NG blob or with the value specified in the `server` kwarg.
+For encryption, the domain controller hostname is either determined using the `domain_name` kwarg for a DNS `SRV` lookup, the `server` kwarg directly or by using the system's search domain (if available).
 It will attempt to authenticate with the current user identifier which on Linux will only exist if `kinit` has already been called to retrieve a user's ticket.
 Otherwise if no identity is available, the `username` and `password` kwargs can be used to specify a custom user.
 
-The following kwargs can be used for both `ncrypt_unprotect_secret` and `async_ncrypt_unprotect_secret`.
+The following kwargs can be used for `ncrypt_unprotect_secret`, `async_ncrypt_unprotect_secret`, `ncrypt_protect_secret` and `async_ncrypt_protect_secret`.
 
 * `server`: Use this server as the RPC target if a key needs to be retrieved
 * `username`: The username to authenticate as for the RPC connection
 * `password`: The password to authenticate with for the RPC connection
 * `auth_protocol`: The authentication protocol (`negotiate`, `kerberos`, `ntlm`) to use for the RPC connection
 * `cache`: A cache to store keys retrieved for future operation
 
-It is also possible to decrypt the DPAPI-NG blob by providing the root key stored in the domain.
+In addition to that, `ncrypt_protect_secret` and `async_ncrypt_protect_secret` take the following additional kwarg.
+
+* `domain_name`: The name of the domain/forest to use when looking up the RPC target to use when retrieving the key info
+* `root_key_identifier`: The root key identifier UUID, necessary in order to make the cache work for these functions
+
+It is also possible to encrypt and decrypt the DPAPI-NG blob by providing the root key stored in the domain.
 This can either be retrieved using an offline attack or through an LDAP query if running as a Domain Admin user.
 To retrieve the domain root keys using PowerShell the following can be run:
 
 ```powershell
 $configurationContext = (Get-ADRootDSE).configurationNamingContext
 $getParams = @{
     LDAPFilter = '(objectClass=msKds-ProvRootKey)'
@@ -189,15 +206,15 @@
     msKds-PrivateKeyLength \
     msKds-PublicKeyLength \
     msKds-RootKeyData
 ```
 
 _Note: ldapsearch will most likely need the -H and user bind information to succeed._
 
-The information retrieved there can be stored in a cache and used for subsequent `ncrypt_unprotect_secret` calls:
+The information retrieved there can be stored in a cache and used for subsequent `ncrypt_protect_secret` and `ncrypt_unprotect_secret` calls:
 
 ```python
 import uuid
 
 import dpapi_ng
 
 cache = dpapi_ng.KeyCache()
@@ -219,15 +236,16 @@
 ```
 
 Currently the `SP800_108_CTR_HMAC` KDF algorithm and `DH`, `ECDH_P256`, and `ECDH_P384` secret agreement algorithms have been tested to work.
 The `ECDH_P521` secret agreement algorithm should also work but has been untested as a test environment cannot be created with it right now.
 
 ## Special Thanks
 
-I would like to thank the following people (Twitter handles in brackets) for their help on this project:
+I would like to thank the following people (GitHub or Twitter handles in brackets) for their help on this project:
 
+* Georg Sieber (@schorschii) for implementing encryption support
 * Grzegorz Tworek (@0gtweet) and Michał Grzegorzewski for providing more information on the internal BCrypt* API workflow used in DPAPI-NG
 * Marc-André Moreau (@awakecoding) for their help with reverse engineering some of the Windows APIs and talking through some theories
 * SkelSec (@SkelSec) for help on the RPC calls and being available as a general sounding board for my theories
 * Steve Syfuhs (@SteveSyfuhs) for connecting me with some Microsoft engineers to help understand some undocumented logic
 
 Without their patience and knowledge this probably would not have been possible.
```

### Comparing `dpapi-ng-0.1.1/src/dpapi_ng.egg-info/SOURCES.txt` & `dpapi-ng-0.2.0/src/dpapi_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/tests/test_asn1.py` & `dpapi-ng-0.2.0/tests/test_asn1.py`

 * *Files 5% similar despite different names*

```diff
@@ -262,14 +262,28 @@
     with asn1.ASN1Writer() as writer:
         writer.write_octet_string(b"\xFF", asn1.ASN1Tag(asn1.TagClass.CONTEXT_SPECIFIC, 0, True))
 
     actual = writer.get_data()
     assert actual == expected
 
 
+def test_writer_write_object_identifier() -> None:
+    expected = b"\x06\t*\x86H\x86\xf7\r\x01\x07\x03"
+    with asn1.ASN1Writer() as writer:
+        writer.write_object_identifier("1.2.840.113549.1.7.3")
+
+    actual = writer.get_data()
+    assert actual == expected
+
+
+def test_fail_pack_invalid_object_identifier() -> None:
+    with pytest.raises(ValueError, match="Illegal object identifier"):
+        asn1._encode_object_identifier("40.50.1.2.3")
+
+
 def test_writer_write_enumerated() -> None:
     expected = b"\x0A\x01\x01"
     with asn1.ASN1Writer() as writer:
         writer.write_enumerated(EnumeratedEnum.ENUM1)
 
     actual = writer.get_data()
     assert actual == expected
```

### Comparing `dpapi-ng-0.1.1/tests/test_epm.py` & `dpapi-ng-0.2.0/tests/test_epm.py`

 * *Files identical despite different names*

### Comparing `dpapi-ng-0.1.1/tests/test_gkdi.py` & `dpapi-ng-0.2.0/tests/test_gkdi.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,14 +181,26 @@
         field_order=17125458317614137930196041979257577826408832324037508573393292981642667139747621778802438775238728592968344613589379932348475613503476932163166973813218698343816463289144185362912602522540494983090531497232965829536524507269848825658311420299335922295709743267508322525966773950394919257576842038771632742044142471053509850123605883815857162666917775193496157372656195558305727009891276006514000409365877218171388319923896309377791762590614311849642961380224851940460421710449368927252974870395873936387909672274883295377481008150475878590270591798350563488168080923804611822387520198054002990623911454389104774092183,
         generator=8041367327046189302693984665026706374844608289874374425728797669509435881459140662650215832833471328470334064628508692231999401840332046192569287351991689963279656892562484773278584208040987631569628520464069532361274047374444344996651832979378318849943741662110395995778429270819222431610927356005913836932462099770076239554042855287138026806960470277326229482818003962004453764400995790974042663675692120758726145869061236443893509136147942414445551848162391468541444355707785697825741856849161233887307017428371823608125699892904960841221593344499088996021883972185241854777608212592397013510086894908468466292313,
     )
     actual = msg.pack()
     assert actual == expected
 
 
+def test_ffc_dh_parameters_pack_small_int() -> None:
+    expected = b"\x0C\x02\x00\x00\x44\x48\x50\x4D\x00\x01\x00\x00" + (b"\x00" * 512)
+
+    msg = gkdi.FFCDHParameters(
+        key_length=256,
+        field_order=0,
+        generator=0,
+    )
+    actual = msg.pack()
+    assert actual == expected
+
+
 def test_ffc_dh_parameters_unpack() -> None:
     data = get_test_data("ffc_dh_parameters")
 
     msg = gkdi.FFCDHParameters.unpack(data)
     assert msg.key_length == 256
     assert (
         msg.field_order
@@ -216,14 +228,27 @@
         generator=8041367327046189302693984665026706374844608289874374425728797669509435881459140662650215832833471328470334064628508692231999401840332046192569287351991689963279656892562484773278584208040987631569628520464069532361274047374444344996651832979378318849943741662110395995778429270819222431610927356005913836932462099770076239554042855287138026806960470277326229482818003962004453764400995790974042663675692120758726145869061236443893509136147942414445551848162391468541444355707785697825741856849161233887307017428371823608125699892904960841221593344499088996021883972185241854777608212592397013510086894908468466292313,
         public_key=5704885921161305204062286453104607919457992927353423073733430775789858496179130688612797173128744245915638749285001365389666398628213879947801588663753164579318944467717026038784117675067248922438216443819787917524104523712708262452393840096093436355765031795113819575193160867788883459494877281145141827767886732955150877747794489653818702322115914625862335942729341854451475767409522001908542192343439374586040439834199899031631166319847176777504380608639274486108367307182844033431414378380156678122207936287391923825983630503829617043562049870198440347689535112361024113575576761204481698354807673154816364980520,
     )
     actual = msg.pack()
     assert actual == expected
 
 
+def test_ffc_dh_key_pack_small_int() -> None:
+    expected = b"\x44\x48\x50\x42\x00\x01\x00\x00" + (b"\x00" * 768)
+
+    msg = gkdi.FFCDHKey(
+        key_length=256,
+        field_order=0,
+        generator=0,
+        public_key=0,
+    )
+    actual = msg.pack()
+    assert actual == expected
+
+
 def test_ffc_dh_key_unpack() -> None:
     data = get_test_data("ffc_dh_key")
 
     msg = gkdi.FFCDHKey.unpack(data)
     assert msg.key_length == 256
     assert (
         msg.field_order
@@ -255,14 +280,26 @@
         x=25243830316603712129559807215192800963817053918117758232684283953073092162706,
         y=5597696687659389228845157203945777531845995814681629604081047981407116394432,
     )
     actual = msg.pack()
     assert actual == expected
 
 
+def test_ecdh_key_pack_small_int() -> None:
+    expected = b"\x45\x43\x4B\x31\x20\x00\x00\x00" + (b"\x00" * 64)
+    msg = gkdi.ECDHKey(
+        curve_name="P256",
+        key_length=32,
+        x=0,
+        y=0,
+    )
+    actual = msg.pack()
+    assert actual == expected
+
+
 def test_ecdh_key_pack_invalid_curve() -> None:
     with pytest.raises(ValueError, match="Unknown curve 'test', cannot pack"):
         gkdi.ECDHKey(curve_name="test", key_length=0, x=0, y=0).pack()
 
 
 def test_ecdh_key_unpack() -> None:
     data = get_test_data("ecdh_key")
@@ -549,25 +586,16 @@
         b"\x2F\x2B\xFF\x7F\x7C\x14\xAA\x18"
     )
     l0 = 361
     key_id = uuid.UUID("2e1b932a-4e21-ced3-0b7b-8815aff8335d")
 
     actual = gkdi.compute_l2_key(
         hashes.SHA512(),
-        blob.KeyIdentifier(
-            version=1,
-            flags=0,
-            l0=l0,
-            l1=0,
-            l2=0,
-            root_key_identifier=key_id,
-            key_info=b"",
-            domain_name="",
-            forest_name="",
-        ),
+        0,
+        0,
         gkdi.GroupKeyEnvelope(
             version=1,
             flags=0,
             l0=l0,
             l1=l1,
             l2=l2,
             root_key_identifier=key_id,
```

### Comparing `dpapi-ng-0.1.1/tests/test_security_descriptor.py` & `dpapi-ng-0.2.0/tests/test_security_descriptor.py`

 * *Files identical despite different names*

