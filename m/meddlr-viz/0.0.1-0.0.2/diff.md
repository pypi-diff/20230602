# Comparing `tmp/meddlr-viz-0.0.1.tar.gz` & `tmp/meddlr-viz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meddlr-viz-0.0.1.tar", last modified: Wed May 31 19:58:04 2023, max compression
+gzip compressed data, was "meddlr-viz-0.0.2.tar", last modified: Fri Jun  2 04:15:28 2023, max compression
```

## Comparing `meddlr-viz-0.0.1.tar` & `meddlr-viz-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-05-31 19:58:04.594985 meddlr-viz-0.0.1/
--rw-r--r--   0 arjundd    (501) staff       (20)      507 2023-05-31 19:58:04.595067 meddlr-viz-0.0.1/PKG-INFO
--rw-r--r--   0 arjundd    (501) staff       (20)       14 2023-05-25 23:03:06.000000 meddlr-viz-0.0.1/README.md
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-05-31 19:58:04.593611 meddlr-viz-0.0.1/meddlr_viz/
--rw-r--r--   0 arjundd    (501) staff       (20)      144 2023-05-31 19:56:57.000000 meddlr-viz-0.0.1/meddlr_viz/__init__.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-05-31 19:58:04.594758 meddlr-viz-0.0.1/meddlr_viz/gui/
--rw-r--r--   0 arjundd    (501) staff       (20)      105 2023-05-31 19:57:19.000000 meddlr-viz-0.0.1/meddlr_viz/gui/__init__.py
--rw-r--r--   0 arjundd    (501) staff       (20)    14503 2023-05-31 19:57:44.000000 meddlr-viz-0.0.1/meddlr_viz/gui/perturbation.py
--rw-r--r--   0 arjundd    (501) staff       (20)     2251 2023-05-31 19:57:01.000000 meddlr-viz-0.0.1/meddlr_viz/utils.py
-drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-05-31 19:58:04.594456 meddlr-viz-0.0.1/meddlr_viz.egg-info/
--rw-r--r--   0 arjundd    (501) staff       (20)      507 2023-05-31 19:58:04.000000 meddlr-viz-0.0.1/meddlr_viz.egg-info/PKG-INFO
--rw-r--r--   0 arjundd    (501) staff       (20)      313 2023-05-31 19:58:04.000000 meddlr-viz-0.0.1/meddlr_viz.egg-info/SOURCES.txt
--rw-r--r--   0 arjundd    (501) staff       (20)        1 2023-05-31 19:58:04.000000 meddlr-viz-0.0.1/meddlr_viz.egg-info/dependency_links.txt
--rw-r--r--   0 arjundd    (501) staff       (20)       66 2023-05-31 19:58:04.000000 meddlr-viz-0.0.1/meddlr_viz.egg-info/requires.txt
--rw-r--r--   0 arjundd    (501) staff       (20)       11 2023-05-31 19:58:04.000000 meddlr-viz-0.0.1/meddlr_viz.egg-info/top_level.txt
--rw-r--r--   0 arjundd    (501) staff       (20)       72 2023-05-31 19:56:57.000000 meddlr-viz-0.0.1/pyproject.toml
--rw-r--r--   0 arjundd    (501) staff       (20)      558 2023-05-31 19:58:04.595405 meddlr-viz-0.0.1/setup.cfg
--rw-r--r--   0 arjundd    (501) staff       (20)     7068 2023-05-31 19:57:02.000000 meddlr-viz-0.0.1/setup.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-06-02 04:15:28.703884 meddlr-viz-0.0.2/
+-rw-r--r--   0 arjundd    (501) staff       (20)     2284 2023-06-02 04:15:28.703966 meddlr-viz-0.0.2/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)     1791 2023-06-01 07:43:48.000000 meddlr-viz-0.0.2/README.md
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-06-02 04:15:28.702529 meddlr-viz-0.0.2/meddlr_viz/
+-rw-r--r--   0 arjundd    (501) staff       (20)      144 2023-06-02 04:15:23.000000 meddlr-viz-0.0.2/meddlr_viz/__init__.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-06-02 04:15:28.703663 meddlr-viz-0.0.2/meddlr_viz/gui/
+-rw-r--r--   0 arjundd    (501) staff       (20)      105 2023-05-31 19:57:19.000000 meddlr-viz-0.0.2/meddlr_viz/gui/__init__.py
+-rw-r--r--   0 arjundd    (501) staff       (20)    14503 2023-05-31 19:57:44.000000 meddlr-viz-0.0.2/meddlr_viz/gui/perturbation.py
+-rw-r--r--   0 arjundd    (501) staff       (20)     2323 2023-06-02 04:15:23.000000 meddlr-viz-0.0.2/meddlr_viz/utils.py
+drwxr-xr-x   0 arjundd    (501) staff       (20)        0 2023-06-02 04:15:28.703348 meddlr-viz-0.0.2/meddlr_viz.egg-info/
+-rw-r--r--   0 arjundd    (501) staff       (20)     2284 2023-06-02 04:15:28.000000 meddlr-viz-0.0.2/meddlr_viz.egg-info/PKG-INFO
+-rw-r--r--   0 arjundd    (501) staff       (20)      313 2023-06-02 04:15:28.000000 meddlr-viz-0.0.2/meddlr_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)        1 2023-06-02 04:15:28.000000 meddlr-viz-0.0.2/meddlr_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)       66 2023-06-02 04:15:28.000000 meddlr-viz-0.0.2/meddlr_viz.egg-info/requires.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)       11 2023-06-02 04:15:28.000000 meddlr-viz-0.0.2/meddlr_viz.egg-info/top_level.txt
+-rw-r--r--   0 arjundd    (501) staff       (20)       72 2023-05-31 19:56:57.000000 meddlr-viz-0.0.2/pyproject.toml
+-rw-r--r--   0 arjundd    (501) staff       (20)      558 2023-06-02 04:15:28.704312 meddlr-viz-0.0.2/setup.cfg
+-rw-r--r--   0 arjundd    (501) staff       (20)     7068 2023-05-31 19:57:02.000000 meddlr-viz-0.0.2/setup.py
```

### Comparing `meddlr-viz-0.0.1/meddlr_viz/gui/perturbation.py` & `meddlr-viz-0.0.2/meddlr_viz/gui/perturbation.py`

 * *Files identical despite different names*

### Comparing `meddlr-viz-0.0.1/meddlr_viz/utils.py` & `meddlr-viz-0.0.2/meddlr_viz/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,19 +51,20 @@
             num_slices = f["kspace"].shape[0]
         for sl in range(num_slices):
             records.append({"path": path, "sl": sl})
 
     df = pd.DataFrame.from_records(records)
     df = mk.DataFrame.from_pandas(df)
     if defer:
-        df_load = mk.defer(df, _load_data)
+        df_load: mk.DataFrame = mk.defer(df, _load_data)
     else:
-        df_load = mk.map(df, _load_data)
-    # df = mk.concat([df, df_load], axis=1).drop("index")
-    df = df.merge(df_load, on="pkey")
+        df_load: mk.DataFrame = mk.map(df, _load_data)
+    df = mk.concat([df, df_load], axis=1).drop("index")
+
+    # df = df.merge(df_load, left_on=df.primary_key, right_on=df_load.primary_key)
 
     # Set formatters
     df["kspace"].formatters = TensorFormatterGroup().defer()
     df["maps"].formatters = TensorFormatterGroup().defer()
     if "target" in df:
         df["target"].formatters = TensorFormatterGroup().defer()
     return df
```

### Comparing `meddlr-viz-0.0.1/setup.cfg` & `meddlr-viz-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `meddlr-viz-0.0.1/setup.py` & `meddlr-viz-0.0.2/setup.py`

 * *Files identical despite different names*

