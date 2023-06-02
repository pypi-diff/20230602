# Comparing `tmp/bluequbit-0.1.2b1.tar.gz` & `tmp/bluequbit-0.2.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluequbit-0.1.2b1.tar", last modified: Wed May 24 05:45:11 2023, max compression
+gzip compressed data, was "bluequbit-0.2.1b1.tar", last modified: Fri Jun  2 09:49:10 2023, max compression
```

## Comparing `bluequbit-0.1.2b1.tar` & `bluequbit-0.2.1b1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.246816 bluequbit-0.1.2b1/bluequbit/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.250816 bluequbit-0.1.2b1/bluequbit/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/backend_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/bluequbit_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/check_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/estimate_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/http_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/job_metadata_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/job_result.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/bluequbit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.246816 bluequbit-0.1.2b1/bluequbit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 05:45:11.000000 bluequbit-0.1.2b1/bluequbit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 05:45:11.254816 bluequbit-0.1.2b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_basic_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_basic_large_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_batch_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_cancel_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_count_wrong.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_get_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_gpu_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_job_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_ok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_quantum_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_stress_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-24 05:44:52.000000 bluequbit-0.1.2b1/tests/test_very_large_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:49:10.220325 bluequbit-0.2.1b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 09:49:10.220325 bluequbit-0.2.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:49:10.216325 bluequbit-0.2.1b1/bluequbit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:49:10.220325 bluequbit-0.2.1b1/bluequbit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/backend_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/bluequbit_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/check_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/estimate_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/job_metadata_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6435 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/job_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/bluequbit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:49:10.216325 bluequbit-0.2.1b1/bluequbit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-02 09:49:10.000000 bluequbit-0.2.1b1/bluequbit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-02 09:49:10.000000 bluequbit-0.2.1b1/bluequbit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:49:10.000000 bluequbit-0.2.1b1/bluequbit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:49:10.000000 bluequbit-0.2.1b1/bluequbit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:49:10.000000 bluequbit-0.2.1b1/bluequbit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:49:10.220325 bluequbit-0.2.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:49:10.220325 bluequbit-0.2.1b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_basic_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_basic_large_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_batch_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_cancel_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_complex_circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_count_wrong.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_get_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_gpu_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_job_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_ok.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_quantum_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_stress_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-02 09:48:57.000000 bluequbit-0.2.1b1/tests/test_very_large_job.py
```

### Comparing `bluequbit-0.1.2b1/LICENSE` & `bluequbit-0.2.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/PKG-INFO` & `bluequbit-0.2.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.1.2b1
+Version: 0.2.1b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bluequbit-0.1.2b1/README.md` & `bluequbit-0.2.1b1/README.md`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/__init__.py` & `bluequbit-0.2.1b1/bluequbit/__init__.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/api/jobs.py` & `bluequbit-0.2.1b1/bluequbit/api/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import json
 import logging
 import zlib
 
 import dateutil.parser
 
-from ..circuit_serialization import encode_circuit
+from ..circuit_serialization import encode_circuit_with_fallback
 from ..exceptions import BQAPIError, BQError
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 _SINGLE_REQUEST_LIMIT = 100
 
 
@@ -73,17 +73,19 @@
     device,
     job_name=None,
     estimate_only=False,
     shots=None,
     asynchronous=False,
 ):
     if isinstance(circuits, list):
-        encoded_circuits = [encode_circuit(circuit) for circuit in circuits]
+        encoded_circuits = [
+            encode_circuit_with_fallback(circuit) for circuit in circuits
+        ]
     else:
-        encoded_circuits = encode_circuit(circuits)
+        encoded_circuits = encode_circuit_with_fallback(circuits)
 
     params = {
         "estimate_only": estimate_only,
         "circuit": encoded_circuits,
         "job_name": job_name,
         "device": device,
         "shots": shots,
```

### Comparing `bluequbit-0.1.2b1/bluequbit/backend_connection.py` & `bluequbit-0.2.1b1/bluequbit/backend_connection.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/bluequbit_client.py` & `bluequbit-0.2.1b1/bluequbit/bluequbit_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 # TODO this requires imports of actual quantum libraries for proper type
 # checking.
 CircuitT = Any
 
 logger = logging.getLogger("bluequbit-python-sdk")
 
 
+_SHOTS_LIMIT_NON_QPU = 131072
+
+
 class BQClient:
     """Client for managing jobs on BlueQubit platform.
 
     :param api_token: API token of the user. If ``None``, the token will be looked
                       in default configuration file ``$HOME/.config/bluequbit/config.json``.
                       If not ``None``, the token will also be saved in the same
                       default configuration file.
@@ -72,15 +75,15 @@
     ) -> EstimateResult | list[EstimateResult]:
         """Estimate job runtime
 
         :param circuits: quantum circuit or circuits
         :type circuits: Cirq, Qiskit, list
         :param device: device for which to estimate the circuit. Can be one of
                        ``"cpu"`` | ``"gpu"`` | ``"quantum"``
-        :return: estimate result or results metadata
+        :return: result or results estimate metadata
         """
         device = self.validate_device(device)
         self.validate_batch(circuits)
         response = jobs.submit_jobs(
             self._backend_connection, circuits, device, estimate_only=True
         )
         if isinstance(circuits, list):
@@ -90,30 +93,40 @@
 
     def run(
         self,
         circuits: CircuitT | list[CircuitT],
         device: str = "cpu",
         asynchronous: bool = False,
         job_name: str | None = None,
-        shots: int = 1000,
+        shots: int | None = None,
     ) -> JobResult | list[JobResult]:
         """Submit a job to run on BlueQubit platform
 
         :param circuits: quantum circuit or list of circuits
         :type circuits: Cirq, Qiskit, list
         :param device: device on which to run the circuit. Can be one of
                        ``"cpu"`` | ``"gpu"`` | ``"quantum"``
         :param asynchronous: if set to ``False``, wait for job completion before
                              returning. If set to ``True``, return immediately
         :param job_name: customizable job name
-        :param shots: number of shots to run if device is quantum.
-        :return: job metadata
+        :param shots: number of shots to run. If device is quantum and shots is None then
+                      it is set to 1000. For non quantum devices, if None, full
+                      probability distribution will be returned. For non quantum
+                      devices it is limited to 131072
+        :return: job or jobs metadata
         """
         device = self.validate_device(device)
         self.validate_batch(circuits)
+        if device == "quantum" and shots is None:
+            shots = 1000
+        elif device != "quantum" and shots is not None and shots > _SHOTS_LIMIT_NON_QPU:
+            logger.warning(
+                "Number of shots is set to %s, because of limit.",
+                _SHOTS_LIMIT_NON_QPU,
+            )
         response = jobs.submit_jobs(
             self._backend_connection,
             circuits,
             device,
             job_name,
             shots=shots,
             asynchronous=asynchronous,
```

### Comparing `bluequbit-0.1.2b1/bluequbit/check_version.py` & `bluequbit-0.2.1b1/bluequbit/check_version.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/circuit_serialization.py` & `bluequbit-0.2.1b1/bluequbit/circuit_serialization.py`

 * *Files 22% similar despite different names*

```diff
@@ -58,14 +58,22 @@
             # Convert bytes to str
             serialized = serialized.decode("utf-8")
         return {"circuit_type": "Qiskit", "circuit": serialized}
     else:
         raise Exception("Unsupported circuit type", qc)
 
 
+def encode_circuit_with_fallback(qc):
+    # Temporary workaround: see https://trello.com/c/0SMvJuLV/266-productofsums-issue
+    encoded = encode_circuit(qc)
+    if encoded["circuit_type"] == "Cirq" and "ProductOfSums" in encoded["circuit"]:
+        return encode_circuit(qc, use_cirq_qasm=True)
+    return encoded
+
+
 def decode_circuit(data):
     """
     Decode the output of encode_circuit.
     """
     if "circuit_type" not in data:
         raise Exception("Wrong data structure. 'circuit_type' must be present.")
     if "circuit" not in data:
```

### Comparing `bluequbit-0.1.2b1/bluequbit/estimate_result.py` & `bluequbit-0.2.1b1/bluequbit/estimate_result.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/exceptions.py` & `bluequbit-0.2.1b1/bluequbit/exceptions.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/http_utils.py` & `bluequbit-0.2.1b1/bluequbit/http_utils.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/bluequbit/job_result.py` & `bluequbit-0.2.1b1/bluequbit/job_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         if self.estimated_cost is not None:
             self.estimated_cost /= 100.0
 
         #: datetime: job creation date in UTC timezone
         self.created_on = parse(data.get("created_on"))
 
         self._results_path = data.get("results_path")
-        self.top_100_results = data.get("top_100_results")
+
+        #: dict: top 128 results
+        self.top_128_results = data.get("top_128")
 
         #: int: number of qubits
         self.num_qubits = data.get("num_qubits")
         self.tags = data.get("tags")
 
         self.run_start = data.get("run_start")
         if self.run_start is not None:
@@ -110,19 +112,23 @@
         if self._statevector is None:
             response = request_retriable("GET", self._results_path + "statevector.txt")
             self._statevector = np.loadtxt(BytesIO(response.content), dtype=np.complex_)
         return self._statevector
 
     def get_counts(self) -> Optional[Dict[str, float]]:
         """
-        "counts" is the measurement probabilities of the computation result,
-        without any statistical fluctuation. It is equivalent to what you would
-        get from a Qiskit result if you do `get_counts` on it from a Qiskit
-        simulation with 0 shot.
+        For non quantum device, "counts" is the measurement probabilities of the
+        computation result, without any statistical fluctuation. It is equivalent to
+        what you would get from a Qiskit result if you do `get_counts` on it from a
+        Qiskit simulation with 0 shot.
+        For quantum device, this returns a number of samples from the measurement
+        provided by the shots argument in bq.run().
         """
+        if self.top_128_results is not None and len(self.top_128_results) < 128:
+            return self.top_128_results
         if self._metadata is None:
             response = request_retriable("GET", self._results_path + "metadata.json")
             self._metadata = response.json()
         if "counts" not in self._metadata:
             raise BQJobDoesNotContainCountsError(self.job_id)
         return self._metadata["counts"]
```

### Comparing `bluequbit-0.1.2b1/bluequbit.egg-info/PKG-INFO` & `bluequbit-0.2.1b1/bluequbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluequbit
-Version: 0.1.2b1
+Version: 0.2.1b1
 Summary: Python SDK to BlueQubit app
 Author: BlueQubit
 Author-email: hovnatan@bluequbit.io
 License: Apache 2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bluequbit-0.1.2b1/bluequbit.egg-info/SOURCES.txt` & `bluequbit-0.2.1b1/bluequbit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 bluequbit/api/__init__.py
 bluequbit/api/jobs.py
 tests/test_basic_jobs.py
 tests/test_basic_large_jobs.py
 tests/test_batch_jobs.py
 tests/test_cancel_job.py
 tests/test_circuit_serialization.py
+tests/test_complex_circuits.py
 tests/test_count_wrong.py
 tests/test_get_job.py
 tests/test_gpu_job.py
 tests/test_job_estimate.py
-tests/test_metadata.py
 tests/test_ok.py
 tests/test_quantum_job.py
 tests/test_stress_jobs.py
 tests/test_very_large_job.py
```

### Comparing `bluequbit-0.1.2b1/pyproject.toml` & `bluequbit-0.2.1b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/setup.py` & `bluequbit-0.2.1b1/setup.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_basic_jobs.py` & `bluequbit-0.2.1b1/tests/test_basic_jobs.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_basic_large_jobs.py` & `bluequbit-0.2.1b1/tests/test_basic_large_jobs.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_batch_jobs.py` & `bluequbit-0.2.1b1/tests/test_batch_jobs.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_cancel_job.py` & `bluequbit-0.2.1b1/tests/test_cancel_job.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_circuit_serialization.py` & `bluequbit-0.2.1b1/tests/test_circuit_serialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 
 
 def test_cirq_oq2():
     qs = cirq.LineQubit.range(2)
     circuit = cirq.Circuit([cirq.ry(0.5).on(qs[1]).controlled_by(qs[0])])
 
     # If we encode normally, we should see "ProductOfSums" in the output.
-    encoded_cirq = circuit_serialization.encode_circuit(circuit)
-    assert "ProductOfSums" in encoded_cirq["circuit"]
+    # TODO Disabled for now because we are using the old version of Cirq (0.x)
+    # which doesn't have ProductOfSums.
+    # encoded_cirq = circuit_serialization.encode_circuit(circuit)
+    # assert "ProductOfSums" in encoded_cirq["circuit"]
 
     # If we use OQ2, there should be none, because it's not in OpenQASM spec.
     encoded_cirq = circuit_serialization.encode_circuit(circuit, use_cirq_qasm=True)
     assert "ProductOfSums" not in encoded_cirq["circuit"]
 
-    decoded_cirq = circuit_serialization.decode_circuit(encoded_cirq)
-    all_ops = list(decoded_cirq.all_operations())
-    # The cirq.ry is expanded into 5 operations
-    assert len(all_ops) == 5
-    assert isinstance(all_ops[0].gate, cirq.circuits.qasm_output.QasmUGate), all_ops[
-        0
-    ].gate
+    # Disabled for now, because Cirq 0.x and 1.x have different output for this.
+    # The cirq.ry is expanded into 6 operations
+    # decoded_cirq = circuit_serialization.decode_circuit(encoded_cirq)
+    # all_ops = list(decoded_cirq.all_operations())
+    # assert len(all_ops) == 6
+    # assert isinstance(all_ops[0].gate, cirq.ZPowGate), all_ops[0].gate
 
 
 def test_qiskit():
     qc_qiskit = qiskit.QuantumCircuit(2)
     qc_qiskit.h(0)
     qc_qiskit.x(1)
```

### Comparing `bluequbit-0.1.2b1/tests/test_count_wrong.py` & `bluequbit-0.2.1b1/tests/test_count_wrong.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_get_job.py` & `bluequbit-0.2.1b1/tests/test_get_job.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,7 +17,19 @@
     assert result._results_path is not None
 
     response = requests.get(result._results_path + "statevector.txt", timeout=60.0)
     assert len(response.content) == 326
 
     assert result.get_statevector().shape == (4,)
     assert len(result.get_counts()) == 2
+
+
+def test_get_job_counts():
+    dq_client = bluequbit.init()
+    qc_qiskit = qiskit.QuantumCircuit(2)
+    qc_qiskit.h(0)
+    qc_qiskit.x(1)
+    qc_qiskit.measure_all()
+    result = dq_client.run(qc_qiskit, shots=6)
+
+    assert result.num_qubits == 2
+    assert sum(result.get_counts().values()) == 6
```

### Comparing `bluequbit-0.1.2b1/tests/test_gpu_job.py` & `bluequbit-0.2.1b1/tests/test_gpu_job.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_job_estimate.py` & `bluequbit-0.2.1b1/tests/test_job_estimate.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_quantum_job.py` & `bluequbit-0.2.1b1/tests/test_quantum_job.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_stress_jobs.py` & `bluequbit-0.2.1b1/tests/test_stress_jobs.py`

 * *Files identical despite different names*

### Comparing `bluequbit-0.1.2b1/tests/test_very_large_job.py` & `bluequbit-0.2.1b1/tests/test_very_large_job.py`

 * *Files identical despite different names*

