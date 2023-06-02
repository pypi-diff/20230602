# Comparing `tmp/vcert-0.9.0.tar.gz` & `tmp/vcert-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vcert-0.9.0.tar", last modified: Wed Sep 30 19:46:06 2020, max compression
+gzip compressed data, was "dist/vcert-0.9.1.tar", last modified: Tue Dec 15 18:55:38 2020, max compression
```

## Comparing `vcert-0.9.0.tar` & `vcert-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-30 19:46:06.690671 vcert-0.9.0/
--rw-r--r--   0 root         (0) root         (0)      677 2020-09-30 19:46:06.690671 vcert-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4080 2020-09-30 19:33:24.000000 vcert-0.9.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2020-09-30 19:46:06.690671 vcert-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1033 2020-09-30 19:33:24.000000 vcert-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-30 19:46:06.690671 vcert-0.9.0/vcert/
--rw-r--r--   0 root         (0) root         (0)     3303 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22956 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/common.py
--rw-r--r--   0 root         (0) root         (0)    12867 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/connection_cloud.py
--rw-r--r--   0 root         (0) root         (0)     8736 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/connection_fake.py
--rw-r--r--   0 root         (0) root         (0)    15652 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/connection_tpp.py
--rw-r--r--   0 root         (0) root         (0)    19355 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/connection_tpp_token.py
--rw-r--r--   0 root         (0) root         (0)      986 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/errors.py
--rw-r--r--   0 root         (0) root         (0)     6523 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/http.py
--rw-r--r--   0 root         (0) root         (0)     1791 2020-09-30 19:33:24.000000 vcert-0.9.0/vcert/pem.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-30 19:46:06.690671 vcert-0.9.0/vcert.egg-info/
--rw-r--r--   0 root         (0) root         (0)      677 2020-09-30 19:46:06.000000 vcert-0.9.0/vcert.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      344 2020-09-30 19:46:06.000000 vcert-0.9.0/vcert.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-09-30 19:46:06.000000 vcert-0.9.0/vcert.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2020-09-30 19:46:06.000000 vcert-0.9.0/vcert.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2020-09-30 19:46:06.000000 vcert-0.9.0/vcert.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:55:38.818439 vcert-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)      677 2020-12-15 18:55:38.818439 vcert-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4315 2020-12-15 18:42:03.000000 vcert-0.9.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2020-12-15 18:55:38.818439 vcert-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1033 2020-12-15 18:42:03.000000 vcert-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:55:38.818439 vcert-0.9.1/vcert/
+-rw-r--r--   0 root         (0) root         (0)     3303 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23736 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/common.py
+-rw-r--r--   0 root         (0) root         (0)    12867 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/connection_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/connection_fake.py
+-rw-r--r--   0 root         (0) root         (0)    16848 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/connection_tpp.py
+-rw-r--r--   0 root         (0) root         (0)    20473 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/connection_tpp_token.py
+-rw-r--r--   0 root         (0) root         (0)      986 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/http.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2020-12-15 18:42:03.000000 vcert-0.9.1/vcert/pem.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-15 18:55:38.818439 vcert-0.9.1/vcert.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      677 2020-12-15 18:55:38.000000 vcert-0.9.1/vcert.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      344 2020-12-15 18:55:38.000000 vcert-0.9.1/vcert.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-12-15 18:55:38.000000 vcert-0.9.1/vcert.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2020-12-15 18:55:38.000000 vcert-0.9.1/vcert.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-12-15 18:55:38.000000 vcert-0.9.1/vcert.egg-info/top_level.txt
```

### Comparing `vcert-0.9.0/PKG-INFO` & `vcert-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vcert
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python bindings for Venafi TPP/Venfi Cloud API.
 Home-page: https://github.com/Venafi/vcert-python
 Author: Denis Subbotin
 Author-email: denis.subbotin@venafi.com
 License: ASL
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `vcert-0.9.0/README.md` & `vcert-0.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 ![Venafi](Venafi_logo.png)
 [![Apache 2.0 License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Community Supported](https://img.shields.io/badge/Support%20Level-Community-brightgreen)
 ![Compatible with TPP 17.3+ & Cloud](https://img.shields.io/badge/Compatibility-TPP%2017.3+%20%26%20Cloud-f9a90c)  
-_This open source project is community-supported. To report a problem or share an idea, use the
-**[Issues](../../issues)** tab; and if you have a suggestion for fixing the issue, please include those details, too.
-In addition, use the **[Pull requests](../../pulls)** tab to contribute actual bug fixes or proposed enhancements.
-We welcome and appreciate all contributions._
+_**This open source project is community-supported.** To report a problem or share an idea, use
+**[Issues](../../issues)**; and if you have a suggestion for fixing the issue, please include those details, too.
+In addition, use **[Pull Requests](../../pulls)** to contribute actual bug fixes or proposed enhancements.
+We welcome and appreciate all contributions. Got questions or want to discuss something with our team?
+**[Join us on Slack](https://join.slack.com/t/venafi-integrations/shared_invite/zt-i8fwc379-kDJlmzU8OiIQOJFSwiA~dg)**!_
 
 # VCert Python
  
 VCert Python is a Python library and SDK  designed to simplify key generation and enrollment of machine identities
 (also known as SSL/TLS certificates and keys) that comply with enterprise security policy by using the
 [Venafi Platform](https://www.venafi.com/platform/trust-protection-platform) or [Venafi Cloud](https://pki.venafi.com/venafi-cloud/).
 
 This implementation is based on the original Go library, https://github.com/Venafi/vcert.
 
 #### Compatibility
-VCert supports Python 3, and Python 2.7.  VCert releases are tested using the latest version of Trust Protection Platform.  The [latest VCert release](../../releases/latest) should be compatible with Trust Protection Platform 17.3 or higher based on the subset of API methods it consumes.
+VCert supports Python 3, and Python 2.7 (when the [future](http://python-future.org/) module is installed).  VCert releases are tested using the latest version of Trust Protection Platform.  The [latest VCert release](../../releases/latest) should be compatible with Trust Protection Platform 17.3 or higher based on the subset of API methods it consumes.
 
 ## Installation
 Get the library using pip:  
 `pip install vcert`  
 
 You also can install latest version from github:  
 `pip install https://github.com/Venafi/vcert-python/archive/master.zip`
@@ -36,15 +37,15 @@
 
 1. A user account that has been granted WebSDK Access
 2. A folder (zone) where the user has been granted the following permissions: View, Read, Write, Create, Revoke (for the revoke action), and Private Key Read (for the pickup action when CSR is service generated)
 3. Policy applied to the folder which specifies:
     1. CA Template that Trust Protection Platform will use to enroll certificate requests submitted by VCert
     2. Subject DN values for Organizational Unit (OU), Organization (O), City (L), State (ST) and Country (C)
     3. Management Type not locked or locked to 'Enrollment'
-    4. Certificate Signing Request (CSR) Generation not locked or locked to 'Service Generated CSR'
+    4. Certificate Signing Request (CSR) Generation unlocked or not locked to 'Service Generated CSR'.
     5. Generate Key/CSR on Application not locked or locked to 'No'
     6. (Recommended) Disable Automatic Renewal set to 'Yes'
     7. (Recommended) Key Bit Strength set to 2048 or higher
     8. (Recommended) Domain Whitelisting policy appropriately assigned
 
 ## Contributing to VCert
```

### Comparing `vcert-0.9.0/setup.py` & `vcert-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 
 setup(name='vcert',
-      version='0.9.0',
+      version='0.9.1',
       url="https://github.com/Venafi/vcert-python",
       packages=['vcert'],
       install_requires=['requests', 'python-dateutil>=2.6.1', 'certvalidator', 'six',
                         'enum34;python_version<"3.4"', 'ipaddress;python_version<"3.3"',
                         'cryptography', 'future;python_version<"3"'],
       description='Python bindings for Venafi TPP/Venfi Cloud API.',
       author='Denis Subbotin',
```

### Comparing `vcert-0.9.0/vcert/__init__.py` & `vcert-0.9.1/vcert/__init__.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert/common.py` & `vcert-0.9.1/vcert/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         """
         self.key_type = {"rsa": "rsa", "ec": "ec", "ecdsa": "ec"}.get(key_type.lower().strip())
         if self.key_type == KeyType.RSA:
             if option not in KeyType.ALLOWED_SIZES:
                 log.error("unknown size: %s" % option)
                 raise BadData
         elif self.key_type == KeyType.ECDSA:
-            option = {"secp521r1": "p521", "secp384r1": "p384", "secp256r1": "p256", "p256": "p256", "p384":"p384", "p521": "p521"}[option.lower().strip()]
+            option = {"secp521r1": "p521", "secp384r1": "p384", "secp256r1": "p256", "p256": "p256", "p384": "p384",
+                      "p521": "p521"}[option.lower().strip()]
             if option not in KeyType.ALLOWED_CURVES:
                 log.error("unknown curve: %s, should be one of %s" % (option, KeyType.ALLOWED_CURVES))
                 raise BadData
         else:
             log.error("unknown key type: %s" % key_type)
             raise BadData
         self.option = option
@@ -193,15 +194,16 @@
                  common_name=None,
                  thumbprint=None,
                  organization=None,
                  organizational_unit=None,
                  country=None,
                  province=None,
                  locality=None,
-                 origin=None
+                 origin=None,
+                 custom_fields=None,
                  ):
         """
         :param str cert_id: Certificate request id. Generating by server.
         :param list[str] san_dns: Alternative names for SNI.
         :param list[str] email_addresses: List of email addresses
         :param list[str] ip_addresses: List of IP addresses
         :param list[str] user_principal_names: user principal names in username@domain format
@@ -211,14 +213,15 @@
         :param asymmetric.PrivateKey private_key: String with pem encoded private key or  asymmetric.PrivateKey
         :param str key_password: Password for encrypted private key. Not supported at this moment.
         :param str csr: Certificate Signing Request in pem format
         :param str friendly_name: Name for certificate in the platform. If not specified common name will be used.
         :param str common_name: Common name of certificate. Usually domain name.
         :param str thumbprint: Certificate thumbprint. Can be used for identifying certificate on the platform.
         :param str origin: application identifier
+        :param list[CustomField] custom_fields: list of custom fields values to be added to the certificate.
         """
 
         self.chain_option = "last"
         self.san_dns = san_dns or []
         self.email_addresses = email_addresses
         self.ip_addresses = ip_addresses or []
         self.user_principal_names = user_principal_names or []
@@ -237,14 +240,16 @@
         self.organizational_unit = organizational_unit
         self.country = country
         self.province = province
         self.locality = locality
         # CSR should be last, because it checks subject to match with over parameters
         self.csr = csr
         self.origin = origin or "Venafi VCert-Python"
+        self.custom_fields = custom_fields
+        self.cert_guid = None
 
     def __setattr__(self, key, value):
         if key == "key_password":
             if isinstance(value, string_types):
                 value = value.encode()
         elif key == "common_name":
             if isinstance(value, binary_type):
@@ -363,34 +368,34 @@
                 # and https://docs.microsoft.com/en-us/windows/security/identity-protection/smart-cards/smart-card-certificate-requirements-and-enumeration
                 UPNOID = x509.ObjectIdentifier('1.3.6.1.4.1.311.20.2.3')
                 # x509 library expects DER encoded string, so encode UPN into bytes
                 # with ASN1 syntax for UTF8String, which is a type/length/value encoding
                 # per https://docs.microsoft.com/en-us/windows/win32/seccertenroll/about-utf8string
                 # Construct the array of bytes (note bytes are strings in python2)
                 # by inserting the header consisting of the tag '0x0C' followed by the length of the upn
-                if (sys.version_info > (3,0)):
+                if sys.version_info > (3, 0):
                     # For python3, since we have native bytes available we'll convert the string into bytes.
                     # However, for cases when this method is called with inputs extracted from existing certificates
                     # & csrs, the input will already be encoded as bytes. So we'll check the input, if it is a 
                     # string we'll convert it into a bytes object then insert our header. Otherwise, we'll just
                     # insert the header in the passed in bytes.
-                    if (isinstance(upn,str)):
+                    if isinstance(upn, str):
                         bupn = bytes(upn,'utf-8')
                     else:
                         bupn = upn
                     values = [12,len(upn)]
                     header = bytes(values)
                     data = header + bupn
-                    alt_names.append(x509.OtherName(UPNOID,data))
+                    alt_names.append(x509.OtherName(UPNOID, data))
                 else:
                     # For python2, since there is no native bytes method, we'll use the bytes method 
                     # in the future module to convert the string we constructed into bytes.
                     bupn = ''.join(chr(x) for x in [12,len(upn)])
                     bupn = bupn + str(upn)
-                    alt_names.append(x509.OtherName(UPNOID,bytes(bupn,'utf-8')))
+                    alt_names.append(x509.OtherName(UPNOID,bytes(bupn, 'utf-8')))
 
         csr_builder = csr_builder.add_extension(
             x509.SubjectAlternativeName(alt_names),
             critical=False,
         )
 
         csr_builder = csr_builder.sign(self.private_key, hashes.SHA256(),
@@ -438,14 +443,40 @@
             self.province = zone.province.value
         if zone.locality.locked or (not self.locality and zone.locality):
             self.locality = zone.locality.value
         if not self.key_type and zone.key_type:
             self.key_type = zone.key_type
 
 
+class CustomField:
+    def __init__(self, name, value):
+        """
+        :param str name: The name of the custom field
+        :param str value: The value to be added to the specified custom field
+        """
+        self.name = name
+        self.value = value
+
+    @property
+    def name(self):
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        self._name = value
+
+    @property
+    def value(self):
+        return self._value
+
+    @value.setter
+    def value(self, value):
+        self._value = value
+
+
 class RevocationRequest:
     class RevocationReasons:
         NoReason = 0
         key_compromise = 1
         ca_compromise = 2
         affiliation_changed = 3
         superseded = 4
```

### Comparing `vcert-0.9.0/vcert/connection_cloud.py` & `vcert-0.9.1/vcert/connection_cloud.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert/connection_fake.py` & `vcert-0.9.1/vcert/connection_fake.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert/connection_tpp.py` & `vcert-0.9.1/vcert/connection_tpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,27 @@
 import logging as log
 import re
 import time
 
 import requests
 from cryptography.hazmat.backends import default_backend
 from cryptography import x509
-from cryptography.x509 import SignatureAlgorithmOID as algos
+from cryptography.x509 import SignatureAlgorithmOID as AlgOID
 
 from .common import CommonConnection, MIME_JSON, CertField, ZoneConfig, Policy, KeyType
 from .pem import parse_pem
 from .errors import (ServerUnexptedBehavior, ClientBadData, CertificateRequestError, AuthenticationError,
                      CertificateRenewError)
 from .http import HTTPStatus
 
 
 class URLS:
+    def __init__(self):
+        pass
+
     API_BASE_URL = ""
 
     AUTHORIZE = "authorize/"
     CERTIFICATE_REQUESTS = "certificates/request"
     CERTIFICATE_RETRIEVE = "certificates/retrieve"
     FIND_POLICY = "config/findpolicy"
     CERTIFICATE_REVOKE = "certificates/revoke"
@@ -90,15 +93,15 @@
     def _post(self, url, data=None):
         if not self._token or self._token[1] < time.time() + 1:
             self.auth()
             log.debug("Token is %s, timeout is %s" % (self._token[0], self._token[1]))
 
         if isinstance(data, dict):
             r = requests.post(self._base_url + url, headers={TOKEN_HEADER_NAME: self._token[0], 'content-type':
-                              MIME_JSON, "cache-control": "no-cache"}, json=data,  **self._http_request_kwargs)
+                              MIME_JSON, "cache-control": "no-cache"}, json=data, **self._http_request_kwargs)
         else:
             log.error("Unexpected client data type: %s for %s" % (type(data), url))
             raise ClientBadData
         return self.process_server_response(r)
 
     @staticmethod
     def _normalize_and_verify_base_url(u):
@@ -130,28 +133,49 @@
             raise AuthenticationError
 
     # TODO: Need to add service generated CSR implementation
     def request_cert(self, request, zone):
         if not request.csr:
             request.build_csr()
         request_data = {"PolicyDN": self._get_policy_dn(zone),
-                 "PKCS10": request.csr,
-                 "ObjectName": request.friendly_name,
-                 "DisableAutomaticRenewal": "true"}
+                        "PKCS10": request.csr,
+                        "ObjectName": request.friendly_name,
+                        "DisableAutomaticRenewal": "true"}
         if request.origin:
             request_data["Origin"] = request.origin
             ca_origin = {"Name": "Origin", "Value": request.origin}
             if request_data.get("CASpecificAttributes"):
                 request_data["CASpecificAttributes"].append(ca_origin)
             else:
                 request_data["CASpecificAttributes"] = [ca_origin]
+
+        if request.custom_fields:
+            custom_fields_map = {}
+            for c_field in request.custom_fields:
+                if custom_fields_map.get(c_field.name):
+                    custom_fields_map[c_field.name].append(c_field.value)
+                else:
+                    custom_fields_map[c_field.name] = [c_field.value]
+
+            for key in custom_fields_map:
+                custom_field_json = {
+                    "Name": key,
+                    "Values": custom_fields_map[key]
+                }
+                if request_data.get("CustomFields"):
+                    request_data["CustomFields"].append(custom_field_json)
+                else:
+                    request_data["CustomFields"] = [custom_field_json]
+
         status, data = self._post(URLS.CERTIFICATE_REQUESTS, data=request_data)
         if status == HTTPStatus.OK:
             request.id = data['CertificateDN']
-            log.debug("Certificate sucessfully requested with request id %s." % request.id)
+            request.cert_guid = data['Guid']
+            log.debug("Certificate successfully requested with request id %s." % request.id)
+            log.debug("Certificate successfully requested with GUID %s." % request.cert_guid)
             return True
 
         log.error("Request status is not %s. %s." % HTTPStatus.OK, status)
         raise CertificateRequestError
 
     def retrieve_cert(self, certificate_request):
         log.debug("Getting certificate status for id %s" % certificate_request.id)
@@ -235,20 +259,21 @@
             if e.oid == x509.OID_SUBJECT_ALTERNATIVE_NAME:
                 request.san_dns = list([x.value for x in e.value if isinstance(x, x509.DNSName)])
                 request.email_addresses = list([x.value for x in e.value if isinstance(x, x509.RFC822Name)])
                 request.ip_addresses = list([x.value.exploded for x in e.value if isinstance(x, x509.IPAddress)])
                 # remove header bytes from ASN1 encoded UPN field before setting it in the request object
                 upns = []
                 for x in e.value:
-                    if isinstance(x,x509.OtherName):
-                        upns.append(x.value[2 : :])
+                    if isinstance(x, x509.OtherName):
+                        upns.append(x.value[2::])
                 request.user_principal_names = upns
-                request.uniform_resource_identifiers = list([x.value for x in e.value if isinstance(x,x509.UniformResourceIdentifier)])
-        if cert.signature_algorithm_oid in (algos.ECDSA_WITH_SHA1, algos.ECDSA_WITH_SHA224, algos.ECDSA_WITH_SHA256,
-                                            algos.ECDSA_WITH_SHA384, algos.ECDSA_WITH_SHA512):
+                request.uniform_resource_identifiers = list(
+                    [x.value for x in e.value if isinstance(x, x509.UniformResourceIdentifier)])
+        if cert.signature_algorithm_oid in (AlgOID.ECDSA_WITH_SHA1, AlgOID.ECDSA_WITH_SHA224, AlgOID.ECDSA_WITH_SHA256,
+                                            AlgOID.ECDSA_WITH_SHA384, AlgOID.ECDSA_WITH_SHA512):
             request.key_type = (KeyType.ECDSA, KeyType.ALLOWED_CURVES[0])
         else:
             request.key_type = KeyType(KeyType.RSA, 2048)  # todo: make parsing key size
         if not request.csr:
             request.build_csr()
         status, data = self._post(URLS.CERTIFICATE_RENEW,
                                   data={"CertificateDN": request.id, "PKCS10": request.csr})
@@ -309,15 +334,15 @@
             locality=CertField(s['City']['Value'], locked=s['City']['Locked']),
             policy=policy,
             key_type=key_type,
         )
         return z
 
     def read_zone_conf(self, tag):
-        status, data = self._post(URLS.ZONE_CONFIG, {"PolicyDN":  self._get_policy_dn(tag)})
+        status, data = self._post(URLS.ZONE_CONFIG, {"PolicyDN": self._get_policy_dn(tag)})
         if status != HTTPStatus.OK:
             raise ServerUnexptedBehavior("Server returns %d status on reading zone configuration." % status)
         return self._parse_zone_data_to_object(data)
 
     def import_cert(self, request):
         raise NotImplementedError
 
@@ -352,7 +377,13 @@
         status, data = self._post(URLS.CONFIG_READ_DN, {
             "ObjectDN": dn,
             "AttributeName": attribute_name,
         })
         if status != HTTPStatus.OK:
             raise ServerUnexptedBehavior("")
         return data
+
+    def _get_certificate_details(self, cert_guid):
+        status, data = self._get(URLS.CERTIFICATE_SEARCH + cert_guid)
+        if status != HTTPStatus.OK:
+            raise ServerUnexptedBehavior("")
+        return data
```

### Comparing `vcert-0.9.0/vcert/connection_tpp_token.py` & `vcert-0.9.1/vcert/connection_tpp_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import base64
 import logging as log
 import re
 import time
 
 from cryptography.hazmat.backends import default_backend
 from cryptography import x509
-from cryptography.x509 import SignatureAlgorithmOID as algos
+from cryptography.x509 import SignatureAlgorithmOID as AlgOID
 
 from .http import HTTPStatus
 
 import requests
 
 from .common import MIME_JSON, TokenInfo, Authentication, CommonConnection, KeyType, Policy, ZoneConfig, CertField
 from .errors import (ClientBadData, ServerUnexptedBehavior, AuthenticationError, CertificateRequestError,
@@ -160,18 +160,39 @@
         if request.origin:
             request_data["Origin"] = request.origin
             ca_origin = {"Name": "Origin", "Value": request.origin}
             if request_data.get("CASpecificAttributes"):
                 request_data["CASpecificAttributes"].append(ca_origin)
             else:
                 request_data["CASpecificAttributes"] = [ca_origin]
+
+        if request.custom_fields:
+            custom_fields_map = {}
+            for c_field in request.custom_fields:
+                if custom_fields_map.get(c_field.name):
+                    custom_fields_map[c_field.name].append(c_field.value)
+                else:
+                    custom_fields_map[c_field.name] = [c_field.value]
+
+            for key in custom_fields_map:
+                custom_field_json = {
+                    "Name": key,
+                    "Values": custom_fields_map[key]
+                }
+                if request_data.get("CustomFields"):
+                    request_data["CustomFields"].append(custom_field_json)
+                else:
+                    request_data["CustomFields"] = [custom_field_json]
+
         status, data = self._post(URLS.CERTIFICATE_REQUESTS, data=request_data)
         if status == HTTPStatus.OK:
             request.id = data['CertificateDN']
-            log.debug("Certificate sucessfully requested with request id %s." % request.id)
+            request.cert_guid = data['Guid']
+            log.debug("Certificate successfully requested with request id %s." % request.id)
+            log.debug("Certificate successfully requested with GUID %s." % request.cert_guid)
             return True
 
         log.error("Request status is not %s. %s." % HTTPStatus.OK, status)
         raise CertificateRequestError
 
     def retrieve_cert(self, certificate_request):
         log.debug("Getting certificate status for id %s" % certificate_request.id)
@@ -259,16 +280,16 @@
                 # remove header bytes from ASN1 encoded UPN field before setting it in the request object
                 upns = []
                 for x in e.value:
                     if isinstance(x,x509.OtherName):
                         upns.append(x.value[2 : :])
                 request.user_principal_names = upns
                 request.uniform_resource_identifiers = list([x.value for x in e.value if isinstance(x,x509.UniformResourceIdentifier)])
-        if cert.signature_algorithm_oid in (algos.ECDSA_WITH_SHA1, algos.ECDSA_WITH_SHA224, algos.ECDSA_WITH_SHA256,
-                                            algos.ECDSA_WITH_SHA384, algos.ECDSA_WITH_SHA512):
+        if cert.signature_algorithm_oid in (AlgOID.ECDSA_WITH_SHA1, AlgOID.ECDSA_WITH_SHA224, AlgOID.ECDSA_WITH_SHA256,
+                                            AlgOID.ECDSA_WITH_SHA384, AlgOID.ECDSA_WITH_SHA512):
             request.key_type = (KeyType.ECDSA, KeyType.ALLOWED_CURVES[0])
         else:
             request.key_type = KeyType(KeyType.RSA, 2048)  # todo: make parsing key size
         if not request.csr:
             request.build_csr()
         status, data = self._post(URLS.CERTIFICATE_RENEW,
                                   data={"CertificateDN": request.id, "PKCS10": request.csr})
@@ -370,14 +391,20 @@
             "ObjectDN": dn,
             "AttributeName": attribute_name,
         })
         if status != HTTPStatus.OK:
             raise ServerUnexptedBehavior("")
         return data
 
+    def _get_certificate_details(self, cert_guid):
+        status, data = self._get(URLS.CERTIFICATE_SEARCH + cert_guid)
+        if status != HTTPStatus.OK:
+            raise ServerUnexptedBehavior("")
+        return data
+
     def get_access_token(self, authentication=None):
         """
         Obtains an access token to be used for subsequent api operations.
         """
         if authentication and isinstance(authentication, Authentication):
             self._auth = authentication
```

### Comparing `vcert-0.9.0/vcert/errors.py` & `vcert-0.9.1/vcert/errors.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert/http.py` & `vcert-0.9.1/vcert/http.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert/pem.py` & `vcert-0.9.1/vcert/pem.py`

 * *Files identical despite different names*

### Comparing `vcert-0.9.0/vcert.egg-info/PKG-INFO` & `vcert-0.9.1/vcert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: vcert
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python bindings for Venafi TPP/Venfi Cloud API.
 Home-page: https://github.com/Venafi/vcert-python
 Author: Denis Subbotin
 Author-email: denis.subbotin@venafi.com
 License: ASL
 Description: UNKNOWN
 Platform: UNKNOWN
```

