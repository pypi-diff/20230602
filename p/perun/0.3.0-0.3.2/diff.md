# Comparing `tmp/perun-0.3.0.tar.gz` & `tmp/perun-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun-0.3.0.tar", max compression
+gzip compressed data, was "perun-0.3.2.tar", max compression
```

## Comparing `perun-0.3.0.tar` & `perun-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1527 2023-05-31 09:51:29.914219 perun-0.3.0/LICENSE
--rw-r--r--   0        0        0     8486 2023-05-31 09:51:29.914219 perun-0.3.0/README.md
--rw-r--r--   0        0        0      319 2023-05-31 09:51:30.662215 perun-0.3.0/perun/__init__.py
--rw-r--r--   0        0        0       88 2023-05-31 09:51:29.918220 perun-0.3.0/perun/__main__.py
--rw-r--r--   0        0        0      190 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/__init__.py
--rw-r--r--   0        0        0     1963 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/backend.py
--rw-r--r--   0        0        0     7426 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/intel_rapl.py
--rw-r--r--   0        0        0     3401 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/nvml.py
--rw-r--r--   0        0        0     4435 2023-05-31 09:51:29.918220 perun-0.3.0/perun/backend/psutil.py
--rw-r--r--   0        0        0     7550 2023-05-31 09:51:29.918220 perun-0.3.0/perun/cli.py
--rw-r--r--   0        0        0     1992 2023-05-31 09:51:29.918220 perun-0.3.0/perun/comm.py
--rw-r--r--   0        0        0     3044 2023-05-31 09:51:29.918220 perun-0.3.0/perun/configuration.py
--rw-r--r--   0        0        0     3793 2023-05-31 09:51:29.918220 perun-0.3.0/perun/coordination.py
--rw-r--r--   0        0        0       26 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/__init__.py
--rw-r--r--   0        0        0     7136 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/data.py
--rw-r--r--   0        0        0     1900 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/measurement_type.py
--rw-r--r--   0        0        0      988 2023-05-31 09:51:29.918220 perun-0.3.0/perun/data_model/sensor.py
--rw-r--r--   0        0        0      878 2023-05-31 09:51:29.918220 perun-0.3.0/perun/decorator.py
--rw-r--r--   0        0        0       21 2023-05-31 09:51:29.918220 perun-0.3.0/perun/extras/__init__.py
--rw-r--r--   0        0        0     1863 2023-05-31 09:51:29.918220 perun-0.3.0/perun/extras/horeka.py
--rw-r--r--   0        0        0       18 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/__init__.py
--rw-r--r--   0        0        0     1544 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/bench.py
--rw-r--r--   0        0        0     6458 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/hdf5.py
--rw-r--r--   0        0        0     4384 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/io.py
--rw-r--r--   0        0        0     1414 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/json.py
--rw-r--r--   0        0        0     2612 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/pandas.py
--rw-r--r--   0        0        0      536 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/pickle.py
--rw-r--r--   0        0        0     3983 2023-05-31 09:51:29.918220 perun-0.3.0/perun/io/text_report.py
--rw-r--r--   0        0        0      828 2023-05-31 09:51:29.918220 perun-0.3.0/perun/logging.py
--rw-r--r--   0        0        0    12299 2023-05-31 09:51:29.918220 perun-0.3.0/perun/perun.py
--rw-r--r--   0        0        0     7107 2023-05-31 09:51:29.918220 perun-0.3.0/perun/processing.py
--rw-r--r--   0        0        0     4189 2023-05-31 09:51:29.918220 perun-0.3.0/perun/util.py
--rw-r--r--   0        0        0     1873 2023-05-31 09:51:30.662215 perun-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9410 1970-01-01 00:00:00.000000 perun-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1527 2023-06-02 08:25:25.606819 perun-0.3.2/LICENSE
+-rw-r--r--   0        0        0     8581 2023-06-02 08:25:25.606819 perun-0.3.2/README.md
+-rw-r--r--   0        0        0      319 2023-06-02 08:25:26.370831 perun-0.3.2/perun/__init__.py
+-rw-r--r--   0        0        0       88 2023-06-02 08:25:25.606819 perun-0.3.2/perun/__main__.py
+-rw-r--r--   0        0        0      190 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/__init__.py
+-rw-r--r--   0        0        0     1963 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/backend.py
+-rw-r--r--   0        0        0     7673 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/intel_rapl.py
+-rw-r--r--   0        0        0     3404 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/nvml.py
+-rw-r--r--   0        0        0     4435 2023-06-02 08:25:25.606819 perun-0.3.2/perun/backend/psutil.py
+-rw-r--r--   0        0        0     7550 2023-06-02 08:25:25.606819 perun-0.3.2/perun/cli.py
+-rw-r--r--   0        0        0     1992 2023-06-02 08:25:25.606819 perun-0.3.2/perun/comm.py
+-rw-r--r--   0        0        0     3044 2023-06-02 08:25:25.606819 perun-0.3.2/perun/configuration.py
+-rw-r--r--   0        0        0     3793 2023-06-02 08:25:25.606819 perun-0.3.2/perun/coordination.py
+-rw-r--r--   0        0        0       26 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/__init__.py
+-rw-r--r--   0        0        0     7136 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/data.py
+-rw-r--r--   0        0        0     1900 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/measurement_type.py
+-rw-r--r--   0        0        0      988 2023-06-02 08:25:25.606819 perun-0.3.2/perun/data_model/sensor.py
+-rw-r--r--   0        0        0      878 2023-06-02 08:25:25.606819 perun-0.3.2/perun/decorator.py
+-rw-r--r--   0        0        0       21 2023-06-02 08:25:25.606819 perun-0.3.2/perun/extras/__init__.py
+-rw-r--r--   0        0        0     1863 2023-06-02 08:25:25.606819 perun-0.3.2/perun/extras/horeka.py
+-rw-r--r--   0        0        0       18 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/__init__.py
+-rw-r--r--   0        0        0     1544 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/bench.py
+-rw-r--r--   0        0        0     6458 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/hdf5.py
+-rw-r--r--   0        0        0     4384 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/io.py
+-rw-r--r--   0        0        0     1414 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/json.py
+-rw-r--r--   0        0        0     2612 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/pandas.py
+-rw-r--r--   0        0        0      536 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/pickle.py
+-rw-r--r--   0        0        0     3983 2023-06-02 08:25:25.606819 perun-0.3.2/perun/io/text_report.py
+-rw-r--r--   0        0        0      828 2023-06-02 08:25:25.606819 perun-0.3.2/perun/logging.py
+-rw-r--r--   0        0        0    12011 2023-06-02 08:25:25.606819 perun-0.3.2/perun/perun.py
+-rw-r--r--   0        0        0     7253 2023-06-02 08:25:25.606819 perun-0.3.2/perun/processing.py
+-rw-r--r--   0        0        0     4189 2023-06-02 08:25:25.610819 perun-0.3.2/perun/util.py
+-rw-r--r--   0        0        0     1873 2023-06-02 08:25:26.374831 perun-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     9505 1970-01-01 00:00:00.000000 perun-0.3.2/PKG-INFO
```

### Comparing `perun-0.3.0/LICENSE` & `perun-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/README.md` & `perun-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 <div align="center">
   <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
 &nbsp;
 &nbsp;
 
-[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-orange)](https://fair-software.eu)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
+[![DOI](https://zenodo.org/badge/523363424.svg)](https://zenodo.org/badge/latestdoi/523363424)
 ![PyPI](https://img.shields.io/pypi/v/perun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `perun-0.3.0/perun/backend/backend.py` & `perun-0.3.2/perun/backend/backend.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/backend/intel_rapl.py` & `perun-0.3.2/perun/backend/intel_rapl.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,14 +93,15 @@
                             np.uint64(0),
                             max_energy,
                             max_energy,
                         )
 
                         energy_path = str(child / "energy_uj")
                         energy_file = open(energy_path, "r")
+                        log.debug(f"RAPL FILE OPENED: {energy_path}")
                         self._files.append(energy_file)
                         device = Sensor(
                             f"{devType.value}_{socket}_{device_name}",
                             devType,
                             self.metadata,
                             dataType,
                             getCallback(energy_file),
@@ -140,14 +141,15 @@
                                         np.uint64(0),
                                         max_energy,
                                         max_energy,
                                     )
 
                                     energy_path = str(grandchild / "energy_uj")
                                     energy_file = open(energy_path, "r")
+                                    log.debug(f"RAPL FILE OPENED: {energy_path}")
                                     self._files.append(energy_file)
                                     device = Sensor(
                                         f"{devType.value}_{socket}_{device_name}",
                                         devType,
                                         self.metadata,
                                         dataType,
                                         getCallback(energy_file),
@@ -156,23 +158,25 @@
                                     self.devices[device.id] = device
 
                                     if "package" in device_name:
                                         packageDevices.append(device)
 
         if foundPsys:
             for pkg, file in zip(packageDevices, packageFiles):
+                log.info(f"Closing file: {file}")
                 file.close()
                 del self.devices[pkg.id]
 
         log.debug(f"IntelRapl devices {self.devices}")
 
     def close(self) -> None:
         """Backend shutdown code (does nothing for intel rapl)."""
-        log.debug("Closing files")
+        log.info("Closing files")
         for file in self._files:
+            log.info(f"Closing file: {file}")
             file.close()
         return
 
     def visibleSensors(self) -> Set[str]:
         """
         Return string ids of visible devices.
```

### Comparing `perun-0.3.0/perun/backend/nvml.py` & `perun-0.3.2/perun/backend/nvml.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         deviceCount = pynvml.nvmlDeviceGetCount()
         self.metadata = {
             "cuda_version": pynvml.nvmlSystemGetCudaDriverVersion(),
             "driver_version": pynvml.nvmlSystemGetDriverVersion(),
             "source": "Nvidia Managment Library",
         }
 
-        log.debug(f"NVML Device count: {deviceCount}")
+        log.info(f"NVML Device count: {deviceCount}")
 
     def close(self):
         """Backend shutdown code."""
         pynvml.nvmlShutdown()
 
     def visibleSensors(self) -> Set[str]:
         """
@@ -102,14 +102,14 @@
                         device_type,
                         device_metadata,
                         data_type,
                         getCallback(handle),
                     )
                 )
             except NVMLError as e:
-                log.debug(f"Could not find device {deviceId}")
-                log.debug(e)
+                log.warning(f"Could not find device {deviceId}")
+                log.warning(e)
 
         return devices
 
 
 NVMLBackend()
```

### Comparing `perun-0.3.0/perun/backend/psutil.py` & `perun-0.3.2/perun/backend/psutil.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/cli.py` & `perun-0.3.2/perun/cli.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/comm.py` & `perun-0.3.2/perun/comm.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/configuration.py` & `perun-0.3.2/perun/configuration.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/coordination.py` & `perun-0.3.2/perun/coordination.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/data_model/data.py` & `perun-0.3.2/perun/data_model/data.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/data_model/measurement_type.py` & `perun-0.3.2/perun/data_model/measurement_type.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/data_model/sensor.py` & `perun-0.3.2/perun/data_model/sensor.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/decorator.py` & `perun-0.3.2/perun/decorator.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/extras/horeka.py` & `perun-0.3.2/perun/extras/horeka.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/bench.py` & `perun-0.3.2/perun/io/bench.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/hdf5.py` & `perun-0.3.2/perun/io/hdf5.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/io.py` & `perun-0.3.2/perun/io/io.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/json.py` & `perun-0.3.2/perun/io/json.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/pandas.py` & `perun-0.3.2/perun/io/pandas.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/pickle.py` & `perun-0.3.2/perun/io/pickle.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/io/text_report.py` & `perun-0.3.2/perun/io/text_report.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/logging.py` & `perun-0.3.2/perun/logging.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/perun/perun.py` & `perun-0.3.2/perun/perun.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,25 +57,25 @@
             backends, app, app_args, app_kwargs, record=True
         )
         if dataNode:
             # Only on first rank, export data
             exportTo(data_out, dataNode, format, includeRawData, depth)
     else:
         # Start with warmup rounds
-        log.debug(f"Rank {COMM_WORLD.Get_rank()} : Started warmup rounds")
+        log.info(f"Rank {COMM_WORLD.Get_rank()} : Started warmup rounds")
         for i in range(config.getint("benchmarking", "bench_warmup_rounds")):
-            log.debug(f"Warmup run: {i}")
+            log.info(f"Warmup run: {i}")
             app_results, _ = _run_application(
                 backends, app, app_args, app_kwargs, record=False
             )
 
-        log.debug(f"Rank {COMM_WORLD.Get_rank()} : Started bench rounds")
+        log.info(f"Rank {COMM_WORLD.Get_rank()} : Started bench rounds")
         runNodes: List[DataNode] = []
         for i in range(config.getint("benchmarking", "bench_rounds")):
-            log.debug(f"Rank {COMM_WORLD.Get_rank()} : Bench run: {i}")
+            log.info(f"Rank {COMM_WORLD.Get_rank()} : Bench run: {i}")
             app_results, runNode = _run_application(
                 backends, app, app_args, app_kwargs, record=True, run_id=str(i)
             )
             if runNode:
                 runNodes.append(runNode)
 
         if len(runNodes) > 0:
@@ -89,31 +89,28 @@
                 },
                 nodes={node.id: node for node in runNodes},
             )
             benchNode = processDataNode(benchNode)
 
             exportTo(data_out, benchNode, format, includeRawData, depth)
 
-    for backend in backends:
-        backend.close()
-
     return app_results
 
 
 def _run_application(
     backends: List,
     app: Union[Path, Callable],
     app_args: tuple = tuple(),
     app_kwargs: dict = dict(),
     record: bool = True,
     run_id: Optional[str] = None,
 ) -> Tuple[Optional[Any], Optional[DataNode]]:
     app_result: Optional[Any] = None
 
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: _run_application")
+    log.info(f"Rank {COMM_WORLD.Get_rank()}: _run_application")
     if record:
         # 1) Get sensor configuration
         mpiRanks, localBackends = getLocalSensorRankConfiguration(COMM_WORLD, backends)
 
         start_event = Event()
         stop_event = Event()
 
@@ -137,63 +134,64 @@
                 ],
             )
             perunSP.start()
         else:
             start_event.set()
 
         # 3) Start application
-        log.debug(f"Rank {COMM_WORLD.Get_rank()}: Started Timer")
-        run_starttime = datetime.utcnow()
 
         if isinstance(app, Path):
             try:
                 with open(str(app), "r") as scriptFile:
                     start_event.wait()
                     COMM_WORLD.barrier()
-                    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Started App")
+                    log.info(f"Rank {COMM_WORLD.Get_rank()}: Started App")
+                    run_starttime = datetime.utcnow()
                     exec(
                         scriptFile.read(),
                         {"__name__": "__main__", "__file__": app.name},
                     )
-                    log.debug(f"Rank {COMM_WORLD.Get_rank()}: AppStoppedStopped")
+                    log.info(f"Rank {COMM_WORLD.Get_rank()}: App Stopped")
                     stop_event.set()
             except Exception as e:
                 log.error(
                     f"Rank {COMM_WORLD.Get_rank()}:  Found error on monitored script: {str(app)}"
                 )
                 stop_event.set()
                 raise e
 
         elif isinstance(app, types.FunctionType):
             try:
                 start_event.wait()
                 COMM_WORLD.barrier()
-                log.debug(f"Rank {COMM_WORLD.Get_rank()}: Started App")
+                log.info(f"Rank {COMM_WORLD.Get_rank()}: Started App")
+                run_starttime = datetime.utcnow()
+
                 app_result = app(*app_args, **app_kwargs)
-                log.debug(f"Rank {COMM_WORLD.Get_rank()}: Stopped App")
+                log.info(f"Rank {COMM_WORLD.Get_rank()}: Stopped App")
             except Exception as e:
                 stop_event.set()
                 raise e
             stop_event.set()
 
         # 4) App finished, stop subrocess and get data
         if queue and perunSP:
-            log.debug(f"Rank {COMM_WORLD.Get_rank()}: Getting queue contents")
+            log.info(f"Rank {COMM_WORLD.Get_rank()}: Getting queue contents")
             nodeData = queue.get(block=True)
-            log.debug(f"Rank {COMM_WORLD.Get_rank()}: Got queue contents")
-            log.debug(f"Rank {COMM_WORLD.Get_rank()}: Waiting for subprocess to close")
+            log.info(f"Rank {COMM_WORLD.Get_rank()}: Got queue contents")
+            log.info(f"Rank {COMM_WORLD.Get_rank()}: Waiting for subprocess to close")
             perunSP.join()
             perunSP.close()
-            log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess closed")
+            log.info(f"Rank {COMM_WORLD.Get_rank()}: Subprocess closed")
             queue.close()
         else:
             nodeData = None
 
         COMM_WORLD.barrier()
-        log.debug(f"Rank {COMM_WORLD.Get_rank()}: Everyone exited the subprocess")
+        log.info(f"Rank {COMM_WORLD.Get_rank()}: Everyone exited the subprocess")
 
         if nodeData:
             nodeData.metadata["mpi_ranks"] = mpiRanks
 
         # 5) Collect data from everyone on the first rank
         dataNodes: Optional[List[DataNode]] = COMM_WORLD.gather(nodeData, root=0)
         if dataNodes:
@@ -255,15 +253,14 @@
         deviceIds (Set[str]): List of device ids to sample from
         sampling_rate (int): Sampling rate in s
     """
     from perun.backend import backends
 
     lSensors: List[Sensor] = []
     for backend in backends:
-        backend.setup()
         if backend.name in backendConfig:
             lSensors += backend.getSensors(backendConfig[backend.name])
 
     timesteps = []
     t_mT = MetricMetaData(
         Unit.SECOND,
         Magnitude.ONE,
@@ -288,19 +285,16 @@
         for idx, device in enumerate(lSensors):
             rawValues[idx].append(device.read())
 
     timesteps.append(time.time_ns())
     for idx, device in enumerate(lSensors):
         rawValues[idx].append(device.read())
 
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Stop event received.")
-    for backend in backends:
-        backend.close()
+    log.info(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Stop event received.")
 
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Closed backends")
     sensorNodes: Dict = {}
 
     t_s = np.array(timesteps)
     t_s -= t_s[0]
     t_s = t_s.astype("float32")
     t_s *= 1e-9
 
@@ -315,15 +309,15 @@
             deviceType=sensor.type,
             raw_data=RawData(t_s, np.array(values), t_mT, sensor.dataType),
         )
         # Apply processing to sensor node
         dn = processSensorData(dn)
         sensorNodes[sensor.type].append(dn)
 
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Preprocessed Sensor Data")
+    log.info(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Preprocessed Sensor Data")
     deviceGroupNodes = []
     for deviceType, sensorNodes in sensorNodes.items():
         if deviceType != DeviceType.NODE:
             dn = DataNode(
                 id=deviceType.value,
                 type=NodeType.DEVICE_GROUP,
                 metadata={},
@@ -332,23 +326,20 @@
             )
 
             dn = processDataNode(dn)
             deviceGroupNodes.append(dn)
         else:
             deviceGroupNodes.extend(sensorNodes)
 
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Preprocessed Device Data")
+    log.info(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Preprocessed Device Data")
 
     hostNode = DataNode(
         id=platform.node(),
         type=NodeType.NODE,
         metadata={},
         nodes={node.id: node for node in deviceGroupNodes},
     )
     processDataNode(hostNode)
 
     # This should send a single processed node for the current computational node
     queue.put(hostNode, block=True)
-    log.debug(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Sent data")
-
-    for backend in backends:
-        backend.close()
+    log.info(f"Rank {COMM_WORLD.Get_rank()}: Subprocess: Sent data")
```

### Comparing `perun-0.3.0/perun/processing.py` & `perun-0.3.2/perun/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,20 @@
                     metricType = MetricType.NET_WRITE
             else:
                 if "READ" in sensorData.id:
                     metricType = MetricType.DISK_READ
                 else:
                     metricType = MetricType.DISK_WRITE
 
-            result = rawData.values[-1] - rawData.values[0]
+            bytes_v = rawData.values
+            maxValue = rawData.v_md.max
+            dtype = rawData.v_md.dtype.name
+            d_bytes = bytes_v[1:] - bytes_v[:-1]
+            result = d_bytes.sum()
+
             sensorData.metrics[metricType] = Metric(
                 metricType,
                 result.astype(rawData.v_md.dtype),
                 rawData.v_md,
                 AggregateType.SUM,
             )
```

### Comparing `perun-0.3.0/perun/util.py` & `perun-0.3.2/perun/util.py`

 * *Files identical despite different names*

### Comparing `perun-0.3.0/pyproject.toml` & `perun-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perun"
-version = "0.3.0"
+version = "0.3.2"
 description = ""
 authors = ["Gutiérrez Hermosillo Muriedas, Juan Pedro <juanpedroghm@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/Helmholtz-AI-Energy/perun"
 
 [tool.poetry.scripts]
```

### Comparing `perun-0.3.0/PKG-INFO` & `perun-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun
-Version: 0.3.0
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/Helmholtz-AI-Energy/perun
 License: BSD-3-Clause
 Author: Gutiérrez Hermosillo Muriedas, Juan Pedro
 Author-email: juanpedroghm@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,16 @@
 <div align="center">
   <img src="https://raw.githubusercontent.com/Helmholtz-AI-Energy/perun/main/docs/images/full_logo.svg">
 </div>
 
 &nbsp;
 &nbsp;
 
-[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B%20%20%E2%97%8B-orange)](https://fair-software.eu)
+[![fair-software.eu](https://img.shields.io/badge/fair--software.eu-%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8F%20%20%E2%97%8B-yellow)](https://fair-software.eu)
+[![DOI](https://zenodo.org/badge/523363424.svg)](https://zenodo.org/badge/latestdoi/523363424)
 ![PyPI](https://img.shields.io/pypi/v/perun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/perun)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Documentation Status](https://readthedocs.org/projects/perun/badge/?version=latest)](https://perun.readthedocs.io/en/latest/?badge=latest)
```

