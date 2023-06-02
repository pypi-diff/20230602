# Comparing `tmp/dask_awkward-2023.5.1.tar.gz` & `tmp/dask_awkward-2023.6.0.tar.gz`

## Comparing `dask_awkward-2023.5.1.tar` & `dask_awkward-2023.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0    61467 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     5894 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15172 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14183 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/LICENSE
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/README.md
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0     6818 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0    61474 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    15303 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    11155 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    27429 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    16762 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/README.md
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dask_awkward-2023.6.0/PKG-INFO
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.6.0/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/typing.py` & `dask_awkward-2023.6.0/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/utils.py` & `dask_awkward-2023.6.0/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.6.0/src/dask_awkward/layers/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import TYPE_CHECKING, Any
 
 from dask.blockwise import Blockwise, BlockwiseDepDict, blockwise_token
 
 from dask_awkward.utils import LazyInputsDict
 
 if TYPE_CHECKING:
-    from awkward._nplikes.typetracer import TypeTracerReport
+    from awkward.typetracer import TypeTracerReport
 
 
 class AwkwardBlockwiseLayer(Blockwise):
     """Just like upstream Blockwise, except we override pickling"""
 
     @classmethod
     def from_blockwise(cls, layer) -> AwkwardBlockwiseLayer:
@@ -141,15 +141,15 @@
             starting_layout.to_typetracer(forget_length=True),
             behavior=self._behavior,
         )
         form = new_meta.layout.form
 
         set_form_keys(form, key=self.name)
 
-        new_meta_labelled, report = ak._nplikes.typetracer.typetracer_with_report(form)
+        new_meta_labelled, report = ak.typetracer.typetracer_with_report(form)
         new_meta_array = ak.Array(new_meta_labelled, behavior=self._behavior)
         new_input_layer = AwkwardInputLayer(
             name=self.name,
             columns=self.columns,
             inputs=[None][: int(list(self.numblocks.values())[0][0])],
             io_func=lambda *_, **__: new_meta_array,
             label=self.label,
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     from_awkward,
     from_dask_array,
     from_delayed,
     from_lists,
     from_map,
     to_dask_array,
     to_dask_bag,
+    to_dataframe,
     to_delayed,
 )
 from dask_awkward.lib.io.json import from_json, to_json
 from dask_awkward.lib.io.parquet import from_parquet, to_parquet
 from dask_awkward.lib.operations import concatenate
 from dask_awkward.lib.reducers import (
     all,
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/core.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,16 +677,17 @@
             return self._meta.layout.form
         raise ValueError("This collection's meta is None; unknown form.")
 
     @property
     def type(self) -> ArrayType:
         """awkward Array type associated with the eventual computed result."""
         t = ak.types.ArrayType(
-            self._meta._layout.form.type_from_behavior(self._meta._behavior),
+            self._meta._layout.form.type,
             0,
+            behavior=self._meta._behavior,
         )
         t._length = "??"
         return t
 
     @cached_property
     def keys_array(self) -> np.ndarray:
         """NumPy array of task graph keys."""
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/structure.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/testutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,24 +109,38 @@
     assert ares == bres
 
 
 def make_xy_point() -> dict[str, int]:
     return {"x": _RG.randint(0, 10), "y": _RG.randint(0, 10)}
 
 
+def make_xy_point_str() -> dict[str, str]:
+    return {"x": str(_RG.randint(0, 10)), "y": str(_RG.randint(0, 10))}
+
+
 def list_of_xy_points(n: int) -> list[dict[str, int]]:
     return [make_xy_point() for _ in range(n)]
 
 
+def list_of_xy_points_str(n: int) -> list[dict[str, str]]:
+    return [make_xy_point_str() for _ in range(n)]
+
+
 def awkward_xy_points(lengths: tuple[int, ...] | None = None) -> ak.Array:
     if lengths is None:
         lengths = (3, 0, 2, 1, 3)
     return ak.Array([list_of_xy_points(n) for n in lengths])
 
 
+def awkward_xy_points_str(lengths: tuple[int, ...] | None = None) -> ak.Array:
+    if lengths is None:
+        lengths = (3, 0, 2, 1, 3)
+    return ak.Array([list_of_xy_points_str(n) for n in lengths])
+
+
 def list1() -> list:
     return [
         [{"x": 1.0, "y": 1.1}, {"x": 2.0, "y": 2.2}, {"x": 3, "y": 3.3}],
         [],
         [{"x": 4.0, "y": 4.4}, {"x": 5.0, "y": 5.5}],
         [{"x": 6.0, "y": 6.6}],
         [{"x": 7.0, "y": 7.7}, {"x": 8.0, "y": 8.8}, {"x": 9, "y": 9.9}],
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/io/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     new_array_object,
     typetracer_array,
 )
 
 if TYPE_CHECKING:
     from dask.array.core import Array as DaskArray
     from dask.bag.core import Bag as DaskBag
+    from dask.dataframe.core import DataFrame as DaskDataFrame
     from dask.delayed import Delayed
 
     from dask_awkward.lib.core import Array
 
 
 class ImplementsFormTransformation(Protocol):
     behavior: dict | None
@@ -56,15 +57,15 @@
 
 def from_awkward(
     source: ak.Array,
     npartitions: int,
     behavior: dict | None = None,
     label: str | None = None,
 ) -> Array:
-    """Create a Dask collection from a concrete awkward array.
+    """Create an Array collection from a concrete :class:`awkward.Array` object.
 
     Parameters
     ----------
     source : ak.Array
         The concrete awkward array.
     npartitions : int
         The total number of partitions for the collection.
@@ -109,15 +110,15 @@
         self.behavior = behavior
 
     def __call__(self, x, **kwargs):
         return ak.Array(x, behavior=self.behavior)
 
 
 def from_lists(source: list[list[Any]], behavior: dict | None = None) -> Array:
-    """Create a Dask collection from a list of lists.
+    """Create an Array collection from a list of lists.
 
     Parameters
     ----------
     source : list[list[Any]]
         List of lists, each outer list will become a partition in the
         collection.
 
@@ -152,15 +153,15 @@
 def from_delayed(
     source: list[Delayed] | Delayed,
     meta: ak.Array | None = None,
     behavior: dict | None = None,
     divisions: tuple[int | None, ...] | None = None,
     prefix: str = "from-delayed",
 ) -> Array:
-    """Create a Dask Awkward Array from Dask Delayed objects.
+    """Create an Array collection from a set of :class:`~dask.delayed.Delayed` objects.
 
     Parameters
     ----------
     source : list[dask.delayed.Delayed] | dask.delayed.Delayed
         List of :py:class:`~dask.delayed.Delayed` objects (or a single
         object). Each Delayed object represents a single partition in
         the resulting awkward array.
@@ -193,15 +194,15 @@
     hlg = HighLevelGraph.from_collections(name, dsk, dependencies=parts)
     return new_array_object(
         hlg, name=name, meta=meta, behavior=behavior, divisions=divs
     )
 
 
 def to_delayed(array: Array, optimize_graph: bool = True) -> list[Delayed]:
-    """Convert the collection to a list of delayed objects.
+    """Convert Arrray the collection to a list of :class:`~dask.delayed.Delayed` objects.
 
     One dask.delayed.Delayed object per partition.
 
     Parameters
     ----------
     optimize_graph : bool
         If ``True`` the task graph associated with the collection will
@@ -222,26 +223,27 @@
         graph = array.__dask_optimize__(graph, keys)
         layer = f"delayed-{array.name}"
         graph = HighLevelGraph.from_collections(layer, graph, dependencies=())
     return [Delayed(k, graph, layer=layer) for k in keys]
 
 
 def to_dask_bag(array: Array) -> DaskBag:
+    """Convert Array collection to a :class:`dask.bag.Bag` collection."""
     from dask.bag.core import Bag
 
     return Bag(array.dask, array.name, array.npartitions)
 
 
 def to_dask_array(
     array: Array,
     *,
     dtype: Any = None,
     optimize_graph: bool = True,
 ) -> DaskArray:
-    """Convert awkward array collection to a Dask array collection.
+    """Convert Array collection to a :class:`dask.array.Array` collection.
 
     This conversion requires the awkward array to have a rectilinear
     shape (that is, no lists of variable length lists).
 
     Parameters
     ----------
     array : Array
@@ -366,14 +368,58 @@
             hlg, name, npartitions=array.npartitions, meta=meta, behavior=behavior
         )
     else:
         divs = (0, *np.cumsum(array.chunks))
         return new_array_object(hlg, name, divisions=divs, meta=meta, behavior=behavior)
 
 
+def to_dataframe(
+    array,
+    optimize_graph: bool = True,
+    **kwargs: Any,
+) -> DaskDataFrame:
+    """Convert :class:`dask_awkward.Array` collection to :class:`~dask.dataframe.DataFrame`.
+
+    Parameters
+    ----------
+    array : dask_awkward.Array
+        Array collection to be converted.
+    optimize_graph : bool
+        If ``True``, optimize the Array collection task graph before
+        converting to DataFrame collection.
+    **kwargs : Any
+        Additional arguments passed to :func:`ak.to_dataframe`.
+
+    Returns
+    -------
+    dask.dataframe.DataFrame
+        Resulting DataFrame collection.
+
+    """
+    import dask
+    from dask.dataframe.core import new_dd_object
+
+    if optimize_graph:
+        (array,) = dask.optimize(array)
+    intermediate = map_partitions(
+        ak.to_dataframe,
+        array,
+        meta=empty_typetracer(),
+        label="to-dataframe",
+        **kwargs,
+    )
+    meta = ak.to_dataframe(array._meta.layout.form.length_zero_array(), **kwargs)
+    return new_dd_object(
+        intermediate.dask,
+        intermediate.name,
+        meta,
+        intermediate.divisions,
+    )
+
+
 class PackedArgCallable:
     """Wrap a callable such that packed arguments can be unrolled.
 
     Inspired by dask.dataframe.io.io._PackedArgCallable.
 
     """
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/io/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,14 +449,15 @@
     path: str,
     line_delimited: bool = True,
     storage_options: dict[str, Any] | None = None,
     compute: bool = False,
     compression: str | None = "infer",
     **kwargs: Any,
 ) -> Scalar:
+    """Write data to line delimited JSON."""
     storage_options = storage_options or {}
     fs, _ = url_to_fs(path, **storage_options)
     nparts = array.npartitions
     map_res = map_partitions(
         _ToJsonFn(
             fs,
             path,
```

### Comparing `dask_awkward-2023.5.1/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.6.0/src/dask_awkward/lib/io/parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     storage_options: dict | None = None,
     ignore_metadata: bool = True,
     scan_files: bool = False,
     columns: Sequence[str] | None = None,
     filters: Any | None = None,
     split_row_groups: Any | None = None,
 ) -> Array:
-    """Read parquet dataset into an :py:obj:`~dask_awkward.Array` collection.
+    """Create an Array collection from a Parquet dataset.
 
     Parameters
     ----------
     url : str
         Location of data, including protocol (e.g. ``s3://``)
     storage_options : dict
         For creating filesystem (see ``fsspec`` documentation).
@@ -422,15 +422,15 @@
     data: Array,
     path: Any,
     storage_options: dict[str, Any] | None = None,
     write_metadata: bool = False,
     compute: bool = True,
     prefix: str | None = None,
 ) -> Scalar | None:
-    """Write data to parquet format.
+    """Write data to Parquet format.
 
     Parameters
     ----------
     data : dask_awkward.Array
         Array to write to parquet.
     path : str
         Root directory of location to write to
```

### Comparing `dask_awkward-2023.5.1/.gitignore` & `dask_awkward-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/LICENSE` & `dask_awkward-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/README.md` & `dask_awkward-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.5.1/pyproject.toml` & `dask_awkward-2023.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-  "awkward >=2.2.0",
+  "awkward >=2.2.1",
   "dask >=2023.04.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-awkward"
 "Bug Tracker" = "https://github.com/dask-contrib/dask-awkward/issues"
```

### Comparing `dask_awkward-2023.5.1/PKG-INFO` & `dask_awkward-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.5.1
+Version: 2023.6.0
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Requires-Dist: awkward>=2.2.0
+Requires-Dist: awkward>=2.2.1
 Requires-Dist: dask>=2023.04.0
 Provides-Extra: complete
 Requires-Dist: aiohttp; extra == 'complete'
 Requires-Dist: pyarrow; extra == 'complete'
 Requires-Dist: pytest-cov>=3.0.0; extra == 'complete'
 Requires-Dist: pytest>=6.0; extra == 'complete'
 Requires-Dist: requests>=2.27.1; extra == 'complete'
```

