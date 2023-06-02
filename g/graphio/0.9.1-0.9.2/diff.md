# Comparing `tmp/graphio-0.9.1.tar.gz` & `tmp/graphio-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphio-0.9.1.tar", last modified: Tue Apr  4 17:15:12 2023, max compression
+gzip compressed data, was "graphio-0.9.2.tar", last modified: Fri Jun  2 10:08:13 2023, max compression
```

## Comparing `graphio-0.9.1.tar` & `graphio-0.9.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 17:15:12.348646 graphio-0.9.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-04 17:14:57.000000 graphio-0.9.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-04 17:15:12.352646 graphio-0.9.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-04 17:14:57.000000 graphio-0.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 17:15:12.348646 graphio-0.9.1/graphio/
--rw-r--r--   0 root         (0) root         (0)      574 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/defaults.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/graph.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/helper.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 17:15:12.348646 graphio-0.9.1/graphio/objects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/datacontainer.py
--rw-r--r--   0 root         (0) root         (0)    20220 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/nodeset.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/properties.py
--rw-r--r--   0 root         (0) root         (0)    26751 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/relationshipset.py
--rw-r--r--   0 root         (0) root         (0)     3693 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/unstructured_nodeset.py
--rw-r--r--   0 root         (0) root         (0)     6663 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/unstructured_relationshipset.py
--rw-r--r--   0 root         (0) root         (0)     3874 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/objects/update.py
--rw-r--r--   0 root         (0) root         (0)    10987 2023-04-04 17:14:57.000000 graphio-0.9.1/graphio/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 17:15:12.348646 graphio-0.9.1/graphio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2189 2023-04-04 17:15:09.000000 graphio-0.9.1/graphio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-04 17:15:12.000000 graphio-0.9.1/graphio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 17:15:09.000000 graphio-0.9.1/graphio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 17:15:09.000000 graphio-0.9.1/graphio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-04 17:15:09.000000 graphio-0.9.1/graphio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-04 17:15:09.000000 graphio-0.9.1/graphio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-04 17:15:12.352646 graphio-0.9.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2023-04-04 17:14:57.000000 graphio-0.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 17:15:12.348646 graphio-0.9.1/test/
--rw-r--r--   0 root         (0) root         (0)      296 2023-04-04 17:14:57.000000 graphio-0.9.1/test/test_graph.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-04-04 17:14:57.000000 graphio-0.9.1/test/test_helper.py
--rw-r--r--   0 root         (0) root         (0)     2529 2023-04-04 17:14:57.000000 graphio-0.9.1/test/test_model.py
--rw-r--r--   0 root         (0) root         (0)     6579 2023-04-04 17:14:57.000000 graphio-0.9.1/test/test_queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.567498 graphio-0.9.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 10:07:58.000000 graphio-0.9.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:08:13.567498 graphio-0.9.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-02 10:07:58.000000 graphio-0.9.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.559498 graphio-0.9.2/graphio/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/helper.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/graphio/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/datacontainer.py
+-rw-r--r--   0 root         (0) root         (0)    20220 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/nodeset.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/properties.py
+-rw-r--r--   0 root         (0) root         (0)    26836 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/relationshipset.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/unstructured_nodeset.py
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/unstructured_relationshipset.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/update.py
+-rw-r--r--   0 root         (0) root         (0)    10987 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/graphio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-02 10:08:13.567498 graphio-0.9.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-02 10:07:58.000000 graphio-0.9.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/test/
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_model.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_queries.py
```

### Comparing `graphio-0.9.1/LICENSE` & `graphio-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/PKG-INFO` & `graphio-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphio
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library to load data sets to Neo4j.
 Home-page: https://github.com/kaiserpreusse/graphio
 Author: Martin Preusse
 Author-email: martin.preusse@gmail.com
 License: Apache License 2.0
 Keywords: NEO4J
 Platform: UNKNOWN
```

### Comparing `graphio-0.9.1/README.md` & `graphio-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/__init__.py` & `graphio-0.9.2/graphio/__init__.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/helper.py` & `graphio-0.9.2/graphio/helper.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/model.py` & `graphio-0.9.2/graphio/model.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/objects/datacontainer.py` & `graphio-0.9.2/graphio/objects/datacontainer.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/objects/nodeset.py` & `graphio-0.9.2/graphio/objects/nodeset.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/objects/relationshipset.py` & `graphio-0.9.2/graphio/objects/relationshipset.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,25 +278,28 @@
         :param write_mode: Write mode for the CSV file.
         """
         self.to_csv(csv_file_path)
         with open(json_file_path, write_mode) as f:
             json.dump(self.metadata_dict, f)
 
     @classmethod
-    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items: bool = False):
+    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items: bool = False, reltype_key=None):
         """
         Read the default CSV/JSON file combination.
 
         Needs paths to CSV and JSON file.
 
         :param csv_file_path: Path to the CSV file.
         :param json_file_path: Path to the JSON file.
         :param load_items: Yield items from file (False, default) or load them to memory (True).
         :return: The RelationshipSet.
         """
+        if not reltype_key:
+            reltype_key = 'rel_type'
+
         with open(json_file_path) as f:
             metadata = json.load(f)
 
         # map properties
         property_map = None
         if 'property_map' in metadata:
             # replace start_node/end_node keys if necessary
@@ -307,15 +310,15 @@
                                                metadata['end_node_properties']]
 
         # type conversions
         start_node_type_conversion = metadata.get('start_node_type_conversion', None)
         end_node_type_conversion = metadata.get('end_node_type_conversion', None)
 
         # RelationshipSet instance
-        rs = cls(metadata['rel_type'],
+        rs = cls(metadata[reltype_key],
                  metadata['start_node_labels'],
                  metadata['end_node_labels'],
                  remove_prefix_from_keys(metadata['start_node_properties']),
                  remove_prefix_from_keys(metadata['end_node_properties']))
 
         start_key_to_header = {}
         for k in rs.start_node_properties:
```

### Comparing `graphio-0.9.1/graphio/objects/unstructured_nodeset.py` & `graphio-0.9.2/graphio/objects/unstructured_nodeset.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/objects/unstructured_relationshipset.py` & `graphio-0.9.2/graphio/objects/unstructured_relationshipset.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/objects/update.py` & `graphio-0.9.2/graphio/objects/update.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio/queries.py` & `graphio-0.9.2/graphio/queries.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/graphio.egg-info/PKG-INFO` & `graphio-0.9.2/graphio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphio
-Version: 0.9.1
+Version: 0.9.2
 Summary: Library to load data sets to Neo4j.
 Home-page: https://github.com/kaiserpreusse/graphio
 Author: Martin Preusse
 Author-email: martin.preusse@gmail.com
 License: Apache License 2.0
 Keywords: NEO4J
 Platform: UNKNOWN
```

### Comparing `graphio-0.9.1/graphio.egg-info/SOURCES.txt` & `graphio-0.9.2/graphio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/setup.py` & `graphio-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/test/test_helper.py` & `graphio-0.9.2/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/test/test_model.py` & `graphio-0.9.2/test/test_model.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.1/test/test_queries.py` & `graphio-0.9.2/test/test_queries.py`

 * *Files identical despite different names*

