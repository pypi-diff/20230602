# Comparing `tmp/viv-23.5a4.tar.gz` & `tmp/viv-23.5a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv-23.5a4.tar", last modified: Mon May 29 17:52:49 2023, max compression
+gzip compressed data, was "viv-23.5a5.tar", last modified: Fri Jun  2 19:10:02 2023, max compression
```

## Comparing `viv-23.5a4.tar` & `viv-23.5a5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2022-12-26 14:03:58.055665 viv-23.5a4/LICENSE
--rw-r--r--   0        0        0     3928 2023-05-29 17:46:35.595217 viv-23.5a4/README.md
--rw-r--r--   0        0        0      813 2023-05-29 17:43:32.762971 viv-23.5a4/pyproject.toml
--rw-r--r--   0        0        0       48 2023-05-28 22:22:55.204851 viv-23.5a4/src/viv/__init__.py
--rw-r--r--   0        0        0       61 2023-02-03 19:40:10.351352 viv-23.5a4/src/viv/__main__.py
--rwxr-xr-x   0        0        0    48457 2023-05-29 17:52:27.622335 viv-23.5a4/src/viv/viv.py
--rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 viv-23.5a4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.5a5/LICENSE
+-rw-r--r--   0        0        0     3666 2023-06-02 19:09:37.319887 viv-23.5a5/README.md
+-rw-r--r--   0        0        0      844 2023-06-02 13:44:22.533515 viv-23.5a5/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.5a5/src/viv/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.5a5/src/viv/__main__.py
+-rwxr-xr-x   0        0        0    48724 2023-06-02 19:09:50.793343 viv-23.5a5/src/viv/viv.py
+-rw-r--r--   0        0        0     3990 1970-01-01 00:00:00.000000 viv-23.5a5/PKG-INFO
```

### Comparing `viv-23.5a4/LICENSE` & `viv-23.5a5/LICENSE`

 * *Files identical despite different names*

### Comparing `viv-23.5a4/README.md` & `viv-23.5a5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,67 @@
-# viv
+Metadata-Version: 2.1
+Name: viv
+Version: 23.5a5
+Summary: viv isn't venv
+License: MIT
+Author-email: Daylin Morgan <daylinmorgan@gmail.com>
+Requires-Python: >= 3.8
+Project-URL: homepage, https://github.com/daylinmorgan/viv
+Project-URL: repository, https://github.com/daylinmorgan/viv
+Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://github.com/daylinmorgan/viv">
     <img src="https://raw.githubusercontent.com/daylinmorgan/viv/main/assets/logo.svg" alt="Logo" width=500 >
   </a>
   <p align="center">
-  viv isn't venv
+  <h1> viv isn't venv </h1>
+  </p>
+  <div align="center">
+    <img
+      src="https://raw.githubusercontent.com/daylinmorgan/viv/main/docs/svgs/viv-help.svg"
+      alt="cli screenshot"
+      width="500"
+      >
+  </div>
+  <p align="center">
+    <a href="https://viv.dayl.in">Documentation</a>
   </p>
 </div>
 
+Try before you buy!
+```sh
+python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay -- "viv isn't venv\!"
+```
 ---
 
 `Viv` is a standalone dependency-free `venv` creator.
 
-These `venvs` can be identified by name or by their specification.
-In any case they will be re-used across scripts (and generated on-demand, if needed).
+`Viv`'s uncompromising insistence on portability means that it will always:
 
-**Importantly**, `viv` will also remove your user site directory.
-(view with: `python -m 'import site;print(site.USER_SITE)'`).
-
-`Viv`'s uncompromising insistence on portability means that it will always (1) only use the standard library (2) never exceed a single script.
+1. only use the standard library
+2. never exceed a single script.
 
 For that reason any usage of the `CLI` can be accomplished using a remote copy as seen in the below install command.
 
 ## Setup
 
 Run the below command to install `viv`.
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage install
+python3 <(curl -fsSL viv.dayl.in/viv.py) manage install
 ```
 
 To access `viv` from within scripts you should add it's location to your `PYTHONPATH`.
 By default `viv` will be installed to `$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can customize this with `--src`.
 
 ```sh
 export PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv"
 ```
 
-Advanced users may recognize that principally,
-the module just needs to be recognized at run time
-and the single script [`viv.py`](https://github.com/daylinmorgan/viv/blob/main/src/viv/viv.py) can be invoked directly for the CLI.
-How you accomplish these options is ultimately up to you but the above instructions can get you started.
-
 ### Pypi (Not Recommended)
 
 ```sh
 pip install viv
 ```
 
 Why is this *not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
@@ -66,28 +81,28 @@
 ```sh
 viv remove $(viv list -q)
 ```
 
 To remove `viv` all together you can use the included `purge` command:
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage purge
+python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge
 ```
 
 ## Additional Features
 
 An experimental feature of `viv` is generating shim's that leverage the principles of `viv`.
 These shims would operate similar to `pipx` in which you can specify a command line app to "install".
 
-*Note* that `--standalone` will auto-generate a code-golfed minified version of `viv` to accomplish the same basic task as using a local copy of `viv`.
-After generating this a standalone `shim` you can freely use this script across unix machines which have `python>3.8`.
+*Note* that `--standalone` will auto-generate a mini function version of `viv` to accomplish the same basic task as using a local copy of `viv`.
+After generating this standalone `shim` you can freely use this script across unix machines which have `python>3.8`.
 See [examples/black](https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of below command.
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) shim black -o ./black --standalone --freeze
+python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze
 ```
 
 ## Alternatives
 
 ### [pip-run](https://github.com/jaraco/pip-run)
 
 ```sh
@@ -117,7 +132,8 @@
 ```sh
 pipx (1.1.0)
 ├── argcomplete>=1.9.4 (2.1.1)
 ├── packaging>=20.0 (23.0)
 └── userpath>=1.6.0 (1.8.0)
     └── click (8.1.3)
 ```
+
```

#### html2text {}

```diff
@@ -1,51 +1,50 @@
-# viv
+Metadata-Version: 2.1 Name: viv Version: 23.5a5 Summary: viv isn't venv
+License: MIT Author-email: Daylin Morgan
+gmail.com> Requires-Python: >= 3.8 Project-URL: homepage, https://github.com/
+daylinmorgan/viv Project-URL: repository, https://github.com/daylinmorgan/viv
+Description-Content-Type: text/markdown
                                     [Logo]
-                                viv isn't venv
---- `Viv` is a standalone dependency-free `venv` creator. These `venvs` can be
-identified by name or by their specification. In any case they will be re-used
-across scripts (and generated on-demand, if needed). **Importantly**, `viv`
-will also remove your user site directory. (view with: `python -m 'import
-site;print(site.USER_SITE)'`). `Viv`'s uncompromising insistence on portability
-means that it will always (1) only use the standard library (2) never exceed a
-single script. For that reason any usage of the `CLI` can be accomplished using
-a remote copy as seen in the below install command. ## Setup Run the below
-command to install `viv`. ```sh python3 <(curl -fsSL gh.dayl.in/viv/viv.py)
-manage install ``` To access `viv` from within scripts you should add it's
-location to your `PYTHONPATH`. By default `viv` will be installed to
-`$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can customize this with `--
-src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` Advanced
-users may recognize that principally, the module just needs to be recognized at
-run time and the single script [`viv.py`](https://github.com/daylinmorgan/viv/
-blob/main/src/viv/viv.py) can be invoked directly for the CLI. How you
-accomplish these options is ultimately up to you but the above instructions can
-get you started. ### Pypi (Not Recommended) ```sh pip install viv ``` Why is
-this *not recommended*? Mainly, because `viv` is all about hacking your
-`sys.path`. Placing it in it's own virtual environment or installing in a user
-site directory may complicate this endeavor. ## Usage In any python script with
-external dependencies you can add this line, to automate `vivenv` creation and
-installation of dependencies. ```python __import__("viv").use("click") ``` To
-remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
--q) ``` To remove `viv` all together you can use the included `purge` command:
-```sh python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage purge ``` ##
-Additional Features An experimental feature of `viv` is generating shim's that
-leverage the principles of `viv`. These shims would operate similar to `pipx`
-in which you can specify a command line app to "install". *Note* that `--
-standalone` will auto-generate a code-golfed minified version of `viv` to
-accomplish the same basic task as using a local copy of `viv`. After generating
-this a standalone `shim` you can freely use this script across unix machines
-which have `python>3.8`. See [examples/black](https://github.com/daylinmorgan/
-viv/blob/dev/examples/black) for output of below command. ```sh python3 <(curl
--fsSL gh.dayl.in/viv/viv.py) shim black -o ./black --standalone --freeze ``` ##
-Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
-(10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
-âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
-âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
-inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
-typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
-âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
-âââ more-itertools (9.1.0) âââ more-itertools>=8.3 (9.1.0)
-âââ packaging (23.0) âââ path>=15.1 (16.6.0) âââ pip>=19.3
-(23.0.1) âââ platformdirs (3.1.0) ``` ### [pipx](https://github.com/pypa/
-pipx/) ```sh pipx (1.1.0) âââ argcomplete>=1.9.4 (2.1.1) âââ
-packaging>=20.0 (23.0) âââ userpath>=1.6.0 (1.8.0) âââ click
-(8.1.3) ```
+                         ****** viv isn't venv ******
+                               [cli screenshot]
+                                 Documentation
+Try before you buy! ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay
+-- "viv isn't venv\!" ``` --- `Viv` is a standalone dependency-free `venv`
+creator. `Viv`'s uncompromising insistence on portability means that it will
+always: 1. only use the standard library 2. never exceed a single script. For
+that reason any usage of the `CLI` can be accomplished using a remote copy as
+seen in the below install command. ## Setup Run the below command to install
+`viv`. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage install ``` To
+access `viv` from within scripts you should add it's location to your
+`PYTHONPATH`. By default `viv` will be installed to `$XDG_DATA_HOME/viv` or
+`~/.local/share/viv` you can customize this with `--src`. ```sh export
+PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` ### Pypi (Not Recommended)
+```sh pip install viv ``` Why is this *not recommended*? Mainly, because `viv`
+is all about hacking your `sys.path`. Placing it in it's own virtual
+environment or installing in a user site directory may complicate this
+endeavor. ## Usage In any python script with external dependencies you can add
+this line, to automate `vivenv` creation and installation of dependencies.
+```python __import__("viv").use("click") ``` To remove all `vivenvs` you can
+use the below command: ```sh viv remove $(viv list -q) ``` To remove `viv` all
+together you can use the included `purge` command: ```sh python3 <(curl -fsSL
+viv.dayl.in/viv.py) manage purge ``` ## Additional Features An experimental
+feature of `viv` is generating shim's that leverage the principles of `viv`.
+These shims would operate similar to `pipx` in which you can specify a command
+line app to "install". *Note* that `--standalone` will auto-generate a mini
+function version of `viv` to accomplish the same basic task as using a local
+copy of `viv`. After generating this standalone `shim` you can freely use this
+script across unix machines which have `python>3.8`. See [examples/black]
+(https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of
+below command. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./
+black --standalone --freeze ``` ## Alternatives ### [pip-run](https://
+github.com/jaraco/pip-run) ```sh pip-run (10.0.5) âââ autocommand (2.2.2)
+âââ jaraco-context (4.3.0) âââ jaraco-functools (3.6.0) â
+âââ more-itertools (9.1.0) âââ jaraco-text (3.11.1) â âââ
+autocommand (2.2.2) â âââ inflect (6.0.2) â â âââ
+pydantic>=1.9.1 (1.10.5) â â âââ typing-extensions>=4.2.0 (4.5.0) â
+âââ jaraco-context>=4.1 (4.3.0) â âââ jaraco-functools (3.6.0)
+â â âââ more-itertools (9.1.0) â âââ more-itertools (9.1.0)
+âââ more-itertools>=8.3 (9.1.0) âââ packaging (23.0) âââ
+path>=15.1 (16.6.0) âââ pip>=19.3 (23.0.1) âââ platformdirs (3.1.0)
+``` ### [pipx](https://github.com/pypa/pipx/) ```sh pipx (1.1.0) âââ
+argcomplete>=1.9.4 (2.1.1) âââ packaging>=20.0 (23.0) âââ
+userpath>=1.6.0 (1.8.0) âââ click (8.1.3) ```
```

### Comparing `viv-23.5a4/pyproject.toml` & `viv-23.5a5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 authors = [
     { name = "Daylin Morgan", email = "daylinmorgan@gmail.com" },
 ]
 dependencies = []
 requires-python = ">= 3.8"
 readme = "README.md"
 dynamic = []
-version = "23.5a4"
+version = "23.5a5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/daylinmorgan/viv"
 repository = "https://github.com/daylinmorgan/viv"
@@ -29,14 +29,15 @@
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pre-commit>=3",
     "mypy>=0.991",
+    "mkdocs-material>=9.1.15",
 ]
 
 [tool.ruff]
 select = [
     "E",
     "F",
     "I",
```

### Comparing `viv-23.5a4/src/viv/viv.py` & `viv-23.5a5/src/viv/viv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
-"""Viv isn't venv!
+"""viv isn't venv!
 
   viv -h
     OR
   __import__("viv").use("requests", "bs4")
 """
 
 from __future__ import annotations
 
 import hashlib
+import inspect
 import itertools
 import json
 import os
 import re
-import shlex
 import shutil
 import site
 import subprocess
 import sys
 import tempfile
 import threading
 import time
@@ -29,69 +29,32 @@
     Namespace,
     RawDescriptionHelpFormatter,
     _SubParsersAction,
 )
 from argparse import ArgumentParser as StdArgParser
 from dataclasses import dataclass
 from datetime import datetime
-from itertools import zip_longest
 from pathlib import Path
-from textwrap import dedent, fill, wrap
+from textwrap import dedent, fill
 from types import TracebackType
 from typing import (
     Any,
     Dict,
-    Generator,
     List,
     NoReturn,
     Optional,
     Sequence,
     TextIO,
     Tuple,
     Type,
 )
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
-__version__ = "23.5a4"
-
-
-class Config:
-    """viv config manager"""
-
-    def __init__(self) -> None:
-        self._cache = Path(os.getenv("XDG_CACHE_HOME", Path.home() / ".cache")) / "viv"
-
-    def _ensure(self, p: Path) -> Path:
-        p.mkdir(parents=True, exist_ok=True)
-        return p
-
-    @property
-    def venvcache(self) -> Path:
-        return self._ensure(self._cache / "venvs")
-
-    @property
-    def srccache(self) -> Path:
-        return self._ensure(self._cache / "src")
-
-    @property
-    def binparent(self) -> Path:
-        return self._ensure(
-            Path(os.getenv("VIV_BIN_DIR", Path.home() / ".local" / "bin"))
-        )
-
-    @property
-    def srcdefault(self) -> Path:
-        parent = (
-            Path(os.getenv("XDG_DATA_HOME", Path.home() / ".local" / "share")) / "viv"
-        )
-        return self._ensure(parent) / "viv.py"
-
-
-c = Config()
+__version__ = "23.5a5"
 
 
 class Spinner:
     """spinner modified from:
     https://raw.githubusercontent.com/Tagar/stuff/master/spinner.py
     """
 
@@ -143,45 +106,33 @@
         if sys.stderr.isatty():
             self.busy = False
             self.remove_spinner(cleanup=True)
         else:
             sys.stderr.write("\r")
 
 
-BOX: Dict[str, str] = {
-    "v": "│",
-    "h": "─",
-    "tl": "╭",
-    "tr": "╮",
-    "bl": "╰",
-    "br": "╯",
-    "sep": "┆",
-}
-
-
-@dataclass
 class Ansi:
     """control ouptut of ansi(VT100) control codes"""
 
-    bold: str = "\033[1m"
-    dim: str = "\033[2m"
-    underline: str = "\033[4m"
-    red: str = "\033[1;31m"
-    green: str = "\033[1;32m"
-    yellow: str = "\033[1;33m"
-    magenta: str = "\033[1;35m"
-    cyan: str = "\033[1;36m"
-    end: str = "\033[0m"
-
-    # for argparse help
-    header: str = cyan
-    option: str = yellow
-    metavar: str = "\033[33m"  # normal yellow
+    def __init__(self) -> None:
+        self.bold: str = "\033[1m"
+        self.dim: str = "\033[2m"
+        self.underline: str = "\033[4m"
+        self.red: str = "\033[1;31m"
+        self.green: str = "\033[1;32m"
+        self.yellow: str = "\033[1;33m"
+        self.magenta: str = "\033[1;35m"
+        self.cyan: str = "\033[1;36m"
+        self.end: str = "\033[0m"
+
+        # for argparse help
+        self.header: str = self.cyan
+        self.option: str = self.yellow
+        self.metavar: str = "\033[33m"  # normal yellow
 
-    def __post_init__(self) -> None:
         if os.getenv("NO_COLOR") or not sys.stderr.isatty():
             for attr in self.__dict__:
                 setattr(self, attr, "")
 
         self._ansi_escape = re.compile(
             r"""
             \x1B  # ESC
@@ -212,109 +163,210 @@
 
     def tagline(self) -> str:
         """generate the viv tagline!"""
 
         return " ".join(
             (
                 self.style(f, "magenta") + self.style(rest, "cyan")
-                for f, rest in (("V", "iv"), ("i", "sn't"), ("v", "env!"))
+                for f, rest in (("v", "iv"), ("i", "sn't"), ("v", "env!"))
             )
         )
 
-    def subprocess(self, output: str) -> None:
+    def subprocess(self, command: List[str], output: str) -> None:
         """generate output for subprocess error
 
         Args:
             output: text output from subprocess, usually from p.stdout
         """
         if not output:
             return
-        echo("subprocess output:")
+
+        error("subprocess failed")
+        echo("see below for command output", style="red")
+        echo(f"cmd:\n  {' '.join(command)}", style="red")
         new_output = [f"{self.red}->{self.end} {line}" for line in output.splitlines()]
-        sys.stdout.write("\n".join(new_output) + "\n")
+        echo("subprocess output:" + "\n".join(("", *new_output, "")), style="red")
 
-    def _get_column_sizes(
-        self, rows: Tuple[Tuple[str, Sequence[str]], ...]
-    ) -> List[int]:
-        """convert list of rows to list of columns sizes
+    def viv_preamble(self, style: str = "magenta", sep: str = "::") -> str:
+        return f"{self.cyan}viv{self.end}{self.__dict__[style]}{sep}{self.end}"
 
-        First convert rows into list of columns,
-        then get max string length for each column.
-        """
-        return list(max(map(len, lst)) for lst in map(list, zip(*rows)))  # type: ignore
 
-    def _make_row(self, row: Generator[Any, None, None]) -> str:
-        return f"  {BOX['v']} " + f" {BOX['sep']} ".join(row) + f" {BOX['v']}"
+a = Ansi()
 
-    def _sanitize_row(
-        self, sizes: List[int], row: Tuple[str, Sequence[str]]
-    ) -> Tuple[Tuple[str, Sequence[str]], ...]:
-        if len(row[1]) > sizes[1]:
-            return tuple(
-                zip_longest(
-                    (row[0],),
-                    wrap(str(row[1]), break_on_hyphens=False, width=sizes[1]),
-                    fillvalue="",
-                )
-            )
+
+class Template:
+    description = f"""
+
+{a.tagline()}
+to create/activate a vivenv:
+- from command line: `{a.style("viv -h","bold")}`
+- within python script: {a.style('__import__("viv").use("typer", "rich-click")','bold')}
+"""
+
+    _standalone_func = r"""def _viv_use(*pkgs, track_exe=False, name=""):
+    import hashlib, json, os, site, shutil, sys, venv  # noqa
+    from pathlib import Path  # noqa
+    from datetime import datetime  # noqa
+    from subprocess import run  # noqa
+
+    if not {*map(type, pkgs)} == {str}:
+        raise ValueError(f"spec: {pkgs} is invalid")
+
+    meta = dict.fromkeys(("created", "accessed"), (t := str(datetime.today())))
+    runner = str(Path(__file__).absolute().resolve())
+    force, verbose, xdg = map(os.getenv, ("VIV_FORCE", "VIV_VERBOSE", "XDG_CACHE_HOME"))
+    cache = (Path(xdg) if xdg else Path.home() / ".cache") / "viv" / "venvs"
+    cache.mkdir(parents=True, exist_ok=True)
+    exe = str(Path(sys.executable).resolve()) if track_exe else "N/A"
+    (sha256 := hashlib.sha256()).update((str(spec := [*pkgs]) + exe).encode())
+    _id = sha256.hexdigest()
+    if (env := cache / (name if name else _id)) not in cache.glob("*/") or force:
+        sys.stderr.write(f"generating new vivenv -> {env.name}\n")
+        venv.create(env, symlinks=True, with_pip=True, clear=True)
+        (env / "pip.conf").write_text("[global]\ndisable-pip-version-check=true")
+        run_kw = dict(zip(("stdout", "stderr"), ((None,) * 2 if verbose else (-1, 2))))
+        p = run([env / "bin" / "pip", "install", "--force-reinstall", *spec], **run_kw)
+        if (rc := p.returncode) != 0:
+            if env.is_dir():
+                shutil.rmtree(env)
+            sys.stderr.write(f"pip had non zero exit ({rc})\n{p.stdout.decode()}\n")
+            sys.exit(rc)
+        meta.update(dict(id=_id, spec=spec, exe=exe, name=name, files=[runner]))
+    else:
+        meta = json.loads((env / "vivmeta.json").read_text())
+        meta.update(dict(accessed=t, files=sorted({*meta["files"],runner})))
+
+    (env / "vivmeta.json").write_text(json.dumps(meta))
+    sys.path = [p for p in sys.path if not p != site.USER_SITE]
+    site.addsitedir(str(*(env / "lib").glob("py*/si*")))
+    return env
+"""
+
+    def noqa(self, txt: str) -> str:
+        max_length = max(map(len, txt.splitlines()))
+        return "\n".join((f"{line:{max_length}} # noqa" for line in txt.splitlines()))
+
+    def _use_str(self, spec: List[str], standalone: bool = False) -> str:
+        spec_str = ", ".join(f'"{req}"' for req in spec)
+        if standalone:
+            return f"""_viv_use({fill(spec_str,width=90,subsequent_indent="    ",)})"""
         else:
-            return (row,)
+            return f"""__import__("viv").use({spec_str})"""
 
-    def viv_preamble(self, style: str = "magenta", sep: str = "::") -> str:
-        return f"{self.cyan}Viv{self.end}{self.__dict__[style]}{sep}{self.end}"
+    def standalone(self, spec: List[str]) -> str:
+        func_use = "\n".join(
+            (self._standalone_func, self.noqa(self._use_str(spec, standalone=True)))
+        )
+        return f"""
+# AUTOGENERATED by viv (v{__version__})
+# see `python3 <(curl -fsSL viv.dayl.in/viv.py) --help`
+{func_use}
+"""
 
-    def table(
-        self, rows: Tuple[Tuple[str, Sequence[str]], ...], header_style: str = "cyan"
-    ) -> None:
-        """generate a table with outline and styled header assumes two columns
+    def _rel_import(self, local_source: Optional[Path]) -> str:
+        if not local_source:
+            raise ValueError("local source must exist")
+
+        path_to_viv = path_to_viv = str(
+            local_source.resolve().absolute().parent.parent
+        ).replace(str(Path.home()), "~")
+        return (
+            """__import__("sys").path.append(__import__("os")"""
+            f""".path.expanduser("{path_to_viv}"))  # noqa"""
+        )
+
+    def _absolute_import(self, local_source: Optional[Path]) -> str:
+        if not local_source:
+            raise ValueError("local source must exist")
+
+        path_to_viv = local_source.resolve().absolute().parent.parent
+        return f"""__import__("sys").path.append("{path_to_viv}")  # noqa"""
+
+    def frozen_import(
+        self, path: str, local_source: Optional[Path], spec: List[str]
+    ) -> str:
+        if path == "abs":
+            imports = self._absolute_import(local_source)
+        elif path == "rel":
+            imports = self._rel_import(local_source)
+        else:
+            imports = ""
+        return f"""\
+{imports}
+{self.noqa(self._use_str(spec))}
+"""
 
-        Args:
-            rows: sequence of the rows, first item assumed to be header
-            header_style: color/style for header row
-        """
+    def shim(
+        self,
+        path: str,
+        local_source: Optional[Path],
+        standalone: bool,
+        spec: List[str],
+        bin: str,
+    ) -> str:
+        if standalone:
+            imports = self._standalone_func
+        elif path == "abs":
+            imports = self._absolute_import(local_source)
+        elif path == "rel":
+            imports = self._rel_import(local_source)
+        else:
+            imports = ""
+        return f"""\
+#!/usr/bin/env python
+# AUTOGENERATED by viv (v{__version__})
+# see `python3 <(curl -fsSL viv.dayl.in/viv.py) --help`
 
-        sizes = self._get_column_sizes(rows)
+{imports}
+import subprocess
+import sys
 
-        col2_limit = shutil.get_terminal_size().columns - 20
-        if col2_limit < 20:
-            error("increase screen size to view table", code=1)
-        elif sizes[1] > col2_limit:
-            sizes[1] = col2_limit
-
-        header, rows = rows[0], rows[1:]
-        # this is maybe taking comprehensions too far....
-        table_rows = (
-            self._make_row(row)
-            for row in (
-                # header row
-                (
-                    self.__dict__[header_style] + f"{cell:<{sizes[i]}}" + self.end
-                    for i, cell in enumerate(header)
-                ),
-                # rest of the rows
-                *(
-                    (f"{cell:<{sizes[i]}}" for i, cell in enumerate(row))
-                    for row in (
-                        newrow
-                        for row in rows
-                        for newrow in self._sanitize_row(sizes, row)
-                    )
-                ),
+if __name__ == "__main__":
+    vivenv = {self.noqa(self._use_str(spec, standalone))}
+    sys.exit(subprocess.run([vivenv / "bin" / "{bin}", *sys.argv[1:]]).returncode)
+"""
+
+    def update(
+        self, src: Optional[Path], cli: Path, local_version: str, next_version: str
+    ) -> str:
+        return f"""
+  Update source at {a.green}{src}{a.end}
+  Symlink {a.bold}{src}{a.end} to {a.bold}{cli}{a.end}
+  Version {a.bold}{local_version}{a.end} -> {a.bold}{next_version}{a.end}
+
+"""
+
+    def install(self, src: Path, cli: Path) -> str:
+        return f"""
+  Install viv.py to {a.green}{src}{a.end}
+  Symlink {a.bold}{src}{a.end} to {a.bold}{cli}{a.end}
+
+"""
+
+    def show(
+        self, cli: Optional[Path | str], running: Path, local: Optional[Path | str]
+    ) -> str:
+        return (
+            "\n".join(
+                f"  {a.bold}{k}{a.end}: {v}"
+                for k, v in (
+                    ("Version", __version__),
+                    ("CLI", cli),
+                    ("Running Source", running),
+                    ("Local Source", local),
+                )
             )
+            + "\n"
         )
 
-        sys.stderr.write(f"  {BOX['tl']}{BOX['h']*(sum(sizes)+5)}{BOX['tr']}\n")
-        sys.stderr.write("\n".join(table_rows) + "\n")
-        sys.stderr.write(f"  {BOX['bl']}{BOX['h']*(sum(sizes)+5)}{BOX['br']}\n")
 
-
-a = Ansi()
+t = Template()
 
 
-# TODO: convet the below functions into a proper file/stream logging interface
+# TODO: convert the below functions into a proper file/stream logging interface
 def echo(
     msg: str, style: str = "magenta", newline: bool = True, fd: TextIO = sys.stderr
 ) -> None:
     """output general message to stdout"""
     output = f"{a.viv_preamble(style)} {msg}"
     if newline:
         output += "\n"
@@ -511,17 +563,15 @@
             command,
             stdout=None if verbose else subprocess.PIPE,
             stderr=None if verbose else subprocess.STDOUT,
             universal_newlines=True,
         )
 
     if p.returncode != 0 and not ignore_error:
-        error("subprocess failed")
-        echo("see below for command output", style="red")
-        a.subprocess(p.stdout)
+        a.subprocess(command, p.stdout)
 
         if clean_up_path and clean_up_path.is_dir():
             shutil.rmtree(str(clean_up_path))
 
         sys.exit(p.returncode)
 
     elif check_output:
@@ -547,45 +597,86 @@
             str(spec) + (str(Path(sys.executable).resolve()) if track_exe else "N/A")
         ).encode()
     )
 
     return sha256.hexdigest()
 
 
+@dataclass
+class Meta:
+    name: str
+    id: str
+    spec: List[str]
+    files: List[str]
+    exe: str
+    created: str = ""
+    accessed: str = ""
+
+    @classmethod
+    def load(cls, name: str) -> "Meta":
+        if not (c.venvcache / name / "vivmeta.json").exists():
+            warn(f"possibly corrupted vivenv: {name}")
+            # add empty values for corrupted vivenvs so it will still load
+            return cls(name=name, spec=[""], files=[""], exe="", id="")
+        else:
+            meta = json.loads((c.venvcache / name / "vivmeta.json").read_text())
+
+        return cls(**meta)
+
+    def write(self, p: Path | None = None) -> None:
+        if not p:
+            p = (c.venvcache) / self.name / "vivmeta.json"
+
+        p.write_text(json.dumps(self.__dict__))
+
+    def addfile(self, f: Path) -> None:
+        self.accessed = str(datetime.today())
+        self.files = sorted({*self.files, str(f.absolute().resolve())})
+
+
 class ViVenv:
     def __init__(
         self,
-        spec: List[str],
+        spec: List[str] = [""],
         track_exe: bool = False,
         id: str | None = None,
         name: str = "",
         path: Path | None = None,
+        skip_load: bool = False,
+        metadata: Meta | None = None,
     ) -> None:
-        self.spec = self._validate_spec(spec)
-        self.exe = str(Path(sys.executable).resolve()) if track_exe else "N/A"
-        self.id = id if id else get_hash(spec, track_exe)
-        self.name = name if name else self.id
+        self.loaded = False
+        spec = self._validate_spec(spec)
+        id = id if id else get_hash(spec, track_exe)
+
+        self.name = name if name else id
         self.path = path if path else c.venvcache / self.name
-        self.exists = self.name in [d.name for d in c.venvcache.iterdir()]
+
+        if not metadata:
+            if self.name in (d.name for d in c.venvcache.iterdir()):
+                self.loaded = True
+                self.meta = Meta.load(self.name)
+            else:
+                self.meta = Meta(
+                    spec=spec,
+                    name=self.name,
+                    id=id,
+                    files=[],
+                    exe=str(Path(sys.executable).resolve()) if track_exe else "N/A",
+                )
+        else:
+            self.meta = metadata
 
     @classmethod
     def load(cls, name: str) -> "ViVenv":
-        """generate a vivenv from a viv-info.json file
+        """generate a vivenv from a vivmeta.json
         Args:
             name: used as lookup in the vivenv cache
         """
-        if not (c.venvcache / name / "viv-info.json").is_file():
-            warn(f"possibly corrupted vivenv: {name}")
-            return cls(name=name, spec=[""])
-        else:
-            with (c.venvcache / name / "viv-info.json").open("r") as f:
-                venvconfig = json.load(f)
-
-        vivenv = cls(name=name, spec=venvconfig["spec"], id=venvconfig["id"])
-        vivenv.exe = venvconfig["exe"]
+        vivenv = cls(name=name, metadata=Meta.load(name))
 
         return vivenv
 
     def _validate_spec(self, spec: List[str]) -> List[str]:
         """ensure spec is at least of sequence of strings
 
         Args:
@@ -597,274 +688,151 @@
 
         return sorted(spec)
 
     def create(self, quiet: bool = False) -> None:
         if not quiet:
             echo(f"new unique vivenv -> {self.name}")
         with Spinner("creating vivenv"):
-            builder = venv.EnvBuilder(with_pip=True, clear=True)
-            builder.create(self.path)
+            venv.create(self.path, with_pip=True, clear=True, symlinks=True)
 
             # add config to ignore pip version
-            with (self.path / "pip.conf").open("w") as f:
-                f.write("[global]\ndisable-pip-version-check = true")
+            (self.path / "pip.conf").write_text(
+                "[global]\ndisable-pip-version-check = true"
+            )
+
+        self.meta.created = str(datetime.today())
 
     def install_pkgs(self) -> None:
         cmd: List[str] = [
             str(self.path / "bin" / "pip"),
             "install",
             "--force-reinstall",
-        ] + self.spec
+        ] + self.meta.spec
 
         run(
             cmd,
             spinmsg="installing packages in vivenv",
             clean_up_path=self.path,
             verbose=bool(os.getenv("VIV_VERBOSE")),
         )
 
-    def dump_info(self, write: bool = False) -> None:
-        # TODO: include associated files in 'info'
-        # means it needs to be loaded first
-        # or keep a seperate file hash in c.share?
-        info = {
-            "created": str(datetime.today()),
-            "id": self.id,
-            "spec": self.spec,
-            "exe": self.exe,
-        }
+    def touch(self) -> None:
+        self.meta.accessed = str(datetime.today())
 
-        # save metadata to json file
-        if write:
-            with (self.path / "viv-info.json").open("w") as f:
-                json.dump(info, f)
-        else:
-            info["spec"] = ", ".join(self.spec)
-            a.table((("key", "value"), *((k, v) for k, v in info.items())))
+    def show(self) -> None:
+        _id = (
+            self.meta.id[:8]
+            if self.meta.id == self.name
+            else (self.name[:5] + "..." if len(self.name) > 8 else self.name)
+        )
+
+        sys.stdout.write(
+            f"""{a.bold}{a.cyan}{_id}{a.end} """
+            f"""{a.style(", ".join(self.meta.spec),'dim')}\n"""
+        )
+
+    def _tree_leaves(self, items: List[str], indent: str = "") -> str:
+        tree_chars = ["├"] * (len(items) - 1) + ["╰"]
+        return "\n".join(
+            (f"{indent}{a.yellow}{c}─{a.end} {i}" for c, i in zip(tree_chars, items))
+        )
+
+    def tree(self) -> None:
+        _id = self.meta.id if self.meta.id == self.name else self.name
+        # TODO: generarlize and loop this or make a template..
+        items = [
+            f"{a.magenta}{k}{a.end}: {v}"
+            for k, v in {
+                **{
+                    "spec": ", ".join(self.meta.spec),
+                    "created": self.meta.created,
+                    "accessed": self.meta.accessed,
+                },
+                **({"exe": self.meta.exe} if self.meta.exe != "N/A" else {}),
+                **({"files": ""} if self.meta.files else {}),
+            }.items()
+        ]
+        rows = [f"\n{a.bold}{a.cyan}{_id}{a.end}", self._tree_leaves(items)]
+        if self.meta.files:
+            rows += (self._tree_leaves(self.meta.files, indent="   "),)
+
+        sys.stdout.write("\n".join(rows) + "\n")
+
+
+def get_caller_path() -> Path:
+    """get callers callers file path"""
+    # viv.py is fist in stack since function is used in `viv.use()`
+    frame_info = inspect.stack()[2]
+    filepath = frame_info.filename  # in python 3.5+, you can use frame_info.filename
+    del frame_info  # drop the reference to the stack frame to avoid reference cycles
+
+    return Path(filepath).absolute()
 
 
 def use(*packages: str, track_exe: bool = False, name: str = "") -> Path:
     """create a vivenv and append to sys.path
 
     Args:
         packages: package specifications with optional version specifiers
         track_exe: if true make env python exe specific
         name: use as vivenv name, if not provided id is used
     """
-    vivenv = ViVenv(list(packages), track_exe=track_exe, name=name)
 
-    if not vivenv.exists or os.getenv("VIV_FORCE"):
+    vivenv = ViVenv(list(packages), track_exe=track_exe, name=name)
+    if not vivenv.loaded or os.getenv("VIV_FORCE"):
         vivenv.create()
         vivenv.install_pkgs()
-        vivenv.dump_info(write=True)
+
+    vivenv.meta.addfile(get_caller_path())
+    vivenv.meta.write()
 
     modify_sys_path(vivenv.path)
     return vivenv.path
 
 
 def modify_sys_path(new_path: Path) -> None:
-    # remove user-site
-    for i, path in enumerate(sys.path):
-        if path == site.USER_SITE:
-            sys.path.pop(i)
-
-    sys.path.append(
-        str([p for p in (new_path / "lib").glob("python*/site-packages")][0])
-    )
+    sys.path = [p for p in sys.path if p is not site.USER_SITE]
+    site.addsitedir(str(*(new_path / "lib").glob("python*/site-packages")))
 
 
 def get_venvs() -> Dict[str, ViVenv]:
     vivenvs = {}
     for p in c.venvcache.iterdir():
         vivenv = ViVenv.load(p.name)
         vivenvs[vivenv.name] = vivenv
     return vivenvs
 
 
-# TODO: make a template class?
-
-SYS_PATH_TEMPLATE = """__import__("sys").path.append("{path_to_viv}")  # noqa"""
-REL_SYS_PATH_TEMPLATE = (
-    """__import__("sys").path.append(__import__("os")"""
-    """.path.expanduser("{path_to_viv}"))  # noqa"""
-)
-IMPORT_TEMPLATE = """__import__("viv").use({spec})  # noqa"""
-
-STANDALONE_TEMPLATE = r"""
-# <<<<< auto-generated by viv (v{version})
-# see `python3 <(curl -fsSL gh.dayl.in/viv/viv.py) --help`
-# fmt: off
-{func}
-# fmt: on
-# >>>>> code golfed with <3
-"""  # noqa
-
-STANDALONE_TEMPLATE_FUNC = r"""def _viv_use(*pkgs, track_exe=False, name=""):
-    T,F=True,False;i,s,m,e,spec=__import__,str,map,lambda x: T if x else F,[*pkgs]
-    if not {*m(type,pkgs)}=={s}: raise ValueError(f"spec: {pkgs} is invalid")
-    ge,sys,P,ew=i("os").getenv,i("sys"),i("pathlib").Path,i("sys").stderr.write
-    (cache:=(P(ge("XDG_CACHE_HOME",P.home()/".cache"))/"viv"/"venvs")).mkdir(parents=T,exist_ok=T)
-    ((sha256:=i("hashlib").sha256()).update((s(spec)+
-     (((exe:=("N/A",s(P(i("sys").executable).resolve()))[e(track_exe)])))).encode()))
-    if ((env:=cache/(name if name else (_id:=sha256.hexdigest())))
-        not in cache.glob("*/")) or ge("VIV_FORCE"):
-        v=e(ge("VIV_VERBOSE"));ew(f"generating new vivenv -> {env.name}\n")
-        i("venv").EnvBuilder(with_pip=T,clear=T).create(env)
-        with (env/"pip.conf").open("w") as f:f.write("[global]\ndisable-pip-version-check=true")
-        if (p:=i("subprocess").run([env/"bin"/"pip","install","--force-reinstall",*spec],text=True,
-            stdout=(-1,None)[v],stderr=(-2,None)[v])).returncode!=0:
-            if env.is_dir():i("shutil").rmtree(env)
-            ew(f"pip had non zero exit ({p.returncode})\n{p.stdout}\n");sys.exit(p.returncode)
-        with (env/"viv-info.json").open("w") as f:
-            i("json").dump({"created":s(i("datetime").datetime.today()),
-            "id":_id,"spec":spec,"exe":exe},f)
-    sys.path = [p for p in (*sys.path,s(*(env/"lib").glob("py*/si*"))) if p!=i("site").USER_SITE]
-    return env
-"""  # noqa
-
-SHOW_TEMPLATE = f"""
-  {a.style('Version', 'bold')}: {{version}}
-  {a.style('CLI', 'bold')}: {{cli}}
-  {a.style('Running Source', 'bold')}: {{running_src}}
-  {a.style('Local Source', 'bold')}: {{local_src}}
-"""
-
-INSTALL_TEMPLATE = f"""
-  Install viv.py to {a.green}{{src_location}}{a.end}
-  Symlink {a.bold}{{src_location}}{a.end} to {a.bold}{{cli_location}}{a.end}
-
-"""
-
-UPDATE_TEMPLATE = f"""
-  Update source at {a.green}{{src_location}}{a.end}
-  Symlink {a.bold}{{src_location}}{a.end} to {a.bold}{{cli_location}}{a.end}
-  Version {a.bold}{{local_version}}{a.end} -> {a.bold}{{next_version}}{a.end}
-
-"""
-
-SHIM_TEMPLATE = """\
-#!/usr/bin/env python3
-
-{imports}
-import subprocess
-import sys
-
-if __name__ == "__main__":
-    vivenv = {use}
-    sys.exit(subprocess.run([vivenv / "bin" / "{bin}", *sys.argv[1:]]).returncode)
-"""
-
-DESCRIPTION = f"""
-
-{a.tagline()}
-to create/activate a vivenv:
-- from command line: `{a.style("viv -h","bold")}`
-- within python script: {a.style('__import__("viv").use("typer", "rich-click")','bold')}
-"""
-
-
-def noqa(txt: str) -> str:
-    max_length = max(map(len, txt.splitlines()))
-    return "\n".join((f"{line:{max_length}} # noqa" for line in txt.splitlines()))
-
-
-def spec_to_import(spec: List[str]) -> None:
-    spec_str = ", ".join(f'"{pkg}"' for pkg in spec)
-    sys.stdout.write(IMPORT_TEMPLATE.format(spec=spec_str) + "\n")
-
-
 def combined_spec(reqs: List[str], requirements: Path) -> List[str]:
     if requirements:
         with requirements.open("r") as f:
             reqs += f.readlines()
-
     return reqs
 
 
 def resolve_deps(args: Namespace) -> List[str]:
     spec = combined_spec(args.reqs, args.requirements)
 
-    with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
-        echo("generating frozen spec")
-        vivenv = ViVenv(spec, track_exe=False, path=Path(tmpdir))
-
-        vivenv.create(quiet=True)
-        # populate the environment for now use
-        # custom cmd since using requirements file
-        cmd = [
-            str(vivenv.path / "bin" / "pip"),
-            "install",
-            "--force-reinstall",
-        ] + spec
-
-        run(cmd, spinmsg="resolving dependencies", clean_up_path=vivenv.path)
+    cmd = [
+        "pip",
+        "install",
+        "--dry-run",
+        "--quiet",
+        "--ignore-installed",
+        "--report",
+        "-",
+    ] + spec
+
+    report = json.loads(run(cmd, check_output=True, spinmsg="resolving depedencies"))
+    resolved_spec = [
+        f"{pkg['metadata']['name']}=={pkg['metadata']['version']}"
+        for pkg in report["install"]
+    ]
 
-        cmd = [str(vivenv.path / "bin" / "pip"), "freeze"]
-        resolved_spec = run(cmd, check_output=True)
-    return resolved_spec.splitlines()
-
-
-def generate_import(
-    args: Namespace,
-) -> None:
-    spec = resolve_deps(args)
-    if args.keep:
-        # re-create env again since path's are hard-coded
-        vivenv = ViVenv(spec)
-
-        if vivenv.name not in [d.name for d in c.venvcache.iterdir()] or os.getenv(
-            "VIV_FORCE"
-        ):
-            vivenv.create()
-            vivenv.install_pkgs()
-            vivenv.dump_info(write=True)
-
-        else:
-            echo("re-using existing vivenv")
-
-    echo("see below for import statements\n")
-
-    if args.standalone:
-        sys.stdout.write(
-            STANDALONE_TEMPLATE.format(
-                version=__version__,
-                func=noqa(
-                    STANDALONE_TEMPLATE_FUNC
-                    + "_viv_use("
-                    + fill(
-                        ", ".join(f'"{pkg}"' for pkg in spec),
-                        width=100,
-                        subsequent_indent="    ",
-                    )
-                    + ")"
-                ),
-            )
-            + "\n"
-        )
-        return
-
-    if args.path:
-        if args.path == "abs":
-            sys.stdout.write(
-                SYS_PATH_TEMPLATE.format(
-                    path_to_viv=Path(__file__).resolve().absolute().parent.parent
-                )
-                + "\n"
-            )
-        elif args.path == "rel":
-            sys.stdout.write(
-                REL_SYS_PATH_TEMPLATE.format(
-                    path_to_viv=str(
-                        Path(__file__).resolve().absolute().parent.parent
-                    ).replace(str(Path.home()), "~")
-                )
-                + "\n"
-            )
-
-    spec_to_import(spec)
+    return resolved_spec
 
 
 def fetch_source(reference: str) -> str:
     try:
         r = urlopen(
             "https://raw.githubusercontent.com/daylinmorgan/viv/"
             + reference
@@ -895,21 +863,54 @@
 def make_executable(path: Path) -> None:
     """apply an executable bit for all users with read access"""
     mode = os.stat(path).st_mode
     mode |= (mode & 0o444) >> 2  # copy R bits to X
     os.chmod(path, mode)
 
 
+class Config:
+    """viv config manager"""
+
+    def __init__(self) -> None:
+        self._cache = Path(os.getenv("XDG_CACHE_HOME", Path.home() / ".cache")) / "viv"
+
+    def _ensure(self, p: Path) -> Path:
+        p.mkdir(parents=True, exist_ok=True)
+        return p
+
+    @property
+    def venvcache(self) -> Path:
+        return self._ensure(self._cache / "venvs")
+
+    @property
+    def srccache(self) -> Path:
+        return self._ensure(self._cache / "src")
+
+    @property
+    def binparent(self) -> Path:
+        return self._ensure(
+            Path(os.getenv("VIV_BIN_DIR", Path.home() / ".local" / "bin"))
+        )
+
+    @property
+    def srcdefault(self) -> Path:
+        parent = (
+            Path(os.getenv("XDG_DATA_HOME", Path.home() / ".local" / "share")) / "viv"
+        )
+        return self._ensure(parent) / "viv.py"
+
+
+c = Config()
+
+
 class Viv:
     def __init__(self) -> None:
         self.vivenvs = get_venvs()
         self._get_sources()
-        self.name = (
-            "viv" if self.local else "python3 <(curl -fsSL gh.dayl.in/viv/viv.py)"
-        )
+        self.name = "viv" if self.local else "python3 <(curl -fsSL viv.dayl.in/viv.py)"
 
     def _get_sources(self) -> None:
         self.local_source: Optional[Path] = None
         self.running_source = Path(__file__).resolve()
         self.local = not str(self.running_source).startswith("/proc/")
         if self.local:
             self.local_source = self.running_source
@@ -925,29 +926,22 @@
                 self.local_version = "Not Found"
 
         if self.local_source:
             self.git = (self.local_source.parent.parent.parent / ".git").is_dir()
         else:
             self.git = False
 
-    def _check_local_source(self, args: Namespace) -> None:
-        if not self.local_source and not (args.standalone or args.path):
-            warn(
-                "failed to find local copy of `viv` "
-                "make sure to add it to your PYTHONPATH "
-                "or consider using --path/--standalone"
-            )
-
     def _match_vivenv(self, name_id: str) -> ViVenv:  # type: ignore[return]
-        # TODO: improve matching algorithm to favor names over id's
         matches: List[ViVenv] = []
         for k, v in self.vivenvs.items():
             if name_id == k or v.name == name_id:
                 matches.append(v)
-            elif k.startswith(name_id) or v.id.startswith(name_id):
+            elif k.startswith(name_id) or (
+                v.meta.id.startswith(name_id) and v.meta.id == v.name
+            ):
                 matches.append(v)
             elif v.name.startswith(name_id):
                 matches.append(v)
 
         if len(matches) == 1:
             return matches[0]
         elif len(matches) > 1:
@@ -974,185 +968,166 @@
                     f"cowardly exiting because I didn't find vivenv: {name}",
                     code=1,
                 )
 
     def freeze(self, args: Namespace) -> None:
         """create import statement from package spec"""
 
-        self._check_local_source(args)
+        spec = resolve_deps(args)
+        if args.keep:
+            # re-create env again since path's are hard-coded
+            vivenv = ViVenv(spec)
+
+            if not vivenv.loaded or os.getenv("VIV_FORCE"):
+                vivenv.create()
+                vivenv.install_pkgs()
+                vivenv.meta.write()
+            else:
+                echo("re-using existing vivenv")
 
-        if not args.reqs:
-            error("must specify a requirement", code=1)
-        if args.path and args.standalone:
-            error("-p/--path and -s/--standalone are mutually exclusive", code=1)
+            vivenv.touch()
+            vivenv.meta.write()
 
-        generate_import(
-            args,
-        )
+        echo("see below for import statements\n")
+
+        if args.standalone:
+            sys.stdout.write(t.standalone(spec))
+            return
+
+        if args.path and not self.local_source:
+            error("No local viv found to import from", code=1)
+
+        sys.stdout.write(t.frozen_import(args.path, self.local_source, spec))
 
     def list(self, args: Namespace) -> None:
         """list all vivenvs"""
 
         if args.quiet:
             sys.stdout.write("\n".join(self.vivenvs) + "\n")
         elif len(self.vivenvs) == 0:
             echo("no vivenvs setup")
-        else:
-            rows = (
-                ("vivenv", "spec"),
-                *(
-                    (
-                        f"{vivenv.name[:6]}..."
-                        if len(vivenv.name) > 9
-                        else vivenv.name,
-                        ", ".join(vivenv.spec),
-                    )
-                    for vivenv in self.vivenvs.values()
-                ),
+        elif args.full:
+            for _, vivenv in self.vivenvs.items():
+                vivenv.tree()
+        elif args.json:
+            sys.stdout.write(
+                json.dumps({k: v.meta.__dict__ for k, v in self.vivenvs.items()})
             )
-            a.table(rows)
+        else:
+            for _, vivenv in self.vivenvs.items():
+                vivenv.show()
 
     def exe(self, args: Namespace) -> None:
-        """run python/pip in vivenv"""
+        """\
+        run binary/script in existing vivenv
+
+        examples:
+            viv exe <vivenv> pip -- list
+            viv exe <vivenv> python -- script.py
+        """
 
         vivenv = self._match_vivenv(args.vivenv)
+        bin = vivenv.path / "bin" / args.cmd
+
+        if not bin.exists():
+            error(f"{args.cmd} does not exist in {vivenv.name}", code=1)
 
-        pip_path, python_path = (vivenv.path / "bin" / cmd for cmd in ("pip", "python"))
-        # todo check for vivenv
-        echo(f"executing command within {vivenv.name}")
-
-        cmd = (
-            f"{pip_path} {' '.join(args.cmd)}"
-            if args.exe == "pip"
-            else f"{python_path} {' '.join(args.cmd)}"
-        ) + " ".join(args.rest)
+        cmd = [bin, *args.rest]
 
-        echo(f"executing {cmd}")
-        run(shlex.split(cmd), verbose=True)
+        run(cmd, verbose=True)
 
     def info(self, args: Namespace) -> None:
         """get metadata about a vivenv"""
         vivenv = self._match_vivenv(args.vivenv)
-        metadata_file = vivenv.path / "viv-info.json"
+        metadata_file = vivenv.path / "vivmeta.json"
 
         if not metadata_file.is_file():
             error(f"Unable to find metadata for vivenv: {args.vivenv}", code=1)
-
-        echo(f"more info about {vivenv.name}:")
-
-        vivenv.dump_info()
+        if args.json:
+            sys.stdout.write(json.dumps(vivenv.meta.__dict__))
+        else:
+            vivenv.tree()
 
     def _install_local_src(self, sha256: str, src: Path, cli: Path) -> None:
         echo("updating local source copy of viv")
         shutil.copy(c.srccache / f"{sha256}.py", src)
         make_executable(src)
         echo("symlinking cli")
 
-        if cli.is_file() and confirm(
-            f"Existing file at {a.style(str(cli),'bold')}, "
-            "would you like to overwrite it?"
-        ):
-            cli.unlink()
-            cli.symlink_to(src)
+        if cli.is_file():
+            echo(f"Existing file at {a.style(str(cli),'bold')}")
+            if confirm("Would you like to overwrite it?"):
+                cli.unlink()
+                cli.symlink_to(src)
         else:
             cli.symlink_to(src)
 
         echo("Remember to include the following line in your shell rc file:")
         sys.stderr.write(
             '  export PYTHONPATH="$PYTHONPATH:$HOME/'
             f'{src.relative_to(Path.home()).parent}"\n'
         )
 
+    def _get_new_version(self, ref: str) -> Tuple[str, str]:
+        sys.path.append(str(c.srccache))
+        return (sha256 := fetch_source(ref)), __import__(sha256).__version__
+
     def manage(self, args: Namespace) -> None:
         """manage viv itself"""
 
-        if args.cmd == "show":
+        if args.subcmd == "show":
             if args.pythonpath:
                 if self.local and self.local_source:
                     sys.stdout.write(str(self.local_source.parent) + "\n")
                 else:
                     error("expected to find a local installation", code=1)
             else:
                 echo("Current:")
                 sys.stderr.write(
-                    SHOW_TEMPLATE.format(
-                        version=__version__,
+                    t.show(
                         cli=shutil.which("viv"),
-                        running_src=self.running_source,
-                        local_src=self.local_source,
+                        running=self.running_source,
+                        local=self.local_source,
                     )
                 )
 
-        elif args.cmd == "update":
-            if not self.local_source:
-                error(
-                    a.style("viv manage update", "bold")
-                    + " should be used with an exisiting installation",
-                    1,
-                )
-
-            if self.git:
-                error(
-                    a.style("viv manage update", "bold")
-                    + " shouldn't be used with a git-based installation",
-                    1,
-                )
-            sha256 = fetch_source(args.ref)
-            sys.path.append(str(c.srccache))
-            next_version = __import__(sha256).__version__
+        elif args.subcmd == "update":
+            sha256, next_version = self._get_new_version(args.ref)
 
             if self.local_version == next_version:
                 echo(f"no change between {args.ref} and local version")
                 sys.exit(0)
 
             if confirm(
                 "Would you like to perform the above installation steps?",
-                UPDATE_TEMPLATE.format(
-                    src_location=self.local_source,
-                    local_version=self.local_version,
-                    cli_location=args.cli,
-                    next_version=next_version,
-                ),
+                t.update(self.local_source, args.cli, self.local_version, next_version),
             ):
                 self._install_local_src(
                     sha256,
                     Path(
                         args.src if not self.local_source else self.local_source,
                     ),
                     args.cli,
                 )
 
-        elif args.cmd == "install":
-            if self.local_source:
-                error(f"found existing viv installation at {self.local_source}")
-                echo(
-                    "use "
-                    + a.style("viv manage update", "bold")
-                    + " to modify current installation.",
-                    style="red",
-                )
-                sys.exit(1)
+        elif args.subcmd == "install":
+            sha256, downloaded_version = self._get_new_version(args.ref)
 
-            sha256 = fetch_source(args.ref)
-            sys.path.append(str(c.srccache))
-            downloaded_version = __import__(sha256).__version__
             echo(f"Downloaded version: {downloaded_version}")
 
             # TODO: see if file is actually where
             # we are about to install and give more instructions
 
             if confirm(
                 "Would you like to perform the above installation steps?",
-                INSTALL_TEMPLATE.format(
-                    src_location=args.src,
-                    cli_location=args.cli,
-                ),
+                t.install(args.src, args.cli),
             ):
                 self._install_local_src(sha256, args.src, args.cli)
-        elif args.cmd == "purge":
+
+        elif args.subcmd == "purge":
             to_remove = []
             if c._cache.is_dir():
                 to_remove.append(c._cache)
             if args.src.is_file():
                 to_remove.append(
                     args.src.parent if args.src == c.srcdefault else args.src
                 )
@@ -1174,341 +1149,375 @@
                     if p.is_dir():
                         shutil.rmtree(p)
                     else:
                         p.unlink()
 
                 echo(
                     "to re-install use: "
-                    "`python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage install`"
+                    "`python3 <(curl -fsSL viv.dayl.in/viv.py) manage install`"
                 )
 
     def _pick_bin(self, args: Namespace) -> Tuple[str, str]:
         default = re.split(r"[=><~!*]+", args.reqs[0])[0]
         return default, (default if not args.bin else args.bin)
 
     def shim(self, args: Namespace) -> None:
         """\
         generate viv-powered cli apps
 
         examples:
           viv shim black
           viv shim yartsu -o ~/bin/yartsu --standalone
         """
-        self._check_local_source(args)
-
-        if not args.reqs:
-            error("please specify at lease one dependency", code=1)
-
         default_bin, bin = self._pick_bin(args)
         output = (
             c.binparent / default_bin if not args.output else args.output.absolute()
         )
 
         if output.is_file():
             error(f"{output} already exists...exiting", code=1)
 
         if args.freeze:
             spec = resolve_deps(args)
         else:
             spec = combined_spec(args.reqs, args.requirements)
 
-        spec_str = ", ".join(f'"{req}"' for req in spec)
-        if args.standalone:
-            imports = STANDALONE_TEMPLATE.format(
-                version=__version__, func=noqa(STANDALONE_TEMPLATE_FUNC)
-            )
-            use = f"_viv_use({spec_str})"
-        elif args.path:
-            if not self.local_source:
-                error("No local viv found to import from", code=1)
-            else:
-                imports = (
-                    REL_SYS_PATH_TEMPLATE.format(
-                        path_to_viv=str(
-                            self.local_source.resolve().absolute().parent.parent
-                        ).replace(str(Path.home()), "~")
-                    )
-                    if args.path == "abs"
-                    else SYS_PATH_TEMPLATE.format(
-                        path_to_viv=self.local_source.resolve().absolute().parent.parent
-                    )
-                )
-                use = IMPORT_TEMPLATE.format(spec=spec_str)
-        else:
-            imports = ""
-            use = IMPORT_TEMPLATE.format(spec=spec_str)
-
         if confirm(
             f"Write shim for {a.style(bin,'bold')} to {a.style(output,'green')}?"
         ):
             with output.open("w") as f:
-                f.write(SHIM_TEMPLATE.format(imports=imports, use=use, bin=bin))
+                f.write(
+                    t.shim(args.path, self.local_source, args.standalone, spec, bin)
+                )
 
             make_executable(output)
 
     def run(self, args: Namespace) -> None:
         """\
-        run an app w/ an on-demand venv
+        run an app with an on-demand venv
 
         examples:
-          viv r pycowsay -- "Viv isn't venv\!"
+          viv r pycowsay -- "viv isn't venv\!"
           viv r rich -b python -- -m rich
         """
-        if not args.reqs:
-            error("please specify at lease one dependency", code=1)
 
         _, bin = self._pick_bin(args)
         spec = combined_spec(args.reqs, args.requirements)
         vivenv = ViVenv(spec)
 
         # TODO: respect a VIV_RUN_MODE env variable as the same as keep i.e.
         # ephemeral (default), semi-ephemeral (persist inside /tmp), or
         # persist (use c.cache)
 
-        if not vivenv.exists or os.getenv("VIV_FORCE"):
+        if not vivenv.loaded or os.getenv("VIV_FORCE"):
             if not args.keep:
                 with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
                     vivenv.path = Path(tmpdir)
                     vivenv.create()
                     vivenv.install_pkgs()
                     sys.exit(
                         subprocess.run(
                             [vivenv.path / "bin" / bin, *args.rest]
                         ).returncode
                     )
             else:
                 vivenv.create()
                 vivenv.install_pkgs()
-                vivenv.dump_info(write=True)
+
+        vivenv.touch()
+        vivenv.meta.write()
 
         sys.exit(subprocess.run([vivenv.path / "bin" / bin, *args.rest]).returncode)
 
+
+class Arg:
+    def __init__(self, *args: str, **kwargs: Any) -> None:
+        self.args = args
+        self.kwargs = kwargs
+
+
+class Cli:
+    args = {
+        ("list",): [
+            Arg(
+                "-f",
+                "--full",
+                help="show full metadata for vivenvs",
+                action="store_true",
+            ),
+            Arg(
+                "-q",
+                "--quiet",
+                help="suppress non-essential output",
+                action="store_true",
+            ),
+        ],
+        ("shim",): [
+            Arg(
+                "-f",
+                "--freeze",
+                help="freeze/resolve all dependencies",
+                action="store_true",
+            ),
+            Arg(
+                "-o",
+                "--output",
+                help="path/to/output file",
+                type=Path,
+                metavar="<path>",
+            ),
+        ],
+        ("remove",): [Arg("vivenv", help="name/hash of vivenv", nargs="*")],
+        ("exe", "info"): [Arg("vivenv", help="name/hash of vivenv")],
+        ("list", "info"): [
+            Arg(
+                "--json",
+                help="name:metadata json for vivenvs ",
+                action="store_true",
+                default=False,
+            )
+        ],
+        ("freeze", "shim"): [
+            Arg(
+                "-p",
+                "--path",
+                help="generate line to add viv to sys.path",
+                choices=["abs", "rel"],
+            ),
+            Arg(
+                "-s",
+                "--standalone",
+                help="generate standalone activation function",
+                action="store_true",
+            ),
+        ],
+        ("run", "freeze", "shim"): [
+            Arg(
+                "-k",
+                "--keep",
+                help="preserve environment",
+                action="store_true",
+            ),
+            Arg("reqs", help="requirements specifiers", nargs="*"),
+            Arg(
+                "-r",
+                "--requirements",
+                help="path/to/requirements.txt file",
+                metavar="<path>",
+            ),
+        ],
+        ("run", "shim"): [
+            Arg("-b", "--bin", help="console_script/script to invoke", metavar="<bin>"),
+        ],
+        ("manage|purge", "manage|update", "manage|install"): [
+            Arg(
+                "-r",
+                "--ref",
+                help="git reference (branch/tag/commit)",
+                default="latest",
+                metavar="<ref>",
+            ),
+            Arg(
+                "-s",
+                "--src",
+                help="path/to/source_file",
+                default=c.srcdefault,
+                metavar="<src>",
+            ),
+            Arg(
+                "-c",
+                "--cli",
+                help="path/to/cli (symlink to src)",
+                default=Path.home() / ".local" / "bin" / "viv",
+                metavar="<cli>",
+            ),
+        ],
+        "manage|show": [
+            Arg(
+                "-p",
+                "--pythonpath",
+                help="show the path/to/install",
+                action="store_true",
+            )
+        ],
+        ("exe"): [
+            Arg(
+                "cmd",
+                help="command to to execute",
+            )
+        ],
+    }
+    (
+        cmds := dict.fromkeys(
+            (
+                "list",
+                "shim",
+                "run",
+                "exe",
+                "remove",
+                "freeze",
+                "info",
+                "manage",
+            )
+        )
+    ).update(
+        {
+            "manage": {
+                subcmd: {"help": help, "aliases": [subcmd[0]]}
+                for subcmd, help in (
+                    ("show", "show current installation"),
+                    ("install", "install fresh viv"),
+                    ("update", "update viv version"),
+                    ("purge", "remove traces of viv"),
+                )
+            }
+        }
+    )
+
+    def __init__(self, viv: Viv) -> None:
+        self.viv = viv
+        self.parser = ArgumentParser(prog=viv.name, description=t.description)
+        self._cmd_arg_group_map()
+        self._make_parsers()
+        self._add_args()
+
+    def _cmd_arg_group_map(self) -> None:
+        self.cmd_arg_group_map: Dict[str, List[Sequence[str] | str]] = {}
+        for grp in self.args:
+            if isinstance(grp, str):
+                self.cmd_arg_group_map.setdefault(grp, []).append(grp)
+            else:
+                for cmd in grp:
+                    self.cmd_arg_group_map.setdefault(cmd, []).append(grp)
+
+    def _make_parsers(self) -> None:
+        self.parsers = {**{grp: ArgumentParser(add_help=False) for grp in self.args}}
+
+    def _add_args(self) -> None:
+        for grp, args in self.args.items():
+            for arg in args:
+                self.parsers[grp].add_argument(*arg.args, **arg.kwargs)
+
+    def _validate_args(self, args: Namespace) -> None:
+        if args.func.__name__ in ("freeze", "shim", "run"):
+            if not args.reqs:
+                error("must specify a requirement", code=1)
+        if args.func.__name__ in ("freeze", "shim"):
+            if not self.viv.local_source and not (args.standalone or args.path):
+                warn(
+                    "failed to find local copy of `viv` "
+                    "make sure to add it to your PYTHONPATH "
+                    "or consider using --path/--standalone"
+                )
+
+            if args.path and not self.viv.local_source:
+                error("No local viv found to import from", code=1)
+
+            if args.path and args.standalone:
+                error("-p/--path and -s/--standalone are mutually exclusive", code=1)
+
+        if args.func.__name__ == "manage":
+            if args.subcmd == "install" and self.viv.local_source:
+                error(f"found existing viv installation at {self.viv.local_source}")
+                echo(
+                    "use "
+                    + a.style("viv manage update", "bold")
+                    + " to modify current installation.",
+                    style="red",
+                )
+                sys.exit(1)
+            if args.subcmd == "update":
+                if not self.viv.local_source:
+                    error(
+                        a.style("viv manage update", "bold")
+                        + " should be used with an exisiting installation",
+                        1,
+                    )
+
+                if self.viv.git:
+                    error(
+                        a.style("viv manage update", "bold")
+                        + " shouldn't be used with a git-based installation",
+                        1,
+                    )
+
     def _get_subcmd_parser(
         self,
         subparsers: _SubParsersAction[ArgumentParser],
         name: str,
         attr: Optional[str] = None,
         **kwargs: Any,
     ) -> ArgumentParser:
-        aliases = kwargs.pop("aliases", [name[0]])
-        cmd = getattr(self, attr if attr else name)
+        # override for remove
+        if name == "remove":
+            aliases = ["rm"]
+        else:
+            aliases = kwargs.pop("aliases", [name[0]])
+
+        cmd = getattr(self.viv, attr if attr else name)
         parser: ArgumentParser = subparsers.add_parser(
             name,
             help=cmd.__doc__.splitlines()[0],
             description=dedent(cmd.__doc__),
             aliases=aliases,
             **kwargs,
         )
         parser.set_defaults(func=cmd)
 
         return parser
 
-    def cli(self) -> None:
-        """cli entrypoint"""
-
-        parser = ArgumentParser(prog=self.name, description=DESCRIPTION)
-        parser.add_argument(
+    def run(self) -> None:
+        self.parser.add_argument(
             "-V",
             "--version",
             action="version",
             version=f"{a.bold}viv{a.end}, version {a.cyan}{__version__}{a.end}",
         )
 
-        subparsers = parser.add_subparsers(
+        cmd_p = self.parser.add_subparsers(
             metavar="<sub-cmd>", title="subcommands", required=True
         )
-        p_vivenv_arg = ArgumentParser(add_help=False)
-        p_vivenv_arg.add_argument("vivenv", help="name/hash of vivenv")
-        p_list = self._get_subcmd_parser(subparsers, "list")
-
-        p_list.add_argument(
-            "-q",
-            "--quiet",
-            help="suppress non-essential output",
-            action="store_true",
-            default=False,
-        )
-
-        p_exe = self._get_subcmd_parser(
-            subparsers,
-            "exe",
-        )
-        p_exe_sub = p_exe.add_subparsers(
-            title="subcommand", metavar="<sub-cmd>", required=True
-        )
-
-        p_exe_shared = ArgumentParser(add_help=False)
-        p_exe_shared.add_argument(
-            "cmd",
-            help="command to to execute",
-            nargs="*",
-        )
-
-        p_exe_sub.add_parser(
-            "python",
-            help="run command with python",
-            parents=[p_vivenv_arg, p_exe_shared],
-        ).set_defaults(func=self.exe, exe="python")
-
-        p_exe_sub.add_parser(
-            "pip", help="run command with pip", parents=[p_vivenv_arg, p_exe_shared]
-        ).set_defaults(func=self.exe, exe="pip")
-
-        p_remove = self._get_subcmd_parser(
-            subparsers,
-            "remove",
-            aliases=["rm"],
-        )
-
-        p_remove.add_argument("vivenv", help="name/hash of vivenv", nargs="*")
-
-        p_freeze_shim_shared = ArgumentParser(add_help=False)
-
-        p_freeze_shim_shared.add_argument(
-            "-p",
-            "--path",
-            help="generate line to add viv to sys.path",
-            choices=["abs", "rel"],
-        )
-        p_freeze_shim_shared.add_argument(
-            "-r",
-            "--requirements",
-            help="path/to/requirements.txt file",
-            metavar="<path>",
-        )
-        p_freeze_shim_shared.add_argument(
-            "-k",
-            "--keep",
-            help="preserve environment",
-            action="store_true",
-        )
-        p_freeze_shim_shared.add_argument(
-            "-s",
-            "--standalone",
-            help="generate standalone activation function",
-            action="store_true",
-        )
-        p_freeze_shim_shared.add_argument(
-            "reqs", help="requirements specifiers", nargs="*"
-        )
-
-        self._get_subcmd_parser(subparsers, "freeze", parents=[p_freeze_shim_shared])
-        self._get_subcmd_parser(
-            subparsers,
-            "info",
-            parents=[p_vivenv_arg],
-        )
-        p_manage_shared = ArgumentParser(add_help=False)
-        p_manage_shared.add_argument(
-            "-r",
-            "--ref",
-            help="git reference (branch/tag/commit)",
-            default="latest",
-            metavar="<ref>",
-        )
-
-        p_manage_shared.add_argument(
-            "-s",
-            "--src",
-            help="path/to/source_file",
-            default=c.srcdefault,
-            metavar="<src>",
-        )
-        p_manage_shared.add_argument(
-            "-c",
-            "--cli",
-            help="path/to/cli (symlink to src)",
-            default=Path.home() / ".local" / "bin" / "viv",
-            metavar="<cli>",
-        )
-
-        p_manage_sub = self._get_subcmd_parser(
-            subparsers,
-            name="manage",
-        ).add_subparsers(title="subcommand", metavar="<sub-cmd>", required=True)
-
-        p_manage_sub.add_parser(
-            "install", help="install viv", aliases="i", parents=[p_manage_shared]
-        ).set_defaults(func=self.manage, cmd="install")
-
-        p_manage_sub.add_parser(
-            "update",
-            help="update viv version",
-            aliases="u",
-            parents=[p_manage_shared],
-        ).set_defaults(func=self.manage, cmd="update")
-
-        (
-            p_manage_show := p_manage_sub.add_parser(
-                "show", help="show current installation info", aliases="s"
-            )
-        ).set_defaults(func=self.manage, cmd="show")
 
-        p_manage_show.add_argument(
-            "-p", "--pythonpath", help="show the path/to/install", action="store_true"
-        )
-
-        p_manage_sub.add_parser(
-            "purge", help="remove traces of viv", aliases="p", parents=[p_manage_shared]
-        ).set_defaults(func=self.manage, cmd="purge")
-
-        p_shim = self._get_subcmd_parser(
-            subparsers, "shim", parents=[p_freeze_shim_shared]
-        )
-
-        p_shim.add_argument(
-            "-f",
-            "--freeze",
-            help="freeze/resolve all dependencies",
-            action="store_true",
-        )
-        p_shim.add_argument(
-            "-o",
-            "--output",
-            help="path/to/output file",
-            type=Path,
-            metavar="<path>",
-        )
-        p_shim.add_argument(
-            "-b", "--bin", help="console_script/script to invoke", metavar="<bin>"
-        )
-
-        p_run = self._get_subcmd_parser(subparsers, "run")
-
-        p_run.add_argument(
-            "-r",
-            "--requirements",
-            help="path/to/requirements.txt file",
-            metavar="<path>",
-        )
-        p_run.add_argument(
-            "-k",
-            "--keep",
-            help="preserve environment",
-            action="store_true",
-        )
-        p_run.add_argument("reqs", help="requirements specifiers", nargs="*")
+        for cmd, subcmds in self.cmds.items():
+            if subcmds:
+                subcmd_p = self._get_subcmd_parser(cmd_p, cmd)
+                subcmd_cmd_p = subcmd_p.add_subparsers(
+                    title="subcommand", metavar="<sub-cmd>", required=True
+                )
+                for subcmd, kwargs in subcmds.items():
+                    subcmd_cmd_p.add_parser(
+                        subcmd,
+                        parents=[
+                            self.parsers[k]
+                            for k in self.cmd_arg_group_map[f"{cmd}|{subcmd}"]
+                        ],
+                        **kwargs,
+                    ).set_defaults(func=getattr(self.viv, cmd), subcmd=subcmd)
 
-        p_run.add_argument(
-            "-b", "--bin", help="console_script/script to invoke", metavar="<bin>"
-        )
+            else:
+                self._get_subcmd_parser(
+                    cmd_p,
+                    cmd,
+                    parents=[self.parsers.get(k) for k in self.cmd_arg_group_map[cmd]],
+                )
 
         if "--" in sys.argv:
             i = sys.argv.index("--")
-            args = parser.parse_args(sys.argv[1:i])
+            args = self.parser.parse_args(sys.argv[1:i])
             args.rest = sys.argv[i + 1 :]
         else:
-            args = parser.parse_args()
+            args = self.parser.parse_args()
             args.rest = []
 
+        self._validate_args(args)
         args.func(
             args,
         )
 
 
 def main() -> None:
     viv = Viv()
-    viv.cli()
+    Cli(viv).run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `viv-23.5a4/PKG-INFO` & `viv-23.5a5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,56 @@
-Metadata-Version: 2.1
-Name: viv
-Version: 23.5a4
-Summary: viv isn't venv
-License: MIT
-Author-email: Daylin Morgan <daylinmorgan@gmail.com>
-Requires-Python: >= 3.8
-Project-URL: homepage, https://github.com/daylinmorgan/viv
-Project-URL: repository, https://github.com/daylinmorgan/viv
-Description-Content-Type: text/markdown
-
-# viv
-
 <div align="center">
   <a href="https://github.com/daylinmorgan/viv">
     <img src="https://raw.githubusercontent.com/daylinmorgan/viv/main/assets/logo.svg" alt="Logo" width=500 >
   </a>
   <p align="center">
-  viv isn't venv
+  <h1> viv isn't venv </h1>
+  </p>
+  <div align="center">
+    <img
+      src="https://raw.githubusercontent.com/daylinmorgan/viv/main/docs/svgs/viv-help.svg"
+      alt="cli screenshot"
+      width="500"
+      >
+  </div>
+  <p align="center">
+    <a href="https://viv.dayl.in">Documentation</a>
   </p>
 </div>
 
+Try before you buy!
+```sh
+python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay -- "viv isn't venv\!"
+```
 ---
 
 `Viv` is a standalone dependency-free `venv` creator.
 
-These `venvs` can be identified by name or by their specification.
-In any case they will be re-used across scripts (and generated on-demand, if needed).
-
-**Importantly**, `viv` will also remove your user site directory.
-(view with: `python -m 'import site;print(site.USER_SITE)'`).
+`Viv`'s uncompromising insistence on portability means that it will always:
 
-`Viv`'s uncompromising insistence on portability means that it will always (1) only use the standard library (2) never exceed a single script.
+1. only use the standard library
+2. never exceed a single script.
 
 For that reason any usage of the `CLI` can be accomplished using a remote copy as seen in the below install command.
 
 ## Setup
 
 Run the below command to install `viv`.
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage install
+python3 <(curl -fsSL viv.dayl.in/viv.py) manage install
 ```
 
 To access `viv` from within scripts you should add it's location to your `PYTHONPATH`.
 By default `viv` will be installed to `$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can customize this with `--src`.
 
 ```sh
 export PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv"
 ```
 
-Advanced users may recognize that principally,
-the module just needs to be recognized at run time
-and the single script [`viv.py`](https://github.com/daylinmorgan/viv/blob/main/src/viv/viv.py) can be invoked directly for the CLI.
-How you accomplish these options is ultimately up to you but the above instructions can get you started.
-
 ### Pypi (Not Recommended)
 
 ```sh
 pip install viv
 ```
 
 Why is this *not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
@@ -77,28 +70,28 @@
 ```sh
 viv remove $(viv list -q)
 ```
 
 To remove `viv` all together you can use the included `purge` command:
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage purge
+python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge
 ```
 
 ## Additional Features
 
 An experimental feature of `viv` is generating shim's that leverage the principles of `viv`.
 These shims would operate similar to `pipx` in which you can specify a command line app to "install".
 
-*Note* that `--standalone` will auto-generate a code-golfed minified version of `viv` to accomplish the same basic task as using a local copy of `viv`.
-After generating this a standalone `shim` you can freely use this script across unix machines which have `python>3.8`.
+*Note* that `--standalone` will auto-generate a mini function version of `viv` to accomplish the same basic task as using a local copy of `viv`.
+After generating this standalone `shim` you can freely use this script across unix machines which have `python>3.8`.
 See [examples/black](https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of below command.
 
 ```sh
-python3 <(curl -fsSL gh.dayl.in/viv/viv.py) shim black -o ./black --standalone --freeze
+python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze
 ```
 
 ## Alternatives
 
 ### [pip-run](https://github.com/jaraco/pip-run)
 
 ```sh
@@ -128,8 +121,7 @@
 ```sh
 pipx (1.1.0)
 ├── argcomplete>=1.9.4 (2.1.1)
 ├── packaging>=20.0 (23.0)
 └── userpath>=1.6.0 (1.8.0)
     └── click (8.1.3)
 ```
-
```

#### html2text {}

```diff
@@ -1,55 +1,45 @@
-Metadata-Version: 2.1 Name: viv Version: 23.5a4 Summary: viv isn't venv
-License: MIT Author-email: Daylin Morgan
-gmail.com> Requires-Python: >= 3.8 Project-URL: homepage, https://github.com/
-daylinmorgan/viv Project-URL: repository, https://github.com/daylinmorgan/viv
-Description-Content-Type: text/markdown # viv
                                     [Logo]
-                                viv isn't venv
---- `Viv` is a standalone dependency-free `venv` creator. These `venvs` can be
-identified by name or by their specification. In any case they will be re-used
-across scripts (and generated on-demand, if needed). **Importantly**, `viv`
-will also remove your user site directory. (view with: `python -m 'import
-site;print(site.USER_SITE)'`). `Viv`'s uncompromising insistence on portability
-means that it will always (1) only use the standard library (2) never exceed a
-single script. For that reason any usage of the `CLI` can be accomplished using
-a remote copy as seen in the below install command. ## Setup Run the below
-command to install `viv`. ```sh python3 <(curl -fsSL gh.dayl.in/viv/viv.py)
-manage install ``` To access `viv` from within scripts you should add it's
-location to your `PYTHONPATH`. By default `viv` will be installed to
-`$XDG_DATA_HOME/viv` or `~/.local/share/viv` you can customize this with `--
-src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` Advanced
-users may recognize that principally, the module just needs to be recognized at
-run time and the single script [`viv.py`](https://github.com/daylinmorgan/viv/
-blob/main/src/viv/viv.py) can be invoked directly for the CLI. How you
-accomplish these options is ultimately up to you but the above instructions can
-get you started. ### Pypi (Not Recommended) ```sh pip install viv ``` Why is
-this *not recommended*? Mainly, because `viv` is all about hacking your
-`sys.path`. Placing it in it's own virtual environment or installing in a user
-site directory may complicate this endeavor. ## Usage In any python script with
-external dependencies you can add this line, to automate `vivenv` creation and
-installation of dependencies. ```python __import__("viv").use("click") ``` To
-remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
--q) ``` To remove `viv` all together you can use the included `purge` command:
-```sh python3 <(curl -fsSL gh.dayl.in/viv/viv.py) manage purge ``` ##
-Additional Features An experimental feature of `viv` is generating shim's that
-leverage the principles of `viv`. These shims would operate similar to `pipx`
-in which you can specify a command line app to "install". *Note* that `--
-standalone` will auto-generate a code-golfed minified version of `viv` to
-accomplish the same basic task as using a local copy of `viv`. After generating
-this a standalone `shim` you can freely use this script across unix machines
-which have `python>3.8`. See [examples/black](https://github.com/daylinmorgan/
-viv/blob/dev/examples/black) for output of below command. ```sh python3 <(curl
--fsSL gh.dayl.in/viv/viv.py) shim black -o ./black --standalone --freeze ``` ##
-Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
-(10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
-âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
-âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
-inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
-typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
-âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
-âââ more-itertools (9.1.0) âââ more-itertools>=8.3 (9.1.0)
-âââ packaging (23.0) âââ path>=15.1 (16.6.0) âââ pip>=19.3
-(23.0.1) âââ platformdirs (3.1.0) ``` ### [pipx](https://github.com/pypa/
-pipx/) ```sh pipx (1.1.0) âââ argcomplete>=1.9.4 (2.1.1) âââ
-packaging>=20.0 (23.0) âââ userpath>=1.6.0 (1.8.0) âââ click
-(8.1.3) ```
+                         ****** viv isn't venv ******
+                               [cli screenshot]
+                                 Documentation
+Try before you buy! ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay
+-- "viv isn't venv\!" ``` --- `Viv` is a standalone dependency-free `venv`
+creator. `Viv`'s uncompromising insistence on portability means that it will
+always: 1. only use the standard library 2. never exceed a single script. For
+that reason any usage of the `CLI` can be accomplished using a remote copy as
+seen in the below install command. ## Setup Run the below command to install
+`viv`. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage install ``` To
+access `viv` from within scripts you should add it's location to your
+`PYTHONPATH`. By default `viv` will be installed to `$XDG_DATA_HOME/viv` or
+`~/.local/share/viv` you can customize this with `--src`. ```sh export
+PYTHONPATH="$PYTHONPATH:$HOME/.local/share/viv" ``` ### Pypi (Not Recommended)
+```sh pip install viv ``` Why is this *not recommended*? Mainly, because `viv`
+is all about hacking your `sys.path`. Placing it in it's own virtual
+environment or installing in a user site directory may complicate this
+endeavor. ## Usage In any python script with external dependencies you can add
+this line, to automate `vivenv` creation and installation of dependencies.
+```python __import__("viv").use("click") ``` To remove all `vivenvs` you can
+use the below command: ```sh viv remove $(viv list -q) ``` To remove `viv` all
+together you can use the included `purge` command: ```sh python3 <(curl -fsSL
+viv.dayl.in/viv.py) manage purge ``` ## Additional Features An experimental
+feature of `viv` is generating shim's that leverage the principles of `viv`.
+These shims would operate similar to `pipx` in which you can specify a command
+line app to "install". *Note* that `--standalone` will auto-generate a mini
+function version of `viv` to accomplish the same basic task as using a local
+copy of `viv`. After generating this standalone `shim` you can freely use this
+script across unix machines which have `python>3.8`. See [examples/black]
+(https://github.com/daylinmorgan/viv/blob/dev/examples/black) for output of
+below command. ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) shim black -o ./
+black --standalone --freeze ``` ## Alternatives ### [pip-run](https://
+github.com/jaraco/pip-run) ```sh pip-run (10.0.5) âââ autocommand (2.2.2)
+âââ jaraco-context (4.3.0) âââ jaraco-functools (3.6.0) â
+âââ more-itertools (9.1.0) âââ jaraco-text (3.11.1) â âââ
+autocommand (2.2.2) â âââ inflect (6.0.2) â â âââ
+pydantic>=1.9.1 (1.10.5) â â âââ typing-extensions>=4.2.0 (4.5.0) â
+âââ jaraco-context>=4.1 (4.3.0) â âââ jaraco-functools (3.6.0)
+â â âââ more-itertools (9.1.0) â âââ more-itertools (9.1.0)
+âââ more-itertools>=8.3 (9.1.0) âââ packaging (23.0) âââ
+path>=15.1 (16.6.0) âââ pip>=19.3 (23.0.1) âââ platformdirs (3.1.0)
+``` ### [pipx](https://github.com/pypa/pipx/) ```sh pipx (1.1.0) âââ
+argcomplete>=1.9.4 (2.1.1) âââ packaging>=20.0 (23.0) âââ
+userpath>=1.6.0 (1.8.0) âââ click (8.1.3) ```
```

