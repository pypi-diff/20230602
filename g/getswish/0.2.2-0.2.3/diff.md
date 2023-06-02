# Comparing `tmp/getswish-0.2.2.tar.gz` & `tmp/getswish-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getswish-0.2.2.tar", last modified: Thu Apr 13 14:21:06 2023, max compression
+gzip compressed data, was "getswish-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `getswish-0.2.2.tar` & `getswish-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      482 2023-04-12 11:58:42.537958 getswish-0.2.2/.github/workflows/pytest.yml
--rw-r--r--   0        0        0       82 2023-04-12 10:53:14.553712 getswish-0.2.2/.gitignore
--rw-r--r--   0        0        0      728 2023-04-13 14:19:43.719833 getswish-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0     1069 2023-04-12 05:47:29.766259 getswish-0.2.2/LICENSE
--rw-r--r--   0        0        0     4598 2023-04-12 12:21:45.694971 getswish-0.2.2/README.md
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
--rw-r--r--   0        0        0     3247 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
--rw-r--r--   0        0        0     7165 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
--rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
--rw-r--r--   0        0        0     1338 2023-04-13 10:14:48.087458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
--rw-r--r--   0        0        0     1700 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
--rw-r--r--   0        0        0     3243 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
--rw-r--r--   0        0        0     6006 2023-04-13 10:14:48.087458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
--rw-r--r--   0        0        0     1752 2023-04-12 05:47:28.906216 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
--rw-r--r--   0        0        0     3243 2023-04-12 05:47:28.870215 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
--rw-r--r--   0        0        0     7157 2023-04-12 05:47:28.830213 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
--rw-r--r--   0        0        0     6009 2023-04-12 05:47:28.346189 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
--rw-r--r--   0        0        0     7157 2023-04-13 10:14:48.083458 getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/mss.p12
--rw-r--r--   0        0        0   464323 2023-04-12 05:47:28.194182 getswish-0.2.2/mss_test_1.9/MSS_UserGuide_v1.9.pdf
--rw-r--r--   0        0        0     2565 2023-04-12 05:47:27.938169 getswish-0.2.2/mss_test_1.9/readme.md
--rw-r--r--   0        0        0      312 2023-04-13 09:51:33.541983 getswish-0.2.2/noxfile.py
--rw-r--r--   0        0        0     1567 2023-04-12 13:00:29.698021 getswish-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      328 2023-04-13 14:18:20.695328 getswish-0.2.2/src/getswish/__init__.py
--rw-r--r--   0        0        0     6560 2023-04-13 10:24:03.416266 getswish-0.2.2/src/getswish/client.py
--rw-r--r--   0        0        0     1112 2023-04-13 14:18:09.287262 getswish-0.2.2/src/getswish/environments.py
--rw-r--r--   0        0        0      249 2023-04-12 05:47:29.574250 getswish-0.2.2/src/getswish/exceptions.py
--rw-r--r--   0        0        0     2914 2023-04-12 05:47:29.274235 getswish-0.2.2/src/getswish/models.py
--rw-r--r--   0        0        0     1109 2023-04-12 05:47:29.686255 getswish-0.2.2/src/getswish/utils.py
--rw-r--r--   0        0        0        0 2023-04-12 05:47:30.218282 getswish-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     5186 2023-04-12 07:18:51.268043 getswish-0.2.2/tests/fixtures.py
--rw-r--r--   0        0        0     4089 2023-04-12 10:54:24.594831 getswish-0.2.2/tests/test_client.py
--rw-r--r--   0        0        0      832 2023-04-12 05:47:29.842263 getswish-0.2.2/tests/test_exceptions.py
--rw-r--r--   0        0        0     1390 2023-04-12 10:53:53.850345 getswish-0.2.2/tests/test_models.py
--rw-r--r--   0        0        0     1695 2023-04-12 05:47:29.878265 getswish-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     5452 1970-01-01 00:00:00.000000 getswish-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      482 2023-06-01 04:53:33.993483 getswish-0.2.3/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0       82 2023-06-01 04:53:33.993483 getswish-0.2.3/.gitignore
+-rw-r--r--   0        0        0      887 2023-06-02 13:20:54.296723 getswish-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1069 2023-06-01 04:53:33.993483 getswish-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5446 2023-06-01 08:01:03.944485 getswish-0.2.3/README.md
+-rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3247 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key
+-rw-r--r--   0        0        0     7165 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr
+-rw-r--r--   0        0        0     3243 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key
+-rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12
+-rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem
+-rw-r--r--   0        0        0     1293 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TLS_RootCA.pem
+-rw-r--r--   0        0        0     1700 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr
+-rw-r--r--   0        0        0     3243 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key
+-rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12
+-rw-r--r--   0        0        0     6006 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem
+-rw-r--r--   0        0        0     1752 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr
+-rw-r--r--   0        0        0     3243 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key
+-rw-r--r--   0        0        0     7157 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12
+-rw-r--r--   0        0        0     6009 2023-06-01 04:53:33.997484 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem
+-rw-r--r--   0        0        0     7157 2023-06-01 05:43:50.553375 getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/mss.p12
+-rw-r--r--   0        0        0   464323 2023-06-01 05:43:50.561375 getswish-0.2.3/mss_test_1.9/MSS_UserGuide_v1.9.pdf
+-rw-r--r--   0        0        0     2712 2023-06-01 05:43:50.565375 getswish-0.2.3/mss_test_1.9/readme.md
+-rw-r--r--   0        0        0      312 2023-06-01 04:53:33.997484 getswish-0.2.3/noxfile.py
+-rw-r--r--   0        0        0     1578 2023-06-01 05:13:56.386492 getswish-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      328 2023-06-02 13:23:52.483729 getswish-0.2.3/src/getswish/__init__.py
+-rw-r--r--   0        0        0     6910 2023-06-01 08:00:02.363394 getswish-0.2.3/src/getswish/client.py
+-rw-r--r--   0        0        0     1367 2023-06-01 05:56:09.109830 getswish-0.2.3/src/getswish/environments.py
+-rw-r--r--   0        0        0      249 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/exceptions.py
+-rw-r--r--   0        0        0     2914 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/models.py
+-rw-r--r--   0        0        0     1109 2023-06-01 04:53:33.997484 getswish-0.2.3/src/getswish/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 04:53:33.997484 getswish-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     5284 2023-06-01 08:28:40.092667 getswish-0.2.3/tests/fixtures.py
+-rw-r--r--   0        0        0     4256 2023-06-01 08:29:34.917615 getswish-0.2.3/tests/test_client.py
+-rw-r--r--   0        0        0      832 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1390 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_models.py
+-rw-r--r--   0        0        0     1695 2023-06-01 04:53:34.001484 getswish-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     6338 1970-01-01 00:00:00.000000 getswish-0.2.3/PKG-INFO
```

### Comparing `getswish-0.2.2/LICENSE` & `getswish-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/README.md` & `getswish-0.2.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 agreements are signed, trough https://portal.swish.nu/.
 
 The signing certificate, private key and serial is only required when using the payout API.
 
 ## Example - Test Client
 
 The example code uses the test environment and certificates in this library.
+
 ```python
 import getswish
 
 swish_client = getswish.SwishClient()
 
 callback_url = "https://example.com/callback/"
 
-
 ### Example - Commerce API
 
 # Perform a payment request - E-commerce.
 payment_e = swish_client.create_payment(
     100.00, callback_url, message="Product name."
 )
 
@@ -51,35 +51,41 @@
 payment_cancelled = swish_client.cancel_payment(payment_m.id)
 
 # Refund payment the whole amount to the previous payer which now is the payee.
 payment_refund = swish_client.create_refund(
     payment_e.id, callback_url, payment_e.payer_alias, payment_e.amount
 )
 
-
 ### Example - Payout API
 
+# Generate a merchant specific reference.
+# This reference could be order id or similar.
+# Use generate_transaction_id for convenience.
+
+from getswish.utils import generate_transaction_id
+
+reference_id = generate_transaction_id()
+
 # Perform a payment request
+
 payout = swish_client.create_payout(
-    100.00, callback_url, "46701234567", message="Product name."
+    reference_id, "46701234567", "197001019876", 10.00, callback_url, message="Test payout message."
 )
 
 # Retrieve info about the payout
 payout_retrieved = swish_client.retrieve_payout(payout.payout_instruction_uuid)
 ```
 
-
 ## Example - Production Client
 
 In production the environment must be set
 to `swish.ProductionEnvironment` and all path must be modified to the production certificates that you have generated
 through your bank and swish company portals. The example below is the default configuration for the test certificates
 and environment. Replace all paths and files with your generated production instances.
 
-
 ```python
 from pathlib import Path
 import getswish
 
 cert_base = Path(__file__).parent.parent.parent.resolve()
 cert_base = cert_base / "mss_test_1.9" / "Getswish_Test_Certificates"
 
@@ -92,15 +98,14 @@
         ),
         verify=getswish.Certificate(public=f"{cert_base}/Swish_TLS_RootCA.pem"),
     ),
     merchant_swish_number="1234679304",
 )
 ```
 
-
 ## Example - Production Client with payout
 
 Using the payout API require an additional certificate from your bank and called a signing certificate.
 
 ```python
 from pathlib import Path
 import getswish
@@ -124,14 +129,36 @@
     ),
     merchant_swish_number="1234679304",
 )
 
 callback_url = "https://example.com/callback/"
 ```
 
-
 ### Generating public_serial for signing certificate
 
 The signing certificate `public_serial` is extracted from the certificate using this command on linux.
 
     openssl x509 -in Swish_Merchant_TestSigningCertificate_1234679304.pem -serial -noout
 
+## Development setup
+
+Clone the repository and set up a local virtual environment.
+
+    git clone https://github.com/nibon/getswish-python.git && cd getswish-python
+
+    python3 -m venv .venv
+    source .venv/bin/activate
+    python3 -m pip install flit
+    flit install --only-deps
+
+### Testing installing package and pytest
+
+Symlink getswish and run pytest. You might want to uninstall the getswish library depending on your workflow.
+
+    flit install --symlink
+    pytest
+
+### Testing using nox
+
+Isolated testing on configured python versions and running a coverage test.
+
+    nox
```

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_Merchant_TestSigningCertificate_1234679304.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9870474641.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.csr`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.key`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/Swish_TechnicalSupplier_TestCertificate_9871065216.pem`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/Getswish_Test_Certificates/mss.p12` & `getswish-0.2.3/mss_test_1.9/Getswish_Test_Certificates/mss.p12`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/MSS_UserGuide_v1.9.pdf` & `getswish-0.2.3/mss_test_1.9/MSS_UserGuide_v1.9.pdf`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/mss_test_1.9/readme.md` & `getswish-0.2.3/mss_test_1.9/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # Merchant Swish Simulator #
 
 This directory (zip-file) contains a *User Guide* on how to use the
 *Merchant Swish Simulator (MSS)* together with the test
 *authentication* certificates that are needed in order to properly
-communicate with the server.
+communicate with the server. 
+Please also look at our updated documentation,
+https://developer.swish.nu/
+https://developer.swish.nu/api/mss/v1
 
 For payout requests a specific *Swish_Merchant_TestSigningCertificate*
 is provided that **must** be used to sign the payout request payload
 (create the signature property value). No other signing certificate
 will be accepted by MSS but result in error message returned to
 caller.
 
@@ -36,27 +39,28 @@
 2 directories, 16 files
 
 
 # Certificate expire dates #
 
 `
 ./Getswish_Test_Certificates$ openssl x509 -startdate -enddate -serial -noout -in Swish_Merchant_TestCertificate_1234679304.pem 
-notBefore=May 13 07:43:13 2020 GMT
-notAfter=May 13 07:43:13 2022 GMT
-serial=0BF3A59588F654C767835FC95A53610F
+notBefore=Wed, 20 Jul 2022 14:49:34 GMT
+notAfter=Sat, 20 Jul 2024 14:49:34 GMT
+serial=4EF5C55AA5E475A3611087A4897F3F13
 
 ./Getswish_Test_Certificates$ openssl x509 -startdate -enddate -serial -noout -in Swish_Merchant_TestSigningCertificate_1234679304.pem 
-notBefore=Sep 23 12:00:20 2019 GMT
-notAfter=Sep 23 12:00:20 2021 GMT
-serial=7D70445EC8EF4D1E3A713427E973D097
+notBefore=Wed, 20 Jul 2022 14:40:25 GMT
+notAfter=Sat, 20 Jul 2024 14:40:25 GMT
+serial=51FFA3C2336C8D5B4904D53CD9FAB21D
 
 ./Getswish_Test_Certificates$ openssl x509 -startdate -enddate -serial -noout -in Swish_TechnicalSupplier_TestCertificate_9871065216.pem 
-notBefore=Oct 19 13:28:42 2018 GMT
-notAfter=Oct 19 13:28:42 2020 GMT
-serial=21E0B224ADC487718F485230A2F5C76D
+notBefore=Tue, 09 Aug 2022 09:31:29 GMT
+notAfter=Fri, 09 Aug 2024 09:31:29 GMT
+serial=43180BE273556FF6970249395357B583
 
 ./Getswish_Test_Certificates$ openssl x509 -startdate -enddate -serial -noout -in Swish_TLS_RootCA.pem 
-notBefore=Nov 10 00:00:00 2006 GMT
-notAfter=Nov 10 00:00:00 2031 GMT
+notBefore=Fri, 10 2006 00:00:00 GMT
+notAfter=Mon, 10 2031 00:00:00 GMT
 serial=083BE056904246B1A1756AC95991C74A
 
 `
+
```

### Comparing `getswish-0.2.2/pyproject.toml` & `getswish-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 [project.optional-dependencies]
 tests = [
     "pytest >= 7",
     "pytest-mock",
     "pytest-cov >= 4",
     "ruff",
+    "nox",
 ]
 deploy = [
     "flit >= 3.8",
 ]
 
 [build-system]
 requires = ["flit_core >=3.8.0,<4"]
```

### Comparing `getswish-0.2.2/src/getswish/client.py` & `getswish-0.2.3/src/getswish/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import base64
 import hashlib
 import json
+import logging
 from dataclasses import dataclass
 from datetime import datetime
 
 import requests
 import rsa
 from requests import Response
 
 from .environments import Certificates, Environment, TestEnvironment, TestCertificates
 from .exceptions import SwishError
 from .models import Payment, Payout, Refund
 from .utils import generate_transaction_id
 
+logger = logging.getLogger("getswish")
+logger.addHandler(logging.NullHandler())
+
 
 @dataclass
 class SwishClient:
     environment: Environment = None
     certificates: Certificates = None
     merchant_swish_number: str = "1234679304"
 
     def __post_init__(self):
         if self.environment is None and self.certificates is None:
             self.environment = TestEnvironment
             self.certificates = TestCertificates
+        logger.debug("getswish.env: %s", self.environment.name)
 
     def _url(self, version: str, path: str) -> str:
         return f"{self.environment.base}{version}{path}"
 
     def _requests(self, method: str, url: str, /, **kwargs) -> Response:
         """Requests wrapper that add client certificates and handles api errors and raise http status errors."""
 
@@ -160,14 +165,17 @@
         url = self._url("v1", "/payouts")
         payload = {
             "payload": payload,
             "callbackUrl": callback_url,
             "signature": self._sign_payload(payload),
         }
         response = self._requests("post", url, json=payload)
+        logger.debug("getswish.create_payout.response.text: %s", response.text)
         payout.location = response.headers.get("Location")
         return payout
 
     def retrieve_payout(self, transaction_id: str) -> Payout:
         """https://developer.swish.nu/api/payouts/v1#retrieve-payout"""
 
-        return Payout.from_service(self._requests("get", self._url("v1", f"/payouts/{transaction_id}")).json())
+        response = self._requests("get", self._url("v1", f"/payouts/{transaction_id}"))
+        logger.debug("getswish.retrieve_payout.response.text: %s", response.text)
+        return Payout.from_service(response.json())
```

### Comparing `getswish-0.2.2/src/getswish/models.py` & `getswish-0.2.3/src/getswish/models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/src/getswish/utils.py` & `getswish-0.2.3/src/getswish/utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/tests/fixtures.py` & `getswish-0.2.3/tests/fixtures.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
 @pytest.fixture
 def callback_url() -> str:
     return "https://example.com/callback"
 
 
 @pytest.fixture
+def client_default() -> getswish.SwishClient:
+    return getswish.SwishClient()
+
+
+@pytest.fixture
 def client() -> getswish.SwishClient:
     cert_base = Path(__file__).parent.parent.resolve() / "mss_test_1.9" / "Getswish_Test_Certificates"
     return getswish.SwishClient(
         environment=getswish.TestEnvironment,
         certificates=getswish.Certificates(
             communication=getswish.Certificate(
                 public=f"{cert_base}/Swish_Merchant_TestCertificate_1234679304.pem",
```

### Comparing `getswish-0.2.2/tests/test_client.py` & `getswish-0.2.3/tests/test_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,32 @@
 
 
 @dataclass
 class RequestsMockResponse:
     status_code: int = 200
     json_data: list[dict] | dict = ""
     headers: dict = dict
+    text: str = ""
 
     def json(self):
         return self.json_data
 
     def raise_for_status(self):
         if self.status_code >= 400:
             raise HTTPError()
 
 
+def test_client_init_default(client_default):
+    assert client_default is not None
+
+
+def test_client_init(client):
+    assert client is not None
+
+
 def test_url(client):
     version, path = "v1", "path"
     assert client._url(version, path) == f"{client.environment.base}{version}{path}"
 
 
 def test_sign_payload(client):
     a = client._sign_payload({"foo": "bar"})
```

### Comparing `getswish-0.2.2/tests/test_exceptions.py` & `getswish-0.2.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/tests/test_models.py` & `getswish-0.2.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/tests/test_utils.py` & `getswish-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `getswish-0.2.2/PKG-INFO` & `getswish-0.2.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getswish
-Version: 0.2.2
+Version: 0.2.3
 Summary: Getswish python client library
 Keywords: swish,getswish,payment,payout
 Author-email: Daniel Nibon <daniel@nibon.se>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Requires-Dist: requests >= 2.27
 Requires-Dist: rsa >= 4.7.2
 Requires-Dist: flit >= 3.8 ; extra == "deploy"
 Requires-Dist: pytest >= 7 ; extra == "tests"
 Requires-Dist: pytest-mock ; extra == "tests"
 Requires-Dist: pytest-cov >= 4 ; extra == "tests"
 Requires-Dist: ruff ; extra == "tests"
+Requires-Dist: nox ; extra == "tests"
 Project-URL: Source, https://github.com/nibon/getswish-python
 Provides-Extra: deploy
 Provides-Extra: tests
 
 # Swish - Python client
 
 Client library to integrate with the swish commerce and payout api.
@@ -43,22 +44,22 @@
 agreements are signed, trough https://portal.swish.nu/.
 
 The signing certificate, private key and serial is only required when using the payout API.
 
 ## Example - Test Client
 
 The example code uses the test environment and certificates in this library.
+
 ```python
 import getswish
 
 swish_client = getswish.SwishClient()
 
 callback_url = "https://example.com/callback/"
 
-
 ### Example - Commerce API
 
 # Perform a payment request - E-commerce.
 payment_e = swish_client.create_payment(
     100.00, callback_url, message="Product name."
 )
 
@@ -74,35 +75,41 @@
 payment_cancelled = swish_client.cancel_payment(payment_m.id)
 
 # Refund payment the whole amount to the previous payer which now is the payee.
 payment_refund = swish_client.create_refund(
     payment_e.id, callback_url, payment_e.payer_alias, payment_e.amount
 )
 
-
 ### Example - Payout API
 
+# Generate a merchant specific reference.
+# This reference could be order id or similar.
+# Use generate_transaction_id for convenience.
+
+from getswish.utils import generate_transaction_id
+
+reference_id = generate_transaction_id()
+
 # Perform a payment request
+
 payout = swish_client.create_payout(
-    100.00, callback_url, "46701234567", message="Product name."
+    reference_id, "46701234567", "197001019876", 10.00, callback_url, message="Test payout message."
 )
 
 # Retrieve info about the payout
 payout_retrieved = swish_client.retrieve_payout(payout.payout_instruction_uuid)
 ```
 
-
 ## Example - Production Client
 
 In production the environment must be set
 to `swish.ProductionEnvironment` and all path must be modified to the production certificates that you have generated
 through your bank and swish company portals. The example below is the default configuration for the test certificates
 and environment. Replace all paths and files with your generated production instances.
 
-
 ```python
 from pathlib import Path
 import getswish
 
 cert_base = Path(__file__).parent.parent.parent.resolve()
 cert_base = cert_base / "mss_test_1.9" / "Getswish_Test_Certificates"
 
@@ -115,15 +122,14 @@
         ),
         verify=getswish.Certificate(public=f"{cert_base}/Swish_TLS_RootCA.pem"),
     ),
     merchant_swish_number="1234679304",
 )
 ```
 
-
 ## Example - Production Client with payout
 
 Using the payout API require an additional certificate from your bank and called a signing certificate.
 
 ```python
 from pathlib import Path
 import getswish
@@ -147,15 +153,37 @@
     ),
     merchant_swish_number="1234679304",
 )
 
 callback_url = "https://example.com/callback/"
 ```
 
-
 ### Generating public_serial for signing certificate
 
 The signing certificate `public_serial` is extracted from the certificate using this command on linux.
 
     openssl x509 -in Swish_Merchant_TestSigningCertificate_1234679304.pem -serial -noout
 
+## Development setup
+
+Clone the repository and set up a local virtual environment.
+
+    git clone https://github.com/nibon/getswish-python.git && cd getswish-python
+
+    python3 -m venv .venv
+    source .venv/bin/activate
+    python3 -m pip install flit
+    flit install --only-deps
+
+### Testing installing package and pytest
+
+Symlink getswish and run pytest. You might want to uninstall the getswish library depending on your workflow.
+
+    flit install --symlink
+    pytest
+
+### Testing using nox
+
+Isolated testing on configured python versions and running a coverage test.
+
+    nox
```

