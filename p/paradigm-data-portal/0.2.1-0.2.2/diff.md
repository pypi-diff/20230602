# Comparing `tmp/paradigm-data-portal-0.2.1.tar.gz` & `tmp/paradigm-data-portal-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradigm-data-portal-0.2.1.tar", last modified: Fri Mar 17 23:31:18 2023, max compression
+gzip compressed data, was "paradigm-data-portal-0.2.2.tar", last modified: Fri Jun  2 04:00:56 2023, max compression
```

## Comparing `paradigm-data-portal-0.2.1.tar` & `paradigm-data-portal-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,61 @@
--rw-r--r--   0        0        0      244 2023-03-17 08:49:09.231499 paradigm-data-portal-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2023-03-08 19:50:45.125865 paradigm-data-portal-0.2.1/LICENSE-APACHE
--rw-r--r--   0        0        0     1075 2023-03-08 19:51:00.041345 paradigm-data-portal-0.2.1/LICENSE-MIT
--rw-r--r--   0        0        0     1545 2023-03-16 21:51:43.306856 paradigm-data-portal-0.2.1/README.md
--rw-r--r--   0        0        0      549 2023-03-16 20:07:28.066076 paradigm-data-portal-0.2.1/datasets/README.md
--rw-r--r--   0        0        0     7048 2023-03-16 21:39:43.273487 paradigm-data-portal-0.2.1/datasets/ethereum_contracts/LICENSE-CC0
--rw-r--r--   0        0        0     5207 2023-03-17 16:12:10.042638 paradigm-data-portal-0.2.1/datasets/ethereum_contracts/README.md
--rw-r--r--   0        0        0     5817 2023-03-17 16:12:10.032686 paradigm-data-portal-0.2.1/datasets/ethereum_contracts/dataset_manifest.json
--rw-r--r--   0        0        0     7048 2023-03-16 21:40:09.489070 paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/LICENSE-CC0
--rw-r--r--   0        0        0    19670 2023-03-17 16:11:57.836357 paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/README.md
--rw-r--r--   0        0        0    18479 2023-03-17 16:11:57.814463 paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/dataset_manifest.json
--rw-r--r--   0        0        0     7048 2023-03-17 04:16:21.139079 paradigm-data-portal-0.2.1/datasets/ethereum_slots/LICENSE-CC0
--rw-r--r--   0        0        0     4113 2023-03-17 16:12:03.285570 paradigm-data-portal-0.2.1/datasets/ethereum_slots/README.md
--rw-r--r--   0        0        0     4610 2023-03-17 16:12:03.277000 paradigm-data-portal-0.2.1/datasets/ethereum_slots/dataset_manifest.json
--rw-r--r--   0        0        0     7791 2023-03-17 15:53:41.108997 paradigm-data-portal-0.2.1/datasets/global_manifest.json
--rw-r--r--   0        0        0    74507 2023-03-17 08:46:47.847219 paradigm-data-portal-0.2.1/notebooks/explore_ethereum_contracts.ipynb
--rw-r--r--   0        0        0      251 2023-03-17 23:30:59.686834 paradigm-data-portal-0.2.1/pdp/__init__.py
--rw-r--r--   0        0        0       87 2023-03-09 00:09:52.258280 paradigm-data-portal-0.2.1/pdp/__main__.py
--rw-r--r--   0        0        0     1351 2023-03-17 05:23:27.122651 paradigm-data-portal-0.2.1/pdp/cli/cli_run.py
--rw-r--r--   0        0        0        0 2023-03-08 18:45:38.780173 paradigm-data-portal-0.2.1/pdp/cli/commands/__init__.py
--rw-r--r--   0        0        0     1152 2023-03-15 23:22:13.689945 paradigm-data-portal-0.2.1/pdp/cli/commands/dataset_command.py
--rw-r--r--   0        0        0      898 2023-03-14 01:15:16.630188 paradigm-data-portal-0.2.1/pdp/cli/commands/download_command.py
--rw-r--r--   0        0        0     1584 2023-03-17 07:04:37.983236 paradigm-data-portal-0.2.1/pdp/cli/commands/generate_command.py
--rw-r--r--   0        0        0     2934 2023-03-14 05:43:32.363332 paradigm-data-portal-0.2.1/pdp/cli/commands/ls_command.py
--rw-r--r--   0        0        0     2969 2023-03-17 05:35:31.644693 paradigm-data-portal-0.2.1/pdp/cli/commands/package_command.py
--rw-r--r--   0        0        0      473 2023-03-14 02:52:34.383089 paradigm-data-portal-0.2.1/pdp/cli/commands/root_command.py
--rw-r--r--   0        0        0     3746 2023-03-14 02:00:55.599955 paradigm-data-portal-0.2.1/pdp/cli/commands/upload_command.py
--rw-r--r--   0        0        0      990 2023-03-17 05:29:38.016173 paradigm-data-portal-0.2.1/pdp/cli/commands/validate_command.py
--rw-r--r--   0        0        0     5812 2023-03-17 16:19:52.709467 paradigm-data-portal-0.2.1/pdp/dataset_utils.py
--rw-r--r--   0        0        0       31 2023-03-16 17:37:37.175652 paradigm-data-portal-0.2.1/pdp/generate/__init__.py
--rwxr-xr-x   0        0        0      571 2023-03-16 01:21:30.476860 paradigm-data-portal-0.2.1/pdp/generate/generate_contracts_dataset.py
--rwxr-xr-x   0        0        0      598 2023-03-16 17:38:57.476086 paradigm-data-portal-0.2.1/pdp/generate/generate_native_transfers_dataset.py
--rwxr-xr-x   0        0        0      538 2023-03-16 03:28:23.628925 paradigm-data-portal-0.2.1/pdp/generate/generate_slots_dataset.py
--rw-r--r--   0        0        0      641 2023-03-16 17:40:30.384651 paradigm-data-portal-0.2.1/pdp/generate/generate_utils.py
--rw-r--r--   0        0        0     2897 2023-03-14 23:51:33.642439 paradigm-data-portal-0.2.1/pdp/io_utils.py
--rw-r--r--   0        0        0     8032 2023-03-17 05:39:00.207017 paradigm-data-portal-0.2.1/pdp/package_utils.py
--rw-r--r--   0        0        0     4846 2023-03-17 16:11:50.555223 paradigm-data-portal-0.2.1/pdp/readme_utils.py
--rw-r--r--   0        0        0     6908 2023-03-17 05:37:32.895709 paradigm-data-portal-0.2.1/pdp/spec.py
--rw-r--r--   0        0        0     1285 2023-03-17 23:29:48.137498 paradigm-data-portal-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2680 1970-01-01 00:00:00.000000 paradigm-data-portal-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      282 2023-03-27 23:35:34.357922 paradigm-data-portal-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2023-03-08 19:50:45.125865 paradigm-data-portal-0.2.2/LICENSE-APACHE
+-rw-r--r--   0        0        0     1075 2023-03-08 19:51:00.041345 paradigm-data-portal-0.2.2/LICENSE-MIT
+-rw-r--r--   0        0        0     1545 2023-04-28 21:47:53.737941 paradigm-data-portal-0.2.2/README.md
+-rw-r--r--   0        0        0      549 2023-03-16 20:07:28.066076 paradigm-data-portal-0.2.2/datasets/README.md
+-rw-r--r--   0        0        0     7048 2023-03-16 21:39:43.273487 paradigm-data-portal-0.2.2/datasets/ethereum_contracts/LICENSE-CC0
+-rw-r--r--   0        0        0     5208 2023-04-28 16:54:32.288423 paradigm-data-portal-0.2.2/datasets/ethereum_contracts/README.md
+-rw-r--r--   0        0        0     5817 2023-03-17 16:12:10.032686 paradigm-data-portal-0.2.2/datasets/ethereum_contracts/dataset_manifest.json
+-rw-r--r--   0        0        0     7048 2023-03-16 21:40:09.489070 paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/LICENSE-CC0
+-rw-r--r--   0        0        0    19678 2023-04-28 16:55:18.485014 paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/README.md
+-rw-r--r--   0        0        0    18479 2023-03-17 16:11:57.814463 paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/dataset_manifest.json
+-rw-r--r--   0        0        0     7048 2023-03-17 04:16:21.139079 paradigm-data-portal-0.2.2/datasets/ethereum_slots/LICENSE-CC0
+-rw-r--r--   0        0        0     4110 2023-04-28 16:55:40.554177 paradigm-data-portal-0.2.2/datasets/ethereum_slots/README.md
+-rw-r--r--   0        0        0     4610 2023-03-17 16:12:03.277000 paradigm-data-portal-0.2.2/datasets/ethereum_slots/dataset_manifest.json
+-rw-r--r--   0        0        0     7791 2023-03-17 15:53:41.108997 paradigm-data-portal-0.2.2/datasets/global_manifest.json
+-rw-r--r--   0        0        0    74507 2023-03-17 08:46:47.847219 paradigm-data-portal-0.2.2/notebooks/explore_ethereum_contracts.ipynb
+-rw-r--r--   0        0        0      171 2023-06-02 04:00:02.670168 paradigm-data-portal-0.2.2/pdp/__init__.py
+-rw-r--r--   0        0        0       87 2023-03-09 00:09:52.258280 paradigm-data-portal-0.2.2/pdp/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-28 05:16:58.901457 paradigm-data-portal-0.2.2/pdp/cli/__init__.py
+-rw-r--r--   0        0        0     2627 2023-05-31 22:39:18.067537 paradigm-data-portal-0.2.2/pdp/cli/cli_run.py
+-rw-r--r--   0        0        0        0 2023-03-08 18:45:38.780173 paradigm-data-portal-0.2.2/pdp/cli/commands/__init__.py
+-rw-r--r--   0        0        0     5685 2023-05-31 22:27:56.294360 paradigm-data-portal-0.2.2/pdp/cli/commands/collect_command.py
+-rw-r--r--   0        0        0     2134 2023-05-04 23:37:05.830703 paradigm-data-portal-0.2.2/pdp/cli/commands/dataset_command.py
+-rw-r--r--   0        0        0      921 2023-05-07 20:59:14.948229 paradigm-data-portal-0.2.2/pdp/cli/commands/download_command.py
+-rw-r--r--   0        0        0     2934 2023-03-14 05:43:32.363332 paradigm-data-portal-0.2.2/pdp/cli/commands/ls_command.py
+-rw-r--r--   0        0        0     2965 2023-04-28 16:48:51.331426 paradigm-data-portal-0.2.2/pdp/cli/commands/package_command.py
+-rw-r--r--   0        0        0      473 2023-03-14 02:52:34.383089 paradigm-data-portal-0.2.2/pdp/cli/commands/root_command.py
+-rw-r--r--   0        0        0     1241 2023-06-02 03:57:28.860511 paradigm-data-portal-0.2.2/pdp/cli/commands/update_command.py
+-rw-r--r--   0        0        0     3746 2023-03-14 02:00:55.599955 paradigm-data-portal-0.2.2/pdp/cli/commands/upload_command.py
+-rw-r--r--   0        0        0      990 2023-03-17 05:29:38.016173 paradigm-data-portal-0.2.2/pdp/cli/commands/validate_command.py
+-rw-r--r--   0        0        0     2036 2023-05-03 00:22:06.781751 paradigm-data-portal-0.2.2/pdp/config_utils.py
+-rw-r--r--   0        0        0      253 2023-05-31 22:38:31.753008 paradigm-data-portal-0.2.2/pdp/data_utils/__init__.py
+-rw-r--r--   0        0        0      276 2023-05-04 22:49:38.476761 paradigm-data-portal-0.2.2/pdp/data_utils/collect_utils.py
+-rw-r--r--   0        0        0     4317 2023-04-28 05:08:02.938101 paradigm-data-portal-0.2.2/pdp/data_utils/download_utils.py
+-rw-r--r--   0        0        0     3097 2023-06-02 00:23:40.871683 paradigm-data-portal-0.2.2/pdp/data_utils/file_utils.py
+-rw-r--r--   0        0        0     6956 2023-06-02 03:48:17.214693 paradigm-data-portal-0.2.2/pdp/data_utils/job_utils.py
+-rw-r--r--   0        0        0    10716 2023-05-04 23:44:33.463380 paradigm-data-portal-0.2.2/pdp/data_utils/manifest_utils.py
+-rw-r--r--   0        0        0     5841 2023-05-03 00:22:16.498513 paradigm-data-portal-0.2.2/pdp/data_utils/query_utils.py
+-rw-r--r--   0        0        0     4910 2023-04-28 16:57:04.812540 paradigm-data-portal-0.2.2/pdp/data_utils/readme_utils.py
+-rw-r--r--   0        0        0     2833 2023-04-28 05:51:33.760891 paradigm-data-portal-0.2.2/pdp/data_utils/schema_utils.py
+-rw-r--r--   0        0        0      197 2023-06-02 03:58:21.270880 paradigm-data-portal-0.2.2/pdp/data_utils/update_utils.py
+-rw-r--r--   0        0        0        0 2023-03-27 23:49:38.453027 paradigm-data-portal-0.2.2/pdp/datasets/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-28 16:55:59.674895 paradigm-data-portal-0.2.2/pdp/datasets/contracts/__init__.py
+-rw-r--r--   0        0        0     2778 2023-06-02 03:54:45.285099 paradigm-data-portal-0.2.2/pdp/datasets/contracts/contracts_collect.py
+-rw-r--r--   0        0        0     3206 2023-04-28 05:15:12.844847 paradigm-data-portal-0.2.2/pdp/datasets/contracts/contracts_queries.py
+-rw-r--r--   0        0        0     3357 2023-04-08 04:13:54.423100 paradigm-data-portal-0.2.2/pdp/datasets/contracts/contracts_spec.py
+-rw-r--r--   0        0        0      117 2023-04-28 16:54:42.432282 paradigm-data-portal-0.2.2/pdp/datasets/native_transfers/__init__.py
+-rw-r--r--   0        0        0     3242 2023-06-02 03:55:18.534143 paradigm-data-portal-0.2.2/pdp/datasets/native_transfers/native_transfers_collect.py
+-rw-r--r--   0        0        0     1929 2023-04-28 05:14:30.584341 paradigm-data-portal-0.2.2/pdp/datasets/native_transfers/native_transfers_queries.py
+-rw-r--r--   0        0        0     1851 2023-03-28 06:51:04.338319 paradigm-data-portal-0.2.2/pdp/datasets/native_transfers/native_transfers_spec.py
+-rw-r--r--   0        0        0       84 2023-04-28 16:55:49.515864 paradigm-data-portal-0.2.2/pdp/datasets/slots/__init__.py
+-rw-r--r--   0        0        0     2665 2023-06-02 03:53:49.212144 paradigm-data-portal-0.2.2/pdp/datasets/slots/slots_collect.py
+-rw-r--r--   0        0        0     2429 2023-05-08 01:18:22.786719 paradigm-data-portal-0.2.2/pdp/datasets/slots/slots_queries.py
+-rw-r--r--   0        0        0     1953 2023-04-09 03:58:28.452294 paradigm-data-portal-0.2.2/pdp/datasets/slots/slots_spec.py
+-rw-r--r--   0        0        0        0 2023-04-28 05:36:09.946322 paradigm-data-portal-0.2.2/pdp/py.typed
+-rw-r--r--   0        0        0     3332 2023-05-04 23:42:26.718905 paradigm-data-portal-0.2.2/pdp/spec.py
+-rw-r--r--   0        0        0     1519 2023-06-02 03:59:29.917646 paradigm-data-portal-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      373 2023-05-02 23:57:57.819917 paradigm-data-portal-0.2.2/tests/remote_tests/test_manifests.py
+-rw-r--r--   0        0        0     1152 2023-05-02 23:05:21.484472 paradigm-data-portal-0.2.2/tests/test_collect.py
+-rw-r--r--   0        0        0      475 2023-05-03 00:25:12.132049 paradigm-data-portal-0.2.2/tests/test_validate.py
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 paradigm-data-portal-0.2.2/PKG-INFO
```

### Comparing `paradigm-data-portal-0.2.1/LICENSE-APACHE` & `paradigm-data-portal-0.2.2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/LICENSE-MIT` & `paradigm-data-portal-0.2.2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/README.md` & `paradigm-data-portal-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/README.md` & `paradigm-data-portal-0.2.2/datasets/README.md`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_contracts/LICENSE-CC0` & `paradigm-data-portal-0.2.2/datasets/ethereum_contracts/LICENSE-CC0`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_contracts/README.md` & `paradigm-data-portal-0.2.2/datasets/ethereum_contracts/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Ethereum Contracts Dataset v1.0.0
 
 This is a dataset of all historical contract deployments
 
-The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/generate/generate_contracts_dataset.py)
+The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/datasets/contracts/contracts_collect.py)
 
 Data is distributed as [parquet](https://data.paradigm.xyz/about) files and released into the public domain under a [CC0 license](https://creativecommons.org/share-your-work/public-domain/cc0/)
 
 ## Usage
 
 Some example uses of this dataset include:
 - look up all contracts deployed by an address
```

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_contracts/dataset_manifest.json` & `paradigm-data-portal-0.2.2/datasets/ethereum_contracts/dataset_manifest.json`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/LICENSE-CC0` & `paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/LICENSE-CC0`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/README.md` & `paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Ethereum Native Transfers Dataset v1.0.0
 
 This is a dataset of all native transfers in similar format to ERC20 Transfers (excluding tx fees)
 
-The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/generate/generate_native_transfers_dataset.py)
+The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/datasets/native_transfers/native_transfers_collect.py)
 
 Data is distributed as [parquet](https://data.paradigm.xyz/about) files and released into the public domain under a [CC0 license](https://creativecommons.org/share-your-work/public-domain/cc0/)
 
 ## Usage
 
 Some example uses of this dataset include:
 - look up all inbound transfers to an address
```

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_native_transfers/dataset_manifest.json` & `paradigm-data-portal-0.2.2/datasets/ethereum_native_transfers/dataset_manifest.json`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_slots/LICENSE-CC0` & `paradigm-data-portal-0.2.2/datasets/ethereum_slots/LICENSE-CC0`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_slots/README.md` & `paradigm-data-portal-0.2.2/datasets/ethereum_slots/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # Ethereum Slots Dataset v1.0.0
 
 This is a dataset of all slots of each contract, including historical usage metadata
 
-The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/generate/generate_slots_dataset.py)
+The dataset was created by using [this script](https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/datasets/slots/slots_collect.py)
 
 Data is distributed as [parquet](https://data.paradigm.xyz/about) files and released into the public domain under a [CC0 license](https://creativecommons.org/share-your-work/public-domain/cc0/)
 
 ## Usage
 
 Some example uses of this dataset include:
 - look up how much storage space is used by a given contract
```

### Comparing `paradigm-data-portal-0.2.1/datasets/ethereum_slots/dataset_manifest.json` & `paradigm-data-portal-0.2.2/datasets/ethereum_slots/dataset_manifest.json`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/datasets/global_manifest.json` & `paradigm-data-portal-0.2.2/datasets/global_manifest.json`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/notebooks/explore_ethereum_contracts.ipynb` & `paradigm-data-portal-0.2.2/notebooks/explore_ethereum_contracts.ipynb`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/pdp/cli/commands/dataset_command.py` & `paradigm-data-portal-0.2.2/pdp/cli/commands/ls_command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,102 @@
 from __future__ import annotations
 
+import sys
+
 import toolcli
 import toolstr
 
 import pdp
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
-        'f': dataset_command,
-        'help': 'show info about a dataset',
+        'f': ls_command,
+        'help': 'list datasets or dataset files',
         'args': [
-            {'name': 'dataset', 'help': 'name of dataset'},
-        ],
-        'examples': [
-            'ethereum_contracts',
-            'ethereum_native_transfers',
+            {
+                'name': 'dataset',
+                'help': 'dataset to list info of, omit for global manifest',
+                'nargs': '?',
+            },
+            {
+                'name': '--hashes',
+                'help': 'show md5 hashes of each file',
+                'action': 'store_true',
+            },
+            {
+                'name': '--urls',
+                'help': 'show full urls of each file',
+                'action': 'store_true',
+            },
+            {'name': '--portal-root', 'help': 'root url of data portal'},
         ],
+        'examples': {
+            '': 'show all datasets',
+            'ethereum_contracts': 'show files of dataset',
+            'ethereum_contracts --hashes': 'show files of dataset with hashes',
+            'ethereum_contracts --urls': 'show urls of files in dataset',
+        },
     }
 
 
-def dataset_command(dataset: str) -> None:
-    manifest = pdp.get_dataset_manifest(dataset)
-    toolstr.print(manifest['name'], style=pdp.styles['title'])
-    toolstr.print_bullet(
-        key='description',
-        value=manifest['description'],
-        styles=pdp.styles,
-    )
-    toolstr.print_bullet(
-        key='version',
-        value=manifest['version'],
-        styles=pdp.styles,
-    )
-    toolstr.print_bullet(
-        key='n_files',
-        value=len(manifest['files']),
-        styles=pdp.styles,
-    )
-    total_size = sum(file['n_bytes'] for file in manifest['files'])
-    toolstr.print_bullet(
-        key='total_size',
-        value=toolstr.format_nbytes(total_size, decimals=1),
-        styles=pdp.styles,
-    )
+def ls_command(
+    dataset: str | None,
+    hashes: bool,
+    urls: bool,
+    portal_root: str | None,
+) -> None:
+
+    if dataset is None:
+
+        toolstr.print(
+            'fetching global manifest...', style=pdp.styles['comment'], end='\r'
+        )
+        global_manifest = pdp.get_global_manifest()
+        sys.stdout.write("\033[K")
+        toolstr.print('Datasets', style=pdp.styles['title'])
+        for dataset_name, dataset_manifest in global_manifest[
+            'datasets'
+        ].items():
+            toolstr.print_bullet(
+                key=dataset_name,
+                value=dataset_manifest['description'],
+                styles=pdp.styles,
+            )
+        print()
+        toolstr.print(
+            '(use '
+            + toolstr.add_style(
+                'pdp dataset <DATASET>', pdp.styles['description']
+            )
+            + ' for info or '
+            + toolstr.add_style('pdp ls <DATASET>', pdp.styles['description'])
+            + ' for file list)',
+            style=pdp.styles['comment'],
+        )
+
+    else:
+
+        # get dataset manifest
+        manifest = pdp.get_dataset_manifest(dataset=dataset)
+
+        # get id of each file, either filename or url
+        if urls:
+            file_ids = pdp.get_dataset_file_urls(
+                dataset=dataset,
+                portal_root=portal_root,
+                manifest=manifest,
+            )
+        else:
+            file_ids = [file['name'] for file in manifest['files']]
+
+        # print either with or without hashes
+        if hashes:
+            rows = [
+                [file_id, file['hash']]
+                for file_id, file in zip(file_ids, manifest['files'])
+            ]
+            toolstr.print_table(rows, compact=True)
+        else:
+            for file_id in file_ids:
+                print(file_id)
```

### Comparing `paradigm-data-portal-0.2.1/pdp/cli/commands/download_command.py` & `paradigm-data-portal-0.2.2/pdp/cli/commands/download_command.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pdp
 
 
 def get_command_spec() -> toolcli.CommandSpec:
     return {
         'f': download_command,
-        'help': 'download files for a dataset',
+        'help': 'download dataset directly from Paradigm data portal',
         'args': [
             {'name': 'dataset', 'help': 'dataset to list info of'},
             {'name': '--output-dir', 'help': 'output directory path'},
             {'name': '--portal-root', 'help': 'root url of data portal'},
         ],
         'examples': [
             'ethereum_contracts',
```

### Comparing `paradigm-data-portal-0.2.1/pdp/cli/commands/package_command.py` & `paradigm-data-portal-0.2.2/pdp/cli/commands/package_command.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             {
                 'name': 'directory',
                 'help': 'data directory to use for manifest',
                 'nargs': '?',
             },
             {
                 'name': '--global',
-                'help': 'generate a global manifest instead of a dataset manifest',
+                'help': 'create a global manifest instead of a dataset manifest',
                 'action': 'store_true',
                 'dest': 'global_manifest',
             },
             {
                 'name': '--output-path',
                 'help': 'output path of manifest',
             },
@@ -97,14 +97,14 @@
             readme_path = os.path.join(
                 os.path.dirname(output_path),
                 pdp.dataset_readme_filename,
             )
         else:
             raise Exception('unknown output_path type: ' + str(output_path))
 
-        # generate readme
+        # create readme
         pdp.create_dataset_readme(
             dataset_manifest=dataset_manifest,
             output_path=readme_path,
             confirm=confirm,
         )
```

### Comparing `paradigm-data-portal-0.2.1/pdp/cli/commands/upload_command.py` & `paradigm-data-portal-0.2.2/pdp/cli/commands/upload_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/pdp/cli/commands/validate_command.py` & `paradigm-data-portal-0.2.2/pdp/cli/commands/validate_command.py`

 * *Files identical despite different names*

### Comparing `paradigm-data-portal-0.2.1/pdp/dataset_utils.py` & `paradigm-data-portal-0.2.2/pdp/data_utils/download_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,18 @@
+"""functions for downloading datasets"""
+
 from __future__ import annotations
 
 import os
 import typing
 
-
-from . import io_utils
-from . import spec
-
-
-def get_global_manifest(
-    *, portal_root: str | None = None
-) -> spec.GlobalManifest:
-    """get global manifest of all datasets"""
-
-    import requests  # type: ignore
-
-    # build url
-    if portal_root is None:
-        portal_root = spec.portal_root
-    url = spec.urls['global_manifest'].format(portal_root=portal_root)
-
-    # get manifest
-    response = requests.get(url)
-    if response.status_code != 200:
-        raise Exception('could not obtain global manifest at url: ' + str(url))
-    manifest: spec.GlobalManifest = response.json()
-
-    return manifest
-
-
-def get_dataset_manifest(
-    dataset: str, *, portal_root: str | None = None
-) -> spec.DatasetManifest:
-    """get manifest of a particular dataset"""
-
-    import requests
-
-    parsed = parse_dataset_name(dataset)
-
-    # build url
-    if portal_root is None:
-        portal_root = spec.portal_root
-    url = spec.urls['dataset_manifest'].format(
-        portal_root=portal_root,
-        datatype=parsed['datatype'],
-        network=parsed['network'],
-    )
-
-    # get manifest
-    response = requests.get(url)
-    if response.status_code != 200:
-        raise Exception('could not obtain dataset manifest at url: ' + str(url))
-    manifest: spec.DatasetManifest = response.json()
-
-    return manifest
+from .. import spec
+from . import file_utils
+from . import manifest_utils
+from . import schema_utils
 
 
 def download_dataset(
     dataset: str,
     *,
     output_dir: str,
     portal_root: str | None = None,
@@ -68,42 +23,42 @@
     print('Downloading dataset:', dataset)
 
     urls = get_dataset_file_urls(dataset, portal_root=portal_root)
 
     base_url = os.path.dirname(urls[0])
     readme_url = os.path.join(base_url, 'README.md')
     manifest_url = os.path.join(base_url, 'dataset_manifest.json')
-    io_utils.download_files(
+    file_utils.download_files(
         urls=[readme_url, manifest_url],
         output_dir=output_dir,
         skip_existing=skip_existing,
     )
 
     # download files
-    io_utils.download_files(
+    file_utils.download_files(
         urls=urls,
         output_dir=output_dir,
         skip_existing=skip_existing,
     )
 
 
 def get_dataset_file_urls(
     dataset: str,
     *,
     portal_root: str | None,
     manifest: spec.DatasetManifest | None = None,
 ) -> typing.Sequence[str]:
     """get file urls of a dataset"""
 
-    parsed = parse_dataset_name(dataset)
+    parsed = schema_utils.parse_dataset_name(dataset)
 
     if portal_root is None:
         portal_root = spec.portal_root
     if manifest is None:
-        manifest = get_dataset_manifest(
+        manifest = manifest_utils.get_dataset_manifest(
             dataset=dataset, portal_root=portal_root
         )
     urls = []
     for file in manifest['files']:
         url = spec.urls['dataset_file'].format(
             portal_root=portal_root,
             datatype=parsed['datatype'],
@@ -126,28 +81,14 @@
         portal_root=portal_root,
         datatype=datatype,
         network=network,
         filename=filename,
     )
 
 
-def get_dataset_name(*, datatype: str, network: str) -> str:
-    """create dataset name based on metadata"""
-    return network + '_' + datatype
-
-
-def parse_dataset_name(dataset: str) -> typing.Mapping[str, str]:
-    """parse metadata from a dataset name"""
-    network, datatype = dataset.split('_', maxsplit=1)
-    return {
-        'network': network,
-        'datatype': datatype,
-    }
-
-
 def validate_dataset_directory(path: str, *, no_hashes: bool = False) -> bool:
     """validate the files in a dataset directory"""
 
     import json
 
     # load manifest
     manifest_path = os.path.join(path, spec.dataset_manifest_filename)
@@ -175,15 +116,17 @@
     # check file hashes
     if no_hashes:
         bad_hashes = None
     else:
         bad_hashes = []
         for file in manifest['files']:
             if file['name'] in present_files:
-                hash = io_utils.get_file_hash(os.path.join(path, file['name']))
+                hash = file_utils.get_file_hash(
+                    os.path.join(path, file['name'])
+                )
                 target_hash = file['hash']
                 if hash != target_hash:
                     bad_hashes.append(file['name'])
 
     # print errors
     print()
     errors_found = 0
```

### Comparing `paradigm-data-portal-0.2.1/pdp/io_utils.py` & `paradigm-data-portal-0.2.2/pdp/data_utils/file_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""functions for generic file operations"""
+
 from __future__ import annotations
 
 import os
 import typing
 
 
 def download_files(
@@ -39,21 +41,24 @@
         if url not in skip_urls:
             download_file(url)
 
     print()
     print('done')
 
 
-def download_file(url: str) -> None:
+def download_file(url: str, output_path: str | None = None) -> None:
     """download a file"""
     import subprocess
 
     print()
     print('downloading', url)
-    subprocess.call(['curl', url, '--output', os.path.basename(url)])
+    if output_path is None:
+        output_path = os.path.basename(url)
+    os.makedirs(os.path.dirname(output_path), exist_ok=True)
+    subprocess.call(['curl', url, '--output', output_path])
 
 
 def get_file_hash(path: str) -> str:
     """get hash of file"""
 
     import hashlib
```

### Comparing `paradigm-data-portal-0.2.1/pdp/package_utils.py` & `paradigm-data-portal-0.2.2/pdp/data_utils/manifest_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,118 @@
 from __future__ import annotations
 
 import os
-import shutil
 import typing
 
-from . import dataset_utils
-from . import io_utils
-from . import spec
+from .. import config_utils
+from .. import spec
+from . import file_utils
+from . import schema_utils
 
 if typing.TYPE_CHECKING:
     import toolsql
 
 
+def get_global_manifest(
+    *,
+    portal_root: str | None = None,
+    source: typing.Literal['remote', 'local'] = 'remote',
+) -> spec.GlobalManifest:
+    """get global manifest of all datasets"""
+
+    if source == 'remote':
+
+        import requests
+
+        # build url
+        if portal_root is None:
+            portal_root = spec.portal_root
+        url = spec.urls['global_manifest'].format(portal_root=portal_root)
+
+        # get manifest
+        response = requests.get(url)
+        if response.status_code != 200:
+            raise Exception('could not obtain global manifest at url: ' + str(url))
+        manifest: spec.GlobalManifest = response.json()
+
+        return manifest
+
+    elif source == 'local':
+        import json
+
+        if portal_root is not None:
+            data_root = portal_root
+        else:
+            data_root = config_utils.get_data_root(require=True)
+        path = os.path.join(data_root, spec.global_manifest_filename)
+        with open(path, 'r') as f:
+            result: spec.GlobalManifest = json.load(f)
+            return result
+
+    else:
+        raise Exception('invalid source: ' + str(source))
+
+
+def get_dataset_manifest(
+    dataset: str,
+    *,
+    portal_root: str | None = None,
+    source: typing.Literal['remote', 'local'] = 'remote',
+) -> spec.DatasetManifest:
+    """get manifest of a particular dataset"""
+
+    if source == 'remote':
+        import requests
+
+        parsed = schema_utils.parse_dataset_name(dataset)
+
+        # build url
+        if portal_root is None:
+            portal_root = spec.portal_root
+        url = spec.urls['dataset_manifest'].format(
+            portal_root=portal_root,
+            datatype=parsed['datatype'],
+            network=parsed['network'],
+        )
+
+        # get manifest
+        response = requests.get(url)
+        if response.status_code != 200:
+            raise Exception(
+                'could not obtain dataset manifest at url: ' + str(url)
+            )
+        manifest: spec.DatasetManifest = response.json()
+
+        return manifest
+
+    elif source == 'local':
+        import json
+
+        if portal_root is not None:
+            data_root = portal_root
+        else:
+            data_root = config_utils.get_data_root(require=True)
+        path = os.path.join(data_root, dataset, spec.dataset_manifest_filename)
+        with open(path, 'r') as f:
+            result: spec.DatasetManifest = json.load(f)
+            return result
+
+    else:
+        raise Exception('invalid source: ' + str(source))
+
+
 def create_global_manifest(
     *,
     data_root: str | None = None,
     datasets: typing.Mapping[str, spec.DatasetManifestSlim] | None = None,
     version: str | None,
     output_path: str | bool | None = None,
     confirm: bool = False,
 ) -> spec.GlobalManifest:
-    """generate global manifest describing all datasets"""
+    """create global manifest describing all datasets"""
 
     import json
 
     # versions
     if version is None:
         version = spec.global_version
 
@@ -64,14 +152,16 @@
 
     if len(datasets) == 0:
         print('no datasets detected for global manifest')
         return global_manifest
 
     # write output file
     if output_path is not None and output_path:
+        import shutil
+
         if isinstance(output_path, bool):
             if data_root is not None:
                 output_dir = data_root
             else:
                 output_dir = '.'
             output_path = os.path.join(
                 output_dir, spec.global_manifest_filename
@@ -144,40 +234,45 @@
     if dataset_dir is not None:
         dataset_dir = os.path.abspath(os.path.expanduser(dataset_dir))
     if name is None:
         if dataset_dir is None:
             raise Exception('must specify dataset_dir or name')
         name = os.path.basename(dataset_dir)
     if network is None or datatype is None:
-        parsed = dataset_utils.parse_dataset_name(name)
+        parsed = schema_utils.parse_dataset_name(name)
         parsed_network = parsed['network']
         parsed_datatype = parsed['datatype']
         if network is None:
             network = parsed_network
         elif network != parsed_network:
             raise Exception('parsed network does not equal input network')
         if datatype is None:
             datatype = parsed_datatype
         elif datatype != parsed_datatype:
             raise Exception('parsed datatype does not equal input datatype')
+    try:
+        module = schema_utils._get_datatype_module(datatype)
+    except Exception:
+        module = None
     if version is None:
-        if name in spec.dataset_versions:
-            version = spec.dataset_versions[name]
+        if module is not None:
+            version = module.version
         else:
             raise Exception('unknown version for dataset')
     if description is None:
-        if datatype in spec.datatype_schemas:
-            description = spec.datatype_schemas[datatype]['description']
+        if module is not None:
+            description = module.schema['description']
         else:
             raise Exception('could not find description for dataset')
     if schema is None:
-        if datatype in spec.datatype_schemas:
-            schema = spec.datatype_schemas[datatype]
+        if module is not None:
+            schema = module.schema
         else:
             raise Exception('could not find schema for dataset')
+    schema_normalized = toolsql.normalize_shorthand_db_schema(schema)
     print('creating manifest for', name, version)
 
     # gather files
     if paths is None:
         if dataset_dir is None:
             raise Exception('must specify paths or dataset_dir')
         exclude = [
@@ -199,15 +294,15 @@
             old_data = json.load(f)
         old_hashes = {file['name']: file['hash'] for file in old_data['files']}
     file_hashes = []
     for path in paths:
         if reuse_hashes and os.path.basename(path) in old_hashes:
             file_hashes.append(old_hashes[os.path.basename(path)])
         else:
-            file_hashes.append(io_utils.get_file_hash(path))
+            file_hashes.append(file_utils.get_file_hash(path))
 
     # assemble files
     files = []
     for path, file_hash in zip(paths, file_hashes):
         file: spec.FileMetadata = {
             'name': os.path.basename(path),
             'hash': file_hash,
@@ -219,19 +314,21 @@
     manifest: spec.DatasetManifest = {
         'name': name,
         'version': version,
         'description': description or '',
         'datatype': datatype,
         'network': network,
         'files': files,
-        'schema': schema,
+        'schema': schema_normalized,
     }
 
     # save manifest
     if output_path is not None and output_path:
+        import shutil
+
         with open(output_path + '_tmp', 'w') as f:
             json.dump(manifest, f, indent=4, sort_keys=True)
 
         shutil.move(output_path + '_tmp', output_path)
         if data_root is not None:
             print_dir = os.path.relpath(output_path, data_root)
         else:
```

### Comparing `paradigm-data-portal-0.2.1/pdp/readme_utils.py` & `paradigm-data-portal-0.2.2/pdp/data_utils/readme_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""functions for creating dataset README's"""
+
 from __future__ import annotations
 
 import os
 
-from . import dataset_utils
-from . import spec
+from .. import spec
+from . import download_utils
+from . import schema_utils
 
 
 readme_template = """
 # {network} {datatype} Dataset v{version}
 
 This is a dataset of {description}
 
@@ -41,15 +44,15 @@
 ### Use URLs
 
 | | file | size |
 | - | - | - |
 {file_urls}
 """
 
-script_url_template = 'https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/generate/generate_{datatype}_dataset.py'
+script_url_template = 'https://github.com/paradigmxyz/paradigm-data-portal/blob/main/pdp/datasets/{dataset}/{dataset}_collect.py'
 
 notebook_url_template = 'https://github.com/paradigmxyz/paradigm-data-portal/blob/main/notebooks/explore_{dataset_name}.ipynb'
 
 table_schema_template = """#### `{table_name}` table
 {table_description}
 | column | type | description |
 | - | - | - |
@@ -60,38 +63,36 @@
     dataset_manifest: spec.DatasetManifest,
     output_path: str | bool = False,
     confirm: bool = False,
 ) -> str:
 
     import shutil
 
-    readme_str = _generate_readme_str(dataset_manifest)
+    readme_str = _create_readme_str(dataset_manifest)
 
     if output_path is not None and output_path:
         if isinstance(output_path, bool):
             output_path = spec.dataset_readme_filename
         if os.path.exists(output_path) and not confirm:
             print('use --confirm to overwrite existing README')
         with open(output_path + '_tmp', 'w') as f:
             f.write(readme_str)
         shutil.move(output_path + '_tmp', output_path)
         print('wrote README to ' + output_path)
 
     return readme_str
 
 
-def _generate_readme_str(dataset_manifest: spec.DatasetManifest) -> str:
+def _create_readme_str(dataset_manifest: spec.DatasetManifest) -> str:
 
     import toolsql
     import toolstr
 
-    example_usage_pieces = [
-        '- ' + example
-        for example in spec.datatype_example_usage[dataset_manifest['datatype']]
-    ]
+    module = schema_utils._get_datatype_module(dataset_manifest['datatype'])
+    example_usage_pieces = ['- ' + example for example in module.example_usage]
     example_usage_str = '\n'.join(example_usage_pieces)
 
     schema_pieces = []
     db_schema = toolsql.normalize_shorthand_db_schema(
         dataset_manifest['schema']
     )
     for table_name, table in db_schema['tables'].items():
@@ -114,15 +115,15 @@
         schema_pieces.append(table_schema_str)
     schema_str = '\n'.join(schema_pieces)
 
     url_pieces: list[str] = []
     for file in dataset_manifest['files']:
         if file['name'] == spec.dataset_readme_filename:
             continue
-        file_url = dataset_utils.get_dataset_file_url(
+        file_url = download_utils.get_dataset_file_url(
             datatype=dataset_manifest['datatype'],
             network=dataset_manifest['network'],
             filename=file['name'],
         )
         url_piece = (
             '| '
             + str(len(url_pieces) + 1)
@@ -152,14 +153,12 @@
         network=dataset_manifest['network'].replace('_', ' ').title(),
         datatype=dataset_manifest['datatype'].replace('_', ' ').title(),
         version=dataset_manifest['version'],
         description=dataset_manifest['description'],
         example_usage=example_usage_str,
         schema=schema_str,
         dataset_size=toolstr.format_nbytes(dataset_nbytes),
-        script_url=script_url_template.format(
-            datatype=dataset_manifest['datatype']
-        ),
+        script_url=script_url_template.format(dataset=dataset_manifest['name']),
         notebook_str=notebook_str,
         file_urls=url_str,
     )
```

### Comparing `paradigm-data-portal-0.2.1/PKG-INFO` & `paradigm-data-portal-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradigm-data-portal
-Version: 0.2.1
+Version: 0.2.2
 Summary: pdp downloads and manages datasets from the Paradigm Data Portal
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
@@ -17,17 +17,22 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: typing-extensions >=4.2.0, <5
-Requires-Dist: toolcli >=0.6.8, <0.7
-Requires-Dist: toolstr >=0.9.1, <0.10
 Requires-Dist: requests >=2.20.0, <3
+Requires-Dist: toolcli >=0.6.13, <0.7
+Requires-Dist: toolstr >=0.9.3, <0.10
+Requires-Dist: tooljob >=0.1.6, <0.2
+Requires-Dist: mypy ==1.2.0 ; extra == "test"
+Requires-Dist: mypy_extensions >= 1.0.0, <1.1.0 ; extra == "test"
+Requires-Dist: pytest >=6, <7 ; extra == "test"
+Provides-Extra: test
 
 
 # Paradigm Data Portal
 
 The Paradigm Data Portal is a collection of open source crypto datasets for researchers and tool builders
 
 ## Datasets
```

