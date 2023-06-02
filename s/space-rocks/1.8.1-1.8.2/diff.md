# Comparing `tmp/space_rocks-1.8.1.tar.gz` & `tmp/space_rocks-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_rocks-1.8.1.tar", max compression
+gzip compressed data, was "space_rocks-1.8.2.tar", max compression
```

## Comparing `space_rocks-1.8.1.tar` & `space_rocks-1.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.8.1/LICENSE
--rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.8.1/README.md
--rw-r--r--   0        0        0     1519 2023-05-25 09:25:12.015727 space_rocks-1.8.1/pyproject.toml
--rw-r--r--   0        0        0      450 2023-05-25 09:25:06.687727 space_rocks-1.8.1/rocks/__init__.py
--rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.8.1/rocks/cache.py
--rw-r--r--   0        0        0    11492 2023-05-10 09:34:41.049861 space_rocks-1.8.1/rocks/cli.py
--rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.8.1/rocks/config.py
--rw-r--r--   0        0        0    39666 2023-05-06 14:21:15.505975 space_rocks-1.8.1/rocks/core.py
--rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.8.1/rocks/datacloud.py
--rw-r--r--   0        0        0    13082 2023-04-25 11:37:04.378144 space_rocks-1.8.1/rocks/index.py
--rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.8.1/rocks/logging.py
--rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.8.1/rocks/metadata.py
--rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.8.1/rocks/plots.py
--rw-r--r--   0        0        0    12799 2023-04-24 08:24:01.017288 space_rocks-1.8.1/rocks/resolve.py
--rw-r--r--   0        0        0    12222 2023-05-04 09:06:04.136860 space_rocks-1.8.1/rocks/ssodnet.py
--rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 space_rocks-1.8.1/setup.py
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 space_rocks-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-21 07:53:47.207007 space_rocks-1.8.2/LICENSE
+-rw-r--r--   0        0        0     1731 2023-04-21 07:53:47.207007 space_rocks-1.8.2/README.md
+-rw-r--r--   0        0        0     1519 2023-06-02 15:35:49.717529 space_rocks-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0      450 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/__init__.py
+-rw-r--r--   0        0        0     4886 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/cache.py
+-rw-r--r--   0        0        0    11457 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/cli.py
+-rw-r--r--   0        0        0     7078 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/config.py
+-rw-r--r--   0        0        0    39666 2023-05-26 20:42:35.837290 space_rocks-1.8.2/rocks/core.py
+-rw-r--r--   0        0        0    32930 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/datacloud.py
+-rw-r--r--   0        0        0    14953 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/index.py
+-rw-r--r--   0        0        0      982 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/logging.py
+-rw-r--r--   0        0        0     3765 2023-04-21 07:53:47.215006 space_rocks-1.8.2/rocks/metadata.py
+-rw-r--r--   0        0        0     6300 2023-02-19 15:02:48.465877 space_rocks-1.8.2/rocks/plots.py
+-rw-r--r--   0        0        0    13145 2023-06-02 15:35:49.717529 space_rocks-1.8.2/rocks/resolve.py
+-rw-r--r--   0        0        0    12222 2023-05-04 09:06:04.136860 space_rocks-1.8.2/rocks/ssodnet.py
+-rw-r--r--   0        0        0     3198 1970-01-01 00:00:00.000000 space_rocks-1.8.2/setup.py
+-rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 space_rocks-1.8.2/PKG-INFO
```

### Comparing `space_rocks-1.8.1/LICENSE` & `space_rocks-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/README.md` & `space_rocks-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/pyproject.toml` & `space_rocks-1.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "space-rocks"
-version = "1.8.1"
+version = "1.8.2"
 description = "Python client for SsODNet data access."
 authors = ["Max Mahlke <max.mahlke@oca.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://rocks.readthedocs.io/en/latest/"
 documentation = "https://rocks.readthedocs.io/en/latest/"
 repository = "https://github.com/maxmahlke/rocks.git"
```

### Comparing `space_rocks-1.8.1/rocks/cache.py` & `space_rocks-1.8.2/rocks/cache.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/cli.py` & `space_rocks-1.8.2/rocks/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from rocks import __version__
 
 
 class AliasedGroup(click.Group):
     """Click group with custom default mode implementation."""
 
     def get_command(self, ctx, cmd_name):
-
         # ------
         # Resolve known commands
 
         # Add command aliases
         if cmd_name == "identify":
             cmd_name = "id"
         elif cmd_name == "aliases":
@@ -126,21 +125,19 @@
     """Echo the aliases of an asteroid."""
 
     if not id_:
         id_ = resolve._interactive()
     else:
         id_ = id_[0]
 
-    name, number, ssodnetid = resolve.identify(id_, return_id=True)  # type: ignore
+    name, number, *aliases = resolve.identify(id_, return_aliases=True, local=False)  # type: ignore
 
     if name is None:
         sys.exit()
 
-    aliases = index.get_aliases(ssodnetid)
-
     rich.print(f"({number}) {name}, aka \n {aliases}")
 
 
 @cli_rocks.command()
 @click.option(
     "--clear",
     "-c",
@@ -184,17 +181,15 @@
     else:
         rich.print(
             f"[green] the latest version ({__version__}) is installed.[/green]\n"
         )
 
     # Update or clear
     if cached_cards:
-
         if not clear and not update:
-
             decision = prompt.Prompt.ask(
                 "Update or clear the cached ssoCards and datacloud catalogues?\n"
                 "[blue][0][/blue] Do nothing "
                 "[blue][1][/blue] Clear the cache "
                 "[blue][2][/blue] Update the data",
                 choices=["0", "1", "2", "3"],
                 show_choices=False,
@@ -204,37 +199,34 @@
             decision = "none"
 
         if clear or decision == "1":
             rich.print("\nClearing the cached ssoCards and datacloud catalogues..")
             cache.clear()
 
         elif update or decision == "2":
-
             # Update metadata
             metadata.retrieve("mappings")
 
             # Update ssoCards
             rich.print("\n(1/2) Updating the cached ssoCards..")
             cache.update_cards(cached_cards)
 
             # Update datacloud catalogues
             rich.print("\n(2/2) Updating the cached datacloud catalogues..")
             cache.update_catalogues(cached_catalogues)
 
         elif decision == "3":
-
             from rich.console import Console
 
             with Console().status("Observing all asteroids.. [~11GB]", spinner="earth"):
                 cache.retrieve_all_ssocards()
 
     # ------
     # Update asteroid name-number index
     if not clear and not update:
-
         decision = prompt.Prompt.ask(
             "\nUpdate the asteroid name-number index?\n"
             "[blue][0][/blue] No "
             "[blue][1][/blue] Yes",
             choices=["0", "1"],
             show_choices=False,
             default="1",
@@ -293,26 +285,24 @@
     import keyword
 
     from rocks import core
     from rocks import datacloud
 
     # Should we plot?
     for arg in ["-p", "--plot"]:
-
         if arg in sys.argv:
             sys.argv.remove(arg)
 
             plot = True
             break
     else:
         plot = False
 
     # Verbose output?
     for arg in ["-v", "--verbose"]:
-
         if arg in sys.argv:
             sys.argv.remove(arg)
 
             verbose = True
             break
     else:
         verbose = False
```

### Comparing `space_rocks-1.8.1/rocks/config.py` & `space_rocks-1.8.2/rocks/config.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/core.py` & `space_rocks-1.8.2/rocks/core.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/datacloud.py` & `space_rocks-1.8.2/rocks/datacloud.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/index.py` & `space_rocks-1.8.2/rocks/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Asteroid name-number index functions for rocks."""
 
+from concurrent.futures import ProcessPoolExecutor
 from functools import lru_cache
+import multiprocessing
 import pickle
 import pickletools
 import re
 import string
 import sys
 import typing
 import time
 
 import numpy as np
 import rich
-from rich import progress
+from rich import console, progress
 
 from rocks import __version__
 from rocks import config
 from rocks import resolve
 from rocks.logging import logger
 
 
@@ -23,55 +25,84 @@
 # Building the index
 def _build_index():
     """Build asteroid name-number index from SsODNet sso_index."""
 
     config.PATH_INDEX.mkdir(exist_ok=True, parents=True)
 
     tasks_descs = [
-        (_build_fuzzy_searchable_index, ":kiwi_fruit: Differentiating parent bodies"),
-        (_build_number_index, ":ringed_planet: Cleaning out resonances"),
-        (_build_name_index, ":waning_gibbous_moon: Gardening the regolith"),
-        (_build_designation_index, ":five:  Assigning numbers"),
-        (_build_palomar_transit_index, ":u6307: Composing name citations"),
-        (_build_index_of_aliases, ":comet: Index updated"),
+        (_build_fuzzy_searchable_index, f"[dim]{'Differentiating Parent Bodies':>36}"),
+        (_build_number_index, f"[dim]{'Gardening Regolith':>36}"),
+        (_build_name_index, f"[dim]{'Clearing out Resonances':>36}"),
+        (_build_designation_index, f"[dim]{'Populating near-Earth Space':>36}"),
+        (_build_palomar_transit_index, f"[dim]{'Separating Trojans':>36}"),
     ]
 
+    # ------
+    # Retrieve index while showing spinner
+    c = console.Console()
+    with c.status("Searching for minor bodies...", spinner="dots8Bit"):
+        index = _retrieve_index_from_ssodnet()
+
+    # ------
+    # Process index with multiple process
+    N_WORKERS = 5  # number of processes to launch
+
     with progress.Progress(
         "[progress.description]{task.description}",
         progress.BarColumn(),
         "[progress.percentage]{task.percentage:>3.0f}%",
     ) as pbar:
-        # Initiate progress bar and retrieve index from SsODNet
-        steps = pbar.add_task(
-            ":telescope: Counting minor bodies", total=len(tasks_descs) + 1
-        )
-        index = _retrieve_index_from_ssodnet()
-        pbar.update(steps, description=f":telescope: Found {len(index):,} ", advance=1)
-
-        for task, desc in tasks_descs:
-            task(index)
-            pbar.update(steps, description=desc, advance=1)
-
-
-def _build_index_of_aliases(index):
-    """Create the SsODNetID -> aliases index.
+        futures = []
 
-    Parameters
-    ----------
-    index : pd.DataFrame
-        The formatted index from SsODNet.
-    """
+        with multiprocessing.Manager() as manager:
+            _progress = manager.dict()
+            overall_progress_task = pbar.add_task(
+                f"Processing {len(index):,} minor bodies..."
+            )
 
-    index.Aliases = index.Aliases.str.split(";")
-    index = index.set_index("SsODNetID")
-    aliases = index.Aliases.to_dict()
-    _write_to_cache(aliases, "aliases.pkl")
+            with ProcessPoolExecutor(max_workers=N_WORKERS) as executor:
+                for task, desc in tasks_descs:  # iterate over the jobs we need to run
+                    task_id = pbar.add_task(desc, visible=True)
+                    futures.append(executor.submit(task, index, _progress, task_id))
+
+                # monitor the progress
+                n_finished = 0
+                while n_finished < len(futures):
+
+                    # Update overall bar
+                    pbar.update(
+                        overall_progress_task, completed=n_finished, total=len(futures)
+                    )
+                    for task_id, update_data in _progress.items():
+                        latest = update_data["progress"]
+                        total = update_data["total"]
+
+                        # update the progress bar for task
+                        pbar.update(
+                            task_id,
+                            completed=latest,
+                            total=total,
+                            visible=latest < total,
+                        )
+                    # see if we're done
+                    n_finished = sum([future.done() for future in futures])
+
+                # raise any errors:
+                for future in futures:
+                    future.result()
+
+            pbar.update(
+                overall_progress_task,
+                completed=len(futures),
+                total=len(futures),
+                description="All done!",
+            )
 
 
-def _build_number_index(index):
+def _build_number_index(index, pbar, task_id):
     """Build the number -> name,SsODNetID index parts.
 
     Parameters
     ----------
     index : pd.DataFrame
         The formatted index from SsODNet.
     """
@@ -79,49 +110,53 @@
     import pandas as pd
 
     SIZE = 1e3  # Build chunks of 1k entries
 
     # Find next 10,000 to largest number
     numbered = index[~pd.isna(index.Number)]
     parts = np.arange(1, np.ceil(numbered.Number.max() / SIZE) * SIZE, SIZE, dtype=int)
+    pbar[task_id] = {"progress": 0, "total": len(parts)}
 
-    for part in parts:
+    for i, part in enumerate(parts):
         part_index = numbered.loc[
             (part <= numbered.Number) & (numbered.Number < part + SIZE)
         ]
 
         part_index = dict(
             zip(
                 part_index.Number,
                 part_index[["Name", "SsODNetID"]].to_numpy().tolist(),
             )
         )
 
         _write_to_cache(part_index, f"{part}.pkl")
 
+        pbar[task_id] = {"progress": i + 1, "total": len(parts)}
 
-def _build_name_index(index):
+
+def _build_name_index(index, pbar, task_id):
     """Build the reduced -> number,SsODNetID index.
 
     Parameters
     ----------
     index : pd.DataFrame
         The formatted index from SsODNet.
     """
 
     import pandas as pd
 
     parts = string.ascii_lowercase  # first character of name
+    pbar[task_id] = {"progress": 0, "total": len(parts)}
 
     index = index[~pd.isna(index.Number)]
 
     names = set(red for red in index.Reduced if re.match(r"^[a-z\'-]*$", red))
     names.add(r"g!kun||'homdima")  # everyone's favourite shell injection
 
-    for part in parts:
+    for i, part in enumerate(parts):
         names_subset = set(name for name in names if name.startswith(part))
 
         if part == "a":
             names_subset.add(
                 "'aylo'chaxnim"
             )  # another edge case for the daughter of venus
         part_index = index.loc[index.Reduced.isin(names_subset)]
@@ -129,49 +164,28 @@
             zip(
                 part_index.Reduced,
                 part_index[["Name", "Number", "SsODNetID"]].to_numpy().tolist(),
             )
         )
 
         _write_to_cache(part_index, f"{part}.pkl")
+        pbar[task_id] = {"progress": i + 1, "total": len(parts)}
 
 
-def _build_designation_index(index):
+def _build_designation_index(index, pbar, task_id):
     """Build the designation -> name,number,SsODNetID index.
 
     Parameters
     ----------
     index : pd.DataFrame
         The formatted index from SsODNet.
     """
-
     import pandas as pd
 
-    designations = set(
-        red
-        for red in index.Reduced
-        if re.match(
-            r"(^([11][8-9][0-9]{2}[a-z]{2}[0-9]{0,3}$)|"
-            r"(^20[0-9]{2}[a-z]{2}[0-9]{0,3}$))",
-            red,
-        )
-    )
-    max_year = max([int(year[2:4]) for year in designations if year.startswith("20")])
-    parts = [
-        "18",
-        "19",
-        *[f"20{year:02}" for year in range(0, max_year + 1)],
-    ]
-
-    for part in parts:
-        part_designations = set(desi for desi in designations if desi.startswith(part))
-
-        # Asteroids in this chunk
-        part_index = index.loc[index.Reduced.isin(part_designations)]
-
+    def _convert_part(part, part_index):
         no_number = pd.isna(part_index.Number)
         has_number = part_index[~no_number]
         no_number = part_index[no_number]
 
         part_index = dict(
             zip(
                 has_number.Reduced,
@@ -184,27 +198,57 @@
                 no_number.Reduced,
                 no_number[["Name", "SsODNetID"]].values.tolist(),
             )
         )
 
         _write_to_cache(part_index, f"d{part}.pkl")
 
+    designations = set(
+        red
+        for red in index.Reduced
+        if re.match(
+            r"(^([11][8-9][0-9]{2}[a-z]{2}[0-9]{0,3}$)|"
+            r"(^20[0-9]{2}[a-z]{2}[0-9]{0,3}$))",
+            red,
+        )
+    )
+
+    index = index[index.Reduced.isin(designations)]
+
+    # treat 18xx and 19xx separately
+    part_18 = index.Reduced.str.startswith("18")
+    pbar[task_id] = {"progress": 1, "total": 26}
+    part_19 = index.Reduced.str.startswith("19")
+    pbar[task_id] = {"progress": 2, "total": 26}
+
+    _convert_part("18", index[part_18])
+    _convert_part("19", index[part_19])
+
+    index = index[(~part_18) & (~part_19)]
 
-def _build_palomar_transit_index(index):
+    # now divide by year
+    index["parts"] = index.Reduced.str[:4]
+    for i, (part, part_index) in enumerate(index.groupby("parts")):
+        _convert_part(part, part_index)
+        pbar[task_id] = {"progress": i + 3, "total": 26}
+
+
+def _build_palomar_transit_index(index, pbar, task_id):
     """Build the reduced -> name,number,SsODNetID index for anything that is not
     a name and not a designation.
 
     Parameters
     ----------
     index : pd.DataFrame
         The formatted index from SsODNet.
     """
 
     import pandas as pd
 
+    pbar[task_id] = {"progress": 1, "total": 2}
     rest = set(
         red
         for red in index.Reduced
         if not re.match(
             r"(^([11][8-9][0-9]{2}[a-z]{2}[0-9]{0,3}$)|"
             r"(^20[0-9]{2}[a-z]{2}[0-9]{0,3}$))",
             red,
@@ -229,27 +273,30 @@
         zip(
             no_number.Reduced,
             no_number[["Name", "SsODNetID"]].to_numpy().tolist(),
         )
     )
 
     _write_to_cache(part_index, "PLT.pkl")
+    pbar[task_id] = {"progress": 2, "total": 2}
 
 
-def _build_fuzzy_searchable_index(index):
+def _build_fuzzy_searchable_index(index, pbar, task_id):
     """Merge name, number and SsODNet ID of all entries to fuzzy-searchable lines.
 
     Parameters
     ----------
     index : pd.DataFrame
         The formatted index from SsODNet.
     """
 
     import pandas as pd
 
+    pbar[task_id] = {"progress": 1, "total": 2}
+
     index = index.sort_values(["Number", "Name"])
 
     no_number = pd.isna(index.Number)
     has_number = index[~no_number]
     no_number = index[no_number]
 
     numbered = (
@@ -262,14 +309,15 @@
     ]
     LINES += [
         line.encode(sys.getdefaultencoding()) + b"\n"
         for line in unnumbered.to_numpy().tolist()
     ]
 
     _write_to_cache(LINES, "fuzzy_index.pkl")
+    pbar[task_id] = {"progress": 2, "total": 2}
 
 
 def _write_to_cache(obj, filename):
     """Save the pickled object to the path in the rocks cache.
 
     Parameters
     ----------
@@ -300,37 +348,24 @@
     # The gzipped index is exposed under this address
     URL_INDEX = "https://asterm.imcce.fr/public/ssodnet/sso_index.csv.gz"
     index = pd.read_csv(URL_INDEX)
 
     # There are some spurious spaces in the column headers
     index = index.rename(columns={c: c.replace(" ", "") for c in index.columns})
 
+    # Don't need other columns
+    index = index[["Name", "Number", "SsODNetID", "Reduced"]]
+
     # We use NaNs instead of 0 for unnumbered objects
     index.loc[index["Number"] == 0, "Number"] = np.nan
     index["Number"] = index["Number"].astype("Int64")
 
     return index
 
 
-def get_aliases(ssodnetid):
-    """Return the aliases of the passed reduced identifier.
-
-    Parameters
-    ----------
-    ssodnetid :  str
-        The SsODNetID of the asteroid to alias.
-
-    Returns
-    -------
-    list
-        The list of aliases of the asteroid.
-    """
-    return _load("aliases.pkl")[ssodnetid]
-
-
 def _get_index_file(id_: typing.Union[int, str]) -> dict:
     """Get part of the index where id_ is located.
 
     Parameters
     ----------
     id_ : str, int
         The asteroid identifier.
@@ -348,15 +383,14 @@
             index_number = index_range[index_range <= id_][-1]
         # The passed id_ is larger than 1e6
         except IndexError:
             index_number = 1
         which = f"{index_number}.pkl"
 
         if not (config.PATH_INDEX / which).exists():
-
             if id_ > 1e6:
                 logger.error(
                     f"The provided number {id_} is larger than the largest number of any asteroid."
                 )
             else:
                 logger.error(
                     f"Could not resolve asteroid number {id_}. The index may be broken, run \n'$ rocks status --update' to update it."
```

### Comparing `space_rocks-1.8.1/rocks/logging.py` & `space_rocks-1.8.2/rocks/logging.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/metadata.py` & `space_rocks-1.8.2/rocks/metadata.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/plots.py` & `space_rocks-1.8.2/rocks/plots.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/rocks/resolve.py` & `space_rocks-1.8.2/rocks/resolve.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,24 +33,27 @@
     except RuntimeError as ex:
         if "There is no current event loop in thread" in str(ex):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             return asyncio.get_event_loop()
 
 
-def identify(id_, return_id=False, local=True, progress=False):
+def identify(id_, return_id=False, return_aliases=False, local=True, progress=False):
     """Resolve names and numbers of one or more minor bodies using identifiers.
 
     Parameters
     ----------
     id_ : str, int, float, list, range, set, np.ndarray, pd.Series
         One or more identifying names or numbers to resolve.
     return_id : bool
         Return the SsODNet ID of the asteroid as third member of
         the tuple. Default is False.
+    return_list : bool
+        Return the known aliases of the asteroid as third member of
+        the tuple. Default is False.
     local : bool
         Try resolving the name locally first. Default is True.
     progress : bool
         Show progress bar. Default is False.
 
     Returns
     -------
@@ -123,16 +126,21 @@
             results[idx_failed] = loop.run_until_complete(
                 _identify(np.array(id_)[idx_failed], local, progress_bar, task)
             )
             results = results.tolist()
 
     # ------
     # Verify the output format
-    if not return_id:
+    if not return_id and not return_aliases:
         results = [r[:2] for r in results]
+    else:
+        if return_id:
+            results = [r[:3] for r in results]
+        else:
+            results = [r[:2] + tuple(r[-1]) for r in results]
 
     if len(id_) == 1:  # type: ignore
         results = results[0]
 
     return results  # type: ignore
 
 
@@ -394,15 +402,15 @@
         # Unclear which match is correct.
         logger.warning(f"Could not identify '{id_}'.")
         return (None, np.nan, None)
 
     # Found match
     numeric = [int(alias) for alias in match["aliases"] if alias.isnumeric()]
     number = min(numeric) if numeric else np.nan
-    return (match["name"], number, match["id"])
+    return (match["name"], number, match["id"], match["aliases"])
 
 
 def _interactive():
     """Launch interactive, fuzzy-searchable selection of asteroid.
 
     Returns
     -------
```

### Comparing `space_rocks-1.8.1/rocks/ssodnet.py` & `space_rocks-1.8.2/rocks/ssodnet.py`

 * *Files identical despite different names*

### Comparing `space_rocks-1.8.1/setup.py` & `space_rocks-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
  ':python_version >= "3.7" and python_version < "3.11"': ['numpy>=1.21']}
 
 entry_points = \
 {'console_scripts': ['rocks = rocks.cli:cli_rocks']}
 
 setup_kwargs = {
     'name': 'space-rocks',
-    'version': '1.8.1',
+    'version': '1.8.2',
     'description': 'Python client for SsODNet data access.',
     'long_description': '<p align="center">\n  <img width="260" src="https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/logo_rocks.svg">\n</p>\n\n<p align="center">\n  <a href="https://github.com/maxmahlke/rocks#features"> Features </a> - <a href="https://github.com/maxmahlke/rocks#install"> Install </a> - <a href="https://github.com/maxmahlke/rocks#documentation"> Documentation </a>\n</p>\n\n<br>\n\n<div align="center">\n  <a href="https://img.shields.io/pypi/pyversions/space-rocks">\n    <img src="https://img.shields.io/pypi/pyversions/space-rocks"/>\n  </a>\n  <a href="https://img.shields.io/pypi/v/space-rocks">\n    <img src="https://img.shields.io/pypi/v/space-rocks"/>\n  </a>\n  <a href="https://readthedocs.org/projects/rocks/badge/?version=latest">\n    <img src="https://readthedocs.org/projects/rocks/badge/?version=latest"/>\n  </a>\n  <a href="https://arxiv.org/abs/2209.10697">\n    <img src="https://img.shields.io/badge/arXiv-2209.10697-f9f107.svg"/>\n  </a>\n</div>\n\n<br>\n\n## Features\n\nExplore asteroid data on the command-line...\n\n``` sh\n$ rocks id 221\n(221) Eos\n\n$ rocks class Eos\nMB>Outer\n\n$ rocks albedo Eos\n0.136 +- 0.004\n\n$ rocks taxonomy Eos\nK\n\n$ rocks density Eos\n4.559e+03 +- 1.139e+03 kg/m$^3$\n```\n\n... and in a `python` script.\n\n``` python\n>>> import rocks\n>>> rocks.identify("1902ug")\n(\'Fortuna\', 19)\n>>> ceres = rocks.Rock("ceres")\n>>> ceres.diameter.value\n848.4\n>>> ceres.diameter.unit\n\'km\'\n>>> ceres.mass.value\n9.384e+20\n>>> ceres.mass.error\n6.711e+17\n```\n\n## Install\n\nInstall from PyPi using `pip`:\n\n     $ pip install space-rocks\n\nThe minimum required `python` version is 3.7.\n\n\n## Documentation\n\nCheck out the documentation at [rocks.readthedocs.io](https://rocks.readthedocs.io/en/latest/) or run\n\n     $ rocks docs\n',
     'author': 'Max Mahlke',
     'author_email': 'max.mahlke@oca.eu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://rocks.readthedocs.io/en/latest/',
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 'matplotlib>=3.4.3', 'nest-asyncio>=1.5.1,<2.0.0', 'pandas>=1.3.5',
 'platformdirs>=2.6.2,<3.0.0', 'pydantic>=1.8.2,<2.0.0', 'rapidfuzz>=3,<4',
 'requests>=2.26.0,<3.0.0', 'rich>=12.2.0', 'sphinx-copybutton>=0.5.0,<0.6.0',
 'sphinx_design>=0.3.0,<0.4.0'] extras_require = \ {':python_version >= "3.11"
 and python_version < "4.0"': ['numpy>=1.24'], ':python_version >= "3.7" and
 python_version < "3.11"': ['numpy>=1.21']} entry_points = \ {'console_scripts':
 ['rocks = rocks.cli:cli_rocks']} setup_kwargs = { 'name': 'space-rocks',
-'version': '1.8.1', 'description': 'Python client for SsODNet data access.',
+'version': '1.8.2', 'description': 'Python client for SsODNet data access.',
 'long_description': '
   \n [https://raw.githubusercontent.com/maxmahlke/rocks/master/docs/_static/
                                logo_rocks.svg]\n
 \n\n
                     \n Features - Install - Documentation\n
 \n\n
 \n\n
```

### Comparing `space_rocks-1.8.1/PKG-INFO` & `space_rocks-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: space-rocks
-Version: 1.8.1
+Version: 1.8.2
 Summary: Python client for SsODNet data access.
 Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT
 Author: Max Mahlke
 Author-email: max.mahlke@oca.eu
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: space-rocks Version: 1.8.1 Summary: Python client
+Metadata-Version: 2.1 Name: space-rocks Version: 1.8.2 Summary: Python client
 for SsODNet data access. Home-page: https://rocks.readthedocs.io/en/latest/
 License: MIT Author: Max Mahlke Author-email: max.mahlke@oca.eu Requires-
 Python: >=3.7.1,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist: Levenshtein
```

