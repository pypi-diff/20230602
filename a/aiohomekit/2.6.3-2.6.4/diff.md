# Comparing `tmp/aiohomekit-2.6.3.tar.gz` & `tmp/aiohomekit-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohomekit-2.6.3.tar", max compression
+gzip compressed data, was "aiohomekit-2.6.4.tar", max compression
```

## Comparing `aiohomekit-2.6.3.tar` & `aiohomekit-2.6.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11537 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/LICENSE.md
--rw-r--r--   0        0        0     5841 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/README.md
--rw-r--r--   0        0        0     1867 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/aiohomekit/__init__.py
--rw-r--r--   0        0        0    18829 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/aiohomekit/__main__.py
--rw-r--r--   0        0        0     4465 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/aiohomekit/characteristic_cache.py
--rw-r--r--   0        0        0     1162 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/aiohomekit/const.py
--rw-r--r--   0        0        0      697 2023-04-04 00:45:15.430453 aiohomekit-2.6.3/aiohomekit/controller/__init__.py
--rw-r--r--   0        0        0    15767 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/abstract.py
--rw-r--r--   0        0        0      704 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/__init__.py
--rw-r--r--   0        0        0     6832 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/bleak.py
--rw-r--r--   0        0        0     7819 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/client.py
--rw-r--r--   0        0        0     2017 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/connection.py
--rw-r--r--   0        0        0     1310 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/const.py
--rw-r--r--   0        0        0     7024 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/controller.py
--rw-r--r--   0        0        0     7614 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/discovery.py
--rw-r--r--   0        0        0     1894 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/key.py
--rw-r--r--   0        0        0     3749 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/manufacturer_data.py
--rw-r--r--   0        0        0    68500 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/pairing.py
--rw-r--r--   0        0        0    11737 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/structs.py
--rw-r--r--   0        0        0     2140 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ble/values.py
--rw-r--r--   0        0        0      708 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/__init__.py
--rw-r--r--   0        0        0    25705 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/connection.py
--rw-r--r--   0        0        0     1182 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/controller.py
--rw-r--r--   0        0        0     2422 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/discovery.py
--rw-r--r--   0        0        0     9972 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/pairing.py
--rw-r--r--   0        0        0     3433 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/pdu.py
--rw-r--r--   0        0        0    12547 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/coap/structs.py
--rw-r--r--   0        0        0     9288 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/controller.py
--rw-r--r--   0        0        0      757 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ip/__init__.py
--rw-r--r--   0        0        0    21656 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ip/connection.py
--rw-r--r--   0        0        0     1120 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ip/controller.py
--rw-r--r--   0        0        0     4108 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ip/discovery.py
--rw-r--r--   0        0        0    20914 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/controller/ip/pairing.py
--rw-r--r--   0        0        0      868 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/crypto/__init__.py
--rw-r--r--   0        0        0     4789 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/crypto/chacha20poly1305.py
--rw-r--r--   0        0        0     1036 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/crypto/hkdf.py
--rw-r--r--   0        0        0    10728 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/crypto/srp.py
--rw-r--r--   0        0        0     4060 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/debounce.py
--rw-r--r--   0        0        0      985 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/enum.py
--rw-r--r--   0        0        0     7746 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/exceptions.py
--rw-r--r--   0        0        0     2116 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/hkjson.py
--rw-r--r--   0        0        0     2049 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/http/__init__.py
--rw-r--r--   0        0        0     5265 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/http/response.py
--rw-r--r--   0        0        0     2609 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/meshcop.py
--rw-r--r--   0        0        0    12582 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/__init__.py
--rw-r--r--   0        0        0     1245 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/categories.py
--rw-r--r--   0        0        0     1892 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/__init__.py
--rw-r--r--   0        0        0    14170 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic.py
--rw-r--r--   0        0        0     1815 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic_formats.py
--rw-r--r--   0        0        0    22463 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic_types.py
--rw-r--r--   0        0        0     4438 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/const.py
--rw-r--r--   0        0        0    29366 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/data.py
--rw-r--r--   0        0        0      800 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/permissions.py
--rw-r--r--   0        0        0     4410 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/structs.py
--rw-r--r--   0        0        0      731 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/types.py
--rw-r--r--   0        0        0     1067 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/characteristics/units.py
--rw-r--r--   0        0        0     1439 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/entity_map.py
--rw-r--r--   0        0        0      723 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/feature_flags.py
--rw-r--r--   0        0        0      685 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/mixin.py
--rw-r--r--   0        0        0      796 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/services/__init__.py
--rw-r--r--   0        0        0    19993 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/services/data.py
--rw-r--r--   0        0        0     5021 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/services/service.py
--rw-r--r--   0        0        0     5380 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/services/service_types.py
--rw-r--r--   0        0        0      703 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/services/types.py
--rw-r--r--   0        0        0      717 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/model/status_flags.py
--rw-r--r--   0        0        0     4067 2023-04-04 00:45:15.434453 aiohomekit-2.6.3/aiohomekit/pdu.py
--rw-r--r--   0        0        0    20539 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/protocol/__init__.py
--rw-r--r--   0        0        0     3494 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/protocol/statuscodes.py
--rw-r--r--   0        0        0     8483 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/protocol/tlv.py
--rw-r--r--   0        0        0        0 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/py.typed
--rw-r--r--   0        0        0    12836 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/testing.py
--rw-r--r--   0        0        0     8265 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/tlv8.py
--rw-r--r--   0        0        0     3581 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/utils.py
--rw-r--r--   0        0        0     1662 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/uuid.py
--rw-r--r--   0        0        0    11606 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/aiohomekit/zeroconf.py
--rw-r--r--   0        0        0     1829 2023-04-04 00:45:15.438452 aiohomekit-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     7122 1970-01-01 00:00:00.000000 aiohomekit-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11537 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/LICENSE.md
+-rw-r--r--   0        0        0     5841 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/README.md
+-rw-r--r--   0        0        0     1867 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/__init__.py
+-rw-r--r--   0        0        0    18829 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/__main__.py
+-rw-r--r--   0        0        0     4465 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/characteristic_cache.py
+-rw-r--r--   0        0        0     1162 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/const.py
+-rw-r--r--   0        0        0      697 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/__init__.py
+-rw-r--r--   0        0        0    15767 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/abstract.py
+-rw-r--r--   0        0        0      704 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/bleak.py
+-rw-r--r--   0        0        0     7819 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/client.py
+-rw-r--r--   0        0        0     2017 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/connection.py
+-rw-r--r--   0        0        0     1310 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/const.py
+-rw-r--r--   0        0        0     7024 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/controller.py
+-rw-r--r--   0        0        0     7614 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/discovery.py
+-rw-r--r--   0        0        0     1894 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/key.py
+-rw-r--r--   0        0        0     3749 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/manufacturer_data.py
+-rw-r--r--   0        0        0    68500 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/pairing.py
+-rw-r--r--   0        0        0    11737 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/structs.py
+-rw-r--r--   0        0        0     2140 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/values.py
+-rw-r--r--   0        0        0      708 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/__init__.py
+-rw-r--r--   0        0        0    25705 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/connection.py
+-rw-r--r--   0        0        0     1182 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/controller.py
+-rw-r--r--   0        0        0     2422 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/discovery.py
+-rw-r--r--   0        0        0     9972 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/pairing.py
+-rw-r--r--   0        0        0     3433 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/pdu.py
+-rw-r--r--   0        0        0    12547 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/structs.py
+-rw-r--r--   0        0        0     9288 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/controller.py
+-rw-r--r--   0        0        0      757 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/__init__.py
+-rw-r--r--   0        0        0    22040 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/connection.py
+-rw-r--r--   0        0        0     1120 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/controller.py
+-rw-r--r--   0        0        0     4108 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/discovery.py
+-rw-r--r--   0        0        0    20914 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/pairing.py
+-rw-r--r--   0        0        0      868 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/__init__.py
+-rw-r--r--   0        0        0     4789 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/chacha20poly1305.py
+-rw-r--r--   0        0        0     1036 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/hkdf.py
+-rw-r--r--   0        0        0    10728 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/srp.py
+-rw-r--r--   0        0        0     4060 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/debounce.py
+-rw-r--r--   0        0        0      985 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/enum.py
+-rw-r--r--   0        0        0     7746 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/exceptions.py
+-rw-r--r--   0        0        0     2116 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/hkjson.py
+-rw-r--r--   0        0        0     2049 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/http/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/http/response.py
+-rw-r--r--   0        0        0     2609 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/meshcop.py
+-rw-r--r--   0        0        0    12582 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/__init__.py
+-rw-r--r--   0        0        0     1245 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/categories.py
+-rw-r--r--   0        0        0     1892 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/__init__.py
+-rw-r--r--   0        0        0    14170 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic.py
+-rw-r--r--   0        0        0     1815 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_formats.py
+-rw-r--r--   0        0        0    22463 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_types.py
+-rw-r--r--   0        0        0     4956 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/const.py
+-rw-r--r--   0        0        0    29366 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/data.py
+-rw-r--r--   0        0        0      800 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/permissions.py
+-rw-r--r--   0        0        0     4410 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/structs.py
+-rw-r--r--   0        0        0      731 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/types.py
+-rw-r--r--   0        0        0     1067 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/units.py
+-rw-r--r--   0        0        0     1439 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/entity_map.py
+-rw-r--r--   0        0        0      723 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/feature_flags.py
+-rw-r--r--   0        0        0      685 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/mixin.py
+-rw-r--r--   0        0        0      796 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/__init__.py
+-rw-r--r--   0        0        0    19993 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/data.py
+-rw-r--r--   0        0        0     5021 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/service.py
+-rw-r--r--   0        0        0     5380 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/service_types.py
+-rw-r--r--   0        0        0      703 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/types.py
+-rw-r--r--   0        0        0      717 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/status_flags.py
+-rw-r--r--   0        0        0     4067 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/pdu.py
+-rw-r--r--   0        0        0    20539 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/__init__.py
+-rw-r--r--   0        0        0     3494 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/statuscodes.py
+-rw-r--r--   0        0        0     8483 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/tlv.py
+-rw-r--r--   0        0        0        0 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/py.typed
+-rw-r--r--   0        0        0    12836 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/testing.py
+-rw-r--r--   0        0        0     8265 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/tlv8.py
+-rw-r--r--   0        0        0     3581 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/utils.py
+-rw-r--r--   0        0        0     1662 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/uuid.py
+-rw-r--r--   0        0        0    11606 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/zeroconf.py
+-rw-r--r--   0        0        0     1809 2023-06-01 21:57:55.270367 aiohomekit-2.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.4/PKG-INFO
```

### Comparing `aiohomekit-2.6.3/LICENSE.md` & `aiohomekit-2.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/README.md` & `aiohomekit-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/__init__.py` & `aiohomekit-2.6.4/aiohomekit/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/__main__.py` & `aiohomekit-2.6.4/aiohomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/characteristic_cache.py` & `aiohomekit-2.6.4/aiohomekit/characteristic_cache.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/const.py` & `aiohomekit-2.6.4/aiohomekit/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/__init__.py` & `aiohomekit-2.6.4/aiohomekit/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/abstract.py` & `aiohomekit-2.6.4/aiohomekit/controller/abstract.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/__init__.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/bleak.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/bleak.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/client.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/client.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/connection.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/const.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/controller.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/discovery.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/key.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/key.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/manufacturer_data.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/manufacturer_data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/pairing.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/structs.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ble/values.py` & `aiohomekit-2.6.4/aiohomekit/controller/ble/values.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/__init__.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/connection.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/controller.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/discovery.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/pairing.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/pdu.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/coap/structs.py` & `aiohomekit-2.6.4/aiohomekit/controller/coap/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/controller.py` & `aiohomekit-2.6.4/aiohomekit/controller/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ip/__init__.py` & `aiohomekit-2.6.4/aiohomekit/controller/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ip/connection.py` & `aiohomekit-2.6.4/aiohomekit/controller/ip/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,21 @@
 
         self._connect_lock = asyncio.Lock()
 
         self._concurrency_limit = asyncio.Semaphore(concurrency_limit)
         self._reconnect_wait_task = None
 
     @property
+    def name(self):
+        """Return the name of the connection."""
+        if self.owner:
+            return self.owner.name
+        return f"{self.host}:{self.port}"
+
+    @property
     def is_connected(self):
         return self.transport and self.protocol and not self.closed
 
     def _start_connector(self):
         """
         Start a reconnect background task.
 
@@ -420,15 +427,15 @@
         buffer.append(f"{method.upper()} {target} HTTP/1.1")
 
         # WARNING: It is vital that a Host: header is present or some devices
         # will reject the request.
         buffer.append(f"Host: {self.host}")
 
         if headers:
-            for (header, value) in headers:
+            for header, value in headers:
                 buffer.append(f"{header}: {value}")
 
         buffer.append("")
         buffer.append("")
 
         # WARNING: We use \r\n explicitly. \n is not enough for some.
         request_bytes = "\r\n".join(buffer).encode("utf-8")
@@ -523,34 +530,38 @@
         if self._connect_lock.locked():
             # Reconnect already in progress.
             return
         async with self._connect_lock:
             interval = 0.5
 
             logger.debug("Starting reconnect loop to %s:%s", self.host, self.port)
+
             while not self.closing:
                 try:
                     return await self._connect_once()
 
                 except AuthenticationError:
                     # Authentication errors should bubble up because auto-reconnect is unlikely to help
                     raise
 
                 except asyncio.CancelledError:
                     return
 
-                except HomeKitException:
+                except HomeKitException as ex:
                     logger.debug(
-                        "Connecting to accessory failed. Retrying in %i seconds",
+                        "%s: Connecting to accessory failed: %s; Retrying in %i seconds",
+                        self.name,
+                        ex,
                         interval,
                     )
 
                 except Exception:
                     logger.exception(
-                        "Unexpected error whilst trying to connect to accessory. Will retry."
+                        "%s: Unexpected error whilst trying to connect to accessory. Will retry.",
+                        self.name,
                     )
 
                 interval = min(60, 1.5 * interval)
                 self._reconnect_wait_task = asyncio.ensure_future(
                     asyncio.sleep(interval)
                 )
 
@@ -600,23 +611,25 @@
         self.is_secure = False
 
         if self.owner and self.owner.description:
             pairing: IpPairing = self.owner
             try:
                 if self.host != pairing.description.address:
                     logger.debug(
-                        "Host changed from %s to %s",
+                        "%s: Host changed from %s to %s",
+                        pairing.name,
                         self.host,
                         pairing.description.address,
                     )
                     self.host = pairing.description.address
 
                 if self.port != pairing.description.port:
                     logger.debug(
-                        "Port changed from %s to %s",
+                        "%s: Port changed from %s to %s",
+                        pairing.name,
                         self.port,
                         pairing.description.port,
                     )
                     self.port = pairing.description.port
             except AccessoryNotFoundError:
                 pass
```

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ip/controller.py` & `aiohomekit-2.6.4/aiohomekit/controller/ip/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ip/discovery.py` & `aiohomekit-2.6.4/aiohomekit/controller/ip/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/controller/ip/pairing.py` & `aiohomekit-2.6.4/aiohomekit/controller/ip/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/crypto/__init__.py` & `aiohomekit-2.6.4/aiohomekit/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/crypto/chacha20poly1305.py` & `aiohomekit-2.6.4/aiohomekit/crypto/chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/crypto/hkdf.py` & `aiohomekit-2.6.4/aiohomekit/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/crypto/srp.py` & `aiohomekit-2.6.4/aiohomekit/crypto/srp.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/debounce.py` & `aiohomekit-2.6.4/aiohomekit/debounce.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/enum.py` & `aiohomekit-2.6.4/aiohomekit/enum.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/exceptions.py` & `aiohomekit-2.6.4/aiohomekit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/hkjson.py` & `aiohomekit-2.6.4/aiohomekit/hkjson.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/http/__init__.py` & `aiohomekit-2.6.4/aiohomekit/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/http/response.py` & `aiohomekit-2.6.4/aiohomekit/http/response.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/meshcop.py` & `aiohomekit-2.6.4/aiohomekit/meshcop.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/__init__.py` & `aiohomekit-2.6.4/aiohomekit/model/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/categories.py` & `aiohomekit-2.6.4/aiohomekit/model/categories.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/__init__.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic_formats.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_formats.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/characteristic_types.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/const.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,14 +95,31 @@
     """Possible values for the current status of an accessory.
     https://developer.apple.com/documentation/homekit/hmcharacteristicvalueactivationstate"""
 
     INACTIVE = 0
     ACTIVE = 1
 
 
+class CurrentAirPurifierStateValues(enum.IntEnum):
+    """Possible values for the current state of an air purifier.
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluecurrentairpurifierstate"""
+
+    INACTIVE = 0
+    IDLE = 1
+    ACTIVE = 2
+
+
+class TargetAirPurifierStateValues(enum.IntEnum):
+    """Possible values for the target state  of an air purifier.
+    https://developer.apple.com/documentation/homekit/hmcharacteristicvaluetargetairpurifierstate"""
+
+    MANUAL = 0
+    AUTOMATIC = 1
+
+
 class SwingModeValues(enum.IntEnum):
     """Possible values for fan movement.
     https://developer.apple.com/documentation/homekit/hmcharacteristicvalueswingmode"""
 
     DISABLED = 0
     ENABLED = 1
```

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/data.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/permissions.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/permissions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/structs.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/types.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/characteristics/units.py` & `aiohomekit-2.6.4/aiohomekit/model/characteristics/units.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/entity_map.py` & `aiohomekit-2.6.4/aiohomekit/model/entity_map.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/feature_flags.py` & `aiohomekit-2.6.4/aiohomekit/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/mixin.py` & `aiohomekit-2.6.4/aiohomekit/model/mixin.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/services/__init__.py` & `aiohomekit-2.6.4/aiohomekit/model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/services/data.py` & `aiohomekit-2.6.4/aiohomekit/model/services/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/services/service.py` & `aiohomekit-2.6.4/aiohomekit/model/services/service.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/services/service_types.py` & `aiohomekit-2.6.4/aiohomekit/model/services/service_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/services/types.py` & `aiohomekit-2.6.4/aiohomekit/model/services/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/model/status_flags.py` & `aiohomekit-2.6.4/aiohomekit/model/status_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/pdu.py` & `aiohomekit-2.6.4/aiohomekit/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/protocol/__init__.py` & `aiohomekit-2.6.4/aiohomekit/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/protocol/statuscodes.py` & `aiohomekit-2.6.4/aiohomekit/protocol/statuscodes.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/protocol/tlv.py` & `aiohomekit-2.6.4/aiohomekit/protocol/tlv.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/testing.py` & `aiohomekit-2.6.4/aiohomekit/testing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/tlv8.py` & `aiohomekit-2.6.4/aiohomekit/tlv8.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/utils.py` & `aiohomekit-2.6.4/aiohomekit/utils.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/uuid.py` & `aiohomekit-2.6.4/aiohomekit/uuid.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/aiohomekit/zeroconf.py` & `aiohomekit-2.6.4/aiohomekit/zeroconf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.3/pyproject.toml` & `aiohomekit-2.6.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohomekit"
-version = "2.6.3"
+version = "2.6.4"
 description = "An asyncio HomeKit client"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Jc2k/aiohomekit"
 repository = "https://github.com/Jc2k/aiohomekit"
 keywords = ["HomeKit", "home", "automation"]
@@ -34,15 +34,14 @@
 [tool.poetry.dev-dependencies]
 isort = "^5.10.1"
 mypy = "^0.931"
 black = "^22.1.0"
 flake8 = "^4.0.1"
 pytest = "^6.2.5"
 coverage = "^6.3"
-codecov = "^2.1.12"
 pylint = "^2.12.2"
 pytest-aiohttp = "^1.0.3"
 pyupgrade = "^2.31.0"
 pytest-cov = "^3.0.0"
 asynctest = "^0.13.0"
 aiohttp = ">=3.8.3"
```

### Comparing `aiohomekit-2.6.3/PKG-INFO` & `aiohomekit-2.6.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: aiohomekit
-Version: 2.6.3
+Version: 2.6.4
 Summary: An asyncio HomeKit client
 Home-page: https://github.com/Jc2k/aiohomekit
 License: Apache-2.0
 Keywords: HomeKit,home,automation
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Home Automation
 Requires-Dist: aiocoap (>=0.4.5)
 Requires-Dist: async-timeout (>=4.0.2,<5.0.0)
 Requires-Dist: bleak (>=0.19.0)
 Requires-Dist: bleak-retry-connector (>=2.9.0)
 Requires-Dist: chacha20poly1305 (>=0.0.3,<0.0.4)
 Requires-Dist: chacha20poly1305-reuseable (>=0.0.4)
```

