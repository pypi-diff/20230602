# Comparing `tmp/ngff_zarr-0.4.2.tar.gz` & `tmp/ngff_zarr-0.4.3.tar.gz`

## Comparing `ngff_zarr-0.4.2.tar` & `ngff_zarr-0.4.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/__about__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/__init__.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/_array_split.py
--rwxr-xr-x   0        0        0    10945 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/cli.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/config.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/detect_cli_io_backend.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/from_ngff_zarr.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/memory_usage.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/multiscales.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/ngff_image.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/ngff_image_to_itk_image.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/rich_dask_progress.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/task_count.py
--rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/to_multiscales.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/to_ngff_image.py
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/to_ngff_zarr.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/zarr_metadata.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/methods/__init__.py
--rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/methods/_dask_image.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/methods/_itk.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/ngff_zarr/methods/_support.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/__init__.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/_data.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_detect_cli_input_backend.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_from_ngff_zarr.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_large_serialization.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_memory_usage.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_ngff_image_scale_factors.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_ngff_image_to_itk_image.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_task_count.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_to_ngff_zarr_dask_image.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/test_to_ngff_zarr_itk.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/README.md
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 ngff_zarr-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/README.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/__about__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/__init__.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/_array_split.py
+-rwxr-xr-x   0        0        0    10945 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/cli.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/config.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/detect_cli_io_backend.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/from_ngff_zarr.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/memory_usage.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/multiscales.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/ngff_image.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/rich_dask_progress.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/task_count.py
+-rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/to_multiscales.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/to_ngff_image.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/to_ngff_zarr.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/zarr_metadata.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/methods/__init__.py
+-rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/methods/_dask_image.py
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/methods/_itk.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/ngff_zarr/methods/_support.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/__init__.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/_data.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_detect_cli_input_backend.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_from_ngff_zarr.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_large_serialization.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_memory_usage.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_ngff_image_scale_factors.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_task_count.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_to_ngff_zarr_dask_image.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/test_to_ngff_zarr_itk.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 ngff_zarr-0.4.3/PKG-INFO
```

### Comparing `ngff_zarr-0.4.2/.github/workflows/test.yml` & `ngff_zarr-0.4.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/.pytest_cache/v/cache/nodeids` & `ngff_zarr-0.4.3/.pytest_cache/v/cache/nodeids`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {'insert': "[(29, 'test/test_to_ngff_zarr_itk.py::test_three_scales')]"}*

```diff
@@ -23,9 +23,10 @@
     "test/test_ngff_image_to_itk_image.py::test_2d_itkwasm_image",
     "test/test_ngff_image_to_itk_image.py::test_2d_rgb_itk_image",
     "test/test_ngff_image_to_itk_image.py::test_3d_itk_image",
     "test/test_ngff_image_to_itk_image.py::test_3d_itk_vector_image",
     "test/test_task_count.py::test_memory_usage",
     "test/test_to_ngff_zarr_dask_image.py::test_gaussian_isotropic_scale_factors",
     "test/test_to_ngff_zarr_itk.py::test_bin_shrink_isotropic_scale_factors",
-    "test/test_to_ngff_zarr_itk.py::test_gaussian_isotropic_scale_factors"
+    "test/test_to_ngff_zarr_itk.py::test_gaussian_isotropic_scale_factors",
+    "test/test_to_ngff_zarr_itk.py::test_three_scales"
 ]
```

### Comparing `ngff_zarr-0.4.2/ngff_zarr/__init__.py` & `ngff_zarr-0.4.3/ngff_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/_array_split.py` & `ngff_zarr-0.4.3/ngff_zarr/_array_split.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/cli.py` & `ngff_zarr-0.4.3/ngff_zarr/cli.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/cli_input_to_ngff_image.py` & `ngff_zarr-0.4.3/ngff_zarr/cli_input_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/config.py` & `ngff_zarr-0.4.3/ngff_zarr/config.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/detect_cli_io_backend.py` & `ngff_zarr-0.4.3/ngff_zarr/detect_cli_io_backend.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/from_ngff_zarr.py` & `ngff_zarr-0.4.3/ngff_zarr/from_ngff_zarr.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/itk_image_to_ngff_image.py` & `ngff_zarr-0.4.3/ngff_zarr/itk_image_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/memory_usage.py` & `ngff_zarr-0.4.3/ngff_zarr/memory_usage.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/multiscales.py` & `ngff_zarr-0.4.3/ngff_zarr/multiscales.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/ngff_image_to_itk_image.py` & `ngff_zarr-0.4.3/ngff_zarr/ngff_image_to_itk_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/rich_dask_progress.py` & `ngff_zarr-0.4.3/ngff_zarr/rich_dask_progress.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/to_multiscales.py` & `ngff_zarr-0.4.3/ngff_zarr/to_multiscales.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/to_ngff_image.py` & `ngff_zarr-0.4.3/ngff_zarr/to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/to_ngff_zarr.py` & `ngff_zarr-0.4.3/ngff_zarr/to_ngff_zarr.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             progress.update_multiscales_task_completed((index+1))
         image = next_image
         arr = image.data
         path = multiscales.metadata.datasets[index].path
         array_dims_group = root.create_group(str(PurePosixPath(path).parent))
         array_dims_group.attrs["_ARRAY_DIMENSIONS"] = image.dims
 
-        if index < nscales - 1:
+        if index > 0 and index < nscales - 1:
             dim_factors = _dim_scale_factors(dims, multiscales.scale_factors[index], previous_dim_factors)
         else:
             dim_factors = { d: 1 for d in dims }
         previous_dim_factors = dim_factors
 
         if memory_usage(image) > config.memory_target:
             shrink_factors = []
@@ -102,15 +102,14 @@
             shape = image.data.shape
             x_index = dims.index('x')
             y_index = dims.index('y')
             if 'z' in dims:
                 z_index = dims.index('z')
                 # TODO address, c, t, large 2D
                 slice_bytes = memory_usage(image, {'z'})
-                scale_factors = multiscales.scale_factors
                 slab_slices = min(int(np.ceil(config.memory_target / slice_bytes)), arr.shape[z_index])
                 z_chunks = chunks[z_index]
                 slice_planes = False
                 if slab_slices < z_chunks:
                     slab_slices = z_chunks
                     slice_planes = True
                 if slab_slices > arr.shape[z_index]:
@@ -194,24 +193,25 @@
                 overwrite=False,
                 compute=True,
                 return_stored=False,
                 **kwargs,
             )
 
         # Minimize task graph depth
-        if index < nscales - 2 and multiscales.scale_factors and multiscales.method and multiscales.chunks:
+        if index > 1 and index < nscales - 2 and multiscales.scale_factors and multiscales.method and multiscales.chunks:
             image.data = dask.array.from_zarr(store, component=path)
-            next_multiscales_factor = multiscales.scale_factors[index+1]
+            next_multiscales_factor = multiscales.scale_factors[index]
             if isinstance(next_multiscales_factor, int):
-                next_multiscales_factor = next_multiscales_factor // multiscales.scale_factors[index]
+                next_multiscales_factor = next_multiscales_factor // multiscales.scale_factors[index-1]
             else:
                 updated_factors = {}
                 for d, f in next_multiscales_factor.items():
-                    updated_factors[d] = f // multiscales.scale_factors[index][d]
+                    updated_factors[d] = f // multiscales.scale_factors[index-1][d]
                 next_multiscales_factor = updated_factors
+
             next_multiscales = to_multiscales(image,
                 scale_factors=[next_multiscales_factor,],
                 method=multiscales.method,
                 chunks=multiscales.chunks,
                 progress=progress,
                 cache=False)
             multiscales.images[index+1] = next_multiscales.images[1]
```

### Comparing `ngff_zarr-0.4.2/ngff_zarr/zarr_metadata.py` & `ngff_zarr-0.4.3/ngff_zarr/zarr_metadata.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/methods/_dask_image.py` & `ngff_zarr-0.4.3/ngff_zarr/methods/_dask_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/methods/_itk.py` & `ngff_zarr-0.4.3/ngff_zarr/methods/_itk.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/ngff_zarr/methods/_support.py` & `ngff_zarr-0.4.3/ngff_zarr/methods/_support.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/_data.py` & `ngff_zarr-0.4.3/test/_data.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_cli_input_to_ngff_image.py` & `ngff_zarr-0.4.3/test/test_cli_input_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_detect_cli_input_backend.py` & `ngff_zarr-0.4.3/test/test_detect_cli_input_backend.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_from_ngff_zarr.py` & `ngff_zarr-0.4.3/test/test_from_ngff_zarr.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_itk_image_to_ngff_image.py` & `ngff_zarr-0.4.3/test/test_itk_image_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_large_serialization.py` & `ngff_zarr-0.4.3/test/test_large_serialization.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_memory_usage.py` & `ngff_zarr-0.4.3/test/test_memory_usage.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_ngff_image_scale_factors.py` & `ngff_zarr-0.4.3/test/test_ngff_image_scale_factors.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_ngff_image_to_itk_image.py` & `ngff_zarr-0.4.3/test/test_ngff_image_to_itk_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_task_count.py` & `ngff_zarr-0.4.3/test/test_task_count.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_to_ngff_zarr_dask_image.py` & `ngff_zarr-0.4.3/test/test_to_ngff_zarr_dask_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/test_to_ngff_zarr_itk.py` & `ngff_zarr-0.4.3/test/test_to_ngff_zarr_itk.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/test/.pytest_cache/v/cache/nodeids` & `ngff_zarr-0.4.3/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/LICENSE.txt` & `ngff_zarr-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/README.md` & `ngff_zarr-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/pyproject.toml` & `ngff_zarr-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.2/PKG-INFO` & `ngff_zarr-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngff-zarr
-Version: 0.4.2
+Version: 0.4.3
 Project-URL: Documentation, https://github.com/thewtex/ngff-zarr#readme
 Project-URL: Issues, https://github.com/thewtex/ngff-zarr/issues
 Project-URL: Source, https://github.com/thewtex/ngff-zarr
 Author-email: Matt McCormick <matt.mccormick@kitware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

