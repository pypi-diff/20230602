# Comparing `tmp/resotoshell-3.5.0.tar.gz` & `tmp/resotoshell-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotoshell-3.5.0.tar", last modified: Fri May 26 18:25:25 2023, max compression
+gzip compressed data, was "resotoshell-3.5.1.tar", last modified: Fri Jun  2 14:54:04 2023, max compression
```

## Comparing `resotoshell-3.5.0.tar` & `resotoshell-3.5.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:43.000000 resotoshell-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-26 18:25:25.456874 resotoshell-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-26 18:21:43.000000 resotoshell-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 18:21:43.000000 resotoshell-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.452874 resotoshell-3.5.0/resotoshell/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35784 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-05-26 18:21:43.000000 resotoshell-3.5.0/resotoshell/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/resotoshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 18:25:25.000000 resotoshell-3.5.0/resotoshell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 18:25:25.456874 resotoshell-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-26 18:21:43.000000 resotoshell-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:25:25.456874 resotoshell-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-26 18:21:43.000000 resotoshell-3.5.0/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:50:19.000000 resotoshell-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-02 14:54:04.172063 resotoshell-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-02 14:50:19.000000 resotoshell-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-02 14:50:19.000000 resotoshell-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/resotoshell/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9557 2023-06-02 14:50:19.000000 resotoshell-3.5.1/resotoshell/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/resotoshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:26.000000 resotoshell-3.5.1/resotoshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:54:04.000000 resotoshell-3.5.1/resotoshell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 14:54:04.172063 resotoshell-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:54:04.172063 resotoshell-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-02 14:50:19.000000 resotoshell-3.5.1/test/test_protected_files.py
```

### Comparing `resotoshell-3.5.0/PKG-INFO` & `resotoshell-3.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.0
+Version: 3.5.1
 Summary: Commandline interpreter to interact with Resoto.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
-License: Apache 2.0
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # `resh`
 Resoto Shell
 
 
 ## Table of contents
```

### Comparing `resotoshell-3.5.0/README.md` & `resotoshell-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.0/resotoshell/__main__.py` & `resotoshell-3.5.1/resotoshell/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import resotolib.proc
 from resotolib.args import ArgumentParser
 from resotolib.core import resotocore, add_args as core_add_args, wait_for_resotocore
 from resotolib.core.ca import TLSData
 from resotolib.jwt import add_args as jwt_add_args
 from resotolib.logger import log, setup_logger, add_args as logging_add_args
 from resotoshell import authorized_client
-from resotoshell.promptsession import PromptSession, core_metadata
+from resotoshell.promptsession import PromptSession, core_metadata, ResotoHistory
 from resotoshell.shell import Shell, ShutdownShellError
 
 
 async def main_async() -> None:
     resotolib.proc.parent_pid = os.getpid()
     setup_logger("resotoshell", json_format=False)
     arg_parser = ArgumentParser(description="resoto shell", env_args_prefix="RESOTOSHELL_")
@@ -55,33 +55,33 @@
     except Exception:
         await client.shutdown()
         sys.exit(1)
     if args.stdin or not sys.stdin.isatty():
         await handle_from_stdin(client)
     else:
         cmds, kinds, props = await core_metadata(client)
-        session = PromptSession(cmds=cmds, kinds=kinds, props=props)
-        await repl(client, args, session)
+        history = ResotoHistory.default()
+        session = PromptSession(cmds=cmds, kinds=kinds, props=props, history=history)
+        shell = Shell(client, True, detect_color_system(args), history=history)
+        await repl(shell, session, args)
 
     # update the eventually changed auth token
     await authorized_client.update_auth_header(client)
     await client.shutdown()
 
 
-async def repl(client: ResotoClient, args: Namespace, session: PromptSession) -> None:
+async def repl(shell: Shell, session: PromptSession, args: Namespace) -> None:
     shutdown_event = Event()
-    shell = Shell(client, True, detect_color_system(args))
+
     log.debug("Starting interactive session")
 
     # send the welcome command to the core
-    await shell.handle_command("welcome")
+    await shell.handle_command("welcome", no_history=True)
 
-    event_listener = (
-        None if args.no_events else asyncio.create_task(attach_to_event_stream(client, shell, shutdown_event))
-    )
+    event_listener = None if args.no_events else asyncio.create_task(attach_to_event_stream(shell, shutdown_event))
     try:
         while not shutdown_event.is_set():
             try:
                 await asyncio.sleep(0.1)
                 command = await session.prompt()
                 if command == "":
                     continue
@@ -98,18 +98,18 @@
             except Exception:
                 log.exception("Caught unhandled exception while processing CLI command")
     finally:
         if event_listener:
             event_listener.cancel()
 
 
-async def attach_to_event_stream(client: ResotoClient, shell: Shell, shutdown_event: Event) -> None:
+async def attach_to_event_stream(shell: Shell, shutdown_event: Event) -> None:
     while not shutdown_event.is_set():
         try:
-            async for event in client.events({"error"}):
+            async for event in shell.client.events({"error"}):
                 data = event.get("data", {})
                 message = data.get("message")
                 context = ",".join([f"{k}={v}" for k, v in data.items() if k != "message"])
                 if message:
                     shell.stderr(
                         FormattedText(
                             [
```

### Comparing `resotoshell-3.5.0/resotoshell/authorized_client.py` & `resotoshell-3.5.1/resotoshell/authorized_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             if decoded.get("exp", 0) > time.time():
                 return method, jwt_token
         return None
 
     def write(self) -> None:
         if self.dirty:
             self.path.parent.mkdir(mode=0o700, parents=True, exist_ok=True)
-            with open(os.open(self.path, os.O_CREAT | os.O_WRONLY, 0o600), "w+") as f:
+            with open(os.open(self.path, os.O_CREAT | os.O_WRONLY, 0o600), "w+", encoding="utf-8") as f:
                 self.config.write(f)
 
     @staticmethod
     def default() -> ReshConfig:
         return ReshConfig(Path.home() / ".resoto" / "resh.ini")
```

### Comparing `resotoshell-3.5.0/resotoshell/promptsession.py` & `resotoshell-3.5.1/resotoshell/promptsession.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
+from __future__ import annotations
 import pathlib
 import re
+import shutil
 from abc import ABC
-
-from attr import evolve
-from attrs import define, field
 from re import Pattern
-from math import floor
 from shutil import get_terminal_size
 from typing import Iterable, Optional, List, Dict, Union, Tuple, Callable, Any
 
 import jsons
+from attr import evolve
+from attrs import define, field
+from math import floor
 from prompt_toolkit import PromptSession as PTSession
 from prompt_toolkit.auto_suggest import AutoSuggestFromHistory
 from prompt_toolkit.completion import (
     Completer,
     CompleteEvent,
     Completion,
     WordCompleter,
     NestedCompleter,
     merge_completers,
     PathCompleter,
     FuzzyCompleter,
 )
 from prompt_toolkit.document import Document
-from prompt_toolkit.history import FileHistory
+from prompt_toolkit.history import FileHistory, History
 from prompt_toolkit.styles import Style
 from resotoclient.async_client import ResotoClient
 from resotoclient.models import Property
 
 from resotolib.logger import log
 
 
@@ -721,33 +722,55 @@
             result = self.completer.get_completions(document, complete_event)
             return [] if result is None else result
         except Exception as ex:
             log.warning(f"Error in completer: {ex}", exc_info=ex)
             return []
 
 
+class ResotoHistory(History):
+    def __init__(self, history_file: str) -> None:
+        super().__init__()
+        self.file_history = FileHistory(history_file)
+
+    def load_history_strings(self) -> Iterable[str]:
+        return self.file_history.load_history_strings()
+
+    def store_string(self, string: str) -> None:
+        # called by prompt_toolkit - ignore this call.
+        # we store the string in the store_command method which is called from Shell
+        pass
+
+    def store_command(self, string: str) -> None:
+        self.file_history.store_string(string)
+
+    @staticmethod
+    def default() -> ResotoHistory:
+        # this path existed until 3.5.0
+        old_path = pathlib.Path.home() / ".resotoshell_history"
+        path = pathlib.Path.home() / ".resoto" / "shell_history"
+        # make sure the directory exists
+        path.parent.mkdir(mode=0o700, parents=True, exist_ok=True)
+        # move the old history file to the new location
+        if old_path.exists() and not path.exists():
+            shutil.move(str(old_path), str(path))
+        return ResotoHistory(str(path))
+
+
 class PromptSession:
     style = Style.from_dict(
         {
             "green": "#00ff00",
             "red": "#ff0000",
             "prompt": "#C724B1",
         }
     )
 
     prompt_message = [("class:prompt", "> ")]
 
-    def __init__(
-        self,
-        cmds: List[CommandInfo],
-        kinds: List[str],
-        props: List[str],
-        history_file: str = str(pathlib.Path.home() / ".resotoshell_history"),
-    ):
-        history = FileHistory(history_file)
+    def __init__(self, cmds: List[CommandInfo], kinds: List[str], props: List[str], history: History):
         _, tty_rows = get_terminal_size(fallback=(80, 25))
         reserved_row_ratio = 1 / 4
         min_reserved_rows = 4
         max_reserved_rows = 12
         reserved_space_for_menu = max(min_reserved_rows, min(floor(tty_rows * reserved_row_ratio), max_reserved_rows))
         self.completer = CommandLineCompleter.create_completer(cmds, kinds, props)
         self.session: PTSession[str] = PTSession(history=history, reserve_space_for_menu=reserved_space_for_menu)
```

### Comparing `resotoshell-3.5.0/resotoshell/protected_files.py` & `resotoshell-3.5.1/resotoshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.0/resotoshell/shell.py` & `resotoshell-3.5.1/resotoshell/shell.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.output import ColorDepth
 from resotoclient.async_client import HttpResponse
 from resotoclient.async_client import ResotoClient
 from rich.markdown import Markdown
 
 from resotolib.args import ArgumentParser
+from resotolib.core import CLIEnvelope
 from resotolib.logger import log
 from resotolib.utils import sha256sum
+from resotoshell.promptsession import ResotoHistory
 from resotoshell.protected_files import validate_paths
 
 color_system_to_color_depth = {
     "monochrome": ColorDepth.DEPTH_1_BIT,
     "standard": ColorDepth.DEPTH_8_BIT,
     "eight_bit": ColorDepth.DEPTH_8_BIT,
     "truecolor": ColorDepth.DEPTH_24_BIT,
@@ -36,29 +38,33 @@
 
 class Shell:
     def __init__(
         self,
         client: ResotoClient,
         tty: bool,
         color_system: str,
+        *,
         graph: Optional[str] = None,
         section: Optional[str] = None,
+        history: Optional[ResotoHistory] = None,
     ):
         self.client = client
+        self.history = history
         self.tty = tty
         self.color_system = color_system
         self.color_depth = color_system_to_color_depth.get(color_system) or ColorDepth.DEPTH_8_BIT
         self.graph = graph
         self.section = section
 
     async def handle_command(
         self,
         command: str,
         additional_headers: Optional[Dict[str, str]] = None,
         files: Optional[Dict[str, str]] = None,
+        no_history: bool = False,
     ) -> None:
         headers: Dict[str, str] = {}
         headers.update({"Accept": "text/plain"})
         headers.update(additional_headers or {})
 
         # set tty headers
         if self.tty:
@@ -73,14 +79,17 @@
                 }
             )
 
         async def handle_response(maybe: Optional[HttpResponse], upload: bool = False) -> None:
             if maybe is not None:
                 with maybe as response:
                     if response.status_code == 200:
+                        # only store history if the command was successful, and no no_history flag was set
+                        if self.history and not no_history and CLIEnvelope.no_history not in response.headers:
+                            self.history.store_command(command)
                         await self.handle_result(response)
                     elif response.status_code == 424 and not upload:
                         js_data = await response.json()
                         required = js_data.get("required", [])
                         to_upload = validate_paths({fp["name"]: fp["path"] for fp in required})
                         mp: HttpResponse = await self.client.cli_execute_raw(
                             command=command,
@@ -137,16 +146,16 @@
                     content = await response.payload_bytes()
                 else:
                     content = await response.read()
                 fh.write(content)
             return filename, filepath
 
         content_type = response.headers.get("Content-Type", "text/plain")
-        action = response.headers.get("Resoto-Shell-Action")
-        command = response.headers.get("Resoto-Shell-Command")
+        action = response.headers.get(CLIEnvelope.action)
+        command = response.headers.get(CLIEnvelope.command)
         line_delimiter = "---"
 
         # If we get a plain text result, we simply print it to the console.
         if content_type == "text/plain":
             # Received plain text: print it.
             if not first:
                 self.stdout(line_delimiter)
```

### Comparing `resotoshell-3.5.0/resotoshell.egg-info/PKG-INFO` & `resotoshell-3.5.1/resotoshell.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: resotoshell
-Version: 3.5.0
+Version: 3.5.1
 Summary: Commandline interpreter to interact with Resoto.
-Home-page: https://github.com/someengineering/resoto/tree/main/resotoshell
-License: Apache 2.0
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/resotoshell
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # `resh`
 Resoto Shell
 
 
 ## Table of contents
```

### Comparing `resotoshell-3.5.0/resotoshell.egg-info/SOURCES.txt` & `resotoshell-3.5.1/resotoshell.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resotoshell/__init__.py
 resotoshell/__main__.py
 resotoshell/authorized_client.py
 resotoshell/promptsession.py
 resotoshell/protected_files.py
 resotoshell/shell.py
 resotoshell.egg-info/PKG-INFO
```

### Comparing `resotoshell-3.5.0/test/test_promptsession.py` & `resotoshell-3.5.1/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `resotoshell-3.5.0/test/test_protected_files.py` & `resotoshell-3.5.1/test/test_protected_files.py`

 * *Files identical despite different names*

