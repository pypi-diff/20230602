# Comparing `tmp/iris_pex_embedded_python-2.3.1.tar.gz` & `tmp/iris_pex_embedded_python-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.1.tar", last modified: Wed May 31 16:24:12 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.2.tar", last modified: Fri Jun  2 07:52:45 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.1.tar` & `iris_pex_embedded_python-2.3.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.201367 iris_pex_embedded_python-2.3.1/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.1/LICENSE
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 16:24:12.200313 iris_pex_embedded_python-2.3.1/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49099 2023-05-31 14:32:55.000000 iris_pex_embedded_python-2.3.1/README.md
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.1/pyproject.toml
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-05-31 16:24:12.201732 iris_pex_embedded_python-2.3.1/setup.cfg
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2295 2023-05-31 16:23:50.000000 iris_pex_embedded_python-2.3.1/setup.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.142758 iris_pex_embedded_python-2.3.1/src/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.141596 iris_pex_embedded_python-2.3.1/src/grongier/
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.151296 iris_pex_embedded_python-2.3.1/src/grongier/iris/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/iris/__init__.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.186260 iris_pex_embedded_python-2.3.1/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5491 2023-05-31 11:56:27.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8057 2023-05-31 15:44:03.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.1/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-05-31 16:24:12.198356 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    50008 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      933 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       47 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/entry_points.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-05-31 16:24:12.000000 iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.902573 iris_pex_embedded_python-2.3.2/
+-rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.2/LICENSE
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-02 07:52:45.901644 iris_pex_embedded_python-2.3.2/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.2/README.md
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.2/pyproject.toml
+-rw-r--r--   0 grongier (902446405) 1252422112       38 2023-06-02 07:52:45.902858 iris_pex_embedded_python-2.3.2/setup.cfg
+-rw-r--r--   0 grongier (902446405) 1252422112     2295 2023-06-02 07:52:21.000000 iris_pex_embedded_python-2.3.2/setup.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.841233 iris_pex_embedded_python-2.3.2/src/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.840175 iris_pex_embedded_python-2.3.2/src/grongier/
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.850172 iris_pex_embedded_python-2.3.2/src/grongier/iris/
+-rw-r--r--   0 grongier (902446405) 1252422112        0 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/iris/__init__.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.886553 iris_pex_embedded_python-2.3.2/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-04-21 15:01:34.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5471 2023-05-31 16:30:39.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15107 2023-04-21 08:43:30.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) 1252422112     8057 2023-05-31 15:44:03.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      325 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) 1252422112    15120 2023-05-31 13:10:44.000000 iris_pex_embedded_python-2.3.2/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-06-02 07:52:45.899649 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) 1252422112      933 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        1 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       47 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) 1252422112       43 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) 1252422112        9 2023-06-02 07:52:45.000000 iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.1/LICENSE` & `iris_pex_embedded_python-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/PKG-INFO` & `iris_pex_embedded_python-2.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.1
+Version: 2.3.2
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -1123,19 +1123,19 @@
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Command line
 
-Since version 2.3.0, you can use the command line to register your components and productions.
+Since version 2.3.1, you can use the command line to register your components and productions.
 
 To use it, you have to use the following command :
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex 
+iop 
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 optional arguments:
   -h, --help            display help and default production name
@@ -1159,15 +1159,15 @@
 ```
 
 ## 8.1. help
 
 The help command display the help and the default production name.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -h
+iop -h
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 ...
 default production: PEX.Production
@@ -1176,34 +1176,34 @@
 ## 8.2. default
 
 The default command set the default production.
 
 With no argument, it display the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d
+iop -d
 ```
 
 output :
 ```bash
 default production: PEX.Production
 ```
 
 With an argument, it set the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+iop -d PEX.Production
 ```
 
 ## 8.3. lists
 
 The lists command list productions.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -l
+iop -l
 ```
 
 output :
 ```bash
 {
     "PEX.Production": {
         "Status": "Stopped",
@@ -1217,15 +1217,15 @@
 ## 8.4. start
 
 The start command start a production.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+iop -s PEX.Production
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
@@ -1237,63 +1237,63 @@
 The kill command kill a production (force stop).
 
 Kill command is the same as stop command but with a force stop.
 
 Kill command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -k 
+iop -k 
 ```
 
 ## 8.6. stop
 
 The stop command stop a production.
 
 Stop command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -S 
+iop -S 
 ```
 
 ## 8.7. restart
 
 The restart command restart a production.
 
 Restart command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -r 
+iop -r 
 ```
 
 ## 8.8. migrate
 
 The migrate command migrate a production and classes with settings file.
 
 Migrate command must take the absolute path of the settings file.
 
 Settings file must be in the same folder as the python code.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+iop -M /tmp/settings.py
 ```
 
 ## 8.9. export
 
 The export command export a production.
 
 If no argument is given, the export command export the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e
+iop -e
 ```
 
 If an argument is given, the export command export the production given in argument.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+iop -e PEX.Production
 ```
 
 output :
 ```bash
 {
     "Production": {
         "@Name": "PEX.Production",
@@ -1338,15 +1338,15 @@
 ## 8.10. status
 
 The status command status a production.
 
 Status command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -x 
+iop -x 
 ```
 
 output :
 ```bash
 {
     "Production": "PEX.Production",
     "Status": "stopped"
@@ -1360,30 +1360,30 @@
 - troubled
 
 ## 8.11. version
 
 The version command display the version.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -v
+iop -v
 ```
 
 output :
 ```bash
 2.3.0
 ```
 
 ## 8.12. log
 
 The log command display the log.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -L
+iop -L
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
```

### Comparing `iris_pex_embedded_python-2.3.1/README.md` & `iris_pex_embedded_python-2.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1099,19 +1099,19 @@
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Command line
 
-Since version 2.3.0, you can use the command line to register your components and productions.
+Since version 2.3.1, you can use the command line to register your components and productions.
 
 To use it, you have to use the following command :
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex 
+iop 
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 optional arguments:
   -h, --help            display help and default production name
@@ -1135,15 +1135,15 @@
 ```
 
 ## 8.1. help
 
 The help command display the help and the default production name.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -h
+iop -h
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 ...
 default production: PEX.Production
@@ -1152,34 +1152,34 @@
 ## 8.2. default
 
 The default command set the default production.
 
 With no argument, it display the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d
+iop -d
 ```
 
 output :
 ```bash
 default production: PEX.Production
 ```
 
 With an argument, it set the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+iop -d PEX.Production
 ```
 
 ## 8.3. lists
 
 The lists command list productions.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -l
+iop -l
 ```
 
 output :
 ```bash
 {
     "PEX.Production": {
         "Status": "Stopped",
@@ -1193,15 +1193,15 @@
 ## 8.4. start
 
 The start command start a production.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+iop -s PEX.Production
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
@@ -1213,63 +1213,63 @@
 The kill command kill a production (force stop).
 
 Kill command is the same as stop command but with a force stop.
 
 Kill command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -k 
+iop -k 
 ```
 
 ## 8.6. stop
 
 The stop command stop a production.
 
 Stop command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -S 
+iop -S 
 ```
 
 ## 8.7. restart
 
 The restart command restart a production.
 
 Restart command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -r 
+iop -r 
 ```
 
 ## 8.8. migrate
 
 The migrate command migrate a production and classes with settings file.
 
 Migrate command must take the absolute path of the settings file.
 
 Settings file must be in the same folder as the python code.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+iop -M /tmp/settings.py
 ```
 
 ## 8.9. export
 
 The export command export a production.
 
 If no argument is given, the export command export the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e
+iop -e
 ```
 
 If an argument is given, the export command export the production given in argument.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+iop -e PEX.Production
 ```
 
 output :
 ```bash
 {
     "Production": {
         "@Name": "PEX.Production",
@@ -1314,15 +1314,15 @@
 ## 8.10. status
 
 The status command status a production.
 
 Status command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -x 
+iop -x 
 ```
 
 output :
 ```bash
 {
     "Production": "PEX.Production",
     "Status": "stopped"
@@ -1336,30 +1336,30 @@
 - troubled
 
 ## 8.11. version
 
 The version command display the version.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -v
+iop -v
 ```
 
 output :
 ```bash
 2.3.0
 ```
 
 ## 8.12. log
 
 The log command display the log.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -L
+iop -L
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
```

### Comparing `iris_pex_embedded_python-2.3.1/setup.py` & `iris_pex_embedded_python-2.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.1',
+        version='2.3.2',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_host.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         else:
             # export a production
             dikt = _Utils.export_production(args.export)
         print(json.dumps(dikt, indent=4))
 
     else:
         # display help and default production name
-        print("usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]")
+        print("usage: iop [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]")
         print("optional arguments:")
         print("  -h, --help            display help and default production name")
         print("  -d DEFAULT, --default DEFAULT")
         print("                        set the default production")
         print("  -l, --lists           list productions")
         print("  -s START, --start START")
         print("                        start a production")
```

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.2/src/grongier/pex/_utils.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.1
+Version: 2.3.2
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -1123,19 +1123,19 @@
     - This can one or more Classpaths (separated by '|' character) needed in addition to PYTHON_PATH
 
 e.g :
 <img width="800" alt="component-config" src="https://user-images.githubusercontent.com/47849411/131316308-e1898b19-11df-433b-b1c6-7f69d5cc9974.png">
 
 # 8. Command line
 
-Since version 2.3.0, you can use the command line to register your components and productions.
+Since version 2.3.1, you can use the command line to register your components and productions.
 
 To use it, you have to use the following command :
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex 
+iop 
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 optional arguments:
   -h, --help            display help and default production name
@@ -1159,15 +1159,15 @@
 ```
 
 ## 8.1. help
 
 The help command display the help and the default production name.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -h
+iop -h
 ```
 
 output :
 ```bash
 usage: python3 -m grongier.pex [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]
 ...
 default production: PEX.Production
@@ -1176,34 +1176,34 @@
 ## 8.2. default
 
 The default command set the default production.
 
 With no argument, it display the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d
+iop -d
 ```
 
 output :
 ```bash
 default production: PEX.Production
 ```
 
 With an argument, it set the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -d PEX.Production
+iop -d PEX.Production
 ```
 
 ## 8.3. lists
 
 The lists command list productions.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -l
+iop -l
 ```
 
 output :
 ```bash
 {
     "PEX.Production": {
         "Status": "Stopped",
@@ -1217,15 +1217,15 @@
 ## 8.4. start
 
 The start command start a production.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -s PEX.Production
+iop -s PEX.Production
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
@@ -1237,63 +1237,63 @@
 The kill command kill a production (force stop).
 
 Kill command is the same as stop command but with a force stop.
 
 Kill command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -k 
+iop -k 
 ```
 
 ## 8.6. stop
 
 The stop command stop a production.
 
 Stop command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -S 
+iop -S 
 ```
 
 ## 8.7. restart
 
 The restart command restart a production.
 
 Restart command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -r 
+iop -r 
 ```
 
 ## 8.8. migrate
 
 The migrate command migrate a production and classes with settings file.
 
 Migrate command must take the absolute path of the settings file.
 
 Settings file must be in the same folder as the python code.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -M /tmp/settings.json
+iop -M /tmp/settings.py
 ```
 
 ## 8.9. export
 
 The export command export a production.
 
 If no argument is given, the export command export the default production.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e
+iop -e
 ```
 
 If an argument is given, the export command export the production given in argument.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -e PEX.Production
+iop -e PEX.Production
 ```
 
 output :
 ```bash
 {
     "Production": {
         "@Name": "PEX.Production",
@@ -1338,15 +1338,15 @@
 ## 8.10. status
 
 The status command status a production.
 
 Status command doesn't take an argument because only one production can be running.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -x 
+iop -x 
 ```
 
 output :
 ```bash
 {
     "Production": "PEX.Production",
     "Status": "stopped"
@@ -1360,30 +1360,30 @@
 - troubled
 
 ## 8.11. version
 
 The version command display the version.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -v
+iop -v
 ```
 
 output :
 ```bash
 2.3.0
 ```
 
 ## 8.12. log
 
 The log command display the log.
 
 To exit the command, you have to press CTRL+C.
 
 ```bash
-/usr/irissys/bin/irispython -m grongier.pex -L
+iop -L
 ```
 
 output :
 ```bash
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting production
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.FileOperation
 2021-08-30 15:13:51.000 [PEX.Production] INFO: Starting item Python.EmailOperation
```

### Comparing `iris_pex_embedded_python-2.3.1/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.2/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

