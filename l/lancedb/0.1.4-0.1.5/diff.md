# Comparing `tmp/lancedb-0.1.4.tar.gz` & `tmp/lancedb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.4.tar", last modified: Thu Jun  1 03:20:34 2023, max compression
+gzip compressed data, was "lancedb-0.1.5.tar", last modified: Fri Jun  2 16:27:12 2023, max compression
```

## Comparing `lancedb-0.1.4.tar` & `lancedb-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.444041 lancedb-0.1.4/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-01 03:20:34.443940 lancedb-0.1.4/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.443133 lancedb-0.1.4/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.4/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     3377 2023-05-05 18:26:36.000000 lancedb-0.1.4/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.4/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.4/lancedb/fts.py
--rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.4/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     8833 2023-05-25 04:41:19.000000 lancedb-0.1.4/lancedb/table.py
--rw-r--r--   0 changshe   (501) staff       (20)     1376 2023-05-05 01:55:15.000000 lancedb-0.1.4/lancedb/util.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-01 03:20:34.443781 lancedb-0.1.4/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      151 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-01 03:20:34.000000 lancedb-0.1.4/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-06-01 03:10:24.000000 lancedb-0.1.4/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-01 03:20:34.444085 lancedb-0.1.4/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.4/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.545164 lancedb-0.1.5/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-02 16:27:12.545070 lancedb-0.1.5/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.544464 lancedb-0.1.5/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.5/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.5/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.5/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4134 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.5/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3836 2023-05-25 23:57:48.000000 lancedb-0.1.5/lancedb/fts.py
+-rw-r--r--   0 changshe   (501) staff       (20)     4872 2023-05-25 23:57:48.000000 lancedb-0.1.5/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     8861 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/table.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1800 2023-06-02 16:16:59.000000 lancedb-0.1.5/lancedb/util.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-02 16:27:12.544932 lancedb-0.1.5/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)     1003 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      151 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-02 16:27:12.000000 lancedb-0.1.5/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1333 2023-06-02 16:18:01.000000 lancedb-0.1.5/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-02 16:27:12.545194 lancedb-0.1.5/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.5/setup.py
```

### Comparing `lancedb-0.1.4/PKG-INFO` & `lancedb-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.4
+Version: 0.1.5
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.4/lancedb/__init__.py` & `lancedb-0.1.5/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/common.py` & `lancedb-0.1.5/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/context.py` & `lancedb-0.1.5/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/db.py` & `lancedb-0.1.5/lancedb/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,24 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from __future__ import annotations
 
+import os
 from pathlib import Path
+import os
 
 import pyarrow as pa
+from pyarrow import fs
 
 from .common import DATA, URI
 from .table import LanceTable
-from .util import get_uri_scheme
+from .util import get_uri_scheme, get_uri_location
 
 
 class LanceDBConnection:
     """
     A connection to a LanceDB database.
     """
 
@@ -43,19 +46,28 @@
     def table_names(self) -> list[str]:
         """Get the names of all tables in the database.
 
         Returns
         -------
         A list of table names.
         """
-        if get_uri_scheme(self.uri) == "file":
-            return [p.stem for p in Path(self.uri).glob("*.lance")]
-        raise NotImplementedError(
-            "List table_names is only supported for local filesystem for now"
-        )
+        try:
+            filesystem, path = fs.FileSystem.from_uri(self.uri)
+        except pa.ArrowInvalid:
+            raise NotImplementedError(
+                "Unsupported scheme: " + self.uri
+            )
+
+        try:
+            paths = filesystem.get_file_info(fs.FileSelector(get_uri_location(self.uri)))
+        except FileNotFoundError:
+            # It is ok if the file does not exist since it will be created
+            paths = []
+        tables = [os.path.splitext(file_info.base_name)[0] for file_info in paths if file_info.extension == 'lance']
+        return tables
 
     def __len__(self) -> int:
         return len(self.table_names())
 
     def __contains__(self, name: str) -> bool:
         return name in self.table_names()
 
@@ -108,7 +120,19 @@
             The name of the table.
 
         Returns
         -------
         A LanceTable object representing the table.
         """
         return LanceTable(self, name)
+
+    def drop_table(self, name: str):
+        """Drop a table from the database.
+
+        Parameters
+        ----------
+        name: str
+            The name of the table.
+        """
+        filesystem, path = pa.fs.FileSystem.from_uri(self.uri)
+        table_path = os.path.join(path, name + ".lance")
+        filesystem.delete_dir(table_path)
```

### Comparing `lancedb-0.1.4/lancedb/embeddings.py` & `lancedb-0.1.5/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/fts.py` & `lancedb-0.1.5/lancedb/fts.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/query.py` & `lancedb-0.1.5/lancedb/query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.4/lancedb/table.py` & `lancedb-0.1.5/lancedb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,21 +249,20 @@
     Parameters
     ----------
     data: pa.Table
         The table to sanitize.
     vector_column_name: str
         The name of the vector column.
     """
-    i = data.column_names.index(vector_column_name)
-    if i < 0:
+    if vector_column_name not in data.column_names:
         raise ValueError(f"Missing vector column: {vector_column_name}")
     vec_arr = data[vector_column_name].combine_chunks()
     if pa.types.is_fixed_size_list(vec_arr.type):
         return data
     if not pa.types.is_list(vec_arr.type):
         raise TypeError(f"Unsupported vector column type: {vec_arr.type}")
     values = vec_arr.values
     if not pa.types.is_float32(values.type):
         values = values.cast(pa.float32())
     list_size = len(values) / len(data)
     vec_arr = pa.FixedSizeListArray.from_arrays(values, list_size)
-    return data.set_column(i, vector_column_name, vec_arr)
+    return data.set_column(data.column_names.index(vector_column_name), vector_column_name, vec_arr)
```

### Comparing `lancedb-0.1.4/lancedb/util.py` & `lancedb-0.1.5/lancedb/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,7 +37,27 @@
         scheme = "s3"
     elif len(scheme) == 1:
         # Windows drive names are parsed as the scheme
         # e.g. "c:\path" -> ParseResult(scheme="c", netloc="", path="/path", ...)
         # So we add special handling here for schemes that are a single character
         scheme = "file"
     return scheme
+
+
+def get_uri_location(uri: str) -> str:
+    """
+    Get the location of a URI. If the parameter is not a url, assumes it is just a path
+
+    Parameters
+    ----------
+    uri : str
+        The URI to parse.
+
+    Returns
+    -------
+    str: Location part of the URL, without scheme
+    """
+    parsed = urlparse(uri)
+    if not parsed.netloc:
+        return parsed.path
+    else:
+        return parsed.netloc + parsed.path
```

### Comparing `lancedb-0.1.4/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.5/lancedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.4
+Version: 0.1.5
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.4/pyproject.toml` & `lancedb-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lancedb"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = ["pylance>=0.4.17", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `lancedb-0.1.4/setup.py` & `lancedb-0.1.5/setup.py`

 * *Files identical despite different names*

