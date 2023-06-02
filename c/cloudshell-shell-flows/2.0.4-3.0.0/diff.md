# Comparing `tmp/cloudshell-shell-flows-2.0.4.zip` & `tmp/cloudshell-shell-flows-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,79 +1,80 @@
-Zip file size: 53459 bytes, number of entries: 77
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/
--rw-r--r--  2.0 unx       34 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/MANIFEST.in
--rw-r--r--  2.0 unx     1051 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tox.ini
--rw-r--r--  2.0 unx       60 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/dev_requirements.txt
--rw-r--r--  2.0 unx      840 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/README.md
--rw-r--r--  2.0 unx      276 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/PKG-INFO
--rw-r--r--  2.0 unx       18 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/test_requirements.txt
--rw-r--r--  2.0 unx      831 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/setup.py
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/version.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/setup.cfg
--rw-r--r--  2.0 unx    97622 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/LICENSE.htm
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/requirements.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/__init__.py
--rw-r--r--  2.0 unx       98 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/conftest.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/
--rw-r--r--  2.0 unx     1674 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/test_interfaces.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/__init__.py
--rw-r--r--  2.0 unx     2369 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/__init__.py
--rw-r--r--  2.0 unx     3217 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/test_basic_flow.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_str_helpers.py
--rw-r--r--  2.0 unx     9126 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_url.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/__init__.py
--rw-r--r--  2.0 unx     2158 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/test_basic_flow.py
--rw-r--r--  2.0 unx      698 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/__init__.py
--rw-r--r--  2.0 unx     3314 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/test_basic_flow.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/__init__.py
--rw-r--r--  2.0 unx    10793 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/
--rw-r--r--  2.0 unx     1390 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/interfaces.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/__init__.py
--rw-r--r--  2.0 unx     2543 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/basic_flow.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/__init__.py
--rw-r--r--  2.0 unx     2388 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/basic_flow.py
--rw-r--r--  2.0 unx     9137 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/url.py
--rw-r--r--  2.0 unx      479 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/str_helpers.py
--rw-r--r--  2.0 unx       76 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/errors.py
--rw-r--r--  2.0 unx      206 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/resource_conf.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/__init__.py
--rw-r--r--  2.0 unx     1917 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/basic_flow.py
--rw-r--r--  2.0 unx      576 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/autoload_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/__init__.py
--rw-r--r--  2.0 unx     1534 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/basic_flow.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/__init__.py
--rw-r--r--  2.0 unx    10232 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/basic_flow.py
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2130 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      276 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/requires.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-31 11:09 cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/top_level.txt
-77 files, 168087 bytes uncompressed, 37783 bytes compressed:  77.5%
+Zip file size: 53893 bytes, number of entries: 78
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/setup.cfg
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tox.ini
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/version.txt
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/test_requirements.txt
+-rw-r--r--  2.0 unx       34 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/MANIFEST.in
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/requirements.txt
+-rw-r--r--  2.0 unx      276 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/PKG-INFO
+-rw-r--r--  2.0 unx    97622 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/LICENSE.htm
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/dev_requirements.txt
+-rw-r--r--  2.0 unx      831 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/setup.py
+-rw-r--r--  2.0 unx      883 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/README.md
+-rw-r--r--  2.0 unx      111 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     2172 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      276 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/__init__.py
+-rw-r--r--  2.0 unx      333 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/conftest.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/__init__.py
+-rw-r--r--  2.0 unx     1674 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/test_interfaces.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/__init__.py
+-rw-r--r--  2.0 unx     9126 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_url.py
+-rw-r--r--  2.0 unx      536 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_str_helpers.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/__init__.py
+-rw-r--r--  2.0 unx    10669 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/__init__.py
+-rw-r--r--  2.0 unx     3208 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/test_basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/__init__.py
+-rw-r--r--  2.0 unx     3119 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/test_basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/__init__.py
+-rw-r--r--  2.0 unx      698 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py
+-rw-r--r--  2.0 unx     1766 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/test_basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/__init__.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-02 10:50 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/
+-rw-r--r--  2.0 unx     1732 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/interfaces.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/__init__.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/__init__.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/protocols.py
+-rw-r--r--  2.0 unx      479 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/str_helpers.py
+-rw-r--r--  2.0 unx     9137 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/url.py
+-rw-r--r--  2.0 unx      206 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/resource_conf.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/__init__.py
+-rw-r--r--  2.0 unx    10145 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/__init__.py
+-rw-r--r--  2.0 unx     1544 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/__init__.py
+-rw-r--r--  2.0 unx     1965 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/__init__.py
+-rw-r--r--  2.0 unx      576 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/autoload_utils.py
+-rw-r--r--  2.0 unx     1679 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/basic_flow.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/__init__.py
+-rw-r--r--  2.0 unx     2283 b- defN 23-Jun-02 10:49 cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/basic_flow.py
+78 files, 167679 bytes uncompressed, 38001 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -1,232 +1,235 @@
-Filename: cloudshell-shell-flows-2.0.4/
+Filename: cloudshell-shell-flows-3.0.0/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/
+Filename: cloudshell-shell-flows-3.0.0/tests/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/MANIFEST.in
+Filename: cloudshell-shell-flows-3.0.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tox.ini
+Filename: cloudshell-shell-flows-3.0.0/tox.ini
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/dev_requirements.txt
+Filename: cloudshell-shell-flows-3.0.0/version.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/README.md
+Filename: cloudshell-shell-flows-3.0.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/PKG-INFO
+Filename: cloudshell-shell-flows-3.0.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/test_requirements.txt
+Filename: cloudshell-shell-flows-3.0.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/setup.py
+Filename: cloudshell-shell-flows-3.0.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/version.txt
+Filename: cloudshell-shell-flows-3.0.0/LICENSE.htm
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/setup.cfg
+Filename: cloudshell-shell-flows-3.0.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/LICENSE.htm
+Filename: cloudshell-shell-flows-3.0.0/setup.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/requirements.txt
+Filename: cloudshell-shell-flows-3.0.0/README.md
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/conftest.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/
+Filename: cloudshell-shell-flows-3.0.0/tests/conftest.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/test_interfaces.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/test_basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/test_interfaces.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_str_helpers.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_url.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_url.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_str_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/test_basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/test_basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/test_basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/test_basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/test_basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/
+Filename: cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/interfaces.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/command/basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/interfaces.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/url.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/str_helpers.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/errors.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/errors.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/resource_conf.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/protocols.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/str_helpers.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/url.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/resource_conf.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/autoload_utils.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/state/basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/__init__.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/state/basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/basic_flow.py
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/dependency_links.txt
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/command/basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/SOURCES.txt
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/PKG-INFO
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/autoload_utils.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/requires.txt
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/basic_flow.py
 Comment: 
 
-Filename: cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/top_level.txt
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/__init__.py
+Comment: 
+
+Filename: cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/basic_flow.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-shell-flows-2.0.4/tox.ini` & `cloudshell-shell-flows-3.0.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -36,7 +36,8 @@
 forced_separate = cloudshell.shell.flows,tests
 
 [flake8]
 max-line-length = 88
 ;we don't need have docstrings in every func, class and package
 ;and W503 is not PEP 8 compliant
 ignore = D100,D101,D102,D103,D104,D105,D106,D107,D401,W503,E203
+known-modules = cloudshell-shell-flows:[cloudshell.shell.flows],cloudshell-logging:[cloudshell.logging],cloudshell-shell-standards:[cloudshell.shell.standards],cloudshell-shell-core:[cloudshell.shell.core]
```

## Comparing `cloudshell-shell-flows-2.0.4/README.md` & `cloudshell-shell-flows-3.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # cloudshell-shell-flows
-[![Build status](https://travis-ci.org/QualiSystems/cloudshell-shell-flows.svg?branch=master)](https://travis-ci.org/QualiSystems/cloudshell-shell-flows)
+[![Build status](https://github.com/QualiSystems/cloudshell-shell-flows/workflows/CI/badge.svg?branch=master)](https://github.com/QualiSystems/cloudshell-shell-flows/actions?query=branch%3Amaster)
 [![codecov](https://codecov.io/gh/QualiSystems/cloudshell-shell-flows/branch/master/graph/badge.svg)](https://codecov.io/gh/QualiSystems/cloudshell-shell-flows)
 [![PyPI version](https://badge.fury.io/py/cloudshell-shell-flows.svg)](https://badge.fury.io/py/cloudshell-shell-flows)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 
 <p align="center">
 <img src="https://github.com/QualiSystems/devguide_source/raw/master/logo.png"></img>
 </p>
```

## Comparing `cloudshell-shell-flows-2.0.4/setup.py` & `cloudshell-shell-flows-3.0.0/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/LICENSE.htm` & `cloudshell-shell-flows-3.0.0/LICENSE.htm`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/test_interfaces.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/test_interfaces.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/firmware/test_firmware_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,64 +14,62 @@
 
 @pytest.fixture()
 def resource_config():
     return ResourceConfig()
 
 
 @pytest.fixture()
-def firmware_flow_do_nothing(logger, resource_config):
+def firmware_flow_do_nothing(resource_config):
     class TestedFlow(AbstractFirmwareFlow):
         def _load_firmware_flow(
             self,
             firmware_url,
             vrf_management_name: str | None,
             timeout: int,
         ) -> None:
             return
 
-    return TestedFlow(logger, resource_config)
+    return TestedFlow(resource_config)
 
 
-def test_abstract_flow(logger, resource_config):
+def test_abstract_flow(resource_config):
     class TestedFlow(AbstractFirmwareFlow):
         def _load_firmware_flow(
             self,
             firmware_url,
             vrf_management_name: str | None,
             timeout: int,
         ) -> None:
             super()._load_firmware_flow(firmware_url, vrf_management_name, timeout)
 
-    flow = TestedFlow(logger, resource_config)
+    flow = TestedFlow(resource_config)
     with pytest.raises(NotImplementedError):
         flow._load_firmware_flow("", None, 100)
 
 
 @pytest.mark.parametrize(
     ("path", "vrf", "expected_url_str", "expected_vrf"),
     (
         ("ftp://user@host/file", "mgmt", "ftp://user@host/file", "mgmt"),
         ("tftp://host/file", None, "tftp://host/file", "vrf name"),
         ("flash://file", None, "flash://file", "vrf name"),
     ),
 )
-def test_load_firmware(
-    path, vrf, expected_url_str, expected_vrf, logger, resource_config
-):
+def test_load_firmware(path, vrf, expected_url_str, expected_vrf, resource_config):
     class TestedFlow(AbstractFirmwareFlow):
         def _load_firmware_flow(
             self,
             firmware_url,
             vrf_management_name: str | None,
             timeout: int,
         ) -> None:
             assert str(firmware_url) == expected_url_str
             assert vrf_management_name == expected_vrf
 
-    flow = TestedFlow(logger, resource_config)
+    flow = TestedFlow(resource_config)
     flow.load_firmware(path, vrf)
 
 
 def test_path_without_file(firmware_flow_do_nothing):
     with pytest.raises(FileNameIsNotPresent):
         firmware_flow_do_nothing.load_firmware("ftp://host")
```

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/command/test_basic_flow.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/command/test_basic_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from unittest import mock
 
 from cloudshell.shell.flows.command.basic_flow import RunCommandFlow
 
 
 class TestRunCommandFlow(unittest.TestCase):
     def setUp(self):
-        self.logger = mock.MagicMock()
         self.cli_configurator = mock.MagicMock()
         self.enable_session = mock.MagicMock()
         self.config_session = mock.MagicMock()
         self.cli_configurator = mock.MagicMock(
             enable_mode_service=mock.MagicMock(
                 return_value=mock.MagicMock(
                     __enter__=mock.MagicMock(return_value=self.enable_session)
@@ -18,17 +17,15 @@
             ),
             config_mode_service=mock.MagicMock(
                 return_value=mock.MagicMock(
                     __enter__=mock.MagicMock(return_value=self.config_session)
                 )
             ),
         )
-        self.run_flow = RunCommandFlow(
-            logger=self.logger, cli_configurator=self.cli_configurator
-        )
+        self.run_flow = RunCommandFlow(self.cli_configurator)
 
     def test_run_custom_command(self):
         custom_command = "test custom command"
         expected_result = mock.MagicMock()
         self.run_flow._run_command_flow = mock.MagicMock(return_value=expected_result)
         # act
         result = self.run_flow.run_custom_command(custom_command)
```

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_str_helpers.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_str_helpers.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/utils/test_url.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/utils/test_url.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/autoload/test_autoload_utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/state/test_basic_flow.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/state/test_basic_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from unittest import mock
 
 from cloudshell.shell.flows.state.basic_flow import StateFlow
 
 
 class TestStateFlow(unittest.TestCase):
     def setUp(self):
-        self.logger = mock.MagicMock()
         self.api = mock.MagicMock()
         self.resource_config = mock.MagicMock()
         self.session = mock.MagicMock(
             send_command=mock.MagicMock(
                 side_effect=lambda command: f"Output of {command!r}"
             )
         )
@@ -18,15 +17,14 @@
             enable_mode_service=mock.MagicMock(
                 return_value=mock.MagicMock(
                     __enter__=mock.MagicMock(return_value=self.session)
                 )
             )
         )
         self.state_flow = StateFlow(
-            logger=self.logger,
             api=self.api,
             resource_config=self.resource_config,
             cli_configurator=self.cli_configurator,
         )
 
     def test_shutdown(self):
         """Check that method will raise exception."""
@@ -44,17 +42,15 @@
         result = self.state_flow.health_check()
         # verify
         self.assertEqual(
             result,
             f"Health check on resource {self.resource_config.name} passed.",
         )
 
-        run_command_flow_class.assert_called_once_with(
-            self.logger, self.cli_configurator
-        )
+        run_command_flow_class.assert_called_once_with(self.cli_configurator)
         run_command_flow.run_custom_command.assert_called_once_with("")
         self.api.SetResourceLiveStatus.assert_called_once_with(
             self.resource_config.name, "Online", result
         )
 
     @mock.patch("cloudshell.shell.flows.state.basic_flow.RunCommandFlow")
     def test_health_check_failed(self, run_command_flow_class):
```

## Comparing `cloudshell-shell-flows-2.0.4/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py` & `cloudshell-shell-flows-3.0.0/tests/cloudshell/shell/flows/configuration/test_configuration_flow.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         return l_time
 
     monkeypatch.setattr(time, "localtime", get_local_time)
     return time.strftime("%d%m%y-%H%M%S", l_time)
 
 
 @pytest.fixture()
-def flow_do_nothing(logger):
+def flow_do_nothing():
     class TestedFlow(AbstractConfigurationFlow):
         file_system = "file:/"
 
         def _save_flow(
             self,
             file_dst_url,
             configuration_type: ConfigurationType,
@@ -59,18 +59,18 @@
             configuration_type: ConfigurationType,
             restore_method: RestoreMethod,
             vrf_management_name: str | None,
         ) -> None:
             pass
 
     conf = ResourceConfig("res-name")
-    return TestedFlow(logger, conf)
+    return TestedFlow(conf)
 
 
-def test_file_system_property_not_implemented(logger):
+def test_file_system_property_not_implemented():
     class TestedFlow(AbstractConfigurationFlow):
         def _save_flow(
             self,
             file_dst_url,
             configuration_type: ConfigurationType,
             vrf_management_name: str | None,
         ) -> str | None:
@@ -90,15 +90,15 @@
             )
 
         @property
         def file_system(self) -> str:
             return super().file_system
 
     conf = ResourceConfig("res-name")
-    flow = TestedFlow(logger, conf)
+    flow = TestedFlow(conf)
 
     with pytest.raises(NotImplementedError):
         _ = flow.file_system
     with pytest.raises(NotImplementedError):
         flow._save_flow(None, None, None)
     with pytest.raises(NotImplementedError):
         flow._restore_flow(None, None, None, None)
@@ -181,15 +181,14 @@
     ),
 )
 def test_save_method_get_correct_file_path(
     folder_path,
     resource_config,
     file_system,
     expected_file_prefix,
-    logger,
     local_time_str,
 ):
     config_type = "running"
     expected_file_path = f"{expected_file_prefix}-{config_type}-{local_time_str}"
 
     class TestedConfigurationFlow(AbstractConfigurationFlow):
         _restore_flow = None
@@ -198,60 +197,60 @@
         def file_system(self) -> str:
             return file_system
 
         def _save_flow(self, file_dst_url, configuration_type, vrf_management_name):
             assert str(file_dst_url) == expected_file_path
             assert configuration_type == ConfigurationType.from_str(config_type)
 
-    flow = TestedConfigurationFlow(logger, resource_config)
+    flow = TestedConfigurationFlow(resource_config)
 
     file_name = flow.save(folder_path, config_type)
     assert expected_file_path.endswith(file_name)
 
 
-def test_save_return_another_filename(logger):
+def test_save_return_another_filename():
     class TestedConfigurationFlow(AbstractConfigurationFlow):
         _restore_flow = None
         file_system = None
 
         def _save_flow(
             self,
             file_dst_url,
             configuration_type: ConfigurationType,
             vrf_management_name: str | None,
         ) -> str | None:
             return "another-file-name"
 
     resource_config = ResourceConfig("res-name")
-    flow = TestedConfigurationFlow(logger, resource_config)
+    flow = TestedConfigurationFlow(resource_config)
     file_name = flow.save("ftp://folder-path", "running")
 
     assert file_name == "another-file-name"
 
 
 def test_save_incorrect_folder_path(flow_do_nothing):
     with pytest.raises(ErrorParsingUrl):
         flow_do_nothing.save("flash", "startup")
 
 
-def test_orchestration_save(logger, local_time_str):
+def test_orchestration_save(local_time_str):
     class TestedFlow(AbstractConfigurationFlow):
         file_system = "flash:/"
         _restore_flow = None
 
         def _save_flow(
             self,
             file_dst_url,
             configuration_type: ConfigurationType,
             vrf_management_name: str | None,
         ) -> str | None:
             return None
 
     conf = ResourceConfig("res-name")
-    flow = TestedFlow(logger, conf)
+    flow = TestedFlow(conf)
     custom_params = json.dumps({"custom_params": {"configuration_type": "startup"}})
     file_path = flow.orchestration_save(custom_params=custom_params)
     file_suffix = f"-startup-{local_time_str}"
 
     assert file_path == f"{TestedFlow.file_system}{conf.name}{file_suffix}"
 
 
@@ -272,15 +271,15 @@
         (
             "file_name",
             ResourceConfig("", backup_user="user", backup_password="pass"),
             "disk0:file_name",
         ),
     ),
 )
-def test_restore(logger, passed_config_path, resource_config, expected_config_path):
+def test_restore(passed_config_path, resource_config, expected_config_path):
     class TestedFlow(AbstractConfigurationFlow):
         file_system = "disk0:"
         _save_flow = None
 
         def _restore_flow(
             self,
             config_path,
@@ -289,37 +288,37 @@
             vrf_management_name: str | None,
         ) -> None:
             assert str(config_path) == expected_config_path
             assert configuration_type == ConfigurationType.STARTUP
             assert restore_method == RestoreMethod.OVERRIDE
             assert vrf_management_name == "mgmt-vrf"
 
-    flow = TestedFlow(logger, resource_config)
+    flow = TestedFlow(resource_config)
     flow.restore(passed_config_path, "startup", "override", "mgmt-vrf")
 
 
-def test_restore_invalid_path(logger):
+def test_restore_invalid_path():
     class TestedFlow(AbstractConfigurationFlow):
         file_system = None
         _save_flow = None
         _restore_flow = None
 
     conf = ResourceConfig("")
-    flow = TestedFlow(logger, conf)
+    flow = TestedFlow(conf)
 
     with pytest.raises(ErrorParsingUrl):
         flow.restore("file", "running", "append")
 
 
 def test_restore_without_filename(flow_do_nothing):
     with pytest.raises(FileNameIsNotPresent):
         flow_do_nothing.restore("ftp://host", "running", "append")
 
 
-def test_another_local_url(logger, local_time_str):
+def test_another_local_url(local_time_str):
     file_suffix = f"-running-{local_time_str}"
     conf = ResourceConfig("res-name")
 
     class TestedFlow(AbstractConfigurationFlow):
         LOCAL_URL_CLASS = LocalFileURL
         file_system = "file:/"
 
@@ -337,15 +336,15 @@
             config_path: LOCAL_URL_CLASS,
             configuration_type: ConfigurationType,
             restore_method: RestoreMethod,
             vrf_management_name: str | None,
         ) -> None:
             assert config_path == LocalFileURL(path="/folder/res-name")
 
-    flow = TestedFlow(logger, conf)
+    flow = TestedFlow(conf)
     flow.save("file://folder", "running", "mgmt")
     flow.restore("file://folder/res-name", "running", "append", "mgmt")
 
 
 def test_validation_of_configuration_type(flow_do_nothing):
     flow_do_nothing.SUPPORTED_CONFIGURATION_TYPES = {ConfigurationType.RUNNING}
     with pytest.raises(ConfigurationTypeNotSupported):
```

## Comparing `cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/firmware/basic_flow.py` & `cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/firmware/basic_flow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 from __future__ import annotations
 
 from abc import abstractmethod
-from logging import Logger
-from typing import TYPE_CHECKING
 
 from cloudshell.logging.utils.decorators import command_logging
 
 from cloudshell.shell.flows.interfaces import FirmwareFlowInterface
 from cloudshell.shell.flows.utils.str_helpers import normalize_path
 from cloudshell.shell.flows.utils.url import (
     BasicLocalUrl,
     ErrorParsingUrl,
     RemoteURL,
     ValidationError,
 )
 
-if TYPE_CHECKING:
-    from cloudshell.shell.standards.core.resource_config_entities import (
-        GenericResourceConfig,
-    )
-
 
 class AbstractFirmwareFlow(FirmwareFlowInterface):
     REMOTE_URL_CLASS = RemoteURL
     LOCAL_URL_CLASS = BasicLocalUrl
 
-    def __init__(self, logger: Logger, resource_config: GenericResourceConfig):
-        self._logger = logger
+    def __init__(self, resource_config):
         self._timeout = 3600
         self._resource_config = resource_config
 
     @abstractmethod
     def _load_firmware_flow(
         self,
         firmware_url: REMOTE_URL_CLASS | LOCAL_URL_CLASS,
```

## Comparing `cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/utils/url.py` & `cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/utils/url.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/autoload/autoload_utils.py` & `cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/autoload/autoload_utils.py`

 * *Files identical despite different names*

## Comparing `cloudshell-shell-flows-2.0.4/cloudshell/shell/flows/configuration/basic_flow.py` & `cloudshell-shell-flows-3.0.0/cloudshell/shell/flows/configuration/basic_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 
+import json
 import re
 import time
 from abc import abstractmethod
 from enum import Enum
-from logging import Logger
 from typing import TYPE_CHECKING
 
-import jsonpickle
-
 from cloudshell.logging.utils.decorators import command_logging
 
 from cloudshell.shell.flows.interfaces import ConfigurationFlowInterface
 from cloudshell.shell.flows.utils.errors import ShellFlowsException
 from cloudshell.shell.flows.utils.resource_conf import get_str_backup_type
 from cloudshell.shell.flows.utils.str_helpers import normalize_path
 from cloudshell.shell.flows.utils.url import (
@@ -70,16 +68,15 @@
         ConfigurationType.STARTUP,
     }
     SUPPORTED_RESTORE_METHODS: set[RestoreMethod] = {
         RestoreMethod.OVERRIDE,
         RestoreMethod.APPEND,
     }
 
-    def __init__(self, logger: Logger, resource_config: GenericBackupConfig):
-        self._logger = logger
+    def __init__(self, resource_config: GenericBackupConfig):
         self._resource_config = resource_config
 
     @property
     @abstractmethod
     def file_system(self) -> str:
         """Default File System scheme."""
         raise NotImplementedError
@@ -138,15 +135,15 @@
         save_params = {
             "folder_path": "",
             "configuration_type": "running",
             "return_full_path": True,
         }
         params = {}
         if custom_params:
-            params = jsonpickle.decode(custom_params)
+            params = json.loads(custom_params)
 
         save_params.update(params.get("custom_params", {}))
         path = self.save(**save_params)
 
         return path
 
     @command_logging
```

## Comparing `cloudshell-shell-flows-2.0.4/cloudshell_shell_flows.egg-info/SOURCES.txt` & `cloudshell-shell-flows-3.0.0/cloudshell_shell_flows.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 cloudshell/shell/flows/configuration/basic_flow.py
 cloudshell/shell/flows/firmware/__init__.py
 cloudshell/shell/flows/firmware/basic_flow.py
 cloudshell/shell/flows/state/__init__.py
 cloudshell/shell/flows/state/basic_flow.py
 cloudshell/shell/flows/utils/__init__.py
 cloudshell/shell/flows/utils/errors.py
+cloudshell/shell/flows/utils/protocols.py
 cloudshell/shell/flows/utils/resource_conf.py
 cloudshell/shell/flows/utils/str_helpers.py
 cloudshell/shell/flows/utils/url.py
 cloudshell_shell_flows.egg-info/PKG-INFO
 cloudshell_shell_flows.egg-info/SOURCES.txt
 cloudshell_shell_flows.egg-info/dependency_links.txt
 cloudshell_shell_flows.egg-info/requires.txt
```

