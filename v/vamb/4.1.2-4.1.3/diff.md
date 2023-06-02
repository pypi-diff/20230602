# Comparing `tmp/vamb-4.1.2.tar.gz` & `tmp/vamb-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vamb-4.1.2.tar", last modified: Sun May 28 13:28:37 2023, max compression
+gzip compressed data, was "vamb-4.1.3.tar", last modified: Fri Jun  2 10:43:09 2023, max compression
```

## Comparing `vamb-4.1.2.tar` & `vamb-4.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-05-28 13:28:37.887924 vamb-4.1.2/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-05-22 09:20:29.000000 vamb-4.1.2/LICENSE
--rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-05-22 09:20:29.000000 vamb-4.1.2/MANIFEST.in
--rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-05-28 13:28:37.887924 vamb-4.1.2/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-05-22 09:20:29.000000 vamb-4.1.2/README.md
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1007 2023-05-28 13:17:57.000000 vamb-4.1.2/pyproject.toml
--rw-r--r--   0 jakni     (1000) jakni     (1000)      146 2023-05-28 13:28:37.887924 vamb-4.1.2/setup.cfg
--rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-05-22 09:20:29.000000 vamb-4.1.2/setup.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-05-28 13:28:37.884590 vamb-4.1.2/src/
--rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-05-22 09:20:29.000000 vamb-4.1.2/src/_vambtools.pyx
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-05-28 13:28:37.884590 vamb-4.1.2/test/
--rw-r--r--   0 jakni     (1000) jakni     (1000)    12734 2023-05-22 10:18:33.000000 vamb-4.1.2/test/test_benchmark.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     4879 2023-05-22 10:18:33.000000 vamb-4.1.2/test/test_cluster.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7231 2023-05-22 10:18:33.000000 vamb-4.1.2/test/test_encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     3392 2023-05-22 10:18:33.000000 vamb-4.1.2/test/test_parsebam.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     3841 2023-05-22 10:18:33.000000 vamb-4.1.2/test/test_parsecontigs.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     5604 2023-05-22 09:20:29.000000 vamb-4.1.2/test/test_results.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    18325 2023-05-22 09:20:29.000000 vamb-4.1.2/test/test_vambtools.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     1425 2023-05-22 09:20:29.000000 vamb-4.1.2/test/testtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-05-28 13:28:37.887924 vamb-4.1.2/vamb/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      941 2023-05-28 13:23:28.000000 vamb-4.1.2/vamb/__init__.py
--rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42905 2023-05-23 13:46:15.000000 vamb-4.1.2/vamb/__main__.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    17951 2023-05-22 10:18:33.000000 vamb-4.1.2/vamb/aamb_encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    25117 2023-05-22 09:20:29.000000 vamb-4.1.2/vamb/benchmark.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    19362 2023-05-22 10:53:07.000000 vamb-4.1.2/vamb/cluster.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    22117 2023-05-22 10:18:33.000000 vamb-4.1.2/vamb/encode.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.1.2/vamb/kernel.npz
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7905 2023-05-22 10:18:33.000000 vamb-4.1.2/vamb/parsebam.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)     7041 2023-05-22 14:31:39.000000 vamb-4.1.2/vamb/parsecontigs.py
--rw-r--r--   0 jakni     (1000) jakni     (1000)    21213 2023-05-22 10:34:59.000000 vamb-4.1.2/vamb/vambtools.py
-drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-05-28 13:28:37.887924 vamb-4.1.2/vamb.egg-info/
--rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/PKG-INFO
--rw-r--r--   0 jakni     (1000) jakni     (1000)      601 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/SOURCES.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/dependency_links.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/entry_points.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/requires.txt
--rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-05-28 13:28:37.000000 vamb-4.1.2/vamb.egg-info/top_level.txt
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-06-02 10:43:09.640145 vamb-4.1.3/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1081 2023-05-22 09:20:29.000000 vamb-4.1.3/LICENSE
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       24 2023-05-22 09:20:29.000000 vamb-4.1.3/MANIFEST.in
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-06-02 10:43:09.640145 vamb-4.1.3/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    15245 2023-05-22 09:20:29.000000 vamb-4.1.3/README.md
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1007 2023-05-28 13:17:57.000000 vamb-4.1.3/pyproject.toml
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      146 2023-06-02 10:43:09.640145 vamb-4.1.3/setup.cfg
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      128 2023-05-22 09:20:29.000000 vamb-4.1.3/setup.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-06-02 10:43:09.636812 vamb-4.1.3/src/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     2846 2023-06-01 14:11:40.000000 vamb-4.1.3/src/_vambtools.pyx
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-06-02 10:43:09.636812 vamb-4.1.3/test/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    12734 2023-05-22 10:18:33.000000 vamb-4.1.3/test/test_benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     4934 2023-06-02 10:40:37.000000 vamb-4.1.3/test/test_cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7231 2023-06-02 10:42:31.000000 vamb-4.1.3/test/test_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3392 2023-05-22 10:18:33.000000 vamb-4.1.3/test/test_parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     3841 2023-05-22 10:18:33.000000 vamb-4.1.3/test/test_parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     5604 2023-05-22 09:20:29.000000 vamb-4.1.3/test/test_results.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    18325 2023-05-22 09:20:29.000000 vamb-4.1.3/test/test_vambtools.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     1425 2023-05-22 09:20:29.000000 vamb-4.1.3/test/testtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-06-02 10:43:09.636812 vamb-4.1.3/vamb/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      941 2023-06-02 10:42:31.000000 vamb-4.1.3/vamb/__init__.py
+-rwxr-xr-x   0 jakni     (1000) jakni     (1000)    42905 2023-05-23 13:46:15.000000 vamb-4.1.3/vamb/__main__.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    17951 2023-05-22 10:18:33.000000 vamb-4.1.3/vamb/aamb_encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    25117 2023-05-22 09:20:29.000000 vamb-4.1.3/vamb/benchmark.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    19330 2023-06-02 10:40:37.000000 vamb-4.1.3/vamb/cluster.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    22117 2023-06-02 10:42:31.000000 vamb-4.1.3/vamb/encode.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    77187 2022-04-05 08:20:29.000000 vamb-4.1.3/vamb/kernel.npz
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7905 2023-05-22 10:18:33.000000 vamb-4.1.3/vamb/parsebam.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)     7041 2023-05-22 14:31:39.000000 vamb-4.1.3/vamb/parsecontigs.py
+-rw-r--r--   0 jakni     (1000) jakni     (1000)    21213 2023-06-01 14:11:32.000000 vamb-4.1.3/vamb/vambtools.py
+drwxr-xr-x   0 jakni     (1000) jakni     (1000)        0 2023-06-02 10:43:09.640145 vamb-4.1.3/vamb.egg-info/
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      101 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/PKG-INFO
+-rw-r--r--   0 jakni     (1000) jakni     (1000)      601 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/SOURCES.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        1 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/dependency_links.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/entry_points.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)       44 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/requires.txt
+-rw-r--r--   0 jakni     (1000) jakni     (1000)        5 2023-06-02 10:43:09.000000 vamb-4.1.3/vamb.egg-info/top_level.txt
```

### Comparing `vamb-4.1.2/LICENSE` & `vamb-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/README.md` & `vamb-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/pyproject.toml` & `vamb-4.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/src/_vambtools.pyx` & `vamb-4.1.3/src/_vambtools.pyx`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_benchmark.py` & `vamb-4.1.3/test/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_cluster.py` & `vamb-4.1.3/test/test_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
     # In the code, in __init__ of the cluster generator, the input matrix
     # is shuffled, and an index array is permuted to keep track of which
     # indices was which.
     # This depends on the implementation of shuffling and permute being
     # the same, which I test here.
     def test_shuffling(self):
+        seed = 0
         cp = self.data.copy()
-        np.random.RandomState(0).shuffle(cp)
-        indices = np.random.RandomState(0).permutation(len(cp))
+        np.random.Generator(np.random.PCG64(seed)).shuffle((cp))
+        indices = np.random.Generator(np.random.PCG64(seed)).permutation(len(cp))
         cplike = self.data[indices]
         self.assertTrue(np.all(cplike == cp))
 
     def test_basics(self):
         clstr = vamb.cluster.ClusterGenerator(self.data)
         self.assertIs(clstr, iter(clstr))
```

### Comparing `vamb-4.1.2/test/test_encode.py` & `vamb-4.1.3/test/test_encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_parsebam.py` & `vamb-4.1.3/test/test_parsebam.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_parsecontigs.py` & `vamb-4.1.3/test/test_parsecontigs.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_results.py` & `vamb-4.1.3/test/test_results.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/test_vambtools.py` & `vamb-4.1.3/test/test_vambtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/test/testtools.py` & `vamb-4.1.3/test/testtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/__init__.py` & `vamb-4.1.3/vamb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 3) Calculate a Composition of contigs using vamb.parsecontigs
 4) Create Abundance object from BAM files using vamb.parsebam
 5) Train autoencoder using vamb.encode
 6) Cluster latent representation using vamb.cluster
 7) Split bins using vamb.vambtools
 """
 
-__version__ = (4, 1, 2)
+__version__ = (4, 1, 3)
 
 from . import vambtools
 from . import parsebam
 from . import parsecontigs
 from . import cluster
 from . import benchmark
 from . import encode
```

### Comparing `vamb-4.1.2/vamb/__main__.py` & `vamb-4.1.3/vamb/__main__.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/aamb_encode.py` & `vamb-4.1.3/vamb/aamb_encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/benchmark.py` & `vamb-4.1.3/vamb/benchmark.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/cluster.py` & `vamb-4.1.3/vamb/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,16 +475,15 @@
         matrix = _torch.from_numpy(matrix)
 
     if not inplace:
         matrix = matrix.clone()
 
     # If any rows are kept all zeros, the distance function will return 0.5 to all points
     # inclusive itself, which can break the code in this module
-    matrix[matrix < 0] = 0
-    zeromask = matrix.max(dim=1).values == 0
+    zeromask = (matrix == 0).all(dim=1)
     matrix[zeromask] = 1 / matrix.shape[1]
     matrix /= matrix.norm(dim=1).reshape(-1, 1) * (2**0.5)
     return matrix
 
 
 def _calc_distances(matrix: _Tensor, index: int) -> _Tensor:
     "Return vector of cosine distances from rows of normalized matrix to given row."
```

### Comparing `vamb-4.1.2/vamb/encode.py` & `vamb-4.1.3/vamb/encode.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/kernel.npz` & `vamb-4.1.3/vamb/kernel.npz`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/parsebam.py` & `vamb-4.1.3/vamb/parsebam.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/parsecontigs.py` & `vamb-4.1.3/vamb/parsecontigs.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb/vambtools.py` & `vamb-4.1.3/vamb/vambtools.py`

 * *Files identical despite different names*

### Comparing `vamb-4.1.2/vamb.egg-info/SOURCES.txt` & `vamb-4.1.3/vamb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

