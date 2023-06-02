# Comparing `tmp/gmssl_pyx-1.0.1.tar.gz` & `tmp/gmssl_pyx-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmssl_pyx-1.0.1.tar", last modified: Tue May  2 12:28:05 2023, max compression
+gzip compressed data, was "gmssl_pyx-1.1.0.tar", last modified: Fri Jun  2 16:07:10 2023, max compression
```

## Comparing `gmssl_pyx-1.0.1.tar` & `gmssl_pyx-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7838 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6903 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/gmssl_pyx/
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/gmssl_pyx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/gmssl_pyx/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    29031 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/gmssl_pyx/gmsslmodule.c
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/gmssl_pyx/sm2_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/gmssl_pyx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7838 2023-05-02 12:28:05.000000 gmssl_pyx-1.0.1/gmssl_pyx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-02 12:28:05.000000 gmssl_pyx-1.0.1/gmssl_pyx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 12:28:05.000000 gmssl_pyx-1.0.1/gmssl_pyx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-02 12:28:05.000000 gmssl_pyx-1.0.1/gmssl_pyx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5443 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 12:28:05.401876 gmssl_pyx-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6253 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/tests/test_sm2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/tests/test_sm3.py
--rw-r--r--   0 runner    (1001) docker     (122)     4654 2023-05-02 12:27:56.000000 gmssl_pyx-1.0.1/tests/test_sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7031 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/gmssl_pyx/
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/gmssl_pyx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/gmssl_pyx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30183 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/gmssl_pyx/gmsslext_sm9.c
+-rw-r--r--   0 runner    (1001) docker     (122)    34087 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/gmssl_pyx/gmsslmodule.c
+-rw-r--r--   0 runner    (1001) docker     (122)     1829 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/gmssl_pyx/sm2_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/gmssl_pyx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7966 2023-06-02 16:07:10.000000 gmssl_pyx-1.1.0/gmssl_pyx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-06-02 16:07:10.000000 gmssl_pyx-1.1.0/gmssl_pyx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 16:07:10.000000 gmssl_pyx-1.1.0/gmssl_pyx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-02 16:07:10.000000 gmssl_pyx-1.1.0/gmssl_pyx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5869 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 16:07:10.981315 gmssl_pyx-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     8480 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/tests/test_sm2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2832 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/tests/test_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-06-02 16:07:01.000000 gmssl_pyx-1.1.0/tests/test_sm4.py
```

### Comparing `gmssl_pyx-1.0.1/LICENSE` & `gmssl_pyx-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmssl_pyx-1.0.1/PKG-INFO` & `gmssl_pyx-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmssl_pyx
-Version: 1.0.1
+Version: 1.1.0
 Summary: python wrapper of GmSSL
 Home-page: https://github.com/yetsing/gmssl_pyx
 Author: yeqing
 License: Apache Software License
 Keywords: gmssl
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 使用的版本是 [GmSSL-3.1.0](https://github.com/guanzhi/GmSSL/releases/tag/v3.1.0)
 
 支持 Python 3.7, 3.8, 3.9, 3.10
 
 ## 安装
 
 ```shell
-pip install gmssl_pyx
+pip install gmssl-pyx
 ```
 
 ## SM2
 
 ### 加密和解密
 
 ```python
@@ -166,15 +166,15 @@
 
 ### 公私钥的一些补充说明
 
 公钥长度为 64 字节，是两个 32 字节的整数 x y 拼接而成。
 
 如果公钥长度为 65 字节，那么第一个字节为 '\x04' ，表示后面的 64 字节就是公钥。
 
-如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ， 
+如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ，
 这是一种压缩格式，后面的 32 字节为整数 x ， y 可以根据 x 计算出来。
 
 私钥长度为 32 字节，没有其他变化。
 
 ```python
 from gmssl_pyx import sm2_key_generate, normalize_sm2_public_key
 
@@ -304,7 +304,13 @@
 print('ciphertext', ciphertext)
 
 # 解密
 plaintext = sm4_gcm_decrypt(key, iv=iv, aad=aad, ciphertext=ciphertext, tag=tag)
 print('plaintext', plaintext)
 
 ```
+
+## 其他
+
+[SM9](docs/sm9.md)
+
+如果要查看所有可用的 API ，可以看 [gmsslext.pyi](gmssl_pyx/gmsslext.pyi) 文件。
```

### Comparing `gmssl_pyx-1.0.1/README.md` & `gmssl_pyx-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 使用的版本是 [GmSSL-3.1.0](https://github.com/guanzhi/GmSSL/releases/tag/v3.1.0)
 
 支持 Python 3.7, 3.8, 3.9, 3.10
 
 ## 安装
 
 ```shell
-pip install gmssl_pyx
+pip install gmssl-pyx
 ```
 
 ## SM2
 
 ### 加密和解密
 
 ```python
@@ -141,15 +141,15 @@
 
 ### 公私钥的一些补充说明
 
 公钥长度为 64 字节，是两个 32 字节的整数 x y 拼接而成。
 
 如果公钥长度为 65 字节，那么第一个字节为 '\x04' ，表示后面的 64 字节就是公钥。
 
-如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ， 
+如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ，
 这是一种压缩格式，后面的 32 字节为整数 x ， y 可以根据 x 计算出来。
 
 私钥长度为 32 字节，没有其他变化。
 
 ```python
 from gmssl_pyx import sm2_key_generate, normalize_sm2_public_key
 
@@ -279,7 +279,13 @@
 print('ciphertext', ciphertext)
 
 # 解密
 plaintext = sm4_gcm_decrypt(key, iv=iv, aad=aad, ciphertext=ciphertext, tag=tag)
 print('plaintext', plaintext)
 
 ```
+
+## 其他
+
+[SM9](docs/sm9.md)
+
+如果要查看所有可用的 API ，可以看 [gmsslext.pyi](gmssl_pyx/gmsslext.pyi) 文件。
```

### Comparing `gmssl_pyx-1.0.1/gmssl_pyx/gmsslmodule.c` & `gmssl_pyx-1.1.0/gmssl_pyx/gmsslmodule.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 /*
- * GmSSL sm2 python c extension
+ * GmSSL python c extension
  */
 #define PY_SSIZE_T_CLEAN
 
 #include <Python.h>
 
 #include "gmssl/sm2.h"
 #include "gmssl/sm3.h"
 #include "gmssl/sm4.h"
+#include <gmssl/rand.h>
 
-#define GMSSL_INNER_OK 1
+#include "gmsslext_sm9.h"
+#include "gmsslext.h"
 
-static PyObject *GmsslInnerError;
+PyObject *GmsslInnerError;
 
-static PyObject *InvalidValueError;
+PyObject *InvalidValueError;
 
 static PyObject *
-gmsslext_sm2_key_generate(PyObject *self, PyObject *args) {
+gmsslext_sm2_key_generate(PyObject *self, PyObject *Py_UNUSED(ignored)) {
     SM2_KEY sm2_key;
-    int ret, ok;
+    int ret;
 
     // sm2_key_generate() -> t.Tuple[bytes, bytes]
     // 函数没有参数
-    ok = PyArg_ParseTuple(args, "");
-    if (!ok) {
-        return NULL;
-    }
     ret = sm2_key_generate(&sm2_key);
     if (ret != GMSSL_INNER_OK) {
         PyErr_SetString(GmsslInnerError, "libgmssl inner error in sm2_key_generate");
         return NULL;
     }
     // 整数字面量不是 Py_ssize_t 类型，需要强制转换，不然 Windows 会报错 MemoryError
     return Py_BuildValue("y#y#", &sm2_key.public_key, (Py_ssize_t) 64, &sm2_key.private_key, (Py_ssize_t) 32);
@@ -44,16 +42,17 @@
     Py_ssize_t text_length;
     unsigned char ciphertext[SM2_MAX_CIPHERTEXT_SIZE];
     Py_ssize_t outlen;
     static char *kwlist[] = {"public_key", "plaintext", NULL};
     int ret;
 
     // sm2_encrypt(public_key: bytes, plaintext: bytes) -> bytes
-    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#", kwlist, &public_key, &key_length, &plaintext,
-                                     &text_length)) {
+    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#", kwlist,
+                                     &public_key, &key_length,
+                                     &plaintext, &text_length)) {
         return NULL;
     }
     if (key_length != 64) {
         PyErr_SetString(InvalidValueError, "invalid public key length");
         return NULL;
     }
     if (text_length < SM2_MIN_PLAINTEXT_SIZE || text_length > SM2_MAX_PLAINTEXT_SIZE) {
@@ -120,16 +119,17 @@
     Py_ssize_t digest_length;
     unsigned char sig[SM2_MAX_SIGNATURE_SIZE];
     Py_ssize_t siglen;
     static char *kwlist[] = {"private_key", "digest", NULL};
     int ret;
 
     // sm2_sign_sm3_digest(private_key: bytes, digest: bytes) -> bytes
-    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#", kwlist, &private_key, &key_length, &digest,
-                                     &digest_length)) {
+    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#", kwlist,
+                                     &private_key, &key_length,
+                                     &digest, &digest_length)) {
         return NULL;
     }
     if (key_length != 32) {
         PyErr_SetString(InvalidValueError, "invalid private key length");
         return NULL;
     }
     if (digest_length != SM3_DIGEST_SIZE) {
@@ -158,15 +158,17 @@
     Py_ssize_t digest_length;
     const char *sig;
     Py_ssize_t siglen;
     static char *kwlist[] = {"public_key", "digest", "signature", NULL};
     int ret;
 
     // sm2_verify_sm3_digest(public_key: bytes, digest: bytes, signature: bytes) -> bool
-    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#y#", kwlist, &public_key, &key_length, &digest, &digest_length,
+    if (!PyArg_ParseTupleAndKeywords(args, keywds, "y#y#y#", kwlist,
+                                     &public_key, &key_length,
+                                     &digest, &digest_length,
                                      &sig, &siglen)) {
         return NULL;
     }
     if (key_length != 64) {
         PyErr_SetString(InvalidValueError, "invalid public key length");
         return NULL;
     }
@@ -216,23 +218,31 @@
     size_t signer_id_length = 0;
     if (signer_id_obj == NULL) {
         // 没有传 signer_id ，使用默认值
         signer_id = SM2_DEFAULT_ID;
         signer_id_length = SM2_DEFAULT_ID_LENGTH;
     } else if (signer_id_obj != Py_None) {
         // 参数 signer_id 传的值不是 None
+        signer_id_length = PyBytes_Size(signer_id_obj);
+        if (signer_id_length <= 0 || signer_id_length > SM2_MAX_ID_LENGTH) {
+            PyErr_SetString(InvalidValueError, "invalid signer_id length");
+            return NULL;
+        }
         signer_id = PyBytes_AsString(signer_id_obj);
         if (signer_id == NULL) {
             PyErr_SetString(InvalidValueError, "invalid signer_id");
             return NULL;
         }
-        signer_id_length = PyBytes_Size(signer_id_obj);
     }
     if (public_key_length != 64 || private_key_length != 32) {
-        PyErr_SetString(InvalidValueError, "invalid public_key or private_key");
+        PyErr_SetString(InvalidValueError, "invalid public_key or private_key length");
+        return NULL;
+    }
+    if (message_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty message");
         return NULL;
     }
 
     SM2_KEY sm2_key;
     SM2_SIGN_CTX sign_ctx;
     ret = sm2_key_set_public_key(&sm2_key, (SM2_POINT *) public_key);
     if (ret != GMSSL_INNER_OK) {
@@ -300,24 +310,36 @@
     if (signer_id_obj == NULL) {
         // 没有传 signer_id ，使用默认值
         signer_id = SM2_DEFAULT_ID;
         signer_id_length = SM2_DEFAULT_ID_LENGTH;
     } else if (signer_id_obj != Py_None) {
         // 参数 signer_id 传的值不是 None
         signer_id = PyBytes_AsString(signer_id_obj);
+        signer_id_length = PyBytes_Size(signer_id_obj);
+        if (signer_id_length <= 0 || signer_id_length > SM2_MAX_ID_LENGTH) {
+            PyErr_SetString(InvalidValueError, "invalid signer_id length");
+            return NULL;
+        }
         if (signer_id == NULL) {
             PyErr_SetString(InvalidValueError, "invalid signer_id");
             return NULL;
         }
-        signer_id_length = PyBytes_Size(signer_id_obj);
     }
     if (public_key_length != 64 || private_key_length != 32) {
         PyErr_SetString(InvalidValueError, "invalid public_key or private_key");
         return NULL;
     }
+    if (signature_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty signature");
+        return NULL;
+    }
+    if (message_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty message");
+        return NULL;
+    }
 
     SM2_KEY sm2_key;
     SM2_SIGN_CTX sign_ctx;
     ret = sm2_key_set_public_key(&sm2_key, (SM2_POINT *) public_key);
     if (ret != GMSSL_INNER_OK) {
         PyErr_SetString(InvalidValueError, "invalid public_key");
         return NULL;
@@ -353,14 +375,18 @@
 
     static char *kwlist[] = {"message", NULL};
     // sm3_hash(message: bytes) -> bytes
     ok = PyArg_ParseTupleAndKeywords(args, keywds, "y#", kwlist, &message, &message_length);
     if (!ok) {
         return NULL;
     }
+    if (message_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty message");
+        return NULL;
+    }
     SM3_CTX sm3_ctx;
     uint8_t digest[32];
     sm3_init(&sm3_ctx);
     sm3_update(&sm3_ctx, (uint8_t *) message, message_length);
     sm3_finish(&sm3_ctx, digest);
     return Py_BuildValue("y#", digest, (Py_ssize_t) 32);
 }
@@ -378,14 +404,22 @@
     ok = PyArg_ParseTupleAndKeywords(
             args, keywds, "y#y#", kwlist,
             &key, &key_length,
             &message, &message_length);
     if (!ok) {
         return NULL;
     }
+    if (key_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty key");
+        return NULL;
+    }
+    if (message_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty message");
+        return NULL;
+    }
     SM3_HMAC_CTX hmac_ctx;
     uint8_t digest[SM3_HMAC_SIZE];
     sm3_hmac_init(&hmac_ctx, (uint8_t *) key, key_length);
     sm3_hmac_update(&hmac_ctx, (uint8_t *) message, message_length);
     sm3_hmac_finish(&hmac_ctx, digest);
     return Py_BuildValue("y#", digest, (Py_ssize_t) SM3_HMAC_SIZE);
 }
@@ -402,14 +436,22 @@
     ok = PyArg_ParseTupleAndKeywords(
             args, keywds, "y#k", kwlist,
             &key, &key_length,
             &outlen);
     if (!ok) {
         return NULL;
     }
+    if (key_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty key");
+        return NULL;
+    }
+    if (outlen <= 0) {
+        PyErr_SetString(InvalidValueError, "outlen must be greater than zero");
+        return NULL;
+    }
     char *out = PyMem_RawMalloc(outlen);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
     SM3_KDF_CTX kdf_ctx;
     sm3_kdf_init(&kdf_ctx, outlen);
     sm3_kdf_update(&kdf_ctx, (uint8_t *) key, key_length);
@@ -445,14 +487,18 @@
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
     if (iv_length != SM4_BLOCK_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 iv length");
         return NULL;
     }
+    if (plaintext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty plaintext");
+        return NULL;
+    }
     SM4_KEY sm4_key;
     // 后面最多填充 SM4_BLOCK_SIZE 个字节
     Py_ssize_t outlen = plaintext_length + SM4_BLOCK_SIZE;
     char *out = PyMem_RawMalloc(outlen);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
@@ -492,14 +538,18 @@
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
     if (iv_length != SM4_BLOCK_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 iv length");
         return NULL;
     }
+    if (ciphertext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty ciphertext");
+        return NULL;
+    }
     SM4_KEY sm4_key;
     // 后面最多填充 SM4_BLOCK_SIZE 个字节
     Py_ssize_t outlen = ciphertext_length;
     char *out = PyMem_RawMalloc(outlen);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
@@ -539,14 +589,19 @@
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
     if (ctr_length != SM4_BLOCK_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 ctr length");
         return NULL;
     }
+    if (plaintext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty plaintext");
+        return NULL;
+    }
+
     SM4_KEY sm4_key;
     // 密文长度与明文一致
     char *out = PyMem_RawMalloc(plaintext_length);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
     sm4_set_encrypt_key(&sm4_key, (uint8_t *) key);
@@ -588,14 +643,18 @@
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
     if (ctr_length != SM4_BLOCK_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 ctr length");
         return NULL;
     }
+    if (ciphertext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty ciphertext");
+        return NULL;
+    }
 
     SM4_KEY sm4_key;
     // 明文和密文长度一致
     char *out = PyMem_RawMalloc(ciphertext_length);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
@@ -638,14 +697,23 @@
     if (!ok) {
         return NULL;
     }
     if (key_length != SM4_KEY_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
+    if (iv_length < 1 || iv_length > 64) {
+        PyErr_SetString(InvalidValueError, "invalid sm4 iv length");
+        return NULL;
+    }
+    if (plaintext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty plaintext");
+        return NULL;
+    }
+
     SM4_KEY sm4_key;
     char tag[16];
     // 密文长度与明文一致
     char *out = PyMem_RawMalloc(plaintext_length);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
@@ -653,15 +721,15 @@
     int ret = sm4_gcm_encrypt(
             &sm4_key,
             (uint8_t *) iv, iv_length,
             (uint8_t *) aad, aad_length,
             (uint8_t *) plaintext, plaintext_length,
             (uint8_t *) out, sizeof(tag), (uint8_t *) tag);
     if (ret != GMSSL_INNER_OK) {
-        PyErr_SetString(InvalidValueError, "libgmssl inner error in sm4_gcm_encrypt");
+        PyErr_SetString(GmsslInnerError, "libgmssl inner error in sm4_gcm_encrypt");
         return NULL;
     }
     PyObject *obj = Py_BuildValue("y#y#", out, plaintext_length, tag, (Py_ssize_t) 16);
     PyMem_RawFree(out);
     return obj;
 }
 
@@ -693,50 +761,86 @@
     if (!ok) {
         return NULL;
     }
     if (key_length != SM4_KEY_SIZE) {
         PyErr_SetString(InvalidValueError, "invalid sm4 key length");
         return NULL;
     }
+    if (iv_length < 1 || iv_length > 64) {
+        PyErr_SetString(InvalidValueError, "invalid sm4 iv length");
+        return NULL;
+    }
+    if (ciphertext_length <= 0) {
+        PyErr_SetString(InvalidValueError, "empty ciphertext");
+        return NULL;
+    }
+
     SM4_KEY sm4_key;
     // 密文长度与明文一致
     char *out = PyMem_RawMalloc(ciphertext_length);
     if (out == NULL) {
         return PyErr_NoMemory();
     }
     sm4_set_encrypt_key(&sm4_key, (uint8_t *) key);
     int ret = sm4_gcm_decrypt(
             &sm4_key,
             (uint8_t *) iv, iv_length,
             (uint8_t *) aad, aad_length,
             (uint8_t *) ciphertext, ciphertext_length,
             (uint8_t *) tag, tag_length, (uint8_t *) out);
     if (ret != GMSSL_INNER_OK) {
-        PyErr_SetString(InvalidValueError, "libgmssl inner error in sm4_gcm_decrypt");
+        PyErr_SetString(GmsslInnerError, "libgmssl inner error in sm4_gcm_decrypt");
         return NULL;
     }
     PyObject *obj = Py_BuildValue("y#", out, ciphertext_length);
     PyMem_RawFree(out);
     return obj;
 }
 
+static PyObject *
+gmsslext_rand_bytes(PyObject *self, PyObject *args, PyObject *keywds) {
+    int ok, n, ret;
+    static char *kwlist[] = {"n", NULL};
+    ok = PyArg_ParseTupleAndKeywords(
+            args,
+            keywds,
+            "I",
+            kwlist,
+            &n);
+    if (!ok) {
+        return NULL;
+    }
+    // 256 是 rand_unix.c 的限制
+    if (n <= 0 || n > 256) {
+        PyErr_SetString(InvalidValueError, "n must in [1, 256]");
+        return NULL;
+    }
+    char *buf = PyMem_RawMalloc(n);
+    ret = rand_bytes((uint8_t *) buf, n);
+    if (ret != GMSSL_INNER_OK) {
+        PyErr_SetString(GmsslInnerError, "libgmssl inner error in rand_bytes");
+        return NULL;
+    }
+    PyObject *obj = Py_BuildValue("y#", buf, (Py_ssize_t) n);
+    PyMem_RawFree(buf);
+    return obj;
+}
 
 // 定义模块暴露的函数
 static PyMethodDef SpamMethods[] = {
         {
                 "sm2_key_generate",
                 gmsslext_sm2_key_generate,
-                METH_VARARGS,
+                METH_NOARGS,
                 "生成 SM2 公私密钥对",
         },
         {
                 "sm2_encrypt",
                 (PyCFunction) (void (*)(void)) gmsslext_sm2_encrypt,
                 METH_VARARGS | METH_KEYWORDS,
-
                         "SM2 公钥加密",
         },
         {
                 "sm2_decrypt",
                 (PyCFunction) (void (*)(void)) gmsslext_sm2_decrypt,
                 METH_VARARGS | METH_KEYWORDS,
                         "SM2 私钥解密",
@@ -807,21 +911,27 @@
                 METH_VARARGS | METH_KEYWORDS,
                         "SM3 ctr decrypt",
         },
         {
                 "sm4_gcm_encrypt",
                 (PyCFunction) (void (*)(void)) gmsslext_sm4_gcm_encrypt,
                 METH_VARARGS | METH_KEYWORDS,
-                "SM3 gcm encrypt",
+                        "SM3 gcm encrypt",
         },
         {
                 "sm4_gcm_decrypt",
                 (PyCFunction) (void (*)(void)) gmsslext_sm4_gcm_decrypt,
                 METH_VARARGS | METH_KEYWORDS,
-                "SM3 gcm decrypt",
+                        "SM3 gcm decrypt",
+        },
+        {
+                "rand_bytes",
+                (PyCFunction) (void (*)(void)) gmsslext_rand_bytes,
+                METH_VARARGS | METH_KEYWORDS,
+                        "generate rand bytes",
         },
         {NULL, NULL, 0, NULL}        /* Sentinel */
 };
 
 // 模块属性定义
 static struct PyModuleDef spammodule = {
         PyModuleDef_HEAD_INIT,
@@ -836,35 +946,83 @@
         NULL,
 };
 
 PyMODINIT_FUNC
 PyInit_gmsslext(void) {
     PyObject *m;
 
+    // create custom type
+    if (PyType_Ready(&CustomType) < 0) {
+        return NULL;
+    }
+    if (PyType_Ready(&GmsslextSM9PrivateKeyType) < 0) {
+        return NULL;
+    }
+    if (PyType_Ready(&GmsslextSM9MasterPublicKeyType) < 0) {
+        return NULL;
+    }
+    if (PyType_Ready(&GmsslextSM9MasterKeyType) < 0) {
+        return NULL;
+    }
+
     m = PyModule_Create(&spammodule);
-    if (m == NULL)
+    if (m == NULL) {
         return NULL;
+    }
+
+    Py_INCREF(&CustomType);
+    if (PyModule_AddObject(m, "Custom", (PyObject *) &CustomType) < 0) {
+        Py_DECREF(&CustomType);
+        Py_DECREF(m);
+        return NULL;
+    }
+    Py_INCREF(&GmsslextSM9PrivateKeyType);
+    if (PyModule_AddObject(m, "SM9PrivateKey", (PyObject *) &GmsslextSM9PrivateKeyType) < 0) {
+        Py_DECREF(&GmsslextSM9PrivateKeyType);
+        Py_DECREF(&CustomType);
+        Py_DECREF(m);
+        return NULL;
+    }
+    Py_INCREF(&GmsslextSM9MasterPublicKeyType);
+    if (PyModule_AddObject(m, "SM9MasterPublicKey", (PyObject *) &GmsslextSM9MasterPublicKeyType) < 0) {
+        Py_DECREF(&GmsslextSM9MasterPublicKeyType);
+        Py_DECREF(&GmsslextSM9PrivateKeyType);
+        Py_DECREF(&CustomType);
+        Py_DECREF(m);
+        return NULL;
+    }
+    Py_INCREF(&GmsslextSM9MasterKeyType);
+    if (PyModule_AddObject(m, "SM9MasterKey", (PyObject *) &GmsslextSM9MasterKeyType) < 0) {
+        Py_DECREF(&GmsslextSM9MasterKeyType);
+        Py_DECREF(&GmsslextSM9MasterPublicKeyType);
+        Py_DECREF(&GmsslextSM9PrivateKeyType);
+        Py_DECREF(&CustomType);
+        Py_DECREF(m);
+        return NULL;
+    }
 
     // 新建异常 gmssl.GmsslInnerError ，父类为 Exception
     GmsslInnerError = PyErr_NewException("gmsslext.GmsslInnerError", NULL, NULL);
     Py_XINCREF(GmsslInnerError);
     if (PyModule_AddObject(m, "GmsslInnerError", GmsslInnerError) < 0) {
         Py_XDECREF(GmsslInnerError);
         Py_CLEAR(GmsslInnerError);
+        Py_DECREF(&CustomType);
         Py_DECREF(m);
         return NULL;
     }
     // 新建异常 gmssl.InvalidValueError ，父类为 GmsslInnerError
     InvalidValueError = PyErr_NewException("gmsslext.InvalidValueError", GmsslInnerError, NULL);
     Py_XINCREF(InvalidValueError);
     if (PyModule_AddObject(m, "InvalidValueError", InvalidValueError) < 0) {
         Py_XDECREF(InvalidValueError);
         Py_CLEAR(InvalidValueError);
         Py_XDECREF(GmsslInnerError);
         Py_CLEAR(GmsslInnerError);
+        Py_DECREF(&CustomType);
         Py_DECREF(m);
         return NULL;
     }
 
     return m;
 }
```

### Comparing `gmssl_pyx-1.0.1/gmssl_pyx/sm2_utils.py` & `gmssl_pyx-1.1.0/gmssl_pyx/sm2_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import binascii
 import typing as t
+
 from gmssl_pyx.gmsslext import InvalidValueError
 
 g_default_ecc_table = {
     "n": "FFFFFFFEFFFFFFFFFFFFFFFFFFFFFFFF7203DF6B21C6052B53BBF40939D54123",
     "p": "FFFFFFFEFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF00000000FFFFFFFFFFFFFFFF",
     "g": "32c4ae2c1f1981195f9904466a39c9948fe30bbff2660be1715a4589334c74c7"
     "bc3736a2f4f6779c59bdcee36b692153d0a9877cc62a474002df32e52139f0a0",
```

### Comparing `gmssl_pyx-1.0.1/gmssl_pyx.egg-info/PKG-INFO` & `gmssl_pyx-1.1.0/gmssl_pyx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmssl-pyx
-Version: 1.0.1
+Version: 1.1.0
 Summary: python wrapper of GmSSL
 Home-page: https://github.com/yetsing/gmssl_pyx
 Author: yeqing
 License: Apache Software License
 Keywords: gmssl
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 使用的版本是 [GmSSL-3.1.0](https://github.com/guanzhi/GmSSL/releases/tag/v3.1.0)
 
 支持 Python 3.7, 3.8, 3.9, 3.10
 
 ## 安装
 
 ```shell
-pip install gmssl_pyx
+pip install gmssl-pyx
 ```
 
 ## SM2
 
 ### 加密和解密
 
 ```python
@@ -166,15 +166,15 @@
 
 ### 公私钥的一些补充说明
 
 公钥长度为 64 字节，是两个 32 字节的整数 x y 拼接而成。
 
 如果公钥长度为 65 字节，那么第一个字节为 '\x04' ，表示后面的 64 字节就是公钥。
 
-如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ， 
+如果公钥长度为 33 字节，那么第一个字节为 '\x02' 或者 '\x03' ，
 这是一种压缩格式，后面的 32 字节为整数 x ， y 可以根据 x 计算出来。
 
 私钥长度为 32 字节，没有其他变化。
 
 ```python
 from gmssl_pyx import sm2_key_generate, normalize_sm2_public_key
 
@@ -304,7 +304,13 @@
 print('ciphertext', ciphertext)
 
 # 解密
 plaintext = sm4_gcm_decrypt(key, iv=iv, aad=aad, ciphertext=ciphertext, tag=tag)
 print('plaintext', plaintext)
 
 ```
+
+## 其他
+
+[SM9](docs/sm9.md)
+
+如果要查看所有可用的 API ，可以看 [gmsslext.pyi](gmssl_pyx/gmsslext.pyi) 文件。
```

### Comparing `gmssl_pyx-1.0.1/setup.py` & `gmssl_pyx-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python3
 import os
 import pathlib
-import sys
-import urllib.request
 import shutil
 import subprocess
+import sys
 import tarfile
+import urllib.request
 
+from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
-from setuptools import setup, Extension
-
 
 # 需要给所有文件读写操作都指定编码，避免 windows gbk 编码错误
 utf8 = "utf-8"
 script_directory = pathlib.Path(__file__).resolve().parent
 is_windows = sys.platform.startswith("win32")
 long_description = script_directory.joinpath("README.md").read_text(encoding=utf8)
 
@@ -34,25 +33,26 @@
         urllib.request.urlretrieve(source_url, source_path)
     # 解压到当前文件夹
     with tarfile.open(source_path) as tar:
         tar.extractall()
 
 
 def compile_gmssl():
-    if os.path.exists("./GmSSL-3.1.0/build/bin/libgmssl.a"):
+    if os.path.exists("./GmSSL/build/bin/libgmssl.a"):
         return
     cwd = os.getcwd()
-    # 下载 GmSSL 库编译成静态库
-    # 1.下载源码并解压
-    download_source_code()
+    # 使用了 git submodule 的形式，不需要再单独下载源码
+    # # 下载 GmSSL 库编译成静态库
+    # # 1.下载源码并解压
+    # download_source_code()
 
-    os.chdir("GmSSL-3.1.0")
+    os.chdir("GmSSL")
     if sys.platform.startswith("linux"):
         # 2. 修改 CMakeLists.txt ，直接编译会报错
-        # /usr/bin/ld: ./GmSSL-3.1.0/build/bin/libgmssl.a(sm2_key.c.o): relocation R_X86_64_PC32 against symbol `stderr@@GLIBC_2.2.5' can not be used when making a shared object; recompile with -fPIC
+        # /usr/bin/ld: ./GmSSL/build/bin/libgmssl.a(sm2_key.c.o): relocation R_X86_64_PC32 against symbol `stderr@@GLIBC_2.2.5' can not be used when making a shared object; recompile with -fPIC
         cmake_filename = "CMakeLists.txt"
         with open(cmake_filename, "r", encoding=utf8) as f:
             text = f.read()
         # rand_unix.需要使用 getentropy
         # getentropy 在老版本的Linux发行版和 glibc 中不存在
         text = text.replace("rand_unix.c", "rand.c")
         # 根据错误说明增加编译选项 -fPIC ，加在 "project(GmSSL)" 后面
@@ -71,14 +71,22 @@
         with open(filename, "r", encoding=utf8) as f:
             text = f.read()
         text = text.replace("#include <gmssl/api.h>", "")
         text = text.replace("_gmssl_export", "__declspec(dllexport)")
         with open(filename, "w", encoding=utf8) as f:
             f.write(text)
 
+        filename = "include/gmssl/rand.h"
+        with open(filename, "r", encoding=utf8) as f:
+            text = f.read()
+        text = text.replace("#include <gmssl/api.h>", "")
+        text = text.replace("_gmssl_export", "__declspec(dllexport)")
+        with open(filename, "w", encoding=utf8) as f:
+            f.write(text)
+
     # 3.编译静态库
     if os.path.exists("build"):
         # 删除之前的构建，重新生成
         shutil.rmtree("build")
     # 这两条编译命令来自 GmSSLL 的 github action 配置，文件链接如下
     # https://github.com/guanzhi/GmSSL/blob/v3.1.0/.github/workflows/cmake.yml
     subprocess.check_call("cmake -B build -DBUILD_SHARED_LIBS=OFF", shell=True)
@@ -94,28 +102,31 @@
     def run(self):
         compile_gmssl()
         super().run()
 
 
 def create_extension():
     extra_link_args = []
-    library_dirs = ["./GmSSL-3.1.0/build/bin"]
+    library_dirs = ["./GmSSL/build/bin"]
     libraries = ["gmssl"]
     if sys.platform.startswith("darwin"):
         # macos Symbol not found: _kSecRandomDefault
-        # 对应 GmSSL-3.1.0/src/rand_apple.c
+        # 对应 GmSSL/src/rand_apple.c
         extra_link_args = ["-framework", "Security"]
     elif sys.platform.startswith("win"):
-        # windows security random, 对应 GmSSL-3.1.0/src/rand_win.c
-        library_dirs = ["./GmSSL-3.1.0/build/bin/Debug"]
+        # windows security random, 对应 GmSSL/src/rand_win.c
+        library_dirs = ["./GmSSL/build/bin/Debug"]
         libraries.append("Advapi32")
     extension = Extension(
         "gmssl_pyx.gmsslext",
-        ["gmssl_pyx/gmsslmodule.c"],
-        include_dirs=["./GmSSL-3.1.0/include"],
+        [
+            "gmssl_pyx/gmsslmodule.c",
+            "gmssl_pyx/gmsslext_sm9.c",
+        ],
+        include_dirs=["./GmSSL/include"],
         library_dirs=library_dirs,
         libraries=libraries,
         extra_link_args=extra_link_args,
     )
     return extension
```

### Comparing `gmssl_pyx-1.0.1/tests/test_sm2.py` & `gmssl_pyx-1.1.0/tests/test_sm2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import random
 import secrets
 import unittest
 
 from gmssl_pyx import (
-    sm2_key_generate,
-    sm2_encrypt,
+    GmsslInnerError,
+    InvalidValueError,
+    normalize_sm2_public_key,
+    rand_bytes,
     sm2_decrypt,
-    sm2_sign_sm3_digest,
-    sm2_verify_sm3_digest,
+    sm2_encrypt,
+    sm2_key_generate,
     sm2_sign,
+    sm2_sign_sm3_digest,
     sm2_verify,
-    normalize_sm2_public_key,
-    GmsslInnerError,
-    InvalidValueError,
+    sm2_verify_sm3_digest,
 )
 
 
 class SM2TestCase(unittest.TestCase):
     def test_sm2_encrypt_and_decrypt(self):
         public_key, private_key = sm2_key_generate()
         n = random.randint(1, 255)
@@ -57,17 +58,17 @@
         with self.assertRaises(TypeError):
             sm2_encrypt("abc", b"hello world")
         with self.assertRaises(TypeError):
             sm2_encrypt(public_key, "hello world")
 
         with self.assertRaises(InvalidValueError):
             sm2_decrypt(public_key, b"hello" * 10)
-        with self.assertRaises(GmsslInnerError):
+        with self.assertRaises(InvalidValueError):
             sm2_decrypt(private_key, b"1" * 44)
-        with self.assertRaises(GmsslInnerError):
+        with self.assertRaises(InvalidValueError):
             sm2_decrypt(private_key, b"1" * 367)
         with self.assertRaises(TypeError):
             sm2_decrypt("a" * 32, b"1" * 60)
         with self.assertRaises(TypeError):
             sm2_decrypt(private_key, "1" * 60)
 
     def test_sm2_sign_and_verify_sm3_digest(self):
@@ -156,14 +157,46 @@
             public_key,
             message=message,
             signature=secrets.token_bytes(32),
             signer_id=signer_id,
         )
         self.assertFalse(verify)
 
+    def test_sm2_sign_and_verify_error(self):
+        public_key, private_key = sm2_key_generate()
+        message = b"hello world"
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_sign(private_key[:31], public_key, message)
+        self.assertEqual(str(cm.exception), "invalid public_key or private_key length")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_sign(private_key, public_key[:63], message)
+        self.assertEqual(str(cm.exception), "invalid public_key or private_key length")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_sign(private_key, public_key, b"")
+        self.assertEqual(str(cm.exception), "empty message")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_sign(private_key, public_key, message, signer_id="")
+        self.assertEqual(str(cm.exception), "invalid signer_id length")
+
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_verify(private_key[:31], public_key, message, b"signature")
+        self.assertEqual(str(cm.exception), "invalid public_key or private_key")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_verify(private_key, public_key[:63], message, b"signature")
+        self.assertEqual(str(cm.exception), "invalid public_key or private_key")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_verify(private_key, public_key, b"", b"signature")
+        self.assertEqual(str(cm.exception), "empty message")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_verify(private_key, public_key, message, b"")
+        self.assertEqual(str(cm.exception), "empty signature")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm2_verify(private_key, public_key, message, b"signature", signer_id="")
+        self.assertEqual(str(cm.exception), "invalid signer_id length")
+
     def test_normalize_sm2_public_key(self):
         raw_public_key, _ = sm2_key_generate()
         k1 = normalize_sm2_public_key(raw_public_key)
         self.assertEqual(k1, raw_public_key)
         k1 = normalize_sm2_public_key(b"\x04" + raw_public_key)
         self.assertEqual(k1, raw_public_key)
 
@@ -172,7 +205,16 @@
         if y % 2 == 0:
             # y 是偶数
             compressed_public_key = b"\x02" + raw_public_key[:32]
         else:
             compressed_public_key = b"\x03" + raw_public_key[:32]
         k1 = normalize_sm2_public_key(compressed_public_key)
         self.assertEqual(k1, raw_public_key)
+
+    def test_randbytes(self):
+        for i in range(1, 257):
+            bs = rand_bytes(i)
+            self.assertEqual(len(bs), i)
+
+        with self.assertRaises(InvalidValueError) as cm:
+            rand_bytes(257)
+        self.assertEqual(str(cm.exception), "n must in [1, 256]")
```

### Comparing `gmssl_pyx-1.0.1/tests/test_sm4.py` & `gmssl_pyx-1.1.0/tests/test_sm4.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import random
 import secrets
 import unittest
 
 from gmssl_pyx import (
-    sm4_cbc_padding_encrypt,
+    SM4_BLOCK_SIZE,
+    SM4_KEY_SIZE,
+    InvalidValueError,
     sm4_cbc_padding_decrypt,
-    sm4_ctr_encrypt,
+    sm4_cbc_padding_encrypt,
     sm4_ctr_decrypt,
-    sm4_gcm_encrypt,
+    sm4_ctr_encrypt,
     sm4_gcm_decrypt,
-    SM4_KEY_SIZE,
-    SM4_BLOCK_SIZE,
-    InvalidValueError,
+    sm4_gcm_encrypt,
 )
 
 
 class SM4TestCase(unittest.TestCase):
     def test_cbc_encrypt_and_decrypt(self):
         for i in range(3):
             n = random.randint(1, 4096)
@@ -31,26 +31,36 @@
     def test_cbc_encrypt_and_decrypt_error(self):
         key = secrets.token_bytes(SM4_KEY_SIZE + 1)
         iv = secrets.token_bytes(SM4_BLOCK_SIZE)
         plaintext = b"hello world"
         ciphertext = b"ciphertext"
         with self.assertRaises(InvalidValueError) as cm:
             sm4_cbc_padding_encrypt(key, iv, plaintext)
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
         with self.assertRaises(InvalidValueError) as cm:
             sm4_cbc_padding_decrypt(key, iv, ciphertext)
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
+
         key = secrets.token_bytes(SM4_KEY_SIZE)
         iv = secrets.token_bytes(SM4_BLOCK_SIZE + 1)
         with self.assertRaises(InvalidValueError) as cm:
             sm4_cbc_padding_encrypt(key, iv, plaintext)
-            self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
         with self.assertRaises(InvalidValueError) as cm:
             sm4_cbc_padding_decrypt(key, iv, ciphertext)
-            self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+
+        key = secrets.token_bytes(SM4_KEY_SIZE)
+        iv = secrets.token_bytes(SM4_BLOCK_SIZE)
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_cbc_padding_encrypt(key, iv, b"")
+        self.assertEqual(str(cm.exception), "empty plaintext")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_cbc_padding_decrypt(key, iv, b"")
+        self.assertEqual(str(cm.exception), "empty ciphertext")
 
     def test_ctr_encrypt_and_decrypt(self):
         for i in range(3):
             n = random.randint(1, 4096)
             plaintext = secrets.token_bytes(20)
             key = secrets.token_bytes(SM4_KEY_SIZE)
             ctr = secrets.token_bytes(SM4_BLOCK_SIZE)
@@ -61,26 +71,36 @@
     def test_ctr_encrypt_and_decrypt_error(self):
         key = secrets.token_bytes(SM4_KEY_SIZE + 1)
         ctr = secrets.token_bytes(SM4_BLOCK_SIZE)
         plaintext = b"hello world"
         ciphertext = b"ciphertext"
         with self.assertRaises(InvalidValueError) as cm:
             sm4_ctr_encrypt(key, ctr, plaintext)
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
         with self.assertRaises(InvalidValueError) as cm:
             sm4_ctr_decrypt(key, ctr, ciphertext)
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
+
         key = secrets.token_bytes(SM4_KEY_SIZE)
         ctr = secrets.token_bytes(SM4_BLOCK_SIZE + 1)
         with self.assertRaises(InvalidValueError) as cm:
             sm4_ctr_encrypt(key, ctr, plaintext)
-            self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        self.assertEqual(str(cm.exception), "invalid sm4 ctr length")
         with self.assertRaises(InvalidValueError) as cm:
             sm4_ctr_decrypt(key, ctr, ciphertext)
-            self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        self.assertEqual(str(cm.exception), "invalid sm4 ctr length")
+
+        key = secrets.token_bytes(SM4_KEY_SIZE)
+        ctr = secrets.token_bytes(SM4_BLOCK_SIZE)
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_ctr_encrypt(key, ctr, b"")
+        self.assertEqual(str(cm.exception), "empty plaintext")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_ctr_decrypt(key, ctr, b"")
+        self.assertEqual(str(cm.exception), "empty ciphertext")
 
     def test_gcm_encrypt_and_decrypt(self):
         for i in range(3):
             n = random.randint(1, 4096)
             plaintext = secrets.token_bytes(n)
             key = secrets.token_bytes(SM4_KEY_SIZE)
             iv = secrets.token_bytes(SM4_BLOCK_SIZE)
@@ -95,11 +115,34 @@
         key = secrets.token_bytes(SM4_KEY_SIZE + 1)
         iv = secrets.token_bytes(SM4_BLOCK_SIZE)
         aad = secrets.token_bytes(16)
         plaintext = b"hello world"
         ciphertext = b"ciphertext"
         with self.assertRaises(InvalidValueError) as cm:
             sm4_gcm_encrypt(key, iv, aad, plaintext)
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
         with self.assertRaises(InvalidValueError) as cm:
             sm4_gcm_decrypt(key, iv, aad, ciphertext, tag=secrets.token_bytes(16))
-            self.assertEqual(str(cm.exception), "invalid sm4 key length")
+        self.assertEqual(str(cm.exception), "invalid sm4 key length")
+
+        key = secrets.token_bytes(SM4_KEY_SIZE)
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_encrypt(key, b"", aad, plaintext)
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_encrypt(key, b"1" * 65, aad, plaintext)
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_decrypt(key, b"", aad, ciphertext, tag=secrets.token_bytes(16))
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_decrypt(
+                key, b"1" * 65, aad, ciphertext, tag=secrets.token_bytes(16)
+            )
+        self.assertEqual(str(cm.exception), "invalid sm4 iv length")
+
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_encrypt(key, iv, aad, b"")
+        self.assertEqual(str(cm.exception), "empty plaintext")
+        with self.assertRaises(InvalidValueError) as cm:
+            sm4_gcm_decrypt(key, iv, aad, b"", tag=secrets.token_bytes(16))
+        self.assertEqual(str(cm.exception), "empty ciphertext")
```

