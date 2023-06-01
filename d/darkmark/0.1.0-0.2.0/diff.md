# Comparing `tmp/darkmark-0.1.0.tar.gz` & `tmp/darkmark-0.2.0.tar.gz`

## Comparing `darkmark-0.1.0.tar` & `darkmark-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 darkmark-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 darkmark-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__about__.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__init__.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/__main__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/console.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/darkmark.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/replacer.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/cli/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 darkmark-0.1.0/darkmark/cli/common.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 darkmark-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 darkmark-0.1.0/tests/test_me.py
--rw-r--r--   0        0        0    17320 2020-02-02 00:00:00.000000 darkmark-0.1.0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 darkmark-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 darkmark-0.1.0/README.md
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 darkmark-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 darkmark-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 darkmark-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 darkmark-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/__about__.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/__init__.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/__main__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/console.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/darkmark.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/replacer.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/cli/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 darkmark-0.2.0/darkmark/cli/common.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 darkmark-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 darkmark-0.2.0/tests/test_me.py
+-rw-r--r--   0        0        0    17320 2020-02-02 00:00:00.000000 darkmark-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 darkmark-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 darkmark-0.2.0/README.md
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 darkmark-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 darkmark-0.2.0/PKG-INFO
```

### Comparing `darkmark-0.1.0/darkmark/darkmark.py` & `darkmark-0.2.0/darkmark/darkmark.py`

 * *Files identical despite different names*

### Comparing `darkmark-0.1.0/darkmark/replacer.py` & `darkmark-0.2.0/darkmark/replacer.py`

 * *Files identical despite different names*

### Comparing `darkmark-0.1.0/darkmark/cli/__init__.py` & `darkmark-0.2.0/darkmark/cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 import hashlib
 from pathlib import Path
 import time
 
 from rich.console import Console
+from rich.markdown import Markdown
 import typer
 
 from darkmark.cli.common import verbose_callback
 from darkmark.console import console
 from darkmark.darkmark import DarkMark
 
 from ..__about__ import __version__, name
@@ -23,72 +24,119 @@
 
 app = typer.Typer(
     name=name,
     help="run code blocks in markdown",
 )
 
 
+@app.command()
+def tui(ctx: typer.Context) -> None:
+    try:
+        from trogon import Trogon
+        from typer.main import get_group
+    except ImportError:
+        typer.echo("trogon not installed")
+        typer.echo(
+            "install markata with optional tui group to use tui `pip install 'darkmark[tui]'`"
+        )
+        return
+
+    Trogon(get_group(app), click_context=ctx).run()
+
+
 def get_hash(file, retries=5, sleep=1):
     try:
         new_hash = hashlib.md5(Path(file).read_text().encode()).hexdigest()
     except FileNotFoundError:
         if retries > 0:
             time.sleep(sleep)
             return get_hash(file, retries - 1, sleep)
         raise typer.Exit(1)
 
     return new_hash
 
 
-@app.callback(invoke_without_command=True)
-def main(
+def _run(file: Path, dry_run: bool, clear: bool, verbose: bool) -> None:
+    d = DarkMark(file)
+    d.clear()
+
+    if clear and dry_run:
+        Console().print(d.md)
+        return
+    elif clear:
+        d.write_text()
+        return
+
+    d.run_cells()
+
+    if dry_run:
+        md = Markdown(d.md)
+        Console().print(md)
+        return
+    else:
+        d.write_text()
+
+
+@app.command()
+def run(
     file: Path = typer.Argument(...),
     version: bool = typer.Option(
         False,
         "--version",
         callback=version_callback,  # is_eager=True
     ),
     debug: bool = typer.Option(None, "--debug", help="start with debug mode running"),
     dry_run: bool = typer.Option(False, help="run without saving"),
-    sexp: bool = typer.Option(False, help="print the sexp of the document"),
     clear: bool = typer.Option(False, help="clear existing darkmarks"),
     verbose: bool = typer.Option(
         False,
         callback=verbose_callback,
         help="show the log messages",
     ),
-    watch: bool = typer.Option(False, help="rerun when file changes"),
 ) -> None:
-    if watch:
-        old_hash = ""
-        while True:
-            if get_hash(file) != old_hash:
-                console.log("running")
-                console.log(f"old_hash: {old_hash}")
-                console.log(f"new_hash: {get_hash(file)}")
-                d = DarkMark(file)
-                d.clear()
-                d.run_cells()
-                d.write_text()
-                time.sleep(1)
-                old_hash = hashlib.md5(Path(file).read_text().encode()).hexdigest()
+    _run(file=file, dry_run=dry_run, clear=clear, verbose=verbose)
 
-    d = DarkMark(file)
-    d.clear()
 
-    if clear and dry_run:
-        Console().print(d.md)
-        return
-    elif clear:
-        d.write_text()
-        return
+@app.command()
+def watch(
+    file: Path = typer.Argument(...),
+    version: bool = typer.Option(
+        False,
+        "--version",
+        callback=version_callback,  # is_eager=True
+    ),
+    debug: bool = typer.Option(None, "--debug", help="start with debug mode running"),
+    dry_run: bool = typer.Option(False, help="run without saving"),
+    clear: bool = typer.Option(False, help="clear existing darkmarks"),
+    verbose: bool = typer.Option(
+        False,
+        callback=verbose_callback,
+        help="show the log messages",
+    ),
+) -> None:
+    old_hash = ""
+    while True:
+        if get_hash(file) != old_hash:
+            _run(file=file, dry_run=dry_run, clear=clear, verbose=verbose)
+            time.sleep(1)
+            old_hash = hashlib.md5(Path(file).read_text().encode()).hexdigest()
 
-    d.run_cells()
 
-    if sexp:
-        Console().print(d.sexp())
-        return
-    if dry_run:
-        Console().print(d.md)
-        return
-    else:
-        d.write_text()
+@app.command()
+def sexp(
+    file: Path = typer.Argument(...),
+    version: bool = typer.Option(
+        False,
+        "--version",
+        callback=version_callback,  # is_eager=True
+    ),
+    debug: bool = typer.Option(None, "--debug", help="start with debug mode running"),
+    clear: bool = typer.Option(False, help="clear existing darkmarks"),
+    verbose: bool = typer.Option(
+        False,
+        callback=verbose_callback,
+        help="show the log messages",
+    ),
+) -> None:
+    d = DarkMark(file)
+    Console().print(d.sexp())
+    return
```

### Comparing `darkmark-0.1.0/.gitignore` & `darkmark-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `darkmark-0.1.0/LICENSE.txt` & `darkmark-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `darkmark-0.1.0/pyproject.toml` & `darkmark-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -20,23 +20,29 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "typer",
-  "tree-sitter-languages",
+  "checksumdir",
   "ipython",
-  "rich",
   "pyflyby",
-  "checksumdir",
+  "rich",
+  "tree-sitter-languages",
+  "typer",
 ]
+
 dynamic = ["version"]
 
+[project.optional-dependencies]
+tui = [
+  "trogon",
+]
+
 [project.urls]
 Documentation = "https://github.com/unknown/darkmark#readme"
 Issues = "https://github.com/unknown/darkmark/issues"
 Source = "https://github.com/unknown/darkmark"
 
 [project.scripts]
 darkmark = "darkmark.cli:app"
@@ -78,7 +84,21 @@
 build-docs = "markata build"
 lint-test = [
  "format",
  "lint",
  "cov",
 ]
 test-lint = "lint-test"
+
+[tool.ruff]
+# E501 let black control line length errors
+ignore = [
+  "E501"
+]
+
+target-version = "py37"
+[tool.ruff.per-file-ignores]
+'tests/**/*.py' = ['S101']
+select = [
+  "A",
+  "E",
+]
```

### Comparing `darkmark-0.1.0/PKG-INFO` & `darkmark-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darkmark
-Version: 0.1.0
+Version: 0.2.0
 Summary: Execute codeblocks inside of markdown
 Project-URL: Documentation, https://github.com/unknown/darkmark#readme
 Project-URL: Issues, https://github.com/unknown/darkmark/issues
 Project-URL: Source, https://github.com/unknown/darkmark
 Author-email: "Waylon S. Walker" <waylon@waylonwalker.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -20,73 +20,56 @@
 Requires-Python: >=3.7
 Requires-Dist: checksumdir
 Requires-Dist: ipython
 Requires-Dist: pyflyby
 Requires-Dist: rich
 Requires-Dist: tree-sitter-languages
 Requires-Dist: typer
+Provides-Extra: tui
+Requires-Dist: trogon; extra == 'tui'
 Description-Content-Type: text/markdown
 
 # DarkMark
 
 <img src="https://user-images.githubusercontent.com/22648375/216847624-d4dbc93b-76d7-4d2c-ba71-fa58b4b331e5.png" alt="darkmark" width="250" align=right>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/darkmark.svg)](https://pypi.org/project/darkmark)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/darkmark.svg)](https://pypi.org/project/darkmark)
 
 Runs codeblocks marked with the darkmark, and inserts the results.  
 
 DarkMark uses tree-sitter to identify codeblocks.  Currently it only supports python codeblocks in markdown files and runs them with ipython.  Handy for writing docs/blog posts so you can stay right in your markdown editor of choice and get the outputs in line.  No need to jump into a whole other tool just to do live execution.
 
------
+---
 
 ## Installation
 
 ```console
 pip install darkmark
 ```
 
 ```console
 ❯ darkmark --help
 
- Usage: darkmark [OPTIONS] FILE COMMAND [ARGS]...
+ Usage: darkmark [OPTIONS] COMMAND [ARGS]...
 
  run code blocks in markdown
 
-╭─ Arguments ────────────────────────────────────────────────────────────────────────────╮
-│ *    file      PATH  [default: None] [required]                                        │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Options ──────────────────────────────────────────────────────────────────────────────╮
-│ --version                                                                              │
-│ --debug                                                        start with debug mode   │
-│                                                                running                 │
-│ --dry-run               --no-dry-run                           run without saving      │
-│                                                                [default: no-dry-run]   │
-│ --sexp                  --no-sexp                              print the sexp of the   │
-│                                                                document                │
-│                                                                [default: no-sexp]      │
-│ --clear                 --no-clear                             clear existing          │
-│                                                                darkmarks               │
-│                                                                [default: no-clear]     │
-│ --verbose               --no-verbose                           show the log messages   │
-│                                                                [default: no-verbose]   │
-│ --watch                 --no-watch                             rerun when file changes │
-│                                                                [default: no-watch]     │
-│ --install-completion                    [bash|zsh|fish|powers  Install completion for  │
-│                                         hell|pwsh]             the specified shell.    │
-│                                                                [default: None]         │
-│ --show-completion                       [bash|zsh|fish|powers  Show completion for the │
-│                                         hell|pwsh]             specified shell, to     │
-│                                                                copy it or customize    │
-│                                                                the installation.       │
-│                                                                [default: None]         │
-│ --help                                                         Show this message and   │
-│                                                                exit.                   │
-╰────────────────────────────────────────────────────────────────────────────────────────╯
-
+╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ --install-completion        [bash|zsh|fish|powershell|pwsh]  Install completion for the specified shell.       │
+│                                                              [default: None]                                   │
+│ --show-completion           [bash|zsh|fish|powershell|pwsh]  Show completion for the specified shell, to copy  │
+│                                                              it or customize the installation.                 │
+│                                                              [default: None]                                   │
+│ --help                                                       Show this message and exit.                       │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ run                                                                                                            │
+│ sexp                                                                                                           │
+│ tui                                                                                                            │
+│ watch                                                                                                          │
+╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 
 ```
 
 ## Usage
 
 Mark your codeblocks with the darkmark.
 
@@ -113,16 +96,14 @@
 
 Currently the only language supported is python.
 
 * python
 
 ## Example
 
-Running `darkmark --watch <file.md>` updates the file on save.
+Running `darkmark watch <file.md>` updates the file on save.
 
 [darkmark.webm](https://user-images.githubusercontent.com/22648375/216849738-12897dfc-3e2b-4e5b-9b6d-cbb29c3ae782.webm)
 
-
-
 ## License
 
 `darkmark` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

