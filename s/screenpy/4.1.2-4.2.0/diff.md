# Comparing `tmp/screenpy-4.1.2.tar.gz` & `tmp/screenpy-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screenpy-4.1.2.tar", max compression
+gzip compressed data, was "screenpy-4.2.0.tar", max compression
```

## Comparing `screenpy-4.1.2.tar` & `screenpy-4.2.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1071 2023-02-03 04:58:53.259801 screenpy-4.1.2/LICENSE
--rw-r--r--   0        0        0     2688 2022-12-06 23:17:17.604373 screenpy-4.1.2/README.md
--rw-r--r--   0        0        0     3373 2023-02-03 14:41:28.061312 screenpy-4.1.2/pyproject.toml
--rw-r--r--   0        0        0     1275 2023-02-03 06:36:23.245620 screenpy-4.1.2/screenpy/__init__.py
--rw-r--r--   0        0        0      955 2023-02-03 04:58:53.265656 screenpy-4.1.2/screenpy/__version__.py
--rw-r--r--   0        0        0     1015 2022-02-23 04:24:47.235318 screenpy-4.1.2/screenpy/actions/__init__.py
--rw-r--r--   0        0        0     1043 2022-05-13 20:32:24.832168 screenpy-4.1.2/screenpy/actions/attach_the_file.py
--rw-r--r--   0        0        0     1442 2023-01-18 21:29:11.958649 screenpy-4.1.2/screenpy/actions/debug.py
--rw-r--r--   0        0        0     5682 2022-05-13 20:32:24.832920 screenpy-4.1.2/screenpy/actions/eventually.py
--rw-r--r--   0        0        0     2562 2022-12-06 23:17:17.605502 screenpy-4.1.2/screenpy/actions/make_note.py
--rw-r--r--   0        0        0     3144 2023-01-18 21:29:14.857475 screenpy-4.1.2/screenpy/actions/pause.py
--rw-r--r--   0        0        0     2358 2022-12-06 23:17:17.605778 screenpy-4.1.2/screenpy/actions/see.py
--rw-r--r--   0        0        0     2207 2022-12-06 23:17:17.605913 screenpy-4.1.2/screenpy/actions/see_all_of.py
--rw-r--r--   0        0        0     2517 2022-12-06 23:17:17.606041 screenpy-4.1.2/screenpy/actions/see_any_of.py
--rw-r--r--   0        0        0     8197 2023-02-03 05:28:29.752577 screenpy-4.1.2/screenpy/actor.py
--rw-r--r--   0        0        0      863 2022-05-12 21:09:06.646022 screenpy-4.1.2/screenpy/directions.py
--rw-r--r--   0        0        0     1011 2023-02-03 04:58:53.266070 screenpy-4.1.2/screenpy/director.py
--rw-r--r--   0        0        0      938 2022-02-23 04:24:47.247767 screenpy-4.1.2/screenpy/exceptions.py
--rw-r--r--   0        0        0     1415 2021-04-11 20:35:21.605562 screenpy-4.1.2/screenpy/given_when_then.py
--rw-r--r--   0        0        0      232 2023-02-03 14:34:45.651971 screenpy-4.1.2/screenpy/narration/__init__.py
--rw-r--r--   0        0        0      190 2023-02-03 05:49:46.971125 screenpy-4.1.2/screenpy/narration/adapters/__init__.py
--rw-r--r--   0        0        0     4773 2023-02-03 14:34:45.656332 screenpy-4.1.2/screenpy/narration/adapters/stdout_adapter.py
--rw-r--r--   0        0        0      293 2023-02-03 14:36:33.549592 screenpy-4.1.2/screenpy/narration/gravitas.py
--rw-r--r--   0        0        0     9445 2023-02-03 14:26:59.118621 screenpy-4.1.2/screenpy/narration/narrator.py
--rw-r--r--   0        0        0     3773 2023-02-03 14:22:22.197182 screenpy-4.1.2/screenpy/pacing.py
--rw-r--r--   0        0        0     3804 2023-02-03 14:08:37.632887 screenpy-4.1.2/screenpy/protocols.py
--rw-r--r--   0        0        0       39 2020-02-18 02:58:20.409661 screenpy-4.1.2/screenpy/py.typed
--rw-r--r--   0        0        0     2657 2023-02-03 04:59:40.887282 screenpy-4.1.2/screenpy/resolutions/__init__.py
--rw-r--r--   0        0        0     3056 2022-05-12 20:39:48.080661 screenpy-4.1.2/screenpy/resolutions/base_resolution.py
--rw-r--r--   0        0        0      825 2023-02-03 04:58:53.267303 screenpy-4.1.2/screenpy/resolutions/contains_item_matching.py
--rw-r--r--   0        0        0     1258 2022-05-12 20:39:48.081648 screenpy-4.1.2/screenpy/resolutions/contains_the_entry.py
--rw-r--r--   0        0        0      693 2022-05-12 20:39:48.082570 screenpy-4.1.2/screenpy/resolutions/contains_the_item.py
--rw-r--r--   0        0        0      655 2022-05-12 20:39:48.083351 screenpy-4.1.2/screenpy/resolutions/contains_the_key.py
--rw-r--r--   0        0        0      592 2022-05-12 20:39:48.084621 screenpy-4.1.2/screenpy/resolutions/contains_the_text.py
--rw-r--r--   0        0        0      692 2022-05-12 20:39:48.085861 screenpy-4.1.2/screenpy/resolutions/contains_the_value.py
--rw-r--r--   0        0        0        0 2023-02-03 04:58:53.267363 screenpy-4.1.2/screenpy/resolutions/custom_matchers/__init__.py
--rw-r--r--   0        0        0     3021 2023-02-03 06:29:01.936608 screenpy-4.1.2/screenpy/resolutions/custom_matchers/is_in_bounds.py
--rw-r--r--   0        0        0     1796 2023-02-03 04:58:53.267740 screenpy-4.1.2/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
--rw-r--r--   0        0        0      616 2023-02-03 04:58:53.267961 screenpy-4.1.2/screenpy/resolutions/ends_with.py
--rw-r--r--   0        0        0      608 2022-05-12 20:39:48.087033 screenpy-4.1.2/screenpy/resolutions/has_length.py
--rw-r--r--   0        0        0      850 2022-05-12 20:39:48.087981 screenpy-4.1.2/screenpy/resolutions/is_close_to.py
--rw-r--r--   0        0        0      491 2022-05-12 20:39:48.089002 screenpy-4.1.2/screenpy/resolutions/is_empty.py
--rw-r--r--   0        0        0      559 2022-05-12 20:39:48.092608 screenpy-4.1.2/screenpy/resolutions/is_equal_to.py
--rw-r--r--   0        0        0      638 2023-02-03 06:25:09.843884 screenpy-4.1.2/screenpy/resolutions/is_greater_than.py
--rw-r--r--   0        0        0      726 2023-02-03 06:24:46.343728 screenpy-4.1.2/screenpy/resolutions/is_greater_than_or_equal_to.py
--rw-r--r--   0        0        0     1002 2023-02-03 06:39:17.509870 screenpy-4.1.2/screenpy/resolutions/is_in_range.py
--rw-r--r--   0        0        0      652 2023-02-03 06:38:56.517246 screenpy-4.1.2/screenpy/resolutions/is_less_than.py
--rw-r--r--   0        0        0      724 2023-02-03 06:25:25.395918 screenpy-4.1.2/screenpy/resolutions/is_less_than_or_equal_to.py
--rw-r--r--   0        0        0      746 2022-05-12 20:39:48.093667 screenpy-4.1.2/screenpy/resolutions/is_not.py
--rw-r--r--   0        0        0      700 2023-02-03 04:58:53.268192 screenpy-4.1.2/screenpy/resolutions/matches.py
--rw-r--r--   0        0        0      559 2022-05-12 20:39:48.094570 screenpy-4.1.2/screenpy/resolutions/reads_exactly.py
--rw-r--r--   0        0        0      626 2023-02-03 04:58:53.268408 screenpy-4.1.2/screenpy/resolutions/starts_with.py
--rw-r--r--   0        0        0      256 2021-08-24 00:38:06.806795 screenpy-4.1.2/screenpy/settings.py
--rw-r--r--   0        0        0     1842 2022-12-06 23:17:17.606465 screenpy-4.1.2/screenpy/speech_tools.py
--rw-r--r--   0        0        0      912 2022-02-23 04:24:47.257184 screenpy-4.1.2/screenpy/test_utils.py
--rw-r--r--   0        0        0     4333 1970-01-01 00:00:00.000000 screenpy-4.1.2/setup.py
--rw-r--r--   0        0        0     5353 1970-01-01 00:00:00.000000 screenpy-4.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-02 03:55:36.644684 screenpy-4.2.0/LICENSE
+-rw-r--r--   0        0        0     2688 2023-06-02 03:55:36.644684 screenpy-4.2.0/README.md
+-rw-r--r--   0        0        0     3625 2023-06-02 03:55:36.644684 screenpy-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2360 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/__init__.py
+-rw-r--r--   0        0        0      955 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/__version__.py
+-rw-r--r--   0        0        0     1903 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/__init__.py
+-rw-r--r--   0        0        0     1049 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/attach_the_file.py
+-rw-r--r--   0        0        0     1442 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/debug.py
+-rw-r--r--   0        0        0     5733 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/eventually.py
+-rw-r--r--   0        0        0     1353 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/log.py
+-rw-r--r--   0        0        0     2597 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/make_note.py
+-rw-r--r--   0        0        0     3144 2023-06-02 03:55:36.644684 screenpy-4.2.0/screenpy/actions/pause.py
+-rw-r--r--   0        0        0     2337 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see.py
+-rw-r--r--   0        0        0     2246 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see_all_of.py
+-rw-r--r--   0        0        0     2628 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/see_any_of.py
+-rw-r--r--   0        0        0     4477 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actions/silently.py
+-rw-r--r--   0        0        0     9622 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/actor.py
+-rw-r--r--   0        0        0     3698 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/configuration.py
+-rw-r--r--   0        0        0      863 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/directions.py
+-rw-r--r--   0        0        0     1011 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/director.py
+-rw-r--r--   0        0        0     1401 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/exceptions.py
+-rw-r--r--   0        0        0     1415 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/given_when_then.py
+-rw-r--r--   0        0        0      369 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/gravitas.py
+-rw-r--r--   0        0        0     9445 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/narrator.py
+-rw-r--r--   0        0        0      278 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/__init__.py
+-rw-r--r--   0        0        0      943 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/configuration.py
+-rw-r--r--   0        0        0     4732 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/narration/stdout_adapter/stdout_adapter.py
+-rw-r--r--   0        0        0     3707 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/pacing.py
+-rw-r--r--   0        0        0     4126 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/protocols.py
+-rw-r--r--   0        0        0       39 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/py.typed
+-rw-r--r--   0        0        0     2657 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/__init__.py
+-rw-r--r--   0        0        0     3615 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/base_resolution.py
+-rw-r--r--   0        0        0     1061 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_item_matching.py
+-rw-r--r--   0        0        0     2375 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_entry.py
+-rw-r--r--   0        0        0      830 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_item.py
+-rw-r--r--   0        0        0      868 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_key.py
+-rw-r--r--   0        0        0      745 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_text.py
+-rw-r--r--   0        0        0      869 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/contains_the_value.py
+-rw-r--r--   0        0        0        0 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/__init__.py
+-rw-r--r--   0        0        0     2911 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/is_in_bounds.py
+-rw-r--r--   0        0        0     1796 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py
+-rw-r--r--   0        0        0      777 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/ends_with.py
+-rw-r--r--   0        0        0      870 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/has_length.py
+-rw-r--r--   0        0        0      897 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_close_to.py
+-rw-r--r--   0        0        0      613 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_empty.py
+-rw-r--r--   0        0        0      730 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_equal_to.py
+-rw-r--r--   0        0        0      772 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_greater_than.py
+-rw-r--r--   0        0        0      872 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_greater_than_or_equal_to.py
+-rw-r--r--   0        0        0     1677 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_in_range.py
+-rw-r--r--   0        0        0      761 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_less_than.py
+-rw-r--r--   0        0        0      845 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_less_than_or_equal_to.py
+-rw-r--r--   0        0        0      961 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/is_not.py
+-rw-r--r--   0        0        0      866 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/matches.py
+-rw-r--r--   0        0        0      733 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/reads_exactly.py
+-rw-r--r--   0        0        0      778 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/resolutions/starts_with.py
+-rw-r--r--   0        0        0     1890 2023-06-02 03:55:36.648684 screenpy-4.2.0/screenpy/speech_tools.py
+-rw-r--r--   0        0        0     5439 1970-01-01 00:00:00.000000 screenpy-4.2.0/PKG-INFO
```

### Comparing `screenpy-4.1.2/LICENSE` & `screenpy-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/README.md` & `screenpy-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/pyproject.toml` & `screenpy-4.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 # Poetry:
 #   poetry install --extras dev
 # PIP:
 #   pip install -e .[dev]
 
 [tool.poetry]
 name = "screenpy"
-version = "4.1.2"
-description = "Screenplay pattern base for Python automated UI test suites."
+version = "4.2.0"
+description = "Screenplay pattern base for Python automated test suites."
 authors = ["Perry Goy <perry.goy@gmail.com>"]
 maintainers = ["Gabe Langton", "Marcel Wilson"]
 license = "MIT"
 repository = "https://github.com/ScreenPyHQ/screenpy"
 documentation = "https://screenpy-docs.readthedocs.io"
 readme = "README.md"
 classifiers = [
@@ -44,14 +44,16 @@
 # Poetry users will need to use the `--extras dev` option rather than the `--with dev`
 # so we dont have two different sets of package versions to update.
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyHamcrest = ">=2.0.0"
 typing-extensions = ">=4.1.1"
+pydantic = "^1.10.7"
+tomli = "^2.0.1"
 importlib_metadata = {version = "*", python = "3.8.*"}
 
 # convenience packages for development of screenpy only
 pre-commit = {version = "*", optional = true}
 pytest = {version = "*", optional = true}
 tox = {version = "*", optional = true}
 mypy = {version = "*", optional = true}
@@ -62,40 +64,48 @@
 coverage = {version = "*", optional = true}
 screenpy-adapter_allure = {version = "^4.0.1", optional = true}
 screenpy-appium = {version = "*", optional = true}
 screenpy-playwright = {version = "*", optional = true}
 screenpy-pyotp = {version = "^4.0.1", optional = true}
 screenpy-requests = {version = "^4.0.1", optional = true}
 screenpy-selenium = {version = "^4.0.3", optional = true}
+sphinx = "^6.1.3"
+autodoc-pydantic = {version = "^1.8.0", optional = true}
+pytest-mock = {version = "*", optional = true}
 
 [tool.poetry.extras]
 allure = ["screenpy-adapter-allure"]
 appium = ["screenpy-appium"]
 playwright = ["screenpy-playwright"]
 pyotp = ["screenpy-pyotp"]
 requests = ["screenpy-requests"]
 selenium = ["screenpy-selenium"]
 dev = [
     "pre-commit",
     "pytest",
+    "pytest-mock",
     "tox",
     "pylint",
 ]
 dev_all = [
     "pre-commit",
     "pytest",
+    "pytest-mock",
     "tox",
     "pylint",
     "mypy",
     "black",
     "isort",
     "flake8",
     "coverage",
+    "sphinx",
+    "autodoc-pydantic",
 ]
 test = [
     "pytest",
+    "pytest-mock",
     "coverage",
 ]
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `screenpy-4.1.2/screenpy/__version__.py` & `screenpy-4.2.0/screenpy/__version__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/actions/attach_the_file.py` & `screenpy-4.2.0/screenpy/actions/attach_the_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Attach a file.
 """
 
 import os
 from typing import Any
 
-from screenpy import Actor
+from screenpy.actor import Actor
 from screenpy.pacing import the_narrator
 
 
 class AttachTheFile:
     """Attach a file for :ref:`Narration`.
 
     Supports passing arbitrary keyword arguments along to the adapters hooked
```

### Comparing `screenpy-4.1.2/screenpy/actions/debug.py` & `screenpy-4.2.0/screenpy/actions/debug.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/actions/eventually.py` & `screenpy-4.2.0/screenpy/actions/eventually.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Eventually perform a Task or Action, trying until a set timeout.
 """
 
 import time
-from typing import Optional, Set, Tuple
+from typing import Dict, Optional
 
-from screenpy import Actor, settings
+from screenpy.actor import Actor
+from screenpy.configuration import settings
 from screenpy.exceptions import DeliveryError
 from screenpy.pacing import beat, the_narrator
 from screenpy.protocols import Performable
 from screenpy.speech_tools import get_additive_description
 
 
 class Eventually:
@@ -52,15 +53,15 @@
 
         def __init__(
             self, eventually: "Eventually", amount: float, attribute: str
         ) -> None:
             self.eventually = eventually
             self.amount = amount
             self.attribute = attribute
-            self.eventually.timeout = amount
+            setattr(self.eventually, self.attribute, self.amount)
 
         def milliseconds(self) -> "Eventually":
             """Set the timeout in milliseconds."""
             setattr(self.eventually, self.attribute, self.amount / 1000)
             return self.eventually
 
         millisecond = milliseconds
@@ -133,30 +134,30 @@
             while True:
                 the_narrator.clear_backup()
                 try:
                     the_actor.attempts_to(self.performable)
                     return
                 except Exception as exc:  # pylint: disable=broad-except
                     self.caught_error = exc
-                    self.unique_errors.add((exc.__class__.__name__, str(exc)))
+                    self.unique_errors[exc] = None
 
                 count += 1
                 time.sleep(self.poll)
                 if time.time() > end_time:
                     break
 
         unique_errors_message = "\n    ".join(
-            f"{e[0]}: {e[1]}" for e in self.unique_errors
+            f"{e.__class__.__name__}: {e}" for e in self.unique_errors
         )
         msg = (
             f"{the_actor} tried to Eventually {self.performable_to_log} {count} times"
             f" over {self.timeout} seconds, but got:\n    {unique_errors_message}"
         )
         raise DeliveryError(msg) from self.caught_error
 
     def __init__(self, performable: Performable):
         self.performable = performable
         self.performable_to_log = get_additive_description(self.performable)
         self.caught_error = None
-        self.unique_errors: Set[Tuple[str, str]] = set()
+        self.unique_errors: Dict[Exception, None] = {}
         self.timeout = settings.TIMEOUT
-        self.poll = 0.5
+        self.poll = settings.POLLING
```

### Comparing `screenpy-4.1.2/screenpy/actions/make_note.py` & `screenpy-4.2.0/screenpy/actions/make_note.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Make a quick note about the answer to a Question.
 """
 
 from typing import Optional, Type, TypeVar, Union
 
-from screenpy import Actor, Director
+from screenpy.actor import Actor
+from screenpy.director import Director
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import aside, beat
 from screenpy.protocols import Answerable, ErrorKeeper
 
 SelfMakeNote = TypeVar("SelfMakeNote", bound="MakeNote")
 T_Q = Union[Answerable, object]
```

### Comparing `screenpy-4.1.2/screenpy/actions/pause.py` & `screenpy-4.2.0/screenpy/actions/pause.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/actions/see.py` & `screenpy-4.2.0/screenpy/actions/see.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Make an assertion using a Question and a Resolution.
 """
 
 from typing import Type, TypeVar, Union
 
 from hamcrest import assert_that
 
-from screenpy import Actor
+from screenpy.actor import Actor
 from screenpy.pacing import aside, beat
-from screenpy.protocols import Answerable, ErrorKeeper
-from screenpy.resolutions import BaseResolution
+from screenpy.protocols import Answerable, ErrorKeeper, Resolvable
 from screenpy.speech_tools import get_additive_description
 
 SelfSee = TypeVar("SelfSee", bound="See")
 T_Q = Union[Answerable, object]
+T_R = Resolvable
 
 
 class See:
     """See if a value or the answer to a Question matches the Resolution.
 
     This is a very important Action in ScreenPy. It is the way to perform
     test assertions. For more information, see the documentation for
@@ -32,19 +32,19 @@
         the_actor.should(
             See.the(list_of_items, ContainsTheItem("juice extractor")),
         )
     """
 
     question: T_Q
     question_to_log: str
-    resolution: BaseResolution
+    resolution: T_R
     resolution_to_log: str
 
     @classmethod
-    def the(cls: Type[SelfSee], question: T_Q, resolution: BaseResolution) -> SelfSee:
+    def the(cls: Type[SelfSee], question: T_Q, resolution: T_R) -> SelfSee:
         """Supply the Question (or value) and Resolution to test."""
         return cls(question, resolution)
 
     def describe(self: SelfSee) -> str:
         """Describe the Action in present tense."""
         return f"See if {self.question_to_log} is {self.resolution_to_log}."
 
@@ -58,14 +58,14 @@
             value = self.question
             aside(f"the actual value is: {value}")
 
         reason = ""
         if isinstance(self.question, ErrorKeeper):
             reason = f"{self.question.caught_exception}"
 
-        assert_that(value, self.resolution, reason)
+        assert_that(value, self.resolution.resolve(), reason)
 
-    def __init__(self: SelfSee, question: T_Q, resolution: BaseResolution) -> None:
+    def __init__(self: SelfSee, question: T_Q, resolution: T_R) -> None:
         self.question = question
         self.question_to_log = get_additive_description(question)
         self.resolution = resolution
-        self.resolution_to_log = resolution.get_line()
+        self.resolution_to_log = get_additive_description(resolution)
```

### Comparing `screenpy-4.1.2/screenpy/actions/see_all_of.py` & `screenpy-4.2.0/screenpy/actions/see_all_of.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Make several assertions using any number of Question and Resolution tuples,
 all of which are expected to be true.
 """
 
-from typing import Tuple, Type, TypeVar, Union
+from typing import Tuple, Type, TypeVar
 
-from screenpy import Actor
+from screenpy.actor import Actor
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import beat
-from screenpy.protocols import Answerable
-from screenpy.resolutions import BaseResolution
 
-from .see import See
+from .see import T_Q, T_R, See
 
 SelfSeeAllOf = TypeVar("SelfSeeAllOf", bound="SeeAllOf")
-T_T = Tuple[Union[Answerable, object], BaseResolution]
+T_T = Tuple[T_Q, T_R]
 
 
 class SeeAllOf:
     """See if all the provided values or Questions match their Resolutions.
 
     Uses :class:`~screenpy.actions.See` to assert all values or the answers to
     the :ref:`Questions` match their paired :ref:`Resolutions`:.
@@ -44,25 +42,30 @@
     @classmethod
     def the(cls: Type[SelfSeeAllOf], *tests: T_T) -> SelfSeeAllOf:
         """Supply any number of Question/value + Resolution tuples to test."""
         return cls(*tests)
 
     def describe(self: SelfSeeAllOf) -> str:
         """Describe the Action in present tense."""
-        return f"See if all of {self.number_of_tests} tests pass."
+        return f"See if {self.log_message}."
 
-    @beat("{} sees if all of the following {number_of_tests} tests pass:")
+    @beat("{} sees if {log_message}:")
     def perform_as(self: SelfSeeAllOf, the_actor: Actor) -> None:
         """Direct the Actor to make a series of observations."""
         for question, resolution in self.tests:
             the_actor.should(See.the(question, resolution))
 
     def __init__(self: SelfSeeAllOf, *tests: T_T) -> None:
         for tup in tests:
             if isinstance(tup, tuple):
                 if len(tup) != 2:
-                    raise UnableToAct("Tuple must contain Question and Resolution")
+                    raise UnableToAct("Tuple must contain Question and Resolution.")
             else:
-                raise TypeError("Arguments must be tuples")
+                raise TypeError("Arguments must be tuples.")
 
         self.tests = tests
-        self.number_of_tests = len(tests)
+        if len(self.tests) == 0:
+            self.log_message = "no tests pass 🤔"
+        elif len(self.tests) == 1:
+            self.log_message = "1 test passes"
+        else:
+            self.log_message = f"all of {len(self.tests)} tests pass"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `screenpy-4.1.2/screenpy/actions/see_any_of.py` & `screenpy-4.2.0/screenpy/actions/see_any_of.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 Make several assertions using any number of Question and Resolution tuples,
 at least one of which is expected to be true.
 """
 
-from typing import Tuple, Type, TypeVar, Union
+from typing import Tuple, Type, TypeVar
 
-from screenpy import Actor
+from screenpy.actor import Actor
 from screenpy.exceptions import UnableToAct
 from screenpy.pacing import beat
-from screenpy.protocols import Answerable
-from screenpy.resolutions import BaseResolution
 
-from .see import See
+from .see import T_Q, T_R, See
 
 SelfSeeAnyOf = TypeVar("SelfSeeAnyOf", bound="SeeAnyOf")
-T_T = Tuple[Union[Answerable, object], BaseResolution]
+T_T = Tuple[T_Q, T_R]
 
 
 class SeeAnyOf:
     """See if at least one value or Question matches its Resolution.
 
     Uses :class:`~screenpy.actions.See` to assert at least one of the
     values or the answers to the :ref:`Questions` match their paired
@@ -45,33 +43,42 @@
     @classmethod
     def the(cls: Type[SelfSeeAnyOf], *tests: T_T) -> SelfSeeAnyOf:
         """Supply any number of Question/value + Resolution tuples to test."""
         return cls(*tests)
 
     def describe(self: SelfSeeAnyOf) -> str:
         """Describe the Action in present tense."""
-        return f"See if any of {self.number_of_tests} tests pass."
+        return f"See if {self.log_message}."
 
-    @beat("{} sees if any of the following {number_of_tests} tests pass:")
+    @beat("{} sees if {log_message}:")
     def perform_as(self: SelfSeeAnyOf, the_actor: Actor) -> None:
         """Direct the Actor to make a series of observations."""
-        none_passed = True
+        if not self.tests:
+            # No tests is OK!
+            return
+
         for question, resolution in self.tests:
             try:
                 the_actor.should(See.the(question, resolution))
-                none_passed = False
+                break
             except AssertionError:
                 pass  # well, not *pass*, but... you get it.
-
-        if none_passed:
-            raise AssertionError(f"{the_actor} did not find any expected answers!")
+        else:
+            # none passed!
+            msg = f"{the_actor} did not find any expected answers!"
+            raise AssertionError(msg)
 
     def __init__(self: SelfSeeAnyOf, *tests: T_T) -> None:
         for tup in tests:
             if isinstance(tup, tuple):
                 if len(tup) != 2:
                     raise UnableToAct("Tuple must contain Question and Resolution")
             else:
                 raise TypeError("Arguments must be tuples")
 
         self.tests = tests
-        self.number_of_tests = len(tests)
+        if len(self.tests) == 0:
+            self.log_message = "no tests pass 🤔"
+        elif len(self.tests) == 1:
+            self.log_message = "1 test passes"
+        else:
+            self.log_message = f"any of {len(self.tests)} tests pass"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `screenpy-4.1.2/screenpy/actor.py` & `screenpy-4.2.0/screenpy/actor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Actors are the stars of the show. They perform your Actions, ask Questions
 about the state of the application, and assert Resolutions, all in the
 service of perfoming their roles.
 """
 
-import warnings
 from random import choice
 from typing import List, Type, TypeVar
 
 from .exceptions import UnableToPerform
 from .pacing import aside
 from .protocols import Forgettable, Performable
 from .speech_tools import get_additive_description
@@ -67,24 +66,14 @@
         self.abilities.extend(abilities)
         return self
 
     def can(self: SelfActor, *abilities: T_Ability) -> SelfActor:
         """Alias for :meth:`~screenpy.actor.Actor.who_can`."""
         return self.who_can(*abilities)
 
-    def has_cleanup_tasks(self: SelfActor, *tasks: Performable) -> SelfActor:
-        """Assign one or more tasks to the Actor to perform when exiting."""
-        warnings.warn(
-            "This method is deprecated and will be removed in ScreenPy 4.2.0."
-            " Please use either `has_ordered_cleanup_tasks`"
-            " or `has_independent_cleanup_tasks` instead.",
-            DeprecationWarning,
-        )
-        return self.has_ordered_cleanup_tasks(*tasks)
-
     def has_ordered_cleanup_tasks(self: SelfActor, *tasks: Performable) -> SelfActor:
         """Assign one or more tasks for the Actor to perform when exiting.
 
         The tasks given to this method must be performed successfully in
         order. If any task fails, any subsequent tasks will not be attempted
         and will be discarded.
 
@@ -148,24 +137,64 @@
 
     def attempts_to(self: SelfActor, *actions: Performable) -> None:
         """Perform a list of Actions, one after the other.
 
         Aliases:
             * :meth:`~screenpy.actor.Actor.was_able_to`
             * :meth:`~screenpy.actor.Actor.should`
+            * :meth:`~screenpy.actor.Actor.shall`
+            * :meth:`~screenpy.actor.Actor.will`
+            * :meth:`~screenpy.actor.Actor.tries_to`
+            * :meth:`~screenpy.actor.Actor.tried_to`
+            * :meth:`~screenpy.actor.Actor.tries`
+            * :meth:`~screenpy.actor.Actor.tried`
+            * :meth:`~screenpy.actor.Actor.does`
+            * :meth:`~screenpy.actor.Actor.did`
         """
         for action in actions:
             self.perform(action)
 
     def was_able_to(self: SelfActor, *actions: Performable) -> None:
-        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`, for test setup."""
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def tries_to(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def tried_to(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def tries(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def tried(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def does(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def did(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def will(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
+    def shall(self: SelfActor, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
         return self.attempts_to(*actions)
 
     def should(self: SelfActor, *actions: Performable) -> None:
-        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`, for test assertions."""
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
         return self.attempts_to(*actions)
 
     def perform(self: SelfActor, action: Performable) -> None:
         """Perform an Action."""
         action.perform_as(self)
 
     def cleans_up_ordered_tasks(self: SelfActor) -> None:
@@ -217,14 +246,18 @@
         """Alias for :meth:`~screenpy.actor.Actor.exit`."""
         return self.exit()
 
     def exit_through_vomitorium(self: SelfActor) -> None:
         """Alias for :meth:`~screenpy.actor.Actor.exit`."""
         return self.exit()
 
+    def __call__(self, *actions: Performable) -> None:
+        """Alias for :meth:`~screenpy.actor.Actor.attempts_to`."""
+        return self.attempts_to(*actions)
+
     def __repr__(self: SelfActor) -> str:
         return self.name
 
     def __init__(self: SelfActor, name: str) -> None:
         self.name = name
         self.abilities = []
         self.ordered_cleanup_tasks = []
```

### Comparing `screenpy-4.1.2/screenpy/directions.py` & `screenpy-4.2.0/screenpy/directions.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/director.py` & `screenpy-4.2.0/screenpy/director.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/exceptions.py` & `screenpy-4.2.0/screenpy/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,7 +37,27 @@
 
 class QuestionError(ScreenPyError):
     """These errors are raised when a Question fails."""
 
 
 class UnableToAnswer(QuestionError):
     """The Question is not answerable."""
+
+
+class ResolutionError(ScreenPyError):
+    """These errors are raised when a Resolution fails."""
+
+
+class UnableToFormResolution(ResolutionError):
+    """The Resolution is unable to be formed."""
+
+
+class NotPerformable(ScreenPyError):
+    """Does not conform to Performable Protocol"""
+
+
+class NotAnswerable(ScreenPyError):
+    """Does not conform to Answerable Protocol"""
+
+
+class NotResolvable(ScreenPyError):
+    """Does not conform to Resolvable Protocol"""
```

### Comparing `screenpy-4.1.2/screenpy/given_when_then.py` & `screenpy-4.2.0/screenpy/given_when_then.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/narration/adapters/stdout_adapter.py` & `screenpy-4.2.0/screenpy/narration/stdout_adapter/stdout_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 """
 
 import logging
 from contextlib import contextmanager
 from functools import wraps
 from typing import Any, Callable, Generator, List, Optional
 
-from screenpy import settings
-
 from ..gravitas import AIRY, EXTREME, HEAVY, LIGHT, NORMAL
+from .configuration import settings
 
 # pylint: disable=unused-argument
 
 
 class StdOutManager:
     """Handle the indentation, formatting, and log action for CLI logging."""
 
     def __init__(self, logger: Optional[logging.Logger] = None) -> None:
         self.logger = logger or logging.getLogger("screenpy")
         self.depth: List[str] = []
-        self.whitespace = settings.INDENT_SIZE * settings.INDENT_CHAR
-        self.enabled = settings.INDENT_LOGS
 
     @contextmanager
     def _indent(self) -> Generator:
         """Increase the indentation level."""
         # We want this indentation to last until we explicitly call _outdent.
         # Keeping something created in this context alive in our depth gauge
         # will persist the context until we pop it off and discard it later!
@@ -36,15 +33,16 @@
     def _outdent(self) -> None:
         """Decrease the indentation level."""
         if self.depth:
             self.depth.pop()
 
     def log(self, line: str, level: int = logging.INFO) -> None:
         """Log a line!"""
-        indent = len(self.depth) * self.whitespace if self.enabled else ""
+        whitespace = settings.INDENT_SIZE * settings.INDENT_CHAR
+        indent = len(self.depth) * whitespace if settings.INDENT_LOGS else ""
         self.logger.log(level, f"{indent}{line}")
 
     @contextmanager
     def log_context(self, line: str, level: int = logging.INFO) -> Generator:
         """Log a line, increasing the indent depth for nested logs."""
         self.log(line, level)
         try:
```

### Comparing `screenpy-4.1.2/screenpy/narration/narrator.py` & `screenpy-4.2.0/screenpy/narration/narrator.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/pacing.py` & `screenpy-4.2.0/screenpy/pacing.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 run through all of the Narrator's adapters.
 """
 
 import re
 from functools import wraps
 from typing import Any, Callable, Optional
 
-from screenpy.narration.adapters.stdout_adapter import StdOutAdapter
-from screenpy.narration.narrator import Narrator
+from screenpy.narration import Narrator, StdOutAdapter
 
 Function = Callable[..., Any]
 the_narrator: Narrator = Narrator(adapters=[StdOutAdapter()])
 
 
 def act(title: str, gravitas: Optional[str] = None) -> Callable[[Function], Function]:
     """Decorator to mark an "act".
@@ -78,15 +77,15 @@
     """
 
     def decorator(func: Function) -> Function:
         @wraps(func)
         def wrapper(*args: Any, **kwargs: Any) -> Any:
             action = args[0] if len(args) > 0 else None
             actor = args[1] if len(args) > 1 else ""
-            markers = re.findall(r"\{([^0-9\}]+)}", line)
+            markers = re.findall(r"\{([^\}]+)}", line)
             cues = {mark: getattr(action, mark) for mark in markers}
 
             completed_line = f"{line.format(actor, **cues)}"
             with the_narrator.stating_a_beat(func, completed_line, gravitas) as n_func:
                 retval = n_func(*args, **kwargs)
                 if retval is not None:
                     aside(f"=> {retval}")
```

### Comparing `screenpy-4.1.2/screenpy/protocols.py` & `screenpy-4.2.0/screenpy/protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 any class that implements ``perform_as`` can be an Action, any class that
 implements ``answered_by`` is a Question, etc. For more information, see
 https://mypy.readthedocs.io/en/stable/protocols.html
 """
 
 from typing import TYPE_CHECKING, Any, Callable, Generator, Optional
 
+from hamcrest.core.base_matcher import Matcher
 from typing_extensions import Protocol, runtime_checkable
 
 if TYPE_CHECKING:
     from .actor import Actor
 
 # pylint: disable=unused-argument
 
@@ -32,14 +33,29 @@
 
         Returns:
             The answer, based on the sleuthing the Actor has done.
         """
 
 
 @runtime_checkable
+class Describable(Protocol):
+    """Classes that describe themselves are Describable"""
+
+    def describe(self) -> str:
+        """Describe the Describable in the present tense."""
+
+
+@runtime_checkable
+class ErrorKeeper(Protocol):
+    """Classes that save exceptions for later are ErrorKeeper(s)"""
+
+    caught_exception: Optional[Exception]
+
+
+@runtime_checkable
 class Forgettable(Protocol):
     """Abilities are Forgettable"""
 
     def forget(self) -> None:
         """
         Forget this Ability by doing any necessary cleanup (quitting browsers,
         closing connections, etc.)
@@ -56,26 +72,23 @@
 
         Args:
             the_actor: the Actor who will perform this Action.
         """
 
 
 @runtime_checkable
-class ErrorKeeper(Protocol):
-    """Classes that save exceptions for later are ErrorKeeper(s)"""
+class Resolvable(Protocol):
+    """Resolutions are Resolvable"""
 
-    caught_exception: Optional[Exception]
+    def resolve(self) -> Matcher:
+        """Form the Matcher for an assertion.
 
-
-@runtime_checkable
-class Describable(Protocol):
-    """Classes that describe themselves are Describable"""
-
-    def describe(self) -> str:
-        """Describe the Describable in the present tense."""
+        Returns:
+            Matcher: the Matcher this Resolution uses for the expected value.
+        """
 
 
 @runtime_checkable
 class Adapter(Protocol):
     """Required functions for an adapter to the Narrator's microphone.
 
     Adapters allow the :ref:`Narrator <narrator api>`'s microphone to
```

### Comparing `screenpy-4.1.2/screenpy/resolutions/__init__.py` & `screenpy-4.2.0/screenpy/resolutions/__init__.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/resolutions/base_resolution.py` & `screenpy-4.2.0/screenpy/resolutions/base_resolution.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 with a Question to get the actual value. An assertion might look like:
 
     Perry.should(
         See.the(Text.of(THE_WELCOME_MESSAGE), ReadsExactly("Welcome!")),
     )
 """
 
+import warnings
 from typing import Any, Callable, TypeVar
 
 from hamcrest.core.base_matcher import BaseMatcher, Matcher
 from hamcrest.core.description import Description
 
 from ..pacing import beat
 
@@ -26,26 +27,34 @@
     """Base class for Resolutions, ScreenPy's "expected value".
 
     An abstraction barrier for PyHamcrest's matchers. Allows for natural
     language assertions and hooks into ScreenPy's logging framework.
 
     You probably shouldn't expect to call any of the defined methods on
     this class or any inherited classes. Just pass an instantiated
-    Resolution to your |Actor|, they'll know what to do with it.
+    Resolution to your Actor, they'll know what to do with it.
     """
 
     matcher: Matcher
     matcher_function: Callable
     expected: Any
     line = (
         "-- I'm sorry, this Resolution did not provide a line. Please define a more "
         "descriptive line for this custom Resolution such that it completes the "
         'phrase: "hoping it\'s...".'
     )
 
+    def describe(self) -> str:
+        """Describe the Resolution's expectation."""
+        return self.get_line().capitalize()
+
+    def resolve(self) -> BaseMatcher[T]:
+        """Produce the Matcher to make the assertion."""
+        return self
+
     @beat("... hoping it's {motivation}")
     def _matches(self, item: T) -> bool:
         """passthrough to the matcher's method."""
         return self.matcher.matches(item)
 
     def describe_to(self, description: Description) -> None:
         """passthrough to the matcher's method."""
@@ -65,14 +74,20 @@
 
     @property
     def motivation(self) -> str:
         """Used to provide fancy logging for the allure report."""
         return self.get_line()
 
     def __init__(self, *args: object, **kwargs: object) -> None:
+        warnings.warn(
+            "BaseResolution is deprecated and will be removed in ScreenPy v5.0.0."
+            " Please make your Resolution Resolvable instead."
+            "\nSee https://screenpy-docs.readthedocs.io/en/latest/deprecations.html",
+            DeprecationWarning,
+        )
         cls = self.__class__
         if args and kwargs:
             self.expected = (args, kwargs)
             self.matcher = cls.matcher_function(*args, **kwargs)
         elif args:
             self.expected = args if len(args) > 1 else args[0]
             self.matcher = cls.matcher_function(*args)
```

### Comparing `screenpy-4.1.2/screenpy/resolutions/contains_item_matching.py` & `screenpy-4.2.0/screenpy/resolutions/contains_item_matching.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """
 Matches a sequence which contains an item matching a given regex pattern.
 """
 
-from .base_resolution import BaseResolution
-from .custom_matchers.sequence_containing_pattern import (
-    IsSequenceContainingPattern,
-    has_item_matching,
-)
+from typing import Sequence
 
+from hamcrest.core.matcher import Matcher
 
-class ContainsItemMatching(BaseResolution):
+from screenpy.pacing import beat
+
+from .custom_matchers.sequence_containing_pattern import has_item_matching
+
+
+class ContainsItemMatching:
     """Match a sequence containing an item matching a regular expression.
 
     Examples::
 
         the_actor.should(
             # matches "Spam...", "Spam spam...", "Spam spam spam..."
             See.the(Text.of_all(MENU_ITEMS), ContainsItemMatching(r"^([Ss]pam ?)+"))
         )
     """
 
-    matcher: IsSequenceContainingPattern
-    line = 'a sequence with an item matching the regular expression "{expectation}".'
-    matcher_function = has_item_matching
+    def describe(self) -> str:
+        """Describe the Resolution's expectation."""
+        return f'A sequence with an item matching the pattern r"{self.pattern}".'
+
+    @beat('... hoping it contains an item matching the pattern r"{pattern}".')
+    def resolve(self) -> Matcher[Sequence[str]]:
+        """Produce the Matcher to make the assertion."""
+        return has_item_matching(self.pattern)
 
-    def __init__(self, match: str) -> None:
-        super().__init__(match)
+    def __init__(self, pattern: str) -> None:
+        self.pattern = pattern
```

### Comparing `screenpy-4.1.2/screenpy/resolutions/custom_matchers/is_in_bounds.py` & `screenpy-4.2.0/screenpy/resolutions/custom_matchers/is_in_bounds.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,54 +8,50 @@
 import operator
 import re
 from typing import Callable, Union
 
 from hamcrest.core.base_matcher import BaseMatcher
 from hamcrest.core.description import Description
 
-InequalityFunc = Callable[[Union[int, float], Union[int, float]], bool]
+InequalityFunc = Callable[[float, float], bool]
 
 
-class IsInBounds(BaseMatcher[int]):
+class IsInBounds(BaseMatcher[float]):
     """Matches a number which is in the given range."""
 
     def __init__(
         self,
-        minorant: Union[int, float],
+        minorant: float,
         lower_comparator: InequalityFunc,
         upper_comparator: InequalityFunc,
-        majorant: Union[int, float],
+        majorant: float,
     ) -> None:
         self.minorant = minorant
         self.lower_comparator = lower_comparator
         self.upper_comparator = upper_comparator
         self.majorant = majorant
 
-    def _matches(self, item: Union[int, float]) -> bool:
+    def _matches(self, item: float) -> bool:
         matches_lower = self.lower_comparator(self.minorant, item)
         matches_upper = self.upper_comparator(item, self.majorant)
         return matches_lower and matches_upper
 
     def describe_to(self, description: Description) -> None:
         """Describe the passing case."""
         description.append_text(
             f"the number is within the range of {self.minorant} and {self.majorant}"
         )
 
-    def describe_match(
-        self, item: Union[int, float], match_description: Description
-    ) -> None:
+    def describe_match(self, item: float, match_description: Description) -> None:
         """Describe the match."""
         match_description.append_text(
             f"{item} was within the range of {self.minorant} and {self.majorant}"
         )
 
-    def describe_mismatch(
-        self, item: Union[int, float], mismatch_description: Description
-    ) -> None:
+    def describe_mismatch(self, item: float, mismatch_description: Description) -> None:
         """Describe the failing case."""
         mismatch_description.append_text(
             f"{item} does not fall within the range of"
             f" {self.minorant} and {self.majorant}"
         )
```

### Comparing `screenpy-4.1.2/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py` & `screenpy-4.2.0/screenpy/resolutions/custom_matchers/sequence_containing_pattern.py`

 * *Files identical despite different names*

### Comparing `screenpy-4.1.2/screenpy/resolutions/is_close_to.py` & `screenpy-4.2.0/screenpy/resolutions/is_close_to.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """
 Matches a value that falls within the range specified by the given delta.
 """
 
 from hamcrest import close_to
-from hamcrest.library.number.iscloseto import IsCloseTo as _IsCloseTo
+from hamcrest.core.matcher import Matcher
 
-from .base_resolution import BaseResolution
+from screenpy.pacing import beat
 
 
-class IsCloseTo(BaseResolution):
+class IsCloseTo:
     """Matches a value that falls within the range specified by the given delta.
 
     Examples::
 
         the_actor.should(
             See.the(Number.of(BALLOONS), IsCloseTo(FILLED_BALLOONS_COUNT, delta=25))
         )
     """
 
-    matcher: _IsCloseTo
-    matcher_function = close_to
-
-    def get_line(self) -> str:
-        """Get the line that describes this Resolution."""
-        args, kwargs = self.expected
-        return f"a value at most {kwargs['delta']} away from {args[0]}."
+    def describe(self) -> str:
+        """Describe the Resolution's expectation."""
+        return f"At most {self.delta} away from {self.num}."
+
+    @beat("... hoping it's at most {delta} away from {num}.")
+    def resolve(self) -> Matcher[float]:
+        """Produce the Matcher to make the assertion."""
+        return close_to(self.num, self.delta)
 
     def __init__(self, num: int, delta: int = 1) -> None:
-        super().__init__(num, delta=delta)
+        self.num = num
+        self.delta = delta
```

### Comparing `screenpy-4.1.2/screenpy/resolutions/matches.py` & `screenpy-4.2.0/screenpy/resolutions/matches.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """
 Matches a string using a regex pattern.
 """
 
 from hamcrest import matches_regexp
-from hamcrest.library.text.stringmatches import StringMatchesPattern
+from hamcrest.core.matcher import Matcher
 
-from .base_resolution import BaseResolution
+from screenpy.pacing import beat
 
 
-class Matches(BaseResolution):
+class Matches:
     """Match a string using a regular expression.
 
     Examples::
 
         the_actor.should(
             # matches "/product/1", "/product/22", "/product/942"...
             See.the(Text.of_the(URL), Matches(r"/product/[0-9]{1,3}"))
         )
     """
 
-    matcher: StringMatchesPattern
-    line = 'text matching the regular expression "{expectation}".'
-    matcher_function = matches_regexp
+    def describe(self) -> str:
+        """Describe the Resolution's expectation."""
+        return f'Text matching the pattern r"{self.pattern}".'
+
+    @beat('... hoping it\'s text matching the pattern r"{pattern}".')
+    def resolve(self) -> Matcher[str]:
+        """Produce the Matcher to make the assertion."""
+        return matches_regexp(self.pattern)
 
-    def __init__(self, match: str) -> None:
-        super().__init__(match)
+    def __init__(self, pattern: str) -> None:
+        self.pattern = pattern
```

### Comparing `screenpy-4.1.2/screenpy/speech_tools.py` & `screenpy-4.2.0/screenpy/speech_tools.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """
 A grab-bag of useful language-massaging functions with broad applicability.
 """
 
 import re
 from typing import Any, Union
 
-from screenpy.protocols import Answerable, Describable, Performable
+from screenpy.protocols import Answerable, Describable, Performable, Resolvable
 
 
-def get_additive_description(
-    describable: Union[Performable, Answerable, Describable, Any]
-) -> str:
+def get_additive_description(describable: Union[Describable, Any]) -> str:
     """Extract a description that can be placed within a sentence.
 
-    The ``describe`` method of Performables and Answerables will provide a
-    description in present tense, capitalized and with punctuation at the end.
-    Lower that case, remove that punctuation; bam! You can stick that in the
-    middle of a different sentence.
+    The ``describe`` method of Describables will provide a description,
+    capitalized and with punctuation at the end. Lower that case, remove that
+    punctuation; bam! You can stick that in the middle of a new sentence.
 
     If there is no ``describe`` method, try to create a description using the
-    class name by replacing each capital letter with a space and a lower-case
+    class name: replace each capital letter with a space and a lower-case
     letter (e.g. "BuildItAndTheyWillCome" -> "build it and they will come").
 
-    If the describable does not appear to be an Answerable or Performable,
-    stick a "the" in front of the class name. This should make it read like
-    "the list" or "the str".
+    If the object does not appear to be any -able, stick a "the" in front of
+    the class name. This should make it read like "the list" or "the str".
+
+    Args:
+        describable: the object to attempt to describe.
+
+    Returns:
+        str: the string to place within another string.
     """
     if isinstance(describable, Describable):
         description = describable.describe()  # type: ignore # see PEP 544
         if description:
             description = description[0].lower() + description[1:]
             description = re.sub(r"[.,?!;:]*$", r"", description)
         else:
             description = "something indescribable"
-    elif isinstance(describable, (Answerable, Performable)):
+    elif isinstance(describable, (Answerable, Performable, Resolvable)):
         # No describe method, so fabricate a description from the class name.
         description = describable.__class__.__name__
         description = re.sub(r"(?<!^)([A-Z])", r" \1", description).lower()
     else:
-        # Neither describable nor Answerable/Performable, must be a value.
+        # Neither Describable nor any other -able, must be a value.
         description = f"the {describable.__class__.__name__}"
 
     return description
```

### Comparing `screenpy-4.1.2/PKG-INFO` & `screenpy-4.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: screenpy
-Version: 4.1.2
-Summary: Screenplay pattern base for Python automated UI test suites.
+Version: 4.2.0
+Summary: Screenplay pattern base for Python automated test suites.
 Home-page: https://github.com/ScreenPyHQ/screenpy
 License: MIT
 Author: Perry Goy
 Author-email: perry.goy@gmail.com
 Maintainer: Gabe Langton
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,46 +15,47 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: BDD
 Provides-Extra: allure
 Provides-Extra: appium
 Provides-Extra: dev
 Provides-Extra: dev-all
 Provides-Extra: playwright
 Provides-Extra: pyotp
 Provides-Extra: requests
 Provides-Extra: selenium
 Provides-Extra: test
 Requires-Dist: PyHamcrest (>=2.0.0)
+Requires-Dist: autodoc-pydantic (>=1.8.0,<2.0.0) ; extra == "dev-all"
 Requires-Dist: black ; extra == "dev-all"
 Requires-Dist: coverage ; extra == "dev-all" or extra == "test"
 Requires-Dist: flake8 ; extra == "dev-all"
-Requires-Dist: importlib_metadata ; python_full_version >= "3.8.0" and python_full_version < "3.9.0"
+Requires-Dist: importlib_metadata ; python_version >= "3.8.dev0" and python_version < "3.9.dev0"
 Requires-Dist: isort ; extra == "dev-all"
 Requires-Dist: mypy ; extra == "dev-all"
 Requires-Dist: pre-commit ; extra == "dev" or extra == "dev-all"
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pylint ; extra == "dev" or extra == "dev-all"
 Requires-Dist: pytest ; extra == "dev" or extra == "dev-all" or extra == "test"
+Requires-Dist: pytest-mock ; extra == "dev" or extra == "dev-all" or extra == "test"
 Requires-Dist: screenpy-adapter_allure (>=4.0.1,<5.0.0) ; extra == "allure"
 Requires-Dist: screenpy-appium ; extra == "appium"
 Requires-Dist: screenpy-playwright ; extra == "playwright"
 Requires-Dist: screenpy-pyotp (>=4.0.1,<5.0.0) ; extra == "pyotp"
 Requires-Dist: screenpy-requests (>=4.0.1,<5.0.0) ; extra == "requests"
 Requires-Dist: screenpy-selenium (>=4.0.3,<5.0.0) ; extra == "selenium"
+Requires-Dist: sphinx (>=6.1.3,<7.0.0) ; extra == "dev-all"
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tox ; extra == "dev" or extra == "dev-all"
 Requires-Dist: typing-extensions (>=4.1.1)
 Project-URL: Documentation, https://screenpy-docs.readthedocs.io
 Project-URL: Repository, https://github.com/ScreenPyHQ/screenpy
 Description-Content-Type: text/markdown
 
 ScreenPy
```

