# Comparing `tmp/chemfunc-1.0.2.tar.gz` & `tmp/chemfunc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemfunc-1.0.2.tar", last modified: Thu Jun  1 19:02:55 2023, max compression
+gzip compressed data, was "chemfunc-1.0.3.tar", last modified: Fri Jun  2 15:51:40 2023, max compression
```

## Comparing `chemfunc-1.0.2.tar` & `chemfunc-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.337622 chemfunc-1.0.2/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.2/LICENSE
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 19:02:55.337757 chemfunc-1.0.2/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.2/README.md
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.335330 chemfunc-1.0.2/chemfunc/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/__init__.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-01 19:01:59.000000 chemfunc-1.0.2/chemfunc/_version.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/canonicalize_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/chemical_diversity.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/cluster_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/compute_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.2/chemfunc/constants.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/deduplicate_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/filter_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/main.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.2/chemfunc/measure_experimental_reproducibility.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4557 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/molecular_fingerprints.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.2/chemfunc/molecular_properties.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/molecular_similarities.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     3387 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/nearest_neighbor.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.2/chemfunc/plot_property_distribution.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/plot_tsne.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/regression_to_classification.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/sample_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/sdf_to_smiles.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/select_from_clusters.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.2/chemfunc/smiles_to_svg.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.2/chemfunc/utils.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.2/chemfunc/visualize_molecules.py
--rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.2/chemfunc/visualize_reactions.py
-drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-01 19:02:55.337341 chemfunc-1.0.2/chemfunc.egg-info/
--rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/PKG-INFO
--rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/SOURCES.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/dependency_links.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/entry_points.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/requires.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-01 19:02:55.000000 chemfunc-1.0.2/chemfunc.egg-info/top_level.txt
--rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-01 19:02:55.338273 chemfunc-1.0.2/setup.cfg
--rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.2/setup.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.232228 chemfunc-1.0.3/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1069 2023-03-07 02:37:32.000000 chemfunc-1.0.3/LICENSE
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-02 15:51:40.232379 chemfunc-1.0.3/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     5644 2023-05-25 21:30:47.000000 chemfunc-1.0.3/README.md
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.228368 chemfunc-1.0.3/chemfunc/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2014 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/__init__.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      176 2023-06-02 15:51:11.000000 chemfunc-1.0.3/chemfunc/_version.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2841 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/canonicalize_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2007 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/chemical_diversity.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1583 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/cluster_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1520 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/compute_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      137 2023-03-07 00:44:25.000000 chemfunc-1.0.3/chemfunc/constants.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      877 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/deduplicate_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4002 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/filter_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1199 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/main.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2643 2023-05-23 20:59:02.000000 chemfunc-1.0.3/chemfunc/measure_experimental_reproducibility.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4600 2023-06-01 23:18:30.000000 chemfunc-1.0.3/chemfunc/molecular_fingerprints.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     4093 2023-06-01 19:01:48.000000 chemfunc-1.0.3/chemfunc/molecular_properties.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     8551 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/molecular_similarities.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     3274 2023-06-02 15:22:59.000000 chemfunc-1.0.3/chemfunc/nearest_neighbor.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1659 2023-05-23 21:00:59.000000 chemfunc-1.0.3/chemfunc/plot_property_distribution.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6620 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/plot_tsne.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1672 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/regression_to_classification.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1654 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/sample_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1956 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/sdf_to_smiles.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1223 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/select_from_clusters.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      878 2023-05-23 21:04:54.000000 chemfunc-1.0.3/chemfunc/smiles_to_svg.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2129 2023-05-23 18:54:45.000000 chemfunc-1.0.3/chemfunc/utils.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2514 2023-05-23 23:24:43.000000 chemfunc-1.0.3/chemfunc/visualize_molecules.py
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     2141 2023-05-23 21:10:47.000000 chemfunc-1.0.3/chemfunc/visualize_reactions.py
+drwxr-xr-x   0 kyleswanson   (501) staff       (20)        0 2023-06-02 15:51:40.231846 chemfunc-1.0.3/chemfunc.egg-info/
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     6386 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/PKG-INFO
+-rw-r--r--   0 kyleswanson   (501) staff       (20)      974 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        1 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       48 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/entry_points.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       93 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/requires.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)        9 2023-06-02 15:51:40.000000 chemfunc-1.0.3/chemfunc.egg-info/top_level.txt
+-rw-r--r--   0 kyleswanson   (501) staff       (20)       79 2023-06-02 15:51:40.232933 chemfunc-1.0.3/setup.cfg
+-rw-r--r--   0 kyleswanson   (501) staff       (20)     1612 2023-05-23 23:24:43.000000 chemfunc-1.0.3/setup.py
```

### Comparing `chemfunc-1.0.2/LICENSE` & `chemfunc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/PKG-INFO` & `chemfunc-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.2.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.3.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.2/README.md` & `chemfunc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/__init__.py` & `chemfunc-1.0.3/chemfunc/__init__.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/canonicalize_smiles.py` & `chemfunc-1.0.3/chemfunc/canonicalize_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/chemical_diversity.py` & `chemfunc-1.0.3/chemfunc/chemical_diversity.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/cluster_molecules.py` & `chemfunc-1.0.3/chemfunc/cluster_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/compute_properties.py` & `chemfunc-1.0.3/chemfunc/compute_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/deduplicate_smiles.py` & `chemfunc-1.0.3/chemfunc/deduplicate_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/filter_molecules.py` & `chemfunc-1.0.3/chemfunc/filter_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/main.py` & `chemfunc-1.0.3/chemfunc/main.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/measure_experimental_reproducibility.py` & `chemfunc-1.0.3/chemfunc/measure_experimental_reproducibility.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/molecular_fingerprints.py` & `chemfunc-1.0.3/chemfunc/molecular_fingerprints.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from rdkit import Chem
 from rdkit.DataStructs import ConvertToNumpyArray
 from rdkit.Chem import AllChem
 from tqdm import tqdm
 
 from chemfunc.constants import Molecule
 
+# Fix for NumPy >= 1.24.0
+np.float = float
 
 FingerprintGenerator = Callable[[Molecule], np.ndarray]
 FINGERPRINT_GENERATOR_REGISTRY = {}
 MORGAN_RADIUS = 2
 MORGAN_NUM_BITS = 2048
```

### Comparing `chemfunc-1.0.2/chemfunc/molecular_properties.py` & `chemfunc-1.0.3/chemfunc/molecular_properties.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/molecular_similarities.py` & `chemfunc-1.0.3/chemfunc/molecular_similarities.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/nearest_neighbor.py` & `chemfunc-1.0.3/chemfunc/nearest_neighbor.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from chemfunc.constants import SMILES_COLUMN
 from chemfunc.molecular_similarities import get_similarity_function
 
 
 def nearest_neighbor(
         data_path: Path,
         reference_data_path: Path,
-        metrics: tuple[Literal['tanimoto', 'mcs', 'tversky'], ...] = ('tanimoto',),
+        metric: Literal['tanimoto', 'mcs', 'tversky'] = 'tanimoto',
         save_path: Path | None = None,
         smiles_column: str = SMILES_COLUMN,
         reference_smiles_column: str | None = None,
         reference_name: str | None = None
 ) -> None:
     """Given a dataset, computes the nearest neighbor molecule by Tanimoto similarity in a second dataset.
 
     :param data_path: Path to CSV file containing data with SMILES whose neighbors are to be computed.
     :param reference_data_path: Path to CSV file containing reference SMILES which will be the neighbors of data_path.
-    :param metrics: Metrics to use when computing similarity.
-                    tanimoto: Tanimoto similarity using Morgan fingerprint.
-                    mcs: Maximum common substructure as a proportion of the number of atoms in the reference molecule.
-                    tversky: Tversky index with alpha = 0 and beta = 1, i.e., the proportion of reference substructures
-                    in the molecule.
+    :param metric: Metric to use when computing similarity.
+                   tanimoto: Tanimoto similarity using Morgan fingerprint.
+                   mcs: Maximum common substructure as a proportion of the number of atoms in the reference molecule.
+                   tversky: Tversky index with alpha = 0 and beta = 1, i.e., the proportion of reference substructures
+                   in the molecule.
     :param save_path: Where the data with the neighbor info should be saved (defaults to data_path).
     :param smiles_column: Name of the column in data_path containing SMILES.
     :param reference_smiles_column: Name of the column in reference_data_path containing SMILES.
                                     If None, then smiles_column is used.
     :param reference_name: Name of the reference data when naming the new columns with neighbor info.
     """
     # Set save path
@@ -45,31 +45,30 @@
     data = pd.read_csv(data_path)
     reference_data = pd.read_csv(reference_data_path)
 
     # Sort reference data and drop duplicates
     reference_data.drop_duplicates(subset=reference_smiles_column, inplace=True)
     reference_data.sort_values(by=reference_smiles_column, ignore_index=True, inplace=True)
 
-    for metric in metrics:
-        print(f'Computing similarities using {metric} metric')
-        similarities = get_similarity_function(metric)(
-            data[smiles_column],
-            reference_data[reference_smiles_column]
-        )
-
-        print('Finding minimum distance SMILES')
-        prefix = f'{f"{reference_name}_" if reference_name is not None else ""}{metric}_'
-
-        max_similarity_indices = np.argmax(similarities, axis=1)
-
-        data[f'{prefix}nearest_neighbor'] = [
-            reference_data[reference_smiles_column][max_similarity_index]
-            for max_similarity_index in max_similarity_indices
-        ]
-        data[f'{prefix}nearest_neighbor_similarity'] = [
-            similarities[i, max_similarity_index]
-            for i, max_similarity_index in enumerate(max_similarity_indices)
-        ]
+    print(f'Computing similarities using {metric} metric')
+    similarities = get_similarity_function(metric)(
+        data[smiles_column],
+        reference_data[reference_smiles_column]
+    )
+
+    print('Finding minimum distance SMILES')
+    prefix = f'{f"{reference_name}_" if reference_name is not None else ""}{metric}_'
+
+    max_similarity_indices = np.argmax(similarities, axis=1)
+
+    data[f'{prefix}nearest_neighbor'] = [
+        reference_data[reference_smiles_column][max_similarity_index]
+        for max_similarity_index in max_similarity_indices
+    ]
+    data[f'{prefix}nearest_neighbor_similarity'] = [
+        similarities[i, max_similarity_index]
+        for i, max_similarity_index in enumerate(max_similarity_indices)
+    ]
 
     print('Saving')
     save_path.parent.mkdir(parents=True, exist_ok=True)
     data.to_csv(save_path, index=False)
```

### Comparing `chemfunc-1.0.2/chemfunc/plot_property_distribution.py` & `chemfunc-1.0.3/chemfunc/plot_property_distribution.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/plot_tsne.py` & `chemfunc-1.0.3/chemfunc/plot_tsne.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/regression_to_classification.py` & `chemfunc-1.0.3/chemfunc/regression_to_classification.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/sample_molecules.py` & `chemfunc-1.0.3/chemfunc/sample_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/sdf_to_smiles.py` & `chemfunc-1.0.3/chemfunc/sdf_to_smiles.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/select_from_clusters.py` & `chemfunc-1.0.3/chemfunc/select_from_clusters.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/smiles_to_svg.py` & `chemfunc-1.0.3/chemfunc/smiles_to_svg.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/utils.py` & `chemfunc-1.0.3/chemfunc/utils.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/visualize_molecules.py` & `chemfunc-1.0.3/chemfunc/visualize_molecules.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc/visualize_reactions.py` & `chemfunc-1.0.3/chemfunc/visualize_reactions.py`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/chemfunc.egg-info/PKG-INFO` & `chemfunc-1.0.3/chemfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: chemfunc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Chem Func
 Home-page: https://github.com/swansonk14/chemfunc
-Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.2.tar.gz
+Download-URL: https://github.com/swansonk14/chemfunc/v_1.0.3.tar.gz
 Author: Kyle Swanson
 Author-email: swansonk.14@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/swansonk14/chemfunc
 Project-URL: PyPi, https://pypi.org/project/chemfunc/
 Keywords: computational chemistry
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chemfunc-1.0.2/chemfunc.egg-info/SOURCES.txt` & `chemfunc-1.0.3/chemfunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chemfunc-1.0.2/setup.py` & `chemfunc-1.0.3/setup.py`

 * *Files identical despite different names*

