# Comparing `tmp/kiwi_cogs-0.1.1.tar.gz` & `tmp/kiwi_cogs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwi_cogs-0.1.1.tar", max compression
+gzip compressed data, was "kiwi_cogs-0.1.2.tar", max compression
```

## Comparing `kiwi_cogs-0.1.1.tar` & `kiwi_cogs-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/LICENSE
--rw-r--r--   0        0        0     6014 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/README.md
--rw-r--r--   0        0        0      169 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/__init__.py
--rw-r--r--   0        0        0     2528 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/event.py
--rw-r--r--   0        0        0      210 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/exceptions.py
--rw-r--r--   0        0        0     7700 2023-06-02 10:31:28.591719 kiwi_cogs-0.1.1/kiwi_cogs/machine.py
--rw-r--r--   0        0        0    10253 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/state.py
--rw-r--r--   0        0        0     4098 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/transition.py
--rw-r--r--   0        0        0      465 2023-06-02 10:31:28.595719 kiwi_cogs-0.1.1/kiwi_cogs/utils.py
--rw-r--r--   0        0        0     2061 2023-06-02 10:31:50.964050 kiwi_cogs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6735 1970-01-01 00:00:00.000000 kiwi_cogs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6014 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/README.md
+-rw-r--r--   0        0        0      211 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/__init__.py
+-rw-r--r--   0        0        0     2542 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/event.py
+-rw-r--r--   0        0        0      210 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/exceptions.py
+-rw-r--r--   0        0        0     7734 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/machine.py
+-rw-r--r--   0        0        0    10289 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/state.py
+-rw-r--r--   0        0        0     4105 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/transition.py
+-rw-r--r--   0        0        0      465 2023-06-02 21:20:16.573785 kiwi_cogs-0.1.2/kiwi_cogs/utils.py
+-rw-r--r--   0        0        0     2045 2023-06-02 21:20:41.461367 kiwi_cogs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 kiwi_cogs-0.1.2/PKG-INFO
```

### Comparing `kiwi_cogs-0.1.1/LICENSE` & `kiwi_cogs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.1/README.md` & `kiwi_cogs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kiwi_cogs-0.1.1/kiwi_cogs/event.py` & `kiwi_cogs-0.1.2/kiwi_cogs/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from .transition import Transition
 
 
 class Event(BaseModel):
     name: Optional[str] = None
     """Name of the event"""
-    guards: Optional[Dict[str, Callable]]
+    guards: Optional[Dict[str, Callable]] = None
     """Possible guards, which are callables"""
-    actions: Optional[Dict[str, Callable]]
+    actions: Optional[Dict[str, Callable]] = None
     """Action side effects for the machine"""
     transitions: List[Transition]
 
     @validator("transitions", pre=True)
     def build_transitions(cls, value: Union[Dict, List], values: Dict) -> List[Transition]:
         """Build a list of transitions from the given transition data
```

### Comparing `kiwi_cogs-0.1.1/kiwi_cogs/machine.py` & `kiwi_cogs-0.1.2/kiwi_cogs/machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         :returns: The final state after all possible transitions have been processed
         :rtype: State
         """
         if state is None:
             state = self.state
 
         transition = await self.state.get_transition(context=self.context)  # type: ignore[union-attr , arg-type]
-        if transition:
+        if transition and transition.target is not None:
             await self.do_transition(transition.target)
             return await self.step()  # step through the new state
 
         return state  # type: ignore[return-value]
 
     async def on_entry(self, context: dict) -> None:
         """Perform any entry actions for the new state
```

### Comparing `kiwi_cogs-0.1.1/kiwi_cogs/state.py` & `kiwi_cogs-0.1.2/kiwi_cogs/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,16 +259,17 @@
         :returns: The next transition to take, if a condition is met
         :rtype: Optional[Transition]
         """
 
         if self.state:  # noqa: SIM102
             # Go depth first to the last state
             if new_transition := await self.state.get_transition(context=context):
-                await self.on_exit(context=context)
-                await self.update_state(target=new_transition.target, context=context)  # type: ignore[arg-type]
+                if new_transition.target is not None:
+                    await self.on_exit(context=context)
+                    await self.update_state(target=new_transition.target, context=context)
 
         for transition in self.transitions:
             if asyncio.iscoroutinefunction(transition.cond):
                 condition = await transition.cond(context, None)
             else:
                 condition = transition.cond(context, None)
```

### Comparing `kiwi_cogs-0.1.1/kiwi_cogs/transition.py` & `kiwi_cogs-0.1.2/kiwi_cogs/transition.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     :type cond: Callable or str
     :param actions: A list of functions or strings that represent the actions to be executed during the transition.
                    If an item is a string, it is assumed to be the name of a function
                    that must be available in the current context.
     :type actions: List[Union[Callable, str]]
     """
 
-    target: Optional[str]
+    target: Optional[str] = None
     """The target state for this transition if the condition is met"""
     guards: Optional[Dict[str, Callable]]
     """Possible guards, which are callables"""
     actions_map: Optional[Dict[str, Callable]] = None
     """Action map"""
     actions: List[Callable] = []
     """Action side effects for the machine"""
```

### Comparing `kiwi_cogs-0.1.1/pyproject.toml` & `kiwi_cogs-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 [tool.poetry]
 name = "kiwi_cogs"
-version = "v0.1.1"
+version = "v0.1.2"
 description = "A simple and easy to use state machine library "
-authors = ["David Hall <fdev@davidhall.tech>"]
-repository = "https://github.com/mopeyjellyfish/kiwi-cogs"
-documentation = "https://mopeyjellyfish.github.io/kiwi-cogs/"
+authors = ["David Hall <dev@davidhall.tech>"]
+repository = "https://github.com/mopeyjellyfish/KiwiCogs/"
+documentation = "https://mopeyjellyfish.github.io/KiwiCogs/"
 readme = "README.md"
-packages = [
-  {include = "kiwi_cogs"}
-]
+packages = [{ include = "kiwi_cogs" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pydantic = "^1.10.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 deptry = "^0.6.4"
-mypy = "^0.981"
+mypy = ">=0.981,<1.4"
 pre-commit = "^2.20.0"
 tox = "^3.25.1"
 pytest-asyncio = "^0.21.0"
 greenlet = "^2.0.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^8.5.10"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocstrings = { extras = ["python"], version = "^0.19.0" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -68,15 +66,16 @@
     # flake8-simplify
     "SIM",
     # isort
     "I",
     # mccabe
     "C90",
     # pycodestyle
-    "E", "W",
+    "E",
+    "W",
     # pyflakes
     "F",
     # pygrep-hooks
     "PGH",
     # pyupgrade
     "UP",
     # ruff
@@ -99,14 +98,11 @@
 
 [tool.coverage.run]
 branch = true
 source = ["kiwi_cogs"]
 concurrency = ["greenlet"]
 
 [tool.pytest.ini_options]
-asyncio_mode="auto"
+asyncio_mode = "auto"
 
 [tool.deptry]
-    extend_exclude = [
-        ".*/tests/",
-        "conftest.py"
-    ]
+extend_exclude = [".*/tests/", "conftest.py"]
```

### Comparing `kiwi_cogs-0.1.1/PKG-INFO` & `kiwi_cogs-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kiwi-cogs
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple and easy to use state machine library 
-Home-page: https://github.com/mopeyjellyfish/kiwi-cogs
+Home-page: https://github.com/mopeyjellyfish/KiwiCogs/
 Author: David Hall
-Author-email: fdev@davidhall.tech
+Author-email: dev@davidhall.tech
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
-Project-URL: Documentation, https://mopeyjellyfish.github.io/kiwi-cogs/
-Project-URL: Repository, https://github.com/mopeyjellyfish/kiwi-cogs
+Project-URL: Documentation, https://mopeyjellyfish.github.io/KiwiCogs/
+Project-URL: Repository, https://github.com/mopeyjellyfish/KiwiCogs/
 Description-Content-Type: text/markdown
 
 # Kiwi Cogs
 
 <div align="center">
 
 [![Release](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)](https://img.shields.io/github/v/release/mopeyjellyfish/KiwiCogs)
```

