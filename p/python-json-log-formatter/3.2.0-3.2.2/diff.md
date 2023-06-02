# Comparing `tmp/python_json_log_formatter-3.2.0.tar.gz` & `tmp/python_json_log_formatter-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_json_log_formatter-3.2.0.tar", last modified: Tue May 23 12:59:55 2023, max compression
+gzip compressed data, was "python_json_log_formatter-3.2.2.tar", last modified: Fri Jun  2 16:01:43 2023, max compression
```

## Comparing `python_json_log_formatter-3.2.0.tar` & `python_json_log_formatter-3.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.490592 python_json_log_formatter-3.2.0/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.0/LICENSE
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3400 2023-05-23 12:59:55.490423 python_json_log_formatter-3.2.0/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2769 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/README.md
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      941 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/pyproject.toml
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.489254 python_json_log_formatter-3.2.0/python_json_log_formatter/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1110 2022-12-15 13:46:18.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       92 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11953 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      553 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.pyi
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/py.typed
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5305 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.py
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      658 2023-05-23 12:59:38.000000 python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.pyi
-drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-05-23 12:59:55.490194 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3400 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/PKG-INFO
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)      540 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-05-23 12:59:55.000000 python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/top_level.txt
--rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-05-23 12:59:55.490638 python_json_log_formatter-3.2.0/setup.cfg
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.024443 python_json_log_formatter-3.2.2/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    11358 2022-11-24 16:19:23.000000 python_json_log_formatter-3.2.2/LICENSE
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-06-02 16:01:43.024285 python_json_log_formatter-3.2.2/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     2793 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/README.md
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      945 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/pyproject.toml
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.023209 python_json_log_formatter-3.2.2/python_json_log_formatter/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     1195 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       93 2023-06-02 13:54:12.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       21 2023-06-02 16:00:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/_version.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       16 2023-06-02 14:51:25.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/_version.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)    12647 2023-06-02 16:00:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      553 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.pyi
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        0 2022-12-13 12:36:44.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/py.typed
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     5397 2023-06-02 14:13:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.py
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      574 2023-06-02 14:51:06.000000 python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.pyi
+drwxr-xr-x   0 nielskorschinsky   (501) staff       (20)        0 2023-06-02 16:01:43.024060 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)     3424 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)      617 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)        1 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       26 2023-06-02 16:01:43.000000 python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/top_level.txt
+-rw-r--r--   0 nielskorschinsky   (501) staff       (20)       38 2023-06-02 16:01:43.024490 python_json_log_formatter-3.2.2/setup.cfg
```

### Comparing `python_json_log_formatter-3.2.0/LICENSE` & `python_json_log_formatter-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.0/PKG-INFO` & `python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python_json_log_formatter
-Version: 3.2.0
+Name: python-json-log-formatter
+Version: 3.2.2
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,27 @@
 3. After the imports, please declare a version constant. \
     This constant should use [semantic versioning](https://semver.org/#semantic-versioning-specification-semver), with a prepended date `(YYYY/MM/DD)`.\
     Other examples, without the date, can be found [here](https://ihateregex.io/expr/semver/)
 4. Before any argument parsing or any other logging, the logger should be initialized
 5. In **EVERY** file, the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION)
 
 LOGGER = logging.getLogger(__name__)
 ```
 
 Optionally, it is also possible to change the log level:
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION, logging.DEBUG)
 
 LOGGER = logging.getLogger(__name__)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.0 Summary:
+Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.2 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
@@ -18,19 +18,19 @@
 module, using a `from module import class` statement. 3. After the imports,
 please declare a version constant. \ This constant should use [semantic
 versioning](https://semver.org/#semantic-versioning-specification-semver), with
 a prepended date `(YYYY/MM/DD)`.\ Other examples, without the date, can be
 found [here](https://ihateregex.io/expr/semver/) 4. Before any argument parsing
 or any other logging, the logger should be initialized 5. In **EVERY** file,
 the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
-```python from python_logger import PythonLogger import logging VERSION =
-"1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
+```python from python_json_log_formatter import PythonLogger import logging
+VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
 logging.getLogger(__name__) ``` Optionally, it is also possible to change the
-log level: ```python from python_logger import PythonLogger import logging
-VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
+log level: ```python from python_json_log_formatter import PythonLogger import
+logging VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
 logging.DEBUG) LOGGER = logging.getLogger(__name__) ``` ## Features Sets the
 logging format for the root logger and thus for every child logger. In EVERY
 file where logging happens, please use `LOGGER = logging.getLogger(__name__)`
 to get an individual logger. Allows printing exception information on any
 logging level, not only on the `EXCEPTION` level but also for `INFO` or
 `DEBUG`. Supply `exec_info` to print these. Sets `pipeline_status` and
 `job_status` to `failed` on `CRITICAL`, supports minor logging levels (41,
```

### Comparing `python_json_log_formatter-3.2.0/README.md` & `python_json_log_formatter-3.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 3. After the imports, please declare a version constant. \
     This constant should use [semantic versioning](https://semver.org/#semantic-versioning-specification-semver), with a prepended date `(YYYY/MM/DD)`.\
     Other examples, without the date, can be found [here](https://ihateregex.io/expr/semver/)
 4. Before any argument parsing or any other logging, the logger should be initialized
 5. In **EVERY** file, the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION)
 
 LOGGER = logging.getLogger(__name__)
 ```
 
 Optionally, it is also possible to change the log level:
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION, logging.DEBUG)
 
 LOGGER = logging.getLogger(__name__)
 ```
```

#### html2text {}

```diff
@@ -10,19 +10,19 @@
 module, using a `from module import class` statement. 3. After the imports,
 please declare a version constant. \ This constant should use [semantic
 versioning](https://semver.org/#semantic-versioning-specification-semver), with
 a prepended date `(YYYY/MM/DD)`.\ Other examples, without the date, can be
 found [here](https://ihateregex.io/expr/semver/) 4. Before any argument parsing
 or any other logging, the logger should be initialized 5. In **EVERY** file,
 the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
-```python from python_logger import PythonLogger import logging VERSION =
-"1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
+```python from python_json_log_formatter import PythonLogger import logging
+VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
 logging.getLogger(__name__) ``` Optionally, it is also possible to change the
-log level: ```python from python_logger import PythonLogger import logging
-VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
+log level: ```python from python_json_log_formatter import PythonLogger import
+logging VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
 logging.DEBUG) LOGGER = logging.getLogger(__name__) ``` ## Features Sets the
 logging format for the root logger and thus for every child logger. In EVERY
 file where logging happens, please use `LOGGER = logging.getLogger(__name__)`
 to get an individual logger. Allows printing exception information on any
 logging level, not only on the `EXCEPTION` level but also for `INFO` or
 `DEBUG`. Supply `exec_info` to print these. Sets `pipeline_status` and
 `job_status` to `failed` on `CRITICAL`, supports minor logging levels (41,
```

### Comparing `python_json_log_formatter-3.2.0/pyproject.toml` & `python_json_log_formatter-3.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/IBM/python-json-log-formatter"
 "Bug Tracker" = "https://github.com/IBM/python-json-log-formatter/issues"
 
 [tool.setuptools.dynamic]
-version = {attr = "python_json_log_formatter.VERSION"}
+version = {attr = "python_json_log_formatter.__version__"}
 
 [tool.setuptools]
 packages = ["python_json_log_formatter"]
 
 [tool.setuptools.package-data]
 python_json_log_formatter = ["*.pyi", "*.py", "py.typed"]
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter/__init__.py` & `python_json_log_formatter-3.2.2/python_json_log_formatter/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,10 +22,11 @@
 Repository:
   https://github.com/IBM/python_json_log_formatter
 
 Author:
  Niels Korschinsky
 """
 
-__all__ = ["PythonLogger", "VERSION"]
+__all__ = ["PythonLogger", "__version__"]
 
-from python_json_log_formatter.python_json_log_formatter import PythonLogger, VERSION
+from python_json_log_formatter.python_json_log_formatter import PythonLogger as PythonLogger
+from python_json_log_formatter._version import __version__ as __version__
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.py` & `python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def __init__(self, context: Dict[str, str], disable_log_formatting: bool = False) -> None:
         super().__init__()
         self.__disable_log_formatting = disable_log_formatting
         self.__context: Dict[str, str] = {}
         self.update_context(context)
 
-    def __add_env_variables(self, context_dict: Mapping[str, str]) -> Dict[str, Any]:
+    def __add_selected_env_vars_to_context(self, context_dict: Mapping[str, str]) -> Dict[str, Any]:
         """Creates a union of the existing context data and included environment variables.
 
         The result will be a new dictionary containing both keys,
         If a key exists in both the context and the env, the context has higher priority.
         A warning will be issued.
 
         Args:
@@ -156,70 +156,83 @@
 
         This static context will then applied onto every logging line.
 
         Args:
             context (Dict[str, str]): New logging context to be applied as static context
         """
 
-        new_dict = self.__add_env_variables(new_context_dict)
+        new_dict = self.__add_selected_env_vars_to_context(new_context_dict)
 
         job_retries_context = self.__calculate_remaining_job_retries()
         new_dict.update(job_retries_context)
 
         self.__context.update(new_dict)
 
     def __add_log_record_info(self, record: LogRecord) -> Dict[str, Any]:
-        """Extracts log record information into a logging dict context.
+        """Extracts log record information into a new logging dict context.
 
         Used for transferring certain required information into the new logging context to avoid loosing this data.
 
         Args:
-            new_record_dict (Dict[str, Any]): The new context which will receive the existing data, overwriting existing entries.
-            old_record (LogRecord): old context of the log
+            record (LogRecord): the log record which contents will be transferred
+
+        Returns:
+            Dict[str, Any]: Dict with context information to be merged into other context information
         """
 
         # add all available attributes of the record
         # copy to ensure to not edit the record itself
         new_dict: Dict[str, Any] = record.__dict__.copy()
 
         for key in self.__excluded_logging_context_keys:
             new_dict.pop(key, None)
 
-        # add exec info to the message if available
-        message = record.msg
-        if record.exc_info:
-
-            # get the individual parts
-            exc_type, exc_value, exc_traceback = record.exc_info
-
-            # only save the trace
-            exc_info = ''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))
-
-            # delete the info from the saved dict
-            new_dict.pop("exc_info")
-
-            # append it to the message to have it displayed as log message
-            message = message + '\n' + exc_info
-
-        # remove msg, unsure whether the logging tool parser requires msg or message.
-        new_dict.pop("msg", None)
-        new_dict['message'] = message
-
+        new_dict["level"] = record.levelname
+        new_dict["message"] = record.msg
 
         # Add arguments individual to the new record message
         if isinstance(record.args, dict):
             for k, v in record.args.items():
                 new_dict[k] = v
             # set them to empty, as already included
             record.args = {}
             # remove it from the new_dict, as they are saved individually
             new_dict.pop("args", None)
 
         return new_dict
 
+    def __add_available_exec_info(self, new_record_dict: Dict[str, Any], record: LogRecord):
+        """Updates the provided context information with exc_information from the log record.
+
+        Will remove the exc_info from the record.
+        Updates the message of the context dict.
+
+        Args:
+            new_record_dict (Dict[str, Any]): Context dict with existing message and other information
+            record (LogRecord): LogRecord with possible exc_info field
+        """
+
+        message = new_record_dict['message']
+
+        if record.exc_info:
+
+            # get the individual parts
+            exc_type, exc_value, exc_traceback = record.exc_info
+
+            # only save the trace
+            exc_info = ''.join(traceback.format_exception(exc_type, exc_value, exc_traceback))
+
+            # delete the info from the saved dict
+            new_record_dict.pop("exc_info", None)
+            # Clear record.exc_info
+            record.exc_info = None
+
+            # append it to the message to have it displayed as log message
+            new_record_dict['message'] = message + '\n' + exc_info
+
     def __check_is_imported_module(self, path_name: str) -> bool:
         work_dir = Path(getcwd())
         log_path = Path(path_name)
 
         # from python 3.9 the main module should always be absolute, but sometimes it is not somehow.
         # make sure the path is absolute
         if not log_path.is_absolute():
@@ -299,16 +312,20 @@
 
         new_dict = self.__add_log_record_info(record)
         new_record_msg.update(new_dict)
 
         new_dict = self.__check_failed_pipeline_status(record)
         new_record_msg.update(new_dict)
 
+        # Add exception info to log message
+        self.__add_available_exec_info(new_record_msg, record)
+
+        # Override record message and clear record args
         dumped_new_dict = json.dumps(new_record_msg)
         if not self.__disable_log_formatting:
             # Override record message and clear record args
             record.msg = dumped_new_dict
         else:
             # save it in new attribute, will not be shown.
             record.log_formatting_message = dumped_new_dict
 
-        return True
+        return True
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter/context_filter.pyi` & `python_json_log_formatter-3.2.2/python_json_log_formatter/context_filter.pyi`

 * *Files identical despite different names*

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.py` & `python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,15 @@
 
 from logging import INFO, StreamHandler, basicConfig
 from os import getenv
 import re
 from typing import ClassVar, Dict, List, Optional
 
 from python_json_log_formatter.context_filter import ContextFilter
-
-
-VERSION = "3.2.0"
+from python_json_log_formatter._version import __version__
 
 class PythonLogger:
     """This class wraps functions used for logging for an easier, direct access.
 
     Methods:
         setup_logger - Configures the root as required. To be called before any logging commands in the main file (very top).
         update_context -
@@ -102,14 +100,15 @@
 
         handler = StreamHandler()
 
         context_dict = extra_context_dict or {}
         if app:
             context_dict["app"] = app
         context_dict["version"] = version_constant
+        context_dict["logger_version"] = __version__
         cls.__context_filter = ContextFilter(context_dict, disable_log_formatting)
         handler.addFilter(cls.__context_filter)
         basicConfig(
             level=logging_level,
             format="[%(asctime)s %(name)s] %(levelname)s: %(message)s",
             handlers=[handler]
     )
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter/python_json_log_formatter.pyi` & `python_json_log_formatter-3.2.2/python_json_log_formatter/python_json_log_formatter.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from python_json_log_formatter.context_filter import ContextFilter as ContextFilter
 from typing import Dict, List, Optional
 
 VERSION: str
 
 class PythonLogger:
     @property
     def excluded_logging_context_keys(self) -> List[str]: ...
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/PKG-INFO` & `python_json_log_formatter-3.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: python-json-log-formatter
-Version: 3.2.0
+Name: python_json_log_formatter
+Version: 3.2.2
 Summary: Supplements a default formatter configuration for machine-readable JSON logging and applies it
 Author-email: Niels Korschinsky <niels.korschinsky@ibm.com>
 Project-URL: Homepage, https://github.com/IBM/python-json-log-formatter
 Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-formatter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -35,27 +35,27 @@
 3. After the imports, please declare a version constant. \
     This constant should use [semantic versioning](https://semver.org/#semantic-versioning-specification-semver), with a prepended date `(YYYY/MM/DD)`.\
     Other examples, without the date, can be found [here](https://ihateregex.io/expr/semver/)
 4. Before any argument parsing or any other logging, the logger should be initialized
 5. In **EVERY** file, the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION)
 
 LOGGER = logging.getLogger(__name__)
 ```
 
 Optionally, it is also possible to change the log level:
 
 ```python
-from python_logger import PythonLogger
+from python_json_log_formatter import PythonLogger
 import logging
 
 VERSION = "1.0.0 (2022/11/24)"
 PythonLogger.setup_logger(VERSION, logging.DEBUG)
 
 LOGGER = logging.getLogger(__name__)
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-json-log-formatter Version: 3.2.0 Summary:
+Metadata-Version: 2.1 Name: python_json_log_formatter Version: 3.2.2 Summary:
 Supplements a default formatter configuration for machine-readable JSON logging
 and applies it Author-email: Niels Korschinsky
 korschinsky@ibm.com> Project-URL: Homepage, https://github.com/IBM/python-json-
 log-formatter Project-URL: Bug Tracker, https://github.com/IBM/python-json-log-
 formatter/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
@@ -18,19 +18,19 @@
 module, using a `from module import class` statement. 3. After the imports,
 please declare a version constant. \ This constant should use [semantic
 versioning](https://semver.org/#semantic-versioning-specification-semver), with
 a prepended date `(YYYY/MM/DD)`.\ Other examples, without the date, can be
 found [here](https://ihateregex.io/expr/semver/) 4. Before any argument parsing
 or any other logging, the logger should be initialized 5. In **EVERY** file,
 the logger needs to be imported using `LOGGER = logging.getLogger(__name__)`
-```python from python_logger import PythonLogger import logging VERSION =
-"1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
+```python from python_json_log_formatter import PythonLogger import logging
+VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION) LOGGER =
 logging.getLogger(__name__) ``` Optionally, it is also possible to change the
-log level: ```python from python_logger import PythonLogger import logging
-VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
+log level: ```python from python_json_log_formatter import PythonLogger import
+logging VERSION = "1.0.0 (2022/11/24)" PythonLogger.setup_logger(VERSION,
 logging.DEBUG) LOGGER = logging.getLogger(__name__) ``` ## Features Sets the
 logging format for the root logger and thus for every child logger. In EVERY
 file where logging happens, please use `LOGGER = logging.getLogger(__name__)`
 to get an individual logger. Allows printing exception information on any
 logging level, not only on the `EXCEPTION` level but also for `INFO` or
 `DEBUG`. Supply `exec_info` to print these. Sets `pipeline_status` and
 `job_status` to `failed` on `CRITICAL`, supports minor logging levels (41,
```

### Comparing `python_json_log_formatter-3.2.0/python_json_log_formatter.egg-info/SOURCES.txt` & `python_json_log_formatter-3.2.2/python_json_log_formatter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 python_json_log_formatter/__init__.py
 python_json_log_formatter/__init__.pyi
+python_json_log_formatter/_version.py
+python_json_log_formatter/_version.pyi
 python_json_log_formatter/context_filter.py
 python_json_log_formatter/context_filter.pyi
 python_json_log_formatter/py.typed
 python_json_log_formatter/python_json_log_formatter.py
 python_json_log_formatter/python_json_log_formatter.pyi
 python_json_log_formatter.egg-info/PKG-INFO
 python_json_log_formatter.egg-info/SOURCES.txt
```

