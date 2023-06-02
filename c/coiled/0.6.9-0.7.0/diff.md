# Comparing `tmp/coiled-0.6.9.tar.gz` & `tmp/coiled-0.7.0.tar.gz`

## Comparing `coiled-0.6.9.tar` & `coiled-0.7.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_version.py
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/analytics.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cluster.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/coiled.yaml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/compatibility.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/config.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/context.py
--rw-r--r--   0        0        0   102090 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/core.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/errors.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/exceptions.py
--rw-r--r--   0        0        0    19229 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/magic.py
--rw-r--r--   0        0        0    12287 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/scan.py
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/software.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/types.py
--rw-r--r--   0        0        0    51919 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/utils.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/websockets.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/__init__.py
--rw-r--r--   0        0        0    88669 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/cluster.py
--rw-r--r--   0        0        0    57690 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/core.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/cwi_log_link.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/states.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/__init__.py
--rw-r--r--   0        0        0    15458 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/rich.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/_beta/widgets/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/config.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/core.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/curl.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/diagnostics.py
--rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/env.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/login.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/package_sync.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/utils.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/__init__.py
--rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/better_logs.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/logs.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/ssh.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/cluster/utils.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/notebook/__init__.py
--rw-r--r--   0        0        0    12830 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/notebook/notebook.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/__init__.py
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/amp.py
--rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/aws.py
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/entry.py
--rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/gcp.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/prometheus.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/cli/setup/util.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.6.9/coiled/v2/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.6.9/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.6.9/LICENSE
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.6.9/README.md
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 coiled-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 coiled-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_version.py
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/analytics.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cluster.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/coiled.yaml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/compatibility.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/config.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/context.py
+-rw-r--r--   0        0        0   102142 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/core.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/errors.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/exceptions.py
+-rw-r--r--   0        0        0    19523 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/magic.py
+-rw-r--r--   0        0        0    13390 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/scan.py
+-rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/software.py
+-rw-r--r--   0        0        0     9156 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/types.py
+-rw-r--r--   0        0        0    51928 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/utils.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/websockets.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/__init__.py
+-rw-r--r--   0        0        0    89867 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/cluster.py
+-rw-r--r--   0        0        0    58518 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/core.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/cwi_log_link.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/states.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/widgets/__init__.py
+-rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/widgets/rich.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/_beta/widgets/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/config.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/core.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/curl.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/diagnostics.py
+-rw-r--r--   0        0        0     4824 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/env.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/login.py
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/package_sync.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/utils.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/cluster/__init__.py
+-rw-r--r--   0        0        0     9606 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/cluster/better_logs.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/cluster/logs.py
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/cluster/ssh.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/cluster/utils.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/notebook/__init__.py
+-rw-r--r--   0        0        0    13756 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/notebook/notebook.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/__init__.py
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/amp.py
+-rw-r--r--   0        0        0    43611 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/aws.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/entry.py
+-rw-r--r--   0        0        0    26723 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/gcp.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/prometheus.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/cli/setup/util.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coiled-0.7.0/coiled/v2/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 coiled-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 coiled-0.7.0/LICENSE
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 coiled-0.7.0/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 coiled-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 coiled-0.7.0/PKG-INFO
```

### Comparing `coiled-0.6.9/coiled/__init__.py` & `coiled-0.7.0/coiled/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/analytics.py` & `coiled-0.7.0/coiled/analytics.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cluster.py` & `coiled-0.7.0/coiled/cluster.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,8 +32,8 @@
         logger.info(f"Adaptive scaling up to {n} workers.")
         await self.cluster.scale_up(n, reason=f"Adaptive scaling up to {n} workers.")
 
     async def scale_down(self, workers):
         if not workers:
             return
         logger.info(f"Adaptive is removing {len(workers)} workers: {workers}.")
-        await self.cluster.scale_down(workers)
+        await self.cluster.scale_down(workers, reason=f"Adaptive removing {len(workers)} workers.")
```

### Comparing `coiled-0.6.9/coiled/coiled.yaml` & `coiled-0.7.0/coiled/coiled.yaml`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/context.py` & `coiled-0.7.0/coiled/context.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/core.py` & `coiled-0.7.0/coiled/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 import dask
 import dask.distributed
 import distributed
 import rich
 from distributed.comm import parse_address
 from distributed.utils import LoopRunner, sync
 from importlib_metadata import PackageNotFoundError, version
+from packaging.version import Version
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from tornado.ioloop import IOLoop
 from typing_extensions import Literal, ParamSpec, Protocol, TypeAlias
 
 from coiled.exceptions import (
@@ -1566,15 +1567,15 @@
         try:
             pip_version = version("pip")
         except PackageNotFoundError:
             pip_version = "None"
 
         return {
             "operating_system": platform.platform(),
-            "python": PY_VERSION,
+            "python": str(PY_VERSION),
             "pip": pip_version,
             "conda": conda_version,
             "coiled": COILED_VERSION,
             "dask": dask.__version__,
             "distributed": distributed.__version__,
         }
 
@@ -2445,15 +2446,15 @@
         Associated the account which user wishes to upload to. If not specified, current / default
         account will be utilized.
 
     """
     perf_url = PerformanceReportURL(None)
     # stacklevel= is newer kwarg after version check below
     try:
-        report_kwargs = {"stacklevel": 3} if DISTRIBUTED_VERSION >= "2021.05.0" else {}
+        report_kwargs = {"stacklevel": 3} if DISTRIBUTED_VERSION >= Version("2021.05.0") else {}
         with dask.distributed.performance_report(filename=filename, **report_kwargs):
             yield perf_url
     except Exception as ex:
         raise Exception("Exception in coiled.performance_report() context").with_traceback(ex.__traceback__)
     finally:
         # by this point dask will have written local file as <filename>
         results = _upload_report(filename, private=private, account=account)
```

### Comparing `coiled-0.6.9/coiled/exceptions.py` & `coiled-0.7.0/coiled/exceptions.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/magic.py` & `coiled-0.7.0/coiled/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from logging import getLogger
 from pathlib import Path
 from sys import executable
 from tempfile import TemporaryDirectory
 from threading import Lock
-from typing import Dict, List, Optional, Set, TextIO, Tuple, Union
+from typing import Dict, List, Literal, Optional, Set, TextIO, Tuple, Union, cast
 from urllib.parse import urlparse
 
 from dask import config
 from filelock import BaseFileLock, FileLock
 from packaging.utils import parse_wheel_filename
 from rich.progress import Progress
 
@@ -98,15 +98,15 @@
     package_lock, thread_lock, tmpdir = WHEEL_BUILD_LOCKS.setdefault(
         pkg_name,
         (FileLock(lock_path / ("." + pkg_name + version + ".build-lock")), Lock(), TemporaryDirectory()),
     )
     async with async_lock(package_lock, thread_lock):
         outdir = Path(tmpdir.name) / Path(pkg_name)
         if outdir.exists():
-            logger.info(f"Checking for existing wheel for {pkg_name} @ {outdir}")
+            logger.debug(f"Checking for existing wheel for {pkg_name} @ {outdir}")
             wheel_fn = next((file for file in outdir.iterdir() if file.suffix == ".whl"), None)
         else:
             wheel_fn = None
         if not wheel_fn:
             logger.info(f"No existing wheel, creating a wheel for {pkg_name} @ {src}")
             # must use executable to avoid using some other random python
             p = await create_subprocess_shell(
@@ -203,15 +203,15 @@
     }
 
 
 @track_context
 async def approximate_packages(
     cloud: CloudBeta,
     packages: List[PackageInfo],
-    priorities: Dict[str, PackageLevelEnum],
+    priorities: Dict[Tuple[str, Literal["conda", "pip"]], PackageLevelEnum],
     progress: Optional[Progress] = None,
     strict: bool = False,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> typing.List[ResolvedPackageInfo]:
     user_conda_installed_python = next((p for p in packages if p["name"] == "python"), None)
     user_conda_installed_pip = next(
         (i for i, p in enumerate(packages) if p["name"] == "pip" and p["source"] == "conda"),
@@ -263,17 +263,21 @@
         coiled_selected_python = await default_python()
         packages.append(coiled_selected_python)
     with simple_progress("Validating environment", progress=progress):
         results = await cloud._approximate_packages(
             packages=[
                 {
                     "name": pkg["name"],
-                    "priority_override": PackageLevelEnum.CRITICAL
-                    if (strict or pkg["wheel_target"])
-                    else priorities.get(pkg["conda_name"] or pkg["name"]),
+                    "priority_override": (
+                        PackageLevelEnum.CRITICAL
+                        if (strict or pkg["wheel_target"])
+                        else priorities.get(
+                            ((cast(str, pkg["conda_name"]) if pkg["source"] == "conda" else pkg["name"]), pkg["source"])
+                        )
+                    ),
                     "python_major_version": PYTHON_VERSION[0],
                     "python_minor_version": PYTHON_VERSION[1],
                     "python_patch_version": PYTHON_VERSION[2],
                     "source": pkg["source"],
                     "channel_url": pkg["channel_url"],
                     "channel": pkg["channel"],
                     "subdir": pkg["subdir"],
@@ -419,15 +423,15 @@
                 faulty_packages[groups["package"]].append(warning)
         return faulty_packages
 
 
 @track_context
 async def create_environment_approximation(
     cloud: CloudBeta,
-    priorities: Dict[str, PackageLevelEnum],
+    priorities: Dict[Tuple[str, Literal["conda", "pip"]], PackageLevelEnum],
     only: Optional[Set[str]] = None,
     strict: bool = False,
     progress: Optional[Progress] = None,
     architecture: ArchitectureTypesEnum = ArchitectureTypesEnum.X86_64,
 ) -> typing.List[ResolvedPackageInfo]:
     packages = await scan_prefix(progress=progress)
     bad_packages = await check_pip_happy(progress)
@@ -473,18 +477,18 @@
     from rich.table import Table
 
     async def run():
         async with CloudBeta(asynchronous=True) as cloud:
             return await create_environment_approximation(
                 cloud=cloud,
                 priorities={
-                    "dask": PackageLevelEnum.CRITICAL,
-                    "twisted": PackageLevelEnum.IGNORE,
-                    "graphviz": PackageLevelEnum.LOOSE,
-                    "icu": PackageLevelEnum.LOOSE,
+                    ("dask", "conda"): PackageLevelEnum.CRITICAL,
+                    ("twisted", "conda"): PackageLevelEnum.IGNORE,
+                    ("graphviz", "conda"): PackageLevelEnum.LOOSE,
+                    ("icu", "conda"): PackageLevelEnum.LOOSE,
                 },
             )
 
     result = asyncio.run(run())
 
     table = Table(title="Packages")
     keys = ("name", "source", "include", "client_version", "specifier", "error", "note")
```

### Comparing `coiled-0.6.9/coiled/scan.py` & `coiled-0.7.0/coiled/scan.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,30 +7,46 @@
 from collections import defaultdict
 from logging import getLogger
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 from urllib.parse import urlparse
 
 from importlib_metadata import Distribution
+from packaging.version import InvalidVersion
+from packaging.version import parse as parse_version
 from rich.progress import Progress
 from typing_extensions import Literal
 
 from coiled.types import CondaPackage, CondaPlaceHolder, PackageInfo
 from coiled.utils import parse_file_uri
 
 logger = getLogger("coiled.package_sync")
 subdir_datas = {}
 PYTHON_VERSION = platform.python_version_tuple()
 
 
-def consistent_name(name: str):
+def normalize_name(name: str):
     # gives the best shot at names being consistent between pypi/conda
     return name.lower().replace("-", "_")
 
 
+def normalize_version(version: str):
+    """Attempt to normalize version between conda and pip without tripping over conda not supporting PEP440"""
+    # Bail on non-PEP440 versions like 2023c, which will get parsed as 2023rc0
+    if not len(version.split(".")) > 2:
+        return version
+    else:
+        try:
+            # Normalize things like 23.04.00 to 23.4.0
+            return str(parse_version(version))
+        # Fallback to original version if its unparseable like 1.7.1dev.rapidsai23.04
+        except InvalidVersion:
+            return version
+
+
 async def scan_conda(prefix: Path, progress: Optional[Progress] = None) -> typing.Dict[str, List[PackageInfo]]:
     conda_meta = prefix / "conda-meta"
     if conda_meta.exists() and conda_meta.is_dir():
         conda_packages = [
             CondaPackage(json.load(metafile.open("r")), prefix=prefix)
             for metafile in conda_meta.iterdir()
             if metafile.suffix == ".json"
@@ -50,15 +66,15 @@
                 pkg for pkg in await asyncio.gather(*[handle_conda_package(pkg) for pkg in conda_packages]) if pkg
             ]
         # it's possible for multiple similar packages to be "installed"
         # eg importlib-metadata & importlib_metadata
         # we have to check later which one is actually being imported
         result: Dict[str, List[PackageInfo]] = defaultdict(list)
         for pkg in sorted(packages, key=lambda pkg: (pkg["name"], pkg["conda_name"]), reverse=True):
-            result[consistent_name(pkg["conda_name"] or pkg["name"])].append(pkg)
+            result[normalize_name(pkg["conda_name"] or pkg["name"])].append(pkg)
         return result
     else:
         return {}
 
 
 async def handle_conda_package(pkg: CondaPackage) -> Optional[PackageInfo]:
     # Are there conda packages that install multiple python packages?
@@ -238,15 +254,15 @@
             asyncio.as_completed([handle_dist(dist, locations) for dist in dists]),
             total=len(dists),
             description=f"Scanning {len(dists)} python packages",
         ):
             packages.append(await task)
     else:
         packages = await asyncio.gather(*(handle_dist(dist, locations) for dist in dists))
-    return {consistent_name(pkg["name"]): pkg for pkg in packages if pkg}
+    return {normalize_name(pkg["name"]): pkg for pkg in packages if pkg}
 
 
 async def scan_prefix(
     prefix: Optional[Path] = None, progress: Optional[Progress] = None, locations: Optional[List[Path]] = None
 ) -> typing.List[PackageInfo]:
     # TODO: private conda channels
     # TODO: detect pre-releases and only set --pre flag for those packages (for conda)
@@ -270,21 +286,36 @@
         # that claims to have this pypi name
         for possible_name in [name] + [p["name"] for p in packages]:
             if pip_env.get(possible_name):
                 found = True
                 pip_package = pip_env[possible_name]
                 if isinstance(pip_package, CondaPlaceHolder):
                     # find the conda package that actually matches with what is importable
-                    importable_package = next(p for p in packages if p["name"].lower() == pip_package["name"].lower())
+                    importable_package = next(
+                        p for p in packages if normalize_name(p["name"]) == normalize_name(pip_package["name"])
+                    )
                     filtered_conda[name] = importable_package
                     break
-                elif next((p for p in packages if p["version"] == pip_package["version"]), None):
+                elif next(
+                    (
+                        p
+                        for p in packages
+                        if normalize_version(p["version"]) == normalize_version(pip_package["version"])
+                    ),
+                    None,
+                ):
                     # if the versions match, we can fall back to using the conda version
                     pip_env.pop(possible_name, None)
-                    filtered_conda[name] = next((p for p in packages if p["version"] == pip_package["version"]))
+                    filtered_conda[name] = next(
+                        (
+                            p
+                            for p in packages
+                            if normalize_version(p["version"]) == normalize_version(pip_package["version"])
+                        )
+                    )
                     break
         if not found:
             # a non python package and safe to include
             filtered_conda[name] = packages[0]
     # remove conda placeholders
     pip_env = {pkg_name: pkg for pkg_name, pkg in pip_env.items() if not isinstance(pkg, CondaPlaceHolder)}
     return sorted(
```

### Comparing `coiled-0.6.9/coiled/software.py` & `coiled-0.7.0/coiled/software.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/types.py` & `coiled-0.7.0/coiled/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,22 +83,21 @@
 class PackageLevelEnum(int, Enum):
     """
     Package mismatch severity level
     Using a high int so we have room to add extra levels as needed
 
     Ordering is allow comparison like
 
-    if somelevel >= PackageLevelEnum.HIGH:
+    if somelevel >= PackageLevelEnum.STRICT_MATCH:
         <some logic for high or critical levels>
     """
 
     CRITICAL = 100
-    HIGH = 75
-    MEDIUM = 50
-    LOW = 25
+    STRICT_MATCH = 75
+    WARN = 50
     NONE = 0
     LOOSE = -1
     IGNORE = -2
 
 
 class ApproximatePackageRequest(TypedDict):
     name: str
@@ -158,14 +157,15 @@
             self.channel_url = result.group(1) + "/" + result.group(2)
             self.channel: str = result.group(2)
 
 
 class PackageLevel(TypedDict):
     name: str
     level: PackageLevelEnum
+    source: Literal["pip", "conda"]
 
 
 class ApiBase(TypedDict):
     id: int
     created: str
     updated: str
```

### Comparing `coiled-0.6.9/coiled/utils.py` & `coiled-0.7.0/coiled/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -601,15 +601,15 @@
     and run the command in subprocess instead.
 
     For reference on the RuntimeError exception: https://bugs.python.org/issue35621
 
     """
     platform = get_platform()
 
-    if PY_VERSION < "3.8" or platform == "windows":
+    if PY_VERSION < Version("3.8") or platform == "windows":
         proc = subprocess.Popen(
             cmd.split(" "),
             bufsize=1,
             universal_newlines=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
```

### Comparing `coiled-0.6.9/coiled/websockets.py` & `coiled-0.7.0/coiled/websockets.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/_beta/__init__.py` & `coiled-0.7.0/coiled/_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/_beta/cluster.py` & `coiled-0.7.0/coiled/_beta/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import botocore
 import dask
 import dask.distributed
 import distributed
 from dateutil import tz
 from distributed.core import Status
 from distributed.deploy.adaptive import Adaptive
+from packaging.version import Version
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import BarColumn, Progress, TextColumn, TimeElapsedColumn
 from typing_extensions import Literal, TypeAlias
 from urllib3.util import parse_url
 
 from coiled import magic
@@ -92,15 +93,15 @@
 
 def use_rich_widget():
     return EXECUTION_CONTEXT in ["ipython_terminal", "notebook"] and HAS_RICH
 
 
 BEHAVIOR_TO_LEVEL = {
     "critical-only": PackageLevelEnum.CRITICAL,
-    "warning-or-higher": PackageLevelEnum.MEDIUM,
+    "warning-or-higher": PackageLevelEnum.WARN,
     "any": PackageLevelEnum.NONE,
 }
 ClusterSyncAsync: TypeAlias = Union["Cluster[Async]", "Cluster[Sync]"]
 
 _vm_type_cpu_memory_error_msg = (
     "Argument '{kind}_vm_types' can't be used together with '{kind}_cpu' or '{kind}_memory'. "
     "Please use either '{kind}_vm_types' or '{kind}_cpu'/'{kind}_memory' separately."
@@ -320,15 +321,15 @@
         credentials_duration_seconds: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
         environ: Optional[Dict[str, str]] = None,
         tags: Optional[Dict[str, str]] = None,
         send_dask_config: bool = True,
         backend_options: Optional[Union[AWSOptions, GCPOptions]] = None,  # intentionally not in the docstring yet
         show_widget: bool = True,
-        configure_logging: bool = False,
+        configure_logging: Optional[bool] = None,
         wait_for_workers: Optional[Union[int, float, bool]] = None,
         package_sync: Union[bool, List[str]] = False,
         package_sync_strict: bool = False,
         package_sync_ignore: Optional[List[str]] = None,
         package_sync_fail_on: Literal["critical-only", "warning-or-higher", "any"] = "critical-only",
         private_to_creator: Optional[bool] = None,
         use_best_zone: bool = True,
@@ -386,14 +387,19 @@
                     " in the backend_options dict. Only one of those should be specified."
                 )
             backend_options["region_name"] = region
 
         if configure_logging:
             setup_logging()
 
+        if configure_logging is None:
+            # setup logging only if we're not using the widget
+            if not use_rich_widget():
+                setup_logging()
+
         # Determine consistent sync/async
         if cloud and asynchronous is not None and cloud.asynchronous != asynchronous:
             warnings.warn(
                 f"Requested a Cluster with asynchronous={asynchronous}, but "
                 f"cloud.asynchronous={cloud.asynchronous}, so the cluster will be"
                 f"{cloud.asynchronous}"
             )
@@ -412,15 +418,15 @@
         #     self.cleanup_cloud = True
         #     self.cloud: CloudBeta[IsAsynchronous] = CloudBeta(asynchronous=asynchronous)
 
         # As of distributed 2021.12.0, deploy.Cluster has a ``loop`` attribute on the
         # base class. We add the attribute manually here for backwards compatibility.
         # TODO: if/when we set the minimum distributed version to be >= 2021.12.0,
         # remove this check.
-        if DISTRIBUTED_VERSION >= "2021.12.0":
+        if DISTRIBUTED_VERSION >= Version("2021.12.0"):
             kwargs = {"loop": self.cloud.loop}
         else:
             kwargs = {}
             self.loop = self.cloud.loop
 
         # we really need to call this first before any of the below code errors
         # out; otherwise because of the fact that this object inherits from
@@ -777,18 +783,21 @@
 
             else:
                 live = contextlib.nullcontext()
             with live:
                 with simple_progress("Fetching latest package priorities", progress):
                     logger.info("Resolving your local Python environment...")
                     package_levels = await self.cloud._fetch_package_levels()
-                package_level_lookup = {pkg["name"]: PackageLevelEnum(pkg["level"]) for pkg in package_levels}
+                package_level_lookup = {
+                    (pkg["name"], pkg["source"]): PackageLevelEnum(pkg["level"]) for pkg in package_levels
+                }
                 if self.package_sync_ignore:
                     for package in self.package_sync_ignore:
-                        package_level_lookup[package] = PackageLevelEnum.IGNORE
+                        package_level_lookup[(package, "conda")] = PackageLevelEnum.IGNORE
+                        package_level_lookup[(package, "pip")] = PackageLevelEnum.IGNORE
                 approximation = await magic.create_environment_approximation(
                     cloud=self.cloud,
                     only=self.package_sync_only,
                     priorities=package_level_lookup,
                     strict=self.package_sync_strict,
                     progress=progress,
                     architecture=architecture,
@@ -796,49 +805,67 @@
 
                 if not self.package_sync_only:
                     # if we're not operating on a subset, check
                     # all the coiled defined critical packages are present
                     packages_by_name: Dict[str, magic.ResolvedPackageInfo] = {p["name"]: p for p in approximation}
                     self._check_halting_issues(package_levels, packages_by_name)
                 packages_with_errors = [
-                    (pkg, package_level_lookup.get(pkg["name"], PackageLevelEnum.MEDIUM))
+                    (
+                        pkg,
+                        package_level_lookup.get(
+                            (
+                                (cast(str, pkg["conda_name"]) if pkg["source"] == "conda" else pkg["name"]),
+                                pkg["source"],
+                            ),
+                            PackageLevelEnum.WARN,
+                        ),
+                    )
                     for pkg in approximation
                     if pkg["error"]
                 ]
                 for pkg_with_error, level in packages_with_errors:
-                    if level >= PackageLevelEnum.MEDIUM:
+                    if level >= PackageLevelEnum.WARN:
                         logfunc = logger.warn
                     else:
                         logfunc = logger.info
                     logfunc(f"Package - {pkg_with_error['name']}, {pkg_with_error['error']}")
                 packages_with_notes = [
                     pkg
                     for pkg in approximation
                     if (
                         pkg["note"]
-                        and package_level_lookup.get(pkg["name"], PackageLevelEnum.MEDIUM) > PackageLevelEnum.IGNORE
+                        and (
+                            package_level_lookup.get(
+                                (
+                                    (cast(str, pkg["conda_name"]) if pkg["source"] == "conda" else pkg["name"]),
+                                    pkg["source"],
+                                ),
+                                PackageLevelEnum.WARN,
+                            )
+                            > PackageLevelEnum.IGNORE
+                        )
                     )
                 ]
                 for pkg_with_note in packages_with_notes:
                     logger.info(f"Package - {pkg_with_note['name']}, {pkg_with_note['note']}")
 
                 package_sync_env_alias = await self.cloud._create_package_sync_env(
                     packages=approximation,
                     account=self.account,
                     progress=progress,
                     gpu_enabled=gpu_enabled,
                     architecture=architecture,
                 )
                 package_sync_env = package_sync_env_alias["id"]
-            if HAS_RICH and self.show_widget:
+            if use_rich_widget() and self.show_widget:
                 from .widgets.rich import print_rich_package_table
 
                 print_rich_package_table(packages_with_notes, packages_with_errors)
 
-            logger.info(f"Environment magic complete ,{package_sync_env}")
+            logger.debug(f"Environment magic complete, {package_sync_env}")
         else:
             package_sync_env = None
 
         return package_sync_env
 
     @track_context
     def _check_halting_issues(
@@ -1039,14 +1066,15 @@
                     )
                 # TODO (future PR) still use strict mode for GPU cluster if local env also has GPU
                 if (
                     platform.machine() == architecture
                     and platform.system() == "Linux"
                     and not is_system_python()
                     and not self._is_gpu_cluster
+                    and not self.package_sync_ignore
                 ):
                     self.package_sync_strict = True
 
                 # create an ad hoc software environment if container was specified
                 if self.software_container:
                     # make a valid software env name unique for this container
                     image_and_tag = self.software_container.split("/")[-1]
@@ -1067,14 +1095,15 @@
                     parse_identifier(
                         self.software_environment,
                         property_name="software_environment",
                         can_have_revision=False,
                     )
 
                 senv_v2_id = await self._determine_senv(architecture=architecture, gpu_enabled=self._is_gpu_cluster)
+
                 self.cluster_id, cluster_existed = await cloud._create_cluster(
                     account=self.account,
                     name=self.name,
                     workers=self._start_n_workers,
                     software_environment=self.software_environment,
                     worker_class=self.worker_class,
                     worker_options=self.worker_options,
@@ -1177,15 +1206,15 @@
             # just a measure of how long this object has been around
             "cluster_object_life": str(datetime.datetime.now() - self.init_time),
         }
 
     def _maybe_log_summary(self, cluster_details):
         now = time.time()
         if self._last_logged_state_summary is None or now > self._last_logged_state_summary + 5:
-            logger.info(summarize_status(cluster_details))
+            logger.debug(summarize_status(cluster_details))
             self._last_logged_state_summary = now
 
     @track_context
     async def _wait_until_ready(self, is_new_cluster: bool) -> None:
         cloud = self.cloud
         cluster_id = self._assert_cluster_id()
         timeout_at = (
@@ -1296,15 +1325,15 @@
                     assert final_update is not None
                     if widget:
                         widget.update(
                             cluster_details,
                             self._cluster_status_logs,
                             final_update=final_update,
                         )
-                    logger.info(summarize_status(cluster_details))
+                    logger.debug(summarize_status(cluster_details))
                     return
                 else:
                     reason_not_ready = scheduler_reason_not_ready if not scheduler_ready else workers_reason_not_ready
                     if cluster_state in (
                         ClusterStateEnum.error,
                         ClusterStateEnum.stopped,
                     ):
@@ -1312,42 +1341,42 @@
                         error = f"Cluster status is {cluster_state.value} (reason: {reason})"
                         if widget:
                             widget.update(
                                 cluster_details,
                                 self._cluster_status_logs,
                                 final_update=error,
                             )
-                        logger.info(summarize_status(cluster_details))
+                        logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             error,
                             cluster_id=self.cluster_id,
                         )
                     elif cluster_state == ClusterStateEnum.ready:
                         # (cluster state "ready" means all worked either started or errored, so
                         # this cluster will ever have all the workers we want)
                         if widget:
                             widget.update(
                                 cluster_details,
                                 self._cluster_status_logs,
                                 final_update=reason_not_ready,
                             )
-                        logger.info(summarize_status(cluster_details))
+                        logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             reason_not_ready,
                             cluster_id=self.cluster_id,
                         )
                     elif timeout_at is not None and datetime.datetime.now() > timeout_at:
                         error = "User-specified timeout expired: " + reason_not_ready
                         if widget:
                             widget.update(
                                 cluster_details,
                                 self._cluster_status_logs,
                                 final_update=error,
                             )
-                        logger.info(summarize_status(cluster_details))
+                        logger.debug(summarize_status(cluster_details))
                         raise ClusterCreationError(
                             error,
                             cluster_id=self.cluster_id,
                         )
                     else:
                         await asyncio.sleep(1.0)
 
@@ -1767,15 +1796,15 @@
         ----------
         n
             Number of workers to scale cluster size to.
         """
         return self.sync(self._scale, n=n)
 
     @track_context
-    async def scale_down(self, workers: set) -> None:
+    async def scale_down(self, workers: set, reason: Optional[str] = None) -> None:
         if not self.cluster_id:
             raise ValueError("No cluster available to scale!")
         cloud = cast(CloudBeta[Async], self.cloud)
         try:
             scheduler_comm = self._ensure_scheduler_comm()
             await scheduler_comm.retire_workers(
                 names=workers,
@@ -1785,14 +1814,15 @@
         except Exception as e:
             logging.warning(f"error retiring workers {e}. Trying more forcefully")
         # close workers more forcefully
         await cloud._scale_down(
             account=self.account,
             cluster_id=self.cluster_id,
             workers=workers,
+            reason=reason,
         )
         self._plan.difference_update(workers)
         self._requested.difference_update(workers)
 
     async def recommendations(self, target: int) -> dict:
         """
         Make scale up/down recommendations based on current state and target
```

### Comparing `coiled-0.6.9/coiled/_beta/core.py` & `coiled-0.7.0/coiled/_beta/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,18 +65,29 @@
     log_states,
 )
 
 logger = logging.getLogger(COILED_LOGGER_NAME)
 
 
 def setup_logging(level=logging.INFO):
-    # only set up logging if there's no log level specified yet on the coiled logger
-    if logging.getLogger(COILED_LOGGER_NAME).level == 0:
-        logging.getLogger(COILED_LOGGER_NAME).setLevel(level)
-        logging.basicConfig(format="[%(asctime)s][%(levelname)-8s][%(name)s] %(message)s")
+    # We want to be able to give info-level messages to users.
+    # For users who haven't set up a log handler, this requires creating one (b/c the handler of "last resort,
+    # logging.lastResort, has a level of "warning".
+    #
+    # Conservatively, we only do anything here if the user hasn't set up any log handlers on the root logger
+    # or the Coiled logger. If they have any handler, we assume logging is configured how they want it.
+    coiled_logger = logging.getLogger(COILED_LOGGER_NAME)
+    root_logger = logging.getLogger()
+    if coiled_logger.handlers == [] and root_logger.handlers == []:
+        stream_handler = logging.StreamHandler()
+        stream_handler.setFormatter(logging.Formatter(fmt="[%(asctime)s][%(levelname)-8s][%(name)s] %(message)s"))
+        # Conservatively, only change the Coiled logger level there's no log level specified yet.
+        if coiled_logger.level == 0:
+            coiled_logger.setLevel(level)
+            coiled_logger.addHandler(stream_handler)
 
 
 async def handle_api_exception(response, exception_cls=ServerError) -> NoReturn:
     try:
         error_body = await response.json()
     except ContentTypeError:
         raise exception_cls(
@@ -565,15 +576,15 @@
         if data["should_upload"]:
             await self._put_package(
                 url=data["upload_url"],
                 package_data=package_data,
                 file_md5=wheel_md5,
             )
         else:
-            logger.info(f"{package_name} MD5 matches existing, skipping upload")
+            logger.debug(f"{package_name} MD5 matches existing, skipping upload")
         return data["id"]
 
     @backoff.on_exception(
         backoff.expo,
         ClientResponseError,
         max_time=120,
         giveup=lambda error: cast(ClientResponseError, error).status < 500,
@@ -1368,21 +1379,25 @@
             await handle_api_exception(response)
 
         workers_info = await response.json()
 
         return {"workers": {w["name"] for w in workers_info}}
 
     @track_context
-    async def _scale_down(self, cluster_id: int, workers: Set[str], account: Optional[str] = None) -> None:
+    async def _scale_down(
+        self, cluster_id: int, workers: Set[str], account: Optional[str] = None, reason: Optional[str] = None
+    ) -> None:
         pass
         account = account or self.default_account
+
+        reason_dict = {"reason": reason} if reason else {}
         response = await self._do_request(
             "DELETE",
             f"{self.server}/api/v2/workers/account/{account}/cluster/{cluster_id}/",
-            params={"name": workers},
+            params={"name": workers, **reason_dict},
         )
         if response.status >= 400:
             await handle_api_exception(response)
 
     @overload
     def security(
         self: Cloud[Sync], cluster_id: int, account: Optional[str] = None
```

### Comparing `coiled-0.6.9/coiled/_beta/cwi_log_link.py` & `coiled-0.7.0/coiled/_beta/cwi_log_link.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/_beta/states.py` & `coiled-0.7.0/coiled/_beta/states.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/_beta/widgets/__init__.py` & `coiled-0.7.0/coiled/_beta/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/_beta/widgets/rich.py` & `coiled-0.7.0/coiled/_beta/widgets/rich.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,28 +28,31 @@
 from .util import get_instance_types, get_worker_statuses
 
 LOCAL_TIMEZONE = datetime.datetime.now(datetime.timezone.utc).astimezone().tzinfo
 
 # This is annoying. I think Ian explained to me that the reason
 # we need to manage the size so manually is that if we aren't explicit,
 # Jupyter notebooks (but not IPython terminal) messes up the size.
-WAITING_CONSOLE_HEIGHT = 26
+BASE_CONSOLE_HEIGHT = 17
 WAITING_PROGRESS_HEIGHT = 9
+WAITING_CONSOLE_HEIGHT = BASE_CONSOLE_HEIGHT + WAITING_PROGRESS_HEIGHT
 DONE_PROGRESS_HEIGHT = 6
-DONE_CONSOLE_HEIGHT = WAITING_CONSOLE_HEIGHT - (WAITING_PROGRESS_HEIGHT - DONE_PROGRESS_HEIGHT)
+DONE_CONSOLE_HEIGHT = BASE_CONSOLE_HEIGHT + DONE_PROGRESS_HEIGHT
 CONSOLE_WIDTH = 100
 
 
-def level_to_str(level: PackageLevelEnum):
+def level_to_str(level: PackageLevelEnum) -> Optional[str]:
     if level >= PackageLevelEnum.CRITICAL:
         return "Critical"
-    elif level >= PackageLevelEnum.MEDIUM:
+    elif level >= PackageLevelEnum.WARN:
         return "Warning"
     elif level >= PackageLevelEnum.NONE:
         return "Low"
+    else:
+        return None
 
 
 def print_rich_package_table(
     packages_with_notes: List[ResolvedPackageInfo],
     packages_with_errors: List[Tuple[ResolvedPackageInfo, PackageLevelEnum]],
 ):
     console = rich.console.Console(width=CONSOLE_WIDTH)
@@ -57,21 +60,23 @@
     if packages_with_notes:
         note_table = rich.table.Table(expand=True, box=rich.box.MINIMAL)
         note_table.add_column("Package")
         note_table.add_column("Note", overflow="fold")
         for pkg in packages_with_notes:
             note_table.add_row(pkg["name"], pkg["note"])
         console.print(rich.panel.Panel(note_table, title="[bold green]Package Info[/bold green]"))
-    if packages_with_errors:
+    if packages_with_errors and any(level_to_str(level) for _, level in packages_with_errors):
         error_table = rich.table.Table(expand=True, box=rich.box.MINIMAL)
         error_table.add_column("Package")
         error_table.add_column("Error")
         error_table.add_column("Risk")
         for pkg_info, level in sorted(packages_with_errors, key=lambda p: (p[1], p[0]["name"]), reverse=True):
-            error_table.add_row(pkg_info["name"], pkg_info["error"], level_to_str(level))
+            level_str = level_to_str(level)
+            if level_str is not None:
+                error_table.add_row(pkg_info["name"], pkg_info["error"], level_str)
         console.print(rich.panel.Panel(error_table, title="[bold red]Not Synced with Cluster[/bold red]"))
 
 
 class RichClusterWidget:
     """A Rich renderable showing cluster status."""
 
     n_workers: int
@@ -95,15 +100,15 @@
         self._loader_frames = ["...", " ..", "  .", "   ", ".  ", ".. "]
         self._frame = 0
         self.last_updated_utc = datetime.datetime.now(datetime.timezone.utc)
         if console:
             self.console = console
         else:
             self.console = rich.console.Console()
-            self.console.size = (CONSOLE_WIDTH, WAITING_CONSOLE_HEIGHT)
+            self.console.size = (CONSOLE_WIDTH, BASE_CONSOLE_HEIGHT)
 
         self._progress = progress = rich.progress.Progress(
             "{task.description}",
             rich.progress.BarColumn(complete_style="progress.remaining"),
             rich.progress.TextColumn("[progress.percentage]{task.completed}"),
         )
         self._error_progress = error_progress = rich.progress.Progress(
@@ -300,33 +305,44 @@
             dashboard_address = None
             scheduler_instance_type = current_loader_frame
             worker_instance_types = Counter()
             region = current_loader_frame
             zone_desc = ""
             cluster_name = ""
             desired_workers = ""
+            n_workers = []
+
+        show_worker_states = bool(desired_workers or n_workers)
 
         dashboard_label = (
             f"[link={dashboard_address}]{dashboard_address}[/link]" if dashboard_address else current_loader_frame
         )
         if any(k for k, v in worker_instance_types.items()):
             worker_instance_types_label = ", ".join(
                 f"{k or 'Unknown'} ({v:,})" for k, v in worker_instance_types.items()
             )
         else:
             worker_instance_types_label = current_loader_frame
+
+        worker_line = (
+            f"""
+            [bold green]Worker Instance Type(s):[/bold green] {worker_instance_types_label or current_loader_frame}
+            """
+            if show_worker_states
+            else ""
+        )
+
         config = dedent(
             f"""
             [bold green]Region:[/bold green] {region}{zone_desc}
 
             [bold green]Scheduler Instance Type:[/bold green] {scheduler_instance_type or current_loader_frame}
-
-            [bold green]Worker Instance Type(s):[/bold green] {worker_instance_types_label or current_loader_frame}
-
-            [bold green]Workers Requested:[/bold green] {desired_workers}"""
+            {worker_line}
+            [bold green]Workers Requested:[/bold green] {desired_workers}
+            """
         )
 
         status = dedent(
             f"""
             [bold green]Cluster Name:[/bold green] {cluster_name}
 
             [bold green]Scheduler Status:[/bold green] {scheduler_status}
@@ -334,64 +350,73 @@
             [bold green]Dashboard Address:[/bold green] {dashboard_label}"""
         )
 
         """Define the layout."""
         layout = rich.layout.Layout(name="root")
         self._frame = (self._frame + 1) % len(self._loader_frames)
 
-        if self._final_update is None:
-            progress_height = WAITING_PROGRESS_HEIGHT
-            console_size = (CONSOLE_WIDTH, WAITING_CONSOLE_HEIGHT)
+        if show_worker_states:
+            if self._final_update is None:
+                progress_height = WAITING_PROGRESS_HEIGHT
+                console_size = (CONSOLE_WIDTH, WAITING_CONSOLE_HEIGHT)
+            else:
+                progress_height = DONE_PROGRESS_HEIGHT
+                console_size = (CONSOLE_WIDTH, DONE_CONSOLE_HEIGHT)
         else:
-            progress_height = DONE_PROGRESS_HEIGHT
-            console_size = (CONSOLE_WIDTH, DONE_CONSOLE_HEIGHT)
+            progress_height = 0
+            console_size = (CONSOLE_WIDTH, BASE_CONSOLE_HEIGHT)
 
         self.console.size = console_size
 
         if self._cluster_details is None:
             link = ""
         else:
             link = get_details_url(self.server, self.account, self._cluster_details["id"])
             assert link is not None  # typechecker, go away please
 
         linked_details_link = (
             f"[link={link}]{link}[/link]" if EXECUTION_CONTEXT == "notebook" else f"[link]{link}[/link]"
         )
 
-        layout.split(
+        layout_panels = [
             rich.layout.Layout(
                 rich.panel.Panel(
                     rich.align.Align.center(linked_details_link),
                     title="[bold green frame]Coiled Cluster",
                 ),
                 name="header",
                 size=3,
             ),
             rich.layout.Layout(name="body", size=11),
-            rich.layout.Layout(name="progress", size=progress_height),
-        )
+        ]
+
+        if show_worker_states:
+            layout_panels.append(rich.layout.Layout(name="progress", size=progress_height))
+
+        layout.split(*layout_panels)
         layout["body"].split_row(
             rich.layout.Layout(name="overview"),
             rich.layout.Layout(name="configuration"),
         )
 
         time = self.last_updated_utc.astimezone(LOCAL_TIMEZONE).strftime("%Y/%m/%d %H:%M:%S %Z")
-        if self._final_update is None:
-            layout["progress"].update(
-                rich.panel.Panel(
-                    rich.align.Align.center(
-                        rich.console.Group(progress.get_renderable(), error_progress.get_renderable()),
-                        vertical="middle",
-                    ),
-                    title=f"Dask Worker States ({time})",
+        if show_worker_states:
+            if self._final_update is None:
+                layout["progress"].update(
+                    rich.panel.Panel(
+                        rich.align.Align.center(
+                            rich.console.Group(progress.get_renderable(), error_progress.get_renderable()),
+                            vertical="middle",
+                        ),
+                        title=f"Dask Worker States ({time})",
+                    )
                 )
-            )
-        else:
-            layout["progress"].update(
-                rich.panel.Panel(
-                    rich.align.Align.center(self._final_update, vertical="middle"),
-                    title=f"({time})",
+            else:
+                layout["progress"].update(
+                    rich.panel.Panel(
+                        rich.align.Align.center(self._final_update, vertical="middle"),
+                        title=f"({time})",
+                    )
                 )
-            )
         layout["body"]["overview"].update(rich.panel.Panel(status, title="Overview"))
         layout["body"]["configuration"].update(rich.panel.Panel(config, title="Configuration"))
         return layout
```

### Comparing `coiled-0.6.9/coiled/_beta/widgets/util.py` & `coiled-0.7.0/coiled/_beta/widgets/util.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/config.py` & `coiled-0.7.0/coiled/cli/config.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/core.py` & `coiled-0.7.0/coiled/cli/core.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/curl.py` & `coiled-0.7.0/coiled/cli/curl.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/env.py` & `coiled-0.7.0/coiled/cli/env.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/login.py` & `coiled-0.7.0/coiled/cli/login.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/package_sync.py` & `coiled-0.7.0/coiled/cli/package_sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,27 +24,29 @@
 def scan(csv: bool):
     result = asyncio.run(scan_prefix(Path(sys.prefix)))
     table = Table(title="Packages")
     table.add_column("Package Name", style="cyan", no_wrap=True)
     table.add_column("Conda Name", style="cyan", no_wrap=True)
     table.add_column("Version", style="magenta")
     table.add_column("Source", style="magenta")
+    table.add_column("Channel", style="magenta", overflow="fold")
     table.add_column("Wheel target", style="green", overflow="fold")
     table.add_column("Path", overflow="fold")
     table.add_column("Can build wheel", style="green")
     rows = []
     for pkg in result:
         rows.append(
             [
                 pkg["name"],
                 pkg["conda_name"],
                 pkg["version"],
                 pkg["source"],
-                str(pkg["wheel_target"] or ""),
-                str(pkg["path"]),
+                pkg["channel"] or "",
+                pkg["wheel_target"] or "",
+                str(pkg["path"]) if pkg["path"] else "",
                 True,
             ]
         )
 
     for _, name, ispkg in pkgutil.iter_modules(path=["."]):
         will_sync = False
         if ispkg:
@@ -53,22 +55,23 @@
                     if (pkg["path"] / name).resolve() == (Path(".") / name).resolve():  # type: ignore
                         will_sync = True
         if not will_sync:
             rows.append(
                 [
                     name,
                     "",
+                    "",
                     "cwd",
                     "",
                     "",
                     str(Path(".") / name) if ispkg else str((Path(".") / name).with_suffix(".py")),
                     False,
                 ]
             )
-    rows = sorted(rows, key=lambda x: (x[5], x[0].lower()))
+    rows = sorted(rows, key=lambda x: (x[3], x[0].lower()))
 
     if csv:
         writer = csv_writer(sys.stdout, lineterminator="\n")
         writer.writerow([c.header for c in table.columns])
         writer.writerows(rows)
     else:
         for row in rows:
```

### Comparing `coiled-0.6.9/coiled/cli/utils.py` & `coiled-0.7.0/coiled/cli/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/cluster/__init__.py` & `coiled-0.7.0/coiled/cli/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/cluster/better_logs.py` & `coiled-0.7.0/coiled/cli/cluster/better_logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/cluster/logs.py` & `coiled-0.7.0/coiled/cli/cluster/logs.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/cluster/ssh.py` & `coiled-0.7.0/coiled/cli/cluster/ssh.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 import coiled
 
 from ..utils import CONTEXT_SETTINGS
 from .utils import find_cluster
 
 
-def open_ssh(address: str, key: str, jump_to_address: Optional[str] = None):
+def open_ssh(address: str, key: str, jump_to_address: Optional[str] = None, host_command: Optional[str] = None):
     """Open an SSH session, relies on `ssh` and `ssh-add` (agent)."""
     if not add_key_to_agent(address, key, t=5):
         return
 
-    ssh_shell(address, jump_to_address)
+    ssh_shell(address, jump_to_address, host_command)
 
 
 def check_ssh() -> bool:
     if not shutil.which("ssh"):
         print("Unable to find `ssh`, you may need to install OpenSSH or add it to your paths.")
         return False
 
@@ -61,26 +61,29 @@
             print("An error occurred calling `ssh-add`. You may need to enable the ssh agent.")
             print(p.stderr)
             return False
 
     return True
 
 
-def ssh_shell(address: str, jump_to_address: Optional[str] = None):
+def ssh_shell(address: str, jump_to_address: Optional[str] = None, host_command: Optional[str] = None):
     if jump_to_address:
         ssh_target = f"-J ubuntu@{address} ubuntu@{jump_to_address}"
         ssh_target_label = f"worker at {jump_to_address}"
     else:
         ssh_target = f"ubuntu@{address}"
         ssh_target_label = f"scheduler at {address}"
 
-    ssh_command = f"ssh {ssh_target} -o StrictHostKeyChecking=no -o ForwardAgent=yes"
+    ssh_command = f"ssh -t {ssh_target} -o StrictHostKeyChecking=no -o ForwardAgent=yes"
+    ssh_command = f"{ssh_command} {host_command}" if host_command else ssh_command
 
     # print(ssh_command)
     print(f"===Starting SSH session to {ssh_target_label}===")
+    if host_command:
+        print(f"> {host_command}")
     subprocess.run(ssh_command, shell=True)
     print("===SSH session closed===")
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.argument("cluster", default="", required=False)
 @click.option(
@@ -102,15 +105,18 @@
 )
 @click.option(
     "--delete-key",
     default=False,
     is_flag=True,
     help="Just delete ssh key from local OpenSSH agent",
 )
-def ssh(cluster: str, private: bool, worker: Optional[str], add_key: bool, delete_key: bool):
+@click.option(
+    "--dask", default=False, is_flag=True, help="Attach to shell in Dask container rather than shell on host machine."
+)
+def ssh(cluster: str, private: bool, worker: Optional[str], add_key: bool, delete_key: bool, dask: bool):
     with coiled.Cloud() as cloud:
         cluster_info = find_cluster(cloud, cluster)
         cluster_id = cluster_info["id"]
         ssh_info = cloud.get_ssh_key(cluster_id=cluster_id, worker=worker)
 
     scheduler_address = ssh_info["scheduler_private_address"] if private else ssh_info["scheduler_public_address"]
 
@@ -135,12 +141,18 @@
             print("Unable to retrieve scheduler address")
             return
 
         if not ssh_info["private_key"]:
             print("Unable to retrieve SSH key")
             return
 
+        # Default container name is parent dir (tmp) + service name (dask) + instance number (1).
+        # If we need to make this more flexible in the future, name could be returned by cloud.get_ssh_key;
+        # for now we don't need that flexibility and it's okay if SSH CLI requires client update someday.
+        command = "docker exec -it tmp-dask-1 bash" if dask else None
+
         open_ssh(
             address=scheduler_address,
             key=ssh_info["private_key"],
             jump_to_address=ssh_info["worker_address"],
+            host_command=command,
         )
```

### Comparing `coiled-0.6.9/coiled/cli/cluster/utils.py` & `coiled-0.7.0/coiled/cli/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/notebook/__init__.py` & `coiled-0.7.0/coiled/cli/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/notebook/notebook.py` & `coiled-0.7.0/coiled/cli/notebook/notebook.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from __future__ import annotations
 
-import base64
-import hashlib
 import os
-import re
 import shutil
+import signal
 import subprocess
+import threading
+import uuid
 import webbrowser
 from typing import Optional, Sequence
 
 import click
 import importlib_metadata
+from packaging.version import Version
 from rich import print
+from rich.progress import Progress, SpinnerColumn
+from rich.prompt import Confirm
 from urllib3.util import parse_url
 
 import coiled
 from coiled.cli.cluster.ssh import add_key_to_agent, check_ssh
 from coiled.compatibility import DISTRIBUTED_VERSION
 from coiled.errors import DoesNotExist
 
 from ..utils import CONTEXT_SETTINGS
 
 # Path on VM to sync to.
 # We use `/scratch` for now because it's already bind-mounted into docker.
 SYNC_TARGET = "/scratch/synced"
-MIN_DISTRIBUTED_VERSION = "2022.8.1"
+MIN_DISTRIBUTED_VERSION = Version("2022.8.1")
 MUTAGEN_NAME_FORMAT = "coiled-{cluster_id}"
 
 
 def check_distributed_version() -> bool:
     if DISTRIBUTED_VERSION < MIN_DISTRIBUTED_VERSION:
         print(
             "[bold red]"
@@ -66,27 +69,14 @@
 def check_ssh_keygen() -> bool:
     if not shutil.which("ssh-keygen"):
         print("[bold red]Unable to find `ssh-keygen`, you may need to install OpenSSH or add it to your paths.[/]")
         return False
     return True
 
 
-def cwd_cluster_name():
-    "Get a name for the notebook based on the hash of the current path."
-    # Based on https://github.com/python-poetry/poetry/blob/fa5543a6/src/poetry/utils/env.py#L1210-L1212
-    cwd = os.getcwd()
-    normalized_cwd = os.path.normcase(os.path.realpath(cwd))
-    h_bytes = hashlib.sha256(normalized_cwd.encode()).digest()
-    h_str = base64.urlsafe_b64encode(h_bytes).decode()[:8]
-
-    basename = os.path.basename(normalized_cwd)
-    sanitized_name = re.sub(r'[ $`!*@"/\\\r\n\t\.]', "_", basename)[:42]
-    return f"notebook-{sanitized_name}-{h_str}"
-
-
 def mutagen_session_exists(cluster_id: int) -> bool:
     sessions = (
         subprocess.run(
             [
                 "mutagen",
                 "sync",
                 "list",
@@ -116,15 +106,15 @@
 
     raise RuntimeError(f"Multiple mutagen sessions found for cluster {cluster_id}: {sessions}")
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
 @click.option(
     "--name",
-    default=cwd_cluster_name(),
+    default=None,
     help="Cluster name. If not given, defaults to a hash based on current working directory.",
 )
 @click.option(
     "--account",
     default=None,
     help="Coiled account (uses default account if not specified)",
 )
@@ -164,23 +154,30 @@
 )
 @click.option(
     "--open",
     default=True,
     is_flag=True,
     help="Whether to open the notebook in the default browser once it's launched",
 )
+@click.option(
+    "--block/--no-block",
+    default=True,
+    is_flag=True,
+    help="Whether to block while the notebook is running.",
+)
 def start_notebook(
-    name: str,
+    name: Optional[str],
     account: Optional[str],
     sync: bool,
     software: Optional[str],
     container: Optional[str],
     vm_type: Sequence[str],
     gpu: bool,
     open: bool,
+    block: bool,
 ):
     """
     Launch or re-open a notebook session, with optional file syncing.
 
     If a notebook session with the same ``name`` already exists, it's not re-created.
     If file sync was initially not enabled, running ``coiled notebook start --sync``
     will begin file sync without re-launching the notebook.
@@ -200,14 +197,15 @@
     if sync and not (check_mutagen() and check_ssh() and check_ssh_keygen()):
         return
 
     env = None
     if container and "rapidsai" in container:
         env = {"DISABLE_JUPYTER": "true"}  # needed for "stable" RAPIDS image
 
+    name = name or f"notebook-{uuid.uuid4().hex[:8]}"
     with coiled.Cloud(account=account) as cloud:
         print(f"Starting notebook [bold]{name}[/bold]...")
         # TODO how can we get the widget to show up during CLI commands?
         cluster = coiled.Cluster(
             name=name,
             cloud=cloud,
             n_workers=0,
@@ -215,14 +213,15 @@
             container=container,
             jupyter=True,
             scheduler_options={"idle_timeout": "24 hours"},
             scheduler_vm_types=list(vm_type) if vm_type else None,
             allow_ssh=True,
             environ=env,
             scheduler_gpu=gpu,
+            tags={"coiled-cluster-type": "notebook"},
         )
 
         url = cluster.jupyter_link
         cluster_id = cluster.cluster_id
         assert cluster_id is not None
         if sync:
             url = parse_url(url)._replace(path="/jupyter/lab/tree/synced").url
@@ -285,29 +284,58 @@
                     ],
                     check=True,
                 )
 
     print(f"[bold]Jupyter available at {url}[/]")
     print()
 
-    stop_command = f"coiled notebook stop --name {name}"
-    if account:
-        stop_command = f"{stop_command} --account {account}"
-
-    print(f"To stop this notebook server: [green]{stop_command}[/]")
     if open:
         webbrowser.open(url, new=2)
 
+    if block:
+        print("[green]Use Control-C to stop this notebook server [/]")
+        with Progress(SpinnerColumn()) as progress:
+            # Wait for shutdown signal from user
+
+            def signal_handler(signal, frame):
+                progress.stop()
+                if interrupt_nested.is_set():
+                    return
+                else:
+                    interrupt_nested.set()
+                    if Confirm.ask("Are you sure you want to stop this notebook server?", default=True):
+                        interrupt.set()
+                    else:
+                        print("[green]Continuing with this notebook server... [/]")
+                        progress.start()
+                        interrupt_nested.clear()
+
+            signal.signal(signal.SIGINT, signal_handler)
+            interrupt = threading.Event()
+            interrupt_nested = threading.Event()
+            progress.add_task("spinning...", total=None)  # starts an infinite spinner
+            interrupt.wait()
+
+        # `.callback` gets the underlying function from the click command.
+        # It can sometimes be `None`. Not sure why, but we handle that case here
+        # to make type checking happy.
+        stop_func = stop_notebook.callback
+        if stop_func is not None:
+            stop_func(name, account)
+    else:
+        stop_command = "coiled notebook stop"
+        if account:
+            stop_command = f"{stop_command} --account {account}"
+        stop_command = f"{stop_command} {name}"
+
+        print(f"To stop this notebook server: [green]{stop_command}[/]")
+
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-@click.option(
-    "--name",
-    default=cwd_cluster_name(),
-    help=("Cluster name. If not given, defaults to a hash based on current working directory."),
-)
+@click.argument("name")
 @click.option(
     "--account",
     default=None,
     help="Coiled account (uses default account if not specified)",
 )
 def stop_notebook(name: str, account: Optional[str]):
     "Shut down a notebook session."
@@ -348,19 +376,15 @@
             )
 
         print(f"Stopping notebook {name!r} ({cluster_id})...")
         cloud.delete_cluster(cluster_id)
 
 
 @click.command(context_settings=CONTEXT_SETTINGS)
-@click.option(
-    "--name",
-    default=cwd_cluster_name(),
-    help=("Cluster name. If not given, defaults to a hash based on current working directory."),
-)
+@click.argument("name")
 def monitor_sync(name: str):
     "Monitor file sync status for a notebook session."
     if not check_mutagen():
         return
 
     with coiled.Cloud() as cloud:
         try:
```

### Comparing `coiled-0.6.9/coiled/cli/setup/__init__.py` & `coiled-0.7.0/coiled/cli/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/setup/amp.py` & `coiled-0.7.0/coiled/cli/setup/amp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/setup/aws.py` & `coiled-0.7.0/coiled/cli/setup/aws.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/setup/entry.py` & `coiled-0.7.0/coiled/cli/setup/entry.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/setup/gcp.py` & `coiled-0.7.0/coiled/cli/setup/gcp.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/cli/setup/prometheus.py` & `coiled-0.7.0/coiled/cli/setup/prometheus.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/coiled/v2/__init__.py` & `coiled-0.7.0/coiled/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/LICENSE` & `coiled-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/README.md` & `coiled-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `coiled-0.6.9/pyproject.toml` & `coiled-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,29 +11,30 @@
     "dask>=2.23.0",
     "distributed>=2.23.0",
     "filelock",
     "importlib-metadata",
     "ipywidgets",
     "jmespath",
     "jsondiff",
+    "packaging",
     "pip",
     "pip>=19.3",
     "prometheus_client",
     "rich>=11.2.0",
     "setuptools>=49.3.0",
     "typing_extensions",
     "wheel",
 ]
 description = ""
 dynamic = ["version"]
 license = ""
 maintainers = [{ name = "Coiled", email = "info@coiled.io" }]
 name = "coiled"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 
 [project.scripts]
 coiled = "coiled.cli.core:cli"
 
 [project.urls]
 Homepage = "https://coiled.io"
```

### Comparing `coiled-0.6.9/PKG-INFO` & `coiled-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: coiled
-Version: 0.6.9
+Version: 0.7.0
 Project-URL: Homepage, https://coiled.io
 Maintainer-email: Coiled <info@coiled.io>
 License-File: LICENSE
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Requires-Dist: backoff
 Requires-Dist: boto3
 Requires-Dist: click>=7.1
 Requires-Dist: dask>=2.23.0
 Requires-Dist: distributed>=2.23.0
 Requires-Dist: filelock
 Requires-Dist: importlib-metadata
 Requires-Dist: ipywidgets
 Requires-Dist: jmespath
 Requires-Dist: jsondiff
+Requires-Dist: packaging
 Requires-Dist: pip
 Requires-Dist: pip>=19.3
 Requires-Dist: prometheus-client
 Requires-Dist: rich>=11.2.0
 Requires-Dist: setuptools>=49.3.0
 Requires-Dist: typing-extensions
 Requires-Dist: wheel
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: coiled Version: 0.6.9 Project-URL: Homepage, https:
+Metadata-Version: 2.1 Name: coiled Version: 0.7.0 Project-URL: Homepage, https:
 //coiled.io Maintainer-email: Coiled
-coiled.io> License-File: LICENSE Requires-Python: >=3.7 Requires-Dist: aiohttp
+coiled.io> License-File: LICENSE Requires-Python: >=3.8 Requires-Dist: aiohttp
 Requires-Dist: backoff Requires-Dist: boto3 Requires-Dist: click>=7.1 Requires-
 Dist: dask>=2.23.0 Requires-Dist: distributed>=2.23.0 Requires-Dist: filelock
 Requires-Dist: importlib-metadata Requires-Dist: ipywidgets Requires-Dist:
-jmespath Requires-Dist: jsondiff Requires-Dist: pip Requires-Dist: pip>=19.3
-Requires-Dist: prometheus-client Requires-Dist: rich>=11.2.0 Requires-Dist:
-setuptools>=49.3.0 Requires-Dist: typing-extensions Requires-Dist: wheel
-Description-Content-Type: text/markdown
+jmespath Requires-Dist: jsondiff Requires-Dist: packaging Requires-Dist: pip
+Requires-Dist: pip>=19.3 Requires-Dist: prometheus-client Requires-Dist:
+rich>=11.2.0 Requires-Dist: setuptools>=49.3.0 Requires-Dist: typing-extensions
+Requires-Dist: wheel Description-Content-Type: text/markdown
                                    [Coiled]
              Coiled.io â¢ Documentation â¢ Community â¢ Support
 Coiled is a deployment-as-a-service library for scaling Python with Dask, a
 popular open source library for parallel analytics. Coiled manages cloud
 resources, networking, software environments, and everything you need to scale
 Python in the cloud robustly and easily. Go to https://cloud.coiled.io to get
 started with Coiled.
```

