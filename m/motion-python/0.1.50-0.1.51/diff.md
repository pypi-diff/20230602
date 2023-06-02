# Comparing `tmp/motion_python-0.1.50.tar.gz` & `tmp/motion_python-0.1.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.50.tar", max compression
+gzip compressed data, was "motion_python-0.1.51.tar", max compression
```

## Comparing `motion_python-0.1.50.tar` & `motion_python-0.1.51.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-01 23:31:44.246602 motion_python-0.1.50/README.md
--rw-r--r--   0        0        0      202 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/__init__.py
--rw-r--r--   0        0        0     1817 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/component.py
--rw-r--r--   0        0        0    14036 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/execute.py
--rw-r--r--   0        0        0     5166 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/fit_task.py
--rw-r--r--   0        0        0     9364 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      595 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/route.py
--rw-r--r--   0        0        0     6283 2023-06-01 23:31:44.250602 motion_python-0.1.50/motion/utils.py
--rw-r--r--   0        0        0     1517 2023-06-01 23:32:08.100401 motion_python-0.1.50/pyproject.toml
--rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.50/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-02 00:11:05.158117 motion_python-0.1.51/README.md
+-rw-r--r--   0        0        0      202 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/cli.py
+-rw-r--r--   0        0        0    23617 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/component.py
+-rw-r--r--   0        0        0    14089 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/execute.py
+-rw-r--r--   0        0        0     5182 2023-06-02 00:11:05.158117 motion_python-0.1.51/motion/fit_task.py
+-rw-r--r--   0        0        0     9364 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      595 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/route.py
+-rw-r--r--   0        0        0     6283 2023-06-02 00:11:05.162117 motion_python-0.1.51/motion/utils.py
+-rw-r--r--   0        0        0     1555 2023-06-02 00:11:26.690306 motion_python-0.1.51/pyproject.toml
+-rw-r--r--   0        0        0     4050 1970-01-01 00:00:00.000000 motion_python-0.1.51/PKG-INFO
```

### Comparing `motion_python-0.1.50/README.md` & `motion_python-0.1.51/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/cli.py` & `motion_python-0.1.51/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/component.py` & `motion_python-0.1.51/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/execute.py` & `motion_python-0.1.51/motion/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,27 @@
         self._instance_name = instance_name
 
         self._init_state_func = init_state_func
         self._init_state_params = init_state_params
         self._load_state_func = load_state_func
         self._save_state_func = save_state_func
 
-        self.running = False
+        self.running: Any = multiprocessing.Value("b", False)
         self._redis_con = self._connectToRedis()
         try:
             self._redis_con.ping()
         except redis.exceptions.ConnectionError:
             rp = RedisParams()
             raise ConnectionError(
                 f"Could not connect to a Redis backend {rp}. "
                 + "Please set environment variables MOTION_REDIS_HOST, "
                 + "MOTION_REDIS_PORT, MOTION_REDIS_DB, and/or "
                 + "MOTION_REDIS_PASSWORD to your Redis params."
             )
-        self.running = True
+        self.running.value = True
 
         # Set up state
         self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
         self._state = CustomDict(self._instance_name, "state", {})
         if self.version is None:
             self.version = 1
             # Setup state
@@ -107,37 +107,38 @@
 
         return {}
 
     def _build_fit_jobs(self) -> None:
         """Builds fit jobs."""
         # Set up worker loops
         self.worker_tasks = {}
-        self.worker_stop_events = {}
+        # self.worker_stop_events = {}
+
         rp = RedisParams()
         # self.worker_states = {}
 
         for rkey, routes in self._fit_routes.items():
             for udf_name, route in routes.items():
                 pname = f"{self._instance_name}::{rkey}::{udf_name}"
-                worker_stop_event = multiprocessing.Event()
+                multiprocessing.Event()
                 self.worker_tasks[pname] = FitTask(
                     self._instance_name,
                     route,
                     batch_size=route.udf._batch_size,  # type: ignore
                     save_state_func=self._save_state_func,
                     load_state_func=self._load_state_func,
                     queue_identifier=self._get_queue_identifier(rkey, udf_name),
                     channel_identifier=self._get_channel_identifier(rkey, udf_name),
                     redis_host=rp.host,
                     redis_port=rp.port,
                     redis_db=rp.db,
                     redis_password=rp.password,  # type: ignore
-                    stop_event=worker_stop_event,
+                    running=self.running,
                 )
-                self.worker_stop_events[pname] = worker_stop_event
+                # self.worker_stop_events[pname] = worker_stop_event
                 self.worker_tasks[pname].start()
 
         # Set up a monitor thread
         self.stop_event = threading.Event()
         self.monitor_thread = threading.Thread(
             target=self._monitor_processes, daemon=True
         )
@@ -183,29 +184,30 @@
         return f"MOTION_QUEUE:{self._instance_name}/{route_key}/{udf_name}"
 
     def _get_channel_identifier(self, route_key: str, udf_name: str) -> str:
         """Gets the channel identifier for a given route key and UDF name."""
         return f"MOTION_CHANNEL:{self._instance_name}/{route_key}/{udf_name}"
 
     def shutdown(self, is_open: bool) -> None:
-        if not self.running:
+        if not self.running.value:
             return
 
         if is_open:
             logger.info("Running fit operations on remaining data...")
 
         # Set shutdown event
         self.stop_event.set()
+        self.running.value = False
 
         processes_to_wait_for = []
-        for pname, process in self.worker_tasks.items():
+        for process in self.worker_tasks.values():
             if psutil.pid_exists(process.pid):
                 # os.kill(process.pid, signal.SIGUSR1)  # type:ignore
                 # Set stop event
-                self.worker_stop_events[pname].set()
+                # self.worker_stop_events[pname].set()
                 processes_to_wait_for.append(process)
 
         self._redis_con.close()
 
         # Join fit processes
         for process in processes_to_wait_for:
             process.join()
```

### Comparing `motion_python-0.1.50/motion/fit_task.py` & `motion_python-0.1.51/motion/fit_task.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         load_state_func: Optional[Callable],
         queue_identifier: str,
         channel_identifier: str,
         redis_host: str,
         redis_port: int,
         redis_db: int,
         redis_password: str,
-        stop_event: Any,
+        running: Any,
     ):
         super().__init__()
         self.instance_name = instance_name
         self.save_state_func = save_state_func
         self.load_state_func = load_state_func
         self.redis_host = redis_host
         self.redis_port = redis_port
@@ -40,15 +40,16 @@
         self.channel_identifier = channel_identifier
 
         # Keep track of batch
         self.batch: List[Any] = []
 
         # Register the stop event
         # self.running = True
-        self.stop_event = stop_event
+        # self.stop_event = stop_event
+        self.running = running
 
     # def handle_signal(self, signum: int, frame: Any) -> None:
     #     logger.info("Received shutdown signal.")
     #     self.running = False
 
     def run(self) -> None:
         redis_con = redis.Redis(
@@ -57,34 +58,34 @@
             password=self.redis_password,
             db=self.redis_db,
         )
         # Acquire a lock
         lock_timeout = 300  # Lock timeout in seconds
         lock = Lock(redis_con, self.instance_name, lock_timeout)
 
-        while not self.stop_event.is_set():
+        while self.running.value:
             try:
                 for _ in range(self.batch_size):
                     item = redis_con.blpop(self.queue_identifier, timeout=1)
                     if item is None:
-                        if self.stop_event.is_set():
+                        if not self.running.value:
                             break  # no more items in the list
                         else:
                             continue
 
                     item, flush_fit = cloudpickle.loads(item[1])
                     self.batch.append(item)
                     if flush_fit:
                         break
             except redis.exceptions.ConnectionError:
                 logger.error("Connection to redis lost.")
                 break
 
             # Check if we should stop
-            if self.stop_event.is_set():
+            if not self.running.value:
                 self.cleanup()
                 break
 
             if not self.batch:
                 continue
 
             # Remove from batch if it was a noop
```

### Comparing `motion_python-0.1.50/motion/instance.py` & `motion_python-0.1.51/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.51/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/route.py` & `motion_python-0.1.51/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/motion/utils.py` & `motion_python-0.1.51/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.50/pyproject.toml` & `motion_python-0.1.51/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.50"
+version = "0.1.51"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -30,14 +30,16 @@
 pytkdocs = "^0.16.1"
 linkchecker = "^10.2.1"
 ruff = "^0.0.261"
 maturin = "^0.14.17"
 mike = "^1.1.2"
 scikit-learn = "^1.2.2"
 types-redis = "^4.5.5.2"
+fastapi = "^0.95.2"
+httpx = "^0.24.1"
 
 [tool.poetry.scripts]
 motion = "motion.cli:motioncli"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--basetemp=/tmp/pytest"
```

### Comparing `motion_python-0.1.50/PKG-INFO` & `motion_python-0.1.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.50
+Version: 0.1.51
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

