# Comparing `tmp/cloudshell-snmp-5.0.1.zip` & `tmp/cloudshell-snmp-5.0.2.zip`

## zipinfo {}

```diff
@@ -1,117 +1,117 @@
-Zip file size: 145763 bytes, number of entries: 115
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/
--rw-r--r--  2.0 unx    11560 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/LICENSE
--rw-r--r--  2.0 unx      277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/PKG-INFO
--rw-r--r--  2.0 unx     1068 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tox.ini
--rw-r--r--  2.0 unx      855 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/setup.py
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/dev_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/setup.cfg
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/version.txt
--rw-r--r--  2.0 unx       58 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/MANIFEST.in
--rw-r--r--  2.0 unx       74 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/requirements.txt
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/README.txt
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/test_requirements.txt
--rw-r--r--  2.0 unx       52 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/third_party_requirements.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/
--rw-r--r--  2.0 unx      778 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/types.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/__init__.py
--rw-r--r--  2.0 unx     2623 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py
--rw-r--r--  2.0 unx     5256 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py
--rw-r--r--  2.0 unx     6863 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/
--rw-r--r--  2.0 unx      349 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_errors.py
--rw-r--r--  2.0 unx      375 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
--rw-r--r--  2.0 unx    12397 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py
--rw-r--r--  2.0 unx     2549 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/__init__.py
--rw-r--r--  2.0 unx     8876 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py
--rw-r--r--  2.0 unx     1354 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py
--rw-r--r--  2.0 unx    14033 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/__init__.py
--rw-r--r--  2.0 unx     2501 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py
--rw-r--r--  2.0 unx     4281 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py
--rw-r--r--  2.0 unx     1385 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py
--rw-r--r--  2.0 unx     2929 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py
--rw-r--r--  2.0 unx     1997 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py
--rw-r--r--  2.0 unx     1122 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py
--rw-r--r--  2.0 unx     1947 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/__init__.py
--rw-r--r--  2.0 unx     1297 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py
--rw-r--r--  2.0 unx    13419 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py
--rw-r--r--  2.0 unx     2600 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py
--rw-r--r--  2.0 unx     1327 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
--rw-r--r--  2.0 unx     2920 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
--rw-r--r--  2.0 unx    37281 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json
--rw-r--r--  2.0 unx     7637 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py
--rw-r--r--  2.0 unx     4368 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
--rw-r--r--  2.0 unx      611 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
--rw-r--r--  2.0 unx    30835 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json
--rw-r--r--  2.0 unx     2597 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json
--rw-r--r--  2.0 unx     6071 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
--rw-r--r--  2.0 unx      416 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
--rw-r--r--  2.0 unx    24807 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
--rw-r--r--  2.0 unx    21756 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json
--rw-r--r--  2.0 unx     7929 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
--rw-r--r--  2.0 unx   116385 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json
--rw-r--r--  2.0 unx    34416 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json
--rw-r--r--  2.0 unx    32561 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json
--rw-r--r--  2.0 unx    16818 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json
--rw-r--r--  2.0 unx    42496 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__init__.py
--rw-r--r--  2.0 unx    67738 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json
--rw-r--r--  2.0 unx    42211 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
--rw-r--r--  2.0 unx     3398 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py
--rw-r--r--  2.0 unx     6501 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
--rw-r--r--  2.0 unx    90974 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json
--rw-r--r--  2.0 unx    33327 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
--rw-r--r--  2.0 unx    34783 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json
--rw-r--r--  2.0 unx     4092 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py
--rw-r--r--  2.0 unx      162 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
--rw-r--r--  2.0 unx   110034 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json
--rw-r--r--  2.0 unx    24494 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json
--rw-r--r--  2.0 unx    59229 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
--rw-r--r--  2.0 unx      386 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1.py
--rw-r--r--  2.0 unx    23277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json
--rw-r--r--  2.0 unx       73 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/requires.txt
--rw-r--r--  2.0 unx      277 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3574 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/build/
--rw-r--r--  2.0 unx      515 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/.tox/build/.tox-info.json
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/
--rw-r--r--  2.0 unx     8054 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/__init__.py
--rw-r--r--  2.0 unx     6347 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py
--rw-r--r--  2.0 unx     4989 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/__init__.py
--rw-r--r--  2.0 unx     3288 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/__init__.py
--rw-r--r--  2.0 unx     1809 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py
--rw-r--r--  2.0 unx     1245 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py
--rw-r--r--  2.0 unx     1614 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py
--rw-r--r--  2.0 unx     6670 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py
--rw-r--r--  2.0 unx     2786 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py
--rw-r--r--  2.0 unx       79 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/__init__.py
--rw-r--r--  2.0 unx     2032 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py
--rw-r--r--  2.0 unx     7478 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py
--rw-r--r--  2.0 unx     6945 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/__init__.py
--rw-r--r--  2.0 unx     1131 b- defN 23-Apr-21 23:48 cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py
-115 files, 1057791 bytes uncompressed, 124417 bytes compressed:  88.2%
+Zip file size: 145842 bytes, number of entries: 115
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/.tox/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/setup.cfg
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tox.ini
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/version.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/test_requirements.txt
+-rw-r--r--  2.0 unx       58 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/MANIFEST.in
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/README.txt
+-rw-r--r--  2.0 unx       52 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/third_party_requirements.txt
+-rw-r--r--  2.0 unx    11560 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/LICENSE
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/requirements.txt
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/PKG-INFO
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/dev_requirements.txt
+-rw-r--r--  2.0 unx      855 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/setup.py
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     3574 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/configurator/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/
+-rw-r--r--  2.0 unx     8054 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/test_snmp_parameters.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/__init__.py
+-rw-r--r--  2.0 unx     6347 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/test_snmp_context_manager.py
+-rw-r--r--  2.0 unx     4989 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/test_cloudshell_snmp.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/configurator/__init__.py
+-rw-r--r--  2.0 unx     6945 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/configurator/test_snmp_configurator.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/__init__.py
+-rw-r--r--  2.0 unx     3288 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/test_snmp_service.py
+-rw-r--r--  2.0 unx     2786 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_mib_builder.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/__init__.py
+-rw-r--r--  2.0 unx     7478 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib.py
+-rw-r--r--  2.0 unx     6670 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib_parser.py
+-rw-r--r--  2.0 unx     2032 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_transport.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/__init__.py
+-rw-r--r--  2.0 unx     1809 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_record.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_snmp_response.py
+-rw-r--r--  2.0 unx     1614 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_quali_mib_table.py
+-rw-r--r--  2.0 unx     1245 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_type_record.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/
+-rw-r--r--  2.0 unx     6863 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_parameters.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/__init__.py
+-rw-r--r--  2.0 unx      778 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/types.py
+-rw-r--r--  2.0 unx     2623 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/cloudshell_snmp.py
+-rw-r--r--  2.0 unx     5251 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_configurator.py
+-rw-r--r--  2.0 unx     7929 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
+-rw-r--r--  2.0 unx     4092 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-CONF.py
+-rw-r--r--  2.0 unx     2920 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
+-rw-r--r--  2.0 unx    67738 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RFC1271-MIB.json
+-rw-r--r--  2.0 unx    16818 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-MAU-MIB.json
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__init__.py
+-rw-r--r--  2.0 unx    32561 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/BRIDGE-MIB.json
+-rw-r--r--  2.0 unx      162 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
+-rw-r--r--  2.0 unx      386 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1.py
+-rw-r--r--  2.0 unx     3398 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-MIB.py
+-rw-r--r--  2.0 unx    34416 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-MIB.json
+-rw-r--r--  2.0 unx    59229 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
+-rw-r--r--  2.0 unx    42211 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
+-rw-r--r--  2.0 unx    90974 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON-MIB.json
+-rw-r--r--  2.0 unx    42496 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/LLDP-MIB.json
+-rw-r--r--  2.0 unx    30835 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/EtherLike-MIB.json
+-rw-r--r--  2.0 unx      611 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
+-rw-r--r--  2.0 unx     6071 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-TC.json
+-rw-r--r--  2.0 unx     4368 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
+-rw-r--r--  2.0 unx      416 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
+-rw-r--r--  2.0 unx   116385 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON2-MIB.json
+-rw-r--r--  2.0 unx    34783 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/MAU-MIB.json
+-rw-r--r--  2.0 unx    23277 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-MIB.json
+-rw-r--r--  2.0 unx     6501 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
+-rw-r--r--  2.0 unx    21756 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANAifType-MIB.json
+-rw-r--r--  2.0 unx    24807 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
+-rw-r--r--  2.0 unx    33327 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
+-rw-r--r--  2.0 unx     7637 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__SNMPv2-MIB.py
+-rw-r--r--  2.0 unx    37281 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IF-MIB.json
+-rw-r--r--  2.0 unx    24494 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ENTITY-MIB.json
+-rw-r--r--  2.0 unx   110034 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IP-MIB.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/
+-rw-r--r--  2.0 unx    14443 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_service.py
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
+-rw-r--r--  2.0 unx     8876 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_response_reader.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/__init__.py
+-rw-r--r--  2.0 unx      349 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_errors.py
+-rw-r--r--  2.0 unx     1354 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_context_manager.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_engine.py
+-rw-r--r--  2.0 unx    12160 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_view_controller.py
+-rw-r--r--  2.0 unx     2549 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_mib_builder.py
+-rw-r--r--  2.0 unx      992 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_constants.py
+-rw-r--r--  2.0 unx    13419 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/__init__.py
+-rw-r--r--  2.0 unx     1297 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_security.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_parameters_helper.py
+-rw-r--r--  2.0 unx     2600 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_trasnport.py
+-rw-r--r--  2.0 unx     1122 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_context.py
+-rw-r--r--  2.0 unx     1327 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
+-rw-r--r--  2.0 unx     1947 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/mib_builder_helper.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/__init__.py
+-rw-r--r--  2.0 unx     2501 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/quali_mib_table.py
+-rw-r--r--  2.0 unx     4281 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_oid.py
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_json_record.py
+-rw-r--r--  2.0 unx     2967 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_response.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 15:44 cloudshell-snmp-5.0.2/.tox/build/
+-rw-r--r--  2.0 unx      515 b- defN 23-Jun-02 15:44 cloudshell-snmp-5.0.2/.tox/build/.tox-info.json
+115 files, 1057992 bytes uncompressed, 124496 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -1,346 +1,346 @@
-Filename: cloudshell-snmp-5.0.1/
+Filename: cloudshell-snmp-5.0.2/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/
+Filename: cloudshell-snmp-5.0.2/tests/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/.tox/
+Filename: cloudshell-snmp-5.0.2/cloudshell/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/
+Filename: cloudshell-snmp-5.0.2/.tox/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/LICENSE
+Filename: cloudshell-snmp-5.0.2/setup.cfg
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/PKG-INFO
+Filename: cloudshell-snmp-5.0.2/tox.ini
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tox.ini
+Filename: cloudshell-snmp-5.0.2/version.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/setup.py
+Filename: cloudshell-snmp-5.0.2/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/dev_requirements.txt
+Filename: cloudshell-snmp-5.0.2/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/setup.cfg
+Filename: cloudshell-snmp-5.0.2/README.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/version.txt
+Filename: cloudshell-snmp-5.0.2/third_party_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/MANIFEST.in
+Filename: cloudshell-snmp-5.0.2/LICENSE
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/requirements.txt
+Filename: cloudshell-snmp-5.0.2/requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/README.txt
+Filename: cloudshell-snmp-5.0.2/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/test_requirements.txt
+Filename: cloudshell-snmp-5.0.2/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/third_party_requirements.txt
+Filename: cloudshell-snmp-5.0.2/setup.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/types.py
+Filename: cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py
+Filename: cloudshell-snmp-5.0.2/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/configurator/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/
+Filename: cloudshell-snmp-5.0.2/tests/snmp/test_snmp_parameters.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/
+Filename: cloudshell-snmp-5.0.2/tests/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_errors.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/test_snmp_context_manager.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/test_cloudshell_snmp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/configurator/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/__init__.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/configurator/test_snmp_configurator.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/test_snmp_service.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/__init__.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_mib_builder.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib_parser.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_transport.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_snmp_response.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_quali_mib_table.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/__init__.py
+Filename: cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_type_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_parameters.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/types.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/cloudshell_snmp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_configurator.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-CONF.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RFC1271-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-MAU-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/LLDP-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/EtherLike-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-TC.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ASN1-REFINEMENT.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1-ENUMERATION.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON2-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/MAU-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ASN1.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANAifType-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/P-BRIDGE-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/requires.txt
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/PKG-INFO
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__SNMPv2-MIB.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/dependency_links.txt
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IF-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/top_level.txt
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ENTITY-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IP-MIB.json
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/.tox/build/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/.tox/build/.tox-info.json
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_service.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_msg_pdu_dsp.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_response_reader.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_errors.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_context_manager.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_engine.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_view_controller.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_mib_builder.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_security.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_parameters_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_trasnport.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_context.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib_parser.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/mib_builder_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/__init__.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/quali_mib_table.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_oid.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_json_record.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py
+Filename: cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_response.py
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/__init__.py
+Filename: cloudshell-snmp-5.0.2/.tox/build/
 Comment: 
 
-Filename: cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py
+Filename: cloudshell-snmp-5.0.2/.tox/build/.tox-info.json
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-snmp-5.0.1/LICENSE` & `cloudshell-snmp-5.0.2/LICENSE`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tox.ini` & `cloudshell-snmp-5.0.2/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/setup.py` & `cloudshell-snmp-5.0.2/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/types.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/types.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/cloudshell_snmp.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/cloudshell_snmp.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_configurator.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         """Disable snmp service."""
         if self._disable:
             self._logger.debug("Calling disable snmp flow")
             self._enable_disable_flow.disable_snmp(self._snmp_parameters)
         self._snmp_manager.__exit__(exc_type, exc_val, exc_tb)
 
 
-class EnableDisableSnmpConfigurator(ABC):
+class EnableDisableSnmpConfigurator:
     def __init__(
         self,
         enable_disable_snmp_flow: EnableDisableSnmpFlowInterface,
         snmp_parameters: SnmpParameters,
         enable_snmp: bool,
         disable_snmp: bool,
         logger: Logger,
```

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/snmp_parameters.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/snmp_parameters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_view_controller.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_view_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,33 +188,28 @@
         )
         if oid == label:
             raise NoSuchObjectError(
                 str="Can't resolve node name {}::{} at {}".format(
                     modName, nodeName, self
                 )
             )
-        self._logger.debug(
-            "getNodeNameByOid: resolved %s:%s -> %s.%s"
-            % (modName, nodeName, label, suffix)
-        )
         return oid, label, suffix
 
     def getNodeNameByDesc(self, nodeName, modName=""):
         self.index_mib()
         if modName in self._mibSymbolsIdx:
             mibMod = self._mibSymbolsIdx[modName]
         else:
             raise SmiError(f"No module {modName} at {self}")
         if nodeName in mibMod["varToNameIdx"]:
             oid = mibMod["varToNameIdx"][nodeName]
         else:
             raise NoSuchObjectError(
                 str=f"No such symbol {modName}::{nodeName} at {self}"
             )
-        self._logger.debug(f"getNodeNameByDesc: resolved {modName}:{nodeName} -> {oid}")
         return self.getNodeNameByOid(oid, modName)
 
     def getNodeName(self, nodeName, modName=""):
         try:
             return self.getNodeNameByOid(nodeName, modName)
         except NoSuchObjectError:
             oid, label, suffix = self.getNodeNameByDesc(nodeName[0], modName)
```

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_mib_builder.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_mib_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_response_reader.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_response_reader.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_engine.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_engine.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_context_manager.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/snmp_service.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/snmp_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 import os
 import time
 
 from pyasn1.type import univ
-from pysnmp.proto.errind import requestTimedOut
+from pysnmp.proto.errind import RequestTimedOut, requestTimedOut
 
 from cloudshell.snmp.core.domain.quali_mib_table import QualiMibTable
+from cloudshell.snmp.core.domain.snmp_oid import SnmpMibObject, SnmpRawOid
 from cloudshell.snmp.core.domain.snmp_response import SnmpResponse
 from cloudshell.snmp.core.snmp_errors import GeneralSNMPException, ReadSNMPException
 from cloudshell.snmp.core.snmp_response_reader import SnmpResponseReader
 from cloudshell.snmp.core.tools.mib_builder_helper import QualiDirMibSource
 
 
 class SnmpService:
@@ -129,38 +132,37 @@
 
         self._start_dispatcher()
 
         self._check_error(service.cb_ctx, service.result)
 
         return service.result
 
-    def get_property(self, snmp_oid):
+    def get_property(self, snmp_oid: SnmpMibObject | SnmpRawOid) -> SnmpResponse:
         response = SnmpResponse(
             str(snmp_oid.get_oid(self._snmp_engine)),
             None,
             snmp_engine=self._snmp_engine,
             logger=self._logger,
         )
         try:
             return self.get(snmp_oid) or response
         except ReadSNMPException as e:
             self._logger.debug(e, exc_info=True)
 
         return response
 
-    def get(self, snmp_oid):
+    def get(self, snmp_oid: SnmpMibObject | SnmpRawOid) -> SnmpResponse | None:
         """Get snmp operation.
 
         Load appropriate oid value from the device.
         :param snmp_oid: Single SnmpMibOid or SnmpRawOid object.
             For example, an object to get sysContact can by any of the following:
             SnmpMibOid('SNMPv2-MIB', 'sysContact', 0)
             SnmpMibOid('SNMPv2-MIB', 'sysContact')
             SnmpRawOid('1.3.6.1.2.1.1.4.0')
-        :return: SnmpResponse
         """
         oid = snmp_oid.get_oid(self._snmp_engine)
         if hasattr(oid, "index") and not oid.index:
             oid.index = 0
 
         service = self._create_response_service()
         service.send_get_var_binds(oid=oid)
@@ -336,52 +338,53 @@
 
         result_dict = QualiMibTable.create_from_list(table_name, result_list)
 
         return result_dict
 
     def get_multiple_columns(
         self,
-        snmp_oid_obj_list,
-        retry_count=WALK_RETRY_COUNT,
-        get_bulk_flag=None,
-        get_bulk_repetitions=DEFAULT_GET_BULK_REPETITIONS,
-    ):
+        snmp_oid_obj_list: list[SnmpMibObject | SnmpRawOid],
+        retry_count: int = WALK_RETRY_COUNT,
+        get_bulk_flag: bool | None = None,
+        get_bulk_repetitions: int = DEFAULT_GET_BULK_REPETITIONS,
+    ) -> QualiMibTable:
         """Get multiple columns from the table. Based on a walk command.
 
         Load list of appropriate oid values from the device.
         :param get_bulk_repetitions: Specifies amount of entries to be read in
         a single request
         :param get_bulk_flag: Specifies if get_bulk should be used or not
         :param retry_count: Amount of retires to retrieve required data
         :param snmp_oid_obj_list: List of SnmpMibOid or SnmpRawOid objects.
             For example, an object to get sysContact can by any of the following:
             [
             SnmpMibOid('IF-MIB', 'ifName'),
             SnmpMibOid('IF-MIB', 'ifPhysicalAddress'),
             etc.
             ]
-
-        :return: QualiMibTable
         """
         result_list = []
         table_name = (
             snmp_oid_obj_list[0]
             .get_object_type(snmp_engine=self._snmp_engine)[0]
             .getMibSymbol()[1]
         )
         for snmp_oid_obj in snmp_oid_obj_list:
-            result_list.extend(
-                self._walk(
-                    snmp_oid_obj,
-                    get_subtree=True,
-                    retry_count=retry_count,
-                    get_bulk_flag=get_bulk_flag,
-                    get_bulk_repetitions=get_bulk_repetitions,
+            try:
+                result_list.extend(
+                    self._walk(
+                        snmp_oid_obj,
+                        get_subtree=True,
+                        retry_count=retry_count,
+                        get_bulk_flag=get_bulk_flag,
+                        get_bulk_repetitions=get_bulk_repetitions,
+                    )
                 )
-            )
+            except RequestTimedOut as e:
+                self._logger.error(f"Error retrieving snmp response: {e}")
 
         result_dict = QualiMibTable.create_from_list(table_name, result_list)
 
         return result_dict
 
     def _create_response_service(
         self, cb_ctx=None, retry_count=0, get_bulk_flag=False, get_bulk_repetitions=None
```

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/quali_mib_table.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/quali_mib_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_oid.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_oid.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_json_record.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_json_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/domain/snmp_response.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/domain/snmp_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pysnmp.error import PySnmpError
 from pysnmp.hlapi.varbinds import CommandGeneratorVarBinds
 from pysnmp.smi.error import SmiError
 
 from cloudshell.snmp.core.snmp_errors import TranslateSNMPException
```

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_parameters_helper.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_parameters_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_context.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_context.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_constants.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_constants.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/mib_builder_helper.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/mib_builder_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_security.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_security.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_trasnport.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_trasnport.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/core/tools/snmp_json_mib_parser.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/core/tools/snmp_json_mib_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-ADDRESS-FAMILY-NUMBERS-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IF-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IF-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__SNMPv2-MIB.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__SNMPv2-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-SOURCE-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/__PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/EtherLike-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/EtherLike-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-TC.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-TC.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/INET-ADDRESS-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/P-BRIDGE-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/P-BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANAifType-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANAifType-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-USM-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON2-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON2-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IPV6-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IPV6-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/BRIDGE-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IANA-MAU-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IANA-MAU-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/LLDP-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/LLDP-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RFC1271-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RFC1271-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/Q-BRIDGE-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/PYSNMP-MIB.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/PYSNMP-MIB.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMP-FRAMEWORK-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/RMON-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/RMON-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IEEE8023-LAG-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/MAU-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/MAU-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-CONF.py` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-CONF.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/IP-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/IP-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/ENTITY-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/ENTITY-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/TOKEN-RING-RMON-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell/snmp/mibs/SNMPv2-MIB.json` & `cloudshell-snmp-5.0.2/cloudshell/snmp/mibs/SNMPv2-MIB.json`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/cloudshell_snmp.egg-info/SOURCES.txt` & `cloudshell-snmp-5.0.2/cloudshell_snmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/.tox/build/.tox-info.json` & `cloudshell-snmp-5.0.2/.tox/build/.tox-info.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9722222222222223%*

 * *Differences: {"'Python'": "{'virtualenv version': '20.23.0'}"}*

```diff
@@ -4,15 +4,15 @@
         "version_info": [
             3,
             9,
             16,
             "final",
             0
         ],
-        "virtualenv version": "20.22.0"
+        "virtualenv version": "20.23.0"
     },
     "PythonRun": {
         "deps": {
             "constraint_options": {
                 "constrain_package_deps": false,
                 "use_frozen_constraints": false
             },
```

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/test_snmp_parameters.py` & `cloudshell-snmp-5.0.2/tests/snmp/test_snmp_parameters.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/test_snmp_context_manager.py` & `cloudshell-snmp-5.0.2/tests/snmp/test_snmp_context_manager.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/test_cloudshell_snmp.py` & `cloudshell-snmp-5.0.2/tests/snmp/test_cloudshell_snmp.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/test_snmp_service.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/test_snmp_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_snmp_response.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_snmp_response.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_record.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_json_type_record.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_json_type_record.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/domain/test_quali_mib_table.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/domain/test_quali_mib_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib_parser.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib_parser.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_mib_builder.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_mib_builder.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_transport.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_transport.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/core/tools/test_snmp_json_mib.py` & `cloudshell-snmp-5.0.2/tests/snmp/core/tools/test_snmp_json_mib.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/configurator/test_enable_disable_snmp_configurator.py` & `cloudshell-snmp-5.0.2/tests/snmp/configurator/test_enable_disable_snmp_configurator.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-5.0.1/tests/snmp/configurator/test_snmp_configurator.py` & `cloudshell-snmp-5.0.2/tests/snmp/configurator/test_snmp_configurator.py`

 * *Files identical despite different names*

