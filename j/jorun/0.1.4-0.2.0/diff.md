# Comparing `tmp/jorun-0.1.4.tar.gz` & `tmp/jorun-0.2.0.tar.gz`

## Comparing `jorun-0.1.4.tar` & `jorun-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jorun-0.1.4/jorun.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/configuration.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/errors.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/logger.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/main.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/runner.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/runner_thread.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/scanner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/__init__.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/base.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/docker.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/group.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/handler/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/base.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/palette/darcula.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/options.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/types/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/__init__.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/application.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/data_signals.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/main_window.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/pane.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 jorun-0.1.4/src/jorun/ui/task_panel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.1.4/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.1.4/LICENSE
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.1.4/README.md
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 jorun-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 jorun-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 jorun-0.2.0/jorun.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/configuration.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/errors.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/logger.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/main.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/runner.py
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/runner_process.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/scanner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/__init__.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/base.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/docker.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/group.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/handler/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/base.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/palette/darcula.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/options.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/types/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/application.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/data_signals.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/main_window.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/pane.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 jorun-0.2.0/src/jorun/ui/task_panel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jorun-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jorun-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 jorun-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jorun-0.2.0/README.md
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 jorun-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 jorun-0.2.0/PKG-INFO
```

### Comparing `jorun-0.1.4/jorun.yml` & `jorun-0.2.0/jorun.yml`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/configuration.py` & `jorun-0.2.0/src/jorun/configuration.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/logger.py` & `jorun-0.2.0/src/jorun/logger.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/main.py` & `jorun-0.2.0/src/jorun/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 import argparse
-import asyncio
 import sys
 import traceback
 from logging.handlers import QueueHandler
-from queue import Queue
+from multiprocessing import Queue
 from tinyioc import register_instance
 
-from jorun.runner_thread import RunnerThread
+from jorun.runner_process import RunnerProcess
 from .palette.base import BaseColorPalette
 from .palette.darcula import DarculaColorPalette
 from .ui.application import UiApplication
 from .handler.group import GroupTaskHandler
 from .handler.docker import DockerTaskHandler
 from .handler.shell import ShellTaskHandler
 
@@ -35,19 +34,14 @@
 ui_application: UiApplication
 
 
 def main():
     global program_arguments, ui_application
 
     register_instance(DarculaColorPalette(), register_for=BaseColorPalette)
-    register_instance(AppConfiguration([
-        ShellTaskHandler(),
-        DockerTaskHandler(),
-        GroupTaskHandler()
-    ]))
 
     program_arguments = parser.parse_args()
     logger.setLevel(program_arguments.level)
 
     logger.debug("Loading configuration file")
     config: TasksConfiguration = load_config(program_arguments.configuration_file)
 
@@ -64,15 +58,15 @@
     if show_gui:
         logger.debug("Using graphical interface")
         log_handler = QueueHandler(task_streams_queue)
     else:
         logger.debug("Using console output")
         log_handler = NewlineStreamHandler(sys.stdout)
 
-    tasks_thread = RunnerThread(tasks_config, program_arguments, log_handler)
+    tasks_thread = RunnerProcess(tasks_config, program_arguments, show_gui, task_streams_queue)
     tasks_thread.start()
 
     try:
         if show_gui:
             ui_tasks = [t_name for t_name, t_val in missing_tasks.items() if t_val["type"] != "group"]
 
             ui_application = UiApplication(ui_tasks, task_streams_queue, gui_config)
@@ -81,13 +75,18 @@
             tasks_thread.join()
     except KeyboardInterrupt:
         logger.debug("Requested termination")
     except Exception as e:
         logger.error("An error occurred")
         traceback.print_exception(e)
     finally:
-        ui_application.stop_ui()
-        tasks_thread.stop()
+        if show_gui:
+            logger.debug("Quitting the UI")
+            ui_application.stop_ui()
+        logger.debug("Quitting the tasks")
+        tasks_thread.stop(10)
+
+    logger.debug("Terminated")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jorun-0.1.4/src/jorun/runner.py` & `jorun-0.2.0/src/jorun/runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import asyncio
 import logging
 import os.path
+import platform
+import signal
+import time
 from asyncio.subprocess import Process
 from datetime import datetime
 from logging import Logger
 from typing import Optional, Callable, List, Union
+
+import psutil
 from tinyioc import inject
 
 from .handler.base import BaseTaskHandler
+from .logger import logger
 from .scanner import AsyncScanner
 from .types.options import TaskOptions
 from .types.task import Task
 from .configuration import AppConfiguration
 
 OUTPUT_READ_INTERVAL = 0.015
 
@@ -64,18 +70,37 @@
     @property
     def name(self):
         return self._task["name"]
 
     def _on_stop(self):
         self._handler.on_exit(self._task[self._handler.task_type], self._process)
 
-    def stop(self):
+    def stop(self, timeout=1):
         if self._process and self._process.returncode is None:
+            logger.debug(f"Process {self.name} is alive. Killing it")
+
             self._on_stop()
-            self._process.terminate()
+            pid = self._process.pid
+
+            if platform.system() == "Windows":
+                os.kill(pid, signal.CTRL_C_EVENT)
+            else:
+                os.kill(pid, signal.SIGTERM)
+
+            timeout_left = timeout
+            while timeout_left > 0 and psutil.pid_exists(pid):
+                time.sleep(0.2)
+                timeout_left -= 0.2
+
+            if psutil.pid_exists(pid):
+                logger.debug(f"Process {self.name} still alive after {timeout}s timeout. Sending SIGKILL")
+                if platform.system() == "Windows":
+                    os.kill(pid, signal.CTRL_BREAK_EVENT)
+                else:
+                    os.kill(pid, signal.SIGKILL)
 
     async def start(self, completion_callback: Callable):
         try:
             self._completion_callback = completion_callback
             t = self._task
 
             stderr_redirect = t.get('pattern_in_stderr', False)
```

### Comparing `jorun-0.1.4/src/jorun/runner_thread.py` & `jorun-0.2.0/src/jorun/runner_process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,63 @@
+import multiprocessing
+import queue
+import sys
+from logging.handlers import QueueHandler
+from multiprocessing.connection import Connection
 from threading import Thread
 from typing import List, Set, Dict, Optional
 import asyncio
 import logging
 import traceback
 
 from tinyioc import module, IocModule, register_instance, unregister_service
 
+from .configuration import AppConfiguration
+from .handler.docker import DockerTaskHandler
+from .handler.group import GroupTaskHandler
+from .handler.shell import ShellTaskHandler
 from .types.task import Task
 from .runner import TaskRunner
-from .logger import logger
+from .logger import logger, NewlineStreamHandler
 
 
 @module()
 class RunnerThreadModule(IocModule):
     pass
 
 
-class RunnerThread(Thread):
+class RunnerProcess(multiprocessing.Process):
     _running: bool
+    _pipe_emit: Connection
+    _pipe_recv: Connection
 
     _config: Dict[str, Task]
     _arguments: any
     _running_tasks: List[TaskRunner]
     _async_tasks: Set[asyncio.Task]
 
     _missing_tasks: Dict[str, Task]
     _completed_tasks: Set[str]
 
+    _queue: multiprocessing.Queue
     _log_handler: logging.Handler
     _show_gui: bool
 
     _loop: asyncio.AbstractEventLoop
 
-    def __init__(self, configuration: Dict[str, Task], arguments: any, log_handler: logging.Handler):
-        super(RunnerThread, self).__init__()
+    def __init__(self, configuration: Dict[str, Task], arguments: any, is_gui: bool,
+                 output_queue: Optional[multiprocessing.Queue]):
+        super(RunnerProcess, self).__init__()
 
+        self._show_gui = is_gui
         self._config = configuration
         self._arguments = arguments
-        self._log_handler = log_handler
-        self._running_tasks = []
-        self._async_tasks = set()
-        self._missing_tasks = configuration.copy()
-        self._completed_tasks = set()
+        self._queue = output_queue
+
+        self._pipe_recv, self._pipe_emit = multiprocessing.Pipe()
 
     def _run_missing_tasks(self):
         tasks_to_run: List[Task] = [t for t in self._missing_tasks.values() if
                                     (not t.get("depends") or len(t["depends"]) == 0) or set(t["depends"]).issubset(
                                         self._completed_tasks)]
 
         for task in tasks_to_run:
@@ -81,44 +93,73 @@
             except:
                 pass
             finally:
                 self._running_tasks.pop(i)
 
     def _cancel_async_tasks(self):
         logger.debug("Killing async tasks...")
-        for t in self._async_tasks:
+        for t in self._async_tasks.copy():
             t.cancel()
 
     def run(self) -> None:
+        register_instance(AppConfiguration([
+            ShellTaskHandler(),
+            DockerTaskHandler(),
+            GroupTaskHandler()
+        ]))
+
+        self._log_handler = QueueHandler(self._queue) if self._show_gui else NewlineStreamHandler(sys.stdout)
+        self._running_tasks = []
+        self._async_tasks = set()
+        self._missing_tasks = self._config.copy()
+        self._completed_tasks = set()
+
         self._running = True
 
         self._loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(self._loop)
+
         register_instance(self._loop, module=RunnerThreadModule, register_for=asyncio.AbstractEventLoop)
 
+        async def periodic_termination_checker():
+            while self._running:
+                if self._pipe_recv.poll():
+                    self._loop.call_soon_threadsafe(self._loop.stop)
+                    break
+
+                await asyncio.sleep(0.3)
+
         try:
             self._run_missing_tasks()
+
+            term_task = self._loop.create_task(periodic_termination_checker())
+            self._async_tasks.add(term_task)
+            term_task.add_done_callback(self._async_tasks.discard)
+
             self._loop.run_forever()
         except KeyboardInterrupt:
             logger.info("Requested termination")
         except Exception as e:
             logger.error("An error occurred")
             traceback.print_exception(e)
         finally:
             unregister_service(asyncio.AbstractEventLoop, module=RunnerThreadModule)
 
             self._cancel_async_tasks()
             self._cancel_tasks()
 
-            logger.debug("Terminating the async loop...")
             if self._loop.is_running():
+                logger.debug("Terminating the async loop...")
                 self._loop.stop()
 
+            logger.debug("Closing the async loop...")
             self._loop.close()
 
         self._running = False
 
     def stop(self, timeout: Optional[float] = None):
-        if self._running:
-            self._cancel_async_tasks()
-            self._cancel_tasks()
-            self._loop.stop()
+        self._pipe_emit.send(1)
+        try:
             self.join(timeout)
+        except:
+            logger.debug("Task executor process terminated abruptly")
+        logger.debug("Tasks process terminated")
```

### Comparing `jorun-0.1.4/src/jorun/scanner.py` & `jorun-0.2.0/src/jorun/scanner.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/handler/base.py` & `jorun-0.2.0/src/jorun/handler/base.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/handler/docker.py` & `jorun-0.2.0/src/jorun/handler/docker.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/handler/group.py` & `jorun-0.2.0/src/jorun/handler/group.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/handler/shell.py` & `jorun-0.2.0/src/jorun/handler/shell.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/types/task.py` & `jorun-0.2.0/src/jorun/types/task.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/ui/application.py` & `jorun-0.2.0/src/jorun/ui/application.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/ui/main_window.py` & `jorun-0.2.0/src/jorun/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/ui/pane.py` & `jorun-0.2.0/src/jorun/ui/pane.py`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/src/jorun/ui/task_panel.py` & `jorun-0.2.0/src/jorun/ui/task_panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from logging import LogRecord
 from typing import Optional
 
 from PySide6.QtCore import Slot
 from PySide6.QtWidgets import QGroupBox, QVBoxLayout, QWidget, QPlainTextEdit, QLabel, QLineEdit, QSizePolicy
 from tinyioc import inject
 
@@ -44,15 +45,14 @@
         self._actions_group_widget.setLayout(self._actions_group_layout)
 
         self._layout.addWidget(self._actions_group_widget)
 
         self._task_label = QLabel(self)
         self._task_label.setText(self._task_name)
         self._task_label.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Fixed)
-        self._task_label.setMaximumWidth(80)
         self._task_label.setStyleSheet(f"""
             color: {palette.foreground};
             font-weight: bold;
         """)
         self._actions_group_layout.addWidget(self._task_label)
 
         self._filter_edit_text = QLineEdit(self)
@@ -73,25 +73,31 @@
             font-family: monospace;
         """)
         self._layout.addWidget(self._output_stream_edit_text, 1)
 
     # noinspection PyUnresolvedReferences
     def append_text(self, record: LogRecord):
         scroll_bottom = False
+        previous_scrollbar_pos = self._output_stream_edit_text.verticalScrollBar().value()
 
         if self._output_stream_edit_text.verticalScrollBar().value() > \
                 self._output_stream_edit_text.verticalScrollBar().maximum() - constants.SCROLL_TOLERANCE:
             scroll_bottom = True
 
-        self._output_stream += record.message
+        processed_message = re.sub(r'\x1b\[([0-9,A-Z]{1,2}(;[0-9]{1,2})?(;[0-9]{3})?)?[m|K]?', '', record.message)
+        self._output_stream += processed_message
         self._update_output_edit_text()
 
         if scroll_bottom:
             self._output_stream_edit_text.verticalScrollBar().setValue(
                 self._output_stream_edit_text.verticalScrollBar().maximum())
+        else:
+            self._output_stream_edit_text.verticalScrollBar().setValue(
+                min(self._output_stream_edit_text.verticalScrollBar().maximum(),
+                    max(self._output_stream_edit_text.verticalScrollBar().minimum(), previous_scrollbar_pos)))
 
     def _update_output_edit_text(self):
         filter_input = self._filter_edit_text.text()
 
         if filter_input:
             filtered_text = ""
             for line in self._output_stream.splitlines(keepends=True):
```

### Comparing `jorun-0.1.4/LICENSE` & `jorun-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/README.md` & `jorun-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jorun-0.1.4/pyproject.toml` & `jorun-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jorun"
-version = "0.1.4"
+version = "0.2.0"
 authors = [
   { name="Paolo Infante", email="info@paoloinfante.it" },
 ]
 description = "A customizable task runner"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "PyYAML==6.0",
     "PySide6==6.5.0",
-    "tinyioc==0.1.4"
+    "tinyioc==0.1.4",
+    "psutil==5.9.5"
 ]
 
 [project.scripts]
 jorun = "jorun.main:main"
 
 [project.urls]
 "Homepage" = "https://github.com/paolo-projects/jorun"
```

### Comparing `jorun-0.1.4/PKG-INFO` & `jorun-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: jorun
-Version: 0.1.4
+Version: 0.2.0
 Summary: A customizable task runner
 Project-URL: Homepage, https://github.com/paolo-projects/jorun
 Project-URL: Bug Tracker, https://github.com/paolo-projects/jorun/issues
 Author-email: Paolo Infante <info@paoloinfante.it>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: psutil==5.9.5
 Requires-Dist: pyside6==6.5.0
 Requires-Dist: pyyaml==6.0
 Requires-Dist: tinyioc==0.1.4
 Description-Content-Type: text/markdown
 
 # Jorun
```

