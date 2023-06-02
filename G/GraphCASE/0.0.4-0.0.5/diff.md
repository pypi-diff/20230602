# Comparing `tmp/GraphCASE-0.0.4.tar.gz` & `tmp/GraphCASE-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.4.tar", last modified: Fri May 26 07:15:42 2023, max compression
+gzip compressed data, was "GraphCASE-0.0.5.tar", last modified: Fri Jun  2 14:11:57 2023, max compression
```

## Comparing `GraphCASE-0.0.4.tar` & `GraphCASE-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.102336 GraphCASE-0.0.4/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.099966 GraphCASE-0.0.4/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.4/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.4/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11493 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    15634 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     2585 2022-09-26 09:14:26.000000 GraphCASE-0.0.4/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7511 2022-09-23 08:42:42.000000 GraphCASE-0.0.4/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    13470 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    12802 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/position_manager.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.101554 GraphCASE-0.0.4/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-05-26 07:15:42.000000 GraphCASE-0.0.4/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.4/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-05-26 07:15:42.101979 GraphCASE-0.0.4/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.4/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-05-26 07:15:42.102454 GraphCASE-0.0.4/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.543315 GraphCASE-0.0.5/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.539535 GraphCASE-0.0.5/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.5/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.5/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11515 2023-06-02 10:58:22.000000 GraphCASE-0.0.5/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    15818 2023-06-02 13:31:05.000000 GraphCASE-0.0.5/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     3867 2023-06-02 13:25:09.000000 GraphCASE-0.0.5/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7979 2023-06-02 13:29:34.000000 GraphCASE-0.0.5/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13464 2023-06-02 08:41:20.000000 GraphCASE-0.0.5/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    12754 2023-06-02 11:23:19.000000 GraphCASE-0.0.5/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.5/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-06-02 14:11:57.542421 GraphCASE-0.0.5/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-02 14:11:56.000000 GraphCASE-0.0.5/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-06-02 14:11:57.000000 GraphCASE-0.0.5/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-06-02 14:11:56.000000 GraphCASE-0.0.5/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-06-02 14:11:57.000000 GraphCASE-0.0.5/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.5/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-06-02 14:11:57.542882 GraphCASE-0.0.5/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.5/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-06-02 14:11:57.543450 GraphCASE-0.0.5/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-06-02 14:11:23.000000 GraphCASE-0.0.5/setup.py
```

### Comparing `GraphCASE-0.0.4/GAE/dataFeeder.py` & `GraphCASE-0.0.5/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.4/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.5/GAE/data_feeder_graphframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,18 @@
 from pathlib import Path
 import csv
 from pyspark import SparkContext, SparkConf
 from pyspark.sql import SparkSession
 from pyspark.sql.window import Window
 from pyspark.sql import functions as F
 
-if 'spark' not in (locals() or globals()):
-    conf = SparkConf().setAppName('appName').setMaster('local')
-    sc = SparkContext(conf=conf)
-    spark = SparkSession(sc)
-
+# if 'spark' not in (locals() or globals()):
+#     conf = SparkConf().setAppName('appName').setMaster('local')
+#     sc = SparkContext(conf=conf)
+#     spark = SparkSession(sc)s
 class DataFeederGraphFrames:
     """
     This class reads a node and edge dataframe and covert this to
     the samples for training the GraphCase algorithm.
     """
     def __init__(
         self, G, neighb_size=3, batch_size=3, val_fraction=0.3, verbose=False,
@@ -162,15 +161,15 @@
             .withColumn('features', F.concat(F.col('features'), F.col('dummy_edge_features')))
             .orderBy('id')
         )
         sample = np.array(agg_edges.select('sample').collect())
         features = np.array(agg_edges.select('features').collect(), dtype=np.float32)
 
         #add dummy id
-        sample = np.vstack([np.squeeze(sample, 1), [self.dummy_id] * 3])
+        sample = np.vstack([np.squeeze(sample, 1), [self.dummy_id] * self.neighb_size])
         features = np.vstack(
             [np.squeeze(features, 1),
              np.array([[[0] * len(self.edge_labels)] * self.neighb_size])
             ])
 
         return (sample, features.astype(np.float32))
```

### Comparing `GraphCASE-0.0.4/GAE/data_feeder_nx.py` & `GraphCASE-0.0.5/GAE/data_feeder_nx.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.4/GAE/graph_case_controller.py` & `GraphCASE-0.0.5/GAE/graph_case_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,15 +323,15 @@
             **train_dict
         )
         return history
 
 
     def get_l1_structure(self, node_id, graph=None, verbose=None, show_graph=False,
                          node_label=None, get_pyvis=False, deduplicate=True,
-                         delta=0.0001, dummy=0):
+                         delta=0.0001, dummy=0, fraction_sim=1.0):
         """
         Retrieve the input layer and corresponding sampled graph of the local neighbourhood.
 
         Args:
             node_id:    id of the node for which the input layer is calculated
             graph:      graph used for sampling. If no graph is specified then the current graph
                         is used.
@@ -345,27 +345,27 @@
             self.verbose = verbose
 
         if graph is not None:
             self.sampler = self.__init_sampler(graph, self.val_fraction)
 
         inputlayer, _ = self.sampler.get_input_layer([node_id], hub=1)
         target = self.sampler.get_features(node_id)
-        graph_rec = GraphReconstructor(deduplicate=deduplicate, delta=delta, dummy=dummy)
-        recon_graph = graph_rec.reconstruct_graph(target, inputlayer, self.support_size)
+        graph_rec = GraphReconstructor(deduplicate=deduplicate, delta=delta, dummy=dummy, fraction_sim=fraction_sim)
+        recon_graph = graph_rec.reconstruct_graph(target, inputlayer, self.support_size, pos_encoding_size=self.sampler.pos_enc_length)
 
         if show_graph:
             graph_rec.show_graph(recon_graph, node_label=node_label)
 
         if get_pyvis:
             nt = graph_rec.show_pyvis(recon_graph, node_label=node_label)
             return inputlayer, recon_graph, nt
 
         return inputlayer, recon_graph
 
-    def decode(self, embedding, incl_graph=None, delta=0.0001, dummy=0, deduplicate=True):
+    def decode(self, embedding, incl_graph=None, delta=0.0001, dummy=0, deduplicate=True, fraction_sim=1.0):
         """
         Decodes the given embedding into a node and local neighbourhood.
         Args:
             embedding:  Embedding of the node
             incl_graph :{None | pyvis | graph }
             delta:      Min difference between reconstructed feature value and dummy value. Nodes
                         with a smaller difference are considered dummy nodes and are removed.
@@ -376,16 +376,16 @@
         """
         feat_out, df_out = self.model.decode(embedding)
         # create dummy feat_out in case hub0 features are not included.
         if feat_out is None:
             feat_out = tf.constant([1,1,len(self.encoder_labels)])
 
         if incl_graph is not None:
-            graph_rec = GraphReconstructor(delta=delta, dummy=dummy, deduplicate=deduplicate)
-            recon_graph = graph_rec.reconstruct_graph(feat_out, df_out, self.support_size)
+            graph_rec = GraphReconstructor(delta=delta, dummy=dummy, deduplicate=deduplicate, fraction_sim=fraction_sim)
+            recon_graph = graph_rec.reconstruct_graph(feat_out, df_out, self.support_size, pos_encoding_size=self.sampler.pos_enc_length)
 
         if incl_graph == 'graph':
             return feat_out, df_out, recon_graph
 
         if incl_graph == 'pyvis':
             nt = graph_rec.show_pyvis(recon_graph)
             return feat_out, df_out, nt
```

### Comparing `GraphCASE-0.0.4/GAE/graph_reconstructor.py` & `GraphCASE-0.0.5/GAE/graph_reconstructor.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,51 +13,54 @@
 from pyvis import network as net
 
 class GraphReconstructor:
     """
     Class for reconstruction the sampled local neighbourhood into a graph based on the inputlayer
     of the encoder or outputlayer of the decoder. The reconstructed graph is a networkx graph.
     """
-    def __init__(self, deduplicate=True, delta=0.0001, dummy=0):
+    def __init__(self, deduplicate=True, delta=0.0001, dummy=0, fraction_sim=1.0):
         self.node_dim = 0  # dimension of the node labels
         self.edge_dim = 0  # dimension of the edge labels
         self.support_size = [0] # number of samples per layer
         self.layers = 0  # number of layers
         self.deduplicate = deduplicate
         self.delta = delta
+        self.fraction_sim = fraction_sim  # fraction of node dimensions with similar values when determining if node is same.
         self.dummy = [dummy]
         self.node_dict = None
 
-    def reconstruct_graph(self, target, inputlayer, support_size):
+    def reconstruct_graph(self, target, inputlayer, support_size, pos_encoding_size=0):
         """
         Reconstrucs the samples local neighbourhood into a graph based on the inputlayer
         of the encoder or outputlayer of the decoder. The reconstructed graph is a networkx graph.
 
         Args:
             target: numpy array with the features of the target node.
             inputLayer: 2-d numpy array containing the sampled feature and edge values.
             support_size: list containing the number of samples per layer.
 
         Returns:
             graphx graph consisting of the sampled nodes
         """
 
         self.node_dim = target.shape[-1]
-        self.dummy = self.dummy * self.node_dim
-        self.edge_dim = tf.shape(inputlayer)[2].numpy() - self.node_dim
+        self.dummy = self.dummy * (self.node_dim + pos_encoding_size)
+        self.edge_dim = tf.shape(inputlayer)[2].numpy() - self.node_dim - pos_encoding_size
         self.support_size = support_size
         self.layers = len(support_size)
+        self.pos_encoding_size = pos_encoding_size
         self.node_dict = np.zeros((self.layers, self.__get_switch_count(self.layers)), dtype=int)
 
         block_size = self.layers - 1 + self.support_size[-1]
         blocks = tf.shape(inputlayer)[1].numpy() / block_size  # number of blocks
 
         graph = nx.DiGraph()
-        parent_feat = dict([('feat'+str(i[0]), t) for i, t in np.ndenumerate(target.numpy().flatten())])
-        # dict([('feat'+str(i), t) for i, t in enumerate(target.numpy().flatten())])
+        root_encoding = [1]+[0]*(pos_encoding_size-1)
+        root_features = target.numpy().flatten().tolist()
+        parent_feat = dict([('feat'+str(i), t) for i, t in enumerate(root_features + root_encoding)])
         graph.add_node(1, **parent_feat)  # node id 0 is reserved for dummy
         for block_nr in range(int(blocks)):
             start_row = block_nr * block_size
             block = inputlayer[:, start_row : start_row + block_size, :]
             self.__process_blocks(graph, 1, block, 1, block_nr/ blocks)
 
         return graph
@@ -87,43 +90,46 @@
             for i in range(tf.shape(block)[1].numpy()):
                 self.__add_node_edge(graph, parent, block[:, i:i+1, :], is_incoming)
 
     def __get_switch_count(self, layer):
         return np.prod(self.support_size[:layer - 1]) * 2 ** layer
 
     def __add_node_edge(self, graph, parent, node_edge, is_incoming=True):
+        pos_enc = node_edge[0, 0, 0:self.pos_encoding_size]
         node = node_edge[0, 0, -self.node_dim:]
-        edge = node_edge[0, 0, 0:self.node_dim]
+        node = np.concatenate([node, pos_enc], axis=0)
+        edge = node_edge[0, 0, self.pos_encoding_size:self.pos_encoding_size + self.node_dim]
+        
         node_id = self.__add_node(graph, node)
         if node_id != 0: #  node is not a dummy node
             edge_feat = dict([('edge_feat'+str(i), t) for i, t in enumerate(edge.numpy())])
             if is_incoming:
                 graph.add_edge(node_id, parent, **edge_feat)
             else:
                 graph.add_edge(parent, node_id, **edge_feat)
         return node_id
 
     def __add_node(self, graph, node):
         new_id = graph.number_of_nodes() + 1
 
         # check if node matches dummy node.
-        equal_count = len([i for i, j in zip(node.numpy(), self.dummy) if abs(i - j) < self.delta])
-        if equal_count == self.node_dim:
+        equal_count = len([i for i, j in zip(node, self.dummy) if abs(i - j) < self.delta])
+        if equal_count >= node.shape[0] * self.fraction_sim:
             return 0
 
         # check if node is already part of the graph.
         if self.deduplicate:
             for u in graph.nodes(data=True):
                 u_feat = [v for k, v in sorted(u[1].items(), key=lambda tup: int(tup[0][4:]))]
-                count = len([i for i, j in zip(node.numpy(), u_feat) if abs(i - j) < self.delta])
-                if count == self.node_dim:
+                count = len([i for i, j in zip(node, u_feat) if abs(i - j) < self.delta])
+                if count >= node.shape[0] * self.fraction_sim:
                     return u[0]
 
         # add node to graph.
-        node_feat = dict([('feat'+str(i), t) for i, t in enumerate(node.numpy().flatten())])
+        node_feat = dict([('feat'+str(i), t) for i, t in enumerate(node.flatten())])
         graph.add_node(new_id, **node_feat)
         return new_id
 
     @staticmethod
     def show_graph(graph, node_label=None, ax=None):
         """plots the graph in plotly
         """
```

### Comparing `GraphCASE-0.0.4/GAE/input_layer_constructor.py` & `GraphCASE-0.0.5/GAE/input_layer_constructor.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,20 @@
         """
         train_data = self.data_feeder.get_train_samples()
         train_data = train_data.map(lambda x: (self.get_features(x), self.get_input_layer(x, hub=1)))
         # return train_data.map(lambda x, i: ((x, i[0]), (x, i[0]), (1, 1)))
         return train_data.map(lambda x, i: ((x, i[0]), (x, i[0]), (1, tf.math.maximum(i[1], 0.1))))
 
     def get_supervised_train_samples(self):
-        return self.__get_supervised_samples(self.data_feeder.get_train_samples)
+        return self._get_supervised_samples(self.data_feeder.get_train_samples)
 
     def get_supervised_val_samples(self):
-        return self.__get_supervised_samples(self.data_feeder.get_val_samples)
+        return self._get_supervised_samples(self.data_feeder.get_val_samples)
 
-    def __get_supervised_samples(self, feeder):
+    def _get_supervised_samples(self, feeder):
         data = feeder()
         data = data.map(lambda x: (x, tf.nn.embedding_lookup(self.data_feeder.lbls, x)))
         data = data.map(lambda x, y: (self.get_features(x), self.get_input_layer(x, hub=1), y))
         return data.map(lambda x, i, y: ((x, i[0]), y, (1, i[1])))
 
     def get_val_samples(self):
         val_data = self.data_feeder.get_val_samples()
@@ -115,16 +115,16 @@
             a tuple with 1) a tensor of the features for the specified hub and 2) a tensor with
             the weights for the specified hub.
         """
         # extract and store node_ids as the rootnodes for the position encoding lookup
         if hub == 1 and self.pos_enc_cls is not None:
             self.root_nodes = tf.multiply(node_ids, self.factor)  # Multiple with factor
 
-        next_in_feat, next_in_weight = self.__get_next_hub(node_ids, hub, 'in', feat, weight)
-        next_out_feat, next_out_weight = self.__get_next_hub(node_ids, hub, 'out', feat, weight)
+        next_in_feat, next_in_weight = self._get_next_hub(node_ids, hub, 'in', feat, weight)
+        next_out_feat, next_out_weight = self._get_next_hub(node_ids, hub, 'out', feat, weight)
 
         if feat is not None:  # is not the first iteration
             if hub == len(self.support_size):  # is not the last iteration
                 feat = tf.concat([feat, next_in_feat, feat, next_out_feat], -2)
 
                 shape = tf.shape(weight)
                 head = None
@@ -164,15 +164,15 @@
 
         else:
             feat = tf.concat([next_in_feat, next_out_feat], -2)
             weight = tf.concat([next_in_weight, next_out_weight], -1)
 
         return feat, weight
 
-    def __get_next_hub(self, node_ids, hub, direction, feat, weight):
+    def _get_next_hub(self, node_ids, hub, direction, feat, weight):
         """
         Retrieves the features including edge weights for the specified hub and direction.
         The features are combined with the features of the lower hubs.
 
         Args:
             node_ids:   A tensor containing the node_ids for which the featurs need to be
                         retrieved.
```

### Comparing `GraphCASE-0.0.4/GAE/model.py` & `GraphCASE-0.0.5/GAE/model.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.4/GAE/position_manager.py` & `GraphCASE-0.0.5/GAE/position_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,33 +4,29 @@
 import networkx as nx
 import pygsp as gsp
 
 class PositionManager:
     """class that calculate the positional encoding that is used in the input_layer Z
     """   
     def __init__(self, G, in_sample, out_sample, hubs):
-        self.G = G
         self.in_sample = in_sample
         self.out_sample = out_sample
         self.hubs = hubs
-        
+        self.number_of_nodes = out_sample.shape[0]
+
         # rescaling factor used when creating single pos dic
-        self.factor = 10**(int(math.log10(G.number_of_nodes()))+1)
-        
+        self.factor = 10**(int(math.log10(self.number_of_nodes))+1)
+  
         start = time.time()
         print(f"start creating position dict at {start}")
         self.pos_dicts = self.create_pos_dicts()
         self.single_pos_dict = self.create_single_pos_dict(self.pos_dicts)
         end = time.time()
         print(f"pos dictionary created in {end-start} second: {end}")
-        
-        
-         
-        
-    
+
     @staticmethod
     def select_first_embeding(emb1, emb2):
         """Compares two positions embeddings and select the one with the shortest path to the root node.
 
         Args:
             emb1 (array<float>): position embeddding 1
             emb2 (array<float>): position embeddding 1
@@ -64,15 +60,15 @@
             out_sample (_type_): sampled outgoing neighbors per node id
             pos_dic (_type_): dictionary with the positional embedding for all nodes in the local neighborhood of the root node 
             prefix (_type_): first part of the position embedding that is fixed
             hubs (_type_): total number of hubs in the local neighborhood
             current_hub (_type_): current hub.
         """    
         # process the incoming sampled nodes
-        default = [1] * (self.hubs * 2 + 1)  # default value for position embedding when not yet in dict.
+        default = [1] * (self.hubs * 2 + 2)  # default value for position embedding when not yet in dict.
         sample = self.in_sample[id]
         in_lenght = (self.hubs - current_hub) * 2 + 1
         for i, nn in enumerate(sample):
             # update position embedding with the lowest value as this value has the shortest path to the root node
             # position encoding is prefix + 1 + 0 for remaining part of the vector
             this_position = prefix + [1 - i / sample.shape[0]] + [0] * in_lenght
             pos_emb =  self.select_first_embeding(pos_dic.get(nn, default), this_position)
@@ -99,24 +95,24 @@
         and the value of the inner dicts is the positional encoding of that node in related to the root node.
 
         Returns:
             _type_: dict with dict containing root node, local node and value the positional enconding.
         """
         pos_dicts = {}  # dictionary to hold the dictonaries for all nodes
         
-        for id in list(self.G.nodes()) + [self.G.number_of_nodes()]:  # for all node ids + dummy node id
+        for id in range(self.number_of_nodes):  # for all node ids + dummy node id
             # instantiate dictionary for position embedding for this root node.
             pos_dic = {}
             current_hub = 1
             prefix = [1.0]  # only the first dimension of the embedding is set to 1
             self.add_layers_to_pos_dic(id, pos_dic, prefix, current_hub)
         
             # overwrite the position embedding for the root 
             pos_dic[id] = [1.0] + [0] * (self.hubs * 2)
-            pos_dic[self.G.number_of_nodes() - 1] = [0] * (self.hubs * 2 + 1)
+            pos_dic[self.number_of_nodes - 1] = [0] * (self.hubs * 2 + 1)
             
             # add dict to pos_dicts
             pos_dicts[id] = pos_dic
             
         return pos_dicts
         
     def create_single_pos_dict(self, pos_dicts):
```

### Comparing `GraphCASE-0.0.4/GAE/transformation_layer.py` & `GraphCASE-0.0.5/GAE/transformation_layer.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.4/LICENSE.txt` & `GraphCASE-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.4/README.md` & `GraphCASE-0.0.5/README.md`

 * *Files identical despite different names*

