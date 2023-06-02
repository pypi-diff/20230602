# Comparing `tmp/click_extra-4.2.0.tar.gz` & `tmp/click_extra-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.2.0.tar", max compression
+gzip compressed data, was "click_extra-4.3.0.tar", max compression
```

## Comparing `click_extra-4.2.0.tar` & `click_extra-4.3.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6030 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/__init__.py
--rw-r--r--   0        0        0    27870 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/colorize.py
--rw-r--r--   0        0        0    14955 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/commands.py
--rw-r--r--   0        0        0    29591 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/config.py
--rw-r--r--   0        0        0     3973 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6380 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11543 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/logging.py
--rw-r--r--   0        0        0     8515 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/parameters.py
--rw-r--r--   0        0        0    14061 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/py.typed
--rw-r--r--   0        0        0     7672 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4139 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/run.py
--rw-r--r--   0        0        0     6094 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5718 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2534 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/telemetry.py
--rw-r--r--   0        0        0      770 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    14766 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    17759 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    14048 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    21404 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7259 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0     7814 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0     9733 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8377 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0     7062 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_run.py
--rw-r--r--   0        0        0    14284 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3153 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     3531 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     4585 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2385 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/timer.py
--rw-r--r--   0        0        0     7098 2023-05-24 07:54:57.913645 click_extra-4.2.0/click_extra/version.py
--rw-r--r--   0        0        0     6950 2023-05-24 07:54:57.921645 click_extra-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     6637 2023-05-24 07:54:57.921645 click_extra-4.2.0/readme.md
--rw-r--r--   0        0        0     9681 1970-01-01 00:00:00.000000 click_extra-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6143 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    27870 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    14959 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/commands.py
+-rw-r--r--   0        0        0    15734 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/config.py
+-rw-r--r--   0        0        0     3996 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6402 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11542 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/logging.py
+-rw-r--r--   0        0        0    22569 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    14061 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7671 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     6113 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5718 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2534 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23502 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11926 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    17800 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    12945 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    16166 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7238 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    14323 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0     9733 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8377 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14284 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3153 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8215 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3530 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     4585 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2385 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/timer.py
+-rw-r--r--   0        0        0     7098 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/version.py
+-rw-r--r--   0        0        0     6948 2023-06-02 16:27:11.934412 click_extra-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6640 2023-06-02 16:27:11.934412 click_extra-4.3.0/readme.md
+-rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 click_extra-4.3.0/PKG-INFO
```

### Comparing `click_extra-4.2.0/click_extra/__init__.py` & `click_extra-4.3.0/click_extra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.2.0"
+__version__ = "4.3.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -55,47 +55,52 @@
 from click import *  # noqa: E402, F403
 from click.core import ParameterSource  # noqa: E402, F401
 from cloup import *  # type: ignore[no-redef] # noqa: E402, F403
 
 from .colorize import (  # noqa: I001, E402, F401
     ColorOption,
     HelpExtraFormatter,
-    HelpOption,
     HelpExtraTheme,
+    HelpOption,
 )
 from .commands import (  # noqa: I001, E402, F401
     ExtraCommand,
     ExtraContext,
     ExtraGroup,
 )
-from .config import ConfigOption, ShowParamsOption  # noqa: I001, E402, F401
+from .config import ConfigOption  # noqa: I001, E402, F401
 from .decorators import (  # type: ignore[no-redef] # noqa: I001, E402, F401
     color_option,
     command,  # noqa: E402
     config_option,
     extra_command,
     extra_group,
     group,  # noqa: E402
-    help_option,  # type: ignore[has-type]
+    help_option,
     show_params_option,
     table_format_option,
     telemetry_option,
     timer_option,
     verbosity_option,
     version_option,
 )
 from .logging import (  # noqa: I001, E402, F401
-    VerbosityOption,
     ExtraLogFormatter,
     ExtraLogHandler,
+    VerbosityOption,
     extra_basic_config,
 )
-from .parameters import ExtraOption  # noqa: I001, E402, F401
+from .parameters import (  # noqa: I001, E402, F401
+    ExtraOption,
+    ParamStructure,
+    ShowParamsOption,
+)
 from .tabulate import TableFormatOption  # noqa: I001, E402, F401
 from .telemetry import TelemetryOption  # noqa: I001, E402, F401
+from .testing import ExtraCliRunner  # noqa: I001, E402, F401
 from .timer import TimerOption  # noqa: I001, E402, F401
 from .version import VersionOption  # noqa: I001, E402, F401
 
 __all__ = [  # noqa: F405
     "Abort",
     "Argument",
     "argument",
@@ -131,14 +136,15 @@
     "dir_path",
     "echo",
     "echo_via_pager",
     "edit",
     "extra_basic_config",
     "extra_command",
     "extra_group",
+    "ExtraCliRunner",
     "ExtraCommand",
     "ExtraContext",
     "ExtraGroup",
     "ExtraLogFormatter",
     "ExtraLogHandler",
     "ExtraOption",
     "File",
@@ -173,14 +179,15 @@
     "option",
     "option_group",
     "OptionGroup",
     "OptionGroupMixin",
     "OptionParser",
     "Parameter",
     "ParameterSource",
+    "ParamStructure",
     "ParamType",
     "pass_context",
     "pass_obj",
     "password_option",
     "Path",
     "path",
     "pause",
```

### Comparing `click_extra-4.2.0/click_extra/colorize.py` & `click_extra-4.3.0/click_extra/colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,33 +18,33 @@
 from __future__ import annotations
 
 import os
 import re
 from configparser import RawConfigParser
 from gettext import gettext as _
 from operator import getitem
-from typing import NamedTuple, Sequence, cast, Optional
+from typing import NamedTuple, Optional, Sequence, cast
 
+import click
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from cloup._util import identity
-from cloup.styling import IStyle, Color
+from cloup.styling import Color, IStyle
 from cloup.typing import MISSING, Possibly
-import click
 
 from . import (
     Choice,
     Context,
     HelpFormatter,
     Parameter,
     ParameterSource,
     Style,
+    cache,
     echo,
     get_current_context,
-    cache,
 )
 from .parameters import ExtraOption
 
 
 class HelpExtraTheme(NamedTuple):
     """Extends ``cloup.HelpTheme`` with extra properties and ``logging.levels``.
```

### Comparing `click_extra-4.2.0/click_extra/commands.py` & `click_extra-4.3.0/click_extra/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,19 +25,24 @@
 import logging
 from typing import Any, Dict
 
 import click
 import cloup
 
 from . import Command, Group
-from .colorize import ExtraHelpColorsMixin
-from .parameters import ExtraOption, all_envvars, normalize_envvar, search_params
-from .colorize import ColorOption, HelpOption
-from .config import ConfigOption, ShowParamsOption
+from .colorize import ColorOption, ExtraHelpColorsMixin, HelpOption
+from .config import ConfigOption
 from .logging import VerbosityOption
+from .parameters import (
+    ExtraOption,
+    ShowParamsOption,
+    all_envvars,
+    normalize_envvar,
+    search_params,
+)
 from .timer import TimerOption
 from .version import VersionOption
 
 
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
     ``meta`` property at instanciation."""
```

### Comparing `click_extra-4.2.0/click_extra/decorators.py` & `click_extra-4.3.0/click_extra/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 from functools import wraps
 
 import cloup
 
 from .colorize import ColorOption, HelpOption
 from .commands import ExtraCommand, ExtraGroup, default_extra_params
-from .config import ConfigOption, ShowParamsOption
+from .config import ConfigOption
 from .logging import VerbosityOption
+from .parameters import ShowParamsOption
 from .tabulate import TableFormatOption
 from .telemetry import TelemetryOption
 from .timer import TimerOption
 from .version import VersionOption
 
 
 def allow_missing_parenthesis(dec_factory):
```

### Comparing `click_extra-4.2.0/click_extra/docs_update.py` & `click_extra-4.3.0/click_extra/docs_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
 
     # Wrap the Mermaid code into a MyST block.
     return "\n".join(
         (
             # Use attributes blocks extension to add a title.
             ('{caption="' f"`click_extra.platforms.{graph_id}` - {description}" '"}'),
             "```mermaid",
+            ":zoom:",
             "flowchart",
             indent("\n".join(sorted(subgraphs)), INDENT),
             "```",
         )
     )
```

### Comparing `click_extra-4.2.0/click_extra/logging.py` & `click_extra-4.3.0/click_extra/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Logging utilities."""
 
 from __future__ import annotations
 
 import logging
+import sys
+from collections.abc import Generator, Iterable, Sequence
+from gettext import gettext as _
 from logging import (
-    Logger,
     WARNING,
-    _levelToName,
     Formatter,
     Handler,
+    Logger,
     LogRecord,
+    _levelToName,
 )
-import sys
-from collections.abc import Generator, Iterable, Sequence
-from gettext import gettext as _
 from typing import Literal, TypeVar
 
 import click
 
 from . import Choice
 from .colorize import default_theme
 from .parameters import ExtraOption
 
-
 _original_get_logger = logging.getLogger
 
 
 def _patched_get_logger(name: str | None = None) -> Logger:
     """Patch ``logging.getLogger`` to return the right root logger object.
 
     .. warning::
```

### Comparing `click_extra-4.2.0/click_extra/platforms.py` & `click_extra-4.3.0/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/pygments.py` & `click_extra-4.3.0/click_extra/pygments.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 """Helpers and utilities to allow Pygments to parse and render ANSI codes."""
 
 from __future__ import annotations
 
 from pygments import lexers
 from pygments.filter import Filter
 from pygments.filters import TokenMergeFilter
-from pygments.formatters import HtmlFormatter
 from pygments.formatter import _lookup_style  # type: ignore[attr-defined]
+from pygments.formatters import HtmlFormatter
 from pygments.lexer import Lexer, LexerMeta
 from pygments.lexers.algebra import GAPConsoleLexer
 from pygments.lexers.dylan import DylanConsoleLexer
 from pygments.lexers.erlang import ElixirConsoleLexer, ErlangShellLexer
 from pygments.lexers.julia import JuliaConsoleLexer
 from pygments.lexers.matlab import MatlabSessionLexer
 from pygments.lexers.php import PsyshConsoleLexer
@@ -39,15 +39,14 @@
 from pygments.token import Generic, string_to_tokentype
 from pygments_ansi_color import (
     AnsiColorLexer,
     ExtendedColorHtmlFormatterMixin,
     color_tokens,
 )
 
-
 DEFAULT_TOKEN_TYPE = Generic.Output
 """Default Pygments' token type to render with ANSI support.
 
 We defaults to ``Generic.Output`` tokens, as this is the token type used by all REPL-
 like and terminal lexers.
 """
```

### Comparing `click_extra-4.2.0/click_extra/sphinx.py` & `click_extra-4.3.0/click_extra/sphinx.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,41 +124,38 @@
         - ``.. click:example::``
         - ``.. click:run::``
 
     .. danger::
         This function activates lots of monkey-patches:
 
         - ``sphinx.highlighting.PygmentsBridge`` is updated to set its default HTML
-        formatter to an ANSI capable one for the whole Sphinx app.
+          formatter to an ANSI capable one for the whole Sphinx app.
 
         - ``click_compat_hack`` to `bypass old Python 2.x in pallets-sphinx-themes
-        <#click_extra.sphinx.click_compat_hack>`.
+          <#click_extra.sphinx.click_compat_hack>`.
 
         - ``pallets_sphinx_themes.themes.click.domain.ViewList`` is
-        `patched to force an ANSI lexer on the rST code block
-        <#click_extra.sphinx.PatchedViewList>`_.
+          `patched to force an ANSI lexer on the rST code block
+          <#click_extra.sphinx.PatchedViewList>`_.
+
+        - ``pallets_sphinx_themes.themes.click.domain.ExampleRunner`` is replaced with
+          ``click_extra.testing.ExtraCliRunner`` to have full control of
+          contextual color settings by the way of the ``color`` parameter. It also
+          produce unfiltered ANSI codes so that the other ``PatchedViewList``
+          monkey-patch can do its job and render colors in the HTML output.
     """
     # Set Sphinx's default HTML formatter to an ANSI capable one.
     PygmentsBridge.html_formatter = AnsiHtmlFormatter
 
     with click_compat_hack:
         from pallets_sphinx_themes.themes.click import domain
 
         domain.ViewList = PatchedViewList
 
-        ####################################
-        #  pallets_sphinx_themes Patch #2  #
-        ####################################
-        # Replace the call to default ``CliRunner.invoke`` with a call to click_extra
-        # own version which is sensible to contextual color settings and output
-        # unfiltered ANSI codes.
-        # Fixes: <insert upstream bug report here>
-
         # Brutal, but effective.
         # Alternative patching methods: https://stackoverflow.com/a/38928265
         domain.ExampleRunner.__bases__ = (ExtraCliRunner,)
-
         # Force color rendering in ``invoke`` calls.
         domain.ExampleRunner.force_color = True
 
         # Register directives to Sphinx.
         domain.setup(app)
```

### Comparing `click_extra-4.2.0/click_extra/tabulate.py` & `click_extra-4.3.0/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/telemetry.py` & `click_extra-4.3.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/tests/__init__.py` & `click_extra-4.3.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/tests/conftest.py` & `click_extra-4.3.0/click_extra/tests/conftest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,33 +14,30 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Fixtures, configuration and helpers for tests."""
 
 from __future__ import annotations
 
 import os
-from functools import partial
+from configparser import RawConfigParser  # noqa: E402
 from pathlib import Path
 from textwrap import dedent
-from typing import IO, Any, Sequence
 
 import click
 import click.testing
 import cloup
 import pytest
-from boltons.strutils import strip_ansi
-from boltons.tbutils import ExceptionInfo
 
 from ..decorators import command, extra_command, extra_group, group
 from ..platforms import is_linux, is_macos, is_windows
-from ..run import EnvVars, args_cleanup, print_cli_output
+from ..testing import ExtraCliRunner
 
-DESTRUCTIVE_MODE = bool(
-    os.environ.get("DESTRUCTIVE_TESTS", False) not in {True, 1, "True", "true", "1"}
-)
+DESTRUCTIVE_MODE = RawConfigParser.BOOLEAN_STATES[
+    str(os.environ.get("DESTRUCTIVE_TESTS", False)).lower()
+]
 """Pre-computed boolean flag indicating if destructive mode is activated by the presence
 of a ``DESTRUCTIVE_TESTS`` environment variable set to ``True``."""
 
 
 destructive = pytest.mark.skipif(DESTRUCTIVE_MODE, reason="destructive test")
 """Pytest mark to skip a test unless destructive mode is allowed.
 
@@ -86,109 +83,26 @@
 
 See:
 - https://github.com/pallets/click/issues/2111
 - https://github.com/pallets/click/issues/2110
 """
 
 
-class ExtraCliRunner(click.testing.CliRunner):
-    force_color: bool = False
-    """Add a ``force_color`` boolean flag on the class to allow for overriding of the
-    ``color`` parameter in ``invoke``.
-
-    This is only used to initialize the CliRunner in the context of Sphinx
-    documentation.
-    """
-
-    def invoke(
-        self,
-        cli: click.core.BaseCommand,
-        args: str | Sequence[str] | None = None,
-        input: str | bytes | IO | None = None,
-        env: EnvVars | None = None,
-        catch_exceptions: bool = True,
-        color: bool = False,
-        **extra: Any,
-    ) -> click.testing.Result:
-        if self.force_color:
-            color = True
-
-        result = super().invoke(
-            cli=cli,
-            args=args,
-            input=input,
-            env=env,
-            catch_exceptions=catch_exceptions,
-            color=color,
-            **extra,
-        )
-
-        if result.exception:
-            print(ExceptionInfo.from_exc_info(*result.exc_info).get_formatted())
-
-        return result
-
-
 @pytest.fixture
-def runner():
-    runner = ExtraCliRunner(mix_stderr=False)
+def extra_runner():
+    """Runner fixture for ``click.testing.ExtraCliRunner``."""
+    runner = ExtraCliRunner()
     with runner.isolated_filesystem():
         yield runner
 
 
 @pytest.fixture
-def invoke(runner, monkeypatch):
-    """Executes Click's CLI, print output and return results.
-
-    If ``color=False`` both ``<stdout>`` and ``<stderr>`` are stripped out of ANSI
-    codes.
-
-    Adds a special case in the form of ``color="forced"`` parameter, which allows
-    colored output to be kept, while forcing the initialization of
-    ``Context.color = True``. This is not `allowed in current implementation
-    <https://github.com/pallets/click/issues/2110>`_ of
-    ``click.testing.CliRunner.invoke()``.
-    """
-
-    def _run(cli, *args, env: EnvVars | None = None, color=None):
-        # We allow for nested iterables and None values as args for
-        # convenience. We just need to flatten and filters them out.
-        args = args_cleanup(args)
-
-        # Extra parameters passed to the invoked command's ``main()`` constructor.
-        extra = {}
-        if color == "forced":
-            extra["color"] = True
-
-        with monkeypatch.context() as patch:
-            # Monkeypatch the original command's ``main()`` call to pass extra
-            # parameter for Context initialization. Because we cannot simply add
-            # ``color`` to ``**extra``.
-            patch.setattr(cli, "main", partial(cli.main, **extra))
-
-            result = runner.invoke(cli=cli, args=args, env=env, color=bool(color))
-
-        # Force stripping of all colors from results.
-        if color is False:
-            result.stdout_bytes = strip_ansi(result.stdout_bytes)
-            result.stderr_bytes = strip_ansi(result.stderr_bytes)
-
-        print_cli_output(
-            [runner.get_default_prog_name(cli)] + list(args),
-            result.output,
-            result.stderr,
-            result.exit_code,
-        )
-
-        if result.exception:
-            print(ExceptionInfo.from_exc_info(*result.exc_info).get_formatted())
-
-        return result
-
-    return _run
+def invoke(extra_runner):
+    """Invoke fixture shorthand for ``click.testing.ExtraCliRunner.invoke``."""
+    return extra_runner.invoke
 
 
 # XXX Support for decorator without parenthesis in Cloup has been reported upstream:
 # https://github.com/janluke/cloup/issues/127
 skip_naked = pytest.mark.skip(reason="Naked decorator not supported yet.")
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_colorize.py` & `click_extra-4.3.0/click_extra/tests/test_colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
+import logging
 import re
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
 from boltons.strutils import strip_ansi
 from pytest_cases import parametrize
-import logging
+
 from .. import HelpTheme, Style, argument, echo, option, option_group, secho, style
 from ..colorize import (
     HelpExtraFormatter,
     HelpExtraTheme,
     default_theme,
     highlight,
 )
@@ -39,18 +40,18 @@
     extra_group,
     help_option,
     verbosity_option,
 )
 from ..logging import LOG_LEVELS
 from .conftest import (
     command_decorators,
-    default_debug_colored_log_start,
     default_debug_colored_log_end,
-    default_debug_uncolored_log_start,
+    default_debug_colored_log_start,
     default_debug_uncolored_log_end,
+    default_debug_uncolored_log_start,
     default_options_colored_help,
     skip_windows_colors,
 )
 
 
 def test_theme_definition():
     """Ensure we do not leave any property we would have inherited from cloup and
@@ -191,26 +192,26 @@
         r"\x1b\[94m\x1b\[1m\x1b\[4mExtra commands:\x1b\[0m\n"
         r"  \x1b\[36mcommand3\x1b\[0m\n"
         r"  \x1b\[36mcommand4\x1b\[0m  \x1b\[93m\x1b\[1m\(Deprecated\)\x1b\[0m\n"
     )
 
     result = invoke(color_cli1, "--help", color=True)
     assert result.exit_code == 0
-    assert re.fullmatch(help_screen, result.output)
+    assert re.fullmatch(help_screen, result.stdout)
     assert not result.stderr
 
     result = invoke(color_cli1, "-h", color=True)
     assert result.exit_code == 0
-    assert re.fullmatch(help_screen, result.output)
+    assert re.fullmatch(help_screen, result.stdout)
     assert not result.stderr
 
     # CLI main group is invoked before sub-command.
     result = invoke(color_cli1, "command1", "--help", color=True)
     assert result.exit_code == 0
-    assert result.output == (
+    assert result.stdout == (
         "It works!\n"
         "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcolor-cli1 command1\x1b[0m"
         " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
         "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
@@ -220,15 +221,15 @@
         "  \x1b[36m-h\x1b[0m, \x1b[36m--help\x1b[0m  Show this message and exit.\n"
     )
     assert not result.stderr
 
     # Standalone call to command: CLI main group is skipped.
     result = invoke(command1, "--help", color=True)
     assert result.exit_code == 0
-    assert result.output == (
+    assert result.stdout == (
         "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcommand1\x1b[0m"
         " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
         "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
         "  [\x1b[36mMY_ARG\x1b[0m]...  Argument supports help.\n"
@@ -366,17 +367,20 @@
 
     # Params always overrides env's expectations.
     expecting_colors = env_expect_colors
     if param:
         expecting_colors = param_expect_colors
 
     if expecting_colors:
-        assert result.output == "\x1b[33mIt works!\x1b[0m\n"
+        assert result.stdout == "\x1b[33mIt works!\x1b[0m\n"
     else:
-        assert result.output == "It works!\n"
+        assert result.stdout == "It works!\n"
+
+
+# TODO: test with  configuration file
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
     "param, expecting_colors",
     (
         ("--color", True),
@@ -399,15 +403,15 @@
         print(style("print() bypass Click.", fg="blue"))
         secho("Done.", fg="green")
 
     result = invoke(color_cli8, param, "--verbosity", "DEBUG", "command1", color=True)
 
     assert result.exit_code == 0
     if expecting_colors:
-        assert result.output == (
+        assert result.stdout == (
             "\x1b[33mIt works!\x1b[0m\n"
             "\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m\n"
             "\x1b[35mRun command #1.\x1b[0m\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "\x1b[32mDone.\x1b[0m\n"
         )
         assert re.fullmatch(
@@ -416,15 +420,15 @@
                 r"\x1b\[33mwarning\x1b\[0m: Processing...\n"
                 rf"{default_debug_colored_log_end}"
             ),
             result.stderr,
         )
 
     else:
-        assert result.output == (
+        assert result.stdout == (
             "It works!\n"
             "Art\n"
             "Run command #1.\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "Done.\n"
         )
         assert re.fullmatch(
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_commands.py` & `click_extra-4.3.0/click_extra/tests/test_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
 from pytest_cases import fixture
 
-from .. import echo, option, option_group, pass_context
+from .. import echo, option, option_group
 from ..decorators import extra_command, extra_group
 from .conftest import (
-    default_debug_uncolored_log_start,
     default_debug_uncolored_log_end,
+    default_debug_uncolored_log_start,
     default_options_colored_help,
     default_options_uncolored_help,
     skip_windows_colors,
 )
 
 
 def test_module_root_declarations():
@@ -252,16 +252,16 @@
     assert not result.stderr
 
 
 def test_integrated_version_value(invoke, all_command_cli):
     result = invoke(all_command_cli, "--version", color=False)
     assert result.exit_code == 0
 
-    regex_output = r"command-cli1, version 2021.10.08\n{'.+'}\n"
-    assert re.fullmatch(regex_output, result.output)
+    regex_stdout = r"command-cli1, version 2021.10.08\n{'.+'}\n"
+    assert re.fullmatch(regex_stdout, result.stdout)
 
     assert not result.stderr
 
 
 def test_no_option_leaks_between_subcommands(invoke):
     """As reported in https://github.com/kdeldycke/click-extra/issues/489."""
 
@@ -280,15 +280,15 @@
         echo("Run bar...")
 
     cli.add_command(foo)
     cli.add_command(bar)
 
     result = invoke(cli, "--help", color=False)
     assert result.exit_code == 0
-    assert result.output == dedent(
+    assert result.stdout == dedent(
         """\
         Usage: cli [OPTIONS] COMMAND [ARGS]...
 
         Options:
           --help  Show this message and exit.
 
         Commands:
@@ -366,48 +366,14 @@
         ),
         result.stdout,
     )
     assert "It works!" not in result.stdout
     assert not result.stderr
 
 
-def test_raw_args(invoke):
-    """Raw args are expected to be scoped in subcommands."""
-
-    @extra_group
-    @option("--dummy-flag/--no-flag")
-    @pass_context
-    def my_cli(ctx, dummy_flag):
-        echo("-- Group output --")
-        echo(f"dummy_flag is {dummy_flag!r}")
-        echo(f"Raw parameters: {ctx.meta.get('click_extra.raw_args', [])}")
-
-    @my_cli.command()
-    @pass_context
-    @option("--int-param", type=int, default=10)
-    def subcommand(ctx, int_param):
-        echo("-- Subcommand output --")
-        echo(f"int_parameter is {int_param!r}")
-        echo(f"Raw parameters: {ctx.meta.get('click_extra.raw_args', [])}")
-
-    result = invoke(my_cli, "--dummy-flag", "subcommand", "--int-param", "33")
-    assert result.exit_code == 0
-    assert not result.stderr
-    assert result.output == dedent(
-        """\
-        -- Group output --
-        dummy_flag is True
-        Raw parameters: ['--dummy-flag', 'subcommand', '--int-param', '33']
-        -- Subcommand output --
-        int_parameter is 33
-        Raw parameters: ['--int-param', '33']
-        """
-    )
-
-
 @pytest.mark.parametrize(
     "cmd_decorator, ctx_settings, expected_help",
     (
         # Click does not show all envvar in the help screen by default, unless
         # specifficaly set on an option.
         (
             click.command,
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_config.py` & `click_extra-4.3.0/click_extra/tests/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import re
-from os.path import sep
 from pathlib import Path
 
 import click
 import pytest
 from boltons.pathutils import shrinkuser
 from pytest_cases import fixture, parametrize
-from tabulate import tabulate
 
 from .. import (
     BOOL,
     FLOAT,
     INT,
     STRING,
     UNPROCESSED,
@@ -41,21 +39,20 @@
     Tuple,
     argument,
     echo,
     get_app_dir,
     option,
 )
 from ..colorize import escape_for_help_sceen
-from ..config import ConfigOption, ShowParamsOption
-from ..decorators import config_option, extra_command, extra_group, show_params_option
+from ..config import ConfigOption
+from ..decorators import config_option, extra_group
 from ..parameters import search_params
 from .conftest import (
-    command_decorators,
-    default_debug_uncolored_log_start,
     default_debug_uncolored_log_end,
+    default_debug_uncolored_log_start,
 )
 
 DUMMY_TOML_FILE = """
     # Comment
 
     top_level_param             = "to_ignore"
 
@@ -221,64 +218,65 @@
         "stderr is not supposed to be filled with debug logs, but it seems there is a "
         "leak somewhere in our logging system"
     ),
 )
 def test_unset_conf_no_message(invoke, simple_config_cli):
     result = invoke(simple_config_cli, "default-command")
     assert result.exit_code == 0
-    assert result.output == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
     assert not result.stderr
+    assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
 
 
 def test_unset_conf_debug_message(invoke, simple_config_cli):
     result = invoke(
         simple_config_cli, "--verbosity", "DEBUG", "default-command", color=False
     )
     assert result.exit_code == 0
-    assert result.output == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
+    assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
     assert re.fullmatch(
         default_debug_uncolored_log_start + default_debug_uncolored_log_end,
         result.stderr,
     )
 
 
 def test_conf_default_path(invoke, simple_config_cli):
     result = invoke(simple_config_cli, "--help", color=False)
     assert result.exit_code == 0
+    assert not result.stderr
 
     # OS-specific path.
     default_path = shrinkuser(
         Path(get_app_dir("config-cli1")) / "*.{toml,yaml,yml,json,ini,xml}"
     )
 
     # Make path string compatible with regexp.
     assert re.search(
         rf"\[default:\s+{escape_for_help_sceen(str(default_path))}\]",
-        result.output,
+        result.stdout,
     )
 
 
 def test_conf_not_exist(invoke, simple_config_cli):
     conf_path = Path("dummy.toml")
     result = invoke(
         simple_config_cli, "--config", str(conf_path), "default-command", color=False
     )
     assert result.exit_code == 2
-    assert not result.output
+    assert not result.stdout
     assert f"Load configuration matching {conf_path}\n" in result.stderr
     assert "critical: No configuration file found.\n" in result.stderr
 
 
 def test_conf_not_file(invoke, simple_config_cli):
     conf_path = Path().parent
     result = invoke(
         simple_config_cli, "--config", str(conf_path), "default-command", color=False
     )
     assert result.exit_code == 2
-    assert not result.output
+    assert not result.stdout
 
     assert f"Load configuration matching {conf_path}\n" in result.stderr
     assert "critical: No configuration file found.\n" in result.stderr
 
 
 @parametrize("option_decorator", (config_option, config_option()))
 def test_conf_auto_types(invoke, create_config, option_decorator):
@@ -347,15 +345,15 @@
         str(conf_path),
         "random_file1",
         "random_file2",
         color=False,
     )
 
     assert result.exit_code == 0
-    assert result.output == "Works!\n"
+    assert result.stdout == "Works!\n"
 
     cli_config_option = search_params(config_cli2.params, ConfigOption)
     assert cli_config_option.params_template == {
         "config-cli2": {
             "flag1": None,
             "flag2": None,
             "str_param1": None,
@@ -509,15 +507,15 @@
         result = invoke(
             simple_config_cli,
             "default-command",
             color=False,
             env={"CONFIG_TEST_CLI_CONFIG": str(conf_path)},
         )
         assert result.exit_code == 0
-        assert result.output == (
+        assert result.stdout == (
             "dummy_flag = True\nmy_list = ('pip', 'npm', 'gem')\nint_parameter = 3\n"
         )
         # Debug level has been activated by configuration file.
         assert result.stderr == (
             f"Load configuration matching {conf_path.resolve()}\n"
             "debug: Verbosity set to DEBUG.\n"
         )
@@ -546,205 +544,11 @@
             "--my-list",
             "wow",
             "default-command",
             "--int-param",
             "15",
         )
         assert result.exit_code == 0
-        assert result.output == (
+        assert result.stdout == (
             "dummy_flag = False\nmy_list = ('super', 'wow')\nint_parameter = 15\n"
         )
         assert result.stderr == f"Load configuration matching {conf_path.resolve()}\n"
-
-
-@parametrize(
-    "cmd_decorator",
-    # Skip click extra's commands, as show_params option is already part of the default.
-    command_decorators(no_groups=True, no_extra=True),
-)
-@parametrize("option_decorator", (show_params_option, show_params_option()))
-def test_standalone_show_params_option(invoke, cmd_decorator, option_decorator):
-    @cmd_decorator
-    @option_decorator
-    def show_params():
-        echo("It works!")
-
-    result = invoke(show_params, "--show-params")
-    assert result.exit_code == 0
-
-    table = [
-        (
-            "show-params.show_params",
-            "click_extra.config.ShowParamsOption",
-            "--show-params",
-            "bool",
-            "",
-            "✘",
-            "",
-            False,
-            "",
-            "COMMANDLINE",
-        ),
-    ]
-    output = tabulate(
-        table,
-        headers=ShowParamsOption.TABLE_HEADERS,
-        tablefmt="rounded_outline",
-        disable_numparse=True,
-    )
-    assert result.output == f"{output}\n"
-
-    assert result.stderr.endswith(
-        "warning: Cannot extract parameters values: "
-        "<Command show-params> does not inherits from ExtraCommand.\n"
-    )
-
-
-def test_integrated_show_params_option(invoke, create_config):
-    @extra_command
-    @option("--int-param1", type=int, default=10)
-    @option("--int-param2", type=int, default=555)
-    def show_params_cli(int_param1, int_param2):
-        echo(f"int_param1 is {int_param1!r}")
-        echo(f"int_param2 is {int_param2!r}")
-
-    conf_file = """
-        [show-params-cli]
-        int_param1 = 3
-        extra_value = "unallowed"
-        """
-    conf_path = create_config("show-params-cli.toml", conf_file)
-
-    raw_args = [
-        "--verbosity",
-        "DeBuG",
-        "--config",
-        str(conf_path),
-        "--int-param1",
-        "9999",
-        "--show-params",
-        "--help",
-    ]
-    result = invoke(show_params_cli, *raw_args, color=False)
-
-    assert result.exit_code == 0
-    assert f"debug: click_extra.raw_args: {raw_args!r}\n" in result.stderr
-
-    table = [
-        (
-            "show-params-cli.color",
-            "click_extra.colorize.ColorOption",
-            "--color, --ansi / --no-color, --no-ansi",
-            "bool",
-            "✓",
-            "✘",
-            "SHOW_PARAMS_CLI_COLOR",
-            True,
-            True,
-            "DEFAULT",
-        ),
-        (
-            "show-params-cli.config",
-            "click_extra.config.ConfigOption",
-            "-C, --config CONFIG_PATH",
-            "str",
-            "✘",
-            "✘",
-            "SHOW_PARAMS_CLI_CONFIG",
-            f"{Path(get_app_dir('show-params-cli')).resolve()}{sep}*.{{toml,yaml,yml,json,ini,xml}}",
-            str(conf_path),
-            "COMMANDLINE",
-        ),
-        (
-            "show-params-cli.help",
-            "click_extra.colorize.HelpOption",
-            "-h, --help",
-            "bool",
-            "✘",
-            "✘",
-            "SHOW_PARAMS_CLI_HELP",
-            False,
-            True,
-            "COMMANDLINE",
-        ),
-        (
-            "show-params-cli.int_param1",
-            "cloup._params.Option",
-            "--int-param1 INTEGER",
-            "int",
-            "✓",
-            "✓",
-            "SHOW_PARAMS_CLI_INT_PARAM1",
-            3,
-            9999,
-            "COMMANDLINE",
-        ),
-        (
-            "show-params-cli.int_param2",
-            "cloup._params.Option",
-            "--int-param2 INTEGER",
-            "int",
-            "✓",
-            "✓",
-            "SHOW_PARAMS_CLI_INT_PARAM2",
-            555,
-            555,
-            "DEFAULT",
-        ),
-        (
-            "show-params-cli.show_params",
-            "click_extra.config.ShowParamsOption",
-            "--show-params",
-            "bool",
-            "✘",
-            "✘",
-            "SHOW_PARAMS_CLI_SHOW_PARAMS",
-            False,
-            True,
-            "COMMANDLINE",
-        ),
-        (
-            "show-params-cli.time",
-            "click_extra.timer.TimerOption",
-            "--time / --no-time",
-            "bool",
-            "✓",
-            "✘",
-            "SHOW_PARAMS_CLI_TIME",
-            False,
-            False,
-            "DEFAULT",
-        ),
-        (
-            "show-params-cli.verbosity",
-            "click_extra.logging.VerbosityOption",
-            "-v, --verbosity LEVEL",
-            "str",
-            "✓",
-            "✘",
-            "SHOW_PARAMS_CLI_VERBOSITY",
-            "WARNING",
-            "DeBuG",
-            "COMMANDLINE",
-        ),
-        (
-            "show-params-cli.version",
-            "click_extra.version.VersionOption",
-            "--version",
-            "bool",
-            "✘",
-            "✘",
-            "SHOW_PARAMS_CLI_VERSION",
-            False,
-            False,
-            "DEFAULT",
-        ),
-    ]
-    output = tabulate(
-        table,
-        headers=ShowParamsOption.TABLE_HEADERS,
-        tablefmt="rounded_outline",
-        disable_numparse=True,
-    )
-    assert result.output == f"{output}\n"
-
-    assert f"debug: click_extra.raw_args: {raw_args}" in result.stderr
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_logging.py` & `click_extra-4.3.0/click_extra/tests/test_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
-import re
 import logging
 import random
+import re
 
+import click
 import pytest
 from pytest_cases import parametrize
-import click
 
 from .. import echo
 from ..decorators import extra_command, verbosity_option
-from ..logging import LOG_LEVELS
+from ..logging import DEFAULT_LEVEL, LOG_LEVELS
 from .conftest import (
     command_decorators,
+    default_debug_colored_log_end,
     default_debug_colored_log_start,
     default_debug_uncolored_log_end,
-    default_debug_colored_log_end,
     skip_windows_colors,
 )
-from ..logging import DEFAULT_LEVEL
 
 
 def test_level_default_order():
     assert tuple(LOG_LEVELS) == ("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG")
 
 
 def test_root_logger_defaults():
@@ -59,15 +58,15 @@
     @cmd_decorator
     @verbosity_option
     def logging_cli1():
         echo("It works!")
 
     result = invoke(logging_cli1, "--verbosity", "random")
     assert result.exit_code == 2
-    assert not result.output
+    assert not result.stdout
 
     group_help = " COMMAND [ARGS]..." if "group" in cmd_type else ""
     extra_suggest = (
         "Try 'logging-cli1 --help' for help.\n" if "extra" not in cmd_type else ""
     )
     assert result.stderr == (
         f"Usage: logging-cli1 [OPTIONS]{group_help}\n"
@@ -107,15 +106,15 @@
         logging.info("my info message.")
         logging.warning("my warning message.")
         logging.error("my error message.")
         logging.critical("my critical message.")
 
     result = invoke(logging_cli2, "--verbosity", level, color=True)
     assert result.exit_code == 0
-    assert result.output == "It works!\n"
+    assert result.stdout == "It works!\n"
 
     messages = (
         (
             r"\x1b\[34mdebug\x1b\[0m: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
             r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
             r"\x1b\[34mdebug\x1b\[0m: my random message.\n"
             r"\x1b\[34mdebug\x1b\[0m: my debug message.\n"
@@ -139,15 +138,15 @@
 def test_integrated_verbosity_option(invoke, level):
     @extra_command
     def logging_cli3():
         echo("It works!")
 
     result = invoke(logging_cli3, "--verbosity", level, color=True)
     assert result.exit_code == 0
-    assert result.output == "It works!\n"
+    assert result.stdout == "It works!\n"
     if level == "DEBUG":
         assert re.fullmatch(
             default_debug_colored_log_start + default_debug_colored_log_end,
             result.stderr,
         )
     else:
         assert not result.stderr
@@ -164,15 +163,15 @@
     @verbosity_option(default_logger=logger_param)
     def awesome_app():
         echo("Starting Awesome App...")
         logging.getLogger("awesome_app").debug("Awesome App has started.")
 
     result = invoke(awesome_app, params, color=False)
     assert result.exit_code == 0
-    assert result.output == "Starting Awesome App...\n"
+    assert result.stdout == "Starting Awesome App...\n"
     if params:
         assert re.fullmatch(
             (
                 r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
                 r"debug: Set <Logger awesome_app \(DEBUG\)> to DEBUG.\n"
                 r"debug: Awesome App has started\.\n"
                 r"debug: Reset <Logger awesome_app \(DEBUG\)> to WARNING.\n"
@@ -192,15 +191,15 @@
     def awesome_app():
         root_logger = logging.getLogger()
         root_logger.debug("my debug message.")
 
     for name in param_names:
         result = invoke(awesome_app, name, "DEBUG", color=False)
         assert result.exit_code == 0
-        assert not result.output
+        assert not result.stdout
         assert re.fullmatch(
             (
                 r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
                 r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
                 r"debug: my debug message\.\n"
                 rf"{default_debug_uncolored_log_end}"
             ),
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_platforms.py` & `click_extra-4.3.0/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/tests/test_pygments.py` & `click_extra-4.3.0/click_extra/tests/test_pygments.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,32 +14,32 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import sys
 import tarfile
+from importlib import metadata
 from operator import itemgetter
 from pathlib import Path
-from importlib import metadata
 
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    import tomli as tomllib  # type: ignore[import]
+
+import requests
 from boltons.strutils import camel2under
 from boltons.typeutils import issubclass
 from pygments.filter import Filter
 from pygments.filters import get_filter_by_name
 from pygments.formatter import Formatter
 from pygments.formatters import get_formatter_by_name
 from pygments.lexer import Lexer
 from pygments.lexers import find_lexer_class_by_name, get_lexer_by_name
-import requests
-
-if sys.version_info >= (3, 11):
-    import tomllib
-else:
-    import tomli as tomllib  # type: ignore[import]
 
 from .. import pygments as extra_pygments
 from ..pygments import DEFAULT_TOKEN_TYPE, collect_session_lexers
 
 PROJECT_ROOT = Path(__file__).parent.parent.parent
 
 
@@ -167,14 +167,32 @@
 
 def check_entry_points(entry_points: dict[str, str], *section_path: str) -> None:
     entry_points = dict(sorted(entry_points.items(), key=itemgetter(0)))
     project_entry_points = get_pyproject_section(*section_path)
     assert project_entry_points == entry_points
 
 
+def test_formatter_entry_points():
+    entry_points = {}
+    for name in collect_classes(Formatter):
+        entry_id = camel2under(name).replace("_", "-")
+        entry_points[entry_id] = f"click_extra.pygments:{name}"
+
+    check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.formatters")
+
+
+def test_filter_entry_points():
+    entry_points = {}
+    for name in collect_classes(Filter):
+        entry_id = camel2under(name).replace("_", "-")
+        entry_points[entry_id] = f"click_extra.pygments:{name}"
+
+    check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.filters")
+
+
 def test_lexer_entry_points():
     entry_points = {}
     for lexer in collect_session_lexers():
         # Check an ANSI lexer variant is available for import from Click Extra.
         ansi_lexer_id = f"Ansi{lexer.__name__}"
         assert ansi_lexer_id in extra_pygments.__dict__
 
@@ -186,47 +204,29 @@
         # Generate the lexer entry point.
         class_path = f"click_extra.pygments:{ansi_lexer_id}"
         entry_points[entry_id] = class_path
 
     check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.lexers")
 
 
-def test_filter_entry_points():
-    entry_points = {}
-    for name in collect_classes(Filter):
-        entry_id = camel2under(name).replace("_", "-")
-        entry_points[entry_id] = f"click_extra.pygments:{name}"
-
-    check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.filters")
-
-
-def test_formatter_entry_points():
-    entry_points = {}
-    for name in collect_classes(Formatter):
-        entry_id = camel2under(name).replace("_", "-")
-        entry_points[entry_id] = f"click_extra.pygments:{name}"
-
-    check_entry_points(entry_points, "tool", "poetry", "plugins", "pygments.formatters")
-
-
-def test_registered_lexers():
-    for klass in collect_classes(Lexer).values():
+def test_registered_formatters():
+    for klass in collect_classes(Formatter).values():
         for alias in klass.aliases:
-            get_lexer_by_name(alias)
+            get_formatter_by_name(alias)
 
 
 def test_registered_filters():
     for name in collect_classes(Filter):
         entry_id = camel2under(name).replace("_", "-")
         get_filter_by_name(entry_id)
 
 
-def test_registered_formatters():
-    for klass in collect_classes(Formatter).values():
+def test_registered_lexers():
+    for klass in collect_classes(Lexer).values():
         for alias in klass.aliases:
-            get_formatter_by_name(alias)
+            get_lexer_by_name(alias)
 
 
 def test_ansi_lexers_doc():
     doc_content = PROJECT_ROOT.joinpath("docs/pygments.md").read_text()
     for lexer in collect_session_lexers():
         assert lexer.__name__ in doc_content
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_run.py` & `click_extra-4.3.0/click_extra/tests/test_testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,38 +9,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
-"""Test all runner utilities as well as all the test and pytest helpers."""
+"""Test the testing utilities and the simulation of CLI execution."""
 
 from __future__ import annotations
 
+import logging
 import os
 from pathlib import Path
-import logging
 
 import click
+import pytest
 from pytest_cases import fixture, parametrize
 
-from .. import Style, echo, pass_context, secho, style
+from .. import Style, command, echo, pass_context, secho, style
 from ..platforms import is_windows
-from ..run import env_copy
+from ..testing import ExtraCliRunner, env_copy
 from .conftest import command_decorators, skip_windows_colors
 
 
 def test_real_fs():
     """Check a simple test is not caught into the CLI runner fixture which is
     encapsulating all filesystem access into temporary directory structure."""
     assert str(Path(__file__)).startswith(str(Path.cwd()))
 
 
-def test_temporary_fs(runner):
+def test_temporary_fs(extra_runner):
     """Check the CLI runner fixture properly encapsulated the filesystem in temporary
     directory."""
     assert not str(Path(__file__)).startswith(str(Path.cwd()))
 
 
 def test_env_copy():
     env_var = "MPM_DUMMY_ENV_VAR_93725"
@@ -51,14 +52,53 @@
 
     extended_env = env_copy({env_var: "yo"})
     assert env_var in extended_env
     assert extended_env[env_var] == "yo"
     assert env_var not in os.environ
 
 
+def test_runner_output():
+
+    @command
+    def cli_output():
+        echo("1 - stdout")
+        echo("2 - stderr", err=True)
+        echo("3 - stdout")
+        echo("4 - stderr", err=True)
+
+    runner = ExtraCliRunner(mix_stderr=False)
+    result = runner.invoke(cli_output)
+
+    assert result.output == "1 - stdout\n3 - stdout\n"
+    assert result.stdout == result.output
+    assert result.stderr == "2 - stderr\n4 - stderr\n"
+
+    runner_mix = ExtraCliRunner(mix_stderr=True)
+    result_mix = runner_mix.invoke(cli_output)
+
+    assert result_mix.output == "1 - stdout\n2 - stderr\n3 - stdout\n4 - stderr\n"
+    assert result_mix.stdout == "1 - stdout\n3 - stdout\n"
+    assert result_mix.stderr == "2 - stderr\n4 - stderr\n"
+
+
+@pytest.mark.parametrize("mix_stderr", (True, False))
+def test_runner_empty_stderr(mix_stderr):
+
+    @command
+    def cli_empty_stderr():
+        echo("stdout")
+
+    runner = ExtraCliRunner(mix_stderr=mix_stderr)
+    result = runner.invoke(cli_empty_stderr)
+
+    assert result.output == "stdout\n"
+    assert result.stdout == result.output
+    assert result.stderr == ""
+
+
 @click.command
 @pass_context
 def run_cli1(ctx):
     """https://github.com/pallets/click/issues/2111."""
     echo(Style(fg="green")("echo()"))
     echo(Style(fg="green")("echo(color=None)"), color=None)
     echo(Style(fg="red")("echo(color=True) bypass invoke.color = False"), color=True)
@@ -104,15 +144,15 @@
         echo(f"click.utils.should_strip_ansi = {click.utils.should_strip_ansi()!r}")
 
     return run_cli2
 
 
 def check_default_colored_rendering(result):
     assert result.exit_code == 0
-    assert result.output.startswith(
+    assert result.stdout.startswith(
         "\x1b[32mecho()\x1b[0m\n"
         "\x1b[32mecho(color=None)\x1b[0m\n"
         "\x1b[31mecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "echo(color=False)\n"
         "\x1b[32msecho()\x1b[0m\n"
         "\x1b[32msecho(color=None)\x1b[0m\n"
         "\x1b[31msecho(color=True) bypass invoke.color = False\x1b[0m\n"
@@ -120,15 +160,15 @@
         "\x1b[34mprint() bypass Click.\x1b[0m\n"
     )
     assert result.stderr == "\x1b[33mwarning\x1b[0m: Is the logger colored?\n"
 
 
 def check_default_uncolored_rendering(result):
     assert result.exit_code == 0
-    assert result.output.startswith(
+    assert result.stdout.startswith(
         "echo()\n"
         "echo(color=None)\n"
         "\x1b[31mecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "echo(color=False)\n"
         "secho()\n"
         "secho(color=None)\n"
         "\x1b[31msecho(color=True) bypass invoke.color = False\x1b[0m\n"
@@ -136,15 +176,15 @@
         "\x1b[34mprint() bypass Click.\x1b[0m\n"
     )
     assert result.stderr == "warning: Is the logger colored?\n"
 
 
 def check_forced_uncolored_rendering(result):
     assert result.exit_code == 0
-    assert result.output.startswith(
+    assert result.stdout.startswith(
         "echo()\n"
         "echo(color=None)\n"
         "echo(color=True) bypass invoke.color = False\n"
         "echo(color=False)\n"
         "secho()\n"
         "secho(color=None)\n"
         "secho(color=True) bypass invoke.color = False\n"
@@ -154,53 +194,54 @@
     assert result.stderr == "warning: Is the logger colored?\n"
 
 
 @skip_windows_colors
 def test_invoke_optional_color(invoke):
     result = invoke(run_cli1, color=None)
     check_default_uncolored_rendering(result)
-    assert result.output.endswith(
+    assert result.stdout.endswith(
         "Context.color = None\nclick.utils.should_strip_ansi = True\n"
     )
 
 
 @skip_windows_colors
 def test_invoke_default_color(invoke):
     result = invoke(run_cli1)
     check_default_uncolored_rendering(result)
-    assert result.output.endswith(
+    assert result.stdout.endswith(
         "Context.color = None\nclick.utils.should_strip_ansi = True\n"
     )
 
 
 @skip_windows_colors
 def test_invoke_forced_color_stripping(invoke):
     result = invoke(run_cli1, color=False)
     check_forced_uncolored_rendering(result)
-    assert result.output.endswith(
+    assert result.stdout.endswith(
         "Context.color = None\nclick.utils.should_strip_ansi = True\n"
     )
 
 
 @skip_windows_colors
 def test_invoke_color_keep(invoke):
-    """On windows Click ends up deciding it is not running in an interactive terminal
+    """On Windows Click ends up deciding it is not running in an interactive terminal
     and forces the stripping of all colors."""
     result = invoke(run_cli1, color=True)
     if is_windows():
         check_default_uncolored_rendering(result)
     else:
         check_default_colored_rendering(result)
-    assert result.output.endswith(
+    assert result.stdout.endswith(
         "Context.color = None\nclick.utils.should_strip_ansi = False\n"
     )
 
 
 @skip_windows_colors
 def test_invoke_color_forced(invoke):
-    # Test colors are preserved while invoking, and forced to be rendered
-    # on Windows.
+    """Test colors are preserved while invoking, and forced to be rendered
+    on Windows.
+    """
     result = invoke(run_cli1, color="forced")
     check_default_colored_rendering(result)
-    assert result.output.endswith(
+    assert result.stdout.endswith(
         "Context.color = True\nclick.utils.should_strip_ansi = False\n"
     )
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_tabulate.py` & `click_extra-4.3.0/click_extra/tests/test_tabulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     @cmd_decorator
     @table_format_option
     def tabulate_cli1():
         echo("It works!")
 
     result = invoke(tabulate_cli1, "--table-format", "random")
     assert result.exit_code == 2
-    assert not result.output
+    assert not result.stdout
 
     group_help = " COMMAND [ARGS]..." if "group" in cmd_type else ""
     extra_suggest = (
         "Try 'tabulate-cli1 --help' for help.\n" if "extra" not in cmd_type else ""
     )
     assert result.stderr == (
         f"Usage: tabulate-cli1 [OPTIONS]{group_help}\n"
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_telemetry.py` & `click_extra-4.3.0/click_extra/tests/test_telemetry.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,20 +48,20 @@
           --help                        Show this message and exit.
         """
     )
 
     result = invoke(standalone_telemetry, "--telemetry")
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.output == "It works!\nTelemetry value: True\n"
+    assert result.stdout == "It works!\nTelemetry value: True\n"
 
     result = invoke(standalone_telemetry, "--no-telemetry")
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.output == "It works!\nTelemetry value: False\n"
+    assert result.stdout == "It works!\nTelemetry value: False\n"
 
 
 def test_multiple_envvars(invoke):
     @command(context_settings={"auto_envvar_prefix": "yo", "show_default": True})
     @telemetry_option
     @pass_context
     def standalone_telemetry(ctx):
@@ -82,8 +82,8 @@
           --help                        Show this message and exit.
         """
     )
 
     result = invoke(standalone_telemetry, env={"DO_NOT_TRACK": "1"})
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.output == "It works!\nTelemetry value: True\n"
+    assert result.stdout == "It works!\nTelemetry value: True\n"
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_timer.py` & `click_extra-4.3.0/click_extra/tests/test_timer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from textwrap import dedent
 from time import sleep
 
 from pytest_cases import parametrize
 
 from .. import echo
 from ..decorators import extra_group, timer_option
-
 from .conftest import (
     command_decorators,
 )
 
 
 @extra_group
 def integrated_timer():
@@ -59,26 +58,26 @@
 def test_integrated_time_option(invoke, subcommand_id, time_min, time_max):
     result = invoke(integrated_timer, "--time", f"{subcommand_id}-subcommand")
     assert result.exit_code == 0
     assert not result.stderr
     group = re.fullmatch(
         rf"Start of CLI\nEnd of {subcommand_id} subcommand\n"
         r"Execution time: (?P<time>[0-9.]+) seconds.\n",
-        result.output,
+        result.stdout,
     )
     assert group
     assert time_min < float(group.groupdict()["time"]) < time_max
 
 
 @parametrize("subcommand_id", ("fast", "slow"))
 def test_integrated_notime_option(invoke, subcommand_id):
     result = invoke(integrated_timer, "--no-time", f"{subcommand_id}-subcommand")
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.output == f"Start of CLI\nEnd of {subcommand_id} subcommand\n"
+    assert result.stdout == f"Start of CLI\nEnd of {subcommand_id} subcommand\n"
 
 
 @parametrize(
     "cmd_decorator",
     # Skip click extra's commands, as timer option is already part of the default.
     command_decorators(no_groups=True, no_extra=True),
 )
@@ -103,14 +102,14 @@
     )
 
     result = invoke(standalone_timer, "--time")
     assert result.exit_code == 0
     assert not result.stderr
     assert re.fullmatch(
         r"It works!\nExecution time: [0-9.]+ seconds.\n",
-        result.output,
+        result.stdout,
     )
 
     result = invoke(standalone_timer, "--no-time")
     assert result.exit_code == 0
     assert not result.stderr
-    assert result.output == "It works!\n"
+    assert result.stdout == "It works!\n"
```

### Comparing `click_extra-4.2.0/click_extra/tests/test_version.py` & `click_extra-4.3.0/click_extra/tests/test_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     def color_cli2():
         echo("It works!")
 
     # Test default coloring.
     result = invoke(color_cli2, "--version", color=True)
     assert result.exit_code == 0
 
-    regex_output = (
+    regex_stdout = (
         r"\x1b\[97mcolor-cli2\x1b\[0m, version \x1b\[32m1.2.3.4"
         r"\x1b\[0m\x1b\[90m\n{'.+'}"
         r"\x1b\[0m\n"
     )
-    assert re.fullmatch(regex_output, result.output)
+    assert re.fullmatch(regex_stdout, result.stdout)
 
     assert not result.stderr
 
 
 @pytest.mark.xfail(
     strict=False, reason="version_option always displays click-extra version. See #176."
 )
@@ -77,15 +77,15 @@
     def color_cli3():
         echo("It works!")
 
     # Test default coloring.
     result = invoke(color_cli3, "--version", color=True)
     assert result.exit_code == 0
     assert (
-        result.output == "\x1b[97mcolor-cli3\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
+        result.stdout == "\x1b[97mcolor-cli3\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
     )
     assert not result.stderr
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
     "params", (None, "--help", "blah", ("--config", "random.toml"))
@@ -94,20 +94,20 @@
     @extra_group(version="1.2.3.4")
     def color_cli4():
         echo("It works!")
 
     result = invoke(color_cli4, "--version", params, color=True)
     assert result.exit_code == 0
 
-    regex_output = (
+    regex_stdout = (
         r"\x1b\[97mcolor-cli4\x1b\[0m, version \x1b\[32m1.2.3.4"
         r"\x1b\[0m\x1b\[90m\n{'.+'}"
         r"\x1b\[0m\n"
     )
-    assert re.fullmatch(regex_output, result.output)
+    assert re.fullmatch(regex_stdout, result.stdout)
 
     assert not result.stderr
 
 
 @skip_windows_colors
 def test_color_option_precedence(invoke):
     """--no-color has an effect on --version, if placed in the right order.
@@ -127,14 +127,14 @@
     @color_option
     @version_option(version="2.1.9")
     def color_cli6():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli6, "--no-color", "--version", "command1", color=True)
     assert result.exit_code == 0
-    assert result.output == "color-cli6, version 2.1.9\n"
+    assert result.stdout == "color-cli6, version 2.1.9\n"
     assert not result.stderr
 
     result = invoke(color_cli6, "--version", "--no-color", "command1", color=True)
     assert result.exit_code == 0
-    assert result.output == "\x1b[97mcolor-cli6\x1b[0m, version \x1b[32m2.1.9\x1b[0m\n"
+    assert result.stdout == "\x1b[97mcolor-cli6\x1b[0m, version \x1b[32m2.1.9\x1b[0m\n"
     assert not result.stderr
```

### Comparing `click_extra-4.2.0/click_extra/timer.py` & `click_extra-4.3.0/click_extra/timer.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/click_extra/version.py` & `click_extra-4.3.0/click_extra/version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.2.0/pyproject.toml` & `click_extra-4.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.2.0"
+version = "4.3.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -111,22 +111,28 @@
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
 sphinx-autodoc-typehints = "^1.23.0"
 sphinx-copybutton = "^0.5.2"
 sphinx-design = "^0.4.1"
 sphinx-issues = "^3.0.1"
 sphinxext-opengraph = "^0.7.5"
-sphinxcontrib-mermaid = "^0.8.1"
+sphinxcontrib-mermaid = "^0.9"
 types-Pygments = "^2.15.0.0"
 types-PyYAML = "^6.0.12.9"
 types-regex = "^2023.3.23.1"
 types-requests = "^2.28.11.17"
 types-tabulate = "^0.9.0.2"
 types-xmltodict = "^0.13.0.2"
 
+[tool.poetry.plugins."pygments.formatters"]
+ansi-html-formatter = "click_extra.pygments:AnsiHtmlFormatter"
+
+[tool.poetry.plugins."pygments.filters"]
+ansi-filter = "click_extra.pygments:AnsiFilter"
+
 [tool.poetry.plugins."pygments.lexers"]
 # The name of the entrypoint value doesn’t really matter, Pygments extracts required metadata from the class definition.
 # Source: https://pygments.org/docs/plugins/#defining-plugins-through-entrypoints
 ansi-bash-session = "click_extra.pygments:AnsiBashSessionLexer"
 ansi-dylan-console = "click_extra.pygments:AnsiDylanConsoleLexer"
 ansi-elixir-console = "click_extra.pygments:AnsiElixirConsoleLexer"
 ansi-erlang-shell = "click_extra.pygments:AnsiErlangShellLexer"
@@ -140,20 +146,14 @@
 ansi-psysh-console = "click_extra.pygments:AnsiPsyshConsoleLexer"
 ansi-python-console = "click_extra.pygments:AnsiPythonConsoleLexer"
 ansi-r-console = "click_extra.pygments:AnsiRConsoleLexer"
 ansi-ruby-console = "click_extra.pygments:AnsiRubyConsoleLexer"
 ansi-sqlite-console = "click_extra.pygments:AnsiSqliteConsoleLexer"
 ansi-tcsh-session = "click_extra.pygments:AnsiTcshSessionLexer"
 
-[tool.poetry.plugins."pygments.filters"]
-ansi-filter = "click_extra.pygments:AnsiFilter"
-
-[tool.poetry.plugins."pygments.formatters"]
-ansi-html-formatter = "click_extra.pygments:AnsiHtmlFormatter"
-
 [tool.mypy]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unreachable = true
 pretty = true
```

### Comparing `click_extra-4.2.0/readme.md` & `click_extra-4.3.0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 - Automatic inference of the configuration file structure from your CLI's options
 - Remote loading of [configuration files from URLs](https://kdeldycke.github.io/click-extra/config.html#remote-url)
 - Optional [strict validation](https://kdeldycke.github.io/click-extra/config.html#strictness) of configuration
 - Respect the [default application path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on each platform (XDG spec on Linux)
 - [Glob search patterns](https://kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration files
 - Respect of `CLI` > `Configuration` > `Environment` > `Defaults` [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence)
 - Normalization and discoverability of environment variables
-- [`--show-params` option](https://kdeldycke.github.io/click-extra/config.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [`--show-params` option](https://kdeldycke.github.io/click-extra/parameters.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [Click parameters introspection](https://kdeldycke.github.io/click-extra/parameters.html#introspecting-parameters)
 - [Colorization of help screens](https://kdeldycke.github.io/click-extra/colorize.html) at the semantic-level of options, parameters, subheadings, choices, metavars and defaults
 - Global `show_envvar` option to display all environment variables in help screens
 - `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))
 - `--color`/`--no-color` option flag
 - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code
 - Recognize traditional environment variable conventions:
   - `NO_COLOR` from [`no-color.org`](https://no-color.org)
@@ -62,18 +63,18 @@
 - Global `show_choices` to activate selection of choices on user input prompts
 - [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
   - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
+- [Inline testing of CLI examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in documentation
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
-- Pygments styles and filters for ANSI rendering
-- [Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
-- Rely on [`cloup`](https://github.com/janluke/cloup) to add:
+- [Fixes 40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
+- Rely on [Cloup](https://github.com/janluke/cloup) to add:
   - option groups
   - constraints
   - subcommands sections
   - aliases
   - command suggestion (`Did you mean <subcommand>?`)
 
 ## Used in
@@ -83,15 +84,14 @@
 - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://github.com/kdeldycke/meta-package-manager#readme)
   \- A unifying CLI for multiple package managers.
 - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A
   CLI to deduplicate similar emails.
 - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox tool.
 - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/hugolundin/badger#readme) - An mDNS-based reverse
   proxy for naming services on a local network.
-- ![GitHub stars](https://img.shields.io/github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme)
 
 Feel free to send a PR to add your project in this list if you are relying on Click Extra in any way.
 
 ## Development
 
 [Development guidelines](https://kdeldycke.github.io/meta-package-manager/development.html)
 are the same as
```

#### html2text {}

```diff
@@ -32,55 +32,55 @@
 config.html#strictness) of configuration - Respect the [default application
 path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on
 each platform (XDG spec on Linux) - [Glob search patterns](https://
 kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration
 files - Respect of `CLI` > `Configuration` > `Environment` > `Defaults`
 [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence) -
 Normalization and discoverability of environment variables - [`--show-params`
-option](https://kdeldycke.github.io/click-extra/config.html#show-params-option)
-to debug parameters defaults, values, environment variables and provenance -
-[Colorization of help screens](https://kdeldycke.github.io/click-extra/
-colorize.html) at the semantic-level of options, parameters, subheadings,
-choices, metavars and defaults - Global `show_envvar` option to display all
-environment variables in help screens - `-h`/`--help` option names (see [rant
-on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `--
-color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
-in/out of tracking code - Recognize traditional environment variable
-conventions: - `NO_COLOR` from [`no-color.org`](https://no-color.org) -
-`DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com) -
-Colored `--version` option - [Colored `--verbosity` option and logs](https://
-kdeldycke.github.io/click-extra/logging.html) - `--time`/`--no-time` flag to
-measure duration of command execution - Global `show_choices` to activate
-selection of choices on user input prompts - [Platform recognition](https://
-kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux,
-Windows, UNIX, \*BSD, â¦) - New conditional markers for `pytest`: -
-`@skip_linux`, `@skip_macos` and `@skip_windows` - `@unless_linux`,
-`@unless_macos` and `@unless_windows` - `@destructive` and `@non_destructive` -
-[`.. click:example::` and `.. click:run::` Sphinx directives](https://
-kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
-their execution - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
-click-extra/pygments.html#lexers) for shell session and console output -
-Pygments styles and filters for ANSI rendering - [Fixes 30+ bugs](https://
-kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
-- Rely on [`cloup`](https://github.com/janluke/cloup) to add: - option groups -
-constraints - subcommands sections - aliases - command suggestion (`Did you
-mean ?`) ## Used in Check these projects to get real-life examples of `click-
-extra` usage: - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/
-meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager]
-(https://github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI
-for multiple package managers. - ![GitHub stars](https://img.shields.io/github/
-stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
-Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
-deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
-stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
-[fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
-rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
-stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
-(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse proxy for
-naming services on a local network. - ![GitHub stars](https://img.shields.io/
-github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular
-Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme) Feel
-free to send a PR to add your project in this list if you are relying on Click
-Extra in any way. ## Development [Development guidelines](https://
-kdeldycke.github.io/meta-package-manager/development.html) are the same as
-[parent project `mpm`](https://github.com/kdeldycke/meta-package-manager), from
-which `click-extra` originated.
+option](https://kdeldycke.github.io/click-extra/parameters.html#show-params-
+option) to debug parameters defaults, values, environment variables and
+provenance - [Click parameters introspection](https://kdeldycke.github.io/
+click-extra/parameters.html#introspecting-parameters) - [Colorization of help
+screens](https://kdeldycke.github.io/click-extra/colorize.html) at the
+semantic-level of options, parameters, subheadings, choices, metavars and
+defaults - Global `show_envvar` option to display all environment variables in
+help screens - `-h`/`--help` option names (see [rant on other inconsistencies]
+(https://blog.craftyguy.net/cmdline-help/)) - `--color`/`--no-color` option
+flag - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code -
+Recognize traditional environment variable conventions: - `NO_COLOR` from [`no-
+color.org`](https://no-color.org) - `DO_NOT_TRACK` from
+[`consoledonottrack.com`](https://consoledonottrack.com) - Colored `--version`
+option - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/
+click-extra/logging.html) - `--time`/`--no-time` flag to measure duration of
+command execution - Global `show_choices` to activate selection of choices on
+user input prompts - [Platform recognition](https://kdeldycke.github.io/click-
+extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
+conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
+`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
+`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
+run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
+to document CLI source code and their execution - [Inline testing of CLI
+examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in
+documentation - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
+click-extra/pygments.html#lexers) for shell session and console output - [Fixes
+40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other
+Click-related projects - Rely on [Cloup](https://github.com/janluke/cloup) to
+add: - option groups - constraints - subcommands sections - aliases - command
+suggestion (`Did you mean ?`) ## Used in Check these projects to get real-life
+examples of `click-extra` usage: - ![GitHub stars](https://img.shields.io/
+github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square)
+[Meta Package Manager](https://github.com/kdeldycke/meta-package-
+manager#readme) \- A unifying CLI for multiple package managers. - ![GitHub
+stars](https://img.shields.io/github/stars/kdeldycke/mail-
+deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://
+github.com/kdeldycke/mail-deduplicate#readme) - A CLI to deduplicate similar
+emails. - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-
+Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://
+github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox
+tool. - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/
+badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/
+hugolundin/badger#readme) - An mDNS-based reverse proxy for naming services on
+a local network. Feel free to send a PR to add your project in this list if you
+are relying on Click Extra in any way. ## Development [Development guidelines]
+(https://kdeldycke.github.io/meta-package-manager/development.html) are the
+same as [parent project `mpm`](https://github.com/kdeldycke/meta-package-
+manager), from which `click-extra` originated.
```

### Comparing `click_extra-4.2.0/PKG-INFO` & `click_extra-4.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.2.0
+Version: 4.3.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -107,15 +107,16 @@
 - Automatic inference of the configuration file structure from your CLI's options
 - Remote loading of [configuration files from URLs](https://kdeldycke.github.io/click-extra/config.html#remote-url)
 - Optional [strict validation](https://kdeldycke.github.io/click-extra/config.html#strictness) of configuration
 - Respect the [default application path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on each platform (XDG spec on Linux)
 - [Glob search patterns](https://kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration files
 - Respect of `CLI` > `Configuration` > `Environment` > `Defaults` [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence)
 - Normalization and discoverability of environment variables
-- [`--show-params` option](https://kdeldycke.github.io/click-extra/config.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [`--show-params` option](https://kdeldycke.github.io/click-extra/parameters.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [Click parameters introspection](https://kdeldycke.github.io/click-extra/parameters.html#introspecting-parameters)
 - [Colorization of help screens](https://kdeldycke.github.io/click-extra/colorize.html) at the semantic-level of options, parameters, subheadings, choices, metavars and defaults
 - Global `show_envvar` option to display all environment variables in help screens
 - `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))
 - `--color`/`--no-color` option flag
 - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code
 - Recognize traditional environment variable conventions:
   - `NO_COLOR` from [`no-color.org`](https://no-color.org)
@@ -126,18 +127,18 @@
 - Global `show_choices` to activate selection of choices on user input prompts
 - [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
   - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
+- [Inline testing of CLI examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in documentation
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
-- Pygments styles and filters for ANSI rendering
-- [Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
-- Rely on [`cloup`](https://github.com/janluke/cloup) to add:
+- [Fixes 40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
+- Rely on [Cloup](https://github.com/janluke/cloup) to add:
   - option groups
   - constraints
   - subcommands sections
   - aliases
   - command suggestion (`Did you mean <subcommand>?`)
 
 ## Used in
@@ -147,15 +148,14 @@
 - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://github.com/kdeldycke/meta-package-manager#readme)
   \- A unifying CLI for multiple package managers.
 - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A
   CLI to deduplicate similar emails.
 - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox tool.
 - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/hugolundin/badger#readme) - An mDNS-based reverse
   proxy for naming services on a local network.
-- ![GitHub stars](https://img.shields.io/github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme)
 
 Feel free to send a PR to add your project in this list if you are relying on Click Extra in any way.
 
 ## Development
 
 [Development guidelines](https://kdeldycke.github.io/meta-package-manager/development.html)
 are the same as
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.2.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.3.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -72,55 +72,55 @@
 config.html#strictness) of configuration - Respect the [default application
 path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on
 each platform (XDG spec on Linux) - [Glob search patterns](https://
 kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration
 files - Respect of `CLI` > `Configuration` > `Environment` > `Defaults`
 [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence) -
 Normalization and discoverability of environment variables - [`--show-params`
-option](https://kdeldycke.github.io/click-extra/config.html#show-params-option)
-to debug parameters defaults, values, environment variables and provenance -
-[Colorization of help screens](https://kdeldycke.github.io/click-extra/
-colorize.html) at the semantic-level of options, parameters, subheadings,
-choices, metavars and defaults - Global `show_envvar` option to display all
-environment variables in help screens - `-h`/`--help` option names (see [rant
-on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `--
-color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
-in/out of tracking code - Recognize traditional environment variable
-conventions: - `NO_COLOR` from [`no-color.org`](https://no-color.org) -
-`DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com) -
-Colored `--version` option - [Colored `--verbosity` option and logs](https://
-kdeldycke.github.io/click-extra/logging.html) - `--time`/`--no-time` flag to
-measure duration of command execution - Global `show_choices` to activate
-selection of choices on user input prompts - [Platform recognition](https://
-kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux,
-Windows, UNIX, \*BSD, â¦) - New conditional markers for `pytest`: -
-`@skip_linux`, `@skip_macos` and `@skip_windows` - `@unless_linux`,
-`@unless_macos` and `@unless_windows` - `@destructive` and `@non_destructive` -
-[`.. click:example::` and `.. click:run::` Sphinx directives](https://
-kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
-their execution - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
-click-extra/pygments.html#lexers) for shell session and console output -
-Pygments styles and filters for ANSI rendering - [Fixes 30+ bugs](https://
-kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
-- Rely on [`cloup`](https://github.com/janluke/cloup) to add: - option groups -
-constraints - subcommands sections - aliases - command suggestion (`Did you
-mean ?`) ## Used in Check these projects to get real-life examples of `click-
-extra` usage: - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/
-meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager]
-(https://github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI
-for multiple package managers. - ![GitHub stars](https://img.shields.io/github/
-stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
-Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
-deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
-stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
-[fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
-rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
-stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
-(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse proxy for
-naming services on a local network. - ![GitHub stars](https://img.shields.io/
-github/stars/tclick/mdstab?label=%E2%AD%90&style=flat-square) [Molecular
-Dynamics Trajectory Analysis](https://github.com/tclick/mdstab#readme) Feel
-free to send a PR to add your project in this list if you are relying on Click
-Extra in any way. ## Development [Development guidelines](https://
-kdeldycke.github.io/meta-package-manager/development.html) are the same as
-[parent project `mpm`](https://github.com/kdeldycke/meta-package-manager), from
-which `click-extra` originated.
+option](https://kdeldycke.github.io/click-extra/parameters.html#show-params-
+option) to debug parameters defaults, values, environment variables and
+provenance - [Click parameters introspection](https://kdeldycke.github.io/
+click-extra/parameters.html#introspecting-parameters) - [Colorization of help
+screens](https://kdeldycke.github.io/click-extra/colorize.html) at the
+semantic-level of options, parameters, subheadings, choices, metavars and
+defaults - Global `show_envvar` option to display all environment variables in
+help screens - `-h`/`--help` option names (see [rant on other inconsistencies]
+(https://blog.craftyguy.net/cmdline-help/)) - `--color`/`--no-color` option
+flag - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code -
+Recognize traditional environment variable conventions: - `NO_COLOR` from [`no-
+color.org`](https://no-color.org) - `DO_NOT_TRACK` from
+[`consoledonottrack.com`](https://consoledonottrack.com) - Colored `--version`
+option - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/
+click-extra/logging.html) - `--time`/`--no-time` flag to measure duration of
+command execution - Global `show_choices` to activate selection of choices on
+user input prompts - [Platform recognition](https://kdeldycke.github.io/click-
+extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
+conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
+`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
+`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
+run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
+to document CLI source code and their execution - [Inline testing of CLI
+examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in
+documentation - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
+click-extra/pygments.html#lexers) for shell session and console output - [Fixes
+40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other
+Click-related projects - Rely on [Cloup](https://github.com/janluke/cloup) to
+add: - option groups - constraints - subcommands sections - aliases - command
+suggestion (`Did you mean ?`) ## Used in Check these projects to get real-life
+examples of `click-extra` usage: - ![GitHub stars](https://img.shields.io/
+github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square)
+[Meta Package Manager](https://github.com/kdeldycke/meta-package-
+manager#readme) \- A unifying CLI for multiple package managers. - ![GitHub
+stars](https://img.shields.io/github/stars/kdeldycke/mail-
+deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://
+github.com/kdeldycke/mail-deduplicate#readme) - A CLI to deduplicate similar
+emails. - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-
+Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://
+github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox
+tool. - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/
+badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/
+hugolundin/badger#readme) - An mDNS-based reverse proxy for naming services on
+a local network. Feel free to send a PR to add your project in this list if you
+are relying on Click Extra in any way. ## Development [Development guidelines]
+(https://kdeldycke.github.io/meta-package-manager/development.html) are the
+same as [parent project `mpm`](https://github.com/kdeldycke/meta-package-
+manager), from which `click-extra` originated.
```

