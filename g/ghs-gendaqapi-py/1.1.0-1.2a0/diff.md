# Comparing `tmp/ghs-gendaqapi-py-1.1.0.tar.gz` & `tmp/ghs-gendaqapi-py-1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghs-gendaqapi-py-1.1.0.tar", last modified: Mon Apr 11 04:24:36 2022, max compression
+gzip compressed data, was "ghs-gendaqapi-py-1.2a0.tar", last modified: Fri Jun  2 10:29:48 2023, max compression
```

## Comparing `ghs-gendaqapi-py-1.1.0.tar` & `ghs-gendaqapi-py-1.2a0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-04-11 04:24:36.889302 ghs-gendaqapi-py-1.1.0/
--rw-rw-rw-   0        0        0     1170 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2581 2022-04-11 04:24:36.889302 ghs-gendaqapi-py-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1938 2022-04-08 06:40:04.000000 ghs-gendaqapi-py-1.1.0/README.md
--rw-rw-rw-   0        0        0      108 2022-01-25 12:26:46.000000 ghs-gendaqapi-py-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      741 2022-04-11 04:24:36.891687 ghs-gendaqapi-py-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-04-11 04:24:36.846459 ghs-gendaqapi-py-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2022-04-11 04:24:36.860562 ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/
--rw-rw-rw-   0        0        0     2581 2022-04-11 04:24:36.000000 ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2022-04-11 04:24:36.000000 ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-11 04:24:36.000000 ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-04-11 04:24:36.000000 ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-04-11 04:24:36.887429 ghs-gendaqapi-py-1.1.0/src/ghsapi/
--rw-rw-rw-   0        0        0     1283 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/__init__.py
--rw-rw-rw-   0        0        0     7199 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/acquisition_api.py
--rw-rw-rw-   0        0        0    54366 2022-04-08 05:53:49.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/channel_api.py
--rw-rw-rw-   0        0        0     7577 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/connection.py
--rw-rw-rw-   0        0        0     3925 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/connection_api.py
--rw-rw-rw-   0        0        0    53233 2022-04-08 06:38:31.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/ghsapi.py
--rw-rw-rw-   0        0        0     6783 2022-04-08 05:53:49.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/ghsapi_states.py
--rw-rw-rw-   0        0        0     4484 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/json_rpc.py
--rw-rw-rw-   0        0        0     7471 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/mainframe_api.py
--rw-rw-rw-   0        0        0     4678 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/manage_mainframe_settings.py
--rw-rw-rw-   0        0        0    11169 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/manage_recordings_api.py
--rw-rw-rw-   0        0        0    13005 2022-02-01 06:34:43.000000 ghs-gendaqapi-py-1.1.0/src/ghsapi/recorder_api.py
+drwxr-xr-x   0 pedro     (1000) pedro     (1000)        0 2023-06-02 10:29:48.741889 ghs-gendaqapi-py-1.2a0/
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     1147 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/LICENSE
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     2438 2023-06-02 10:29:48.741889 ghs-gendaqapi-py-1.2a0/PKG-INFO
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     1851 2023-03-17 10:33:34.000000 ghs-gendaqapi-py-1.2a0/README.md
+-rw-r--r--   0 pedro     (1000) pedro     (1000)      103 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/pyproject.toml
+-rw-r--r--   0 pedro     (1000) pedro     (1000)      711 2023-06-02 10:29:48.745222 ghs-gendaqapi-py-1.2a0/setup.cfg
+drwxr-xr-x   0 pedro     (1000) pedro     (1000)        0 2023-06-02 10:29:48.691889 ghs-gendaqapi-py-1.2a0/src/
+drwxr-xr-x   0 pedro     (1000) pedro     (1000)        0 2023-06-02 10:29:48.715222 ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     2438 2023-06-02 10:29:48.000000 ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/PKG-INFO
+-rw-r--r--   0 pedro     (1000) pedro     (1000)      581 2023-06-02 10:29:48.000000 ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro     (1000) pedro     (1000)        1 2023-06-02 10:29:48.000000 ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro     (1000) pedro     (1000)        7 2023-06-02 10:29:48.000000 ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/top_level.txt
+drwxr-xr-x   0 pedro     (1000) pedro     (1000)        0 2023-06-02 10:29:48.741889 ghs-gendaqapi-py-1.2a0/src/ghsapi/
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     1256 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/__init__.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     6964 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/acquisition_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)    52581 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/channel_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     7360 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/connection.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     3812 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/connection_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     5589 2023-06-01 14:35:21.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/fieldbus_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)    54745 2023-06-01 14:35:21.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/ghsapi.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     6657 2023-06-01 14:35:21.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/ghsapi_states.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     4366 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/json_rpc.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     7228 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/mainframe_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)     4539 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/manage_mainframe_settings.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)    10807 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/manage_recordings_api.py
+-rw-r--r--   0 pedro     (1000) pedro     (1000)    12577 2023-03-17 10:11:46.000000 ghs-gendaqapi-py-1.2a0/src/ghsapi/recorder_api.py
```

### Comparing `ghs-gendaqapi-py-1.1.0/LICENSE` & `ghs-gendaqapi-py-1.2a0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-Schutweg 15a
-5145 NP Waalwijk
-The Netherlands
-http://www.hbm.com
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+Schutweg 15a
+5145 NP Waalwijk
+The Netherlands
+http://www.hbm.com
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ghs-gendaqapi-py-1.1.0/PKG-INFO` & `ghs-gendaqapi-py-1.2a0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,102 @@
-Metadata-Version: 2.1
-Name: ghs-gendaqapi-py
-Version: 1.1.0
-Summary: Setup, control and acquire data from the Genesis Highspeed systems via python.
-Home-page: https://github.com/hbk-world/ghs-gendaqapi-python
-Author: Vishal Goel
-Author-email: ext_VGOEL@hbm.com
-License: UNKNOWN
-Project-URL: Documentation, https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GEN DAQ API - Python Driver
-> Setup, control and acquire data from the Genesis Highspeed systems via python.
-
-[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
-
-The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
-
-## Requirements
-
-Python 3.10+
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
-
-```bash
-pip install ghs-gendaqapi-py
-```
-
-## Usage
-
-Refer [examples](./examples) for detailed use cases. 
-Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
-
-```python
-from ghsapi import ghsapi
-
-# create Gen Daq API's object
-gen = ghsapi.GHS()
-
-# connect to mainframe
-gen.ghs_connect(IP_ADDRESS, PORT_NO)
-
-# disconnect from mainframe
-gen.ghs_disconnect()
-```
-
-## Development environment setup
-
-Below are the steps to follow to setup devlopement enviroment for system integration and testing.
-
-### Requirements
-
-- `Python 3.10+`
-- `Anaconda/Miniconda`
-
-### Clone repo
-
-```bash
-git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
-```
-
-### Virtual Environment
-
-```bash
-conda create --name <env> --file spec-file.txt
-```
-
-### Install dependencies
-
-```bash
-pip install -r requirements.txt
-```
-
-## Run example files
-
-Edit files in [examples](./examples) to enter mainframe IP and Port number
-
-```bash
-python examples\FILENAME
-```
-
-## Testing
-
-Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
-
-### Unit test
-
-```bash
-python unittest\FILENAME
-```
-
-### Functional test
-
-```bash
-python functionaltest\FILENAME
-```
-
-
+Metadata-Version: 2.1
+Name: ghs-gendaqapi-py
+Version: 1.2a0
+Summary: Setup, control and acquire data from the Genesis Highspeed systems via python.
+Home-page: https://github.com/hbk-world/ghs-gendaqapi-python
+Author: Vishal Goel
+Author-email: ext_VGOEL@hbm.com
+Project-URL: Documentation, https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GEN DAQ API - Python Driver
+> Setup, control and acquire data from the Genesis Highspeed systems via python.
+
+[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
+
+The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
+
+## Requirements
+
+Python 3.10+
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
+
+```bash
+pip install ghs-gendaqapi-py
+```
+
+## Usage
+
+Refer [examples](./examples) for detailed use cases. 
+Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
+
+```python
+from ghsapi import ghsapi
+
+# create Gen Daq API's object
+gen = ghsapi.GHS()
+
+# connect to mainframe
+gen.ghs_connect(IP_ADDRESS, PORT_NO)
+
+# disconnect from mainframe
+gen.ghs_disconnect()
+```
+
+## Development environment setup
+
+Below are the steps to follow to setup devlopement enviroment for system integration and testing.
+
+### Requirements
+
+- `Python 3.10+`
+- `Anaconda/Miniconda`
+
+### Clone repo
+
+```bash
+git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
+```
+
+### Virtual Environment
+
+```bash
+conda create --name <env> --file spec-file.txt
+```
+
+### Install dependencies
+
+```bash
+pip install -r requirements.txt
+```
+
+## Run example files
+
+Edit files in [examples](./examples) to enter mainframe IP and Port number
+
+```bash
+python examples\FILENAME
+```
+
+## Testing
+
+Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
+
+### Unit test
+
+```bash
+python unittest\FILENAME
+```
+
+### Functional test
+
+```bash
+python functionaltest\FILENAME
+```
```

### Comparing `ghs-gendaqapi-py-1.1.0/README.md` & `ghs-gendaqapi-py-1.2a0/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# GEN DAQ API - Python Driver
-> Setup, control and acquire data from the Genesis Highspeed systems via python.
-
-[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
-
-The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
-
-## Requirements
-
-Python 3.10+
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
-
-```bash
-pip install ghs-gendaqapi-py
-```
-
-## Usage
-
-Refer [examples](./examples) for detailed use cases. 
-Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
-
-```python
-from ghsapi import ghsapi
-
-# create Gen Daq API's object
-gen = ghsapi.GHS()
-
-# connect to mainframe
-gen.ghs_connect(IP_ADDRESS, PORT_NO)
-
-# disconnect from mainframe
-gen.ghs_disconnect()
-```
-
-## Development environment setup
-
-Below are the steps to follow to setup devlopement enviroment for system integration and testing.
-
-### Requirements
-
-- `Python 3.10+`
-- `Anaconda/Miniconda`
-
-### Clone repo
-
-```bash
-git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
-```
-
-### Virtual Environment
-
-```bash
-conda create --name <env> --file spec-file.txt
-```
-
-### Install dependencies
-
-```bash
-pip install -r requirements.txt
-```
-
-## Run example files
-
-Edit files in [examples](./examples) to enter mainframe IP and Port number
-
-```bash
-python examples\FILENAME
-```
-
-## Testing
-
-Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
-
-### Unit test
-
-```bash
-python unittest\FILENAME
-```
-
-### Functional test
-
-```bash
-python functionaltest\FILENAME
-```
+# GEN DAQ API - Python Driver
+> Setup, control and acquire data from the Genesis Highspeed systems via python.
+
+[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
+
+The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
+
+## Requirements
+
+Python 3.10+
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
+
+```bash
+pip install ghs-gendaqapi-py
+```
+
+## Usage
+
+Refer [examples](./examples) for detailed use cases. 
+Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
+
+```python
+from ghsapi import ghsapi
+
+# create Gen Daq API's object
+gen = ghsapi.GHS()
+
+# connect to mainframe
+gen.ghs_connect(IP_ADDRESS, PORT_NO)
+
+# disconnect from mainframe
+gen.ghs_disconnect()
+```
+
+## Development environment setup
+
+Below are the steps to follow to setup devlopement enviroment for system integration and testing.
+
+### Requirements
+
+- `Python 3.10+`
+- `Anaconda/Miniconda`
+
+### Clone repo
+
+```bash
+git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
+```
+
+### Virtual Environment
+
+```bash
+conda create --name <env> --file spec-file.txt
+```
+
+### Install dependencies
+
+```bash
+pip install -r requirements.txt
+```
+
+## Run example files
+
+Edit files in [examples](./examples) to enter mainframe IP and Port number
+
+```bash
+python examples\FILENAME
+```
+
+## Testing
+
+Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
+
+### Unit test
+
+```bash
+python unittest\FILENAME
+```
+
+### Functional test
+
+```bash
+python functionaltest\FILENAME
+```
```

### Comparing `ghs-gendaqapi-py-1.1.0/setup.cfg` & `ghs-gendaqapi-py-1.2a0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2067 6873 2d67 656e 6461 7161 7069   = ghs-gendaqapi
-00000020: 2d70 790d 0a76 6572 7369 6f6e 203d 2031  -py..version = 1
-00000030: 2e31 2e30 0d0a 6175 7468 6f72 203d 2056  .1.0..author = V
-00000040: 6973 6861 6c20 476f 656c 0d0a 6175 7468  ishal Goel..auth
-00000050: 6f72 5f65 6d61 696c 203d 2065 7874 5f56  or_email = ext_V
-00000060: 474f 454c 4068 626d 2e63 6f6d 0d0a 6465  GOEL@hbm.com..de
-00000070: 7363 7269 7074 696f 6e20 3d20 5365 7475  scription = Setu
-00000080: 702c 2063 6f6e 7472 6f6c 2061 6e64 2061  p, control and a
-00000090: 6371 7569 7265 2064 6174 6120 6672 6f6d  cquire data from
-000000a0: 2074 6865 2047 656e 6573 6973 2048 6967   the Genesis Hig
-000000b0: 6873 7065 6564 2073 7973 7465 6d73 2076  hspeed systems v
-000000c0: 6961 2070 7974 686f 6e2e 0d0a 6c6f 6e67  ia python...long
-000000d0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000e0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
-000000f0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000100: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
-00000110: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
-00000120: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
-00000130: 6875 622e 636f 6d2f 6862 6b2d 776f 726c  hub.com/hbk-worl
-00000140: 642f 6768 732d 6765 6e64 6171 6170 692d  d/ghs-gendaqapi-
-00000150: 7079 7468 6f6e 0d0a 7072 6f6a 6563 745f  python..project_
-00000160: 7572 6c73 203d 200d 0a09 446f 6375 6d65  urls = ...Docume
-00000170: 6e74 6174 696f 6e20 3d20 6874 7470 733a  ntation = https:
-00000180: 2f2f 6862 6b2d 776f 726c 642e 6769 7468  //hbk-world.gith
-00000190: 7562 2e69 6f2f 6768 732d 6765 6e64 6171  ub.io/ghs-gendaq
-000001a0: 6170 692d 7079 7468 6f6e 2f68 746d 6c2f  api-python/html/
-000001b0: 696e 6465 782e 6874 6d6c 0d0a 636c 6173  index.html..clas
-000001c0: 7369 6669 6572 7320 3d20 0d0a 0950 726f  sifiers = ...Pro
-000001d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-000001e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-000001f0: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000200: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000210: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-00000220: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000230: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000240: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-00000250: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
-00000260: 7372 630d 0a70 6163 6b61 6765 7320 3d20  src..packages = 
-00000270: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-00000280: 7175 6972 6573 203d 203e 3d33 2e31 300d  quires = >=3.10.
-00000290: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000002a0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000002b0: 6520 3d20 7372 630d 0a0d 0a5b 6567 675f  e = src....[egg_
-000002c0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-000002d0: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000002e0: 300d 0a0d 0a                             0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6768 732d 6765 6e64 6171 6170 692d  = ghs-gendaqapi-
+00000020: 7079 0a76 6572 7369 6f6e 203d 2031 2e32  py.version = 1.2
+00000030: 610a 6175 7468 6f72 203d 2056 6973 6861  a.author = Visha
+00000040: 6c20 476f 656c 0a61 7574 686f 725f 656d  l Goel.author_em
+00000050: 6169 6c20 3d20 6578 745f 5647 4f45 4c40  ail = ext_VGOEL@
+00000060: 6862 6d2e 636f 6d0a 6465 7363 7269 7074  hbm.com.descript
+00000070: 696f 6e20 3d20 5365 7475 702c 2063 6f6e  ion = Setup, con
+00000080: 7472 6f6c 2061 6e64 2061 6371 7569 7265  trol and acquire
+00000090: 2064 6174 6120 6672 6f6d 2074 6865 2047   data from the G
+000000a0: 656e 6573 6973 2048 6967 6873 7065 6564  enesis Highspeed
+000000b0: 2073 7973 7465 6d73 2076 6961 2070 7974   systems via pyt
+000000c0: 686f 6e2e 0a6c 6f6e 675f 6465 7363 7269  hon..long_descri
+000000d0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
+000000e0: 4144 4d45 2e6d 640a 6c6f 6e67 5f64 6573  ADME.md.long_des
+000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000110: 6b64 6f77 6e0a 7572 6c20 3d20 6874 7470  kdown.url = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00000130: 626b 2d77 6f72 6c64 2f67 6873 2d67 656e  bk-world/ghs-gen
+00000140: 6461 7161 7069 2d70 7974 686f 6e0a 7072  daqapi-python.pr
+00000150: 6f6a 6563 745f 7572 6c73 203d 200a 0944  oject_urls = ..D
+00000160: 6f63 756d 656e 7461 7469 6f6e 203d 2068  ocumentation = h
+00000170: 7474 7073 3a2f 2f68 626b 2d77 6f72 6c64  ttps://hbk-world
+00000180: 2e67 6974 6875 622e 696f 2f67 6873 2d67  .github.io/ghs-g
+00000190: 656e 6461 7161 7069 2d70 7974 686f 6e2f  endaqapi-python/
+000001a0: 6874 6d6c 2f69 6e64 6578 2e68 746d 6c0a  html/index.html.
+000001b0: 636c 6173 7369 6669 6572 7320 3d20 0a09  classifiers = ..
+000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001e0: 3a20 330a 094c 6963 656e 7365 203a 3a20  : 3..License :: 
+000001f0: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000200: 4d49 5420 4c69 6365 6e73 650a 094f 7065  MIT License..Ope
+00000210: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000220: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000230: 0a5b 6f70 7469 6f6e 735d 0a70 6163 6b61  .[options].packa
+00000240: 6765 5f64 6972 203d 200a 093d 2073 7263  ge_dir = ..= src
+00000250: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000260: 3a0a 7079 7468 6f6e 5f72 6571 7569 7265  :.python_require
+00000270: 7320 3d20 3e3d 332e 3130 0a0a 5b6f 7074  s = >=3.10..[opt
+00000280: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
+00000290: 6e64 5d0a 7768 6572 6520 3d20 7372 630a  nd].where = src.
+000002a0: 0a5b 6567 675f 696e 666f 5d0a 7461 675f  .[egg_info].tag_
+000002b0: 6275 696c 6420 3d20 0a74 6167 5f64 6174  build = .tag_dat
+000002c0: 6520 3d20 300a 0a                        e = 0..
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/PKG-INFO` & `ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,102 @@
-Metadata-Version: 2.1
-Name: ghs-gendaqapi-py
-Version: 1.1.0
-Summary: Setup, control and acquire data from the Genesis Highspeed systems via python.
-Home-page: https://github.com/hbk-world/ghs-gendaqapi-python
-Author: Vishal Goel
-Author-email: ext_VGOEL@hbm.com
-License: UNKNOWN
-Project-URL: Documentation, https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# GEN DAQ API - Python Driver
-> Setup, control and acquire data from the Genesis Highspeed systems via python.
-
-[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
-
-The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
-
-## Requirements
-
-Python 3.10+
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
-
-```bash
-pip install ghs-gendaqapi-py
-```
-
-## Usage
-
-Refer [examples](./examples) for detailed use cases. 
-Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
-
-```python
-from ghsapi import ghsapi
-
-# create Gen Daq API's object
-gen = ghsapi.GHS()
-
-# connect to mainframe
-gen.ghs_connect(IP_ADDRESS, PORT_NO)
-
-# disconnect from mainframe
-gen.ghs_disconnect()
-```
-
-## Development environment setup
-
-Below are the steps to follow to setup devlopement enviroment for system integration and testing.
-
-### Requirements
-
-- `Python 3.10+`
-- `Anaconda/Miniconda`
-
-### Clone repo
-
-```bash
-git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
-```
-
-### Virtual Environment
-
-```bash
-conda create --name <env> --file spec-file.txt
-```
-
-### Install dependencies
-
-```bash
-pip install -r requirements.txt
-```
-
-## Run example files
-
-Edit files in [examples](./examples) to enter mainframe IP and Port number
-
-```bash
-python examples\FILENAME
-```
-
-## Testing
-
-Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
-
-### Unit test
-
-```bash
-python unittest\FILENAME
-```
-
-### Functional test
-
-```bash
-python functionaltest\FILENAME
-```
-
-
+Metadata-Version: 2.1
+Name: ghs-gendaqapi-py
+Version: 1.2a0
+Summary: Setup, control and acquire data from the Genesis Highspeed systems via python.
+Home-page: https://github.com/hbk-world/ghs-gendaqapi-python
+Author: Vishal Goel
+Author-email: ext_VGOEL@hbm.com
+Project-URL: Documentation, https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# GEN DAQ API - Python Driver
+> Setup, control and acquire data from the Genesis Highspeed systems via python.
+
+[![Build Status](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_apis/build/status/hbk-world.ghs-gendaqapi-python?branchName=main)](https://dev.azure.com/GenesisHighSpeed/GHS%20ESW/_build/latest?definitionId=117&branchName=main)
+
+The GEN DAQ API can be used to control the HBM GEN Series tethered mainframes.
+
+## Requirements
+
+Python 3.10+
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install [GEN DAQ API - Python Driver](https://pypi.org/project/ghs-gendaqapi-py/) package.
+
+```bash
+pip install ghs-gendaqapi-py
+```
+
+## Usage
+
+Refer [examples](./examples) for detailed use cases. 
+Refer [documentation](https://hbk-world.github.io/ghs-gendaqapi-python/html/index.html) for detailed API documentation
+
+```python
+from ghsapi import ghsapi
+
+# create Gen Daq API's object
+gen = ghsapi.GHS()
+
+# connect to mainframe
+gen.ghs_connect(IP_ADDRESS, PORT_NO)
+
+# disconnect from mainframe
+gen.ghs_disconnect()
+```
+
+## Development environment setup
+
+Below are the steps to follow to setup devlopement enviroment for system integration and testing.
+
+### Requirements
+
+- `Python 3.10+`
+- `Anaconda/Miniconda`
+
+### Clone repo
+
+```bash
+git clone https://github.com/hbk-world/ghs-gendaqapi-python.git
+```
+
+### Virtual Environment
+
+```bash
+conda create --name <env> --file spec-file.txt
+```
+
+### Install dependencies
+
+```bash
+pip install -r requirements.txt
+```
+
+## Run example files
+
+Edit files in [examples](./examples) to enter mainframe IP and Port number
+
+```bash
+python examples\FILENAME
+```
+
+## Testing
+
+Edit files in [functionaltest](./functionaltest) to enter mainframe IP and Port number
+
+### Unit test
+
+```bash
+python unittest\FILENAME
+```
+
+### Functional test
+
+```bash
+python functionaltest\FILENAME
+```
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghs_gendaqapi_py.egg-info/SOURCES.txt` & `ghs-gendaqapi-py-1.2a0/src/ghs_gendaqapi_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/ghs_gendaqapi_py.egg-info/dependency_links.txt
 src/ghs_gendaqapi_py.egg-info/top_level.txt
 src/ghsapi/__init__.py
 src/ghsapi/acquisition_api.py
 src/ghsapi/channel_api.py
 src/ghsapi/connection.py
 src/ghsapi/connection_api.py
+src/ghsapi/fieldbus_api.py
 src/ghsapi/ghsapi.py
 src/ghsapi/ghsapi_states.py
 src/ghsapi/json_rpc.py
 src/ghsapi/mainframe_api.py
 src/ghsapi/manage_mainframe_settings.py
 src/ghsapi/manage_recordings_api.py
 src/ghsapi/recorder_api.py
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/__init__.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Import all Gen Daq APIs for integration"""
-
-from . import ghsapi
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Import all Gen Daq APIs for integration"""
+
+from . import ghsapi
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/acquisition_api.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/acquisition_api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,235 +1,235 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Acquisition control module interface.
-
-It is used to control acquisition state of the mainframe.
-"""
-
-from .connection import ConnectionHandler
-from .ghsapi_states import (
-    RETURN_KEY,
-    GHSAcquisitionState,
-    GHSReturnValue,
-    to_string,
-)
-
-
-def start_preview(con_handle: ConnectionHandler) -> str:
-    """Interface to start preview mode.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response("StartPreview", None)
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def stop_preview(con_handle: ConnectionHandler) -> str:
-    """Interface to stop preview mode.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        An String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response("StopPreview", None)
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def start_recording(con_handle: ConnectionHandler) -> str:
-    """Interface to start recording on local storage.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "StartRecording", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def pause_recording(con_handle: ConnectionHandler) -> str:
-    """Interface to pause a started recording.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "PauseRecording", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def resume_recording(con_handle: ConnectionHandler) -> str:
-    """Interface to resume a paused recording.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "ResumeRecording", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def stop_recording(con_handle: ConnectionHandler) -> str:
-    """Interface to stop a started recording.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "StopRecording", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def trigger(con_handle: ConnectionHandler) -> str:
-    """Interface to issue a trigger.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response("Trigger", None)
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def get_acquisition_state(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None]:
-    """Interface to get acquisition state of mainframe.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        Tuple with status and acquisition state of the mainframe.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetAcquisitionState", None
-    )
-    if ("GHSAcquisitionState" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return to_string(response_json[RETURN_KEY], GHSReturnValue), to_string(
-        response_json["GHSAcquisitionState"], GHSAcquisitionState
-    )
-
-
-def get_acquisition_start_time(
-    con_handle: ConnectionHandler,
-) -> tuple[str, int | None, int | None, float | None]:
-    """Interface to get absolute time of the start of acquisition.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        Tuple with status and the absolute time of the start of
-        acquisition.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetAcquisitionStartTime", None
-    )
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "AbsoluteTimeYear",
-                "AbsoluteTimeDay",
-                "AbsoluteTimeSeconds",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["AbsoluteTimeYear"],
-        response_json["AbsoluteTimeDay"],
-        response_json["AbsoluteTimeSeconds"],
-    )
-
-
-def get_acquisition_time(
-    con_handle: ConnectionHandler,
-) -> tuple[str, float | None]:
-    """Interface to get current acquisition time relative to the start
-    of acquistion.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status and current acquisition time relative to
-       the start of acquistion.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetAcquisitionTime", None
-    )
-
-    if ("AcquisitionTime" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["AcquisitionTime"],
-    )
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Acquisition control module interface.
+
+It is used to control acquisition state of the mainframe.
+"""
+
+from .connection import ConnectionHandler
+from .ghsapi_states import (
+    RETURN_KEY,
+    GHSAcquisitionState,
+    GHSReturnValue,
+    to_string,
+)
+
+
+def start_preview(con_handle: ConnectionHandler) -> str:
+    """Interface to start preview mode.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response("StartPreview", None)
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def stop_preview(con_handle: ConnectionHandler) -> str:
+    """Interface to stop preview mode.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        An String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response("StopPreview", None)
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def start_recording(con_handle: ConnectionHandler) -> str:
+    """Interface to start recording on local storage.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "StartRecording", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def pause_recording(con_handle: ConnectionHandler) -> str:
+    """Interface to pause a started recording.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "PauseRecording", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def resume_recording(con_handle: ConnectionHandler) -> str:
+    """Interface to resume a paused recording.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "ResumeRecording", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def stop_recording(con_handle: ConnectionHandler) -> str:
+    """Interface to stop a started recording.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "StopRecording", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def trigger(con_handle: ConnectionHandler) -> str:
+    """Interface to issue a trigger.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response("Trigger", None)
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def get_acquisition_state(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None]:
+    """Interface to get acquisition state of mainframe.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        Tuple with status and acquisition state of the mainframe.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetAcquisitionState", None
+    )
+    if ("GHSAcquisitionState" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return to_string(response_json[RETURN_KEY], GHSReturnValue), to_string(
+        response_json["GHSAcquisitionState"], GHSAcquisitionState
+    )
+
+
+def get_acquisition_start_time(
+    con_handle: ConnectionHandler,
+) -> tuple[str, int | None, int | None, float | None]:
+    """Interface to get absolute time of the start of acquisition.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        Tuple with status and the absolute time of the start of
+        acquisition.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetAcquisitionStartTime", None
+    )
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "AbsoluteTimeYear",
+                "AbsoluteTimeDay",
+                "AbsoluteTimeSeconds",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["AbsoluteTimeYear"],
+        response_json["AbsoluteTimeDay"],
+        response_json["AbsoluteTimeSeconds"],
+    )
+
+
+def get_acquisition_time(
+    con_handle: ConnectionHandler,
+) -> tuple[str, float | None]:
+    """Interface to get current acquisition time relative to the start
+    of acquistion.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status and current acquisition time relative to
+       the start of acquistion.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetAcquisitionTime", None
+    )
+
+    if ("AcquisitionTime" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["AcquisitionTime"],
+    )
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/connection.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/connection.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Implementaion of Connection module."""
-
-import errno
-import socket
-from struct import pack, unpack
-
-from . import json_rpc
-from .ghsapi_states import RETURN_KEY, GHSReturnValue
-
-MAX_CONNECTIONS = 30
-
-
-class ConnectionHandler:
-    """A unique identifier per mainframe connection.
-
-    It is used by all API calls to distinguish between mainframes.
-
-    Attributes:
-        connection_count: An integer count of all connections.
-        api_version_header: Client API header version.
-        request_id: Client request id
-        sock: Socket object
-        ip_address: Mainframe ip address
-    """
-
-    connection_count = 0
-    api_version_header = 1195638785
-
-    def __init__(self):
-        self.request_id = 0
-        self.sock = 0
-        self.ip_address = 0
-
-    def get_num_of_connections(self) -> int:
-        """Get count of all connections."""
-
-        return self.connection_count
-
-    def get_ip_address(self) -> int:
-        """Get ip address of mainframe."""
-
-        return self.ip_address
-
-    def connection_establish(self, ip_address: int, port_num: int) -> int:
-        """Establishes connection to the mainframe.
-
-        Args:
-            ip_address: IP address of the mainframe.
-            port_num: Mainframe port number.
-
-        Returns:
-            Integer value representing connection status code.
-        """
-
-        if not ip_address or not port_num:
-            return GHSReturnValue["NullPtrArgument"]
-        if self.get_num_of_connections() > MAX_CONNECTIONS:
-            return GHSReturnValue["ConnectionFailed"]
-
-        try:
-            self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        except socket.error:
-            return GHSReturnValue["ConnectionFailed"]
-        except RuntimeError:
-            return GHSReturnValue["NOK"]
-
-        try:
-            self.sock.connect((ip_address, port_num))
-        except socket.gaierror:
-            return GHSReturnValue["ConnectionFailed"]
-        except socket.error:
-            return GHSReturnValue["NoConnection"]
-        except RuntimeError:
-            return GHSReturnValue["NOK"]
-
-        self.ip_address = ip_address
-        self.connection_count += 1
-        return GHSReturnValue["OK"]
-
-    def send_request_wait_response(
-        self, method_name: str, method_param: dict | None
-    ) -> dict:
-        """Sends request to the mainframe.
-
-        Args:
-            method_name: Request method name .
-            method_param: Request method parameter.
-
-        Returns:
-            Dict representing response from the mainframe.
-        """
-
-        if not method_name:
-            return {RETURN_KEY: GHSReturnValue["NullPtrArgument"]}
-
-        self.request_id += 1
-        request_json = json_rpc.json_rpc_create_request(
-            self.request_id, method_name, method_param
-        )
-        write_len = len(request_json)
-        header_sx = pack("!I", write_len) + pack("!I", self.api_version_header)
-
-        try:
-            if self.connection_write(header_sx, len(header_sx)) != len(
-                header_sx
-            ):
-                return {RETURN_KEY: GHSReturnValue["NOK"]}
-            if self.connection_write(request_json, write_len) != write_len:
-                return {RETURN_KEY: GHSReturnValue["NOK"]}
-        except OSError:
-            return {RETURN_KEY: GHSReturnValue["NoConnection"]}
-        except RuntimeError:
-            return {RETURN_KEY: GHSReturnValue["NOK"]}
-        except Exception:
-            return {RETURN_KEY: GHSReturnValue["NoConnection"]}
-
-        header_rx_size = 8
-        header_rx = self.connection_read(header_rx_size)
-        if header_rx_size != len(header_rx):
-            return {RETURN_KEY: GHSReturnValue["NOK"]}
-
-        header_rx_packet_header = unpack(">II", header_rx)
-        if header_rx_packet_header[1] != self.api_version_header:
-            return {RETURN_KEY: GHSReturnValue["NOK"]}
-
-        response_json = self.connection_read(header_rx_packet_header[0])
-        return json_rpc.json_rpc_parse_response(self.request_id, response_json)
-
-    def connection_read(self, length: int) -> bytes:
-        """Read message in bytes.
-
-        Args:
-            length: Message length.
-
-        Returns:
-            Bytes of message read.
-
-        Raises:
-            OSError: When socket not connected
-            RuntimeError: When socket connection broken
-        """
-
-        message = b""
-        while len(message) < length:
-            try:
-                packet = self.sock.recv(length - len(message))
-                if not packet:
-                    return None
-                message += packet
-            except socket.error as socket_error:
-                err = socket_error.args[0]
-                if err in (errno.EAGAIN, errno.EWOULDBLOCK):
-                    print("connection_read: No data available")
-                # return None
-                # print("connection_read: No data available")
-                # return None
-        return message
-
-    def connection_write(self, message: bytes, length: int) -> int:
-        """Writes message in bytes.
-
-        Args:
-            message: Message to write.
-            length: Message length.
-
-        Returns:
-            Integer representing bytes written.
-
-        Raises:
-            OSError: When socket not connected
-            RuntimeError: When socket connection broken
-        """
-
-        written_bytes = 0
-        sent_bytes = 0
-
-        while written_bytes < length:
-            try:
-                sent_bytes = self.sock.send(message[written_bytes:])
-            except AttributeError as no_socket:
-                raise OSError("Socket not Connected") from no_socket
-            except socket.gaierror as no_socket:
-                raise OSError("Socket not Connected") from no_socket
-            except RuntimeError as un_specific_error:
-                raise RuntimeError from un_specific_error
-            except Exception as any_exception:
-                raise Exception from any_exception
-            if sent_bytes == 0:
-                raise RuntimeError("Socket Connection Broken")
-            written_bytes = written_bytes + sent_bytes
-            sent_bytes = 0
-
-        return written_bytes
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Implementaion of Connection module."""
+
+import errno
+import socket
+from struct import pack, unpack
+
+from . import json_rpc
+from .ghsapi_states import RETURN_KEY, GHSReturnValue
+
+MAX_CONNECTIONS = 30
+
+
+class ConnectionHandler:
+    """A unique identifier per mainframe connection.
+
+    It is used by all API calls to distinguish between mainframes.
+
+    Attributes:
+        connection_count: An integer count of all connections.
+        api_version_header: Client API header version.
+        request_id: Client request id
+        sock: Socket object
+        ip_address: Mainframe ip address
+    """
+
+    connection_count = 0
+    api_version_header = 1195638785
+
+    def __init__(self):
+        self.request_id = 0
+        self.sock = 0
+        self.ip_address = 0
+
+    def get_num_of_connections(self) -> int:
+        """Get count of all connections."""
+
+        return self.connection_count
+
+    def get_ip_address(self) -> int:
+        """Get ip address of mainframe."""
+
+        return self.ip_address
+
+    def connection_establish(self, ip_address: int, port_num: int) -> int:
+        """Establishes connection to the mainframe.
+
+        Args:
+            ip_address: IP address of the mainframe.
+            port_num: Mainframe port number.
+
+        Returns:
+            Integer value representing connection status code.
+        """
+
+        if not ip_address or not port_num:
+            return GHSReturnValue["NullPtrArgument"]
+        if self.get_num_of_connections() > MAX_CONNECTIONS:
+            return GHSReturnValue["ConnectionFailed"]
+
+        try:
+            self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        except socket.error:
+            return GHSReturnValue["ConnectionFailed"]
+        except RuntimeError:
+            return GHSReturnValue["NOK"]
+
+        try:
+            self.sock.connect((ip_address, port_num))
+        except socket.gaierror:
+            return GHSReturnValue["ConnectionFailed"]
+        except socket.error:
+            return GHSReturnValue["NoConnection"]
+        except RuntimeError:
+            return GHSReturnValue["NOK"]
+
+        self.ip_address = ip_address
+        self.connection_count += 1
+        return GHSReturnValue["OK"]
+
+    def send_request_wait_response(
+        self, method_name: str, method_param: dict | None
+    ) -> dict:
+        """Sends request to the mainframe.
+
+        Args:
+            method_name: Request method name .
+            method_param: Request method parameter.
+
+        Returns:
+            Dict representing response from the mainframe.
+        """
+
+        if not method_name:
+            return {RETURN_KEY: GHSReturnValue["NullPtrArgument"]}
+
+        self.request_id += 1
+        request_json = json_rpc.json_rpc_create_request(
+            self.request_id, method_name, method_param
+        )
+        write_len = len(request_json)
+        header_sx = pack("!I", write_len) + pack("!I", self.api_version_header)
+
+        try:
+            if self.connection_write(header_sx, len(header_sx)) != len(
+                header_sx
+            ):
+                return {RETURN_KEY: GHSReturnValue["NOK"]}
+            if self.connection_write(request_json, write_len) != write_len:
+                return {RETURN_KEY: GHSReturnValue["NOK"]}
+        except OSError:
+            return {RETURN_KEY: GHSReturnValue["NoConnection"]}
+        except RuntimeError:
+            return {RETURN_KEY: GHSReturnValue["NOK"]}
+        except Exception:
+            return {RETURN_KEY: GHSReturnValue["NoConnection"]}
+
+        header_rx_size = 8
+        header_rx = self.connection_read(header_rx_size)
+        if header_rx_size != len(header_rx):
+            return {RETURN_KEY: GHSReturnValue["NOK"]}
+
+        header_rx_packet_header = unpack(">II", header_rx)
+        if header_rx_packet_header[1] != self.api_version_header:
+            return {RETURN_KEY: GHSReturnValue["NOK"]}
+
+        response_json = self.connection_read(header_rx_packet_header[0])
+        return json_rpc.json_rpc_parse_response(self.request_id, response_json)
+
+    def connection_read(self, length: int) -> bytes:
+        """Read message in bytes.
+
+        Args:
+            length: Message length.
+
+        Returns:
+            Bytes of message read.
+
+        Raises:
+            OSError: When socket not connected
+            RuntimeError: When socket connection broken
+        """
+
+        message = b""
+        while len(message) < length:
+            try:
+                packet = self.sock.recv(length - len(message))
+                if not packet:
+                    return None
+                message += packet
+            except socket.error as socket_error:
+                err = socket_error.args[0]
+                if err in (errno.EAGAIN, errno.EWOULDBLOCK):
+                    print("connection_read: No data available")
+                # return None
+                # print("connection_read: No data available")
+                # return None
+        return message
+
+    def connection_write(self, message: bytes, length: int) -> int:
+        """Writes message in bytes.
+
+        Args:
+            message: Message to write.
+            length: Message length.
+
+        Returns:
+            Integer representing bytes written.
+
+        Raises:
+            OSError: When socket not connected
+            RuntimeError: When socket connection broken
+        """
+
+        written_bytes = 0
+        sent_bytes = 0
+
+        while written_bytes < length:
+            try:
+                sent_bytes = self.sock.send(message[written_bytes:])
+            except AttributeError as no_socket:
+                raise OSError("Socket not Connected") from no_socket
+            except socket.gaierror as no_socket:
+                raise OSError("Socket not Connected") from no_socket
+            except RuntimeError as un_specific_error:
+                raise RuntimeError from un_specific_error
+            except Exception as any_exception:
+                raise Exception from any_exception
+            if sent_bytes == 0:
+                raise RuntimeError("Socket Connection Broken")
+            written_bytes = written_bytes + sent_bytes
+            sent_bytes = 0
+
+        return written_bytes
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/ghsapi_states.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/ghsapi_states.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,284 +1,287 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""GHS API States"""
-
-RETURN_KEY = "GHSReturnValue"
-
-# All possible API return values
-GHSReturnValue = {
-    "Reserved": 0,
-    "OK": 1,
-    "NOK": 2,
-    "EmptySlot": 3,
-    "NullPtrArgument": 4,
-    "InvalidSlotID": 5,
-    "SystemNotIdle": 6,
-    "SystemNotRecording": 7,
-    "SystemNotPaused": 8,
-    "InvalidSampleRate": 9,
-    "InvalidHandle": 10,
-    "APIMismatch": 11,
-    "ConnectionFailed": 12,
-    "InvalidIP": 13,
-    "MainframeTimeout": 14,
-    "InsufficientDiskSpace": 15,
-    "CreateRecordingFailed": 16,
-    "NoConnection": 17,
-    "IncompatibleStorage": 18,
-    "RecordingNotFound": 19,
-    "SystemNotInPreview": 20,
-    "AlreadyConnected": 21,
-    "InvalidRecordingName": 22,
-    "InvalidChannelIndex": 23,
-    "InvalidUserMode": 24,
-    "InvalidChannelType": 25,
-    "InvalidTriggerPosition": 26,
-    "InvalidSweepMode": 27,
-    "NoRecordersInMainframe": 28,
-    "InvalidContinuousMode": 29,
-    "InvalidModeForTriggerPosition": 30,
-    "Adapted": 31,
-    "InvalidUTF8Character": 32,
-    "DuplicateChannelName": 33,
-    "InvalidDataType": 34,
-    "MethodNotFound": 35,
-    "InvalidJSONFormat": 36,
-    "UnkownErrorMessage": 37,
-    "FieldBusAlready_Enabled": 39,
-    "CANBusNotFound": 46,
-    "WriteAccessBlocked": 47,
-    "InvalidOutputNumber": 49,
-    "IncompatibleDigitalOutputMode": 50,
-}
-
-GHSAccess = {
-    "ReadOnly": 0,
-    "ReadWrite": 1,
-}
-
-GHSAcquisitionState = {
-    "Reserved": 0,
-    "Recording": 1,
-    "Pause": 2,
-    "SavingData": 3,
-    "Idle": 4,
-    "Preview": 5,
-}
-
-GHSSyncStatus = {
-    "Reserved": 0,
-    "NotSynced": 1,
-    "Syncing": 2,
-    "Synced": 3,
-    "ReSyncing": 4,
-    "NoSignal": 5,
-    "CoarseSynced": 6,
-    "NoGMR1000": 7,
-    "NoOTMC100": 8,
-}
-
-GHSUserMode = {
-    "Reserved": 0,
-    "Sweeps": 1,
-    "Continuous": 2,
-    "Dual": 3,
-}
-
-GHSStorageLocation = {
-    "Reserved": 0,
-    "Remote": 1,
-    "Local1": 2,
-    "Local2": 3,
-    "iSCSI1": 4,
-    "iSCSI2": 5,
-}
-
-GHSSweepRecordingMode = {"Reserved": 0, "Normal": 1, "PreTrigger": 2}
-
-GHSContinuousRecordingMode = {
-    "Reserved": 0,
-    "Standard": 1,
-    "Circular": 2,
-    "Limited": 3,
-    "StopOnTrigger": 4,
-}
-
-GHSChannelType = {
-    "Invalid": 0,
-    "Analog": 1,
-    "Event": 2,
-    "TimerCounter": 3,
-}
-
-GHSAmplifierMode = {
-    "None": -1,
-    "Basic": 0,
-    "Bridge": 1,
-    "Icp": 2,
-    "ThermoCouple": 3,
-    "BasicSensor": 4,
-    "Charge": 5,
-    "Current4_20": 6,
-    "ThermoResistor": 7,
-}
-
-GHSExcitationType = {
-    "Voltage": 0,
-    "Voltage_Sense": 1,
-    "Current": 2,
-    "Voltage_Strobed": 3,
-    "Voltage_Sense_Strobed": 4,
-    "Current_Strobed": 5,
-}
-
-GHSFilterType = {
-    "Bessel": 0,
-    "Butterworth": 1,
-    "Elliptic": 2,
-    "FIR": 3,
-    "IIR": 4,
-    "Wideband": 5,
-    "Bessel_AA": 6,
-    "Butterworth_AA": 7,
-    "SigmaDeltaWB": 8,
-    "SigmaDelta": 9,
-    "BandPass": 10,
-    "FIR3dB": 11,
-}
-
-GHSInputCoupling = {
-    "SingleEndedPositive": 0,
-    "SingleEndedNegative": 1,
-    "Differential": 2,
-    "Current": 3,
-    "FloatingDifferential": 4,
-}
-
-GHSSignalCoupling = {
-    "GND": 0,
-    "DC": 1,
-    "AC": 2,
-    "DC_RMS": 3,
-    "AC_RMS": 4,
-    "DC_Frequency": 5,
-    "AC_Frequency": 6,
-    "DC_TrueRMS": 7,
-    "AC_TrueRMS": 8,
-    "DC_ExternalProbe": 9,
-    "AC_ExternalProbe": 10,
-    "Reference": 11,
-    "ZeroSet": 12,
-    "SinglePrecision": 13,
-    "DoublePrecision": 14,
-    "QuadPrecision": 15,
-    "Charge": 16,
-}
-
-GHSTriggerMode = {
-    "Off": 0,
-    "Basic": 1,
-    "Dual": 2,
-    "Window": 3,
-    "DualWindow": 4,
-    "Sequential": 5,
-    "QualifierBasic": 6,
-    "QualifierDual": 7,
-}
-
-GHSDirection = {"RisingEdge": 0, "FallingEdge": 1}
-
-GHSTimerCounterMode = {
-    "RPMUniDirectional": 0,
-    "RPMBiDirectional": 1,
-    "RPMQuadrature": 2,
-    "FrequencyUniDirectional": 3,
-    "FrequencyBiDirectional": 4,
-    "FrequencyQuadrature": 5,
-    "CountUniDirectional": 6,
-    "CountBiDirectional": 7,
-    "CountQuadrature": 8,
-    "AngleQuadrature": 9,
-    "AngleQuadratureWithRefPos": 10,
-    "AngleUniDirectional": 11,
-    "AngleUniDirectionalWithRefPos": 12,
-    "AngleBiDirectional": 13,
-    "AngleBiDirectionalWithRefPos": 14,
-}
-
-GHSEnableDisable = {
-    "Disable": 0,
-    "Enable": 1,
-}
-
-GHSRecordingDataSource = {
-    "SyncChannels": 0,
-    "SyncRealTimeFormulas": 1,
-}
-
-GHSDigitalOutput = {
-    "Output1": 0,
-    "Output2": 1,
-}
-
-GHSDigitalOutMode = {
-    "Low": 0,
-    "High": 1,
-    "Acquiring": 2,
-    "Trigger": 3,
-    "Alarm": 4,
-}
-
-
-def to_string(value: int, ghs_dict: dict) -> str:
-    """Get status key by value from dictionary."""
-
-    for string_val, return_val in ghs_dict.items():
-        if value == return_val:
-            return string_val
-    if ghs_dict == "GHSChannelType":
-        return "Invalid"
-    return "Reserved"
-
-
-def from_string(key: str, ghs_dict: dict) -> int:
-    """Get status value by key from dictionary."""
-
-    for string_val, return_val in ghs_dict.items():
-        if key == string_val:
-            return return_val
-    return 0
-
-
-# TODO: Formating down from here
-def getDictEntryFromValue(value, ghsDict):
-    for stringReturnVal, returnVal in ghsDict.items():
-        if value == returnVal:
-            return {stringReturnVal: value}
-
-
-def getDictEntryFromKey(key, ghsDict):
-    for stringReturnVal, returnVal in ghsDict.items():
-        if key == stringReturnVal:
-            return {key: returnVal}
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""GHS API States"""
+
+RETURN_KEY = "GHSReturnValue"
+
+# All possible API return values
+GHSReturnValue = {
+    "Reserved": 0,
+    "OK": 1,
+    "NOK": 2,
+    "EmptySlot": 3,
+    "NullPtrArgument": 4,
+    "InvalidSlotID": 5,
+    "SystemNotIdle": 6,
+    "SystemNotRecording": 7,
+    "SystemNotPaused": 8,
+    "InvalidSampleRate": 9,
+    "InvalidHandle": 10,
+    "APIMismatch": 11,
+    "ConnectionFailed": 12,
+    "InvalidIP": 13,
+    "MainframeTimeout": 14,
+    "InsufficientDiskSpace": 15,
+    "CreateRecordingFailed": 16,
+    "NoConnection": 17,
+    "IncompatibleStorage": 18,
+    "RecordingNotFound": 19,
+    "SystemNotInPreview": 20,
+    "AlreadyConnected": 21,
+    "InvalidRecordingName": 22,
+    "InvalidChannelIndex": 23,
+    "InvalidUserMode": 24,
+    "InvalidChannelType": 25,
+    "InvalidTriggerPosition": 26,
+    "InvalidSweepMode": 27,
+    "NoRecordersInMainframe": 28,
+    "InvalidContinuousMode": 29,
+    "InvalidModeForTriggerPosition": 30,
+    "Adapted": 31,
+    "InvalidUTF8Character": 32,
+    "DuplicateChannelName": 33,
+    "InvalidDataType": 34,
+    "MethodNotFound": 35,
+    "InvalidJSONFormat": 36,
+    "UnkownErrorMessage": 37,
+    "FieldBusError_FieldBusAlready_NotConfigured": 38,
+    "FieldBusError_FieldBusAlready_Enabled": 39,
+    "FieldBusError_NoFormulasDeployed" : 43,
+    "FieldBusError_BufferSizeInvalid" : 44,
+    "CANBusNotFound": 46,
+    "WriteAccessBlocked": 47,
+    "InvalidOutputNumber": 49,
+    "IncompatibleDigitalOutputMode": 50,
+}
+
+GHSAccess = {
+    "ReadOnly": 0,
+    "ReadWrite": 1,
+}
+
+GHSAcquisitionState = {
+    "Reserved": 0,
+    "Recording": 1,
+    "Pause": 2,
+    "SavingData": 3,
+    "Idle": 4,
+    "Preview": 5,
+}
+
+GHSSyncStatus = {
+    "Reserved": 0,
+    "NotSynced": 1,
+    "Syncing": 2,
+    "Synced": 3,
+    "ReSyncing": 4,
+    "NoSignal": 5,
+    "CoarseSynced": 6,
+    "NoGMR1000": 7,
+    "NoOTMC100": 8,
+}
+
+GHSUserMode = {
+    "Reserved": 0,
+    "Sweeps": 1,
+    "Continuous": 2,
+    "Dual": 3,
+}
+
+GHSStorageLocation = {
+    "Reserved": 0,
+    "Remote": 1,
+    "Local1": 2,
+    "Local2": 3,
+    "iSCSI1": 4,
+    "iSCSI2": 5,
+}
+
+GHSSweepRecordingMode = {"Reserved": 0, "Normal": 1, "PreTrigger": 2}
+
+GHSContinuousRecordingMode = {
+    "Reserved": 0,
+    "Standard": 1,
+    "Circular": 2,
+    "Limited": 3,
+    "StopOnTrigger": 4,
+}
+
+GHSChannelType = {
+    "Invalid": 0,
+    "Analog": 1,
+    "Event": 2,
+    "TimerCounter": 3,
+}
+
+GHSAmplifierMode = {
+    "None": -1,
+    "Basic": 0,
+    "Bridge": 1,
+    "Icp": 2,
+    "ThermoCouple": 3,
+    "BasicSensor": 4,
+    "Charge": 5,
+    "Current4_20": 6,
+    "ThermoResistor": 7,
+}
+
+GHSExcitationType = {
+    "Voltage": 0,
+    "Voltage_Sense": 1,
+    "Current": 2,
+    "Voltage_Strobed": 3,
+    "Voltage_Sense_Strobed": 4,
+    "Current_Strobed": 5,
+}
+
+GHSFilterType = {
+    "Bessel": 0,
+    "Butterworth": 1,
+    "Elliptic": 2,
+    "FIR": 3,
+    "IIR": 4,
+    "Wideband": 5,
+    "Bessel_AA": 6,
+    "Butterworth_AA": 7,
+    "SigmaDeltaWB": 8,
+    "SigmaDelta": 9,
+    "BandPass": 10,
+    "FIR3dB": 11,
+}
+
+GHSInputCoupling = {
+    "SingleEndedPositive": 0,
+    "SingleEndedNegative": 1,
+    "Differential": 2,
+    "Current": 3,
+    "FloatingDifferential": 4,
+}
+
+GHSSignalCoupling = {
+    "GND": 0,
+    "DC": 1,
+    "AC": 2,
+    "DC_RMS": 3,
+    "AC_RMS": 4,
+    "DC_Frequency": 5,
+    "AC_Frequency": 6,
+    "DC_TrueRMS": 7,
+    "AC_TrueRMS": 8,
+    "DC_ExternalProbe": 9,
+    "AC_ExternalProbe": 10,
+    "Reference": 11,
+    "ZeroSet": 12,
+    "SinglePrecision": 13,
+    "DoublePrecision": 14,
+    "QuadPrecision": 15,
+    "Charge": 16,
+}
+
+GHSTriggerMode = {
+    "Off": 0,
+    "Basic": 1,
+    "Dual": 2,
+    "Window": 3,
+    "DualWindow": 4,
+    "Sequential": 5,
+    "QualifierBasic": 6,
+    "QualifierDual": 7,
+}
+
+GHSDirection = {"RisingEdge": 0, "FallingEdge": 1}
+
+GHSTimerCounterMode = {
+    "RPMUniDirectional": 0,
+    "RPMBiDirectional": 1,
+    "RPMQuadrature": 2,
+    "FrequencyUniDirectional": 3,
+    "FrequencyBiDirectional": 4,
+    "FrequencyQuadrature": 5,
+    "CountUniDirectional": 6,
+    "CountBiDirectional": 7,
+    "CountQuadrature": 8,
+    "AngleQuadrature": 9,
+    "AngleQuadratureWithRefPos": 10,
+    "AngleUniDirectional": 11,
+    "AngleUniDirectionalWithRefPos": 12,
+    "AngleBiDirectional": 13,
+    "AngleBiDirectionalWithRefPos": 14,
+}
+
+GHSEnableDisable = {
+    "Disable": 0,
+    "Enable": 1,
+}
+
+GHSRecordingDataSource = {
+    "SyncChannels": 0,
+    "SyncRealTimeFormulas": 1,
+}
+
+GHSDigitalOutput = {
+    "Output1": 0,
+    "Output2": 1,
+}
+
+GHSDigitalOutMode = {
+    "Low": 0,
+    "High": 1,
+    "Acquiring": 2,
+    "Trigger": 3,
+    "Alarm": 4,
+}
+
+
+def to_string(value: int, ghs_dict: dict) -> str:
+    """Get status key by value from dictionary."""
+
+    for string_val, return_val in ghs_dict.items():
+        if value == return_val:
+            return string_val
+    if ghs_dict == "GHSChannelType":
+        return "Invalid"
+    return "Reserved"
+
+
+def from_string(key: str, ghs_dict: dict) -> int:
+    """Get status value by key from dictionary."""
+
+    for string_val, return_val in ghs_dict.items():
+        if key == string_val:
+            return return_val
+    return 0
+
+
+# TODO: Formating down from here
+def getDictEntryFromValue(value, ghsDict):
+    for stringReturnVal, returnVal in ghsDict.items():
+        if value == returnVal:
+            return {stringReturnVal: value}
+
+
+def getDictEntryFromKey(key, ghsDict):
+    for stringReturnVal, returnVal in ghsDict.items():
+        if key == stringReturnVal:
+            return {key: returnVal}
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/json_rpc.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/json_rpc.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""``Request`` ``Response`` utilities for JSON-RPC client.
-
-Implementation of request and response utility function for JSON-RPC
-client APIs.
-"""
-
-import json
-from collections import OrderedDict
-
-from .ghsapi_states import RETURN_KEY, GHSReturnValue
-
-
-def json_rpc_create_request(
-    request_id: int, method_name: str, method_param: dict | None
-) -> bytes:
-    """``Create`` ``JSON-RPC`` client request"""
-
-    if method_param:
-        json_obj = OrderedDict(
-            [
-                ("jsonrpc", "2.0"),
-                ("method", method_name),
-                ("params", method_param),
-                ("id", request_id),
-            ]
-        )
-    else:
-        json_obj = OrderedDict(
-            [
-                ("jsonrpc", "2.0"),
-                ("method", method_name),
-                ("id", request_id),
-            ]
-        )
-    request_json = json.dumps(json_obj, separators=(",", ":")) + "\0"
-    return request_json.encode("utf-8")
-
-
-def json_rpc_check_errors(request_id: int, response_dict: dict) -> int:
-    """Check for errors in JSON-RPC response"""
-
-    if int(response_dict["id"]) != request_id:
-        return GHSReturnValue["NOK"]
-    # If retreivedRequestID is null means some critical error was
-    # received by the client
-    if response_dict["id"] == "null":
-        try:
-            # if response_dict has key "error"
-            # Depending on the code the message sent to application can
-            # differ
-            error_code = response_dict["error"]["code"]
-            if error_code == -32700:
-                return GHSReturnValue["InvalidJSONFormat"]
-            return GHSReturnValue["UnkownErrorMessage"]
-        except KeyError:
-            return GHSReturnValue["NOK"]
-    # Determine how to handle the message depending on what's in it
-    try:
-        # if response_dict.has_key("error"):
-        error_code = response_dict["error"]["code"]
-        if error_code == -32601:
-            return GHSReturnValue["MethodNotFound"]
-        return GHSReturnValue["UnkownErrorMessage"]
-    except KeyError:
-        return GHSReturnValue["OK"]
-
-
-def json_rpc_parse_response(
-    request_id: int, response_json: bytes | None
-) -> dict:
-    """``Parse`` ``JSON-RPC`` response"""
-
-    parsed_json = json.loads(response_json[:-1])
-    # Check if retrevied JSON has any error code in it
-    return_var = json_rpc_check_errors(request_id, parsed_json)
-    if return_var != GHSReturnValue["OK"]:
-        return {RETURN_KEY: return_var}
-    try:
-        # if parsed_json has key "result"
-        # A result number in the response MUST be a GHSReturnValue
-        # integer, return that
-        if isinstance(parsed_json["result"], int):
-            return {RETURN_KEY: parsed_json["result"]}
-        # A result object in the response MUST have a GHSReturnValue
-        # named parameter, return that
-        try:
-            # if parsed_json["result"] has key "GHSReturnValue"
-            return parsed_json["result"]
-        # Invalid JSON-RPC response
-        except KeyError:
-            return {RETURN_KEY: GHSReturnValue["NOK"]}
-    # Invalid JSON-RPC response
-    except KeyError:
-        return {RETURN_KEY: GHSReturnValue["NOK"]}
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""``Request`` ``Response`` utilities for JSON-RPC client.
+
+Implementation of request and response utility function for JSON-RPC
+client APIs.
+"""
+
+import json
+from collections import OrderedDict
+
+from .ghsapi_states import RETURN_KEY, GHSReturnValue
+
+
+def json_rpc_create_request(
+    request_id: int, method_name: str, method_param: dict | None
+) -> bytes:
+    """``Create`` ``JSON-RPC`` client request"""
+
+    if method_param:
+        json_obj = OrderedDict(
+            [
+                ("jsonrpc", "2.0"),
+                ("method", method_name),
+                ("params", method_param),
+                ("id", request_id),
+            ]
+        )
+    else:
+        json_obj = OrderedDict(
+            [
+                ("jsonrpc", "2.0"),
+                ("method", method_name),
+                ("id", request_id),
+            ]
+        )
+    request_json = json.dumps(json_obj, separators=(",", ":")) + "\0"
+    return request_json.encode("utf-8")
+
+
+def json_rpc_check_errors(request_id: int, response_dict: dict) -> int:
+    """Check for errors in JSON-RPC response"""
+
+    if int(response_dict["id"]) != request_id:
+        return GHSReturnValue["NOK"]
+    # If retreivedRequestID is null means some critical error was
+    # received by the client
+    if response_dict["id"] == "null":
+        try:
+            # if response_dict has key "error"
+            # Depending on the code the message sent to application can
+            # differ
+            error_code = response_dict["error"]["code"]
+            if error_code == -32700:
+                return GHSReturnValue["InvalidJSONFormat"]
+            return GHSReturnValue["UnkownErrorMessage"]
+        except KeyError:
+            return GHSReturnValue["NOK"]
+    # Determine how to handle the message depending on what's in it
+    try:
+        # if response_dict.has_key("error"):
+        error_code = response_dict["error"]["code"]
+        if error_code == -32601:
+            return GHSReturnValue["MethodNotFound"]
+        return GHSReturnValue["UnkownErrorMessage"]
+    except KeyError:
+        return GHSReturnValue["OK"]
+
+
+def json_rpc_parse_response(
+    request_id: int, response_json: bytes | None
+) -> dict:
+    """``Parse`` ``JSON-RPC`` response"""
+
+    parsed_json = json.loads(response_json[:-1])
+    # Check if retrevied JSON has any error code in it
+    return_var = json_rpc_check_errors(request_id, parsed_json)
+    if return_var != GHSReturnValue["OK"]:
+        return {RETURN_KEY: return_var}
+    try:
+        # if parsed_json has key "result"
+        # A result number in the response MUST be a GHSReturnValue
+        # integer, return that
+        if isinstance(parsed_json["result"], int):
+            return {RETURN_KEY: parsed_json["result"]}
+        # A result object in the response MUST have a GHSReturnValue
+        # named parameter, return that
+        try:
+            # if parsed_json["result"] has key "GHSReturnValue"
+            return parsed_json["result"]
+        # Invalid JSON-RPC response
+        except KeyError:
+            return {RETURN_KEY: GHSReturnValue["NOK"]}
+    # Invalid JSON-RPC response
+    except KeyError:
+        return {RETURN_KEY: GHSReturnValue["NOK"]}
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/mainframe_api.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/mainframe_api.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Mainframe module interface."""
-
-from .connection import ConnectionHandler
-from .ghsapi_states import (
-    RETURN_KEY,
-    GHSReturnValue,
-    GHSSyncStatus,
-    GHSUserMode,
-    from_string,
-    to_string,
-)
-
-
-def get_mainframe_info(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None, str | None, str | None, str | None]:
-    """Interface to determine type, name, serial number and firmware
-    version information for the connected mainframe.
-
-    The mainframeType, mainframeName, serialNumber and firmwareVersion
-    parameters are UTF-8 encoded.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with type, name, serial number and firmware version.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetMainframeInformation", None
-    )
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "MainframeType",
-                "MainframeName",
-                "SerialNumber",
-                "FirmwareVersion",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["MainframeType"],
-        response_json["MainframeName"],
-        response_json["SerialNumber"],
-        response_json["FirmwareVersion"],
-    )
-
-
-def get_disk_space(
-    con_handle: ConnectionHandler,
-) -> tuple[str, float | None, float | None]:
-    """Interface to get total and available mainframe internal disk
-    space.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status, total and available mainframe internal
-       disk.
-    """
-
-    response_json = con_handle.send_request_wait_response("DiskSpace", None)
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "TotalSize",
-                "AvailableSize",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["TotalSize"],
-        response_json["AvailableSize"],
-    )
-
-
-def get_slot_count(
-    con_handle: ConnectionHandler,
-) -> tuple[str, int | None]:
-    """Interface to get the number of slots in the mainframe.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status and number of slots in the mainframe.
-    """
-
-    response_json = con_handle.send_request_wait_response("GetSlotCount", None)
-
-    if ("SlotCount" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["SlotCount"],
-    )
-
-
-def get_sync_status(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None]:
-    """Interface to determine the mainframe sync status.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status and sync status
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetSyncStatus", None
-    )
-
-    if ("SyncStatus" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        to_string(response_json["SyncStatus"], GHSSyncStatus),
-    )
-
-
-def get_user_mode(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None]:
-    """Interface to retrieve the user mode.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status and user mode.
-    """
-
-    response_json = con_handle.send_request_wait_response("GetUserMode", None)
-
-    if ("UserMode" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        to_string(response_json["UserMode"], GHSUserMode),
-    )
-
-
-def set_user_mode(con_handle: ConnectionHandler, user_mode: str | int) -> str:
-    """Interface to set the user mode.
-
-    The system needs to be idle before calling this function.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        user_mode: The desired user mode.
-
-    Returns:
-       String value representing request status.
-    """
-
-    if isinstance(user_mode, str) and user_mode in GHSUserMode:
-        user_mode_dict = {"UserMode": from_string(user_mode, GHSUserMode)}
-
-    elif isinstance(user_mode, int) and user_mode in GHSUserMode.values():
-        user_mode_dict = {"UserMode": user_mode}
-
-    else:
-        return "InvalidUserMode"
-
-    response_json = con_handle.send_request_wait_response(
-        "SetUserMode", user_mode_dict
-    )
-
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def identity(con_handle: ConnectionHandler, identity_flag: bool) -> str:
-    """Interface to enable or disable the identification sound of the
-    connected mainframe.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        identity_flag: Enable or disable flag.
-
-    Returns:
-       String value representing request status.
-    """
-
-    identity_dict = {"Identify": 1} if identity_flag else {"Identify": 0}
-
-    response_json = con_handle.send_request_wait_response(
-        "Identify", identity_dict
-    )
-
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Mainframe module interface."""
+
+from .connection import ConnectionHandler
+from .ghsapi_states import (
+    RETURN_KEY,
+    GHSReturnValue,
+    GHSSyncStatus,
+    GHSUserMode,
+    from_string,
+    to_string,
+)
+
+
+def get_mainframe_info(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None, str | None, str | None, str | None]:
+    """Interface to determine type, name, serial number and firmware
+    version information for the connected mainframe.
+
+    The mainframeType, mainframeName, serialNumber and firmwareVersion
+    parameters are UTF-8 encoded.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with type, name, serial number and firmware version.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetMainframeInformation", None
+    )
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "MainframeType",
+                "MainframeName",
+                "SerialNumber",
+                "FirmwareVersion",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["MainframeType"],
+        response_json["MainframeName"],
+        response_json["SerialNumber"],
+        response_json["FirmwareVersion"],
+    )
+
+
+def get_disk_space(
+    con_handle: ConnectionHandler,
+) -> tuple[str, float | None, float | None]:
+    """Interface to get total and available mainframe internal disk
+    space.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status, total and available mainframe internal
+       disk.
+    """
+
+    response_json = con_handle.send_request_wait_response("DiskSpace", None)
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "TotalSize",
+                "AvailableSize",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["TotalSize"],
+        response_json["AvailableSize"],
+    )
+
+
+def get_slot_count(
+    con_handle: ConnectionHandler,
+) -> tuple[str, int | None]:
+    """Interface to get the number of slots in the mainframe.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status and number of slots in the mainframe.
+    """
+
+    response_json = con_handle.send_request_wait_response("GetSlotCount", None)
+
+    if ("SlotCount" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["SlotCount"],
+    )
+
+
+def get_sync_status(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None]:
+    """Interface to determine the mainframe sync status.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status and sync status
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetSyncStatus", None
+    )
+
+    if ("SyncStatus" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        to_string(response_json["SyncStatus"], GHSSyncStatus),
+    )
+
+
+def get_user_mode(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None]:
+    """Interface to retrieve the user mode.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status and user mode.
+    """
+
+    response_json = con_handle.send_request_wait_response("GetUserMode", None)
+
+    if ("UserMode" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        to_string(response_json["UserMode"], GHSUserMode),
+    )
+
+
+def set_user_mode(con_handle: ConnectionHandler, user_mode: str | int) -> str:
+    """Interface to set the user mode.
+
+    The system needs to be idle before calling this function.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        user_mode: The desired user mode.
+
+    Returns:
+       String value representing request status.
+    """
+
+    if isinstance(user_mode, str) and user_mode in GHSUserMode:
+        user_mode_dict = {"UserMode": from_string(user_mode, GHSUserMode)}
+
+    elif isinstance(user_mode, int) and user_mode in GHSUserMode.values():
+        user_mode_dict = {"UserMode": user_mode}
+
+    else:
+        return "InvalidUserMode"
+
+    response_json = con_handle.send_request_wait_response(
+        "SetUserMode", user_mode_dict
+    )
+
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def identity(con_handle: ConnectionHandler, identity_flag: bool) -> str:
+    """Interface to enable or disable the identification sound of the
+    connected mainframe.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        identity_flag: Enable or disable flag.
+
+    Returns:
+       String value representing request status.
+    """
+
+    identity_dict = {"Identify": 1} if identity_flag else {"Identify": 0}
+
+    response_json = con_handle.send_request_wait_response(
+        "Identify", identity_dict
+    )
+
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/manage_mainframe_settings.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/manage_mainframe_settings.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Manage mainframe settings module interface."""
-
-from .connection import ConnectionHandler
-from .ghsapi_states import RETURN_KEY, GHSReturnValue, to_string
-
-
-def apply_persisted_settings(con_handle: ConnectionHandler) -> str:
-    """A mainframe might contain persisted settings (being applied upon
-    boot). This method re-applies these settings. In Perception this
-    maps on the 'Configured boot' feature.
-
-    The system needs to be idle before calling this function.
-    This function overwrites any previously set settings and / or
-    persisted settings.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "ApplyPersistedSettings", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def persist_current_settings(con_handle: ConnectionHandler) -> str:
-    """Persists the current mainframe settings.
-
-    The persisted mainframe settings are applied upon a mainframe boot.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "PersistCurrentSettings", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def get_current_settings(
-    con_handle: ConnectionHandler,
-) -> tuple[str, bytes | None, int | None]:
-    """Retrieves the current mainframe settings as a blob.
-
-    As this blob can be of variable size, it is upon the caller to
-    ensure reading the correct amount of memory.
-    Memory for this blob is allocated by the API.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        Tuple with status, base name and index of the recording file.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetCurrentSettings", None
-    )
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "Size",
-                "Blob",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["Blob"],
-        response_json["Size"],
-    )
-
-
-def set_current_settings(
-    con_handle: ConnectionHandler, blob: bytes, blob_size: int
-) -> str:
-    """Applies the mainframe settings contained in the input argument.
-
-    Note that this function overwrites any previously set settings and
-    / or applied setup.
-
-    The system needs to be idle before calling this function.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        blob: Settings blob.
-        blob_size: Size of the settings blob.
-
-    Returns:
-        String value representing request status.
-    """
-
-    if not blob or not blob_size:
-        return "NullPtrArgument"
-
-    current_settings_dict = {"Blob": blob, "Size": blob_size}
-    response_json = con_handle.send_request_wait_response(
-        "SetCurrentSettings", current_settings_dict
-    )
-
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Manage mainframe settings module interface."""
+
+from .connection import ConnectionHandler
+from .ghsapi_states import RETURN_KEY, GHSReturnValue, to_string
+
+
+def apply_persisted_settings(con_handle: ConnectionHandler) -> str:
+    """A mainframe might contain persisted settings (being applied upon
+    boot). This method re-applies these settings. In Perception this
+    maps on the 'Configured boot' feature.
+
+    The system needs to be idle before calling this function.
+    This function overwrites any previously set settings and / or
+    persisted settings.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "ApplyPersistedSettings", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def persist_current_settings(con_handle: ConnectionHandler) -> str:
+    """Persists the current mainframe settings.
+
+    The persisted mainframe settings are applied upon a mainframe boot.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "PersistCurrentSettings", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def get_current_settings(
+    con_handle: ConnectionHandler,
+) -> tuple[str, bytes | None, int | None]:
+    """Retrieves the current mainframe settings as a blob.
+
+    As this blob can be of variable size, it is upon the caller to
+    ensure reading the correct amount of memory.
+    Memory for this blob is allocated by the API.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        Tuple with status, base name and index of the recording file.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetCurrentSettings", None
+    )
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "Size",
+                "Blob",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["Blob"],
+        response_json["Size"],
+    )
+
+
+def set_current_settings(
+    con_handle: ConnectionHandler, blob: bytes, blob_size: int
+) -> str:
+    """Applies the mainframe settings contained in the input argument.
+
+    Note that this function overwrites any previously set settings and
+    / or applied setup.
+
+    The system needs to be idle before calling this function.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        blob: Settings blob.
+        blob_size: Size of the settings blob.
+
+    Returns:
+        String value representing request status.
+    """
+
+    if not blob or not blob_size:
+        return "NullPtrArgument"
+
+    current_settings_dict = {"Blob": blob, "Size": blob_size}
+    response_json = con_handle.send_request_wait_response(
+        "SetCurrentSettings", current_settings_dict
+    )
+
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
```

### Comparing `ghs-gendaqapi-py-1.1.0/src/ghsapi/manage_recordings_api.py` & `ghs-gendaqapi-py-1.2a0/src/ghsapi/manage_recordings_api.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,362 +1,362 @@
-# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
-# Schutweg 15a
-# 5145 NP Waalwijk
-# The Netherlands
-# http://www.hbm.com
-
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in
-# all copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-"""Manage recordings module interface."""
-
-from .connection import ConnectionHandler
-from .ghsapi_states import (
-    RETURN_KEY,
-    GHSEnableDisable,
-    GHSRecordingDataSource,
-    GHSReturnValue,
-    GHSStorageLocation,
-    from_string,
-    to_string,
-)
-
-
-def delete_all_recordings(con_handle: ConnectionHandler) -> str:
-    """Interface to deletes all recordings from local mainframe storage
-
-    Recordings are deleted asynchronously.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "DeleteAllRecordings", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def delete_last_recording(con_handle: ConnectionHandler) -> str:
-    """Interface to delete the most recent recording from local
-    mainframe storage.
-
-    Recordings are deleted asynchronously.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       String value representing request status.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "DeleteLastRecording", None
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def get_recording_name(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None, int | None]:
-    """Interface to get recording base name and recording index of the
-    last recording file.
-
-    The recording base name parameter is UTF-8 encoded.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-        Tuple with status, base name and index of the recording file.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetRecordingName", None
-    )
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "RecordingIndex",
-                "RecordingName",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        response_json["RecordingName"],
-        response_json["RecordingIndex"],
-    )
-
-
-def set_recording_name(
-    con_handle: ConnectionHandler, recording_name: str, recording_index: int
-) -> str:
-    """Interface to set the recording base name and recording index for
-    the next recording file.
-
-    The system needs to be idle before calling this function.
-    The recording base name parameter must be UTF-8 encoded.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        recording_name: The desired base name of the recording file.
-        recording_index: The desired index of the recording file.
-
-    Returns:
-       String value representing request status.
-    """
-
-    if not recording_name or not recording_index:
-        return "NullPtrArgument"
-
-    recording_name_dict = {
-        "RecordingBaseName": recording_name,
-        "RecordingIndex": recording_index,
-    }
-
-    response_json = con_handle.send_request_wait_response(
-        "SetRecordingName", recording_name_dict
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def get_storage_location(
-    con_handle: ConnectionHandler,
-) -> tuple[str, str | None]:
-    """Interface to retrieve the storage location.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-
-    Returns:
-       Tuple with status and storage location.
-    """
-
-    response_json = con_handle.send_request_wait_response(
-        "GetStorageLocation", None
-    )
-
-    if ("StorageLocation" not in response_json) or (
-        response_json[RETURN_KEY] != GHSReturnValue["OK"]
-    ):
-        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        to_string(response_json["StorageLocation"], GHSStorageLocation),
-    )
-
-
-def set_storage_location(
-    con_handle: ConnectionHandler, storage_location: str | int
-) -> str:
-    """Interface to set the storage location.
-
-    The system needs to be idle before calling this function.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        storage_location: The desired storage location.
-
-    Returns:
-       String value representing request status.
-    """
-
-    if not storage_location:
-        return "NullPtrArgument"
-
-    if (
-        isinstance(storage_location, str)
-        and storage_location in GHSStorageLocation
-    ):
-        storage_loc_dict = {
-            "StorageLocation": from_string(
-                storage_location, GHSStorageLocation
-            )
-        }
-
-    elif (
-        isinstance(storage_location, int)
-        and storage_location in GHSStorageLocation.values()
-    ):
-        storage_loc_dict = {"StorageLocation": storage_location}
-
-    else:
-        return "IncompatibleStorage"
-
-    response_json = con_handle.send_request_wait_response(
-        "SetStorageLocation", storage_loc_dict
-    )
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
-
-
-def get_high_low_rate_storage_enabled(
-    con_handle: ConnectionHandler,
-    source: str | int,
-    slot_id: str,
-) -> tuple[str, str | None, str | None]:
-    """Interface to retrieve storage enabled status of high and low
-    rate data for the specified recording data source.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        source: The recording data source to retrieve the storage
-        enabled status for.
-        slot_id: The slot containing the recorder to retrieve the
-        storage enabled status for (e.g. 'A' for the first slot). This
-        argument is only evaluated for recorder based data sources.
-
-    Returns:
-        Tuple with status, flag to indicate if high and low rate data
-        is stored.
-    """
-
-    if not source or not slot_id:
-        return "NullPtrArgument"
-
-    if isinstance(source, str) and source in GHSRecordingDataSource:
-        source_slot_dict = {
-            "Source": from_string(source, GHSRecordingDataSource),
-            "SlotId": slot_id,
-        }
-
-    elif isinstance(source, int) and source in GHSRecordingDataSource.values():
-        source_slot_dict = {"Source": source, "SlotId": slot_id}
-
-    else:
-        return "InvalidDataType"
-
-    response_json = con_handle.send_request_wait_response(
-        "GetHighLowRateStorageEnabled", source_slot_dict
-    )
-
-    if (
-        not any(
-            key in response_json
-            for key in [
-                "HighRateEnable",
-                "LowRateEnable",
-            ]
-        )
-    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
-        return (
-            to_string(response_json[RETURN_KEY], GHSReturnValue),
-            None,
-            None,
-        )
-    return (
-        to_string(response_json[RETURN_KEY], GHSReturnValue),
-        to_string(response_json["HighRateEnable"], GHSEnableDisable),
-        to_string(response_json["LowRateEnable"], GHSEnableDisable),
-    )
-
-
-def set_high_low_rate_storage_enabled(
-    con_handle: ConnectionHandler,
-    source: str | int,
-    slot_id: str,
-    high_rate_enabled: str | int,
-    low_rate_enabled: str | int,
-) -> str:
-    """Interface to enable/disable storage of high and low rate data
-    for the specified recording data source.
-
-    The system needs to be idle before calling this function.
-
-    Args:
-        con_handle: A unique identifier per mainframe connection.
-        source: The recording data source to retrieve the storage
-        enabled status for.
-        slot_id: The slot containing the recorder to retrieve the
-        storage enabled status for (e.g. 'A' for the first slot). This
-        argument is only evaluated for recorder based data sources.
-        high_rate_enabled: Enable/disable storage of high rate data.
-        low_rate_enabled: Enable/disable storage of low rate data.
-
-    Returns:
-        String value representing request status.
-    """
-
-    if (
-        not source
-        or not slot_id
-        or not high_rate_enabled
-        or not low_rate_enabled
-    ):
-        return "NullPtrArgument"
-
-    if isinstance(source, str) and source in GHSRecordingDataSource:
-        source = from_string(source, GHSRecordingDataSource)
-
-    elif isinstance(source, int) and source in GHSRecordingDataSource.values():
-        pass
-
-    else:
-        return "InvalidDataType"
-
-    if (
-        isinstance(high_rate_enabled, str)
-        and high_rate_enabled in GHSEnableDisable
-    ):
-        high_rate_enabled = from_string(high_rate_enabled, GHSEnableDisable)
-
-    elif (
-        isinstance(high_rate_enabled, int)
-        and high_rate_enabled in GHSEnableDisable.values()
-    ):
-        pass
-
-    else:
-        return "InvalidDataType"
-
-    if (
-        isinstance(low_rate_enabled, str)
-        and low_rate_enabled in GHSEnableDisable
-    ):
-        low_rate_enabled = from_string(low_rate_enabled, GHSEnableDisable)
-
-    elif (
-        isinstance(low_rate_enabled, int)
-        and low_rate_enabled in GHSEnableDisable.values()
-    ):
-        pass
-
-    else:
-        return "InvalidDataType"
-
-    source_slot_dict = {
-        "Source": source,
-        "SlotId": slot_id,
-        "HighRateEnable": high_rate_enabled,
-        "LowRateEnable": low_rate_enabled,
-    }
-
-    response_json = con_handle.send_request_wait_response(
-        "SetHighLowRateStorageEnabled", source_slot_dict
-    )
-
-    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+# Copyright (C) 2022 Hottinger Bruel and Kjaer Benelux B.V.
+# Schutweg 15a
+# 5145 NP Waalwijk
+# The Netherlands
+# http://www.hbm.com
+
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in
+# all copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+"""Manage recordings module interface."""
+
+from .connection import ConnectionHandler
+from .ghsapi_states import (
+    RETURN_KEY,
+    GHSEnableDisable,
+    GHSRecordingDataSource,
+    GHSReturnValue,
+    GHSStorageLocation,
+    from_string,
+    to_string,
+)
+
+
+def delete_all_recordings(con_handle: ConnectionHandler) -> str:
+    """Interface to deletes all recordings from local mainframe storage
+
+    Recordings are deleted asynchronously.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "DeleteAllRecordings", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def delete_last_recording(con_handle: ConnectionHandler) -> str:
+    """Interface to delete the most recent recording from local
+    mainframe storage.
+
+    Recordings are deleted asynchronously.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       String value representing request status.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "DeleteLastRecording", None
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def get_recording_name(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None, int | None]:
+    """Interface to get recording base name and recording index of the
+    last recording file.
+
+    The recording base name parameter is UTF-8 encoded.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+        Tuple with status, base name and index of the recording file.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetRecordingName", None
+    )
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "RecordingIndex",
+                "RecordingName",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        response_json["RecordingName"],
+        response_json["RecordingIndex"],
+    )
+
+
+def set_recording_name(
+    con_handle: ConnectionHandler, recording_name: str, recording_index: int
+) -> str:
+    """Interface to set the recording base name and recording index for
+    the next recording file.
+
+    The system needs to be idle before calling this function.
+    The recording base name parameter must be UTF-8 encoded.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        recording_name: The desired base name of the recording file.
+        recording_index: The desired index of the recording file.
+
+    Returns:
+       String value representing request status.
+    """
+
+    if not recording_name or not recording_index:
+        return "NullPtrArgument"
+
+    recording_name_dict = {
+        "RecordingBaseName": recording_name,
+        "RecordingIndex": recording_index,
+    }
+
+    response_json = con_handle.send_request_wait_response(
+        "SetRecordingName", recording_name_dict
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def get_storage_location(
+    con_handle: ConnectionHandler,
+) -> tuple[str, str | None]:
+    """Interface to retrieve the storage location.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+
+    Returns:
+       Tuple with status and storage location.
+    """
+
+    response_json = con_handle.send_request_wait_response(
+        "GetStorageLocation", None
+    )
+
+    if ("StorageLocation" not in response_json) or (
+        response_json[RETURN_KEY] != GHSReturnValue["OK"]
+    ):
+        return to_string(response_json[RETURN_KEY], GHSReturnValue), None
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        to_string(response_json["StorageLocation"], GHSStorageLocation),
+    )
+
+
+def set_storage_location(
+    con_handle: ConnectionHandler, storage_location: str | int
+) -> str:
+    """Interface to set the storage location.
+
+    The system needs to be idle before calling this function.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        storage_location: The desired storage location.
+
+    Returns:
+       String value representing request status.
+    """
+
+    if not storage_location:
+        return "NullPtrArgument"
+
+    if (
+        isinstance(storage_location, str)
+        and storage_location in GHSStorageLocation
+    ):
+        storage_loc_dict = {
+            "StorageLocation": from_string(
+                storage_location, GHSStorageLocation
+            )
+        }
+
+    elif (
+        isinstance(storage_location, int)
+        and storage_location in GHSStorageLocation.values()
+    ):
+        storage_loc_dict = {"StorageLocation": storage_location}
+
+    else:
+        return "IncompatibleStorage"
+
+    response_json = con_handle.send_request_wait_response(
+        "SetStorageLocation", storage_loc_dict
+    )
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
+
+
+def get_high_low_rate_storage_enabled(
+    con_handle: ConnectionHandler,
+    source: str | int,
+    slot_id: str,
+) -> tuple[str, str | None, str | None]:
+    """Interface to retrieve storage enabled status of high and low
+    rate data for the specified recording data source.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        source: The recording data source to retrieve the storage
+        enabled status for.
+        slot_id: The slot containing the recorder to retrieve the
+        storage enabled status for (e.g. 'A' for the first slot). This
+        argument is only evaluated for recorder based data sources.
+
+    Returns:
+        Tuple with status, flag to indicate if high and low rate data
+        is stored.
+    """
+
+    if not source or not slot_id:
+        return "NullPtrArgument"
+
+    if isinstance(source, str) and source in GHSRecordingDataSource:
+        source_slot_dict = {
+            "Source": from_string(source, GHSRecordingDataSource),
+            "SlotId": slot_id,
+        }
+
+    elif isinstance(source, int) and source in GHSRecordingDataSource.values():
+        source_slot_dict = {"Source": source, "SlotId": slot_id}
+
+    else:
+        return "InvalidDataType"
+
+    response_json = con_handle.send_request_wait_response(
+        "GetHighLowRateStorageEnabled", source_slot_dict
+    )
+
+    if (
+        not any(
+            key in response_json
+            for key in [
+                "HighRateEnable",
+                "LowRateEnable",
+            ]
+        )
+    ) or (response_json[RETURN_KEY] != GHSReturnValue["OK"]):
+        return (
+            to_string(response_json[RETURN_KEY], GHSReturnValue),
+            None,
+            None,
+        )
+    return (
+        to_string(response_json[RETURN_KEY], GHSReturnValue),
+        to_string(response_json["HighRateEnable"], GHSEnableDisable),
+        to_string(response_json["LowRateEnable"], GHSEnableDisable),
+    )
+
+
+def set_high_low_rate_storage_enabled(
+    con_handle: ConnectionHandler,
+    source: str | int,
+    slot_id: str,
+    high_rate_enabled: str | int,
+    low_rate_enabled: str | int,
+) -> str:
+    """Interface to enable/disable storage of high and low rate data
+    for the specified recording data source.
+
+    The system needs to be idle before calling this function.
+
+    Args:
+        con_handle: A unique identifier per mainframe connection.
+        source: The recording data source to retrieve the storage
+        enabled status for.
+        slot_id: The slot containing the recorder to retrieve the
+        storage enabled status for (e.g. 'A' for the first slot). This
+        argument is only evaluated for recorder based data sources.
+        high_rate_enabled: Enable/disable storage of high rate data.
+        low_rate_enabled: Enable/disable storage of low rate data.
+
+    Returns:
+        String value representing request status.
+    """
+
+    if (
+        not source
+        or not slot_id
+        or not high_rate_enabled
+        or not low_rate_enabled
+    ):
+        return "NullPtrArgument"
+
+    if isinstance(source, str) and source in GHSRecordingDataSource:
+        source = from_string(source, GHSRecordingDataSource)
+
+    elif isinstance(source, int) and source in GHSRecordingDataSource.values():
+        pass
+
+    else:
+        return "InvalidDataType"
+
+    if (
+        isinstance(high_rate_enabled, str)
+        and high_rate_enabled in GHSEnableDisable
+    ):
+        high_rate_enabled = from_string(high_rate_enabled, GHSEnableDisable)
+
+    elif (
+        isinstance(high_rate_enabled, int)
+        and high_rate_enabled in GHSEnableDisable.values()
+    ):
+        pass
+
+    else:
+        return "InvalidDataType"
+
+    if (
+        isinstance(low_rate_enabled, str)
+        and low_rate_enabled in GHSEnableDisable
+    ):
+        low_rate_enabled = from_string(low_rate_enabled, GHSEnableDisable)
+
+    elif (
+        isinstance(low_rate_enabled, int)
+        and low_rate_enabled in GHSEnableDisable.values()
+    ):
+        pass
+
+    else:
+        return "InvalidDataType"
+
+    source_slot_dict = {
+        "Source": source,
+        "SlotId": slot_id,
+        "HighRateEnable": high_rate_enabled,
+        "LowRateEnable": low_rate_enabled,
+    }
+
+    response_json = con_handle.send_request_wait_response(
+        "SetHighLowRateStorageEnabled", source_slot_dict
+    )
+
+    return to_string(response_json[RETURN_KEY], GHSReturnValue)
```

