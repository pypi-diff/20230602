# Comparing `tmp/graphio-0.9.2.tar.gz` & `tmp/graphio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphio-0.9.2.tar", last modified: Fri Jun  2 10:08:13 2023, max compression
+gzip compressed data, was "graphio-0.9.3.tar", last modified: Fri Jun  2 10:24:36 2023, max compression
```

## Comparing `graphio-0.9.2.tar` & `graphio-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.567498 graphio-0.9.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 10:07:58.000000 graphio-0.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:08:13.567498 graphio-0.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-02 10:07:58.000000 graphio-0.9.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.559498 graphio-0.9.2/graphio/
--rw-r--r--   0 root         (0) root         (0)      574 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/__init__.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/defaults.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/graph.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/helper.py
--rw-r--r--   0 root         (0) root         (0)     6059 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/graphio/objects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/datacontainer.py
--rw-r--r--   0 root         (0) root         (0)    20220 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/nodeset.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/properties.py
--rw-r--r--   0 root         (0) root         (0)    26836 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/relationshipset.py
--rw-r--r--   0 root         (0) root         (0)     3693 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/unstructured_nodeset.py
--rw-r--r--   0 root         (0) root         (0)     6663 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/unstructured_relationshipset.py
--rw-r--r--   0 root         (0) root         (0)     3874 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/objects/update.py
--rw-r--r--   0 root         (0) root         (0)    10987 2023-06-02 10:07:58.000000 graphio-0.9.2/graphio/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/graphio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 10:08:13.000000 graphio-0.9.2/graphio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-02 10:08:13.567498 graphio-0.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-02 10:07:58.000000 graphio-0.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:08:13.563498 graphio-0.9.2/test/
--rw-r--r--   0 root         (0) root         (0)      296 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_graph.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_helper.py
--rw-r--r--   0 root         (0) root         (0)     2529 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_model.py
--rw-r--r--   0 root         (0) root         (0)     6579 2023-06-02 10:07:58.000000 graphio-0.9.2/test/test_queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:24:36.261693 graphio-0.9.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 10:24:25.000000 graphio-0.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:24:36.261693 graphio-0.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-02 10:24:25.000000 graphio-0.9.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:24:36.257692 graphio-0.9.3/graphio/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/helper.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:24:36.261693 graphio-0.9.3/graphio/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/datacontainer.py
+-rw-r--r--   0 root         (0) root         (0)    20494 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/nodeset.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/properties.py
+-rw-r--r--   0 root         (0) root         (0)    27435 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/relationshipset.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/unstructured_nodeset.py
+-rw-r--r--   0 root         (0) root         (0)     6663 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/unstructured_relationshipset.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/objects/update.py
+-rw-r--r--   0 root         (0) root         (0)    10987 2023-06-02 10:24:25.000000 graphio-0.9.3/graphio/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:24:36.261693 graphio-0.9.3/graphio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-02 10:24:36.000000 graphio-0.9.3/graphio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-02 10:24:36.261693 graphio-0.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-02 10:24:25.000000 graphio-0.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 10:24:36.261693 graphio-0.9.3/test/
+-rw-r--r--   0 root         (0) root         (0)      296 2023-06-02 10:24:25.000000 graphio-0.9.3/test/test_graph.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-02 10:24:25.000000 graphio-0.9.3/test/test_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-06-02 10:24:25.000000 graphio-0.9.3/test/test_model.py
+-rw-r--r--   0 root         (0) root         (0)     6579 2023-06-02 10:24:25.000000 graphio-0.9.3/test/test_queries.py
```

### Comparing `graphio-0.9.2/LICENSE` & `graphio-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/PKG-INFO` & `graphio-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphio
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library to load data sets to Neo4j.
 Home-page: https://github.com/kaiserpreusse/graphio
 Author: Martin Preusse
 Author-email: martin.preusse@gmail.com
 License: Apache License 2.0
 Keywords: NEO4J
 Platform: UNKNOWN
```

### Comparing `graphio-0.9.2/README.md` & `graphio-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/__init__.py` & `graphio-0.9.3/graphio/__init__.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/helper.py` & `graphio-0.9.3/graphio/helper.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/model.py` & `graphio-0.9.3/graphio/model.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/objects/datacontainer.py` & `graphio-0.9.3/graphio/objects/datacontainer.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/objects/nodeset.py` & `graphio-0.9.3/graphio/objects/nodeset.py`

 * *Files 4% similar despite different names*

```diff
@@ -305,40 +305,46 @@
         with open(json_file_path, 'w') as f:
             json_dict = self.metadata_dict
             if type_conversion:
                 json_dict['type_conversion'] = type_conversion
             json.dump(json_dict, f)
 
     @classmethod
-    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items:bool = False):
+    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items:bool = False,
+                          labels_key:str = None, mergekey_key:str = None):
         """
-        Read the default CSV/JSON file combination.
+        Read the default CSV/JSON file combination. Needs paths to CSV and JSON file.
 
-        Needs paths to CSV and JSON file.
+        JSON keys can be overwritten by passing the respective parameters.
 
         :param csv_file_path: Path to the CSV file.
         :param json_file_path: Path to the JSON file.
         :param load_items: Yield items from file (False, default) or load them to memory (True).
         :return: The NodeSet.
         """
+        if not labels_key:
+            labels_key = 'labels'
+        if not mergekey_key:
+            mergekey_key = 'merge_keys'
+
         with open(json_file_path) as f:
             metadata = json.load(f)
 
         # map properties
         property_map = None
         if 'property_map' in metadata:
             # replace mergekeys if necessary
             property_map = metadata['property_map']
-            metadata['merge_keys'] = [property_map[x] if x in property_map else x for x in metadata['merge_keys']]
+            metadata[mergekey_key] = [property_map[x] if x in property_map else x for x in metadata[mergekey_key]]
 
         # type conversion
         type_conversion = metadata.get('type_conversion', None)
 
         # NodeSet instance
-        nodeset = cls(metadata['labels'], merge_keys=metadata['merge_keys'])
+        nodeset = cls(metadata[labels_key], merge_keys=metadata[mergekey_key])
 
         if load_items:
             nodeset.nodes = _read_nodes(csv_file_path, property_map, type_conversion)
         else:
             nodeset.nodes = _yield_node(csv_file_path, property_map, type_conversion)
 
         return nodeset
```

### Comparing `graphio-0.9.2/graphio/objects/relationshipset.py` & `graphio-0.9.3/graphio/objects/relationshipset.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,51 +278,61 @@
         :param write_mode: Write mode for the CSV file.
         """
         self.to_csv(csv_file_path)
         with open(json_file_path, write_mode) as f:
             json.dump(self.metadata_dict, f)
 
     @classmethod
-    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items: bool = False, reltype_key=None):
+    def from_csv_json_set(cls, csv_file_path, json_file_path, load_items: bool = False,
+                          reltype_key=None, startnodeproperties_key=None, endnodeproperties_key=None,
+                          startnodelables_key=None, endnodelables_key=None):
         """
-        Read the default CSV/JSON file combination.
+        Read the default CSV/JSON file combination. Needs paths to CSV and JSON file.
 
-        Needs paths to CSV and JSON file.
+        JSON keys can be overwritten by passing the respective parameters.
 
         :param csv_file_path: Path to the CSV file.
         :param json_file_path: Path to the JSON file.
         :param load_items: Yield items from file (False, default) or load them to memory (True).
         :return: The RelationshipSet.
         """
         if not reltype_key:
             reltype_key = 'rel_type'
+        if not startnodeproperties_key:
+            startnodeproperties_key = 'start_node_properties'
+        if not endnodeproperties_key:
+            endnodeproperties_key = 'end_node_properties'
+        if not startnodelables_key:
+            startnodelables_key = 'start_node_labels'
+        if not endnodelables_key:
+            endnodelables_key = 'end_node_labels'
 
         with open(json_file_path) as f:
             metadata = json.load(f)
 
         # map properties
         property_map = None
         if 'property_map' in metadata:
             # replace start_node/end_node keys if necessary
             property_map = metadata['property_map']
-            metadata['start_node_properties'] = [property_map[x] if x in property_map else x for x in
-                                                 metadata['start_node_properties']]
-            metadata['end_node_properties'] = [property_map[x] if x in property_map else x for x in
-                                               metadata['end_node_properties']]
+            metadata[startnodeproperties_key] = [property_map[x] if x in property_map else x for x in
+                                                 metadata[startnodeproperties_key]]
+            metadata[endnodeproperties_key] = [property_map[x] if x in property_map else x for x in
+                                               metadata[endnodeproperties_key]]
 
         # type conversions
         start_node_type_conversion = metadata.get('start_node_type_conversion', None)
         end_node_type_conversion = metadata.get('end_node_type_conversion', None)
 
         # RelationshipSet instance
         rs = cls(metadata[reltype_key],
-                 metadata['start_node_labels'],
-                 metadata['end_node_labels'],
-                 remove_prefix_from_keys(metadata['start_node_properties']),
-                 remove_prefix_from_keys(metadata['end_node_properties']))
+                 metadata[startnodelables_key],
+                 metadata[endnodelables_key],
+                 remove_prefix_from_keys(metadata[startnodeproperties_key]),
+                 remove_prefix_from_keys(metadata[endnodeproperties_key]))
 
         start_key_to_header = {}
         for k in rs.start_node_properties:
             start_key_to_header[k] = f"start_{k}"
 
         end_key_to_header = {}
         for k in rs.end_node_properties:
```

### Comparing `graphio-0.9.2/graphio/objects/unstructured_nodeset.py` & `graphio-0.9.3/graphio/objects/unstructured_nodeset.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/objects/unstructured_relationshipset.py` & `graphio-0.9.3/graphio/objects/unstructured_relationshipset.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/objects/update.py` & `graphio-0.9.3/graphio/objects/update.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio/queries.py` & `graphio-0.9.3/graphio/queries.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/graphio.egg-info/PKG-INFO` & `graphio-0.9.3/graphio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphio
-Version: 0.9.2
+Version: 0.9.3
 Summary: Library to load data sets to Neo4j.
 Home-page: https://github.com/kaiserpreusse/graphio
 Author: Martin Preusse
 Author-email: martin.preusse@gmail.com
 License: Apache License 2.0
 Keywords: NEO4J
 Platform: UNKNOWN
```

### Comparing `graphio-0.9.2/graphio.egg-info/SOURCES.txt` & `graphio-0.9.3/graphio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/setup.py` & `graphio-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/test/test_helper.py` & `graphio-0.9.3/test/test_helper.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/test/test_model.py` & `graphio-0.9.3/test/test_model.py`

 * *Files identical despite different names*

### Comparing `graphio-0.9.2/test/test_queries.py` & `graphio-0.9.3/test/test_queries.py`

 * *Files identical despite different names*

