# Comparing `tmp/cloudshell-shell-connectivity-flow-3.2.1.zip` & `tmp/cloudshell-shell-connectivity-flow-4.0.0.zip`

## zipinfo {}

```diff
@@ -1,65 +1,65 @@
-Zip file size: 32887 bytes, number of entries: 63
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/
--rw-r--r--  2.0 unx       34 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/MANIFEST.in
--rw-r--r--  2.0 unx     1152 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tox.ini
--rw-r--r--  2.0 unx       71 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/dev_requirements.txt
--rw-r--r--  2.0 unx      924 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/README.md
--rw-r--r--  2.0 unx      337 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/PKG-INFO
--rw-r--r--  2.0 unx       29 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/test_requirements.txt
--rw-r--r--  2.0 unx      896 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/setup.py
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/version.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/setup.cfg
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/requirements.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/
--rw-r--r--  2.0 unx     2384 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/__init__.py
--rw-r--r--  2.0 unx    10203 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py
--rw-r--r--  2.0 unx     5160 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/conftest.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py
--rw-r--r--  2.0 unx     2672 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py
--rw-r--r--  2.0 unx     3706 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/__init__.py
--rw-r--r--  2.0 unx     1290 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/__init__.py
--rw-r--r--  2.0 unx     3199 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py
--rw-r--r--  2.0 unx     1468 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/
--rw-r--r--  2.0 unx     2862 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/parse_request_service.py
--rw-r--r--  2.0 unx       79 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/__init__.py
--rw-r--r--  2.0 unx     4110 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/basic_flow.py
--rw-r--r--  2.0 unx      246 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/exceptions.py
--rw-r--r--  2.0 unx     2470 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/simple_flow.py
--rw-r--r--  2.0 unx     2171 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py
--rw-r--r--  2.0 unx     1515 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py
--rw-r--r--  2.0 unx      808 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py
--rw-r--r--  2.0 unx     3698 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/__init__.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/__init__.py
--rw-r--r--  2.0 unx     2499 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/connectivity_model.py
--rw-r--r--  2.0 unx     1584 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/driver_response.py
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2218 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      337 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       47 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-14 14:57 cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/top_level.txt
-63 files, 62579 bytes uncompressed, 17663 bytes compressed:  71.8%
+Zip file size: 32831 bytes, number of entries: 63
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/setup.cfg
+-rw-r--r--  2.0 unx     1281 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tox.ini
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/version.txt
+-rw-r--r--  2.0 unx       29 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/test_requirements.txt
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/requirements.txt
+-rw-r--r--  2.0 unx      337 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/PKG-INFO
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx      896 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/setup.py
+-rw-r--r--  2.0 unx      924 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/README.md
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     2218 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      337 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/
+-rw-r--r--  2.0 unx     2384 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py
+-rw-r--r--  2.0 unx     2254 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/__init__.py
+-rw-r--r--  2.0 unx     5064 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/conftest.py
+-rw-r--r--  2.0 unx    10091 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/__init__.py
+-rw-r--r--  2.0 unx     1468 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py
+-rw-r--r--  2.0 unx     3199 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/__init__.py
+-rw-r--r--  2.0 unx     1290 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py
+-rw-r--r--  2.0 unx     2672 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py
+-rw-r--r--  2.0 unx     3706 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/exceptions.py
+-rw-r--r--  2.0 unx       79 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/__init__.py
+-rw-r--r--  2.0 unx     4165 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/basic_flow.py
+-rw-r--r--  2.0 unx     2862 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/parse_request_service.py
+-rw-r--r--  2.0 unx     2217 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/simple_flow.py
+-rw-r--r--  2.0 unx     1584 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/driver_response.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/__init__.py
+-rw-r--r--  2.0 unx     2499 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/connectivity_model.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/__init__.py
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py
+-rw-r--r--  2.0 unx     2171 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py
+-rw-r--r--  2.0 unx      808 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py
+-rw-r--r--  2.0 unx     3698 b- defN 23-Jun-02 11:06 cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py
+63 files, 62284 bytes uncompressed, 17607 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -1,190 +1,190 @@
-Filename: cloudshell-shell-connectivity-flow-3.2.1/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/MANIFEST.in
+Filename: cloudshell-shell-connectivity-flow-4.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tox.ini
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/dev_requirements.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/README.md
+Filename: cloudshell-shell-connectivity-flow-4.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/PKG-INFO
+Filename: cloudshell-shell-connectivity-flow-4.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/test_requirements.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/setup.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/version.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/setup.cfg
+Filename: cloudshell-shell-connectivity-flow-4.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/requirements.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/README.md
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/conftest.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/conftest.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/parse_request_service.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/basic_flow.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/exceptions.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/simple_flow.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/exceptions.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/parse_request_service.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/simple_flow.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/__init__.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/driver_response.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/connectivity_model.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/driver_response.py
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/connectivity_model.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/dependency_links.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/PKG-INFO
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/requires.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/top_level.txt
+Filename: cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tox.ini` & `cloudshell-shell-connectivity-flow-4.0.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 forced_separate = cloudshell.shell.flows.connectivity,tests
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
 ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203
+known_modules = cloudshell-shell-connectivity-flow:[cloudshell.shell.flows.connectivity],cloudshell-logging:[cloudshell.logging]
 
 [coverage:report]
 exclude_lines =
     pragma: no cover
     if TYPE_CHECKING
 omit =
     *__init__*
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/README.md` & `cloudshell-shell-connectivity-flow-4.0.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/setup.py` & `cloudshell-shell-connectivity-flow-4.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_parse_request_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_basic_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 def parse_connectivity_request_service():
     return ParseConnectivityRequestService(
         is_vlan_range_supported=True, is_multi_vlan_supported=True
     )
 
 
 @pytest.fixture()
-def connectivity_flow(parse_connectivity_request_service, logger):
+def connectivity_flow(parse_connectivity_request_service):
     class ConnectivityFlow(AbstractConnectivityFlow):
         IS_SUCCESS = True
 
         def _generic_change_vlan_fn(
             self, action: ConnectivityActionModel
         ) -> ConnectivityActionResult:
             if self.IS_SUCCESS:
@@ -38,15 +38,15 @@
                 )
             else:
                 return ConnectivityActionResult.fail_result(action, "fail")
 
         _set_vlan = _generic_change_vlan_fn
         _remove_vlan = _generic_change_vlan_fn
 
-    return ConnectivityFlow(parse_connectivity_request_service, logger)
+    return ConnectivityFlow(parse_connectivity_request_service)
 
 
 def test_connectivity_flow(connectivity_flow, driver_request):
     res = connectivity_flow.apply_connectivity(json.dumps(driver_request))
     assert res == (
         '{"driverResponse": {"actionResults": [{'
         '"actionId": "96582265-2728-43aa-bc97-cefb2457ca44_0900c4b5-0f90-42e3-b495", '
@@ -171,30 +171,28 @@
         '"infoMessage": "successful", '
         '"errorMessage": "", '
         '"success": true'
         "}]}}"
     )
 
 
-def test_connectivity_flow_abstract_methods(parse_connectivity_request_service, logger):
+def test_connectivity_flow_abstract_methods(parse_connectivity_request_service):
     with pytest.raises(TypeError, match="Can't instantiate abstract class"):
-        AbstractConnectivityFlow(parse_connectivity_request_service, logger)
+        AbstractConnectivityFlow(parse_connectivity_request_service)
 
 
-def test_abstract_methods_raises(
-    parse_connectivity_request_service, logger, action_model
-):
+def test_abstract_methods_raises(parse_connectivity_request_service, action_model):
     class TestClass(AbstractConnectivityFlow):
-        def _set_vlan(self, action: ConnectivityActionModel) -> str:
+        def _set_vlan(self, action: ConnectivityActionModel):
             return super()._set_vlan(action_model)
 
-        def _remove_vlan(self, action: ConnectivityActionModel) -> str:
+        def _remove_vlan(self, action: ConnectivityActionModel):
             return super()._remove_vlan(action_model)
 
-    inst = TestClass(parse_connectivity_request_service, logger)
+    inst = TestClass(parse_connectivity_request_service)
     with pytest.raises(NotImplementedError):
         inst._set_vlan(action_model)
 
     with pytest.raises(NotImplementedError):
         inst._remove_vlan(action_model)
 
 
@@ -225,47 +223,47 @@
     action_results = json.loads(res)["driverResponse"]["actionResults"]
     assert len(action_results) == 1
     assert action_results[0]["success"] is False
     connectivity_flow._set_vlan.assert_not_called()
 
 
 def test_do_run_set_vlan_if_remove_vlan_success(
-    create_networking_action_request, parse_connectivity_request_service, logger
+    create_networking_action_request, parse_connectivity_request_service
 ):
     def return_success_result(action):
         return ConnectivityActionResult.success_result(action, "successful")
 
     class TestedConnectivityFlow(AbstractConnectivityFlow):
         _remove_vlan = Mock(side_effect=return_success_result)
         _set_vlan = Mock(side_effect=return_success_result)
 
     action = create_networking_action_request(set_vlan=True)
     request = create_driver_str_request(action)
 
-    flow = TestedConnectivityFlow(parse_connectivity_request_service, logger)
+    flow = TestedConnectivityFlow(parse_connectivity_request_service)
     res = flow.apply_connectivity(request)
 
     assert res
     flow._remove_vlan.assert_called_once()
     flow._set_vlan.assert_called_once()
 
 
 def test_failed_response_if_remove_vlan_failed(
-    create_networking_action_request, parse_connectivity_request_service, logger
+    create_networking_action_request, parse_connectivity_request_service
 ):
     class TestedConnectivityFlow(AbstractConnectivityFlow):
-        def _remove_vlan(self, action: ConnectivityActionModel) -> str:
+        def _remove_vlan(self, a: ConnectivityActionModel):
             1 / 0
 
         _set_vlan = None
 
     action = create_networking_action_request(set_vlan=False)
     request = create_driver_str_request(action)
 
-    flow = TestedConnectivityFlow(parse_connectivity_request_service, logger)
+    flow = TestedConnectivityFlow(parse_connectivity_request_service)
     res = flow.apply_connectivity(request)
 
     assert res
     res = json.loads(res)
     assert len(res["driverResponse"]["actionResults"]) == 1
     action_result = res["driverResponse"]["actionResults"][0]
     assert action_result["success"] is False
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/conftest.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 from __future__ import annotations
 
 import json
-from unittest.mock import Mock
 
 import pytest
 
 from cloudshell.shell.flows.connectivity.models.connectivity_model import (
     ConnectionModeEnum,
     ConnectivityActionModel,
 )
 
 
 @pytest.fixture()
-def logger():
-    return Mock(name="logger")
-
-
-@pytest.fixture()
 def action_request():
     return {
         "connectionId": "96582265-2728-43aa-bc97-cefb2457ca44",
         "connectionParams": {
             "vlanId": "10-11",
             "mode": "Trunk",
             "vlanServiceAttributes": [
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/test_simple_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     return ConnectivityActionResult.success_result(action, "success msg")
 
 
 def _remove_vlan_action(action: ConnectivityActionModel) -> ConnectivityActionResult:
     return ConnectivityActionResult.success_result(action, "success msg")
 
 
-def test_apply_connectivity_changes(logger, action_request):
+def test_apply_connectivity_changes(action_request):
     action_req_remove = action_request
     action_req_set = deepcopy(action_request)
     action_req_set["type"] = "setVlan"
     action_req_set["actionId"] = "new action id"
     driver_request = json.dumps(
         {"driverRequest": {"actions": [action_req_remove, action_req_set]}}
     )
 
     res = apply_connectivity_changes(
-        driver_request, _add_vlan_action, _remove_vlan_action, logger
+        driver_request, _add_vlan_action, _remove_vlan_action
     )
     assert json.loads(res) == {
         "driverResponse": {
             "actionResults": [
                 {
                     "actionId": (
                         "96582265-2728-43aa-bc97-cefb2457ca44_0900c4b5-0f90-42e3-b495"
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_dict_action_helpers.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vnic_helpers.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_vlan_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/helpers/test_remove_vlans.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_connectivity_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py` & `cloudshell-shell-connectivity-flow-4.0.0/tests/cloudshell/shell/flows/connectivity/models/test_driver_response.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/parse_request_service.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/parse_request_service.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/basic_flow.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/basic_flow.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
+import logging
 from abc import ABC, abstractmethod
 from collections.abc import Collection
 from concurrent import futures as ft
-from logging import Logger
+
+from cloudshell.logging.context_filters import pass_log_context
 
 from cloudshell.shell.flows.connectivity.helpers.remove_vlans import (
     prepare_remove_vlan_actions,
 )
 from cloudshell.shell.flows.connectivity.models.connectivity_model import (
     ConnectivityActionModel,
 )
@@ -15,23 +17,23 @@
     ConnectivityActionResult,
     DriverResponseRoot,
 )
 from cloudshell.shell.flows.connectivity.parse_request_service import (
     AbstractParseConnectivityService,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class AbstractConnectivityFlow(ABC):
     def __init__(
         self,
         parse_connectivity_request_service: AbstractParseConnectivityService,
-        logger: Logger,
     ):
         self._parse_connectivity_request_service = parse_connectivity_request_service
-        self._logger = logger
         self._results: dict[str, ConnectivityActionResult] = {}
 
     @abstractmethod
     def _set_vlan(self, action: ConnectivityActionModel) -> ConnectivityActionResult:
         raise NotImplementedError()
 
     @abstractmethod
@@ -57,27 +59,27 @@
                 target_name = action.action_target.name
                 emsg = f"Failed to apply VLAN changes ({vlan}) for target {target_name}"
                 if action.custom_action_attrs.vm_uuid:
                     emsg += f" on VM ID {action.custom_action_attrs.vm_uuid}"
                     if action.custom_action_attrs.vnic:
                         emsg += f" for vNIC {action.custom_action_attrs.vnic}"
                 emsg = f"{emsg}. Error: {e}"
-                self._logger.exception(emsg)
+                logger.exception(emsg)
                 result = ConnectivityActionResult.fail_result(action, emsg)
             self._results[result.actionId] = result
 
     def apply_connectivity(self, request: str) -> str:
-        self._logger.debug(f"Apply connectivity request: {request}")
+        logger.debug(f"Apply connectivity request: {request}")
         actions = self._parse_connectivity_request_service.get_actions(request)
         self._validate_received_actions(actions)
         set_actions = list(filter(lambda a: a.type is a.type.SET_VLAN, actions))
         remove_actions = list(filter(lambda a: a.type is a.type.REMOVE_VLAN, actions))
         remove_actions = prepare_remove_vlan_actions(set_actions, remove_actions)
 
-        with ft.ThreadPoolExecutor() as executor:
+        with ft.ThreadPoolExecutor(initializer=pass_log_context()) as executor:
             remove_vlan_futures = {
                 executor.submit(self._remove_vlan, action): action
                 for action in remove_actions
             }
             self._wait_futures(remove_vlan_futures)
 
             self._filter_set_actions(set_actions)
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/simple_flow.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/simple_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 import logging
-from logging import Logger
-from typing import Callable, Optional
+from typing import Callable
 
 from cloudshell.shell.flows.connectivity.exceptions import ApplyConnectivityException
 from cloudshell.shell.flows.connectivity.models.connectivity_model import (
     ConnectivityActionModel,
 )
 from cloudshell.shell.flows.connectivity.models.driver_response import (
     ConnectivityActionResult,
     DriverResponseRoot,
 )
 from cloudshell.shell.flows.connectivity.parse_request_service import (
     ParseConnectivityRequestService,
 )
 
+logger = logging.getLogger(__name__)
+
 
 def apply_connectivity_changes(
     request: str,
     add_vlan_action: Callable[[ConnectivityActionModel], ConnectivityActionResult],
     remove_vlan_action: Callable[[ConnectivityActionModel], ConnectivityActionResult],
-    logger: Optional[Logger] = None,
 ) -> str:
     """Standard implementation for the apply_connectivity_changes operation.
 
     This function will accept as an input the actions to perform for add/remove vlan.
     It implements the basic flow of decoding the JSON connectivity changes requests,
     and combining the results of the add/remove vlan functions into a result object.
 
     :param str request: json string sent from the CloudShell server
             describing the connectivity changes to perform
     :param Function -> ConnectivityActionResult remove_vlan_action:
             This action will be called for VLAN remove operations
     :param Function -> ConnectivityActionResult add_vlan_action:
             This action will be called for VLAN add operations
-    :param logger: logger to use for the operation, if you don't provide a logger,
-            a default Python logger will be used
     :return Returns a driver action result object,
             this can be returned to CloudShell server by the command result
     """
-    if not logger:
-        logger = logging.getLogger("apply_connectivity_changes")
-
     if request is None or request == "":
         raise ApplyConnectivityException("Request is None or empty")
 
     actions = ParseConnectivityRequestService(
         is_vlan_range_supported=True, is_multi_vlan_supported=True
     ).get_actions(request)
```

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vnic_helpers.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/remove_vlans.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/dict_action_helpers.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/helpers/vlan_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/connectivity_model.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/connectivity_model.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell/shell/flows/connectivity/models/driver_response.py` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell/shell/flows/connectivity/models/driver_response.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-connectivity-flow-3.2.1/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt` & `cloudshell-shell-connectivity-flow-4.0.0/cloudshell_shell_connectivity_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

