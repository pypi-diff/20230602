# Comparing `tmp/robocorp_tasks-0.3.0.tar.gz` & `tmp/robocorp_tasks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.3.0.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.4.0.tar", max compression
```

## Comparing `robocorp_tasks-0.3.0.tar` & `robocorp_tasks-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     4922 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/README.md
--rw-r--r--   0        0        0     1134 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1457 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5120 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     7935 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1123 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5267 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3738 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5487 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      870 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-05-25 10:44:18.577840 robocorp_tasks-0.3.0/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 robocorp_tasks-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/README.md
+-rw-r--r--   0        0        0     1166 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1457 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10160 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     4078 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3943 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     2436 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/_toml_settings.py
+-rw-r--r--   0        0        0      869 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-06-02 19:11:39.762458 robocorp_tasks-0.4.0/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 robocorp_tasks-0.4.0/PKG-INFO
```

### Comparing `robocorp_tasks-0.3.0/README.md` & `robocorp_tasks-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.3.0/pyproject.toml` & `robocorp_tasks-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.3.0"
+version = "0.4.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,22 +13,25 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.2.0"
+robocorp-log = "0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 robocorp-devutils = {path = "../devutils/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
 
+[tool.isort]
+profile = "black"
+
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "pytest_timeout.*"
 ignore_missing_imports = true
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/__init__.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,18 @@
   
 Note: Using the `cli.main(args)` is possible to run tasks programmatically, but
 clients using this approach MUST make sure that any code which must be
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
-from ._protocols import ITask
 
+from ._protocols import ITask
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_argdispatch.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import List
 from logging import getLogger
+from typing import List
 
 log = getLogger(__name__)
 
 
 class _ArgDispatcher:
     def __init__(self):
         self._name_to_func = {}
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import sys
 from pathlib import Path
-from typing import Iterator, List, Callable, Dict, Sequence
 from types import ModuleType
-import sys
+from typing import Callable, Dict, Iterator, List, Sequence
+
 from robocorp.tasks._protocols import ITask
 
 
 def module_name_from_path(path: Path, root: Path) -> str:
     """
     Return a dotted module name based on the given path, anchored on root.
     For example: path="projects/src/tests/test_foo.py" and root="/projects", the
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_commands.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from pathlib import Path
-from typing import Union, Sequence, List
-
 import json
 import os
 import sys
 import traceback
+from pathlib import Path
+from typing import List, Sequence, Union
 
 from ._argdispatch import arg_dispatch as _arg_dispatch
+import threading
 
 
 # Note: the args must match the 'dest' on the configured argparser.
 @_arg_dispatch.register(name="list")
 def list_tasks(
     path: str,
 ) -> int:
@@ -26,18 +26,19 @@
         },
         ...
     ]
 
     Args:
         path: The path (file or directory) from where tasks should be collected.
     """
+    from contextlib import redirect_stdout
+
     from robocorp.tasks._collect_tasks import collect_tasks
-    from robocorp.tasks._task import Context
     from robocorp.tasks._protocols import ITask
-    from contextlib import redirect_stdout
+    from robocorp.tasks._task import Context
 
     p = Path(path)
     context = Context()
     if not p.exists():
         context.show_error(f"Path: {path} does not exist")
         return 1
 
@@ -93,35 +94,31 @@
             Set to True so that if running tasks has an error inside the task
             the return code of the process is 0.
 
     Returns:
         0 if everything went well.
         1 if there was some error running the task.
     """
+    from robocorp.log import console, redirect
+
+    from robocorp.tasks._toml_settings import read_pyproject_toml
+
     from ._collect_tasks import collect_tasks
+    from ._config import RunConfig, set_config
+    from ._exceptions import RobocorpTasksCollectError
     from ._hooks import (
-        before_task_run,
+        after_all_tasks_run,
         after_task_run,
         before_all_tasks_run,
-        after_all_tasks_run,
-    )
-    from ._protocols import ITask
-    from ._task import Context
-    from ._protocols import Status
-    from ._exceptions import RobocorpTasksCollectError
-    from ._log_auto_setup import (
-        setup_cli_auto_logging,
-        read_pyproject_toml,
-        read_filters_from_pyproject_toml,
+        before_task_run,
     )
+    from ._log_auto_setup import read_robocorp_log_config, setup_cli_auto_logging
     from ._log_output_setup import setup_log_output
-    from ._config import RunConfig, set_config
-    from robocorp.log import redirect
-    from robocorp.log import console
-    from ._task import set_current_task
+    from ._protocols import ITask, Status
+    from ._task import Context, set_current_task
 
     console.set_mode(console_colors)
 
     # Don't show internal machinery on tracebacks:
     # setting __tracebackhide__ will make it so that robocorp-log
     # won't show this frame onwards in the logging.
     __tracebackhide__ = 1
@@ -143,24 +140,22 @@
         task_or_tasks = "task"
     else:
         task_names = task_name
         task_name = ", ".join(str(x) for x in task_names)
         task_or_tasks = "task" if len(task_names) == 1 else "tasks"
 
     config: log.BaseConfig
-    pyproject_path_and_contents = read_pyproject_toml(context, p)
+    pyproject_path_and_contents = read_pyproject_toml(p)
     pyproject_toml_contents: dict
-    if not pyproject_path_and_contents:
+    if pyproject_path_and_contents is None:
         config = log.ConfigFilesFiltering()
         pyproject_toml_contents = {}
     else:
-        pyproject, pyproject_toml_contents = pyproject_path_and_contents
-        config = read_filters_from_pyproject_toml(
-            context, pyproject, pyproject_toml_contents
-        )
+        config = read_robocorp_log_config(context, pyproject_path_and_contents)
+        pyproject_toml_contents = pyproject_path_and_contents.toml_contents
 
     run_config = RunConfig(
         Path(output_dir),
         p,
         task_names,
         max_log_files,
         max_log_file_size,
@@ -238,13 +233,74 @@
                     finally:
                         after_task_run(task)
                         set_current_task(None)
             finally:
                 log.start_task("Teardown tasks", "teardown", "", 0)
                 try:
                     after_all_tasks_run(tasks)
+                    # Always do a process snapshot as the process is about to finish.
+                    log.process_snapshot()
                 finally:
                     log.end_task("Teardown tasks", "teardown", Status.PASS, "")
 
             return returncode
         finally:
             log.end_run(run_name, run_status)
+
+            # After the run is finished, start a timer which will print the
+            # current threads if the process doesn't exit after a given timeout.
+            from threading import Timer
+
+            var_name = "RC_DUMP_THREADS_AFTER_RUN_TIMEOUT"
+            try:
+                timeout = float(os.environ.get(var_name, "40"))
+            except:
+                sys.stderr.write(
+                    f"Invalid value for: {var_name} environment value. Cannot convert to float."
+                )
+                timeout = 40
+
+            def on_timeout():
+                _dump_threads(
+                    message=f"All tasks have run but the process still hasn't exited after {timeout} seconds. Showing threads found:"
+                )
+
+            t = Timer(timeout, on_timeout)
+            t.daemon = True
+            t.start()
+
+
+def _dump_threads(stream=None, message="Threads found"):
+    if stream is None:
+        stream = sys.stderr
+
+    thread_id_to_name = {}
+    try:
+        for t in threading.enumerate():
+            thread_id_to_name[t.ident] = "%s  (daemon: %s)" % (t.name, t.daemon)
+    except:
+        pass
+
+    stack_trace = [
+        "===============================================================================",
+        message,
+        "================================= Thread Dump =================================",
+    ]
+
+    for thread_id, stack in sys._current_frames().items():
+        stack_trace.append(
+            "\n-------------------------------------------------------------------------------"
+        )
+        stack_trace.append(" Thread %s" % thread_id_to_name.get(thread_id, thread_id))
+        stack_trace.append("")
+
+        if "self" in stack.f_locals:
+            sys.stderr.write(str(stack.f_locals["self"]) + "\n")
+
+        for filename, lineno, name, line in traceback.extract_stack(stack):
+            stack_trace.append(' File "%s", line %d, in %s' % (filename, lineno, name))
+            if line:
+                stack_trace.append("   %s" % (line.strip()))
+    stack_trace.append(
+        "\n=============================== END Thread Dump ==============================="
+    )
+    stream.write("\n".join(stack_trace))
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_config.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_config.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Optional, Sequence
 from pathlib import Path
+from typing import Optional, Sequence
 
 
 class RunConfig:
     def __init__(
         self,
         output_dir: Path,
         path: Path,
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_hooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from ._callback import Callback
 from ._protocols import (
-    IOnTaskFuncFoundCallback,
-    IBeforeCollectTasksCallback,
-    IBeforeTaskRunCallback,
+    IAfterAllTasksRunCallback,
     IAfterTaskRunCallback,
     IBeforeAllTasksRunCallback,
-    IAfterAllTasksRunCallback,
+    IBeforeCollectTasksCallback,
+    IBeforeTaskRunCallback,
+    IOnTaskFuncFoundCallback,
 )
 
-
 # Called as on_task_func_found(task: ITask)
 on_task_func_found: IOnTaskFuncFoundCallback = Callback()
 
 # Called as before_collect_tasks(path: Path, task_names: Set[str])
 before_collect_tasks: IBeforeCollectTasksCallback = Callback()
 
 # Called as before_all_tasks_run(tasks: List[ITask])
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_protocols.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import typing
+from dataclasses import dataclass
 from pathlib import Path
 from types import TracebackType
-from typing import TypeVar, Optional, Any, Callable, Set, Sequence, Union
-import typing
-
+from typing import Any, Callable, Optional, Sequence, Set, TypeVar, Union
 
 ExcInfo = tuple[type[BaseException], BaseException, TracebackType]
 OptExcInfo = Union[ExcInfo, tuple[None, None, None]]
 
 
 T = TypeVar("T")
 Y = TypeVar("Y", covariant=True)
@@ -34,14 +34,20 @@
     PASS = "PASS"
     ERROR = "ERROR"
     FAIL = "FAIL"
     INFO = "INFO"
     WARN = "WARN"
 
 
+@dataclass
+class PyProjectInfo:
+    pyproject: Path
+    toml_contents: dict
+
+
 class ITask(typing.Protocol):
     module_name: str
     filename: str
     method: typing.Callable
 
     status: str
     message: str
@@ -62,14 +68,19 @@
     def failed(self) -> bool:
         """
         Returns true if the task failed.
         (in which case usually exc_info is not None).
         """
 
 
+class IContextErrorReport(typing.Protocol):
+    def show_error(self, message):
+        pass
+
+
 class ICallback(typing.Protocol):
     """
     Note: the actual __call__ must be defined in a subclass protocol.
     """
 
     def register(self, callback):
         pass
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import typing
-from types import ModuleType
-from robocorp.tasks._protocols import Status, ITask
 from contextlib import contextmanager
-from typing import Optional, Tuple, List
-from robocorp.log.protocols import OptExcInfo
+from types import ModuleType
+from typing import List, Optional, Tuple
+
 from robocorp.log import ConsoleMessageKind, console_message
+from robocorp.log.protocols import OptExcInfo
+
+from robocorp.tasks._protocols import ITask, Status
 
 
 class Task:
     def __init__(self, module: ModuleType, method: typing.Callable):
         self.module_name = module.__name__
         self.filename = module.__file__ or "<filename unavailable>"
         self.method = method
@@ -172,13 +174,13 @@
                     kind=self.KIND_TRACEBACK,
                 )
 
         self._show_header([])
 
     @contextmanager
     def register_lifecycle_prints(self):
-        from ._hooks import before_task_run, after_task_run
+        from ._hooks import after_task_run, before_task_run
 
         with before_task_run.register(self._before_task_run), after_task_run.register(
             self._after_task_run
         ):
             yield
```

### Comparing `robocorp_tasks-0.3.0/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.4.0/src/robocorp/tasks/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 Note: when running tasks, clients using this approach MUST make sure that any
 code which must be automatically logged is not imported prior the the `cli.main`
 call.
 """
 
 import sys
 
-from ._argdispatch import arg_dispatch as _arg_dispatch
-
 # Just importing is enough to register the commands
 from . import _commands  # @UnusedImport
+from ._argdispatch import arg_dispatch as _arg_dispatch
 
 
 def main(args=None, exit: bool = True) -> int:
     """Entry point for running tasks from robocorp-tasks."""
     if args is None:
         args = sys.argv[1:]
     returncode = _arg_dispatch.process_args(args)
```

### Comparing `robocorp_tasks-0.3.0/PKG-INFO` & `robocorp_tasks-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.3.0
+Version: 0.4.0
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.2.0)
+Requires-Dist: robocorp-log (==0.3.0)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
 `robocorp-tasks` is a Python framework designed to simplify the development 
 of Python automations.
```

