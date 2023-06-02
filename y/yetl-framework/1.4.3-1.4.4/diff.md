# Comparing `tmp/yetl-framework-1.4.3.tar.gz` & `tmp/yetl-framework-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.4.3.tar", last modified: Fri Jun  2 00:40:16 2023, max compression
+gzip compressed data, was "yetl-framework-1.4.4.tar", last modified: Fri Jun  2 08:04:32 2023, max compression
```

## Comparing `yetl-framework-1.4.3.tar` & `yetl-framework-1.4.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1150 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.470318 yetl-framework-1.4.3/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15345 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-02 00:39:25.000000 yetl-framework-1.4.3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 00:40:16.474318 yetl-framework-1.4.3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       29 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-02 00:40:16.000000 yetl-framework-1.4.3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4653 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1217 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2775 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.663024 yetl-framework-1.4.4/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16017 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3023 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2007 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8764 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5040 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16393 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3790 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4049 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.667024 yetl-framework-1.4.4/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-06-02 08:03:39.000000 yetl-framework-1.4.4/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-02 08:04:32.671024 yetl-framework-1.4.4/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5150 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      977 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       57 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-06-02 08:04:32.000000 yetl-framework-1.4.4/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.4.3/PKG-INFO` & `yetl-framework-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.3
+Version: 1.4.4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.3/README.md` & `yetl-framework-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/setup.py` & `yetl-framework-1.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.4.3",
+    version="1.4.4",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
@@ -36,11 +36,14 @@
         "yetl.workflow",
 
     ],
     install_requires=[
           'PyYAML',
           'jinja2',
           'pydantic',
-          'typer'
+          'typer',
+          'pandas',
+          'openpyxl',
+          'delta-spark'
       ],
     zip_safe=False
 )
```

### Comparing `yetl-framework-1.4.3/yetl/__main__.py` & `yetl-framework-1.4.4/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/cli/_init.py` & `yetl-framework-1.4.4/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.4.4/yetl/cli/metadata_provider/_xlsx.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,30 +79,32 @@
     deltalake_delta_properties: str = Field(default=None)
     custom_properties: Dict[str, Any] = Field(default=None)
     deltalake_identity: str = Field(default=None)
     deltalake_partition_by: str = Field(default=None)
     deltalake_delta_constraints: str = Field(default=None)
     deltalake_z_order_by: str = Field(default=None)
     deltalake_vacuum: Union[int, None] = Field(default=None)
-    warning_thresholds_invalid_ratio: float = Field(default=None)
-    warning_thresholds_invalid_rows: float = Field(default=None)
-    warning_thresholds_max_rows: float = Field(default=None)
-    warning_thresholds_mins_rows: float = Field(default=None)
+    warning_thresholds_invalid_ratio: int = Field(default=None)
+    warning_thresholds_invalid_rows: int = Field(default=None)
+    warning_thresholds_max_rows: int = Field(default=None)
+    warning_thresholds_mins_rows: int = Field(default=None)
     error_thresholds_invalid_ratio: float = Field(default=None)
-    error_thresholds_invalid_rows: float = Field(default=None)
-    error_thresholds_max_rows: float = Field(default=None)
-    error_thresholds_mins_rows: float = Field(default=None)
-    version: str = Field(default=pkg_resources.get_distribution("yetl-framework").version)
+    error_thresholds_invalid_rows: int = Field(default=None)
+    error_thresholds_max_rows: int = Field(default=None)
+    error_thresholds_mins_rows: int = Field(default=None)
+    version: str = Field(
+        default=pkg_resources.get_distribution("yetl-framework").version
+    )
 
-    def _get_list(self, data: Any):
+    def _get_list(self, data: Any, default_singluar_to_str: bool = True):
         if data is None:
             return None
-        elif isinstance(data, str) and "\n" in data:
+        elif isinstance(data, str):
             datal = [i.strip() for i in data.split("\n")]
-            if len(datal) == 1:
+            if len(datal) == 1 and default_singluar_to_str:
                 return datal[0]
             else:
                 return datal
         else:
             return data
 
     def _get_dict(self, data: str):
@@ -209,15 +211,17 @@
             }
         }
 
         table = None
         if self._has_properties():
             table = {}
             if self.depends_on is not None:
-                table[ColumnNames.depends_on.name] = self._get_list(self.depends_on)
+                table[ColumnNames.depends_on.name] = self._get_list(
+                    self.depends_on, default_singluar_to_str=False
+                )
             if self.ids is not None:
                 table[ColumnNames.ids.name] = self._get_list(self.ids)
             if self.sql is not None and self.sql.lower() == "y":
                 table["sql"] = "../sql/{{database}}/{{table}}.sql"
             if self.deltalake_partition_by is not None:
                 table[ColumnNames.partition_by.name] = self._get_list(
                     self.deltalake_partition_by
@@ -281,14 +285,37 @@
         df = pd.read_excel(self.source, header=[0, 1])
         df = self.validate_schema(df)
         self.data = self._deserialize(df)
 
     source: str = Field(...)
     data: dict = Field(default=None)
 
+    def _auto_convert(self, data: Any):
+
+        if isinstance(data, float):
+            if data.is_integer():
+                return int(data)
+        if isinstance(data, str):
+            try:
+                data = float(data)
+            except ValueError:
+                pass
+
+            try:
+                data = int(data)
+            except ValueError:
+                pass
+
+            if data.lower() in ["true", "false"]:
+                data = bool(data)
+
+            return data
+        else:
+            return data
+
     def _deserialize(self, df: pd.DataFrame):
         df = df.to_dict(orient="records")
         metadata = [
             {
                 "_".join([n for n in list(k) if not n.startswith("Unnamed")]): (
                     None if pd.isna(v) else v
                 )
@@ -297,15 +324,15 @@
             for r in df
         ]
         for item in metadata:
             custom_properties = {}
             for k, v in item.items():
                 if k.startswith(ColumnNames.custom_properties.name) and v is not None:
                     prop_key = k.replace(f"{ColumnNames.custom_properties.name}_", "")
-                    custom_properties[prop_key] = v
+                    custom_properties[prop_key] = self._auto_convert(v)
             if custom_properties:
                 item[ColumnNames.custom_properties.name] = custom_properties
 
         df = [Metadata(**m).dict() for m in metadata]
 
         # deep merge
         data = reduce(XlsMetadata.merge, [r for r in df])
```

### Comparing `yetl-framework-1.4.3/yetl/config/__init__.py` & `yetl-framework-1.4.4/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_config.py` & `yetl-framework-1.4.4/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_decorators.py` & `yetl-framework-1.4.4/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_logging_config.py` & `yetl-framework-1.4.4/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_project.py` & `yetl-framework-1.4.4/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_spark_context.py` & `yetl-framework-1.4.4/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_tables.py` & `yetl-framework-1.4.4/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_timeslice.py` & `yetl-framework-1.4.4/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/_utils.py` & `yetl-framework-1.4.4/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/deltalake.py` & `yetl-framework-1.4.4/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/table/_deltalake.py` & `yetl-framework-1.4.4/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/table/_factory.py` & `yetl-framework-1.4.4/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/table/_read.py` & `yetl-framework-1.4.4/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/config/table/_table.py` & `yetl-framework-1.4.4/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.4.4/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.4.3/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-1.4.4/yetl_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.4.3
+Version: 1.4.4
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.4.3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.4.4/yetl_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

