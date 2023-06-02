# Comparing `tmp/quao-0.1.9.tar.gz` & `tmp/quao-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quao-0.1.9.tar", last modified: Wed May 31 04:34:34 2023, max compression
+gzip compressed data, was "quao-0.2.0.tar", last modified: Fri Jun  2 11:42:27 2023, max compression
```

## Comparing `quao-0.1.9.tar` & `quao-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.387019 quao-0.1.9/
--rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     2839 2023-05-31 04:34:34.386019 quao-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.1.9/README.md
--rw-rw-rw-   0        0        0      846 2023-05-31 04:34:14.000000 quao-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 04:34:34.387019 quao-0.1.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.345421 quao-0.1.9/src/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.9/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.351419 quao-0.1.9/src/quao/
--rw-rw-rw-   0        0        0      134 2023-04-25 02:47:26.000000 quao-0.1.9/src/quao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.373020 quao-0.1.9/src/quao/algorithms/
--rw-rw-rw-   0        0        0        2 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/algorithms/__init__.py
--rw-rw-rw-   0        0        0     5305 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/algorithms/shor.py
--rw-rw-rw-   0        0        0     3475 2023-05-31 04:28:29.000000 quao-0.1.9/src/quao/backend.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.378020 quao-0.1.9/src/quao/config/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:56:58.000000 quao-0.1.9/src/quao/config/__init__.py
--rw-rw-rw-   0        0        0      189 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/config/loggingConfig.py
--rw-rw-rw-   0        0        0      179 2023-05-31 04:07:43.000000 quao-0.1.9/src/quao/config/threadConfig.py
--rw-rw-rw-   0        0        0      529 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/dataUtils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.379019 quao-0.1.9/src/quao/enum/
--rw-rw-rw-   0        0        0      200 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/enum/providerType.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.382022 quao-0.1.9/src/quao/sdk/
--rw-rw-rw-   0        0        0        2 2023-04-25 02:47:26.000000 quao-0.1.9/src/quao/sdk/__init__.py
--rw-rw-rw-   0        0        0     6415 2023-05-31 03:35:27.000000 quao-0.1.9/src/quao/sdk/qiskit.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.384020 quao-0.1.9/src/quao/status/
--rw-rw-rw-   0        0        0        0 2023-05-29 11:57:12.000000 quao-0.1.9/src/quao/status/__init__.py
--rw-rw-rw-   0        0        0     2450 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/status/qiskit_status.py
--rw-rw-rw-   0        0        0     1636 2023-05-31 01:58:09.000000 quao-0.1.9/src/quao/utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-31 04:34:34.370067 quao-0.1.9/src/quao.egg-info/
--rw-rw-rw-   0        0        0     2839 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 04:34:34.000000 quao-0.1.9/src/quao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.035174 quao-0.2.0/
+-rw-rw-rw-   0        0        0     1111 2023-04-27 03:39:26.000000 quao-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2839 2023-06-02 11:42:27.034173 quao-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1163 2023-04-27 03:33:31.000000 quao-0.2.0/README.md
+-rw-rw-rw-   0        0        0      916 2023-06-02 11:41:53.000000 quao-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-02 11:42:27.035174 quao-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.929206 quao-0.2.0/src/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.932443 quao-0.2.0/src/quao/
+-rw-rw-rw-   0        0        0      203 2023-06-02 11:41:53.000000 quao-0.2.0/src/quao/__init__.py
+-rw-rw-rw-   0        0        0     5614 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/backend.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.964175 quao-0.2.0/src/quao/config/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/config/__init__.py
+-rw-rw-rw-   0        0        0      190 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/config/logging_config.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.965176 quao-0.2.0/src/quao/data/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.968175 quao-0.2.0/src/quao/data/job/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/job/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/data/job/job_response.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.973176 quao-0.2.0/src/quao/data/request/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/data/request/__init__.py
+-rw-rw-rw-   0        0        0      566 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/data/request/request_data.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.984176 quao-0.2.0/src/quao/enum/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/__init__.py
+-rw-rw-rw-   0        0        0      212 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/http_status.py
+-rw-rw-rw-   0        0        0      213 2023-06-01 11:44:52.000000 quao-0.2.0/src/quao/enum/job_status.py
+-rw-rw-rw-   0        0        0      258 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/enum/media_type.py
+-rw-rw-rw-   0        0        0      297 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/enum/provider_type.py
+-rw-rw-rw-   0        0        0      179 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/enum/sdk.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.992206 quao-0.2.0/src/quao/factory/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/factory/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-06-01 11:39:48.000000 quao-0.2.0/src/quao/factory/device_factory.py
+-rw-rw-rw-   0        0        0     1351 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/factory/provider_factory.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.994174 quao-0.2.0/src/quao/model/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.010205 quao-0.2.0/src/quao/model/device/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/device/__init__.py
+-rw-rw-rw-   0        0        0     1538 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/device/aws_braket_device.py
+-rw-rw-rw-   0        0        0     3062 2023-06-02 11:14:34.000000 quao-0.2.0/src/quao/model/device/device.py
+-rw-rw-rw-   0        0        0     1012 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/device/ibm_cloud_device.py
+-rw-rw-rw-   0        0        0      794 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/device/ibm_quantum_device.py
+-rw-rw-rw-   0        0        0      776 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/device/qiskit_device.py
+-rw-rw-rw-   0        0        0     2511 2023-06-02 09:52:05.000000 quao-0.2.0/src/quao/model/device/quao_device.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.013177 quao-0.2.0/src/quao/model/job/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/job/__init__.py
+-rw-rw-rw-   0        0        0     2693 2023-06-02 10:03:39.000000 quao-0.2.0/src/quao/model/job/qiskit_status.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.026215 quao-0.2.0/src/quao/model/provider/
+-rw-rw-rw-   0        0        0        0 2023-06-01 02:42:52.000000 quao-0.2.0/src/quao/model/provider/__init__.py
+-rw-rw-rw-   0        0        0     1255 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/aws_braket_provider.py
+-rw-rw-rw-   0        0        0     1008 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/ibm_cloud_provider.py
+-rw-rw-rw-   0        0        0      876 2023-06-02 09:50:48.000000 quao-0.2.0/src/quao/model/provider/ibm_quantum_provider.py
+-rw-rw-rw-   0        0        0      589 2023-06-01 03:12:31.000000 quao-0.2.0/src/quao/model/provider/provider.py
+-rw-rw-rw-   0        0        0     1372 2023-06-02 09:50:49.000000 quao-0.2.0/src/quao/model/provider/quao_provider.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:27.032173 quao-0.2.0/src/quao/util/
+-rw-rw-rw-   0        0        0        0 2023-05-31 12:46:23.000000 quao-0.2.0/src/quao/util/__init__.py
+-rw-rw-rw-   0        0        0     2047 2023-06-02 09:11:35.000000 quao-0.2.0/src/quao/util/json_parser_util.py
+-rw-rw-rw-   0        0        0     1288 2023-06-01 08:49:23.000000 quao-0.2.0/src/quao/util/response_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-02 11:42:26.960179 quao-0.2.0/src/quao.egg-info/
+-rw-rw-rw-   0        0        0     2839 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1447 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-02 11:42:26.000000 quao-0.2.0/src/quao.egg-info/top_level.txt
```

### Comparing `quao-0.1.9/LICENSE` & `quao-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quao-0.1.9/PKG-INFO` & `quao-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `quao-0.1.9/README.md` & `quao-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quao-0.1.9/pyproject.toml` & `quao-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quao"
-version = "0.1.9"
+version = "0.2.0"
 description = "Quao Library supporting Quao Platform for Quantum Computing"
 readme = "README.md"
 authors = [{ name = "CITYNOW Co. Ltd. ", email = "corp@citynow.vn" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["quao", "quantum"]
 dependencies = [
-    "qiskit==0.43.0",
-    "qiskit_ibm_runtime==0.10.0",
-    "qiskit-ibm-provider==0.6.0",
-    "numpy>=1.22.3",
+    "qiskit==0.42.1",
+    "qbraid==0.4.0",
+    "amazon-braket-sdk==1.38.1",
+    "qiskit-ibm-runtime",
+    "qiskit-ibm-provider",
+    "matplotlib",
+    "pylatexenc",
+    "numpy"
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
```

### Comparing `quao-0.1.9/src/quao/dataUtils.py` & `quao-0.2.0/src/quao/data/request/request_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
-    QuaO Project dataUtils.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+    QuaO Project request_data.py Copyright © CITYNOW Co. Ltd. All rights reserved.
 """
 
 
 class RequestData:
 
     def __init__(self, event):
         json_data = event.json()
         self.data = json_data
         self.input = json_data.get("input")
         self.shots = json_data.get("shots")
         self.device_id = json_data.get("deviceId")
-        self.sdk = json_data.get("sdk").lower()
+        self.sdk = json_data.get("sdk").lower() if json_data.get("sdk") else None
         self.server_url = json_data.get("serverUrl")
         self.circuit_export_url = json_data.get("circuitExportUrl")
```

### Comparing `quao-0.1.9/src/quao/status/qiskit_status.py` & `quao-0.2.0/src/quao/model/job/qiskit_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+"""
+    QuaO Project job_status.py Copyright © CITYNOW Co. Ltd. All rights reserved.
+"""
 from qiskit import QiskitError
 from qiskit_ibm_runtime import QiskitRuntimeService
 from qiskit.providers.jobstatus import JobStatus
 from json import dumps
 
-from ..utilities import JobResponse
-
-APPLICATION_JSON = 'application/json'
+from ...data.job.job_response import JobResponse
+from ...enum.media_type import MediaType
+from ...util.json_parser_util import JsonParserUtils
 
 
 class Job:
     def __init__(self, channel, token, crn, provider_job_id):
         self.channel = channel if channel else "ibm_quantum"
         self.token = token if token else ""
         self.crn = crn if crn else None
@@ -25,33 +28,36 @@
         job_status = status.name
 
         if status == JobStatus.DONE:
             try:
                 result = self.retrieve_job.result()
                 # case function `sampler`
                 if self.retrieve_job.program_id == 'sampler':
-                    job_result = result.__dict__
+                    job_result = JsonParserUtils.parse(result.__dict__)
                 # case function `circuit-runner`
+
                 else:
-                    job_result = result.to_dict()
+                    job_result = JsonParserUtils.parse(result.to_dict())
                     # handle case Statevector object not serializable when run with backend `statevector_simulator`
                     if self.retrieve_job.backend().backend_name == 'statevector_simulator':
                         job_result = dumps(job_result, default=str)
-                content_type = APPLICATION_JSON
+                content_type = MediaType.APPLICATION_JSON.value
+
                 # handle circuit has measure
                 try:
                     job_histogram = result.get_counts()
                 except QiskitError:
                     job_histogram = None
+
             except Exception as exception:
                 job_result = {
                     "error": "Exception when get job result",
                     "exception": str(exception)
                 }
-                job_status = "ERROR"
+                job_status = JobStatus.ERROR.value
 
         return JobResponse(
             provider_job_id=self.job_id,
             job_status=job_status,
             job_result=job_result,
             content_type=content_type,
             job_histogram=job_histogram
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `quao-0.1.9/src/quao.egg-info/PKG-INFO` & `quao-0.2.0/src/quao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quao
-Version: 0.1.9
+Version: 0.2.0
 Summary: Quao Library supporting Quao Platform for Quantum Computing
 Author-email: "CITYNOW Co. Ltd. " <corp@citynow.vn>
 License: The MIT License (MIT)
         Copyright © CITYNOW Co. Ltd. All rights reserved.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

